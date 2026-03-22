source "https://rubygems.org"

gem "jekyll", "~> 4.4.1"

# Тема
gem "minimal-mistakes-jekyll", "~> 4.27"
# ДОБАВЬ ЭТУ СТРОКУ НИЖЕ:
gem "jekyll-remote-theme" 

# Плагины
group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-paginate"
  gem "jekyll-sitemap"
  gem "jekyll-seo-tag"
  # И ЗДЕСЬ ТОЖЕ МОЖНО ДУБЛИРОВАТЬ ДЛЯ ВЕРНОСТИ:
  gem "jekyll-remote-theme"
end

# Windows поддержка (оставляй как есть)
platforms :mingw, :x64_mingw, :mswin do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
  gem "wdm", "~> 0.1"
end