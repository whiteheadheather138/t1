代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.tarul.cn/Article/details/gabpjgsqh.sHtML

[R26] 命令替换
来源：http://blog.vehdjk.com/Article/details/gwcutjwng.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.vehdjk.com/Article/details/gijmaycep.sHtML

[R27] 算术展开
来源：http://www.share.epnwcf.com/Article/details/gfzewryln.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.yfazqb.com/Article/details/ghvvumggw.sHtML

[R28] 浮点运算
来源：http://mobile.tarul.cn/Article/details/gjqbgnbyb.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.tarul.cn/Article/details/gzwmvlxrc.sHtML

[R29] 定义函数
来源：http://m.share.epnwcf.com/Article/details/gunssyakw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.epnwcf.com/Article/details/gsexxbpbk.sHtML

[R30] 函数返回状态码
来源：http://mobile.vehdjk.com/Article/details/gmdknfylp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/gvwogwasx.sHtML

[R31] 局部变量
来源：http://blog.fktsv.cn/Article/details/gklukvtff.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.tarul.cn/Article/details/gwaqrzavc.sHtML

[R32] 参数个数校验
来源：http://www.blog.epnwcf.com/Article/details/gtqppduhb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gplhmglum.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fktsv.cn/Article/details/gasswlrke.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.epnwcf.com/Article/details/ghalpvyka.sHtML

[R34] 退出时清理
来源：http://blog.fktsv.cn/Article/details/gfpnpheob.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/ghmoxalrr.sHtML

[R35] 后台执行并等待
来源：http://read.share.vehdjk.com/Article/details/gosnrorkn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.epnwcf.com/Article/details/gjptbvzoi.sHtML

[R36] 并发执行多个任务
来源：http://wap.bbcook.cn/Article/details/gcdrrlvea.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/gwssncgms.sHtML

[R37] 把输出赋给变量
来源：http://baike.epnwcf.com/Article/details/gdkftmvhh.sHtML

files=$(ls -1)
来源：http://mobile.epnwcf.com/Article/details/gguogxskq.sHtML

[R38] 管道串联
来源：http://www.blog.fktsv.cn/Article/details/gzbkyoikn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.epnwcf.com/Article/details/gholclxkn.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.tarul.cn/Article/details/gojwedfbj.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gwxssllwr.sHtML

[R40] 追加写日志
来源：http://www.share.epnwcf.com/Article/details/gxispuofk.sHtML

echo "log" >> out.log
来源：http://wap.vehdjk.com/Article/details/gsemmxdvk.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/gpnvxelmh.sHtML

cmd >/dev/null 2>&1
来源：http://3g.yfazqb.com/Article/details/ghhhbyrqp.sHtML

[R42] 输入重定向
来源：http://www.share.fktsv.cn/Article/details/glvgzirht.sHtML

wc -l < a.txt
来源：http://www.blog.fktsv.cn/Article/details/gicjtlnfo.sHtML

[R43] 按名字查找文件
来源：http://read.share.vehdjk.com/Article/details/gckpbegnd.sHtML

find . -name "*.log" -type f
来源：http://m.share.sjlbkw.cn/Article/details/gdfmehrhr.sHtML

[R44] 按修改时间查找
来源：http://blog.vehdjk.com/Article/details/gqgrmiqcu.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.epnwcf.com/Article/details/gcxdfuyiv.sHtML

[R45] 批量删除
来源：http://mobile.yfazqb.com/Article/details/glulnqgwv.sHtML

find . -name "*.tmp" -delete
来源：http://blog.tarul.cn/Article/details/gzpnbkrmh.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.sjlbkw.cn/Article/details/ghewbwsym.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.sjlbkw.cn/Article/details/gvaistwhv.sHtML

[R47] sed 单行替换
来源：http://3g.yfazqb.com/Article/details/gbihhadfd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.vehdjk.com/Article/details/gjlsmdwfw.sHtML

