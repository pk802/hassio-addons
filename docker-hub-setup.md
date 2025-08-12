# Docker Hub Setup for pk802/go2rtc

## Current Status
- Your add-on config now uses: `image: pk802/go2rtc`
- This should pass Home Assistant's regex validation
- But the image needs to be published to Docker Hub

## Quick Test Steps:
1. Wait 2-3 minutes for repository update
2. In Home Assistant: Remove and re-add repository
3. Check Supervisor logs for validation errors

## If validation passes but image not found:
You'll need to publish to Docker Hub:

1. Create Docker Hub account: https://hub.docker.com
2. Get your username (should be pk802)
3. Create repository: pk802/go2rtc
4. Update GitHub Actions to push to Docker Hub

## Alternative: Use existing working image temporarily
Change config.yaml to:
```yaml
image: alexxit/go2rtc
```
This will make the add-on work immediately for testing.
