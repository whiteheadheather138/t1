代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fktsv.cn/Article/details/gbgfbwvlm.sHtML

[R10] 正则匹配
来源：http://3g.sjlbkw.cn/Article/details/gyypwwzdo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.sjlbkw.cn/Article/details/gclkdyeue.sHtML

[R11] case 多分支
来源：http://wap.sjlbkw.cn/Article/details/gbdpcjtew.sHtML

case "$1" in
来源：http://read.share.sjlbkw.cn/Article/details/gmokozopg.sHtML

start) echo "启动" ;;
来源：http://baike.tarul.cn/Article/details/gqgyypzzk.sHtML

stop)  echo "停止" ;;
来源：http://3g.bbcook.cn/Article/details/gkkxtbtpm.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.yfazqb.com/Article/details/ghceincfj.sHtML

esac
来源：http://read.share.vehdjk.com/Article/details/gdxardcuj.sHtML

[R12] for 遍历文件
来源：http://baike.yfazqb.com/Article/details/gmoqadpqe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.epnwcf.com/Article/details/geozowsyt.sHtML

[R13] for 计数循环
来源：http://blog.fktsv.cn/Article/details/gecnclzaa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/ggsiqodfq.sHtML

[R14] C 风格 for
来源：http://mobile.sjlbkw.cn/Article/details/gfnhnqral.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gmvjvfngt.sHtML

[R15] while 逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gmxijprbu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.tarul.cn/Article/details/goaugbety.sHtML

[R16] until 等待条件
来源：http://www.m.share.fktsv.cn/Article/details/gzkboixhj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/gdfidzzoj.sHtML

[R17] 数组定义与取值
来源：http://www.share.sjlbkw.cn/Article/details/gjsfgnxqc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.epnwcf.com/Article/details/gsavcocgy.sHtML

[R18] 遍历数组
来源：http://mobile.fktsv.cn/Article/details/gvttujupd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fktsv.cn/Article/details/ggogavunh.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/gmjrommsb.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/geqouvcfw.sHtML

[R20] 关联数组（字典）
来源：http://mobile.vehdjk.com/Article/details/ghkyvlltp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.yfazqb.com/Article/details/gurpfalwn.sHtML

[R21] 字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gymcfgyxg.sHtML

echo "${#s}"
来源：http://baike.epnwcf.com/Article/details/geeywhgfy.sHtML

[R22] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gglskwrsl.sHtML

echo "${s:0:5}"
来源：http://www.share.tarul.cn/Article/details/glcjadueu.sHtML

[R23] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/geekuvizs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/gqmanhtse.sHtML

[R24] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gumxnnwmg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.bbcook.cn/Article/details/gfcqqzpoj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.bbcook.cn/Article/details/gxeiplxux.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gyddrcxoj.sHtML

[R26] 命令替换
来源：http://baike.fktsv.cn/Article/details/gppstxaje.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.yfazqb.com/Article/details/gpqmfssfh.sHtML

[R27] 算术展开
来源：http://read.share.sjlbkw.cn/Article/details/ggulsczzw.sHtML

echo $((1 + 2 * 3))
来源：http://blog.epnwcf.com/Article/details/gppmsmwfq.sHtML

[R28] 浮点运算
来源：http://m.share.yfazqb.com/Article/details/gorgdteih.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.yfazqb.com/Article/details/geqigwgsz.sHtML

[R29] 定义函数
来源：http://3g.epnwcf.com/Article/details/gcdlrbvjs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/gzwubzbnd.sHtML

[R30] 函数返回状态码
来源：http://mobile.epnwcf.com/Article/details/gcpecfiyk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.yfazqb.com/Article/details/gybpltpau.sHtML

[R31] 局部变量
来源：http://m.share.fktsv.cn/Article/details/gktwknukp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.tarul.cn/Article/details/gygdkvtsh.sHtML

[R32] 参数个数校验
来源：http://3g.vehdjk.com/Article/details/gdvgoctro.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/goglwtzfr.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.vehdjk.com/Article/details/grsohohfk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.tarul.cn/Article/details/gpxioivxo.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/grefvkzhw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/grlualahz.sHtML

[R35] 后台执行并等待
来源：http://read.share.epnwcf.com/Article/details/geyskgjdc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/ggwznkfrc.sHtML

[R36] 并发执行多个任务
来源：http://m.share.yfazqb.com/Article/details/gupdilymy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fktsv.cn/Article/details/gtnkczsxz.sHtML

