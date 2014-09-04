# Deploy Items from S3

## Requirements

None.

### Role Variables

vailable variables are listed below, along with default values (see `defaults/main.yml`):

    owner: 
      owner: owner of the files and directories
      group: group owner of the file
      aws_access_key:
      aws_secret_key:
      bucket_name:
      app_dirs: list of app directories
      payloads: dictionary of the object, dest, and path for the tarball

## Dependencies

None

## Notes

Add support for alternative notificatiosn methods
