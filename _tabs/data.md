---
layout: page
title: 자료실
icon: fas fa-database
order: 5
---

> **자료실**: `_data` 폴더에 업로드된 백업 및 데이터 파일 목록입니다. 클릭하시면 파일을 직접 다운로드하실 수 있습니다.
{: .prompt-info }

<!-- 업로드 및 설정 패널 -->
<div class="row g-3 mb-4">
  <!-- 파일 업로드 카드 -->
  <div class="col-lg-7">
    <div class="card border-0 shadow-sm h-100 card-custom">
      <div class="card-body">
        <h5 class="card-title mb-3"><i class="fas fa-upload text-primary me-2"></i>파일 업로드</h5>
        
        <div id="drop-zone" class="drop-zone mb-3 d-flex flex-column align-items-center justify-content-center border border-dashed rounded p-4 text-center">
          <i class="fas fa-cloud-upload-alt fa-3x text-muted mb-2"></i>
          <p class="mb-1 text-secondary">마우스로 파일을 끌어오거나 클릭하여 선택하세요.</p>
          <input type="file" id="file-input" class="d-none">
        </div>
        
        <div class="mb-3">
          <label class="form-label d-block fw-semibold mb-2">업로드 대상 저장소</label>
          <div class="d-flex gap-3">
            <div class="form-check">
              <input class="form-check-input" type="radio" name="uploadTarget" id="targetLocal" value="local" checked>
              <label class="form-check-label" for="targetLocal">
                브라우저 로컬 저장소 (IndexedDB)
              </label>
            </div>
            <div class="form-check">
              <input class="form-check-input" type="radio" name="uploadTarget" id="targetRemote" value="remote">
              <label class="form-check-label" for="targetRemote">
                GitHub 원격 저장소 (_data/)
              </label>
            </div>
          </div>
        </div>

        <div id="upload-status" class="alert d-none mb-0 small" role="alert"></div>
      </div>
    </div>
  </div>

  <!-- 설정 카드 -->
  <div class="col-lg-5">
    <div class="card border-0 shadow-sm h-100 card-custom">
      <div class="card-body">
        <h5 class="card-title mb-3 d-flex justify-content-between align-items-center">
          <span><i class="fas fa-cog text-secondary me-2"></i>GitHub 연동 설정</span>
          <button class="btn btn-sm btn-outline-secondary py-0 px-2" type="button" data-bs-toggle="collapse" data-bs-target="#settingsCollapse" aria-expanded="true" aria-controls="settingsCollapse">
            접기/펴기
          </button>
        </h5>
        
        <div class="collapse show" id="settingsCollapse">
          <div class="mb-2">
            <label for="gitOwner" class="form-label small mb-1">Owner (계정명)</label>
            <input type="text" class="form-control form-control-sm" id="gitOwner" placeholder="예: masteritpe">
          </div>
          <div class="mb-2">
            <label for="gitRepo" class="form-label small mb-1">Repository (저장소명)</label>
            <input type="text" class="form-control form-control-sm" id="gitRepo" placeholder="예: masteritpe.github.io">
          </div>
          <div class="mb-2">
            <label for="gitBranch" class="form-label small mb-1">Branch (브랜치)</label>
            <input type="text" class="form-control form-control-sm" id="gitBranch" placeholder="예: master">
          </div>
          <div class="mb-3">
            <label for="gitToken" class="form-label small mb-1">Personal Access Token (PAT)</label>
            <input type="password" class="form-control form-control-sm" id="gitToken" placeholder="ghp_xxxxxxxxxxxx">
            <div class="form-text x-small text-muted">GitHub Token은 브라우저 로컬 저장소에만 안전하게 저장됩니다. <a href="https://github.com/settings/tokens/new?scopes=repo" target="_blank" class="text-primary text-decoration-none">토큰 만들기 <i class="fas fa-external-link-alt"></i></a></div>
          </div>
          <button type="button" class="btn btn-sm btn-primary w-100" id="save-settings-btn">설정 저장</button>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- 자료실 목록 영역 -->
