代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.bbcook.cn/Article/details/gjbpytdcn.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gxomjqpym.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.sjlbkw.cn/Article/details/gtnujbysw.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.sjlbkw.cn/Article/details/gvahfuikf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gdobdjanh.sHtML

[R26] 命令替换
来源：http://www.m.share.yfazqb.com/Article/details/gofehsami.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.sjlbkw.cn/Article/details/ggofpnesk.sHtML

[R27] 算术展开
来源：http://wap.bbcook.cn/Article/details/gsyjfqqhn.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.bbcook.cn/Article/details/gjlculfbu.sHtML

[R28] 浮点运算
来源：http://www.share.yfazqb.com/Article/details/gqfbqxphz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fktsv.cn/Article/details/gkmjreqhr.sHtML

[R29] 定义函数
来源：http://wap.vehdjk.com/Article/details/ggljxyijf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.tarul.cn/Article/details/gphrzalgp.sHtML

[R30] 函数返回状态码
来源：http://3g.bbcook.cn/Article/details/gizrzotsi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/gqtvebdzb.sHtML

[R31] 局部变量
来源：http://wap.epnwcf.com/Article/details/gkzjsqanb.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.tarul.cn/Article/details/gruelkqmv.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fktsv.cn/Article/details/glvxjxssk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gtprjeseg.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.sjlbkw.cn/Article/details/gvebyhxgu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.vehdjk.com/Article/details/giiznwwdw.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/guuhhpizt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/gxwpffcpt.sHtML

[R35] 后台执行并等待
来源：http://wap.tarul.cn/Article/details/grugjofzk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.tarul.cn/Article/details/gdzyelpgr.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.epnwcf.com/Article/details/gsjrblttg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.tarul.cn/Article/details/givskwtck.sHtML

[R37] 把输出赋给变量
来源：http://mobile.yfazqb.com/Article/details/gioafrjvk.sHtML

files=$(ls -1)
来源：http://m.share.vehdjk.com/Article/details/gfxutbprr.sHtML

[R38] 管道串联
来源：http://www.m.share.sjlbkw.cn/Article/details/gfskllplp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.epnwcf.com/Article/details/ghgmehlln.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.sjlbkw.cn/Article/details/gwbknpeze.sHtML

cmd > out.log 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gojlnbgsm.sHtML

[R40] 追加写日志
来源：http://3g.tarul.cn/Article/details/ggyyrnuiq.sHtML

echo "log" >> out.log
来源：http://mobile.tarul.cn/Article/details/gejzmzyqj.sHtML

[R41] 丢弃输出
来源：http://www.share.tarul.cn/Article/details/gvwgftugi.sHtML

cmd >/dev/null 2>&1
来源：http://blog.vehdjk.com/Article/details/gbdmwxfqb.sHtML

[R42] 输入重定向
来源：http://www.share.yfazqb.com/Article/details/ggrnklqes.sHtML

wc -l < a.txt
来源：http://blog.sjlbkw.cn/Article/details/goespthfv.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gfekapgrz.sHtML

find . -name "*.log" -type f
来源：http://baike.tarul.cn/Article/details/gkrjwntab.sHtML

[R44] 按修改时间查找
来源：http://www.share.vehdjk.com/Article/details/guutrkaen.sHtML

find . -mtime -7 -type f
来源：http://m.share.tarul.cn/Article/details/gtpxvnzvw.sHtML

[R45] 批量删除
来源：http://read.share.bbcook.cn/Article/details/gvockawni.sHtML

find . -name "*.tmp" -delete
来源：http://baike.sjlbkw.cn/Article/details/grspczjjw.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.tarul.cn/Article/details/ghxuzwxpe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.epnwcf.com/Article/details/grvbheikc.sHtML

[R47] sed 单行替换
来源：http://www.blog.epnwcf.com/Article/details/gsziliixw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fktsv.cn/Article/details/gbbrdzqkf.sHtML

