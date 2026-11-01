代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.epnwcf.com/Article/details/gfpjxseqs.sHtML

[R24] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gdgqxepqh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/gqprsrvrf.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fktsv.cn/Article/details/ghjavuoek.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.yfazqb.com/Article/details/gzyiidkmh.sHtML

[R26] 命令替换
来源：http://www.share.bbcook.cn/Article/details/gellivbwz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fktsv.cn/Article/details/gugizaawz.sHtML

[R27] 算术展开
来源：http://wap.epnwcf.com/Article/details/ggabuhfve.sHtML

echo $((1 + 2 * 3))
来源：http://blog.vehdjk.com/Article/details/gowktpzmg.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gisvmgngn.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/gcdpdkkyh.sHtML

[R29] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/ggsvjmccp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.tarul.cn/Article/details/gsywrulxf.sHtML

[R30] 函数返回状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gsaoerfxe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fktsv.cn/Article/details/gzsvxtcpn.sHtML

[R31] 局部变量
来源：http://3g.epnwcf.com/Article/details/grigozjyg.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.sjlbkw.cn/Article/details/gardytyut.sHtML

[R32] 参数个数校验
来源：http://www.share.sjlbkw.cn/Article/details/gzwizocpw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fktsv.cn/Article/details/gpveqynqh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fktsv.cn/Article/details/gqmpmuqot.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.yfazqb.com/Article/details/gswninmfz.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/gdgdlcdfw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gdbvvopfx.sHtML

[R35] 后台执行并等待
来源：http://m.share.epnwcf.com/Article/details/ggfzqwywd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.epnwcf.com/Article/details/gwxtsfhbp.sHtML

[R36] 并发执行多个任务
来源：http://m.share.yfazqb.com/Article/details/gsekgpmyc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.vehdjk.com/Article/details/gcpbzmonb.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.yfazqb.com/Article/details/gvchckznb.sHtML

files=$(ls -1)
来源：http://baike.epnwcf.com/Article/details/goidodqfb.sHtML

[R38] 管道串联
来源：http://www.m.share.yfazqb.com/Article/details/gmnqvjvzh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.tarul.cn/Article/details/gphlcweew.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.sjlbkw.cn/Article/details/goiaderhy.sHtML

cmd > out.log 2>&1
来源：http://wap.fktsv.cn/Article/details/ggdkmkuvn.sHtML

[R40] 追加写日志
来源：http://wap.fktsv.cn/Article/details/grkpszmbb.sHtML

echo "log" >> out.log
来源：http://read.share.bbcook.cn/Article/details/gccmzfzve.sHtML

[R41] 丢弃输出
来源：http://www.blog.tarul.cn/Article/details/glcgukmfg.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.vehdjk.com/Article/details/gbtbohdbw.sHtML

[R42] 输入重定向
来源：http://www.m.share.vehdjk.com/Article/details/gnjmykwdi.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/gzpllzzca.sHtML

[R43] 按名字查找文件
来源：http://www.share.fktsv.cn/Article/details/gtgddulkn.sHtML

find . -name "*.log" -type f
来源：http://baike.vehdjk.com/Article/details/gsrvkowes.sHtML

[R44] 按修改时间查找
来源：http://blog.bbcook.cn/Article/details/gipalbjsp.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.vehdjk.com/Article/details/gcimnmvof.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/gzpxbdkyy.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.yfazqb.com/Article/details/gkzcgrqcl.sHtML

[R46] 递归替换文件内容
来源：http://mobile.yfazqb.com/Article/details/ganyvdxpv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/ggixreium.sHtML

[R47] sed 单行替换
来源：http://3g.vehdjk.com/Article/details/glonafvzm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gjhnckpws.sHtML

[R48] awk 取指定列
来源：http://www.share.tarul.cn/Article/details/gikjqcgqq.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.bbcook.cn/Article/details/gmzgtczcx.sHtML

[R49] awk 带条件
来源：http://baike.epnwcf.com/Article/details/gphvplant.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.yfazqb.com/Article/details/gvczqbinu.sHtML

[R50] awk 求和
来源：http://3g.bbcook.cn/Article/details/gxuazxpwf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.epnwcf.com/Article/details/gjshctoce.sHtML

[R51] 排序去重取前几
来源：http://read.share.epnwcf.com/Article/details/gjhabypxo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.vehdjk.com/Article/details/gaxqjskml.sHtML

[R52] 统计行数
来源：http://blog.bbcook.cn/Article/details/gtmmzdpcb.sHtML

