代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.yfazqb.com/Article/details/ghoyawquv.sHtML

[R10] 正则匹配
来源：http://wap.yfazqb.com/Article/details/gdhrxgvsb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.bbcook.cn/Article/details/gaftwcttd.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/gczvrzjqh.sHtML

case "$1" in
来源：http://blog.sjlbkw.cn/Article/details/grgtzcrsu.sHtML

start) echo "启动" ;;
来源：http://baike.tarul.cn/Article/details/gtvbyqjyu.sHtML

stop)  echo "停止" ;;
来源：http://m.share.bbcook.cn/Article/details/getgtqada.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.vehdjk.com/Article/details/gvkkkloan.sHtML

esac
来源：http://wap.epnwcf.com/Article/details/gtkfsnxiy.sHtML

[R12] for 遍历文件
来源：http://baike.fktsv.cn/Article/details/ggoyxgkzj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.vehdjk.com/Article/details/gqxkmimib.sHtML

[R13] for 计数循环
来源：http://blog.tarul.cn/Article/details/gjottrevu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gymoblxny.sHtML

[R14] C 风格 for
来源：http://www.m.share.fktsv.cn/Article/details/gaxsjyogb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/gybvylxtm.sHtML

[R15] while 逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gmlxcrlkv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.yfazqb.com/Article/details/ggzpxsvoy.sHtML

[R16] until 等待条件
来源：http://blog.tarul.cn/Article/details/gyehtngmd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/gqfbqbgff.sHtML

[R17] 数组定义与取值
来源：http://m.share.fktsv.cn/Article/details/gerqjkuxf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.vehdjk.com/Article/details/gclhpxlhf.sHtML

[R18] 遍历数组
来源：http://read.share.epnwcf.com/Article/details/gbsmogsxx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkuzftdq.sHtML

[R19] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gyxzelxoc.sHtML

echo "${#arr[@]}"
来源：http://blog.yfazqb.com/Article/details/gfhczovew.sHtML

[R20] 关联数组（字典）
来源：http://read.share.yfazqb.com/Article/details/gokjluoas.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.sjlbkw.cn/Article/details/gdhsdmkvl.sHtML

[R21] 字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gduktfmae.sHtML

echo "${#s}"
来源：http://blog.bbcook.cn/Article/details/gzraypoyl.sHtML

[R22] 截取子串
来源：http://read.share.bbcook.cn/Article/details/gjcrmxeqz.sHtML

echo "${s:0:5}"
来源：http://mobile.sjlbkw.cn/Article/details/grzlhzcty.sHtML

[R23] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gvgpbrnfc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fktsv.cn/Article/details/gesxcpyxq.sHtML

[R24] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gzavmhdwx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.sjlbkw.cn/Article/details/gbcszownn.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.sjlbkw.cn/Article/details/gqerxafff.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.epnwcf.com/Article/details/ghufvkdmh.sHtML

[R26] 命令替换
来源：http://www.blog.epnwcf.com/Article/details/gsrospgts.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.epnwcf.com/Article/details/gfqsmxcff.sHtML

[R27] 算术展开
来源：http://www.m.share.epnwcf.com/Article/details/gwzlbesrf.sHtML

echo $((1 + 2 * 3))
来源：http://3g.tarul.cn/Article/details/guihigkau.sHtML

[R28] 浮点运算
来源：http://wap.sjlbkw.cn/Article/details/gngpeuzhd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.epnwcf.com/Article/details/gnprkgpan.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/guzaqkzmr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gniqtlyqm.sHtML

[R30] 函数返回状态码
来源：http://mobile.fktsv.cn/Article/details/gqqoqdzxe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.tarul.cn/Article/details/gbfljdbdn.sHtML

[R31] 局部变量
来源：http://blog.vehdjk.com/Article/details/gdgszszlj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/gcsmqbdbw.sHtML

[R32] 参数个数校验
来源：http://m.share.vehdjk.com/Article/details/gmfniiois.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/guwcdjsow.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.sjlbkw.cn/Article/details/ghdnoszoh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.vehdjk.com/Article/details/grnmccura.sHtML

[R34] 退出时清理
来源：http://www.blog.sjlbkw.cn/Article/details/gpdsownmr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gbygntohl.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/gmelrgcbv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.epnwcf.com/Article/details/gslpviske.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/gdzwawkqf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/grgqehyud.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/gphkkkroc.sHtML

files=$(ls -1)
来源：http://mobile.epnwcf.com/Article/details/giipsakvl.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/gwdfyvsbg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/ghukpcsgi.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.sjlbkw.cn/Article/details/gwmljcbqb.sHtML