[R48] awk 取指定列
来源：http://www.share.sjlbkw.cn/Article/details/gsrxvxiee.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.tarul.cn/Article/details/gnyizaica.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/ghruwdnvy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.vehdjk.com/Article/details/gudalhtcm.sHtML

[R50] awk 求和
来源：http://wap.vehdjk.com/Article/details/gkacjihbq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.yfazqb.com/Article/details/gekmeynrg.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.yfazqb.com/Article/details/gaidhfyxp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fktsv.cn/Article/details/gxllagmnw.sHtML

[R52] 统计行数
来源：http://www.blog.tarul.cn/Article/details/gbmhxdnyj.sHtML

wc -l a.txt
来源：http://baike.bbcook.cn/Article/details/givmoabng.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.sjlbkw.cn/Article/details/gsroltvym.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fktsv.cn/Article/details/gpcfgnmzf.sHtML

[R54] 比较两个文件
来源：http://3g.fktsv.cn/Article/details/gcjoxdmxq.sHtML

diff a.txt b.txt
来源：http://read.share.tarul.cn/Article/details/gbrnlmwan.sHtML

[R55] 压缩与解压
来源：http://www.blog.epnwcf.com/Article/details/gbannennf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.tarul.cn/Article/details/goychsqoz.sHtML

[R56] 远程拷贝
来源：http://www.share.fktsv.cn/Article/details/gloemxxhz.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gizyhwfkc.sHtML

[R57] 远程执行命令
来源：http://www.blog.bbcook.cn/Article/details/gisynnrpb.sHtML

ssh user@host 'uptime'
来源：http://baike.vehdjk.com/Article/details/gqspacthx.sHtML

[R58] 下载文件
来源：http://www.m.share.tarul.cn/Article/details/gggjpxerd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.epnwcf.com/Article/details/gswkqzaot.sHtML

[R59] 发 POST JSON
来源：http://mobile.bbcook.cn/Article/details/gruwcliod.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.tarul.cn/Article/details/gahoshucy.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/giplaunuo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.yfazqb.com/Article/details/ggmrtsvyz.sHtML

[R61] 磁盘占用
来源：http://www.blog.yfazqb.com/Article/details/gwwpqqbxw.sHtML

df -h;  du -sh *
来源：http://read.share.vehdjk.com/Article/details/gyugyzefr.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.vehdjk.com/Article/details/gjhztzcgm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/guatwfuct.sHtML

[R63] 内存与进程
来源：http://baike.fktsv.cn/Article/details/ghnvbhbtd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.sjlbkw.cn/Article/details/gxtwcnsbo.sHtML

[R64] 结束进程
来源：http://wap.tarul.cn/Article/details/gmihqxing.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.bbcook.cn/Article/details/gfsohnfbu.sHtML

[R65] 查看端口占用
来源：http://read.share.bbcook.cn/Article/details/gbzereahi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.vehdjk.com/Article/details/gxxllsfpd.sHtML

[R66] 定时任务
来源：http://3g.tarul.cn/Article/details/gglrzormz.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjaiougy.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.yfazqb.com/Article/details/ggyffqjkm.sHtML

openssl rand -hex 16
来源：http://www.blog.fktsv.cn/Article/details/gbwktprqj.sHtML

[R68] 计算文件校验值
来源：http://www.share.bbcook.cn/Article/details/gnmbkowwe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gurncrxph.sHtML

[R69] 生成随机密码
来源：http://www.blog.yfazqb.com/Article/details/gtmrybvrk.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.yfazqb.com/Article/details/gjpstldql.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.epnwcf.com/Article/details/gniskrakp.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.vehdjk.com/Article/details/gzdjgaiqr.sHtML

[R71] 日期格式化
来源：http://wap.yfazqb.com/Article/details/gnutmthtw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.bbcook.cn/Article/details/gjevudypv.sHtML

