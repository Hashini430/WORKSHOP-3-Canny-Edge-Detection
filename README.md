# Canny Edge Detection using OpenCV

## Python Code

```python
import cv2
import matplotlib.pyplot as plt

img = cv2.imread('hash.jpg', cv2.IMREAD_GRAYSCALE)

blurred = cv2.GaussianBlur(img, (5, 5), 0)

edges = cv2.Canny(blurred, 50, 150)

plt.figure(figsize=(10, 5))

plt.subplot(121)
plt.imshow(img, cmap='gray')
plt.title('Original Image')
plt.axis('off')

plt.subplot(122)
plt.imshow(edges, cmap='gray')
plt.title('Detected Edges')
plt.axis('off')

plt.show()
```
## Output
<img width="945" height="530" alt="image" src="https://github.com/user-attachments/assets/e42df80c-885e-43bd-9359-c156babf7b87" />
