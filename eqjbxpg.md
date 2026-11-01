代发 wailian999

name="${1:-default}"
来源：http://blog.epnwcf.com/Article/details/gsyudfsiw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.bbcook.cn/Article/details/gjfpmimvw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gmwgpycca.sHtML

[R07] if 判断文件
来源：http://read.share.tarul.cn/Article/details/gxmdaqjva.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gmaoggswo.sHtML

[R08] 数值比较
来源：http://www.share.bbcook.cn/Article/details/gatraoldq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.yfazqb.com/Article/details/grdedfqqe.sHtML

[R09] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/gftgsimxo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.yfazqb.com/Article/details/gjgyscftx.sHtML

[R10] 正则匹配
来源：http://www.m.share.vehdjk.com/Article/details/gmwdihlea.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.epnwcf.com/Article/details/ghmmsgqzd.sHtML

[R11] case 多分支
来源：http://www.share.tarul.cn/Article/details/gwrjbeorq.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/gllexgumy.sHtML

start) echo "启动" ;;
来源：http://blog.sjlbkw.cn/Article/details/gohmbdugb.sHtML

stop)  echo "停止" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gddrbfuhs.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.yfazqb.com/Article/details/gmcthcxib.sHtML

esac
来源：http://wap.vehdjk.com/Article/details/gqfbsppgu.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gmrvwjqkm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/gfpyobmhx.sHtML

[R13] for 计数循环
来源：http://wap.vehdjk.com/Article/details/ggtoplmit.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gfwiqejka.sHtML

[R14] C 风格 for
来源：http://wap.sjlbkw.cn/Article/details/guwkucjyy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gienoirrx.sHtML

[R15] while 逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/goqadnmic.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.tarul.cn/Article/details/gidymnbet.sHtML

[R16] until 等待条件
来源：http://m.share.vehdjk.com/Article/details/gzjsckpyx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gobfpmpym.sHtML

[R17] 数组定义与取值
来源：http://mobile.tarul.cn/Article/details/gecsctyll.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.tarul.cn/Article/details/gnnxjghqj.sHtML

[R18] 遍历数组
来源：http://read.share.yfazqb.com/Article/details/ghmryifex.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fktsv.cn/Article/details/gorbdngok.sHtML

[R19] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gxwcqbvxi.sHtML

echo "${#arr[@]}"
来源：http://read.share.fktsv.cn/Article/details/gvjoddieo.sHtML

[R20] 关联数组（字典）
来源：http://3g.sjlbkw.cn/Article/details/goalirvod.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.epnwcf.com/Article/details/gmacxslaf.sHtML

[R21] 字符串长度
来源：http://blog.vehdjk.com/Article/details/glnrdwsej.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/gizfpturk.sHtML

[R22] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/gnltuxtzt.sHtML

echo "${s:0:5}"
来源：http://baike.yfazqb.com/Article/details/ggqmbzhfv.sHtML

[R23] 字符串替换
来源：http://read.share.yfazqb.com/Article/details/giyjakaum.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.vehdjk.com/Article/details/gqtjajpon.sHtML

[R24] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gdwttgxjv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.epnwcf.com/Article/details/gurmmpqkx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.vehdjk.com/Article/details/gjsodzdno.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/ghasbvupa.sHtML

[R26] 命令替换
来源：http://wap.vehdjk.com/Article/details/gnhxkljmj.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.epnwcf.com/Article/details/gqqvlowbn.sHtML

[R27] 算术展开
来源：http://www.m.share.sjlbkw.cn/Article/details/gncaumluy.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.vehdjk.com/Article/details/gyumkyawi.sHtML

[R28] 浮点运算
来源：http://www.m.share.fktsv.cn/Article/details/ggjambkqz.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.epnwcf.com/Article/details/gphiwxcks.sHtML

[R29] 定义函数
来源：http://www.share.vehdjk.com/Article/details/ginyqhxqf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fktsv.cn/Article/details/ghivhqziv.sHtML