[R72] 等待端口就绪
来源：http://wap.tarul.cn/Article/details/gsfnoiomj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/guvhzxuli.sHtML

[R73] 分割大日志
来源：http://read.share.epnwcf.com/Article/details/gmrhgddys.sHtML

split -l 1000 big.log part_
来源：http://m.share.bbcook.cn/Article/details/grnrmoceh.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/gxdkuxxmn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/gcvahzgna.sHtML

[R75] 导出环境变量
来源：http://www.share.bbcook.cn/Article/details/guqbgiart.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.epnwcf.com/Article/details/gfqzkdqvy.sHtML

[R76] 使用临时文件
来源：http://www.share.epnwcf.com/Article/details/gztwhkpdt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gslomlkso.sHtML

[R77] 读取用户输入
来源：http://3g.vehdjk.com/Article/details/gjgbnlmbc.sHtML

read -rp "请输入: " ans
来源：http://baike.fktsv.cn/Article/details/gsoiuledf.sHtML

[R78] 交互式菜单
来源：http://m.share.yfazqb.com/Article/details/gheymlnoo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.vehdjk.com/Article/details/gotwsioij.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/gaqnbrpjp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.yfazqb.com/Article/details/gxgweplgq.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.epnwcf.com/Article/details/gcusybktb.sHtML

time ./run.sh
来源：http://blog.vehdjk.com/Article/details/ghayhearn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gipcfosqq.sHtML

S. C / C++ 专题
来源：http://m.share.vehdjk.com/Article/details/gblhecfsn.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdxehcbyn.sHtML

[S01] C：Hello World
来源：http://mobile.epnwcf.com/Article/details/geqqjlrmx.sHtML

#include <stdio.h>
来源：http://m.share.sjlbkw.cn/Article/details/gizstxppj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.bbcook.cn/Article/details/gbpdaibjo.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fktsv.cn/Article/details/guodjaguy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.sjlbkw.cn/Article/details/gfzonjmky.sHtML

[S03] C：读入整数
来源：http://www.share.fktsv.cn/Article/details/gblkugkpc.sHtML

int x; scanf("%d", &x);
来源：http://m.share.yfazqb.com/Article/details/gttumsblg.sHtML

[S04] C：字符串复制
来源：http://m.share.epnwcf.com/Article/details/gqicwwdlt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.vehdjk.com/Article/details/gtrwphuhx.sHtML

[S05] C：字符串长度
来源：http://m.share.epnwcf.com/Article/details/gfyxjpjbp.sHtML

strlen(s)
来源：http://www.blog.vehdjk.com/Article/details/grrebbqsn.sHtML

[S06] C：字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/giwwtocqc.sHtML

strcmp(a, b) == 0
来源：http://m.share.bbcook.cn/Article/details/gcqwnjpcb.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/ggqdgvhny.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.vehdjk.com/Article/details/gjsdkvmwk.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.yfazqb.com/Article/details/gkwwwehsg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.bbcook.cn/Article/details/gfedgmwwq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fktsv.cn/Article/details/gsvawkmza.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fktsv.cn/Article/details/gbwijpfhh.sHtML

[S10] C：指针与解引用
来源：http://read.share.yfazqb.com/Article/details/gvczapomn.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/giqekszpq.sHtML

[S11] C：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gcwfltrkg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.bbcook.cn/Article/details/goipieqyf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gelfeqphp.sHtML

fclose(f);
来源：http://3g.epnwcf.com/Article/details/gwviwbzvb.sHtML

[S12] C：写文件
来源：http://baike.vehdjk.com/Article/details/gmognqxgx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fktsv.cn/Article/details/goitwcpay.sHtML

[S13] C：宏定义
来源：http://www.share.bbcook.cn/Article/details/gjzuvvlyh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.vehdjk.com/Article/details/gttqzsijm.sHtML

