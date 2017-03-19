# helm-myR.el
This package provides two functions, `helm-for-R` and `helm-R-install-packages`.
This package is inspired by helm-R (https://github.com/myuhe/helm-R.el)

## helm-for-R
By using this function, you can see help of R functions and the structure of local object through helm interface.

## helm-R-install-packages
By using this gunction, you can choose an R package in CRAN mirror in Japan( https://cran.ism.ac.jp ).

# key-bindings
You can use any key-bindings to use these functions. For example,

```elisp
(require 'helm-myR)
(define-key ess-mode-map (kbd "C-c h") 'helm-for-R)
(define-key inferior-ess-mode-map (kbd "C-c h") 'helm-for-R)

(define-key ess-mode-map (kbd "A-h") 'helm-R-install-packages)
(define-key inferior-ess-mode-map (kbd "A-h") 'helm-R-install-packages)
```