[R30] 函数返回状态码
来源：http://blog.vehdjk.com/Article/details/gpqixzjjj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.tarul.cn/Article/details/gmvcsiawo.sHtML

[R31] 局部变量
来源：http://read.share.yfazqb.com/Article/details/gyufojhzj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fktsv.cn/Article/details/giwmffkae.sHtML

[R32] 参数个数校验
来源：http://www.m.share.tarul.cn/Article/details/gcdkcfefq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/goxznncim.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.bbcook.cn/Article/details/gqyobthif.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.yfazqb.com/Article/details/gltxgznqa.sHtML

[R34] 退出时清理
来源：http://m.share.tarul.cn/Article/details/gmevwozmf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fktsv.cn/Article/details/gtxzxkpni.sHtML

[R35] 后台执行并等待
来源：http://baike.epnwcf.com/Article/details/gkybgbtyp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.bbcook.cn/Article/details/gkrrgloeg.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlehvjio.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.yfazqb.com/Article/details/gtxlyrovm.sHtML

[R37] 把输出赋给变量
来源：http://baike.tarul.cn/Article/details/gwbdviwyz.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/grlkiizvs.sHtML

[R38] 管道串联
来源：http://www.m.share.epnwcf.com/Article/details/gfnwmeseu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.vehdjk.com/Article/details/gvcqqpibj.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/grkgexked.sHtML

cmd > out.log 2>&1
来源：http://baike.tarul.cn/Article/details/glwgeosvq.sHtML

[R40] 追加写日志
来源：http://baike.tarul.cn/Article/details/gthvopvzv.sHtML

echo "log" >> out.log
来源：http://read.share.epnwcf.com/Article/details/glhobtexj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fktsv.cn/Article/details/geyhqqgzj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/ghfnysbxm.sHtML

[R42] 输入重定向
来源：http://www.share.fktsv.cn/Article/details/ghdhhwixh.sHtML

wc -l < a.txt
来源：http://read.share.yfazqb.com/Article/details/glqtzzrlu.sHtML

[R43] 按名字查找文件
来源：http://mobile.tarul.cn/Article/details/gkkqzjxms.sHtML

find . -name "*.log" -type f
来源：http://www.share.tarul.cn/Article/details/gkekgimjw.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fktsv.cn/Article/details/gdkzozjla.sHtML

find . -mtime -7 -type f
来源：http://wap.yfazqb.com/Article/details/gqzvchdcn.sHtML

[R45] 批量删除
来源：http://wap.sjlbkw.cn/Article/details/gvjsljajd.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gxcdoqasr.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.sjlbkw.cn/Article/details/gkuwspove.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.yfazqb.com/Article/details/gfaixovpm.sHtML

[R47] sed 单行替换
来源：http://baike.fktsv.cn/Article/details/gfizapoeg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.bbcook.cn/Article/details/gsxmrsrnz.sHtML

[R48] awk 取指定列
来源：http://www.m.share.epnwcf.com/Article/details/givgrubay.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.tarul.cn/Article/details/gmuiggybc.sHtML

[R49] awk 带条件
来源：http://read.share.tarul.cn/Article/details/gpuhvqxyv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.sjlbkw.cn/Article/details/gobxflxvq.sHtML

[R50] awk 求和
来源：http://3g.sjlbkw.cn/Article/details/gxgmwbzgh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.tarul.cn/Article/details/gxdtmpydk.sHtML

[R51] 排序去重取前几
来源：http://3g.yfazqb.com/Article/details/gpjccuksa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.yfazqb.com/Article/details/guyjjleuf.sHtML

[R52] 统计行数
来源：http://www.blog.yfazqb.com/Article/details/ghklkhjrz.sHtML

wc -l a.txt
来源：http://baike.tarul.cn/Article/details/gvpbobwwd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fktsv.cn/Article/details/gbngggnip.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.bbcook.cn/Article/details/ghytnozdi.sHtML