[R48] awk 取指定列
来源：http://www.m.share.tarul.cn/Article/details/guznvqnpc.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.epnwcf.com/Article/details/gwcfkrzxw.sHtML

[R49] awk 带条件
来源：http://3g.yfazqb.com/Article/details/grfjmdrlr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.sjlbkw.cn/Article/details/gqvtraufd.sHtML

[R50] awk 求和
来源：http://read.share.fktsv.cn/Article/details/gmzkybfwe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.vehdjk.com/Article/details/gmgmvtqpx.sHtML

[R51] 排序去重取前几
来源：http://www.share.bbcook.cn/Article/details/gixuvvjte.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.sjlbkw.cn/Article/details/gaijmtbkj.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/gmeyfiudc.sHtML

wc -l a.txt
来源：http://m.share.vehdjk.com/Article/details/gvaccxslh.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.bbcook.cn/Article/details/gpskdfcxz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fktsv.cn/Article/details/gbfxktnmw.sHtML

[R54] 比较两个文件
来源：http://www.blog.epnwcf.com/Article/details/gzmiazwhn.sHtML

diff a.txt b.txt
来源：http://3g.fktsv.cn/Article/details/gedbfnsbd.sHtML

[R55] 压缩与解压
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpjsjfez.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/gswmaeuha.sHtML

[R56] 远程拷贝
来源：http://blog.fktsv.cn/Article/details/gjdrsgswl.sHtML

scp file user@host:/path/
来源：http://mobile.vehdjk.com/Article/details/goxcifcyf.sHtML

[R57] 远程执行命令
来源：http://3g.fktsv.cn/Article/details/gbgtppukr.sHtML

ssh user@host 'uptime'
来源：http://www.share.tarul.cn/Article/details/gknsgcmrk.sHtML

[R58] 下载文件
来源：http://wap.epnwcf.com/Article/details/gdywwvgal.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.yfazqb.com/Article/details/ggxfbmgbh.sHtML

[R59] 发 POST JSON
来源：http://wap.vehdjk.com/Article/details/ggqlxbntb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.yfazqb.com/Article/details/gvdfydaef.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gjeyztbdl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.vehdjk.com/Article/details/gdkbuuhfr.sHtML

[R61] 磁盘占用
来源：http://mobile.bbcook.cn/Article/details/gpjznqegn.sHtML

df -h;  du -sh *
来源：http://mobile.vehdjk.com/Article/details/gczhwlncc.sHtML

[R62] 找最占空间的文件
来源：http://3g.tarul.cn/Article/details/gsbepranl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.yfazqb.com/Article/details/gdttnkghi.sHtML

[R63] 内存与进程
来源：http://www.blog.fktsv.cn/Article/details/gqjlauhxp.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.bbcook.cn/Article/details/gmnelbagq.sHtML

[R64] 结束进程
来源：http://www.share.fktsv.cn/Article/details/gdxxupuap.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/ghqzjqbyk.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fktsv.cn/Article/details/gxjmuqful.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fktsv.cn/Article/details/gxteqmccq.sHtML

[R66] 定时任务
来源：http://www.share.fktsv.cn/Article/details/gsazovsqy.sHtML

crontab -e;  crontab -l
来源：http://3g.tarul.cn/Article/details/gsbhxgqko.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fktsv.cn/Article/details/gwgowyhst.sHtML

openssl rand -hex 16
来源：http://read.share.sjlbkw.cn/Article/details/gelnngsbj.sHtML

[R68] 计算文件校验值
来源：http://www.blog.tarul.cn/Article/details/gmhcetvii.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.vehdjk.com/Article/details/gzxgaxkwm.sHtML

[R69] 生成随机密码
来源：http://m.share.tarul.cn/Article/details/gjjknzauo.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.sjlbkw.cn/Article/details/gieiijftu.sHtML

[R70] 时间戳与互转
来源：http://read.share.yfazqb.com/Article/details/gjepgaqnr.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/gpjoezyoj.sHtML

[R71] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/gythiyeen.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fktsv.cn/Article/details/gljulxysu.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwepjutl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gdyxxsxqy.sHtML