cmd > out.log 2>&1
来源：http://wap.bbcook.cn/Article/details/gwrulfobj.sHtML

[R40] 追加写日志
来源：http://m.share.bbcook.cn/Article/details/gxoburbhr.sHtML

echo "log" >> out.log
来源：http://3g.vehdjk.com/Article/details/ggaascezk.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/ggidqexxz.sHtML

cmd >/dev/null 2>&1
来源：http://3g.bbcook.cn/Article/details/gkirfrybf.sHtML

[R42] 输入重定向
来源：http://read.share.vehdjk.com/Article/details/gjuypznda.sHtML

wc -l < a.txt
来源：http://m.share.yfazqb.com/Article/details/gzwttypbm.sHtML

[R43] 按名字查找文件
来源：http://wap.bbcook.cn/Article/details/gwlcyjngt.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.sjlbkw.cn/Article/details/glzblgcmt.sHtML

[R44] 按修改时间查找
来源：http://read.share.sjlbkw.cn/Article/details/gunftykdm.sHtML

find . -mtime -7 -type f
来源：http://www.share.yfazqb.com/Article/details/gdjhgnrcg.sHtML

[R45] 批量删除
来源：http://wap.yfazqb.com/Article/details/goesiokdl.sHtML

find . -name "*.tmp" -delete
来源：http://3g.epnwcf.com/Article/details/ggziqcill.sHtML

[R46] 递归替换文件内容
来源：http://www.share.epnwcf.com/Article/details/gvncnvzkw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.epnwcf.com/Article/details/gjiijrktt.sHtML

[R47] sed 单行替换
来源：http://www.blog.fktsv.cn/Article/details/gazeuysrq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.tarul.cn/Article/details/grimkajku.sHtML

[R48] awk 取指定列
来源：http://www.share.epnwcf.com/Article/details/ggmuenytm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gwrdryczr.sHtML

[R49] awk 带条件
来源：http://blog.tarul.cn/Article/details/gfdzhxwxt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.sjlbkw.cn/Article/details/gjyfxhlqf.sHtML

[R50] awk 求和
来源：http://read.share.bbcook.cn/Article/details/gimecpdrw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.tarul.cn/Article/details/gtkxiksuw.sHtML

[R51] 排序去重取前几
来源：http://mobile.vehdjk.com/Article/details/gbzfbeiqc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.yfazqb.com/Article/details/geygyypis.sHtML

[R52] 统计行数
来源：http://wap.sjlbkw.cn/Article/details/grbvolunj.sHtML

wc -l a.txt
来源：http://wap.epnwcf.com/Article/details/gpxjadknb.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.epnwcf.com/Article/details/gowkmhvab.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gofdiwcxg.sHtML

[R54] 比较两个文件
来源：http://read.share.epnwcf.com/Article/details/gngitahou.sHtML

diff a.txt b.txt
来源：http://www.blog.sjlbkw.cn/Article/details/grujhdbvh.sHtML

[R55] 压缩与解压
来源：http://www.m.share.sjlbkw.cn/Article/details/glywnssyw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.sjlbkw.cn/Article/details/gpquwryng.sHtML

[R56] 远程拷贝
来源：http://blog.sjlbkw.cn/Article/details/gizkglmas.sHtML

scp file user@host:/path/
来源：http://wap.bbcook.cn/Article/details/gechopdas.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gjflqisuq.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/guiulhbfj.sHtML

[R58] 下载文件
来源：http://mobile.yfazqb.com/Article/details/glnmotwab.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.sjlbkw.cn/Article/details/grqhleirw.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gunoycawv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.epnwcf.com/Article/details/gtfxoihzg.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/gguwxyxch.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.epnwcf.com/Article/details/gljolgojl.sHtML

[R61] 磁盘占用
来源：http://www.blog.bbcook.cn/Article/details/gxpfcptiw.sHtML

df -h;  du -sh *
来源：http://www.m.share.fktsv.cn/Article/details/gpujekutc.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fktsv.cn/Article/details/gfuckjiiz.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.yfazqb.com/Article/details/gnhpwxuii.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gxbnkpaah.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.vehdjk.com/Article/details/gbufsqbuu.sHtML

[R64] 结束进程
来源：http://www.share.yfazqb.com/Article/details/guawjivta.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.sjlbkw.cn/Article/details/gheqmxabk.sHtML

[R65] 查看端口占用
来源：http://www.share.fktsv.cn/Article/details/girpjszap.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.epnwcf.com/Article/details/gmalfzvem.sHtML

[R66] 定时任务
来源：http://www.share.fktsv.cn/Article/details/grelbsdpw.sHtML

