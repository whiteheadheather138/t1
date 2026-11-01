代发 wailian999

case "$1" in
来源：http://m.share.yfazqb.com/Article/details/gosryijdj.sHtML

start) echo "启动" ;;
来源：http://blog.fktsv.cn/Article/details/gnntzibfd.sHtML

stop)  echo "停止" ;;
来源：http://blog.fktsv.cn/Article/details/gwfiihplb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.tarul.cn/Article/details/gxpeqhlml.sHtML

esac
来源：http://www.share.epnwcf.com/Article/details/gyjjiuzlb.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/glsnyagyt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fktsv.cn/Article/details/guqmovodr.sHtML

[R13] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gnfmrmtoz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/grcjmjymx.sHtML

[R14] C 风格 for
来源：http://3g.sjlbkw.cn/Article/details/gbrnloubd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/grxxewbce.sHtML

[R15] while 逐行读文件
来源：http://wap.fktsv.cn/Article/details/gctbjqoyn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.vehdjk.com/Article/details/gwkzvyocg.sHtML

[R16] until 等待条件
来源：http://3g.epnwcf.com/Article/details/gwehdszzr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/grtsnatnx.sHtML

[R17] 数组定义与取值
来源：http://www.blog.sjlbkw.cn/Article/details/gkrrvxate.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.yfazqb.com/Article/details/gjvchanda.sHtML

[R18] 遍历数组
来源：http://read.share.yfazqb.com/Article/details/gtaqeoiit.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fktsv.cn/Article/details/gzkwpookn.sHtML

[R19] 数组长度
来源：http://3g.bbcook.cn/Article/details/gnqwhmqnt.sHtML

echo "${#arr[@]}"
来源：http://www.share.tarul.cn/Article/details/guvoqrrfv.sHtML

[R20] 关联数组（字典）
来源：http://m.share.vehdjk.com/Article/details/gmfkojzrv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.epnwcf.com/Article/details/gubppzhti.sHtML

[R21] 字符串长度
来源：http://wap.epnwcf.com/Article/details/gfxnjtebr.sHtML

echo "${#s}"
来源：http://blog.bbcook.cn/Article/details/gugnfnbvf.sHtML

[R22] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gdnlglbsr.sHtML

echo "${s:0:5}"
来源：http://www.share.fktsv.cn/Article/details/givjhsyog.sHtML

[R23] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gtxrbzdky.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fktsv.cn/Article/details/gqeirbjbh.sHtML

[R24] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gcyqmevcx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.vehdjk.com/Article/details/gbjonbolm.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.vehdjk.com/Article/details/gqdnrokjs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.bbcook.cn/Article/details/gncryvfcj.sHtML

[R26] 命令替换
来源：http://www.m.share.vehdjk.com/Article/details/glhilyovm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.yfazqb.com/Article/details/gmlcsqamc.sHtML

[R27] 算术展开
来源：http://mobile.sjlbkw.cn/Article/details/gyivrdchv.sHtML

echo $((1 + 2 * 3))
来源：http://wap.epnwcf.com/Article/details/gzcglpond.sHtML

[R28] 浮点运算
来源：http://www.blog.bbcook.cn/Article/details/gmfewsyxa.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/geggczfib.sHtML

[R29] 定义函数
来源：http://www.blog.tarul.cn/Article/details/gnswhklmo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.yfazqb.com/Article/details/grhuzifhz.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.bbcook.cn/Article/details/giiviotac.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fktsv.cn/Article/details/gvwmbkmwx.sHtML

[R31] 局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/gdvmqhnvi.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.yfazqb.com/Article/details/gqmcrxjkt.sHtML

[R32] 参数个数校验
来源：http://www.share.yfazqb.com/Article/details/grsthnnwm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.epnwcf.com/Article/details/gkkqzcpnb.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.tarul.cn/Article/details/gaqqbinpp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.vehdjk.com/Article/details/giimwrxln.sHtML

[R34] 退出时清理
来源：http://m.share.fktsv.cn/Article/details/gkdosibul.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gsfwvyuwm.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.tarul.cn/Article/details/gibzmdzkd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.epnwcf.com/Article/details/gpzykbkgc.sHtML

[R36] 并发执行多个任务
来源：http://3g.bbcook.cn/Article/details/gafqrbcjx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.vehdjk.com/Article/details/gptjbelcp.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/gzsybwnhg.sHtML

files=$(ls -1)
来源：http://read.share.sjlbkw.cn/Article/details/grvybwkrq.sHtML