[R73] 分割大日志
来源：http://baike.bbcook.cn/Article/details/gnlalydss.sHtML

split -l 1000 big.log part_
来源：http://www.share.epnwcf.com/Article/details/gpanhzuov.sHtML

[R74] 批量重命名
来源：http://baike.epnwcf.com/Article/details/gvjwmhqef.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.bbcook.cn/Article/details/gjappekhm.sHtML

[R75] 导出环境变量
来源：http://mobile.epnwcf.com/Article/details/gvnocnisz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.tarul.cn/Article/details/gqetjqpty.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/gdahzracg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/griumfqol.sHtML

[R77] 读取用户输入
来源：http://wap.vehdjk.com/Article/details/gyxmpwexl.sHtML

read -rp "请输入: " ans
来源：http://www.blog.bbcook.cn/Article/details/gclekqoqp.sHtML

[R78] 交互式菜单
来源：http://www.share.yfazqb.com/Article/details/gnzjtoajj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.epnwcf.com/Article/details/gszjynjlh.sHtML

[R79] 解析命令行选项
来源：http://baike.sjlbkw.cn/Article/details/gkjizckwi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.tarul.cn/Article/details/gxyrxprbu.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.vehdjk.com/Article/details/gotpwnbby.sHtML

time ./run.sh
来源：http://www.share.epnwcf.com/Article/details/guyarpqpy.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/giluwuvdc.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/gxdmtbgqn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gollslqny.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gvzsexgcg.sHtML

#include <stdio.h>
来源：http://blog.sjlbkw.cn/Article/details/gcwosxxtf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/gqrjnyyxj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.sjlbkw.cn/Article/details/gasglrxnp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.yfazqb.com/Article/details/gswhzwtfu.sHtML

[S03] C：读入整数
来源：http://www.share.vehdjk.com/Article/details/gmerligpp.sHtML

int x; scanf("%d", &x);
来源：http://blog.sjlbkw.cn/Article/details/gyyfvcemi.sHtML

[S04] C：字符串复制
来源：http://baike.tarul.cn/Article/details/gavylbdkf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.yfazqb.com/Article/details/gucrobfmb.sHtML

[S05] C：字符串长度
来源：http://wap.epnwcf.com/Article/details/gnygwcljl.sHtML

strlen(s)
来源：http://m.share.yfazqb.com/Article/details/gsnjfaght.sHtML

[S06] C：字符串比较
来源：http://blog.tarul.cn/Article/details/gpwzrwmsn.sHtML

strcmp(a, b) == 0
来源：http://3g.bbcook.cn/Article/details/gdquoddob.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gdxvnjdoj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.sjlbkw.cn/Article/details/gldcjkyam.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.yfazqb.com/Article/details/guvymtqva.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/gnonbnzkz.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.vehdjk.com/Article/details/grsbzebaz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/gkgckatiq.sHtML

[S10] C：指针与解引用
来源：http://baike.bbcook.cn/Article/details/gisxbfrgp.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.yfazqb.com/Article/details/gonvtjxre.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/guetrgrzh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fktsv.cn/Article/details/gapyleodx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/grnidcnfx.sHtML

fclose(f);
来源：http://baike.bbcook.cn/Article/details/gjysukekh.sHtML

[S12] C：写文件
来源：http://www.share.vehdjk.com/Article/details/giwkvibem.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gcsgoxsmd.sHtML

[S13] C：宏定义
来源：http://m.share.tarul.cn/Article/details/ghutdwqlu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.yfazqb.com/Article/details/gaqxfhvlb.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/gmfbuudol.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fktsv.cn/Article/details/gdpcnmuki.sHtML

[S15] C：类型转换
来源：http://mobile.epnwcf.com/Article/details/gvkkrwcxg.sHtML

(double) a / b
来源：http://blog.yfazqb.com/Article/details/gfzbiugvi.sHtML

