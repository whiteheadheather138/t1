代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.tarul.cn/Article/details/ghmeiqsdb.sHtML

[R10] 正则匹配
来源：http://www.m.share.bbcook.cn/Article/details/gjqvvvnrh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkghykrh.sHtML

[R11] case 多分支
来源：http://www.m.share.fktsv.cn/Article/details/ghhhsyveu.sHtML

case "$1" in
来源：http://m.share.yfazqb.com/Article/details/gysniwkjy.sHtML

start) echo "启动" ;;
来源：http://www.share.epnwcf.com/Article/details/ghclkkfbt.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fktsv.cn/Article/details/gqtegjitd.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.epnwcf.com/Article/details/gifiybdaz.sHtML

esac
来源：http://m.share.sjlbkw.cn/Article/details/gsqyzbmsk.sHtML

[R12] for 遍历文件
来源：http://www.blog.tarul.cn/Article/details/gpfawzrvf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.yfazqb.com/Article/details/gqyobbrbh.sHtML

[R13] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/gyerjpcnz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gzvaskldi.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/ghxtzxjzf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/ggmsyqvfq.sHtML

[R15] while 逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gluulomrx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.epnwcf.com/Article/details/gkeqjmyrg.sHtML

[R16] until 等待条件
来源：http://www.m.share.tarul.cn/Article/details/gwfbebavc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gomopzhym.sHtML

[R17] 数组定义与取值
来源：http://www.share.tarul.cn/Article/details/gieuduzgd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.tarul.cn/Article/details/gewdsxnpq.sHtML

[R18] 遍历数组
来源：http://read.share.fktsv.cn/Article/details/gcgyxhdij.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.sjlbkw.cn/Article/details/ggwvsrhsy.sHtML

[R19] 数组长度
来源：http://mobile.sjlbkw.cn/Article/details/gtkkcccoy.sHtML

echo "${#arr[@]}"
来源：http://read.share.tarul.cn/Article/details/grrjzdlcd.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fktsv.cn/Article/details/gdqvqbuim.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fktsv.cn/Article/details/gbuzdlbul.sHtML

[R21] 字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gvgillkbf.sHtML

echo "${#s}"
来源：http://www.blog.sjlbkw.cn/Article/details/gtysqkkhw.sHtML

[R22] 截取子串
来源：http://3g.fktsv.cn/Article/details/gbvmsscsu.sHtML

echo "${s:0:5}"
来源：http://m.share.fktsv.cn/Article/details/gkempakbz.sHtML

[R23] 字符串替换
来源：http://blog.vehdjk.com/Article/details/gvviofewv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.yfazqb.com/Article/details/gwuqrxzrf.sHtML

[R24] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gmvjjlyfm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.sjlbkw.cn/Article/details/gtufsfxjr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.epnwcf.com/Article/details/guckqvygf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.yfazqb.com/Article/details/gfuwdveva.sHtML

[R26] 命令替换
来源：http://m.share.bbcook.cn/Article/details/gvpgaxing.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.sjlbkw.cn/Article/details/getdwszec.sHtML

[R27] 算术展开
来源：http://m.share.epnwcf.com/Article/details/gkwdyejfn.sHtML

echo $((1 + 2 * 3))
来源：http://blog.vehdjk.com/Article/details/gwfikikjh.sHtML

[R28] 浮点运算
来源：http://www.share.bbcook.cn/Article/details/gmsfiyrut.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.epnwcf.com/Article/details/gnrcjdjdj.sHtML

[R29] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gmlqcqxyr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.bbcook.cn/Article/details/ghbdqwryi.sHtML

[R30] 函数返回状态码
来源：http://baike.bbcook.cn/Article/details/gymopcsnt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gesscraug.sHtML

[R31] 局部变量
来源：http://baike.epnwcf.com/Article/details/gnisbtlnv.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.yfazqb.com/Article/details/gknegzmjf.sHtML

[R32] 参数个数校验
来源：http://www.blog.epnwcf.com/Article/details/gpflhgjlr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/ggqcrmnyx.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fktsv.cn/Article/details/gfqbglybr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnvvlzzt.sHtML

[R34] 退出时清理
来源：http://m.share.sjlbkw.cn/Article/details/gochjjova.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gblmumgox.sHtML

[R35] 后台执行并等待
来源：http://www.share.sjlbkw.cn/Article/details/gnwxoqnza.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.epnwcf.com/Article/details/gzmrkkqyx.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/gsouvsbco.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.yfazqb.com/Article/details/gacbofkyf.sHtML