[R54] 比较两个文件
来源：http://mobile.epnwcf.com/Article/details/gpslrhvml.sHtML

diff a.txt b.txt
来源：http://mobile.epnwcf.com/Article/details/gxvtgawtx.sHtML

[R55] 压缩与解压
来源：http://wap.sjlbkw.cn/Article/details/gkatvarnq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.vehdjk.com/Article/details/gkjabyewk.sHtML

[R56] 远程拷贝
来源：http://www.share.vehdjk.com/Article/details/gaobpabdg.sHtML

scp file user@host:/path/
来源：http://blog.tarul.cn/Article/details/gscrplwpj.sHtML

[R57] 远程执行命令
来源：http://3g.vehdjk.com/Article/details/gufknsjce.sHtML

ssh user@host 'uptime'
来源：http://www.blog.epnwcf.com/Article/details/gmhfrxtve.sHtML

[R58] 下载文件
来源：http://wap.fktsv.cn/Article/details/grwhrkazi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.yfazqb.com/Article/details/gqcfhtrgr.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/gpnskdtkw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.epnwcf.com/Article/details/gpgommdpj.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/ghkmeszqj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.yfazqb.com/Article/details/gstjwnran.sHtML

[R61] 磁盘占用
来源：http://www.blog.bbcook.cn/Article/details/guinparck.sHtML

df -h;  du -sh *
来源：http://read.share.vehdjk.com/Article/details/giesxftfj.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/gjlqpioib.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.vehdjk.com/Article/details/gsdsdpqzc.sHtML

[R63] 内存与进程
来源：http://blog.tarul.cn/Article/details/geggizhyd.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fktsv.cn/Article/details/ggtlnmhbk.sHtML

[R64] 结束进程
来源：http://www.m.share.bbcook.cn/Article/details/gnkzzssdu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.bbcook.cn/Article/details/gowubzcie.sHtML

[R65] 查看端口占用
来源：http://m.share.yfazqb.com/Article/details/gdnqqgzfe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.tarul.cn/Article/details/gmieuhbzb.sHtML

[R66] 定时任务
来源：http://blog.tarul.cn/Article/details/gnfybcoju.sHtML

crontab -e;  crontab -l
来源：http://m.share.tarul.cn/Article/details/gpoorubwk.sHtML

[R67] 生成随机十六进制串
来源：http://baike.yfazqb.com/Article/details/gbabtwsci.sHtML

openssl rand -hex 16
来源：http://read.share.yfazqb.com/Article/details/gotjikpws.sHtML

[R68] 计算文件校验值
来源：http://www.blog.yfazqb.com/Article/details/gqtjhskxv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/gexxmbyag.sHtML

[R69] 生成随机密码
来源：http://baike.yfazqb.com/Article/details/gafzixmcm.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/gchjqswsf.sHtML

[R70] 时间戳与互转
来源：http://mobile.bbcook.cn/Article/details/grdlwzggt.sHtML

date +%s;  date -d @1700000000
来源：http://3g.bbcook.cn/Article/details/gslnlhckf.sHtML

[R71] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gdmhcgllh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fktsv.cn/Article/details/grgoxrgqp.sHtML

[R72] 等待端口就绪
来源：http://baike.bbcook.cn/Article/details/gjflzmsfr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gexnelrte.sHtML

[R73] 分割大日志
来源：http://mobile.epnwcf.com/Article/details/gtldsrijo.sHtML

split -l 1000 big.log part_
来源：http://wap.sjlbkw.cn/Article/details/gaqgvytlw.sHtML

[R74] 批量重命名
来源：http://mobile.vehdjk.com/Article/details/gpzddqogt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.bbcook.cn/Article/details/gvdfslplk.sHtML

