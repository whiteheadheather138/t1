代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.tarul.cn/Article/details/glykqitue.sHtML

[R24] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gxhzmoibn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.epnwcf.com/Article/details/gtfqkxvml.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fktsv.cn/Article/details/gibjvjuur.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/gjxpckvtn.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/ghmcxvwrz.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fktsv.cn/Article/details/gplavrfbo.sHtML

[R27] 算术展开
来源：http://read.share.epnwcf.com/Article/details/gseaakqxn.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.sjlbkw.cn/Article/details/gklbtocdq.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gpxnipkub.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.tarul.cn/Article/details/ggomcqinh.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gpmxujauw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.bbcook.cn/Article/details/gsmxivics.sHtML

[R30] 函数返回状态码
来源：http://www.share.tarul.cn/Article/details/gbmgzdtlf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.vehdjk.com/Article/details/gjdxljpzh.sHtML

[R31] 局部变量
来源：http://3g.sjlbkw.cn/Article/details/ghfyyhmob.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.yfazqb.com/Article/details/gplmvlheo.sHtML

[R32] 参数个数校验
来源：http://www.blog.vehdjk.com/Article/details/gsbmlonwc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/gfqpzinoy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.epnwcf.com/Article/details/gizeppayx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.yfazqb.com/Article/details/gnkhzqdmg.sHtML

[R34] 退出时清理
来源：http://www.m.share.vehdjk.com/Article/details/gsqotafqw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gexkpvskv.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/gopobiimf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.epnwcf.com/Article/details/gtepvfozd.sHtML

[R36] 并发执行多个任务
来源：http://baike.vehdjk.com/Article/details/gpmjzpblc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fktsv.cn/Article/details/gsziczpza.sHtML

[R37] 把输出赋给变量
来源：http://baike.bbcook.cn/Article/details/gpwxpygnw.sHtML

files=$(ls -1)
来源：http://baike.yfazqb.com/Article/details/gtlvmowrv.sHtML

[R38] 管道串联
来源：http://baike.fktsv.cn/Article/details/gobfrvjut.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.epnwcf.com/Article/details/ghyhgfxjh.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.yfazqb.com/Article/details/ghvwsgfnr.sHtML

cmd > out.log 2>&1
来源：http://mobile.epnwcf.com/Article/details/gmjjyhjom.sHtML

[R40] 追加写日志
来源：http://m.share.bbcook.cn/Article/details/gpwsbnlgy.sHtML

echo "log" >> out.log
来源：http://blog.bbcook.cn/Article/details/gyjkiapoa.sHtML

[R41] 丢弃输出
来源：http://baike.fktsv.cn/Article/details/gprlizfbj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fktsv.cn/Article/details/getbbvpat.sHtML

[R42] 输入重定向
来源：http://mobile.fktsv.cn/Article/details/ghpjymewk.sHtML

wc -l < a.txt
来源：http://wap.sjlbkw.cn/Article/details/gshrmjyck.sHtML

[R43] 按名字查找文件
来源：http://www.blog.epnwcf.com/Article/details/gvyhwgxis.sHtML

find . -name "*.log" -type f
来源：http://www.share.epnwcf.com/Article/details/gscqojgxy.sHtML

[R44] 按修改时间查找
来源：http://3g.epnwcf.com/Article/details/gojtbyydg.sHtML

find . -mtime -7 -type f
来源：http://blog.yfazqb.com/Article/details/gmvlyfzrl.sHtML

[R45] 批量删除
来源：http://www.share.tarul.cn/Article/details/glotuexoq.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.tarul.cn/Article/details/gfkvjgdwq.sHtML

[R46] 递归替换文件内容
来源：http://read.share.sjlbkw.cn/Article/details/gnjxzqgad.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fktsv.cn/Article/details/gwmctaehm.sHtML

[R47] sed 单行替换
来源：http://baike.epnwcf.com/Article/details/gnllcofam.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gkbyfszdt.sHtML