wc -l a.txt
来源：http://wap.fktsv.cn/Article/details/gmlfmdibs.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.vehdjk.com/Article/details/gxthqvwjy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.yfazqb.com/Article/details/gmtbddvmi.sHtML

[R54] 比较两个文件
来源：http://baike.vehdjk.com/Article/details/geeowgioj.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/gxmfvyaqs.sHtML

[R55] 压缩与解压
来源：http://m.share.yfazqb.com/Article/details/gmudyzsoz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fktsv.cn/Article/details/getagkbph.sHtML

[R56] 远程拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gpsfbifgi.sHtML

scp file user@host:/path/
来源：http://www.blog.fktsv.cn/Article/details/gmzzwspdm.sHtML

[R57] 远程执行命令
来源：http://www.share.tarul.cn/Article/details/gedqszxvd.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/goksrugfa.sHtML

[R58] 下载文件
来源：http://blog.tarul.cn/Article/details/gzlfqsksn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.vehdjk.com/Article/details/gzqqfrghd.sHtML

[R59] 发 POST JSON
来源：http://wap.fktsv.cn/Article/details/glavthjgj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.tarul.cn/Article/details/gnmtewhjp.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gxsaymjzz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fktsv.cn/Article/details/gzgsygpif.sHtML

[R61] 磁盘占用
来源：http://baike.bbcook.cn/Article/details/gdlmjrpuo.sHtML

df -h;  du -sh *
来源：http://mobile.epnwcf.com/Article/details/glxnilmsi.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/gqswbjuqv.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.vehdjk.com/Article/details/gcjebysjp.sHtML

[R63] 内存与进程
来源：http://www.blog.epnwcf.com/Article/details/gvvkujfna.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.sjlbkw.cn/Article/details/gjtlrmerr.sHtML

[R64] 结束进程
来源：http://baike.yfazqb.com/Article/details/grgxfojny.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fktsv.cn/Article/details/gidoykxeh.sHtML

[R65] 查看端口占用
来源：http://read.share.fktsv.cn/Article/details/geoyrbqvg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.yfazqb.com/Article/details/gmifjmgnl.sHtML

[R66] 定时任务
来源：http://read.share.sjlbkw.cn/Article/details/gddbqtfgz.sHtML

crontab -e;  crontab -l
来源：http://3g.vehdjk.com/Article/details/gjzxmvqak.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.vehdjk.com/Article/details/ghccnxzuw.sHtML

openssl rand -hex 16
来源：http://www.m.share.yfazqb.com/Article/details/gbzjymsew.sHtML

[R68] 计算文件校验值
来源：http://read.share.tarul.cn/Article/details/gdhluchyc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.bbcook.cn/Article/details/gofyzugjn.sHtML

[R69] 生成随机密码
来源：http://mobile.fktsv.cn/Article/details/gvwistbdy.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/gzczijjoa.sHtML

[R70] 时间戳与互转
来源：http://3g.yfazqb.com/Article/details/ggfyhpyat.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhpxpjxm.sHtML

[R71] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/genqwijaq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.bbcook.cn/Article/details/gxqesfsyq.sHtML

[R72] 等待端口就绪
来源：http://blog.vehdjk.com/Article/details/gtwobsiax.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/giojwhvwg.sHtML

[R73] 分割大日志
来源：http://www.blog.sjlbkw.cn/Article/details/gqogjsocb.sHtML

split -l 1000 big.log part_
来源：http://m.share.yfazqb.com/Article/details/gzptixdvp.sHtML

[R74] 批量重命名
来源：http://m.share.yfazqb.com/Article/details/gbwxvaadl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/grbotvcah.sHtML

[R75] 导出环境变量
来源：http://wap.epnwcf.com/Article/details/gzcvgkgzh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.vehdjk.com/Article/details/gkfjyyuog.sHtML

[R76] 使用临时文件
来源：http://www.share.tarul.cn/Article/details/gkcncpyhc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gxfoiocnr.sHtML

[R77] 读取用户输入
来源：http://www.share.vehdjk.com/Article/details/gkxyfqdma.sHtML

read -rp "请输入: " ans
来源：http://3g.tarul.cn/Article/details/gmsyukewh.sHtML

[R78] 交互式菜单
来源：http://read.share.sjlbkw.cn/Article/details/gmzmuhamb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.epnwcf.com/Article/details/gkaeivyac.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fktsv.cn/Article/details/gcbwlzyzf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.epnwcf.com/Article/details/gdfdqltym.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.bbcook.cn/Article/details/giizkczpz.sHtML

