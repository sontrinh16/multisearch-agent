# multisearch-agent

#1 REFLEX AGENT
Hàm reflex agent trả về giá trị điểm dựa trên khoảng cách của pacman với ma và với thức ăn. Khoảng cách tới chấm thức ăn càng xa thì điểm càng nhỏ và ngược. Đối với con ma thì điểm sẽ là giá trị âm thế nên càng xa thì giá trị âm càng nhỏ. Chúng ta tính toán khoảng cách tương đối giữa pacman và ma và giữa pacman và thức ăn và cộng lại hai giá trị để ra điểm.


#2 MINIMAX AGENT
Nhận vào độ sâu của cây và trạng thái game hiện tại. Tại mỗi tầng của cây có pacman và con ma (lấy bằng hàm getNumAgents). Với mỗi trạng thái, các hành động có thể thực hiện nằm ở các nút con của nó. Gía trị min và max được tính một cách đệ quy với giá trị min max đã tính trước.(pacman là maxval, ghost là minval). Gía trị ở lá là điểm.


#3 ALPHA-BETA AGENT
Có hàm hỗ trợ alphabeta tính các giá trị alpha cho pacman và beta cho ma. Lá trả về điểm. Nếu là một nút min thì sẽ update giá trị beta nếu nó lớn hơn giá trị nút min, và ngược lại với nút max. Khi alpha lớn hơn beta ta sẽ tỉa nhánh. Trả về đường đi sử dụng alpha-beta để thắng.