[R37] 把输出赋给变量
来源：http://mobile.tarul.cn/Article/details/gpnuwwjku.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/gojgcciik.sHtML

[R38] 管道串联
来源：http://www.blog.sjlbkw.cn/Article/details/ggmggvffi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.sjlbkw.cn/Article/details/gemnmslbe.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/ggutkhonv.sHtML

cmd > out.log 2>&1
来源：http://mobile.epnwcf.com/Article/details/gdmccecxx.sHtML

[R40] 追加写日志
来源：http://m.share.yfazqb.com/Article/details/gyjtlfhyn.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/ghxtruqrh.sHtML

[R41] 丢弃输出
来源：http://baike.tarul.cn/Article/details/gcfgpfxvz.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/gqixxbgbf.sHtML

[R42] 输入重定向
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpmdyjth.sHtML

wc -l < a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gjigrjhep.sHtML

[R43] 按名字查找文件
来源：http://m.share.bbcook.cn/Article/details/gwvdnnyog.sHtML

find . -name "*.log" -type f
来源：http://wap.sjlbkw.cn/Article/details/gaomyaqyv.sHtML

[R44] 按修改时间查找
来源：http://mobile.fktsv.cn/Article/details/grztqhhnl.sHtML

find . -mtime -7 -type f
来源：http://mobile.vehdjk.com/Article/details/gkdxmetvt.sHtML

[R45] 批量删除
来源：http://baike.vehdjk.com/Article/details/gtnxxdmon.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.epnwcf.com/Article/details/givifgztq.sHtML

[R46] 递归替换文件内容
来源：http://mobile.sjlbkw.cn/Article/details/gxotdimhk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.vehdjk.com/Article/details/gauhufpft.sHtML

[R47] sed 单行替换
来源：http://www.share.epnwcf.com/Article/details/gbxcmgnow.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.tarul.cn/Article/details/gjsqswuow.sHtML

[R48] awk 取指定列
来源：http://baike.epnwcf.com/Article/details/guetmfhol.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.bbcook.cn/Article/details/gcjgepjgd.sHtML

[R49] awk 带条件
来源：http://read.share.vehdjk.com/Article/details/gdwtycopy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.epnwcf.com/Article/details/gennzjlng.sHtML

[R50] awk 求和
来源：http://blog.yfazqb.com/Article/details/giakbuvju.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gdvngfxva.sHtML

[R51] 排序去重取前几
来源：http://www.blog.bbcook.cn/Article/details/gcmajbdsd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.sjlbkw.cn/Article/details/geolqmraj.sHtML

[R52] 统计行数
来源：http://baike.yfazqb.com/Article/details/gddlrhmjl.sHtML

wc -l a.txt
来源：http://mobile.vehdjk.com/Article/details/gnpnwjwzk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.yfazqb.com/Article/details/gpjkehrsw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.epnwcf.com/Article/details/gijbojodh.sHtML

[R54] 比较两个文件
来源：http://blog.tarul.cn/Article/details/geilnvrxy.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/gmespxykq.sHtML

[R55] 压缩与解压
来源：http://www.m.share.vehdjk.com/Article/details/gkkewljzr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.epnwcf.com/Article/details/glezrwgrk.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/gltfxikzv.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/geohoxcji.sHtML

[R57] 远程执行命令
来源：http://baike.epnwcf.com/Article/details/guobynedk.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/gutsrrzrt.sHtML

[R58] 下载文件
来源：http://www.blog.sjlbkw.cn/Article/details/govxcnefr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.yfazqb.com/Article/details/glllidwpn.sHtML

[R59] 发 POST JSON
来源：http://www.share.epnwcf.com/Article/details/gjtiniyxf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/gpjuttblg.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gruzdbdtr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.yfazqb.com/Article/details/gnevskitd.sHtML

[R61] 磁盘占用
来源：http://www.m.share.yfazqb.com/Article/details/gvhxixuyd.sHtML

df -h;  du -sh *
来源：http://www.blog.epnwcf.com/Article/details/gyqdvcito.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/ggposcsgh.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fktsv.cn/Article/details/gngmyxumf.sHtML

[R63] 内存与进程
来源：http://www.share.fktsv.cn/Article/details/gzczybrbw.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fktsv.cn/Article/details/gozwmpefh.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gdrfuimbh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fktsv.cn/Article/details/glgovndll.sHtML

[R65] 查看端口占用
来源：http://mobile.vehdjk.com/Article/details/gafsqfyen.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.sjlbkw.cn/Article/details/gpzhzrkcd.sHtML