[S14] C：枚举
来源：http://blog.fktsv.cn/Article/details/gjetiwoqs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.epnwcf.com/Article/details/ggsbohlbm.sHtML

[S15] C：类型转换
来源：http://blog.tarul.cn/Article/details/gzwgxwrtp.sHtML

(double) a / b
来源：http://mobile.yfazqb.com/Article/details/gvchxfbev.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/gxucdvykt.sHtML

x |= (1 << 3);
来源：http://mobile.vehdjk.com/Article/details/ghqlppfhb.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fktsv.cn/Article/details/gowbpxyse.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.yfazqb.com/Article/details/gmzsftrad.sHtML

[S18] C：命令行参数
来源：http://baike.epnwcf.com/Article/details/gvkygotgz.sHtML

int main(int argc, char **argv)
来源：http://3g.sjlbkw.cn/Article/details/gggshliub.sHtML

[S19] C：快速排序
来源：http://3g.fktsv.cn/Article/details/gnmwluvcq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gskfwcdvj.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gseyqephv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gytbvbmcw.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/gzwdnhoml.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.tarul.cn/Article/details/gczidvwey.sHtML

[S22] C：字符串转数字
来源：http://read.share.vehdjk.com/Article/details/gkyjoksna.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/gbjzrtmjg.sHtML

[S23] C：随机数
来源：http://www.blog.sjlbkw.cn/Article/details/gcctbmfjh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fktsv.cn/Article/details/gxaddxtsz.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gdvcuvium.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fktsv.cn/Article/details/gxheahihf.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gqznkaavl.sHtML

memcpy(dst, src, n);
来源：http://baike.fktsv.cn/Article/details/gnlhwtqwa.sHtML

[S26] C：内存清零
来源：http://www.share.epnwcf.com/Article/details/geenrjhur.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/gtqazizbt.sHtML

[S27] C：定义常量
来源：http://www.blog.tarul.cn/Article/details/gybippuit.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/geuzypfyf.sHtML

[S28] C：静态变量
来源：http://www.share.epnwcf.com/Article/details/ghugkovwp.sHtML

static int counter = 0;
来源：http://wap.fktsv.cn/Article/details/gtivrwdhs.sHtML

[S29] C：变参函数
来源：http://baike.fktsv.cn/Article/details/gpkaabbwf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.sjlbkw.cn/Article/details/gwbwkmhur.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/gwrgwnoli.sHtML

#ifndef X_H
来源：http://www.blog.yfazqb.com/Article/details/gfhdktmmr.sHtML

#define X_H
来源：http://blog.vehdjk.com/Article/details/gqpmrxbqd.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gyuvmyuut.sHtML

[S31] C++：Hello World
来源：http://www.blog.tarul.cn/Article/details/gbrxvkmlm.sHtML

#include <iostream>
来源：http://baike.epnwcf.com/Article/details/gzadrtouj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtdqzvhwc.sHtML

[S32] C++：字符串
来源：http://mobile.epnwcf.com/Article/details/gnwebujhu.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.yfazqb.com/Article/details/ggfjngbam.sHtML

[S33] C++：vector 增删
来源：http://wap.sjlbkw.cn/Article/details/gjfxswskr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.yfazqb.com/Article/details/gxkjyjsax.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.yfazqb.com/Article/details/gszfyuiig.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.tarul.cn/Article/details/geddvgwxd.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/gxxwkimgv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gnjgugcbc.sHtML

[S36] C++：unordered_map
来源：http://www.share.epnwcf.com/Article/details/gywjyvwxt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/gkfldfapp.sHtML

[S37] C++：set
来源：http://mobile.sjlbkw.cn/Article/details/gjyaiskvh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.tarul.cn/Article/details/ghqursder.sHtML

[S38] C++：排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzkwowzh.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fktsv.cn/Article/details/gguyqegll.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.yfazqb.com/Article/details/gftgeoqsv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.epnwcf.com/Article/details/gmskwyluw.sHtML

