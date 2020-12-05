Commands
========

The Makefile contains the central entry points for common tasks related to this project.

Syncing data to S3
^^^^^^^^^^^^^^^^^^

* `make sync_data_to_gcs` will use `gsutil rsync` to recursively sync files in `data/` up to `gs://{{ cookiecutter.gcs_bucket }}/data/`.
* `make sync_data_from_gcs` will use `gsutil rsync` to recursively sync files from `gs://{{ cookiecutter.gcs_bucket }}/data/` to `data/`.