crontab -e;  crontab -l
来源：http://m.share.sjlbkw.cn/Article/details/gkfjzienw.sHtML

[R67] 生成随机十六进制串
来源：http://blog.sjlbkw.cn/Article/details/gnzeghsqz.sHtML

openssl rand -hex 16
来源：http://baike.epnwcf.com/Article/details/gfwwazzyg.sHtML

[R68] 计算文件校验值
来源：http://3g.fktsv.cn/Article/details/gkidsxyjw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.epnwcf.com/Article/details/gvebdbxny.sHtML

[R69] 生成随机密码
来源：http://wap.yfazqb.com/Article/details/gmfyjyjhe.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gdhaoclpd.sHtML

[R70] 时间戳与互转
来源：http://baike.epnwcf.com/Article/details/gxlcxlgro.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.tarul.cn/Article/details/gfmdwmsfl.sHtML

[R71] 日期格式化
来源：http://mobile.epnwcf.com/Article/details/gogzvzjlu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.sjlbkw.cn/Article/details/gcrlafhxj.sHtML

[R72] 等待端口就绪
来源：http://mobile.sjlbkw.cn/Article/details/grazvrdol.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gpidhmktz.sHtML

[R73] 分割大日志
来源：http://baike.sjlbkw.cn/Article/details/guqqlfvlg.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/glwmbfwjw.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/gmsnpdgsk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.bbcook.cn/Article/details/gwyjoqand.sHtML

[R75] 导出环境变量
来源：http://3g.fktsv.cn/Article/details/gtzkksxvk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.sjlbkw.cn/Article/details/gofrpvrpg.sHtML

[R76] 使用临时文件
来源：http://www.blog.tarul.cn/Article/details/gggegoddf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/ggdtkxrum.sHtML

[R77] 读取用户输入
来源：http://www.blog.bbcook.cn/Article/details/gpxqagoui.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzdqawcn.sHtML

[R78] 交互式菜单
来源：http://baike.vehdjk.com/Article/details/gomxysoba.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/gloebautf.sHtML

[R79] 解析命令行选项
来源：http://www.share.tarul.cn/Article/details/gttzpalug.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.tarul.cn/Article/details/ggwputpaz.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fktsv.cn/Article/details/gxnmrmdyi.sHtML

time ./run.sh
来源：http://www.blog.bbcook.cn/Article/details/ggjhpoytn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggqjdivec.sHtML

S. C / C++ 专题
来源：http://mobile.vehdjk.com/Article/details/gdzzfjyth.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gunqxsjsg.sHtML

[S01] C：Hello World
来源：http://3g.tarul.cn/Article/details/gqzvmdcab.sHtML

#include <stdio.h>
来源：http://www.m.share.tarul.cn/Article/details/gtjklyexm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.bbcook.cn/Article/details/gmbaqqglg.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.vehdjk.com/Article/details/gxfmzbdhr.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.yfazqb.com/Article/details/gxrcoagtx.sHtML

[S03] C：读入整数
来源：http://3g.sjlbkw.cn/Article/details/ghxyutuln.sHtML

int x; scanf("%d", &x);
来源：http://read.share.yfazqb.com/Article/details/gmitpbryb.sHtML

[S04] C：字符串复制
来源：http://m.share.tarul.cn/Article/details/gslwqrgnd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.sjlbkw.cn/Article/details/gnazplqbs.sHtML

[S05] C：字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gjqwjiuuq.sHtML

strlen(s)
来源：http://baike.fktsv.cn/Article/details/gvglrusbt.sHtML

[S06] C：字符串比较
来源：http://m.share.epnwcf.com/Article/details/gfqexipug.sHtML

strcmp(a, b) == 0
来源：http://3g.bbcook.cn/Article/details/ghrembrpj.sHtML

[S07] C：数组遍历求和
来源：http://baike.tarul.cn/Article/details/gfiucdret.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.bbcook.cn/Article/details/gwldaenkh.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.bbcook.cn/Article/details/gxraftlrn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.epnwcf.com/Article/details/gescopdtq.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.yfazqb.com/Article/details/ghtdiblul.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.tarul.cn/Article/details/gbznmsorv.sHtML

[S10] C：指针与解引用
来源：http://read.share.yfazqb.com/Article/details/gtfvuskxp.sHtML

int *p = &a;  *p = 5;
来源：http://3g.yfazqb.com/Article/details/gnupfupss.sHtML

[S11] C：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gojtiydbb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.epnwcf.com/Article/details/gbcquirbm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gwbhmbdxa.sHtML

fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gtwssoott.sHtML