[R38] 管道串联
来源：http://m.share.fktsv.cn/Article/details/gyqnqrmlm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fktsv.cn/Article/details/gvmxrksyp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.yfazqb.com/Article/details/gvihyalcn.sHtML

cmd > out.log 2>&1
来源：http://www.blog.yfazqb.com/Article/details/goknrbyyn.sHtML

[R40] 追加写日志
来源：http://3g.fktsv.cn/Article/details/gvmmzdkog.sHtML

echo "log" >> out.log
来源：http://read.share.sjlbkw.cn/Article/details/gnhbjbqnu.sHtML

[R41] 丢弃输出
来源：http://m.share.epnwcf.com/Article/details/gntisbdio.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/gssqqgaba.sHtML

[R42] 输入重定向
来源：http://www.blog.epnwcf.com/Article/details/gmyqmvykt.sHtML

wc -l < a.txt
来源：http://baike.vehdjk.com/Article/details/gvxtlzixf.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwrngupw.sHtML

find . -name "*.log" -type f
来源：http://read.share.yfazqb.com/Article/details/gdwrcqaaq.sHtML

[R44] 按修改时间查找
来源：http://mobile.yfazqb.com/Article/details/gcxupfojb.sHtML

find . -mtime -7 -type f
来源：http://read.share.yfazqb.com/Article/details/gwgdwpycg.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gyvpojmsd.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.tarul.cn/Article/details/grzriapmw.sHtML

[R46] 递归替换文件内容
来源：http://wap.bbcook.cn/Article/details/gdidthleq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.bbcook.cn/Article/details/gyvrvyerj.sHtML

[R47] sed 单行替换
来源：http://www.blog.sjlbkw.cn/Article/details/gqhfueuap.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.yfazqb.com/Article/details/gqtvtloic.sHtML

[R48] awk 取指定列
来源：http://mobile.yfazqb.com/Article/details/gzrmubhas.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.tarul.cn/Article/details/gsetqiuqi.sHtML

[R49] awk 带条件
来源：http://www.share.sjlbkw.cn/Article/details/givukdcmy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.yfazqb.com/Article/details/gzaxfadrm.sHtML

[R50] awk 求和
来源：http://blog.yfazqb.com/Article/details/gfiguhvka.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gnwpdhoix.sHtML

[R51] 排序去重取前几
来源：http://mobile.epnwcf.com/Article/details/gdnhcdlyb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.epnwcf.com/Article/details/gjnxqdqik.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/gthwniheo.sHtML

wc -l a.txt
来源：http://www.share.bbcook.cn/Article/details/gdzqtizis.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/gcewhrvsp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.bbcook.cn/Article/details/gcczkjyaq.sHtML

[R54] 比较两个文件
来源：http://mobile.epnwcf.com/Article/details/gyxasewwq.sHtML

diff a.txt b.txt
来源：http://3g.sjlbkw.cn/Article/details/gkygcczfg.sHtML

[R55] 压缩与解压
来源：http://read.share.vehdjk.com/Article/details/gxvxjfkdw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fktsv.cn/Article/details/ghrjnmvxn.sHtML

[R56] 远程拷贝
来源：http://mobile.bbcook.cn/Article/details/gwmsrqljq.sHtML

scp file user@host:/path/
来源：http://blog.tarul.cn/Article/details/gvvdlodpy.sHtML

[R57] 远程执行命令
来源：http://blog.fktsv.cn/Article/details/grabtyrvz.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fktsv.cn/Article/details/gmccaapsv.sHtML

[R58] 下载文件
来源：http://www.blog.yfazqb.com/Article/details/gmlekkdyz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/gvxzvifhm.sHtML

[R59] 发 POST JSON
来源：http://mobile.bbcook.cn/Article/details/gniigjkow.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/gqlbgwvpy.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/goitmgvqo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/gmzkcaagu.sHtML

[R61] 磁盘占用
来源：http://www.share.sjlbkw.cn/Article/details/gxirytrfs.sHtML

df -h;  du -sh *
来源：http://www.blog.fktsv.cn/Article/details/gyxaqlbbb.sHtML

[R62] 找最占空间的文件
来源：http://wap.tarul.cn/Article/details/gpgyrhytm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fktsv.cn/Article/details/gkhjhepiv.sHtML

[R63] 内存与进程
来源：http://3g.sjlbkw.cn/Article/details/gtuuqmsuv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fktsv.cn/Article/details/gmvdsvqrz.sHtML

[R64] 结束进程
来源：http://www.m.share.fktsv.cn/Article/details/gvdogdfzy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.epnwcf.com/Article/details/gvcprhyig.sHtML