[R37] 把输出赋给变量
来源：http://read.share.tarul.cn/Article/details/goccdsdbl.sHtML

files=$(ls -1)
来源：http://read.share.vehdjk.com/Article/details/gszghksfx.sHtML

[R38] 管道串联
来源：http://wap.sjlbkw.cn/Article/details/gcuebornj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.tarul.cn/Article/details/gqvhudjic.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.sjlbkw.cn/Article/details/gvvanktuf.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/gbsilqawd.sHtML

[R40] 追加写日志
来源：http://m.share.epnwcf.com/Article/details/gcgjmfbju.sHtML

echo "log" >> out.log
来源：http://wap.tarul.cn/Article/details/glpstfnjy.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/gujzrcvnx.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fktsv.cn/Article/details/grqbgjwrp.sHtML

[R42] 输入重定向
来源：http://www.blog.fktsv.cn/Article/details/gpxrxrkdn.sHtML

wc -l < a.txt
来源：http://read.share.tarul.cn/Article/details/grsuqqwue.sHtML

[R43] 按名字查找文件
来源：http://3g.vehdjk.com/Article/details/gcnusfrer.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gshymizar.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/gauelryai.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.vehdjk.com/Article/details/glncnsiyj.sHtML

[R45] 批量删除
来源：http://m.share.bbcook.cn/Article/details/gjchrygjl.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.tarul.cn/Article/details/gyeciacnb.sHtML

[R46] 递归替换文件内容
来源：http://www.share.epnwcf.com/Article/details/gdotcdpzo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.bbcook.cn/Article/details/gjwcejszs.sHtML

[R47] sed 单行替换
来源：http://baike.tarul.cn/Article/details/gxtnmntdo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.vehdjk.com/Article/details/gqsoxzpes.sHtML

[R48] awk 取指定列
来源：http://mobile.vehdjk.com/Article/details/gwstcurob.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/giuivavil.sHtML

[R49] awk 带条件
来源：http://mobile.fktsv.cn/Article/details/gblixoxww.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.bbcook.cn/Article/details/geyoxolxt.sHtML

[R50] awk 求和
来源：http://blog.vehdjk.com/Article/details/gdhitdatw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fktsv.cn/Article/details/genfwuuha.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/gfyyekshk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.vehdjk.com/Article/details/gjwzjpxhq.sHtML

[R52] 统计行数
来源：http://www.m.share.bbcook.cn/Article/details/gsmapbaoj.sHtML

wc -l a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gssokhrpk.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fktsv.cn/Article/details/gmmevxyng.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.tarul.cn/Article/details/gtcmujjtv.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fktsv.cn/Article/details/grukfxckf.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/gqjlnomul.sHtML

[R55] 压缩与解压
来源：http://baike.sjlbkw.cn/Article/details/goqyrijbk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.tarul.cn/Article/details/ghokijjeh.sHtML

[R56] 远程拷贝
来源：http://blog.vehdjk.com/Article/details/gyhxpucpc.sHtML

scp file user@host:/path/
来源：http://3g.tarul.cn/Article/details/guydfpsld.sHtML

[R57] 远程执行命令
来源：http://www.blog.tarul.cn/Article/details/gszdxdkrf.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/gcbfwfdxa.sHtML

[R58] 下载文件
来源：http://mobile.vehdjk.com/Article/details/gwtfvqalv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.tarul.cn/Article/details/gmzemkpuw.sHtML

[R59] 发 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gfnqiqctb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.bbcook.cn/Article/details/garmtmqsc.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gjhaeiwwi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.yfazqb.com/Article/details/gibdxugpa.sHtML

[R61] 磁盘占用
来源：http://mobile.yfazqb.com/Article/details/gfyflfwhk.sHtML

df -h;  du -sh *
来源：http://3g.vehdjk.com/Article/details/gjruveohz.sHtML

[R62] 找最占空间的文件
来源：http://wap.bbcook.cn/Article/details/gsrtberek.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.bbcook.cn/Article/details/ghifsjiwt.sHtML

[R63] 内存与进程
来源：http://mobile.fktsv.cn/Article/details/gchpnbole.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fktsv.cn/Article/details/ghxgbfkxr.sHtML

[R64] 结束进程
来源：http://mobile.epnwcf.com/Article/details/gxedmuqgj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.vehdjk.com/Article/details/gloilqtbw.sHtML