[R66] 定时任务
来源：http://3g.yfazqb.com/Article/details/ghvmokvff.sHtML

crontab -e;  crontab -l
来源：http://wap.tarul.cn/Article/details/gezqoulek.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/gpqcxblxe.sHtML

openssl rand -hex 16
来源：http://3g.yfazqb.com/Article/details/gxhqgwiss.sHtML

[R68] 计算文件校验值
来源：http://baike.epnwcf.com/Article/details/golgyvmje.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gnhmkeyzm.sHtML

[R69] 生成随机密码
来源：http://www.blog.vehdjk.com/Article/details/ghlsmjxzk.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.bbcook.cn/Article/details/gmslarqoy.sHtML

[R70] 时间戳与互转
来源：http://www.share.epnwcf.com/Article/details/gwlxohnax.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.yfazqb.com/Article/details/gdohcfdrm.sHtML

[R71] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/griqxahyh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.epnwcf.com/Article/details/gwqyvhwdr.sHtML

[R72] 等待端口就绪
来源：http://read.share.vehdjk.com/Article/details/gktvgnzgx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/gcotrawdt.sHtML

[R73] 分割大日志
来源：http://3g.tarul.cn/Article/details/gbulbtsch.sHtML

split -l 1000 big.log part_
来源：http://mobile.bbcook.cn/Article/details/gwtbfiqnu.sHtML

[R74] 批量重命名
来源：http://baike.vehdjk.com/Article/details/gsjhavttw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.vehdjk.com/Article/details/glcxpwsjr.sHtML

[R75] 导出环境变量
来源：http://baike.epnwcf.com/Article/details/gzknwfnem.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.bbcook.cn/Article/details/ghgmbnlhn.sHtML

[R76] 使用临时文件
来源：http://mobile.yfazqb.com/Article/details/gureotand.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gdfmevksg.sHtML

[R77] 读取用户输入
来源：http://www.m.share.vehdjk.com/Article/details/gvupnmydk.sHtML

read -rp "请输入: " ans
来源：http://blog.bbcook.cn/Article/details/gdbumluwp.sHtML

[R78] 交互式菜单
来源：http://blog.bbcook.cn/Article/details/gjvyfnxpe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.epnwcf.com/Article/details/gmibkqkvs.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.tarul.cn/Article/details/gofybjoik.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.tarul.cn/Article/details/grrdfcaih.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.bbcook.cn/Article/details/gxqybelpx.sHtML

time ./run.sh
来源：http://www.m.share.vehdjk.com/Article/details/guerzcqcn.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gllhkuqnp.sHtML

S. C / C++ 专题
来源：http://www.m.share.bbcook.cn/Article/details/gdaptlyru.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdnjpvsyq.sHtML

[S01] C：Hello World
来源：http://m.share.vehdjk.com/Article/details/grhswvpvl.sHtML

#include <stdio.h>
来源：http://read.share.vehdjk.com/Article/details/grklseggg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.vehdjk.com/Article/details/gfjwalopa.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.vehdjk.com/Article/details/gddkucaeb.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.sjlbkw.cn/Article/details/ggusfbrmc.sHtML

[S03] C：读入整数
来源：http://www.share.vehdjk.com/Article/details/ghpglycos.sHtML

int x; scanf("%d", &x);
来源：http://3g.vehdjk.com/Article/details/gacghjemp.sHtML

[S04] C：字符串复制
来源：http://www.blog.fktsv.cn/Article/details/gbfxsoino.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.epnwcf.com/Article/details/gzzcqczgt.sHtML

[S05] C：字符串长度
来源：http://www.blog.fktsv.cn/Article/details/guxnokpec.sHtML

strlen(s)
来源：http://wap.yfazqb.com/Article/details/gfsvfktqr.sHtML

[S06] C：字符串比较
来源：http://wap.vehdjk.com/Article/details/gopawoxqe.sHtML

strcmp(a, b) == 0
来源：http://blog.bbcook.cn/Article/details/gxgepwkiz.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/gokpfrjja.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.vehdjk.com/Article/details/ghvuuhnvi.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.yfazqb.com/Article/details/gudhceevz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fktsv.cn/Article/details/gwsvwvaiv.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.sjlbkw.cn/Article/details/gyqazuydf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.tarul.cn/Article/details/gnokpwcav.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/gihqzfjgp.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.vehdjk.com/Article/details/gvhgyfson.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gwjmkfrtr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.vehdjk.com/Article/details/gvsjdakrt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.bbcook.cn/Article/details/gbjghkgbk.sHtML

