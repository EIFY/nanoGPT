See the [original repo](https://github.com/karpathy/nanoGPT) for detailed instructions and context. [🦁 Lion - Pytorch implementation](https://github.com/lucidrains/lion-pytorch) courtesy of [lucidrains](https://github.com/lucidrains).

[<img width="1620" alt="Screenshot 2023-02-23 at 3 24 13 PM" src="https://user-images.githubusercontent.com/2584418/221054034-3a6f6d05-85ac-459e-8954-9c2f2066f04f.png">](https://wandb.ai/eify/owt/reports/train-loss-23-02-23-15-24-50---VmlldzozNjMxMjIz?accessToken=2etw7nk0dj51v1urev0rnm3bfs8fr0zrydd7b958iold78k5pp1sn2r5msw84zcc)

[<img width="1617" alt="Screenshot 2023-02-23 at 3 26 10 PM" src="https://user-images.githubusercontent.com/2584418/221054292-319a0f14-784c-4a63-9e6a-dea462dcab1c.png">](https://api.wandb.ai/links/eify/vo80u6yq)

[<img width="1619" alt="Screenshot 2023-02-23 at 3 27 15 PM" src="https://user-images.githubusercontent.com/2584418/221054432-aec8274c-1eff-411d-b5a3-dcf604f8840f.png">](https://api.wandb.ai/links/eify/qjo5hhfl)

[<img width="1614" alt="Screenshot 2023-02-23 at 3 28 12 PM" src="https://user-images.githubusercontent.com/2584418/221054539-ff5aac34-bf17-4a91-9cdb-b14e815f10da.png">](https://wandb.ai/eify/owt/reports/Process-GPU-Time-Spent-Accessing-Memory-23-02-23-15-28-29---VmlldzozNjMxMjM2?accessToken=h468tckn3cuf9v1rxqjy9ckmzxsv0664wnzwum6kjualp6pic397ip3d7biubczl)

So 🦁 is definitely better than AdamW: lower loss and higher iter/s, but somehow (fused) AdamW burns less power and spends less time accessing memory, presumably thanks to the highly-optimized fused kernel...?