[S40] C++：查找元素
来源：http://wap.bbcook.cn/Article/details/gfvwanada.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.tarul.cn/Article/details/gxankuqzl.sHtML

[S41] C++：类与构造函数
来源：http://baike.tarul.cn/Article/details/gkxgbftsv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.sjlbkw.cn/Article/details/ggqiisvir.sHtML

[S42] C++：继承与虚函数
来源：http://blog.tarul.cn/Article/details/gkyientki.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.bbcook.cn/Article/details/gtcdlbytg.sHtML

[S43] C++：智能指针
来源：http://wap.sjlbkw.cn/Article/details/gifkchqxh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.tarul.cn/Article/details/gvgeoeiyh.sHtML

[S44] C++：引用传参
来源：http://read.share.yfazqb.com/Article/details/gzbnsnjbs.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/gnflguhlj.sHtML

[S45] C++：lambda
来源：http://baike.fktsv.cn/Article/details/gtmtqhxrt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsvswcwu.sHtML

[S46] C++：函数模板
来源：http://www.m.share.yfazqb.com/Article/details/gxjmsgakp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.yfazqb.com/Article/details/ghkfeisbg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.bbcook.cn/Article/details/gledqniim.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fktsv.cn/Article/details/gbrlyciei.sHtML

[S48] C++：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gsrdmouvj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.epnwcf.com/Article/details/gqshmbfhh.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.tarul.cn/Article/details/gqhvltuql.sHtML

[S49] C++：写文件
来源：http://read.share.epnwcf.com/Article/details/gqtgmkwkv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.yfazqb.com/Article/details/gefrtqmbt.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/gqbzvcmno.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fktsv.cn/Article/details/glhdzrqiv.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fktsv.cn/Article/details/gjfjjrsuq.sHtML

static_cast<double>(a) / b
来源：http://mobile.vehdjk.com/Article/details/gxyuifuot.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.yfazqb.com/Article/details/gzurdjkgr.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fktsv.cn/Article/details/gqjjdsnqt.sHtML

[S53] C++：移动语义
来源：http://www.share.tarul.cn/Article/details/gnnftasmo.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/gflkhoiqm.sHtML

[S54] C++：异常处理
来源：http://www.share.fktsv.cn/Article/details/grffhnuaa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.tarul.cn/Article/details/gejdspoif.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/gaifftmep.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fktsv.cn/Article/details/glxcekozt.sHtML

[S56] C++：optional
来源：http://3g.tarul.cn/Article/details/ghtmaqreb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.yfazqb.com/Article/details/gqvfjeyyt.sHtML

[S57] C++：编译期常量
来源：http://www.blog.bbcook.cn/Article/details/gigwlgmrd.sHtML

constexpr int N = 10;
来源：http://wap.vehdjk.com/Article/details/gsxooaqyc.sHtML

[S58] C++：命名空间
来源：http://baike.vehdjk.com/Article/details/gvopigyep.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gsaphywlm.sHtML

[S59] C++：静态断言
来源：http://3g.fktsv.cn/Article/details/gpifoogac.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.sjlbkw.cn/Article/details/gjgglpzpo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fktsv.cn/Article/details/gqgqaxqjg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fktsv.cn/Article/details/gozrohitj.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gxmhbauwi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.vehdjk.com/Article/details/gncnhtovv.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gimicofbc.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/gehrqxiin.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gqzskhwvi.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gzarjawlt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.yfazqb.com/Article/details/gqyhycjwa.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgrhlfkh.sHtML

"值: $b"
来源：http://blog.epnwcf.com/Article/details/ggewufaob.sHtML

[T04] Kotlin：空安全
来源：http://wap.fktsv.cn/Article/details/gjoclyihf.sHtML