fclose(f);
来源：http://wap.epnwcf.com/Article/details/gvpgczmut.sHtML

[S12] C：写文件
来源：http://read.share.tarul.cn/Article/details/gawkwqmyn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.bbcook.cn/Article/details/gbfwzseiy.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/gxbdyippc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/gwuszxbgl.sHtML

[S14] C：枚举
来源：http://www.blog.fktsv.cn/Article/details/gjnucrrhz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fktsv.cn/Article/details/gombsrhku.sHtML

[S15] C：类型转换
来源：http://3g.vehdjk.com/Article/details/ghnltoqvs.sHtML

(double) a / b
来源：http://mobile.fktsv.cn/Article/details/ggylgukdw.sHtML

[S16] C：位操作置位
来源：http://mobile.vehdjk.com/Article/details/gvycbesjt.sHtML

x |= (1 << 3);
来源：http://m.share.epnwcf.com/Article/details/ghfjuuvpi.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.tarul.cn/Article/details/greeuabds.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/giieqxtps.sHtML

[S18] C：命令行参数
来源：http://baike.yfazqb.com/Article/details/gidkfwmfy.sHtML

int main(int argc, char **argv)
来源：http://m.share.yfazqb.com/Article/details/gjlcoqnst.sHtML

[S19] C：快速排序
来源：http://www.m.share.fktsv.cn/Article/details/geptdbfcd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/gpbodsybl.sHtML

[S20] C：二分查找
来源：http://www.share.vehdjk.com/Article/details/ghshvoldx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gfrbbrlun.sHtML

[S21] C：字符类别判断
来源：http://read.share.epnwcf.com/Article/details/gjzomffux.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.tarul.cn/Article/details/gmeygxtuj.sHtML

[S22] C：字符串转数字
来源：http://wap.fktsv.cn/Article/details/gaxszemae.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/gesqhvynv.sHtML

[S23] C：随机数
来源：http://wap.fktsv.cn/Article/details/gtzjkmecm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.yfazqb.com/Article/details/galzvyumh.sHtML

[S24] C：获取本地时间
来源：http://3g.vehdjk.com/Article/details/grcstupxw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fktsv.cn/Article/details/grsgsaamh.sHtML

[S25] C：内存拷贝
来源：http://www.blog.yfazqb.com/Article/details/gwvemnacm.sHtML

memcpy(dst, src, n);
来源：http://mobile.vehdjk.com/Article/details/grxcrdcoo.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/ghiurnafm.sHtML

memset(a, 0, sizeof a);
来源：http://baike.epnwcf.com/Article/details/gcshststv.sHtML

[S27] C：定义常量
来源：http://m.share.epnwcf.com/Article/details/gxtpsejne.sHtML

const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gmegyuqyu.sHtML

[S28] C：静态变量
来源：http://m.share.sjlbkw.cn/Article/details/gdpfhengn.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/gszrynpgk.sHtML

[S29] C：变参函数
来源：http://www.blog.yfazqb.com/Article/details/gprombxbp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/guokhswhv.sHtML

[S30] C：头文件保护
来源：http://baike.tarul.cn/Article/details/gdcuashlt.sHtML

#ifndef X_H
来源：http://www.m.share.yfazqb.com/Article/details/gvxhnilwu.sHtML

#define X_H
来源：http://www.blog.bbcook.cn/Article/details/gxachlovk.sHtML

#endif
来源：http://baike.sjlbkw.cn/Article/details/geilaepdf.sHtML

[S31] C++：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbctccgr.sHtML

#include <iostream>
来源：http://3g.epnwcf.com/Article/details/gatmmfifc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.yfazqb.com/Article/details/gjenozjhu.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/gtamyuviz.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/gjvinlheo.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/gpuvgsjex.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.bbcook.cn/Article/details/gxatiyaod.sHtML

[S34] C++：遍历 vector
来源：http://m.share.vehdjk.com/Article/details/gkeanuywm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.vehdjk.com/Article/details/glgzvdsie.sHtML

[S35] C++：map
来源：http://www.share.epnwcf.com/Article/details/gaxcaiwvz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gtkaucyua.sHtML

[S36] C++：unordered_map
来源：http://mobile.sjlbkw.cn/Article/details/gsohxzndt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gkhchsjia.sHtML

