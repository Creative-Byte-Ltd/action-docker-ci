## Use the Action

```yaml
- name: Use Docker Build and Push Composite Action
  uses: Creative-Byte-Ltd/action-docker-ci@dev
  with:
    dockerhub-username: ${{ secrets.DOCKERHUB_USERNAME }}
    dockerhub-token: ${{ secrets.DOCKERHUB_TOKEN }}
    repository-name: ${{ github.event.repository.name }}
    environment: ${{ env.ENVIRONMENT }}
    github-token: ${{ secrets.GITHUB_TOKEN }}
