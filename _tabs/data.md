---
layout: page
title: 자료실
icon: fas fa-database
order: 5
---

> **자료실**: `_data` 폴더에 업로드된 백업 및 데이터 파일 목록입니다. 클릭하시면 파일을 직접 다운로드하실 수 있습니다.
{: .prompt-info }

{% assign data_files = site.static_files | where_exp: "file", "file.relative_path contains '_data/'" %}

{% if data_files.size == 0 %}
  <div class="text-center my-5 py-5 text-muted">
    <i class="fas fa-folder-open fa-3x mb-3 text-secondary"></i>
    <p>등록된 데이터 파일이 없습니다.</p>
  </div>
{% else %}
  <div class="row g-3">
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

  <style>
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
    /* Theme dark mode compatibility */
    [data-theme="dark"] .card-data-download {
      background-color: #1e1e1e !important;
      border-color: #2e2e2e !important;
    }
    [data-theme="dark"] .icon-wrapper {
      background-color: #2b2b2b !important;
    }
    [data-theme="dark"] .card-title {
      color: #e0e0e0 !important;
    }
  </style>
{% endif %}
