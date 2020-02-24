company-capfnb
================
No blocked company backend for `completion-at-point` function, forked from [`company-cafp`](https://github.com/company-mode/company-mode/blob/master/company-capf.el)

# Installation
Using [`quelpa`](https://github.com/quelpa/quelpa) and [`use-package`](https://github.com/jwiegley/use-package)

``` elisp
(use-package company-capfnb
  :quelpa (company-capfnb :fetcher github :repo "kiennq/company-capf-noblock")
  :after company
  :config
  ;; Replace company-capf
  (setf (car (assq 'company-capf company-backends)) 'company-capfnb))
```