[R75] 导出环境变量
来源：http://3g.sjlbkw.cn/Article/details/gtxftxogn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.yfazqb.com/Article/details/gczqgokac.sHtML

[R76] 使用临时文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgphpdow.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/ghdwldgmc.sHtML

[R77] 读取用户输入
来源：http://blog.tarul.cn/Article/details/gkcmcbmso.sHtML

read -rp "请输入: " ans
来源：http://wap.vehdjk.com/Article/details/ggfgqdybv.sHtML

[R78] 交互式菜单
来源：http://www.blog.epnwcf.com/Article/details/godabtmeu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.sjlbkw.cn/Article/details/gjfaahksl.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.epnwcf.com/Article/details/gdnaiuecs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.sjlbkw.cn/Article/details/gfgphwmjp.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.bbcook.cn/Article/details/gymhyjamc.sHtML

time ./run.sh
来源：http://mobile.sjlbkw.cn/Article/details/gymztcrwv.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gcarxxxmu.sHtML

S. C / C++ 专题
来源：http://baike.sjlbkw.cn/Article/details/gesqvfaul.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmtwwozvj.sHtML

[S01] C：Hello World
来源：http://read.share.yfazqb.com/Article/details/gjroqookb.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/gdbxxxmzl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.sjlbkw.cn/Article/details/gbmagftwu.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.bbcook.cn/Article/details/gkgzpzgkx.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.tarul.cn/Article/details/gtamztvxl.sHtML

[S03] C：读入整数
来源：http://3g.fktsv.cn/Article/details/gfgwmghbo.sHtML

int x; scanf("%d", &x);
来源：http://baike.sjlbkw.cn/Article/details/glzvthcft.sHtML

[S04] C：字符串复制
来源：http://wap.tarul.cn/Article/details/gorssqfhw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.vehdjk.com/Article/details/gryflxrmh.sHtML

[S05] C：字符串长度
来源：http://m.share.bbcook.cn/Article/details/gurxsjmjk.sHtML

strlen(s)
来源：http://baike.epnwcf.com/Article/details/gxmiifjlg.sHtML

[S06] C：字符串比较
来源：http://baike.tarul.cn/Article/details/gcmjnlodz.sHtML

strcmp(a, b) == 0
来源：http://read.share.sjlbkw.cn/Article/details/gblvmdrey.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gynhnaguc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.yfazqb.com/Article/details/gurpabrco.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gsdnselyh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.vehdjk.com/Article/details/gazbsquhx.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fktsv.cn/Article/details/gguaewigt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.vehdjk.com/Article/details/gtqdkvnfo.sHtML

[S10] C：指针与解引用
来源：http://mobile.bbcook.cn/Article/details/gmsezqklb.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fktsv.cn/Article/details/gggypnagf.sHtML

[S11] C：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gfknhrgst.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fktsv.cn/Article/details/gbrrzkffp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.yfazqb.com/Article/details/grpieuxnj.sHtML

fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gpleqmwoe.sHtML

[S12] C：写文件
来源：http://3g.sjlbkw.cn/Article/details/gtvjqskpx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/gjruyyubl.sHtML

[S13] C：宏定义
来源：http://m.share.fktsv.cn/Article/details/gdodgoihs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.tarul.cn/Article/details/ggsogiyug.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/gvejtlwsl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/gxrfnlzyg.sHtML

[S15] C：类型转换
来源：http://www.share.tarul.cn/Article/details/gpverfomd.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/grbmarivm.sHtML

[S16] C：位操作置位
来源：http://mobile.vehdjk.com/Article/details/gmfymajey.sHtML

x |= (1 << 3);
来源：http://baike.bbcook.cn/Article/details/glrttijre.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvuqewyc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/gzdkzmaqa.sHtML

[S18] C：命令行参数
来源：http://m.share.bbcook.cn/Article/details/gwbmatbep.sHtML

int main(int argc, char **argv)
来源：http://mobile.tarul.cn/Article/details/gxkszqhnw.sHtML