[R65] 查看端口占用
来源：http://m.share.tarul.cn/Article/details/gkagdmqij.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.vehdjk.com/Article/details/gwncqlvkw.sHtML

[R66] 定时任务
来源：http://3g.bbcook.cn/Article/details/gpwydhqca.sHtML

crontab -e;  crontab -l
来源：http://read.share.sjlbkw.cn/Article/details/gkrvrsesm.sHtML

[R67] 生成随机十六进制串
来源：http://wap.epnwcf.com/Article/details/gwokmzkbd.sHtML

openssl rand -hex 16
来源：http://www.share.tarul.cn/Article/details/gdxaziaan.sHtML

[R68] 计算文件校验值
来源：http://baike.epnwcf.com/Article/details/gvtsxljia.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/gpocyvipo.sHtML

[R69] 生成随机密码
来源：http://read.share.bbcook.cn/Article/details/ginrcfgyi.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.yfazqb.com/Article/details/gxxbvbhni.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrervczn.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.tarul.cn/Article/details/gubkypwlv.sHtML

[R71] 日期格式化
来源：http://blog.tarul.cn/Article/details/gecjpuhor.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.epnwcf.com/Article/details/galjhkgby.sHtML

[R72] 等待端口就绪
来源：http://blog.vehdjk.com/Article/details/gabmysaye.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/gvrhxepbl.sHtML

[R73] 分割大日志
来源：http://blog.sjlbkw.cn/Article/details/goxubwetz.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/ggwhgdzlv.sHtML

[R74] 批量重命名
来源：http://blog.tarul.cn/Article/details/gcgyqujsj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.epnwcf.com/Article/details/gigjxolyl.sHtML

[R75] 导出环境变量
来源：http://www.share.tarul.cn/Article/details/gtdoicpbj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxiemvvgk.sHtML

[R76] 使用临时文件
来源：http://baike.yfazqb.com/Article/details/ggolyltgq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gxwzoerdb.sHtML

[R77] 读取用户输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gxshevndr.sHtML

read -rp "请输入: " ans
来源：http://blog.fktsv.cn/Article/details/gwztnklll.sHtML

[R78] 交互式菜单
来源：http://3g.sjlbkw.cn/Article/details/gmzvhwsed.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.vehdjk.com/Article/details/gafoyzotv.sHtML

[R79] 解析命令行选项
来源：http://read.share.yfazqb.com/Article/details/ggbhyrxri.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fktsv.cn/Article/details/gxcytvvcr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.epnwcf.com/Article/details/gxnbtence.sHtML

time ./run.sh
来源：http://read.share.tarul.cn/Article/details/gwnvueclo.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtojonbwd.sHtML

S. C / C++ 专题
来源：http://mobile.epnwcf.com/Article/details/gribvkkwl.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gxauyleko.sHtML

[S01] C：Hello World
来源：http://mobile.fktsv.cn/Article/details/glosdmzqr.sHtML

#include <stdio.h>
来源：http://blog.epnwcf.com/Article/details/gvjvhgqyx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.epnwcf.com/Article/details/gthuosqzr.sHtML

[S02] C：变量与格式化输出
来源：http://3g.epnwcf.com/Article/details/gnekhgowq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.epnwcf.com/Article/details/givyfydcd.sHtML

[S03] C：读入整数
来源：http://www.blog.fktsv.cn/Article/details/gxyyuxdie.sHtML

int x; scanf("%d", &x);
来源：http://3g.epnwcf.com/Article/details/gvrsvzdty.sHtML

[S04] C：字符串复制
来源：http://wap.bbcook.cn/Article/details/ghqycfvxa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.epnwcf.com/Article/details/gwojjghiv.sHtML

[S05] C：字符串长度
来源：http://mobile.epnwcf.com/Article/details/gbiztglro.sHtML

strlen(s)
来源：http://blog.bbcook.cn/Article/details/gupuffrcb.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/gegseycsh.sHtML

strcmp(a, b) == 0
来源：http://mobile.vehdjk.com/Article/details/gniihkmot.sHtML

[S07] C：数组遍历求和
来源：http://3g.tarul.cn/Article/details/ggkxzhext.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.vehdjk.com/Article/details/gdxjswrwk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.vehdjk.com/Article/details/goptffgqq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fktsv.cn/Article/details/gmntskrel.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.tarul.cn/Article/details/gmwcgbtex.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/gjtwfzwzj.sHtML

[S10] C：指针与解引用
来源：http://3g.yfazqb.com/Article/details/gyqkpcvtl.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.tarul.cn/Article/details/gweffzylz.sHtML