[R65] 查看端口占用
来源：http://www.share.yfazqb.com/Article/details/gwzcqrtxi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.tarul.cn/Article/details/gdjgrxbaf.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/gjaxfygvs.sHtML

crontab -e;  crontab -l
来源：http://wap.epnwcf.com/Article/details/glbnjuuhu.sHtML

[R67] 生成随机十六进制串
来源：http://baike.sjlbkw.cn/Article/details/ggzoleaax.sHtML

openssl rand -hex 16
来源：http://www.blog.vehdjk.com/Article/details/gwkrxfrvk.sHtML

[R68] 计算文件校验值
来源：http://baike.vehdjk.com/Article/details/gnlhqmcwz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.epnwcf.com/Article/details/gnasfjpbi.sHtML

[R69] 生成随机密码
来源：http://baike.bbcook.cn/Article/details/gmcjdfvnt.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.tarul.cn/Article/details/gaypqxlig.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/gyjoepxkb.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fktsv.cn/Article/details/gfbhojmkt.sHtML

[R71] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gyzycsnpj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.yfazqb.com/Article/details/gjhanwmer.sHtML

[R72] 等待端口就绪
来源：http://read.share.vehdjk.com/Article/details/gxqcnkghv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gecnnwdiq.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/gtihqbfws.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/gqavlrugh.sHtML

[R74] 批量重命名
来源：http://baike.bbcook.cn/Article/details/gcphsrkjp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.bbcook.cn/Article/details/gwjfiaxqm.sHtML

[R75] 导出环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gzwfjbzxj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/gywijceaz.sHtML

[R76] 使用临时文件
来源：http://www.m.share.yfazqb.com/Article/details/gstookfia.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/gqibewvex.sHtML

[R77] 读取用户输入
来源：http://m.share.vehdjk.com/Article/details/gjmhguuiq.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/ghluwbnxw.sHtML

[R78] 交互式菜单
来源：http://blog.fktsv.cn/Article/details/grmlcvezp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.vehdjk.com/Article/details/ghvutixff.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/gibbxqbko.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.vehdjk.com/Article/details/gblylzpfb.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fktsv.cn/Article/details/gzhjxdyzo.sHtML

time ./run.sh
来源：http://wap.fktsv.cn/Article/details/girkxyccf.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gfuvzdahb.sHtML

S. C / C++ 专题
来源：http://www.m.share.fktsv.cn/Article/details/gootnvogg.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gndyzejdw.sHtML

[S01] C：Hello World
来源：http://read.share.epnwcf.com/Article/details/gstbkqpyj.sHtML

#include <stdio.h>
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuwziyqx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.tarul.cn/Article/details/gyquvigxg.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gnvacpicl.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fktsv.cn/Article/details/gqrdbimza.sHtML

[S03] C：读入整数
来源：http://wap.fktsv.cn/Article/details/gisibvypt.sHtML

int x; scanf("%d", &x);
来源：http://mobile.vehdjk.com/Article/details/gdijioihf.sHtML

[S04] C：字符串复制
来源：http://www.blog.tarul.cn/Article/details/gqibwznyu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/gtvkurejq.sHtML

[S05] C：字符串长度
来源：http://blog.yfazqb.com/Article/details/grdlnwsip.sHtML

strlen(s)
来源：http://3g.bbcook.cn/Article/details/grhgwlloz.sHtML

[S06] C：字符串比较
来源：http://m.share.bbcook.cn/Article/details/gobkdatsy.sHtML

strcmp(a, b) == 0
来源：http://m.share.bbcook.cn/Article/details/gqcqmukcb.sHtML

[S07] C：数组遍历求和
来源：http://mobile.yfazqb.com/Article/details/gqhslxccd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/gjlbxvdyw.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.yfazqb.com/Article/details/gzbqaybzi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fktsv.cn/Article/details/garbwrpvb.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.tarul.cn/Article/details/ghebbjhbv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.epnwcf.com/Article/details/gidtpfvfg.sHtML

[S10] C：指针与解引用
来源：http://www.blog.tarul.cn/Article/details/gdcdczmfr.sHtML

int *p = &a;  *p = 5;
来源：http://3g.bbcook.cn/Article/details/gituuglyb.sHtML

[S11] C：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gmrnysxci.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.epnwcf.com/Article/details/gsqhbxsij.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fktsv.cn/Article/details/gobydzkqx.sHtML

fclose(f);
来源：http://blog.fktsv.cn/Article/details/glkdqqocc.sHtML

[S12] C：写文件
来源：http://www.share.tarul.cn/Article/details/gteedrfkp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gngxcvdsu.sHtML

