# Phase 3 — Image Prompts: Thỏ Làm Bánh Phô Mai Cháy Basque

Phim đã duyệt 31/10/2026. Phase 3 theo master prompt ChefVision AI, đã chuyển thể sang Anime.
Mỗi cảnh là 1 khối JSON riêng, không gộp. Thứ tự và số cảnh giữ nguyên Phase 2.

## Character Sheet tham chiếu (làm trước khi dùng 8 prompt dưới)
Dùng prompt này để khóa mặt thỏ trước khi render cảnh. Mô tả thỏ dưới đây là bản tạm chốt cho Phase 3 — nếu thỏ gốc của kênh cũ khác màu lông, mũ, tạp dề thì báo em sửa sheet này trước khi render, đừng render cảnh với sheet sai.

```
Character reference sheet, four views on a plain neutral grey background: [1] full body front view, [2] full body rear view, [3] head-and-shoulders front close-up, [4] head-and-shoulders left profile. The same anime bunny chef with cream-white fur, long upright ears with pink inner ears, large round expressive eyes, small pink nose, wearing a white chef hat and a beige apron over a light shirt. Consistent face, ears, proportions and outfit across all four views. Locked style: anime style, large expressive eyes, strong emotional acting, cinematic colours, clean outlines. Keep this exact style in every image and every shot. No 3D, no Pixar look, no photorealism. No text, no watermark, no extra characters, no background environment.
```

## Cảnh 1

```json
{
  "scene_number": 1,
  "shot_type": "Overhead top-down",
  "subject": "Anime bunny chef with cream-white fur, long upright ears with pink inner ears, white chef hat and beige apron, gently pressing crinkled parchment paper into a round brushed-metal springform pan, both paws holding the paper edges, paper folds naturally around the pan rim",
  "background": "Rustic dark oak wooden table, warm morning studio lighting, warm Anime kitchen",
  "aesthetic": "Anime style, large expressive eyes, cinematic colours, clean outlines, high-detail food textures, warm appetizing colours. No 3D, no Pixar look, no photorealism",
  "aspect_ratio": "9:16"
}
```

## Cảnh 2

```json
{
  "scene_number": 2,
  "shot_type": "45-degree close-up",
  "subject": "Anime bunny chef with cream-white fur, long upright ears with pink inner ears, white chef hat and beige apron, whisking cream cheese and sugar in a bowl, mixture turning from thick to smooth and glossy, whisk lifting a soft glossy ribbon of cream cheese",
  "background": "Rustic dark oak wooden table, warm morning studio lighting, warm Anime kitchen",
  "aesthetic": "Anime style, large expressive eyes, cinematic colours, clean outlines, high-detail food textures, warm appetizing colours. No 3D, no Pixar look, no photorealism",
  "aspect_ratio": "9:16"
}
```

## Cảnh 3

```json
{
  "scene_number": 3,
  "shot_type": "Overhead top-down",
  "subject": "Anime bunny chef with cream-white fur, long upright ears with pink inner ears, white chef hat and beige apron, pouring eggs and fresh cream in a slow thick stream into the cream cheese bowl, liquid streams merging smoothly, glossy surface with small ripples",
  "background": "Rustic dark oak wooden table, warm morning studio lighting, warm Anime kitchen",
  "aesthetic": "Anime style, large expressive eyes, cinematic colours, clean outlines, high-detail food textures, warm appetizing colours. No 3D, no Pixar look, no photorealism",
  "aspect_ratio": "9:16"
}
```

## Cảnh 4

```json
{
  "scene_number": 4,
  "shot_type": "Overhead top-down",
  "subject": "Anime bunny chef with cream-white fur, long upright ears with pink inner ears, white chef hat and beige apron, sifting fine flour over the batter with a small sieve, a few drops of vanilla beside the bowl, gently stirring with a spatula, flour falling like fine dust",
  "background": "Rustic dark oak wooden table, warm morning studio lighting, warm Anime kitchen",
  "aesthetic": "Anime style, large expressive eyes, cinematic colours, clean outlines, high-detail food textures, warm appetizing colours. No 3D, no Pixar look, no photorealism",
  "aspect_ratio": "9:16"
}
```

## Cảnh 5

```json
{
  "scene_number": 5,
  "shot_type": "Overhead top-down",
  "subject": "Anime bunny chef with cream-white fur, long upright ears with pink inner ears, white chef hat and beige apron, pouring the smooth thick batter into the parchment-lined brushed-metal springform pan, tapping the pan lightly, batter surface flat, glossy and bubble-free",
  "background": "Rustic dark oak wooden table, warm morning studio lighting, warm Anime kitchen",
  "aesthetic": "Anime style, large expressive eyes, cinematic colours, clean outlines, high-detail food textures, warm appetizing colours. No 3D, no Pixar look, no photorealism",
  "aspect_ratio": "9:16"
}
```

## Cảnh 6

```json
{
  "scene_number": 6,
  "shot_type": "45-degree close-up",
  "subject": "Anime bunny chef with cream-white fur, long upright ears with pink inner ears, white chef hat and beige apron, sliding the filled brushed-metal springform pan into a warm oven, oven door half open, warm golden oven light glowing inside",
  "background": "Rustic dark oak wooden table, warm morning studio lighting, warm Anime kitchen",
  "aesthetic": "Anime style, large expressive eyes, cinematic colours, clean outlines, high-detail food textures, warm appetizing colours. No 3D, no Pixar look, no photorealism",
  "aspect_ratio": "9:16"
}
```

## Cảnh 7

```json
{
  "scene_number": 7,
  "shot_type": "45-degree close-up",
  "subject": "Anime bunny chef with cream-white fur, long upright ears with pink inner ears, white chef hat and beige apron, opening the oven to reveal a Basque burnt cheesecake with a deep golden-brown burnt top, puffed surface gently jiggling, warm steam rising, same brushed-metal springform pan as previous scenes",
  "background": "Rustic dark oak wooden table, warm morning studio lighting, warm Anime kitchen",
  "aesthetic": "Anime style, large expressive eyes, cinematic colours, clean outlines, high-detail food textures, warm appetizing colours. No 3D, no Pixar look, no photorealism",
  "aspect_ratio": "9:16"
}
```

## Cảnh 8

```json
{
  "scene_number": 8,
  "shot_type": "45-degree close-up",
  "subject": "Anime bunny chef with cream-white fur, long upright ears with pink inner ears, white chef hat and beige apron, smiling softly while slicing the Basque burnt cheesecake, soft molten centre flowing slowly, a spoon lifting the first creamy bite, golden-brown top and pale creamy interior clearly visible",
  "background": "Rustic dark oak wooden table, warm morning studio lighting, warm Anime kitchen",
  "aesthetic": "Anime style, large expressive eyes, cinematic colours, clean outlines, high-detail food textures, warm appetizing colours. No 3D, no Pixar look, no photorealism",
  "aspect_ratio": "9:16"
}
```

## Phase Gate
Hỏi TinTin: 8 prompt trên ổn chưa, hay muốn sửa chi tiết nào trước khi làm Phase 4 (video motion prompts)? Không tự chuyển sang Phase 4 khi chưa có duyệt.