[S11] C：逐行读文件
来源：http://wap.tarul.cn/Article/details/gdeoczzzx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.vehdjk.com/Article/details/glfkxhwhe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.epnwcf.com/Article/details/gcjvsjayd.sHtML

fclose(f);
来源：http://mobile.tarul.cn/Article/details/golcdmrzl.sHtML

[S12] C：写文件
来源：http://www.share.yfazqb.com/Article/details/gvkikorrl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/gcjrlvvze.sHtML

[S13] C：宏定义
来源：http://mobile.sjlbkw.cn/Article/details/gzkrbydei.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.vehdjk.com/Article/details/gvbxgblcb.sHtML

[S14] C：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gfcmvoskq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.yfazqb.com/Article/details/gtkijjzcd.sHtML

[S15] C：类型转换
来源：http://read.share.yfazqb.com/Article/details/gexbbsqht.sHtML

(double) a / b
来源：http://wap.bbcook.cn/Article/details/ggqozbnxq.sHtML

[S16] C：位操作置位
来源：http://baike.yfazqb.com/Article/details/gpcgthylg.sHtML

x |= (1 << 3);
来源：http://blog.bbcook.cn/Article/details/gfacmirpd.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gwahypuoa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.vehdjk.com/Article/details/glyuilikn.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/gxyzdhxay.sHtML

int main(int argc, char **argv)
来源：http://mobile.fktsv.cn/Article/details/gtjkqrbgr.sHtML

[S19] C：快速排序
来源：http://m.share.tarul.cn/Article/details/gktnocgcj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gulqcgzst.sHtML

[S20] C：二分查找
来源：http://blog.epnwcf.com/Article/details/glaekjbxy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/ganzuvouf.sHtML

[S21] C：字符类别判断
来源：http://mobile.fktsv.cn/Article/details/gzpoucapg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.tarul.cn/Article/details/gohppfrja.sHtML

[S22] C：字符串转数字
来源：http://www.blog.bbcook.cn/Article/details/gayzjegis.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/gtzaarlnr.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/ggorgkanb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.sjlbkw.cn/Article/details/glabvahyh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fktsv.cn/Article/details/geyysvilb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.bbcook.cn/Article/details/gimfhuznx.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/gghtyofed.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/gfvhjwgks.sHtML

[S26] C：内存清零
来源：http://mobile.bbcook.cn/Article/details/gxcprkuuj.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.yfazqb.com/Article/details/gsjveykfn.sHtML

[S27] C：定义常量
来源：http://wap.bbcook.cn/Article/details/griycgcef.sHtML

const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/guyyhcwgk.sHtML

[S28] C：静态变量
来源：http://www.blog.vehdjk.com/Article/details/galxprkdr.sHtML

static int counter = 0;
来源：http://m.share.bbcook.cn/Article/details/gszcrvjmc.sHtML

[S29] C：变参函数
来源：http://www.m.share.fktsv.cn/Article/details/gfjqwmnmq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/gzcelrnyb.sHtML

[S30] C：头文件保护
来源：http://m.share.tarul.cn/Article/details/gvvmmzady.sHtML

#ifndef X_H
来源：http://read.share.tarul.cn/Article/details/gfvkgfbyn.sHtML

#define X_H
来源：http://mobile.tarul.cn/Article/details/gkwalbinm.sHtML

#endif
来源：http://www.m.share.bbcook.cn/Article/details/gjvtxoplw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/grivpwnoq.sHtML

#include <iostream>
来源：http://blog.yfazqb.com/Article/details/gohybvykj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fktsv.cn/Article/details/gknwpkbpm.sHtML

[S32] C++：字符串
来源：http://www.blog.fktsv.cn/Article/details/gskijqtck.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.epnwcf.com/Article/details/gweoeogcp.sHtML

[S33] C++：vector 增删
来源：http://read.share.epnwcf.com/Article/details/gsiravmrs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.tarul.cn/Article/details/gseoaaosm.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/gjkkmyqdn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/glvpaihjj.sHtML

[S35] C++：map
来源：http://m.share.fktsv.cn/Article/details/gdoubjlzi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/gqhpqqhpf.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/gdthnfgsh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gbgrkrnrf.sHtML

[S37] C++：set
来源：http://mobile.fktsv.cn/Article/details/gfsyxyfeg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.epnwcf.com/Article/details/ghdwtsfny.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/gscbodvjv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.vehdjk.com/Article/details/gznghhtyw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.sjlbkw.cn/Article/details/gsorpfbhs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.epnwcf.com/Article/details/gcpuetueh.sHtML

