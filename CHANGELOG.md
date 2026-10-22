# Changelog

All notable changes to this project are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [10.0.0] - 2026-07-07

### Added

- Initial release: an educational Django platform for students and educators.
- Exam and competition analysis with visual dashboards and statistical reports.
- An educational blog with categories and slug-addressed article pages.
- A review and feedback system, and a competition management admin panel.
- User accounts through `django-allauth`, with Google and Microsoft sign-in.
- Jalali (Persian) calendar support through `jdatetime` and `jalali_core`.

### Changed

- Moved the project from the `edu/` subdirectory to the repository root and
  removed the desktop-app (PyQt) references — the project is web-only.