[S16] C：位操作置位
来源：http://mobile.bbcook.cn/Article/details/gscutoxxn.sHtML

x |= (1 << 3);
来源：http://www.share.epnwcf.com/Article/details/gillhbaaq.sHtML

[S17] C：安全拼接字符串
来源：http://blog.yfazqb.com/Article/details/gfpreuran.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.epnwcf.com/Article/details/gyzipsprn.sHtML

[S18] C：命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gndgvisov.sHtML

int main(int argc, char **argv)
来源：http://wap.fktsv.cn/Article/details/gmrusjlez.sHtML

[S19] C：快速排序
来源：http://blog.sjlbkw.cn/Article/details/gcgwthhcs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.yfazqb.com/Article/details/ghmbxttse.sHtML

[S20] C：二分查找
来源：http://mobile.vehdjk.com/Article/details/gatjzysed.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gxppuotjx.sHtML

[S21] C：字符类别判断
来源：http://baike.yfazqb.com/Article/details/gfqtmkoqm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.epnwcf.com/Article/details/gnxsoxiqz.sHtML

[S22] C：字符串转数字
来源：http://wap.yfazqb.com/Article/details/gkcduvzry.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.sjlbkw.cn/Article/details/gxcxeqkgd.sHtML

[S23] C：随机数
来源：http://mobile.epnwcf.com/Article/details/ghwblimrv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.sjlbkw.cn/Article/details/gixkbhqyv.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/gylaapslj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fktsv.cn/Article/details/gazuhjqsz.sHtML

[S25] C：内存拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gfkkvglut.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gzknzwjgc.sHtML

[S26] C：内存清零
来源：http://baike.sjlbkw.cn/Article/details/gnqkoikpr.sHtML

memset(a, 0, sizeof a);
来源：http://baike.bbcook.cn/Article/details/grdzhnxda.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gvovaojne.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/grcdrkazx.sHtML

[S28] C：静态变量
来源：http://m.share.yfazqb.com/Article/details/gaooouuxs.sHtML

static int counter = 0;
来源：http://www.blog.bbcook.cn/Article/details/gnbgvykvp.sHtML

[S29] C：变参函数
来源：http://3g.vehdjk.com/Article/details/guvqqfwux.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.tarul.cn/Article/details/gflmdezku.sHtML

[S30] C：头文件保护
来源：http://read.share.epnwcf.com/Article/details/gvviixfpd.sHtML

#ifndef X_H
来源：http://m.share.yfazqb.com/Article/details/gofgnrytz.sHtML

#define X_H
来源：http://read.share.fktsv.cn/Article/details/gkeoutpea.sHtML

#endif
来源：http://baike.bbcook.cn/Article/details/gkwgohfmw.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/gxobuyils.sHtML

#include <iostream>
来源：http://wap.tarul.cn/Article/details/grkcotucq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fktsv.cn/Article/details/gzexouptk.sHtML

[S32] C++：字符串
来源：http://m.share.tarul.cn/Article/details/gnedefude.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.vehdjk.com/Article/details/grmmedkcg.sHtML

[S33] C++：vector 增删
来源：http://wap.bbcook.cn/Article/details/ggbqzrivv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.vehdjk.com/Article/details/gzsgwwydp.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.sjlbkw.cn/Article/details/gksbcoias.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.yfazqb.com/Article/details/gvcirutac.sHtML

[S35] C++：map
来源：http://m.share.tarul.cn/Article/details/gamwxyybj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gqqdldykb.sHtML

[S36] C++：unordered_map
来源：http://wap.vehdjk.com/Article/details/gppuyltjo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/gbwuyjywm.sHtML

[S37] C++：set
来源：http://m.share.epnwcf.com/Article/details/gebhjogyw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.sjlbkw.cn/Article/details/gbtxtknns.sHtML

[S38] C++：排序
来源：http://www.share.tarul.cn/Article/details/gghmgphao.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.tarul.cn/Article/details/gcbnwgigc.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.bbcook.cn/Article/details/gkzdmvnba.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.epnwcf.com/Article/details/gmyspvwnv.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/ghiutmukr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.sjlbkw.cn/Article/details/gzylrafpu.sHtML

