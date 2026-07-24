# ZenLeader — zenleader-protocol

GitHub: [`silentlamp/zenleader-protocol`](https://github.com/silentlamp/zenleader-protocol)  
Former name: `silentlamp/plugnmeet-protocol` (GitHub redirects).

Standalone protocol/protobuf package for ZenLeader Meet.

## Remotes & forks

- Remote: chỉ `origin` → `https://github.com/silentlamp/zenleader-protocol.git`
- **Không** sync / merge / so sánh với `mynaparrot/plugnmeet-protocol`

## Go / JS module paths (quan trọng cho CI)

Meet server CI (`zenleader-meet-server` Docker build) vẫn resolve dependency:

```text
github.com/mynaparrot/plugnmeet-protocol v1.4.0
```

qua Go module proxy (tag đã publish). **Không** đổi `go.mod` module path khi chỉ rename GitHub repo — đổi path Go sẽ phá import + CI nếu chưa republish.

Local workspace folder có thể vẫn tên `plugnmeet-protocol`; GitHub repo name là `zenleader-protocol`.

## Deploy

Repo này **không** có workflow deploy VPS riêng. Artifact dùng gián tiếp khi build `silentlamp/zenleader-meet-server` / client.
