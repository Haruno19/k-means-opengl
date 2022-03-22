# k-means-opengl
K-Means clustering algorithm implementation in C++ with GLFW3 OpenGL.

Outputs an animated graphical simulation of the clustering algorithm.  
You can input the number of Data Points and Clusters at the start of the program.
  
## How it works
Data Points and Clusters are stored in linked lists and dynamically allocated.  
Each point is identified by its coordinates (randomly generated); the algorithm is simulated by attaching each Data Point to one Cluster based on their coordinates, the Cluster is then moved at the center of its attached Data Points. These two operations are iterated until no Cluster is moving between one step and the other, meaning every Cluster has reached a stable position and each Data Point is attached to the "right" Cluster. 

---

###### Sample outputs (stable state)

<table>
  <tr>
      <td>
          <img src="https://user-images.githubusercontent.com/61376940/159467427-38e016c3-3a70-4d1d-b341-e32c59de6259.png" width="500">
          10000 Data Points and 10 Clusters
      </td>
      <td>
          <img src="https://user-images.githubusercontent.com/61376940/159467430-43f58630-aa85-45b3-81c8-38d6edda335b.png" width="500">
          1000 Data Points and 9 Clusters
      </td>
      <td>
          <img src="https://user-images.githubusercontent.com/61376940/159467435-1cdca329-da09-4cc6-b090-95debae9edd0.png" width="500">
          2000 Data Points and 12 Clusters
    </td>
  </tr>
</table>