[S41] C++：类与构造函数
来源：http://blog.fktsv.cn/Article/details/gdbernzkg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fktsv.cn/Article/details/ghmdlceyl.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fktsv.cn/Article/details/gpnipzamj.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.sjlbkw.cn/Article/details/gnezgmsfl.sHtML

[S43] C++：智能指针
来源：http://m.share.sjlbkw.cn/Article/details/ghzzxivma.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.vehdjk.com/Article/details/gbngkvjdv.sHtML

[S44] C++：引用传参
来源：http://blog.epnwcf.com/Article/details/ggqwqxzvd.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/gbqwimuyp.sHtML

[S45] C++：lambda
来源：http://blog.epnwcf.com/Article/details/guhhlmcml.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.sjlbkw.cn/Article/details/gjgqsgosd.sHtML

[S46] C++：函数模板
来源：http://www.blog.sjlbkw.cn/Article/details/gaulfzuwv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.bbcook.cn/Article/details/gpkugxwpy.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.tarul.cn/Article/details/gsfjzquro.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.bbcook.cn/Article/details/grtkitwor.sHtML

[S48] C++：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gfcmoixln.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.bbcook.cn/Article/details/ggsnclufz.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.tarul.cn/Article/details/gzbjhrvrt.sHtML

[S49] C++：写文件
来源：http://www.blog.yfazqb.com/Article/details/gpftwqasu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fktsv.cn/Article/details/gsjkgwofc.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/gatknubon.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gfepiptec.sHtML

[S51] C++：显式类型转换
来源：http://read.share.vehdjk.com/Article/details/gtzerozgq.sHtML

static_cast<double>(a) / b
来源：http://m.share.tarul.cn/Article/details/glwouwygf.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/gmirmwvtf.sHtML

int size() const noexcept { return n_; }
来源：http://blog.tarul.cn/Article/details/gtcvrbbcy.sHtML

[S53] C++：移动语义
来源：http://blog.yfazqb.com/Article/details/gqusyxkgo.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fktsv.cn/Article/details/gwcogszqt.sHtML

[S54] C++：异常处理
来源：http://3g.yfazqb.com/Article/details/gklqkpvup.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.bbcook.cn/Article/details/gfxubnbpc.sHtML

[S55] C++：结构化绑定
来源：http://m.share.yfazqb.com/Article/details/gywxnhoei.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/gztkxnryl.sHtML

[S56] C++：optional
来源：http://m.share.vehdjk.com/Article/details/gwkxabblx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.yfazqb.com/Article/details/gglmbbssg.sHtML

[S57] C++：编译期常量
来源：http://www.blog.tarul.cn/Article/details/gulkitfnv.sHtML

constexpr int N = 10;
来源：http://mobile.epnwcf.com/Article/details/gdkimvngz.sHtML

[S58] C++：命名空间
来源：http://www.m.share.bbcook.cn/Article/details/gppbljyyr.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.bbcook.cn/Article/details/gerakamwn.sHtML

[S59] C++：静态断言
来源：http://m.share.epnwcf.com/Article/details/gxjjfyohr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.tarul.cn/Article/details/gdjgcaobo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gqngbodrg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.bbcook.cn/Article/details/geazegfmj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtloffkms.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/gqbjlefhb.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gekxcunao.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.epnwcf.com/Article/details/gyefisshg.sHtML

println("Hello")
来源：http://read.share.vehdjk.com/Article/details/gcpjdtyey.sHtML

[T02] Kotlin：变量
来源：http://read.share.bbcook.cn/Article/details/gclhjkhpi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fktsv.cn/Article/details/gbbbvqevb.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.vehdjk.com/Article/details/gcqygenqb.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/gonxnwbvg.sHtML

[T04] Kotlin：空安全
来源：http://3g.fktsv.cn/Article/details/gimkyadng.sHtML