<h3 class="border-bottom pb-2 mb-3"><i class="fas fa-folder-open text-warning me-2"></i>공동 자료실 (서버 파일)</h3>
{% assign data_files = site.static_files | where_exp: "file", "file.relative_path contains '_data/'" %}

{% if data_files.size == 0 %}
  <div class="text-center my-4 py-4 text-muted border rounded bg-light bg-opacity-10">
    <i class="fas fa-info-circle fa-2x mb-2 text-secondary"></i>
    <p class="mb-0">서버에 등록된 파일이 없습니다.</p>
  </div>
{% else %}
  <div class="row g-3 mb-5">
    {% for file in data_files %}
      <div class="col-md-6">
        <a href="{{ file.url | relative_url }}" download class="text-decoration-none">
          <div class="card h-100 border-0 shadow-sm card-data-download">
            <div class="card-body d-flex align-items-center">
              <div class="flex-shrink-0 me-3">
                <div class="icon-wrapper d-flex align-items-center justify-content-center bg-light rounded" style="width: 48px; height: 48px;">
                  <i class="fas fa-file-alt text-primary fa-lg"></i>
                </div>
              </div>
              <div class="flex-grow-1 min-width-0">
                <h5 class="card-title text-truncate mb-1 text-dark" style="font-size: 1rem; font-weight: 600;">{{ file.name }}</h5>
                <p class="card-text text-muted mb-0 small">
                  {% assign size_kb = file.size | divided_by: 1024 %}
                  {% if size_kb > 1024 %}
                    {% assign size_mb = size_kb | divided_by: 1024.0 | round: 2 %}
                    {{ size_mb }} MB
                  {% else %}
                    {{ size_kb }} KB
                  {% endif %}
                  • {{ file.extname | upcase | replace: '.', '' }} 파일
                </p>
              </div>
              <div class="flex-shrink-0 ms-2">
                <i class="fas fa-download text-muted download-arrow"></i>
              </div>
            </div>
          </div>
        </a>
      </div>
    {% endfor %}
  </div>
{% endif %}

<h3 class="border-bottom pb-2 mb-3 d-flex justify-content-between align-items-center">
  <span><i class="fas fa-hdd text-info me-2"></i>개인 자료실 (로컬 브라우저 Sandbox)</span>
  <span class="badge bg-info rounded-pill fs-7" id="local-count">0개</span>
</h3>
<div class="row g-3 mb-4" id="local-files-container">
  <!-- JavaScript로 렌더링됨 -->
</div>