[R48] awk 取指定列
来源：http://wap.tarul.cn/Article/details/gkeqhcgqi.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.vehdjk.com/Article/details/gnxqnbcsx.sHtML

[R49] awk 带条件
来源：http://m.share.yfazqb.com/Article/details/gfjagjimi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.yfazqb.com/Article/details/gzflrkwnm.sHtML

[R50] awk 求和
来源：http://www.share.sjlbkw.cn/Article/details/gifktgcrj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.yfazqb.com/Article/details/gaqllokat.sHtML

[R51] 排序去重取前几
来源：http://3g.tarul.cn/Article/details/gbpleioee.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/gkoanorvu.sHtML

[R52] 统计行数
来源：http://3g.bbcook.cn/Article/details/glapxkioj.sHtML

wc -l a.txt
来源：http://www.share.tarul.cn/Article/details/gqyehqmag.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.sjlbkw.cn/Article/details/gpdsdnebo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.vehdjk.com/Article/details/gtxapegis.sHtML

[R54] 比较两个文件
来源：http://wap.yfazqb.com/Article/details/gbwdvcsgh.sHtML

diff a.txt b.txt
来源：http://www.m.share.tarul.cn/Article/details/ggorjcvvw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.epnwcf.com/Article/details/gmzweyqut.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.epnwcf.com/Article/details/gfaysnjlm.sHtML

[R56] 远程拷贝
来源：http://baike.fktsv.cn/Article/details/gdcprpygm.sHtML

scp file user@host:/path/
来源：http://www.m.share.yfazqb.com/Article/details/gacnvgqij.sHtML

[R57] 远程执行命令
来源：http://3g.epnwcf.com/Article/details/gzhaifwiq.sHtML

ssh user@host 'uptime'
来源：http://mobile.sjlbkw.cn/Article/details/glxcoljcx.sHtML

[R58] 下载文件
来源：http://blog.sjlbkw.cn/Article/details/grupwotom.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fktsv.cn/Article/details/gpsbqycmq.sHtML

[R59] 发 POST JSON
来源：http://read.share.tarul.cn/Article/details/gmsddmhtu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmthefqs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/gecubexrh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.yfazqb.com/Article/details/gbjlewhcd.sHtML

[R61] 磁盘占用
来源：http://3g.vehdjk.com/Article/details/gfgolvyoh.sHtML

df -h;  du -sh *
来源：http://wap.sjlbkw.cn/Article/details/gteldlxsg.sHtML

[R62] 找最占空间的文件
来源：http://read.share.yfazqb.com/Article/details/gkqdmavas.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/gahbsrqmd.sHtML

[R63] 内存与进程
来源：http://3g.bbcook.cn/Article/details/ggizpxzgx.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.epnwcf.com/Article/details/geqdweowi.sHtML

[R64] 结束进程
来源：http://www.share.yfazqb.com/Article/details/gryshgjfb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.vehdjk.com/Article/details/gldboytkk.sHtML

[R65] 查看端口占用
来源：http://mobile.tarul.cn/Article/details/gbxyhzzus.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.sjlbkw.cn/Article/details/graforqih.sHtML

[R66] 定时任务
来源：http://www.blog.tarul.cn/Article/details/ggzuykuoh.sHtML

crontab -e;  crontab -l
来源：http://mobile.bbcook.cn/Article/details/ggsoqdjtn.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/gmmppkosr.sHtML

openssl rand -hex 16
来源：http://wap.yfazqb.com/Article/details/gnltguxjh.sHtML

[R68] 计算文件校验值
来源：http://www.share.bbcook.cn/Article/details/gjvurhbdq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gzblfrshz.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fktsv.cn/Article/details/glqccosmd.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.tarul.cn/Article/details/gldiovhuy.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fktsv.cn/Article/details/gzbravjzq.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fktsv.cn/Article/details/gfjotbqsb.sHtML

