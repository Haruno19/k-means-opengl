# k-means-opengl
#### 09.2020
K-Means clustering algorithm simulation in C++ with GLFW3 OpenGL.

The output is an animated graphical simulation of the K-means clustering algorithm on a set of randomly generated clusters and data points.
The user can input the number of Data Points and Clusters at the start of the program, and then run the simulation.
  
## How it works
**Data Points** and **Clusters** are stored in separate linked lists and are dynamically allocated.  
Each point is initially positioned in the plane at **randomly generated coordinates**; the algorithm is simulated by attaching each **Data Point** to one **Cluster** based on their coordinates, the **Cluste**r is then moved at the center of its attached **Data Points**. These two operations are then iterated until no **Cluster** is moving between one interation and the next, meaning that every **Cluster** has reached a *stable position* and each **Data Point** is attached to its "correct" **Cluster**. 

---

###### Sample outputs *(stable state)*

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