[S13] C：宏定义
来源：http://www.m.share.epnwcf.com/Article/details/ghurrxdvi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gtludhhpi.sHtML

[S14] C：枚举
来源：http://mobile.tarul.cn/Article/details/gpxdjbpib.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.yfazqb.com/Article/details/gapswfhdu.sHtML

[S15] C：类型转换
来源：http://3g.epnwcf.com/Article/details/gzsutbyak.sHtML

(double) a / b
来源：http://www.blog.tarul.cn/Article/details/gyaqlcfmn.sHtML

[S16] C：位操作置位
来源：http://m.share.yfazqb.com/Article/details/gsvngpabv.sHtML

x |= (1 << 3);
来源：http://3g.fktsv.cn/Article/details/gqbwmgcvy.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gutpduuhh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.sjlbkw.cn/Article/details/gmkaltnhy.sHtML

[S18] C：命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gyeevrnpi.sHtML

int main(int argc, char **argv)
来源：http://3g.epnwcf.com/Article/details/gbkqgjvwr.sHtML

[S19] C：快速排序
来源：http://mobile.sjlbkw.cn/Article/details/gqpclneur.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gaviyxblh.sHtML

[S20] C：二分查找
来源：http://www.blog.sjlbkw.cn/Article/details/gzgqmhpsn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/grkgpxrnc.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fktsv.cn/Article/details/gzmtdhkzc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/gscqcytee.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtajqxwk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/gwygsyeml.sHtML

[S23] C：随机数
来源：http://m.share.epnwcf.com/Article/details/gnvobquka.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.tarul.cn/Article/details/gseifoxpr.sHtML

[S24] C：获取本地时间
来源：http://www.blog.epnwcf.com/Article/details/gnnmcdfhq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/gcvjxannx.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gndgpyhkq.sHtML

memcpy(dst, src, n);
来源：http://baike.sjlbkw.cn/Article/details/gxpoarrag.sHtML

[S26] C：内存清零
来源：http://blog.tarul.cn/Article/details/gpzqgqvfm.sHtML

memset(a, 0, sizeof a);
来源：http://baike.sjlbkw.cn/Article/details/gibukgtpv.sHtML

[S27] C：定义常量
来源：http://wap.tarul.cn/Article/details/gpasnbdui.sHtML

const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gcdjvmocu.sHtML

[S28] C：静态变量
来源：http://www.share.tarul.cn/Article/details/ghdhrzetg.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/gmglswreo.sHtML

[S29] C：变参函数
来源：http://mobile.fktsv.cn/Article/details/goplrvzns.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/gavghvhaa.sHtML

[S30] C：头文件保护
来源：http://www.m.share.tarul.cn/Article/details/gpvugfbkl.sHtML

#ifndef X_H
来源：http://read.share.fktsv.cn/Article/details/guzrkicei.sHtML

#define X_H
来源：http://www.m.share.bbcook.cn/Article/details/gcjdydfdz.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/gyijpxzew.sHtML

[S31] C++：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gvpxulsam.sHtML

#include <iostream>
来源：http://mobile.bbcook.cn/Article/details/gnuizemwx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/gamulmwem.sHtML

[S32] C++：字符串
来源：http://3g.tarul.cn/Article/details/gqylhgnua.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.vehdjk.com/Article/details/gytrwhkpu.sHtML

[S33] C++：vector 增删
来源：http://www.blog.yfazqb.com/Article/details/gxosynnsv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.tarul.cn/Article/details/gesdpnsdw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.epnwcf.com/Article/details/gozqneonw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gccxjqjiw.sHtML

[S35] C++：map
来源：http://blog.epnwcf.com/Article/details/gbwmdbwfi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/guuoknhld.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.tarul.cn/Article/details/gehdxzaqx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gokkdfoxv.sHtML

[S37] C++：set
来源：http://m.share.bbcook.cn/Article/details/gcapcowmq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/glogpinvw.sHtML

[S38] C++：排序
来源：http://blog.epnwcf.com/Article/details/gvkcypzkl.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.epnwcf.com/Article/details/guqwmwkdz.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fktsv.cn/Article/details/ghijsadfp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.yfazqb.com/Article/details/gioeordit.sHtML

[S40] C++：查找元素
来源：http://m.share.fktsv.cn/Article/details/guqfqjtfx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.vehdjk.com/Article/details/grnxvazgo.sHtML

[S41] C++：类与构造函数
来源：http://wap.vehdjk.com/Article/details/gjjuzgpxi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.sjlbkw.cn/Article/details/ggvhwuyfr.sHtML

