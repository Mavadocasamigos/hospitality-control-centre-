# hospitality-control-centre-
commanding centre for hospitality activities 
import shutil, os

src = "/mnt/data/Nabuuma_Recipe_Control_MVP_v3_11_extracted"
out = "/mnt/data/Nabuuma_Recipe_Control_MVP_v3_11_SHAREABLE.zip"

shutil.make_archive(
    base_name=out[:-4],
    format="zip",
    root_dir=src
)

size_mb = os.path.getsize(out) / (1024 * 1024)
print(f"Created: {out}")
print(f"Size: {size_mb:.2f} MB")