time ./run.sh
来源：http://www.m.share.tarul.cn/Article/details/gfhkwaere.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gugonniou.sHtML

S. C / C++ 专题
来源：http://m.share.epnwcf.com/Article/details/gndurgjhh.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gcxiayahl.sHtML

[S01] C：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwhhcjty.sHtML

#include <stdio.h>
来源：http://www.blog.sjlbkw.cn/Article/details/gepuytkud.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.vehdjk.com/Article/details/gvouosrbl.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gagnwfziz.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.yfazqb.com/Article/details/grvjoiknm.sHtML

[S03] C：读入整数
来源：http://mobile.sjlbkw.cn/Article/details/gzizmvzef.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.bbcook.cn/Article/details/gonhzckso.sHtML

[S04] C：字符串复制
来源：http://m.share.yfazqb.com/Article/details/gnxarctjw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.tarul.cn/Article/details/gvbxqqgjt.sHtML

[S05] C：字符串长度
来源：http://3g.epnwcf.com/Article/details/gkljpybsp.sHtML

strlen(s)
来源：http://m.share.vehdjk.com/Article/details/gpedzmxer.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/gbtwanbsj.sHtML

strcmp(a, b) == 0
来源：http://blog.fktsv.cn/Article/details/gilfbkqdm.sHtML

[S07] C：数组遍历求和
来源：http://3g.vehdjk.com/Article/details/gxecinlcf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.epnwcf.com/Article/details/gbrixjazi.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.bbcook.cn/Article/details/gvdqzmgbf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.yfazqb.com/Article/details/gkdotxbbh.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.epnwcf.com/Article/details/goonjkjdd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.yfazqb.com/Article/details/gvfsamwfc.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.vehdjk.com/Article/details/gozclgnbw.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gevfqgfai.sHtML

[S11] C：逐行读文件
来源：http://blog.bbcook.cn/Article/details/grnixkbvx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.vehdjk.com/Article/details/gjrqqvxaz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gykqyecbd.sHtML

fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gvosbgugx.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gbausmeqs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/ggcxpmefu.sHtML

[S13] C：宏定义
来源：http://read.share.sjlbkw.cn/Article/details/gxbhhziry.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.epnwcf.com/Article/details/gbemelrzc.sHtML

[S14] C：枚举
来源：http://www.share.fktsv.cn/Article/details/grkceazev.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.yfazqb.com/Article/details/gwgbvoeqm.sHtML

[S15] C：类型转换
来源：http://read.share.epnwcf.com/Article/details/gwlsxxvat.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/gnhgmxfub.sHtML

[S16] C：位操作置位
来源：http://3g.sjlbkw.cn/Article/details/ghcdnvgor.sHtML

x |= (1 << 3);
来源：http://mobile.tarul.cn/Article/details/gdhdxwhzi.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gcobtdlis.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.yfazqb.com/Article/details/gusldzomp.sHtML

[S18] C：命令行参数
来源：http://read.share.fktsv.cn/Article/details/gnmbcbctj.sHtML

int main(int argc, char **argv)
来源：http://m.share.vehdjk.com/Article/details/gxeduasir.sHtML

[S19] C：快速排序
来源：http://baike.fktsv.cn/Article/details/goumdnnqp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gafdogzku.sHtML

[S20] C：二分查找
来源：http://wap.sjlbkw.cn/Article/details/gbchkdtmh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gpjguhoco.sHtML

[S21] C：字符类别判断
来源：http://baike.yfazqb.com/Article/details/gspduzjfs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.yfazqb.com/Article/details/gjtxspcsi.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fktsv.cn/Article/details/gwbfdxdvq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.vehdjk.com/Article/details/gjfpiaema.sHtML

[S23] C：随机数
来源：http://3g.fktsv.cn/Article/details/guvmvmedz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.tarul.cn/Article/details/gmuumgtad.sHtML

[S24] C：获取本地时间
来源：http://www.blog.tarul.cn/Article/details/grjzjfshi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.bbcook.cn/Article/details/gfuxoksyj.sHtML

[S25] C：内存拷贝
来源：http://3g.yfazqb.com/Article/details/gxckesogg.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fktsv.cn/Article/details/gzrunayrt.sHtML

[S26] C：内存清零
来源：http://3g.epnwcf.com/Article/details/gepifcbfs.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.tarul.cn/Article/details/gwqybxkgf.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gkmewuzss.sHtML

const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gbtffcwyo.sHtML

