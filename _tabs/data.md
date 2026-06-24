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

        <div id="upload-status" class="alert d-none mb-0 small" role="alert"></div>
      </div>
    </div>
  </div>

  <!-- 설정 카드 -->
  <div class="col-lg-5">
    <div class="card border-0 shadow-sm h-100 card-custom">
      <div class="card-body d-flex flex-column justify-content-between">
        <div>
          <h5 class="card-title mb-3"><i class="fas fa-key text-success me-2"></i>GitHub 업로드 인증</h5>
          
          <div class="mb-3">
            <label for="gitToken" class="form-label small mb-1 fw-semibold">Personal Access Token (PAT)</label>
            <input type="password" class="form-control form-control-sm" id="gitToken" placeholder="ghp_xxxxxxxxxxxx">
            <div class="form-text x-small text-muted">
              GitHub Token은 브라우저 로컬 저장소에만 안전하게 저장됩니다. 
              <a href="https://github.com/settings/tokens/new?scopes=repo" target="_blank" class="text-primary text-decoration-none fw-semibold">토큰 발급받기 <i class="fas fa-external-link-alt"></i></a>
            </div>
          </div>
        </div>

        <div>
          <!-- 고급 설정 (접기/펴기) -->
          <div class="accordion accordion-flush" id="advancedAccordion">
            <div class="accordion-item bg-transparent">
              <h2 class="accordion-header" id="headingAdvanced">
                <button class="accordion-button collapsed py-2 px-0 bg-transparent small text-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#collapseAdvanced" aria-expanded="false" aria-controls="collapseAdvanced">
                  고급 설정 (저장소 설정)
                </button>
              </h2>
              <div id="collapseAdvanced" class="accordion-collapse collapse" aria-labelledby="headingAdvanced" data-bs-parent="#advancedAccordion">
                <div class="accordion-body px-0 py-2">
                  <div class="mb-2">
                    <label for="gitOwner" class="form-label small mb-1">Owner (계정명)</label>
                    <input type="text" class="form-control form-control-sm" id="gitOwner" value="masteritpe">
                  </div>
                  <div class="mb-2">
                    <label for="gitRepo" class="form-label small mb-1">Repository (저장소명)</label>
                    <input type="text" class="form-control form-control-sm" id="gitRepo" value="masteritpe.github.io">
                  </div>
                  <div class="mb-2">
                    <label for="gitBranch" class="form-label small mb-1">Branch (브랜치)</label>
                    <input type="text" class="form-control form-control-sm" id="gitBranch" value="master">
                  </div>
                </div>
              </div>
            </div>
          </div>
          <button type="button" class="btn btn-sm btn-primary w-100 mt-2" id="save-settings-btn">설정 저장</button>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- 자료실 목록 영역 -->
<h3 class="border-bottom pb-2 mb-3"><i class="fas fa-list text-warning me-2"></i>자료실 파일 목록</h3>
{% assign data_files = site.static_files | where_exp: "file", "file.relative_path contains '_data/'" %}

{% if data_files.size == 0 %}
  <div class="text-center my-4 py-4 text-muted border rounded bg-light bg-opacity-10">
    <i class="fas fa-info-circle fa-2x mb-2 text-secondary"></i>
    <p class="mb-0">등록된 파일이 없습니다.</p>
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
  /* Accordion styles inside Bootstrap */
  .accordion-button::after {
    filter: var(--accordion-icon-filter, none);
  }
  [data-theme="dark"] .accordion-button::after {
    filter: invert(1) grayscale(1);
  }
</style>

<script>
document.addEventListener('DOMContentLoaded', function() {
  // GitHub Settings Defaults
  const DEFAULT_OWNER = 'masteritpe';
  const DEFAULT_REPO = 'masteritpe.github.io';
  const DEFAULT_BRANCH = 'master';

  // Load Elements
  const dropZone = document.getElementById('drop-zone');
  const fileInput = document.getElementById('file-input');
  const uploadStatus = document.getElementById('upload-status');
  
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
    const owner = gitOwner.value.trim();
    const repo = gitRepo.value.trim();
    const branch = gitBranch.value.trim();
    const token = gitToken.value.trim();

    if (!owner || !repo || !branch || !token) {
      showStatus('<strong>오류:</strong> GitHub 연동 설정에 토큰(PAT)을 입력하고 저장해 주세요.', 'danger');
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
          message: `Upload ${file.name} to _data via Web UI`,
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
          showStatus(`<strong>성공:</strong> '${file.name}' 파일이 GitHub 저장소의 <code>_data/</code> 폴더에 업로드(커밋)되었습니다.<br><small class="text-secondary">GitHub Action 빌드 완료 후 목록에 나타납니다. (약 1~2분 소요)</small>`, 'success');
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
  }

  // Initialize
  loadSettings();
});
</script>