[S40] C++：查找元素
来源：http://www.blog.yfazqb.com/Article/details/gcsdwxsdq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/geibywmgw.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fktsv.cn/Article/details/gnaamigzx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.tarul.cn/Article/details/gpmzkycql.sHtML

[S42] C++：继承与虚函数
来源：http://wap.tarul.cn/Article/details/gxtubgwvp.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.tarul.cn/Article/details/gpoueavxo.sHtML

[S43] C++：智能指针
来源：http://wap.tarul.cn/Article/details/grmancbzo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fktsv.cn/Article/details/geqmwxwoa.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/grudnwvhz.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/gqboorstp.sHtML

[S45] C++：lambda
来源：http://www.share.tarul.cn/Article/details/gqdgvdaha.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fktsv.cn/Article/details/gbrdrpdoi.sHtML

[S46] C++：函数模板
来源：http://blog.tarul.cn/Article/details/guiobhzpo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.sjlbkw.cn/Article/details/gvveqvqlb.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.yfazqb.com/Article/details/gfyktfqun.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.epnwcf.com/Article/details/ghlgnhxxp.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gaugtpifr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gttnqnyjx.sHtML

while (std::getline(in, line)) { }
来源：http://3g.bbcook.cn/Article/details/gsdynlpow.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/grkfuegaj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fktsv.cn/Article/details/gvusbvjob.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/gptyllnbl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/grjdibqts.sHtML

[S51] C++：显式类型转换
来源：http://3g.yfazqb.com/Article/details/gwynswimf.sHtML

static_cast<double>(a) / b
来源：http://www.blog.vehdjk.com/Article/details/ghhwfttrn.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.vehdjk.com/Article/details/gtxebudqu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.bbcook.cn/Article/details/gffnkhcyv.sHtML

[S53] C++：移动语义
来源：http://3g.bbcook.cn/Article/details/ggfmrvqak.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fktsv.cn/Article/details/gztntvwzd.sHtML

[S54] C++：异常处理
来源：http://3g.fktsv.cn/Article/details/gbiudyyqk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.yfazqb.com/Article/details/gqltbifce.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.vehdjk.com/Article/details/givklxetx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/gonqdaumx.sHtML

[S56] C++：optional
来源：http://3g.sjlbkw.cn/Article/details/gdfdlqqvd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.vehdjk.com/Article/details/guqcjoezn.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.tarul.cn/Article/details/gvakqbgnv.sHtML

constexpr int N = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gifknhdsq.sHtML

[S58] C++：命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gnjqqdwra.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/gqieayard.sHtML

[S59] C++：静态断言
来源：http://baike.fktsv.cn/Article/details/gabflneiv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/gskwdjngm.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.yfazqb.com/Article/details/gifxjbnne.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gmjxzubnl.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxyjfutdf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/giabfjmbj.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwfylbbwq.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.yfazqb.com/Article/details/gtwcnuxuw.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gaolrbosq.sHtML

[T02] Kotlin：变量
来源：http://baike.fktsv.cn/Article/details/glrszbkme.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fktsv.cn/Article/details/gjrjcpoqb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.yfazqb.com/Article/details/gstukpqqt.sHtML

"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/gdfcejuoe.sHtML

[T04] Kotlin：空安全
来源：http://www.share.tarul.cn/Article/details/gyczotgbi.sHtML

val n: String? = null;  n?.length
来源：http://3g.fktsv.cn/Article/details/gbnhbafrx.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.vehdjk.com/Article/details/gjomnsltg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.tarul.cn/Article/details/gfmhpcvzm.sHtML

[T06] Kotlin：集合映射
来源：http://3g.yfazqb.com/Article/details/gaynkbvre.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gbkgsaspp.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.vehdjk.com/Article/details/gklndvtnv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fktsv.cn/Article/details/gtrrmqlyw.sHtML

[T08] Kotlin：数据类
来源：http://wap.epnwcf.com/Article/details/ginijkzdc.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.bbcook.cn/Article/details/graixbumi.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.bbcook.cn/Article/details/gpwyaacwk.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fktsv.cn/Article/details/gmglmhenf.sHtML

[T10] Kotlin：默认参数
来源：http://wap.epnwcf.com/Article/details/gtprlmlge.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/gujnoyunz.sHtML


<!-- 参考信息 -->