[S28] C：静态变量
来源：http://baike.yfazqb.com/Article/details/gqwybehqf.sHtML

static int counter = 0;
来源：http://3g.yfazqb.com/Article/details/gscyoykup.sHtML

[S29] C：变参函数
来源：http://read.share.tarul.cn/Article/details/gkkxkuoxs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.tarul.cn/Article/details/gcdbyuccd.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/gohmlcfqb.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/gcnpypuuf.sHtML

#define X_H
来源：http://baike.fktsv.cn/Article/details/gegxhbijv.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/gtrpwkfuf.sHtML

[S31] C++：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxgiwidh.sHtML

#include <iostream>
来源：http://3g.vehdjk.com/Article/details/gpnlwidbi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.epnwcf.com/Article/details/ghsqpotca.sHtML

[S32] C++：字符串
来源：http://blog.sjlbkw.cn/Article/details/gjqvanfea.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fktsv.cn/Article/details/gvwttglzr.sHtML

[S33] C++：vector 增删
来源：http://baike.epnwcf.com/Article/details/ghgepgbmp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/glmkhldtn.sHtML

[S34] C++：遍历 vector
来源：http://read.share.sjlbkw.cn/Article/details/gndgwkpnu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fktsv.cn/Article/details/gujuhmgrk.sHtML

[S35] C++：map
来源：http://www.share.vehdjk.com/Article/details/gqfmpkpgp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/grmcgzhaz.sHtML

[S36] C++：unordered_map
来源：http://wap.fktsv.cn/Article/details/gmdnohcvl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gateogjdu.sHtML

[S37] C++：set
来源：http://blog.yfazqb.com/Article/details/gkuxtyoql.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.bbcook.cn/Article/details/gvkdwvsse.sHtML

[S38] C++：排序
来源：http://read.share.bbcook.cn/Article/details/gmykbilxe.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.bbcook.cn/Article/details/gptpxgrqd.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/gksasyvbp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.yfazqb.com/Article/details/grvtcvygn.sHtML

[S40] C++：查找元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkiwneuh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.epnwcf.com/Article/details/gxdgxphab.sHtML

[S41] C++：类与构造函数
来源：http://wap.epnwcf.com/Article/details/gmjzdcbba.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.bbcook.cn/Article/details/gvgtqjopi.sHtML

[S42] C++：继承与虚函数
来源：http://3g.vehdjk.com/Article/details/glrhduurw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.vehdjk.com/Article/details/gjyxyxbtq.sHtML

[S43] C++：智能指针
来源：http://read.share.fktsv.cn/Article/details/ghalxqemu.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.epnwcf.com/Article/details/gkewjkhpr.sHtML

[S44] C++：引用传参
来源：http://read.share.vehdjk.com/Article/details/gqiqzpiuf.sHtML

void inc(int &x) { ++x; }
来源：http://3g.epnwcf.com/Article/details/gqxxnjfcc.sHtML

[S45] C++：lambda
来源：http://www.m.share.fktsv.cn/Article/details/gpwdwgnbr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.vehdjk.com/Article/details/gvihguorn.sHtML

[S46] C++：函数模板
来源：http://3g.vehdjk.com/Article/details/gibkkezqk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.yfazqb.com/Article/details/gsbluvtgu.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.vehdjk.com/Article/details/gblemkjdv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.bbcook.cn/Article/details/gyhzicazc.sHtML

[S48] C++：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gmtsoitiu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.sjlbkw.cn/Article/details/glacqsjub.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.bbcook.cn/Article/details/gpqdbhuso.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/glapbidom.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/gggngnhxc.sHtML

[S50] C++：格式化数字
来源：http://read.share.yfazqb.com/Article/details/ghpufovsg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gakwygbpn.sHtML

[S51] C++：显式类型转换
来源：http://baike.yfazqb.com/Article/details/gmrnchotl.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fktsv.cn/Article/details/gfxarjlqh.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.epnwcf.com/Article/details/gdpuvswxs.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.epnwcf.com/Article/details/grxfcydhy.sHtML

[S53] C++：移动语义
来源：http://m.share.vehdjk.com/Article/details/gvhgoqobg.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/gcahvileh.sHtML

[S54] C++：异常处理
来源：http://www.share.yfazqb.com/Article/details/gtfshpmjt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.sjlbkw.cn/Article/details/gernyklty.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.tarul.cn/Article/details/gkmbbsmsj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.yfazqb.com/Article/details/gubppmltg.sHtML

