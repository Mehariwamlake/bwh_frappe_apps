docker build \
 --build-arg=FRAPPE_PATH=https://github.com/frappe/frappe \
 --build-arg=FRAPPE_BRANCH=develop \
 --build-arg=PYTHON_VERSION=3.11.9 \
 --build-arg= NODE_VERSION=20.9.0 \
 --build-arg=APPS_JSON_BASE64=$APPS_JSON_BASE64 \
 --tag=ghcr.io/mehariwamlake/bwh_frappe_apps/custom:0.0.1 \
 --file=images/layered/Containerfile .