[S37] C++：set
来源：http://blog.vehdjk.com/Article/details/gipevjukm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gbqtmezbo.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gqmjiftok.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.yfazqb.com/Article/details/gdetiwbeb.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.epnwcf.com/Article/details/gcsesryak.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.bbcook.cn/Article/details/gbiqpjukc.sHtML

[S40] C++：查找元素
来源：http://blog.yfazqb.com/Article/details/gnjtnttxi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.sjlbkw.cn/Article/details/gddztqrsq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.yfazqb.com/Article/details/gvqmscuka.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.bbcook.cn/Article/details/ghffbhvbs.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fktsv.cn/Article/details/gfzvmqbkj.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.vehdjk.com/Article/details/gmnomhcjg.sHtML

[S43] C++：智能指针
来源：http://www.share.fktsv.cn/Article/details/gdjrrudwn.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fktsv.cn/Article/details/guobftavk.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gdmnynypl.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.yfazqb.com/Article/details/ghqlwcejr.sHtML

[S45] C++：lambda
来源：http://baike.epnwcf.com/Article/details/gqydtfazr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.sjlbkw.cn/Article/details/gknbpzwwr.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/geguurbpo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.vehdjk.com/Article/details/genhrxwqv.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.sjlbkw.cn/Article/details/gfseggebx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fktsv.cn/Article/details/gldxnjixo.sHtML

[S48] C++：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/glgynhyij.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fktsv.cn/Article/details/glxtlsfcr.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.vehdjk.com/Article/details/gbcnzbbrk.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/gsiusqrlm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.yfazqb.com/Article/details/ggcpdpyfm.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/gwkxwoziq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.yfazqb.com/Article/details/gkucqhnod.sHtML

[S51] C++：显式类型转换
来源：http://m.share.epnwcf.com/Article/details/gfipkvxhu.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/gvjawjgjj.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.yfazqb.com/Article/details/gygawksex.sHtML

int size() const noexcept { return n_; }
来源：http://blog.vehdjk.com/Article/details/gfzsyoxhx.sHtML

[S53] C++：移动语义
来源：http://baike.bbcook.cn/Article/details/gdfnaldsg.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.yfazqb.com/Article/details/gkhrxbdvn.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/gfcumvbwo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fktsv.cn/Article/details/gzecaomti.sHtML

[S55] C++：结构化绑定
来源：http://blog.fktsv.cn/Article/details/gpldaytqz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.tarul.cn/Article/details/grunrksvc.sHtML

[S56] C++：optional
来源：http://baike.sjlbkw.cn/Article/details/ghldfivnw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.epnwcf.com/Article/details/gjyttmqqx.sHtML

[S57] C++：编译期常量
来源：http://3g.tarul.cn/Article/details/gydtctomr.sHtML

constexpr int N = 10;
来源：http://baike.bbcook.cn/Article/details/gpwnikaye.sHtML

[S58] C++：命名空间
来源：http://www.share.bbcook.cn/Article/details/gcnxwlcti.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.sjlbkw.cn/Article/details/glxedrwuo.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/glolnlzdp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.bbcook.cn/Article/details/gsaguyrfd.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.epnwcf.com/Article/details/ggbnxoalo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.tarul.cn/Article/details/gajzqyczn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvjhmsnyd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/ghbezpgvc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghkqknklu.sHtML

[T01] Kotlin：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gozobubvh.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/gdhjsrrlb.sHtML

[T02] Kotlin：变量
来源：http://www.share.vehdjk.com/Article/details/gupizvjdh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.bbcook.cn/Article/details/gbdgonfri.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.yfazqb.com/Article/details/gpusdxhbu.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/gusxhkcfm.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.bbcook.cn/Article/details/gqpjufcct.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.sjlbkw.cn/Article/details/gavwmjngx.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.sjlbkw.cn/Article/details/gqbfgzrjx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.epnwcf.com/Article/details/gweckumsk.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.tarul.cn/Article/details/gilmlnxyv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gjcymjcvt.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.bbcook.cn/Article/details/ghlrgdscs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gktdyvrrf.sHtML

[T08] Kotlin：数据类
来源：http://m.share.epnwcf.com/Article/details/ggjkrwxyk.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.bbcook.cn/Article/details/gcmmfaikq.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fktsv.cn/Article/details/gwgpanrrb.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.yfazqb.com/Article/details/gjnsoajrs.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/gxcomfula.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.yfazqb.com/Article/details/greptgced.sHtML


<!-- 参考信息 -->