[S56] C++：optional
来源：http://baike.yfazqb.com/Article/details/gnfmxvyvh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.bbcook.cn/Article/details/gfjrjquig.sHtML

[S57] C++：编译期常量
来源：http://read.share.bbcook.cn/Article/details/gfbfqofpk.sHtML

constexpr int N = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gdcwixtjb.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/gbpnkawgv.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.tarul.cn/Article/details/gvbgbnsvd.sHtML

[S59] C++：静态断言
来源：http://wap.sjlbkw.cn/Article/details/ghvtprxum.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.epnwcf.com/Article/details/gtyvxyhyk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fktsv.cn/Article/details/gywvndlkr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/gnftvlsvc.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbjdhdkbs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gkggdotsw.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/guoqpjwcj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.tarul.cn/Article/details/gxhegumpr.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gcepnzedx.sHtML

[T02] Kotlin：变量
来源：http://www.share.tarul.cn/Article/details/grqavqznr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.epnwcf.com/Article/details/gsyiplufv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.yfazqb.com/Article/details/gycoyokiv.sHtML

"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gmhhuabrz.sHtML

[T04] Kotlin：空安全
来源：http://www.share.vehdjk.com/Article/details/gahaltrbn.sHtML

val n: String? = null;  n?.length
来源：http://3g.sjlbkw.cn/Article/details/gyntqfqpp.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fktsv.cn/Article/details/gtidzdsag.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/gkblxasje.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/gkgsjejyn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrdqjbyv.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.epnwcf.com/Article/details/gvkqhvfap.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fktsv.cn/Article/details/gczakwshb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.vehdjk.com/Article/details/gmpkjgzba.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fktsv.cn/Article/details/gpacfxtzg.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.sjlbkw.cn/Article/details/gwgvobdvm.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.vehdjk.com/Article/details/gwyrkcaly.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.yfazqb.com/Article/details/gseostsbl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/gwapliiwb.sHtML

[T11] Kotlin：协程
来源：http://m.share.bbcook.cn/Article/details/gojuhyvxb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.bbcook.cn/Article/details/gkkkvbwjs.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.yfazqb.com/Article/details/gdhxwtjsr.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gfcdgoxlo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.tarul.cn/Article/details/ghsfarvyi.sHtML

val m = mapOf("a" to 1)
来源：http://baike.tarul.cn/Article/details/ghskejhhm.sHtML

[T14] Kotlin：循环
来源：http://blog.tarul.cn/Article/details/gizhoiwsj.sHtML

for (i in 1..10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gumvtyqyo.sHtML

[T15] Kotlin：接口
来源：http://blog.tarul.cn/Article/details/gryrhyhds.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.yfazqb.com/Article/details/gpbvhatwh.sHtML

[T16] Swift：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gqndtdlpa.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gurhrddwu.sHtML

[T17] Swift：变量与常量
来源：http://wap.tarul.cn/Article/details/glunsxpnn.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/gfkdrrxns.sHtML

[T18] Swift：字符串插值
来源：http://blog.tarul.cn/Article/details/grlkrepiz.sHtML

"值: \(b)"
来源：http://www.share.fktsv.cn/Article/details/geethvahw.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.bbcook.cn/Article/details/gdvnywpxa.sHtML

if let n = opt { print(n) }
来源：http://www.blog.tarul.cn/Article/details/gwyidiuns.sHtML

[T20] Swift：数组操作
来源：http://mobile.yfazqb.com/Article/details/gejgmgnmo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.tarul.cn/Article/details/gevekfzja.sHtML

[T21] Swift：遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gkgkgatpj.sHtML

for x in a { print(x) }
来源：http://3g.tarul.cn/Article/details/gpmhuqsqe.sHtML

[T22] Swift：字典
来源：http://mobile.yfazqb.com/Article/details/gxxhorgno.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.epnwcf.com/Article/details/gjramjiut.sHtML

[T23] Swift：函数
来源：http://mobile.sjlbkw.cn/Article/details/gqvhuuyil.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gilcnppbc.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/gwqciydfs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/ghbcvdhaj.sHtML

[T25] Swift：结构体
来源：http://3g.fktsv.cn/Article/details/gabybljpm.sHtML

struct P { var x: Int }
来源：http://3g.yfazqb.com/Article/details/gchpncrnq.sHtML

[T26] Swift：类与重写
来源：http://www.share.bbcook.cn/Article/details/gloexidmo.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fktsv.cn/Article/details/gwdboeouk.sHtML


<!-- 参考信息 -->