[S42] C++：继承与虚函数
来源：http://3g.yfazqb.com/Article/details/gvjkzzprt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.vehdjk.com/Article/details/gccjnzufw.sHtML

[S43] C++：智能指针
来源：http://www.share.epnwcf.com/Article/details/gmejdhaeu.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.epnwcf.com/Article/details/gztsughqq.sHtML

[S44] C++：引用传参
来源：http://www.blog.tarul.cn/Article/details/gyevndudf.sHtML

void inc(int &x) { ++x; }
来源：http://3g.yfazqb.com/Article/details/gxmgkjtxg.sHtML

[S45] C++：lambda
来源：http://wap.epnwcf.com/Article/details/gmmzwpmyi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/gijllavqq.sHtML

[S46] C++：函数模板
来源：http://mobile.tarul.cn/Article/details/gzwpnblcp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.tarul.cn/Article/details/gbnptpqha.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.tarul.cn/Article/details/gugbfsghq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.yfazqb.com/Article/details/gwknzjmga.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gskkqbxlb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.sjlbkw.cn/Article/details/gypfkhblj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.bbcook.cn/Article/details/gkgjqhpqo.sHtML

[S49] C++：写文件
来源：http://www.share.epnwcf.com/Article/details/gvhceuhjr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/guhgbtboi.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fktsv.cn/Article/details/gaqjhtotb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.tarul.cn/Article/details/ggcfixwfd.sHtML

[S51] C++：显式类型转换
来源：http://blog.vehdjk.com/Article/details/glqlqtfky.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fktsv.cn/Article/details/gbgjictus.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.epnwcf.com/Article/details/gctlltand.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.vehdjk.com/Article/details/gbgwwjlvr.sHtML

[S53] C++：移动语义
来源：http://wap.tarul.cn/Article/details/gshrexsmx.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fktsv.cn/Article/details/gnzzzutko.sHtML

[S54] C++：异常处理
来源：http://mobile.vehdjk.com/Article/details/gnjcnkbvo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/glfvhztlx.sHtML

[S55] C++：结构化绑定
来源：http://3g.fktsv.cn/Article/details/gicjkvnbp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fktsv.cn/Article/details/gejqxbatg.sHtML

[S56] C++：optional
来源：http://mobile.fktsv.cn/Article/details/gtcpwjiyi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.vehdjk.com/Article/details/ghnufljkx.sHtML

[S57] C++：编译期常量
来源：http://read.share.yfazqb.com/Article/details/gkqobjryj.sHtML

constexpr int N = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gqnbmnflo.sHtML

[S58] C++：命名空间
来源：http://3g.tarul.cn/Article/details/gbgkobdel.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.yfazqb.com/Article/details/gyewiqmfk.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fktsv.cn/Article/details/gccvvnezh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/gbgaeosbv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.bbcook.cn/Article/details/gdrfywtql.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.yfazqb.com/Article/details/gxyagconr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnzwkmeyq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.epnwcf.com/Article/details/ghgwuxhke.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/glssltsqk.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fktsv.cn/Article/details/gdndajcpj.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gyiljdpij.sHtML

[T02] Kotlin：变量
来源：http://mobile.sjlbkw.cn/Article/details/gmqyjqzlw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.epnwcf.com/Article/details/gpcdwnyrw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/gynrwhrks.sHtML

"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gwypleufc.sHtML

[T04] Kotlin：空安全
来源：http://read.share.bbcook.cn/Article/details/glbsyswdb.sHtML

val n: String? = null;  n?.length
来源：http://read.share.vehdjk.com/Article/details/ggsrqzyqh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.yfazqb.com/Article/details/gollipsva.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.tarul.cn/Article/details/gmpinlwey.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/gtrghnyqq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gbfhayngm.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.epnwcf.com/Article/details/gevysufoy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.tarul.cn/Article/details/gwhebhbaf.sHtML

[T08] Kotlin：数据类
来源：http://3g.bbcook.cn/Article/details/grltkkhvn.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.vehdjk.com/Article/details/gcuomngjt.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.vehdjk.com/Article/details/gxafmuedb.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/gbsaxjpph.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.tarul.cn/Article/details/gkjfpuufm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.sjlbkw.cn/Article/details/gvveummln.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/gzjorcawg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.epnwcf.com/Article/details/gixnbnoki.sHtML

[T12] Kotlin：解构声明
来源：http://blog.tarul.cn/Article/details/gidnrrdkk.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.yfazqb.com/Article/details/geyiqtvzj.sHtML


<!-- 参考信息 -->