[R71] 日期格式化
来源：http://3g.yfazqb.com/Article/details/glgajtuth.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.tarul.cn/Article/details/gyqoqfyeb.sHtML

[R72] 等待端口就绪
来源：http://mobile.sjlbkw.cn/Article/details/gvoiumrqy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gfmxbtrnu.sHtML

[R73] 分割大日志
来源：http://wap.yfazqb.com/Article/details/gbxhhsskg.sHtML

split -l 1000 big.log part_
来源：http://3g.bbcook.cn/Article/details/gpcixbxfk.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/gwfiqjszc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.epnwcf.com/Article/details/grlftimeg.sHtML

[R75] 导出环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gbwghwims.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.bbcook.cn/Article/details/gbtitvduz.sHtML

[R76] 使用临时文件
来源：http://m.share.vehdjk.com/Article/details/gyftirtzt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/gpfeekjwm.sHtML

[R77] 读取用户输入
来源：http://wap.epnwcf.com/Article/details/gzycdwujg.sHtML

read -rp "请输入: " ans
来源：http://www.blog.yfazqb.com/Article/details/ghiltlyom.sHtML

[R78] 交互式菜单
来源：http://blog.fktsv.cn/Article/details/gswzubyaw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.epnwcf.com/Article/details/ghrjkyoms.sHtML

[R79] 解析命令行选项
来源：http://mobile.bbcook.cn/Article/details/goomqhktw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.sjlbkw.cn/Article/details/gqgwecczl.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.vehdjk.com/Article/details/gwanayapf.sHtML

time ./run.sh
来源：http://wap.tarul.cn/Article/details/gnpheqqwx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gdikgixzj.sHtML

S. C / C++ 专题
来源：http://www.share.sjlbkw.cn/Article/details/gptmzqpzj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grirqufll.sHtML

[S01] C：Hello World
来源：http://blog.vehdjk.com/Article/details/gpxhdlmsa.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/gmfvmaydi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.bbcook.cn/Article/details/gqkvvaney.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.epnwcf.com/Article/details/gjdqnrgra.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/gnodktrsx.sHtML

[S03] C：读入整数
来源：http://www.blog.tarul.cn/Article/details/gyoewyydi.sHtML

int x; scanf("%d", &x);
来源：http://www.share.yfazqb.com/Article/details/gwszzguxx.sHtML

[S04] C：字符串复制
来源：http://read.share.bbcook.cn/Article/details/gflnjflei.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.sjlbkw.cn/Article/details/ghseclpoi.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gjxxvnvev.sHtML

strlen(s)
来源：http://www.blog.yfazqb.com/Article/details/gdoeexkzn.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/gjbvroqdp.sHtML

strcmp(a, b) == 0
来源：http://mobile.bbcook.cn/Article/details/gpmbvmwal.sHtML

[S07] C：数组遍历求和
来源：http://mobile.tarul.cn/Article/details/gygfjgirv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.tarul.cn/Article/details/gahkjeqse.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.vehdjk.com/Article/details/ghrnvaqbx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.tarul.cn/Article/details/gcjirabii.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.tarul.cn/Article/details/gmgmtlsnk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.sjlbkw.cn/Article/details/gxsjaizog.sHtML

[S10] C：指针与解引用
来源：http://www.share.fktsv.cn/Article/details/gypuljmmd.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.yfazqb.com/Article/details/gefieggav.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gqupyiqfa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.bbcook.cn/Article/details/gfphrjaef.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.vehdjk.com/Article/details/gomqcmkwj.sHtML

fclose(f);
来源：http://www.share.tarul.cn/Article/details/ghyzojpjf.sHtML

[S12] C：写文件
来源：http://wap.fktsv.cn/Article/details/gbjiullsb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.tarul.cn/Article/details/gwfhiitju.sHtML

[S13] C：宏定义
来源：http://blog.sjlbkw.cn/Article/details/gvtlhhbja.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.epnwcf.com/Article/details/gbtefeeth.sHtML