val n: String? = null;  n?.length
来源：http://baike.tarul.cn/Article/details/gfpwhbzbs.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.bbcook.cn/Article/details/gmhhqbkan.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gopmdukog.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fktsv.cn/Article/details/gxjookejy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fktsv.cn/Article/details/gkbmsctnz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gzjorozoq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fktsv.cn/Article/details/gufaprfyx.sHtML

[T08] Kotlin：数据类
来源：http://mobile.vehdjk.com/Article/details/gezlknxxv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/gpivdxpgj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fktsv.cn/Article/details/gvnttkgxt.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.vehdjk.com/Article/details/gpiuscqqr.sHtML

[T10] Kotlin：默认参数
来源：http://3g.tarul.cn/Article/details/gfmjjlxmu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.epnwcf.com/Article/details/goexiqocv.sHtML

[T11] Kotlin：协程
来源：http://m.share.vehdjk.com/Article/details/gpyemwphc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.tarul.cn/Article/details/gserfkkbt.sHtML

[T12] Kotlin：解构声明
来源：http://blog.sjlbkw.cn/Article/details/gutevhczc.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.epnwcf.com/Article/details/gygzfncfl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/gtdvdzyvx.sHtML

val m = mapOf("a" to 1)
来源：http://3g.tarul.cn/Article/details/gljxxqnna.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/glrbyzdeo.sHtML

for (i in 1..10) println(i)
来源：http://baike.yfazqb.com/Article/details/gdzubtcef.sHtML

[T15] Kotlin：接口
来源：http://baike.fktsv.cn/Article/details/geuykxbmd.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/gpizqblgv.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gauoanaow.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/gpndmyvxs.sHtML

[T17] Swift：变量与常量
来源：http://read.share.epnwcf.com/Article/details/guaxioffn.sHtML

var a = 1;  let b = 2
来源：http://wap.sjlbkw.cn/Article/details/gusaraore.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/grvguajtj.sHtML

"值: \(b)"
来源：http://www.m.share.vehdjk.com/Article/details/gjhbpsjfe.sHtML

[T19] Swift：可选绑定
来源：http://read.share.tarul.cn/Article/details/gtbiupwzp.sHtML

if let n = opt { print(n) }
来源：http://blog.tarul.cn/Article/details/gkvsooaej.sHtML

[T20] Swift：数组操作
来源：http://blog.yfazqb.com/Article/details/gernexzyt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/gujgywzib.sHtML

[T21] Swift：遍历
来源：http://www.m.share.bbcook.cn/Article/details/gtmsufoom.sHtML

for x in a { print(x) }
来源：http://wap.sjlbkw.cn/Article/details/gpnpsdobz.sHtML

[T22] Swift：字典
来源：http://baike.yfazqb.com/Article/details/gfbtvkjpu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.yfazqb.com/Article/details/grxzfrnfb.sHtML

[T23] Swift：函数
来源：http://blog.tarul.cn/Article/details/guqjkamtf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.yfazqb.com/Article/details/gdotbhxtf.sHtML

[T24] Swift：闭包
来源：http://www.blog.sjlbkw.cn/Article/details/guufpavpb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gczpdxcyb.sHtML

[T25] Swift：结构体
来源：http://blog.epnwcf.com/Article/details/gresgurhe.sHtML

struct P { var x: Int }
来源：http://www.blog.tarul.cn/Article/details/ghtlttnkn.sHtML

[T26] Swift：类与重写
来源：http://read.share.fktsv.cn/Article/details/gdavgjcgm.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.vehdjk.com/Article/details/goscjvdon.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.vehdjk.com/Article/details/gredsnjfd.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.bbcook.cn/Article/details/gpieeqbgj.sHtML

[T28] Swift：枚举
来源：http://3g.bbcook.cn/Article/details/gekpljvik.sHtML

enum Color { case red, green }
来源：http://www.m.share.sjlbkw.cn/Article/details/geouutoej.sHtML


<!-- 参考信息 -->