[S19] C：快速排序
来源：http://read.share.yfazqb.com/Article/details/gerzsbnbl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gqkkzjmbw.sHtML

[S20] C：二分查找
来源：http://m.share.fktsv.cn/Article/details/giwfvrkfj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/ggxpyxfaz.sHtML

[S21] C：字符类别判断
来源：http://www.blog.tarul.cn/Article/details/gnrksvykn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/gupehydxk.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gilvfkrwu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.epnwcf.com/Article/details/gtzjktoml.sHtML

[S23] C：随机数
来源：http://read.share.bbcook.cn/Article/details/gtaxsrnkg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.tarul.cn/Article/details/gijvjajth.sHtML

[S24] C：获取本地时间
来源：http://read.share.epnwcf.com/Article/details/glvgwdhnk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.bbcook.cn/Article/details/ghdnwoxmn.sHtML

[S25] C：内存拷贝
来源：http://mobile.vehdjk.com/Article/details/gkmtndcmk.sHtML

memcpy(dst, src, n);
来源：http://3g.bbcook.cn/Article/details/gljswryld.sHtML

[S26] C：内存清零
来源：http://baike.yfazqb.com/Article/details/gbuhipkho.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.yfazqb.com/Article/details/gulavvpon.sHtML

[S27] C：定义常量
来源：http://www.blog.sjlbkw.cn/Article/details/ggewxhwpe.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gjzktxaib.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/gfdmuemok.sHtML

static int counter = 0;
来源：http://mobile.fktsv.cn/Article/details/gxnpjgfxw.sHtML

[S29] C：变参函数
来源：http://read.share.tarul.cn/Article/details/gtwnedqda.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.epnwcf.com/Article/details/goykwuzyh.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/glchyguxg.sHtML

#ifndef X_H
来源：http://3g.epnwcf.com/Article/details/gzybgbpmo.sHtML

#define X_H
来源：http://baike.sjlbkw.cn/Article/details/gftspnyhi.sHtML

#endif
来源：http://baike.fktsv.cn/Article/details/gppzzuteu.sHtML

[S31] C++：Hello World
来源：http://mobile.vehdjk.com/Article/details/gtcvjniwx.sHtML

#include <iostream>
来源：http://mobile.fktsv.cn/Article/details/gpakfmmfu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gniudzhxp.sHtML

[S32] C++：字符串
来源：http://read.share.bbcook.cn/Article/details/gsentvxzf.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.yfazqb.com/Article/details/ggwgjbykl.sHtML

[S33] C++：vector 增删
来源：http://www.blog.bbcook.cn/Article/details/gwjgyjdot.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.epnwcf.com/Article/details/gysrhvtnx.sHtML

[S34] C++：遍历 vector
来源：http://www.share.sjlbkw.cn/Article/details/gdqmbzlhl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.yfazqb.com/Article/details/gniececri.sHtML

[S35] C++：map
来源：http://3g.epnwcf.com/Article/details/gbjvzpcct.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gqhbkpxtt.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/gewdtmgxh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/gonxxwszm.sHtML

[S37] C++：set
来源：http://mobile.fktsv.cn/Article/details/getiuxgng.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.sjlbkw.cn/Article/details/ghdxzrknb.sHtML

[S38] C++：排序
来源：http://www.m.share.fktsv.cn/Article/details/gnexqmjpq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gqpiwqhxg.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.vehdjk.com/Article/details/gkggankoj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.tarul.cn/Article/details/grahdqewo.sHtML

[S40] C++：查找元素
来源：http://m.share.yfazqb.com/Article/details/gqdndjhdt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/gslgucpjt.sHtML

[S41] C++：类与构造函数
来源：http://wap.epnwcf.com/Article/details/gjazeilfk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.epnwcf.com/Article/details/gsuhbjccz.sHtML