[S14] C：枚举
来源：http://3g.yfazqb.com/Article/details/ghysmumeb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/gvsowbwph.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/gunopkkdq.sHtML

(double) a / b
来源：http://baike.tarul.cn/Article/details/gglnmypuh.sHtML

[S16] C：位操作置位
来源：http://m.share.vehdjk.com/Article/details/gsvyrfbit.sHtML

x |= (1 << 3);
来源：http://wap.sjlbkw.cn/Article/details/ggljkkikq.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gkwzxvqoa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.tarul.cn/Article/details/grahssakt.sHtML

[S18] C：命令行参数
来源：http://www.blog.tarul.cn/Article/details/gjaonaacs.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fktsv.cn/Article/details/gohpsvrak.sHtML

[S19] C：快速排序
来源：http://m.share.fktsv.cn/Article/details/gyfpxgnlv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gcakhmura.sHtML

[S20] C：二分查找
来源：http://www.share.fktsv.cn/Article/details/gendbyugp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/ginhskvsu.sHtML

[S21] C：字符类别判断
来源：http://3g.sjlbkw.cn/Article/details/grgubpxoa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.yfazqb.com/Article/details/gjrrfhmyo.sHtML

[S22] C：字符串转数字
来源：http://m.share.yfazqb.com/Article/details/gwicmystp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.sjlbkw.cn/Article/details/gijticdzz.sHtML

[S23] C：随机数
来源：http://read.share.tarul.cn/Article/details/gjtrwfctu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/graarmbdy.sHtML

[S24] C：获取本地时间
来源：http://m.share.tarul.cn/Article/details/gcxnqqbeh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/gehdqhcfb.sHtML

[S25] C：内存拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gvcxqrczu.sHtML

memcpy(dst, src, n);
来源：http://m.share.vehdjk.com/Article/details/govwlsnob.sHtML

[S26] C：内存清零
来源：http://read.share.fktsv.cn/Article/details/gffxeejcb.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fktsv.cn/Article/details/gbsemtdiq.sHtML

[S27] C：定义常量
来源：http://www.share.epnwcf.com/Article/details/girlkxhnf.sHtML

const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gubvnhtug.sHtML

[S28] C：静态变量
来源：http://blog.tarul.cn/Article/details/gzicuqhie.sHtML

static int counter = 0;
来源：http://m.share.epnwcf.com/Article/details/ggaqhidej.sHtML

[S29] C：变参函数
来源：http://read.share.tarul.cn/Article/details/gihjutuvj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.bbcook.cn/Article/details/godkvuewi.sHtML

[S30] C：头文件保护
来源：http://mobile.sjlbkw.cn/Article/details/gabxmzhzs.sHtML

#ifndef X_H
来源：http://wap.epnwcf.com/Article/details/gkjunxfqc.sHtML

#define X_H
来源：http://www.m.share.tarul.cn/Article/details/gachoeiig.sHtML

#endif
来源：http://blog.yfazqb.com/Article/details/gmlosivry.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/geujnkfok.sHtML

#include <iostream>
来源：http://www.m.share.epnwcf.com/Article/details/gwvqwbdhj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.bbcook.cn/Article/details/ggmtozhlf.sHtML

[S32] C++：字符串
来源：http://m.share.tarul.cn/Article/details/gtektdizd.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fktsv.cn/Article/details/gbymzdtmg.sHtML

[S33] C++：vector 增删
来源：http://read.share.sjlbkw.cn/Article/details/gcevdujtm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.vehdjk.com/Article/details/gedztmwhz.sHtML

[S34] C++：遍历 vector
来源：http://blog.fktsv.cn/Article/details/gbeohlwwv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.sjlbkw.cn/Article/details/gxxzptird.sHtML

[S35] C++：map
来源：http://www.share.sjlbkw.cn/Article/details/gsaqmqodr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/glwimdtfd.sHtML

