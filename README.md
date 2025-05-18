---
# - name: Download frontend image
#   community.docker.docker_image:
#     name: "{{ image_name }}"
#     tag: "{{ image_tag}}"
#     build:
#       path: "{{ fronted_path }}"

# - name: Ensures The container is running
#   community.docker.docker_container:
#     name: "{{ frontend_1 }}"
#     image: "{{ image_name }}"
#     state: started
#     ports:
      # - "5000": "5000"