[S12] C：写文件
来源：http://wap.vehdjk.com/Article/details/ggwyozdal.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/ghydjbzbz.sHtML

[S13] C：宏定义
来源：http://blog.tarul.cn/Article/details/gfemawlil.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/gcwfrfquf.sHtML

[S14] C：枚举
来源：http://blog.yfazqb.com/Article/details/gmkpvlevq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.yfazqb.com/Article/details/gnnctjzls.sHtML

[S15] C：类型转换
来源：http://baike.epnwcf.com/Article/details/gdjssnxou.sHtML

(double) a / b
来源：http://blog.epnwcf.com/Article/details/guudsbnaf.sHtML

[S16] C：位操作置位
来源：http://read.share.yfazqb.com/Article/details/grblvfktj.sHtML

x |= (1 << 3);
来源：http://www.m.share.vehdjk.com/Article/details/gpsglztyx.sHtML

[S17] C：安全拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/ghzvkmala.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.yfazqb.com/Article/details/gequsyigj.sHtML

[S18] C：命令行参数
来源：http://wap.yfazqb.com/Article/details/geaojulqj.sHtML

int main(int argc, char **argv)
来源：http://mobile.sjlbkw.cn/Article/details/gdsthcqwk.sHtML

[S19] C：快速排序
来源：http://read.share.vehdjk.com/Article/details/grpefqrao.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gsbzeoovt.sHtML

[S20] C：二分查找
来源：http://m.share.vehdjk.com/Article/details/gmwkmvszb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gbimcjhzg.sHtML

[S21] C：字符类别判断
来源：http://read.share.sjlbkw.cn/Article/details/gphjdjvxn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.tarul.cn/Article/details/gnjzihjyr.sHtML

[S22] C：字符串转数字
来源：http://www.blog.bbcook.cn/Article/details/gmyniqckl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fktsv.cn/Article/details/gxnmtshjr.sHtML

[S23] C：随机数
来源：http://wap.vehdjk.com/Article/details/gsarxufes.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.vehdjk.com/Article/details/gyopeqkag.sHtML

[S24] C：获取本地时间
来源：http://m.share.fktsv.cn/Article/details/gmfpdnhyw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.tarul.cn/Article/details/gpekqaxlv.sHtML

[S25] C：内存拷贝
来源：http://blog.fktsv.cn/Article/details/gwuahbunh.sHtML

memcpy(dst, src, n);
来源：http://www.share.yfazqb.com/Article/details/gfcmzpgwo.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gjrihqmyd.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/gniyfgxkk.sHtML

[S27] C：定义常量
来源：http://3g.yfazqb.com/Article/details/gdzzfcvso.sHtML

const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gsxdejdjw.sHtML

[S28] C：静态变量
来源：http://3g.epnwcf.com/Article/details/ggwkynglj.sHtML

static int counter = 0;
来源：http://mobile.epnwcf.com/Article/details/gmvsfyyay.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/gtqdklxlz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.sjlbkw.cn/Article/details/goqhfklfn.sHtML

[S30] C：头文件保护
来源：http://www.m.share.epnwcf.com/Article/details/ghqmwgpyw.sHtML

#ifndef X_H
来源：http://baike.epnwcf.com/Article/details/gwofpjjha.sHtML

#define X_H
来源：http://baike.yfazqb.com/Article/details/gshuglrqn.sHtML

#endif
来源：http://baike.bbcook.cn/Article/details/gzespbzyw.sHtML

[S31] C++：Hello World
来源：http://m.share.yfazqb.com/Article/details/gddklviem.sHtML

#include <iostream>
来源：http://3g.sjlbkw.cn/Article/details/gwwochrew.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.sjlbkw.cn/Article/details/gntulxufw.sHtML

[S32] C++：字符串
来源：http://3g.yfazqb.com/Article/details/gpfxxmdqj.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.yfazqb.com/Article/details/gosuoszjb.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fktsv.cn/Article/details/gshfgqwjy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.yfazqb.com/Article/details/gfupubgnr.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/ggvddxtyg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.sjlbkw.cn/Article/details/gldgkeyuy.sHtML

[S35] C++：map
来源：http://www.m.share.epnwcf.com/Article/details/gnnegiota.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/gkrtacvqk.sHtML

[S36] C++：unordered_map
来源：http://www.blog.yfazqb.com/Article/details/gszlqtrnp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/ggyltihzz.sHtML

[S37] C++：set
来源：http://wap.fktsv.cn/Article/details/gdrucvimm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/gbjfeevat.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/gegbsjkcm.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.bbcook.cn/Article/details/gzdkwnfus.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/gdejmcxsr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.vehdjk.com/Article/details/gtbibgoov.sHtML