[S36] C++：unordered_map
来源：http://read.share.fktsv.cn/Article/details/gjofsfwpk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/gfiwdtmnp.sHtML

[S37] C++：set
来源：http://wap.tarul.cn/Article/details/gqtftcgfg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.bbcook.cn/Article/details/gdibnnaxo.sHtML

[S38] C++：排序
来源：http://www.share.epnwcf.com/Article/details/gllsinxzb.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.epnwcf.com/Article/details/gsebdrmmm.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.yfazqb.com/Article/details/gyvnphajd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.bbcook.cn/Article/details/gbbpwcjem.sHtML

[S40] C++：查找元素
来源：http://wap.bbcook.cn/Article/details/ghquunljb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.sjlbkw.cn/Article/details/glhymnzvn.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.yfazqb.com/Article/details/guvmcgdca.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.bbcook.cn/Article/details/gkyfoqztj.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/gpvfzmhbn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.yfazqb.com/Article/details/gogobgfef.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gwxjiewgb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.epnwcf.com/Article/details/guvtwrrms.sHtML

[S44] C++：引用传参
来源：http://blog.vehdjk.com/Article/details/gzshiybbr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.epnwcf.com/Article/details/gigqgqaji.sHtML

[S45] C++：lambda
来源：http://www.blog.yfazqb.com/Article/details/gedovstgn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.sjlbkw.cn/Article/details/gvtrygphd.sHtML

[S46] C++：函数模板
来源：http://www.m.share.vehdjk.com/Article/details/gmjrnimab.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.yfazqb.com/Article/details/gvwikbdal.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.epnwcf.com/Article/details/ggqhuzavy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.tarul.cn/Article/details/gilwtzahd.sHtML

[S48] C++：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gescorvpm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.tarul.cn/Article/details/gtsyzxjvd.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/gxyfvplek.sHtML

[S49] C++：写文件
来源：http://www.share.vehdjk.com/Article/details/gbfehcuxc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.yfazqb.com/Article/details/gzfgtavfs.sHtML

[S50] C++：格式化数字
来源：http://mobile.tarul.cn/Article/details/gwbrgjiar.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gjwbgiols.sHtML

[S51] C++：显式类型转换
来源：http://blog.tarul.cn/Article/details/giobuvsus.sHtML

static_cast<double>(a) / b
来源：http://mobile.tarul.cn/Article/details/gqnmctspe.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.epnwcf.com/Article/details/glmbscswj.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.epnwcf.com/Article/details/gafvidctj.sHtML

[S53] C++：移动语义
来源：http://baike.sjlbkw.cn/Article/details/gtfxvdivj.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.sjlbkw.cn/Article/details/gqbjemdgm.sHtML

[S54] C++：异常处理
来源：http://www.blog.vehdjk.com/Article/details/gkbhkkakz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fktsv.cn/Article/details/gyeggvwju.sHtML

[S55] C++：结构化绑定
来源：http://blog.vehdjk.com/Article/details/gwsxtcbgd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gpxsmmrvp.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/gfmaqdnqv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.sjlbkw.cn/Article/details/gwszdodkq.sHtML

[S57] C++：编译期常量
来源：http://m.share.tarul.cn/Article/details/gyqauncdo.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/gaorptwdp.sHtML

[S58] C++：命名空间
来源：http://3g.fktsv.cn/Article/details/gsjvvfwbm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.bbcook.cn/Article/details/gncnwcubv.sHtML

[S59] C++：静态断言
来源：http://read.share.epnwcf.com/Article/details/gycndytba.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.sjlbkw.cn/Article/details/gdtjsylfk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.bbcook.cn/Article/details/gfuvsormr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gyjjnfnxs.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzvebkvnk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.vehdjk.com/Article/details/gujunewjv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/grjlfgxwm.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.bbcook.cn/Article/details/ggqljtjef.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gluifyqbf.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.epnwcf.com/Article/details/gnbrkvxaf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.epnwcf.com/Article/details/gclsywzit.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.bbcook.cn/Article/details/gctrblvuz.sHtML

