all: refresh-po

refresh-po:
	intltool-update --pot --gettext-package=comps

report:
	for cat in *.po; do \
		echo -n "$$cat: "; \
		msgfmt -v --statistics -o /dev/null $$cat; \
	done