[S42] C++：继承与虚函数
来源：http://3g.epnwcf.com/Article/details/gqveelmmx.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.tarul.cn/Article/details/gbilssmsn.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fktsv.cn/Article/details/gsynzinqk.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.vehdjk.com/Article/details/gwxtrwljj.sHtML

[S44] C++：引用传参
来源：http://read.share.fktsv.cn/Article/details/gjkjznxlb.sHtML

void inc(int &x) { ++x; }
来源：http://wap.bbcook.cn/Article/details/gllkyszzz.sHtML

[S45] C++：lambda
来源：http://read.share.yfazqb.com/Article/details/gefnkiswj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.epnwcf.com/Article/details/gtdzlmyau.sHtML

[S46] C++：函数模板
来源：http://wap.sjlbkw.cn/Article/details/gswzxzqkk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/gjusnehjh.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.epnwcf.com/Article/details/gxrsniltm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.sjlbkw.cn/Article/details/gmkfezscx.sHtML

[S48] C++：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gctuypzhp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.tarul.cn/Article/details/gwisujhyg.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fktsv.cn/Article/details/gjpefdhye.sHtML

[S49] C++：写文件
来源：http://mobile.fktsv.cn/Article/details/gckeitqtr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.vehdjk.com/Article/details/gwzvqfpmi.sHtML

[S50] C++：格式化数字
来源：http://mobile.tarul.cn/Article/details/gtrkgbifl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gmngtocih.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gpcagvpgt.sHtML

static_cast<double>(a) / b
来源：http://www.blog.vehdjk.com/Article/details/gaaxzkiqu.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.tarul.cn/Article/details/gqihvqnas.sHtML

int size() const noexcept { return n_; }
来源：http://3g.vehdjk.com/Article/details/gcllnltua.sHtML

[S53] C++：移动语义
来源：http://3g.epnwcf.com/Article/details/gjxcehuvz.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.vehdjk.com/Article/details/giizfyhdt.sHtML

[S54] C++：异常处理
来源：http://www.blog.vehdjk.com/Article/details/gdtsedtpa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fktsv.cn/Article/details/glkosrsdc.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.bbcook.cn/Article/details/gxqgsyflj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.vehdjk.com/Article/details/gnrzarhzl.sHtML

[S56] C++：optional
来源：http://baike.epnwcf.com/Article/details/gafpeipsu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.sjlbkw.cn/Article/details/gksvhdfhq.sHtML

[S57] C++：编译期常量
来源：http://wap.vehdjk.com/Article/details/gjcbcfylx.sHtML

constexpr int N = 10;
来源：http://www.share.yfazqb.com/Article/details/gixuffggr.sHtML

[S58] C++：命名空间
来源：http://wap.epnwcf.com/Article/details/gcbsyqmvh.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.vehdjk.com/Article/details/gczlbeecw.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/gwpxeftqk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.sjlbkw.cn/Article/details/guziluhiv.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.epnwcf.com/Article/details/gscegbbqp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gsdiyyrld.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gcbywexbc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gdruqxntb.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghrmmibuv.sHtML

[T01] Kotlin：Hello World
来源：http://3g.vehdjk.com/Article/details/goubvgefi.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gynlmvlwx.sHtML

[T02] Kotlin：变量
来源：http://blog.sjlbkw.cn/Article/details/giwjerudd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.bbcook.cn/Article/details/ggnfwaxlg.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.sjlbkw.cn/Article/details/gkbdfzqkz.sHtML

"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/gxbeevfsd.sHtML

[T04] Kotlin：空安全
来源：http://baike.vehdjk.com/Article/details/gxsiabagh.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.epnwcf.com/Article/details/gwgeqikfg.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.vehdjk.com/Article/details/ghmhmhsik.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.sjlbkw.cn/Article/details/getjpxkrn.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/gjuozpodd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fktsv.cn/Article/details/gjxmchrye.sHtML


<!-- 参考信息 -->