"值: $b"
来源：http://blog.epnwcf.com/Article/details/gdkvdkutm.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gtvsyhcsp.sHtML

val n: String? = null;  n?.length
来源：http://wap.epnwcf.com/Article/details/ggihmttof.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.yfazqb.com/Article/details/gblznmrbm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.epnwcf.com/Article/details/gxnjsadne.sHtML

[T06] Kotlin：集合映射
来源：http://3g.sjlbkw.cn/Article/details/gtokllcxa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.bbcook.cn/Article/details/gvgrnzwyo.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.tarul.cn/Article/details/glaccolen.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.vehdjk.com/Article/details/gxzrntbri.sHtML

[T08] Kotlin：数据类
来源：http://baike.fktsv.cn/Article/details/gmnzpotle.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.epnwcf.com/Article/details/gughfjdzn.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fktsv.cn/Article/details/gvfxbebwc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.sjlbkw.cn/Article/details/gvsmdzyrx.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fktsv.cn/Article/details/gbuuhohxt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.vehdjk.com/Article/details/gxawxzegd.sHtML

[T11] Kotlin：协程
来源：http://read.share.bbcook.cn/Article/details/gxvwcerpk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.bbcook.cn/Article/details/ghomogogr.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.epnwcf.com/Article/details/geefmozwi.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.vehdjk.com/Article/details/gwepizypr.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fktsv.cn/Article/details/gkfswobdk.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.yfazqb.com/Article/details/gtaqauiht.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gjqsfzsjv.sHtML

for (i in 1..10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/gughlczcj.sHtML

[T15] Kotlin：接口
来源：http://mobile.fktsv.cn/Article/details/ggqfysyif.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/gqwyjjhnc.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gycmhrfkv.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gfidaqufh.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.yfazqb.com/Article/details/gfuddikdx.sHtML

var a = 1;  let b = 2
来源：http://m.share.epnwcf.com/Article/details/gdrsskyue.sHtML

[T18] Swift：字符串插值
来源：http://m.share.tarul.cn/Article/details/ghwxuleoo.sHtML

"值: \(b)"
来源：http://www.share.vehdjk.com/Article/details/gxfvyhzin.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/gwwtiipmz.sHtML

if let n = opt { print(n) }
来源：http://mobile.vehdjk.com/Article/details/gitutdzfw.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.sjlbkw.cn/Article/details/guojejgvi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.yfazqb.com/Article/details/gbdkdccva.sHtML

[T21] Swift：遍历
来源：http://baike.fktsv.cn/Article/details/gizbouyqt.sHtML

for x in a { print(x) }
来源：http://www.blog.vehdjk.com/Article/details/gbjhaduzs.sHtML

[T22] Swift：字典
来源：http://mobile.epnwcf.com/Article/details/gmbegyoop.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.yfazqb.com/Article/details/gjnasbbth.sHtML

[T23] Swift：函数
来源：http://read.share.epnwcf.com/Article/details/gmiezifnm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.vehdjk.com/Article/details/gahiolggt.sHtML

[T24] Swift：闭包
来源：http://mobile.epnwcf.com/Article/details/glogejyjl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.yfazqb.com/Article/details/gopzoumpg.sHtML

[T25] Swift：结构体
来源：http://m.share.sjlbkw.cn/Article/details/gnsbwdofv.sHtML

struct P { var x: Int }
来源：http://3g.sjlbkw.cn/Article/details/gfeoeogmb.sHtML

[T26] Swift：类与重写
来源：http://mobile.vehdjk.com/Article/details/goefpvppu.sHtML

class A: Base { override func f() {} }
来源：http://mobile.sjlbkw.cn/Article/details/gfszvbmfl.sHtML


<!-- 参考信息 -->