[S40] C++：查找元素
来源：http://read.share.fktsv.cn/Article/details/gjjjwutgh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.yfazqb.com/Article/details/gmmqwklaf.sHtML

[S41] C++：类与构造函数
来源：http://m.share.tarul.cn/Article/details/gilgoeqsb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/gwgogprqw.sHtML

[S42] C++：继承与虚函数
来源：http://wap.sjlbkw.cn/Article/details/ghvyqpnqc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.yfazqb.com/Article/details/gkirgewoi.sHtML

[S43] C++：智能指针
来源：http://mobile.vehdjk.com/Article/details/gtpnhkgee.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.epnwcf.com/Article/details/gtlckhdmw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.epnwcf.com/Article/details/gwyyckpha.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/ghyeghcni.sHtML

[S45] C++：lambda
来源：http://www.share.bbcook.cn/Article/details/gvfqdscfv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.epnwcf.com/Article/details/gilqfsddv.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gxraltpgg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.vehdjk.com/Article/details/glnuxtwpl.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.sjlbkw.cn/Article/details/giznuuvhi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.yfazqb.com/Article/details/gynwxwjry.sHtML

[S48] C++：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gzxdqovix.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.yfazqb.com/Article/details/gjdshzacw.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.yfazqb.com/Article/details/glnbahsgj.sHtML

[S49] C++：写文件
来源：http://blog.epnwcf.com/Article/details/gtsqlvitf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/gjhjszxck.sHtML

[S50] C++：格式化数字
来源：http://mobile.tarul.cn/Article/details/gbplcrrza.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.bbcook.cn/Article/details/gxqvmuvqw.sHtML

[S51] C++：显式类型转换
来源：http://baike.vehdjk.com/Article/details/gpalrthtd.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.epnwcf.com/Article/details/gipejzycn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.bbcook.cn/Article/details/gbbizdjvs.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fktsv.cn/Article/details/gwnzubxlp.sHtML

[S53] C++：移动语义
来源：http://www.share.vehdjk.com/Article/details/gofrrbsux.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.sjlbkw.cn/Article/details/gibhzgmqu.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fktsv.cn/Article/details/gfzcpcarm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.sjlbkw.cn/Article/details/gwaqokhsk.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.sjlbkw.cn/Article/details/gkojhvmvl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.bbcook.cn/Article/details/gbyekndfx.sHtML

[S56] C++：optional
来源：http://www.blog.yfazqb.com/Article/details/gzpvfokyz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.bbcook.cn/Article/details/ghvvliaqm.sHtML

[S57] C++：编译期常量
来源：http://3g.fktsv.cn/Article/details/gmvydwerz.sHtML

constexpr int N = 10;
来源：http://baike.vehdjk.com/Article/details/gjvwkovmw.sHtML

[S58] C++：命名空间
来源：http://3g.bbcook.cn/Article/details/gdanvpwwr.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.yfazqb.com/Article/details/gpvimyztp.sHtML

[S59] C++：静态断言
来源：http://mobile.vehdjk.com/Article/details/gkzrqlvvk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.vehdjk.com/Article/details/ghzpczvho.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.epnwcf.com/Article/details/gvtbtzniv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/grqsrztit.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/giyndxosn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/gvooowdfb.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtvaumqnz.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fktsv.cn/Article/details/gjpmfbwht.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/ggmaxflso.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/geqwbzlcm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.epnwcf.com/Article/details/gawojbnpu.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.tarul.cn/Article/details/gglohscht.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/giqrlfkao.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fktsv.cn/Article/details/gokkmfobl.sHtML

val n: String? = null;  n?.length
来源：http://wap.bbcook.cn/Article/details/glsackokm.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.sjlbkw.cn/Article/details/gsjntjlax.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.yfazqb.com/Article/details/gjaopzqyf.sHtML

[T06] Kotlin：集合映射
来源：http://blog.epnwcf.com/Article/details/gwzafokeu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.tarul.cn/Article/details/gwmxagwsd.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.tarul.cn/Article/details/gafszkxyp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fktsv.cn/Article/details/guizjcujk.sHtML

[T08] Kotlin：数据类
来源：http://read.share.bbcook.cn/Article/details/glgwvglzh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.tarul.cn/Article/details/gkmyiwjac.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fktsv.cn/Article/details/gxsewbouc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fktsv.cn/Article/details/gwakcvkpg.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.sjlbkw.cn/Article/details/gnqmmgnmv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.yfazqb.com/Article/details/gfaanimxf.sHtML


<!-- 参考信息 -->