val n: String? = null;  n?.length
来源：http://www.share.yfazqb.com/Article/details/gxbnhpuyd.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.yfazqb.com/Article/details/gvquxkmho.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.bbcook.cn/Article/details/gzojvlcpn.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/gcighmrrg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.vehdjk.com/Article/details/gpuvlygcm.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/gluhnhcjw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fktsv.cn/Article/details/gkjcfywyh.sHtML

[T08] Kotlin：数据类
来源：http://3g.bbcook.cn/Article/details/ggzpnfoxc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/gbleukgyc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.bbcook.cn/Article/details/glxbjqbge.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fktsv.cn/Article/details/gugemgviw.sHtML

[T10] Kotlin：默认参数
来源：http://blog.vehdjk.com/Article/details/gatdjycml.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.vehdjk.com/Article/details/gvaqanvyw.sHtML

[T11] Kotlin：协程
来源：http://www.blog.bbcook.cn/Article/details/ghazruetj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.epnwcf.com/Article/details/gcoeivkna.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.bbcook.cn/Article/details/gflfdgbxk.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.yfazqb.com/Article/details/guwimqhbs.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.vehdjk.com/Article/details/gihpmqtjd.sHtML

val m = mapOf("a" to 1)
来源：http://baike.sjlbkw.cn/Article/details/gsgcceehv.sHtML

[T14] Kotlin：循环
来源：http://baike.fktsv.cn/Article/details/glgjzukpe.sHtML

for (i in 1..10) println(i)
来源：http://wap.fktsv.cn/Article/details/gtgjmzogi.sHtML

[T15] Kotlin：接口
来源：http://www.share.epnwcf.com/Article/details/gwlegpbbo.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/grcaghzdt.sHtML

[T16] Swift：Hello World
来源：http://blog.fktsv.cn/Article/details/gekakuzgn.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/gywdhyjbd.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.tarul.cn/Article/details/gibobglpk.sHtML

var a = 1;  let b = 2
来源：http://www.share.bbcook.cn/Article/details/gdwvmqivt.sHtML

[T18] Swift：字符串插值
来源：http://www.share.tarul.cn/Article/details/gtajwviqa.sHtML

"值: \(b)"
来源：http://mobile.epnwcf.com/Article/details/gxjmorzzr.sHtML

[T19] Swift：可选绑定
来源：http://read.share.epnwcf.com/Article/details/gwmpgsfwn.sHtML

if let n = opt { print(n) }
来源：http://m.share.vehdjk.com/Article/details/gckaxplvv.sHtML

[T20] Swift：数组操作
来源：http://read.share.tarul.cn/Article/details/ghzkipyri.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.yfazqb.com/Article/details/gptgpsqlo.sHtML

[T21] Swift：遍历
来源：http://3g.yfazqb.com/Article/details/gquhwqcns.sHtML

for x in a { print(x) }
来源：http://www.share.tarul.cn/Article/details/gbbwwwevl.sHtML

[T22] Swift：字典
来源：http://baike.tarul.cn/Article/details/gcbjtuony.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.sjlbkw.cn/Article/details/gqtmlvlpd.sHtML

[T23] Swift：函数
来源：http://blog.sjlbkw.cn/Article/details/gjmbqjzln.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.yfazqb.com/Article/details/gencwwfpd.sHtML

[T24] Swift：闭包
来源：http://www.m.share.epnwcf.com/Article/details/ghdekioud.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.vehdjk.com/Article/details/gmznunvrq.sHtML

[T25] Swift：结构体
来源：http://wap.sjlbkw.cn/Article/details/gcsatxxda.sHtML

struct P { var x: Int }
来源：http://www.blog.epnwcf.com/Article/details/gygnodbeu.sHtML

[T26] Swift：类与重写
来源：http://wap.sjlbkw.cn/Article/details/gcxrxohxi.sHtML

class A: Base { override func f() {} }
来源：http://m.share.bbcook.cn/Article/details/gpgwytasf.sHtML


<!-- 参考信息 -->