<style>
  .card-custom {
    background-color: var(--card-bg, #ffffff) !important;
    border: 1px solid var(--card-border-color, #e9ecef) !important;
  }
  .drop-zone {
    cursor: pointer;
    background-color: rgba(var(--bs-primary-rgb), 0.03);
    border-color: var(--card-border-color, #dee2e6) !important;
    transition: background-color 0.2s ease, border-color 0.2s ease;
  }
  .drop-zone:hover, .drop-zone.dragover {
    background-color: rgba(var(--bs-primary-rgb), 0.08);
    border-color: var(--primary, #007bff) !important;
  }
  .card-data-download {
    transition: transform 0.2s ease, box-shadow 0.2s ease;
    background-color: var(--card-bg, #ffffff) !important;
    border: 1px solid var(--card-border-color, #e9ecef) !important;
  }
  .card-data-download:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(0,0,0,0.08) !important;
  }
  .card-data-download:hover .download-arrow {
    color: var(--primary, #007bff) !important;
    transform: scale(1.1);
  }
  .download-arrow {
    transition: color 0.2s ease, transform 0.2s ease;
  }
  .x-small {
    font-size: 0.75rem;
  }
  .fs-7 {
    font-size: 0.8rem;
  }
  .btn-delete-local {
    transition: color 0.2s ease, transform 0.2s ease;
    border: none;
    background: none;
  }
  .btn-delete-local:hover {
    color: #dc3545 !important;
    transform: scale(1.15);
  }
  /* 테마 다크 모드 호환성 */
  [data-theme="dark"] .card-custom,
  [data-theme="dark"] .card-data-download {
    background-color: #1e1e1e !important;
    border-color: #2e2e2e !important;
  }
  [data-theme="dark"] .icon-wrapper {
    background-color: #2b2b2b !important;
  }
  [data-theme="dark"] .card-title,
  [data-theme="dark"] .form-label {
    color: #e0e0e0 !important;
  }
  [data-theme="dark"] .drop-zone {
    background-color: rgba(255, 255, 255, 0.02);
  }
  [data-theme="dark"] .drop-zone:hover,
  [data-theme="dark"] .drop-zone.dragover {
    background-color: rgba(255, 255, 255, 0.05);
  }
  [data-theme="dark"] .form-control {
    background-color: #1a1a1a !important;
    border-color: #2e2e2e !important;
    color: #e0e0e0 !important;
  }
  [data-theme="dark"] .form-control::placeholder {
    color: #666 !important;
  }
</style>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const DB_NAME = 'JekyllDataRoom';
  const DB_VERSION = 1;
  const STORE_NAME = 'uploaded_files';

  // GitHub Settings Defaults
  const DEFAULT_OWNER = 'masteritpe';
  const DEFAULT_REPO = 'masteritpe.github.io';
  const DEFAULT_BRANCH = 'master';

  // Load Elements
  const dropZone = document.getElementById('drop-zone');
  const fileInput = document.getElementById('file-input');
  const uploadStatus = document.getElementById('upload-status');
  const localContainer = document.getElementById('local-files-container');
  const localCount = document.getElementById('local-count');
  
  // Settings Inputs
  const gitOwner = document.getElementById('gitOwner');
  const gitRepo = document.getElementById('gitRepo');
  const gitBranch = document.getElementById('gitBranch');
  const gitToken = document.getElementById('gitToken');
  const saveSettingsBtn = document.getElementById('save-settings-btn');

  // Load Settings from LocalStorage
  function loadSettings() {
    gitOwner.value = localStorage.getItem('git_owner') || DEFAULT_OWNER;
    gitRepo.value = localStorage.getItem('git_repo') || DEFAULT_REPO;
    gitBranch.value = localStorage.getItem('git_branch') || DEFAULT_BRANCH;
    gitToken.value = localStorage.getItem('git_token') || '';
  }

  // Save Settings
  saveSettingsBtn.addEventListener('click', function() {
    localStorage.setItem('git_owner', gitOwner.value.trim());
    localStorage.setItem('git_repo', gitRepo.value.trim());
    localStorage.setItem('git_branch', gitBranch.value.trim());
    localStorage.setItem('git_token', gitToken.value.trim());
    showStatus('설정이 정상적으로 저장되었습니다.', 'success');
  });

  // IndexedDB Helpers
  function getDB() {
    return new Promise((resolve, reject) => {
      const request = indexedDB.open(DB_NAME, DB_VERSION);
      request.onupgradeneeded = (e) => {
        const db = e.target.result;
        if (!db.objectStoreNames.contains(STORE_NAME)) {
          db.createObjectStore(STORE_NAME, { keyPath: 'name' });
        }
      };
      request.onsuccess = (e) => resolve(e.target.result);
      request.onerror = (e) => reject(e.target.error);
    });
  }

  async function saveFileLocal(fileObj) {
    const db = await getDB();
    return new Promise((resolve, reject) => {
      const transaction = db.transaction(STORE_NAME, 'readwrite');
      const store = transaction.objectStore(STORE_NAME);
      const request = store.put(fileObj);
      request.onsuccess = () => resolve();
      request.onerror = (e) => reject(e.target.error);
    });
  }

  async function getLocalFiles() {
    const db = await getDB();
    return new Promise((resolve, reject) => {
      const transaction = db.transaction(STORE_NAME, 'readonly');
      const store = transaction.objectStore(STORE_NAME);
      const request = store.getAll();
      request.onsuccess = (e) => resolve(e.target.result);
      request.onerror = (e) => reject(e.target.error);
    });
  }

  async function deleteLocalFile(name) {
    const db = await getDB();
    return new Promise((resolve, reject) => {
      const transaction = db.transaction(STORE_NAME, 'readwrite');
      const store = transaction.objectStore(STORE_NAME);
      const request = store.delete(name);
      request.onsuccess = () => resolve();
      request.onerror = (e) => reject(e.target.error);
    });
  }

  // Format File Size
  function formatSize(bytes) {
    const kb = bytes / 1024;
    if (kb > 1024) {
      return (kb / 1024).toFixed(2) + ' MB';
    }
    return kb.toFixed(2) + ' KB';
  }

  // Render Local Files
  async function renderLocalFiles() {
    try {
      const files = await getLocalFiles();
      localCount.textContent = `${files.length}개`;
      
      if (files.length === 0) {
        localContainer.innerHTML = `
          <div class="col-12">
            <div class="text-center my-3 py-4 text-muted border rounded bg-light bg-opacity-10">
              <i class="fas fa-hdd fa-2x mb-2 text-secondary"></i>
              <p class="mb-0">로컬 브라우저에 등록된 파일이 없습니다.</p>
            </div>
          </div>
        `;
        return;
      }

      let html = '';
      files.forEach(file => {
        const ext = file.name.split('.').pop().toUpperCase();
        html += `
          <div class="col-md-6" id="local-file-${btoa(encodeURIComponent(file.name)).replace(/=/g, '')}">
            <div class="card h-100 border-0 shadow-sm card-data-download">
              <div class="card-body d-flex align-items-center justify-content-between">
                <a href="${file.dataUrl}" download="${file.name}" class="text-decoration-none flex-grow-1 min-width-0 d-flex align-items-center">
                  <div class="flex-shrink-0 me-3">
                    <div class="icon-wrapper d-flex align-items-center justify-content-center bg-light rounded" style="width: 48px; height: 48px;">
                      <i class="fas fa-file-alt text-info fa-lg"></i>
                    </div>
                  </div>
                  <div class="min-width-0">
                    <h5 class="card-title text-truncate mb-1 text-dark" style="font-size: 1rem; font-weight: 600;">${file.name}</h5>
                    <p class="card-text text-muted mb-0 small">
                      ${formatSize(file.size)} • ${ext} 파일
                    </p>
                  </div>
                </a>
                <div class="flex-shrink-0 ms-2">
                  <button type="button" class="btn btn-link text-muted p-0 btn-delete-local" data-name="${file.name}" title="삭제">
                    <i class="fas fa-trash-alt"></i>
                  </button>
                </div>
              </div>
            </div>
          </div>
        `;
      });
      localContainer.innerHTML = html;

      // Attach Delete Event
      document.querySelectorAll('.btn-delete-local').forEach(btn => {
        btn.addEventListener('click', async function(e) {
          e.preventDefault();
          const name = this.getAttribute('data-name');
          if (confirm(`'${name}' 파일을 로컬 저장소에서 삭제하시겠습니까?`)) {
            await deleteLocalFile(name);
            renderLocalFiles();
            showStatus('파일이 로컬 브라우저에서 제거되었습니다.', 'success');
          }
        });
      });
    } catch (err) {
      console.error(err);
      localContainer.innerHTML = '<div class="col-12"><div class="alert alert-danger">로컬 파일을 불러오는 중 오류가 발생했습니다.</div></div>';
    }
  }

  // Show Alert Status
  function showStatus(message, type) {
    uploadStatus.className = `alert alert-${type} mb-3 small`;
    uploadStatus.innerHTML = message;
    uploadStatus.classList.remove('d-none');
  }

  // Handle Drag & Drop Events
  dropZone.addEventListener('click', () => fileInput.click());
  
  dropZone.addEventListener('dragover', (e) => {
    e.preventDefault();
    dropZone.classList.add('dragover');
  });
  
  dropZone.addEventListener('dragleave', () => {
    dropZone.classList.remove('dragover');
  });
  
  dropZone.addEventListener('drop', (e) => {
    e.preventDefault();
    dropZone.classList.remove('dragover');
    if (e.dataTransfer.files.length > 0) {
      handleFileUpload(e.dataTransfer.files[0]);
    }
  });

  fileInput.addEventListener('change', (e) => {
    if (e.target.files.length > 0) {
      handleFileUpload(e.target.files[0]);
    }
  });

  // Handle Upload
  async function handleFileUpload(file) {
    const isRemote = document.getElementById('targetRemote').checked;
    
    if (isRemote) {
      // Remote GitHub Upload
      const owner = gitOwner.value.trim();
      const repo = gitRepo.value.trim();
      const branch = gitBranch.value.trim();
      const token = gitToken.value.trim();

      if (!owner || !repo || !branch || !token) {
        showStatus('<strong>오류:</strong> GitHub 연동 설정 정보를 모두 입력하고 저장해 주세요. (토큰 필수)', 'danger');
        return;
      }

      showStatus('<i class="fas fa-spinner fa-spin me-2"></i>GitHub에 파일을 전송하는 중입니다...', 'warning');

      try {
        const reader = new FileReader();
        reader.onload = async function() {
          const base64Content = reader.result.split(',')[1];
          const url = `https://api.github.com/repos/${owner}/${repo}/contents/_data/${file.name}`;
          
          let sha = null;
          // Check if file already exists on branch
          try {
            const checkRes = await fetch(url + `?ref=${branch}`, {
              headers: {
                'Authorization': `token ${token}`,
                'Accept': 'application/vnd.github.v3+json'
              }
            });
            if (checkRes.ok) {
              const checkData = await checkRes.json();
              sha = checkData.sha;
            }
          } catch (e) {
            // file doesn't exist
          }

          const body = {
            message: `Upload ${file.name} via Web Data Room`,
            content: base64Content,
            branch: branch
          };
          if (sha) {
            body.sha = sha;
          }

          const uploadRes = await fetch(url, {
            method: 'PUT',
            headers: {
              'Authorization': `token ${token}`,
              'Content-Type': 'application/json',
              'Accept': 'application/vnd.github.v3+json'
            },
            body: JSON.stringify(body)
          });

          if (uploadRes.ok) {
            showStatus(`<strong>성공:</strong> '${file.name}' 파일이 GitHub 저장소에 커밋되었습니다.<br><small class="text-secondary">GitHub Action 빌드 완료 후 목록에 나타납니다. (약 1~2분 소요)</small>`, 'success');
          } else {
            const errData = await uploadRes.json();
            showStatus(`<strong>오류:</strong> GitHub API 전송 실패 (${errData.message})`, 'danger');
          }
        };
        reader.onerror = () => showStatus('파일 읽기 오류가 발생했습니다.', 'danger');
        reader.readAsDataURL(file);
      } catch (err) {
        showStatus(`<strong>오류:</strong> ${err.message}`, 'danger');
      }

    } else {
      // Local IndexedDB Upload
      showStatus('<i class="fas fa-spinner fa-spin me-2"></i>로컬 브라우저에 저장 중...', 'warning');
      
      const reader = new FileReader();
      reader.onload = async function() {
        try {
          const fileObj = {
            name: file.name,
            size: file.size,
            type: file.type,
            dataUrl: reader.result,
            createdAt: new Date().getTime()
          };
          await saveFileLocal(fileObj);
          showStatus(`<strong>성공:</strong> '${file.name}' 파일이 로컬 브라우저 Sandbox에 업로드되었습니다.`, 'success');
          renderLocalFiles();
        } catch (err) {
          showStatus(`<strong>오류:</strong> 로컬 브라우저 저장 실패 (${err.message})`, 'danger');
        }
      };
      reader.onerror = () => showStatus('파일 읽기 오류가 발생했습니다.', 'danger');
      reader.readAsDataURL(file);
    }
  }

  // Initialize
  loadSettings();
  renderLocalFiles();
});
</script>
