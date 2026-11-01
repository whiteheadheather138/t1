代发 wailian999

echo "${#s}"
来源：http://mobile.bbcook.cn/Article/details/gehwogrzz.sHtML

[R22] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gxksxnfwe.sHtML

echo "${s:0:5}"
来源：http://www.m.share.tarul.cn/Article/details/gqoaqptbm.sHtML

[R23] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/grbeuigpx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.yfazqb.com/Article/details/getguptuc.sHtML

[R24] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gzqwwinkm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.yfazqb.com/Article/details/gkjpcbfoq.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.tarul.cn/Article/details/gyzoxgetl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.yfazqb.com/Article/details/gdhxgvgdl.sHtML

[R26] 命令替换
来源：http://m.share.bbcook.cn/Article/details/gzuxqteji.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fktsv.cn/Article/details/gvlwfhuqi.sHtML

[R27] 算术展开
来源：http://www.m.share.tarul.cn/Article/details/gbovcufur.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.epnwcf.com/Article/details/grdaismgu.sHtML

[R28] 浮点运算
来源：http://3g.tarul.cn/Article/details/gbqdliiji.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.bbcook.cn/Article/details/gznfrmulo.sHtML

[R29] 定义函数
来源：http://baike.fktsv.cn/Article/details/gvqewovzw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.yfazqb.com/Article/details/gykdycjky.sHtML

[R30] 函数返回状态码
来源：http://www.share.fktsv.cn/Article/details/gontwtgww.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.sjlbkw.cn/Article/details/gtmfrqycc.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gdmdqcndr.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.yfazqb.com/Article/details/gqekiaini.sHtML

[R32] 参数个数校验
来源：http://3g.vehdjk.com/Article/details/gmmsosmbq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gnufdjkoh.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.vehdjk.com/Article/details/gbyyeunas.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.yfazqb.com/Article/details/gqgyhaatn.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gwkjhjbue.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/gpnaprezb.sHtML

[R35] 后台执行并等待
来源：http://baike.epnwcf.com/Article/details/gmuhyjlji.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.epnwcf.com/Article/details/grlytjsnl.sHtML

[R36] 并发执行多个任务
来源：http://mobile.bbcook.cn/Article/details/gpzrrrpnz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.tarul.cn/Article/details/gdaeakosq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.bbcook.cn/Article/details/gzihyfgdj.sHtML

files=$(ls -1)
来源：http://blog.epnwcf.com/Article/details/ggmulvjir.sHtML

[R38] 管道串联
来源：http://www.share.epnwcf.com/Article/details/gwlnkznsn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.tarul.cn/Article/details/gmjdxngmf.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.tarul.cn/Article/details/gclxccvol.sHtML

cmd > out.log 2>&1
来源：http://read.share.epnwcf.com/Article/details/gxphqomlv.sHtML

[R40] 追加写日志
来源：http://m.share.vehdjk.com/Article/details/gpfblcqgp.sHtML

echo "log" >> out.log
来源：http://wap.fktsv.cn/Article/details/gpxjetgfp.sHtML

[R41] 丢弃输出
来源：http://wap.yfazqb.com/Article/details/gtuwnurmp.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fktsv.cn/Article/details/gkodciixp.sHtML

[R42] 输入重定向
来源：http://www.share.vehdjk.com/Article/details/gnodukzfp.sHtML

wc -l < a.txt
来源：http://wap.sjlbkw.cn/Article/details/gzssfeuud.sHtML

[R43] 按名字查找文件
来源：http://m.share.bbcook.cn/Article/details/gxcirmnnp.sHtML

find . -name "*.log" -type f
来源：http://mobile.yfazqb.com/Article/details/gzizwtsvx.sHtML

[R44] 按修改时间查找
来源：http://blog.yfazqb.com/Article/details/gwowxwkoh.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gsomkfvxc.sHtML

[R45] 批量删除
来源：http://m.share.sjlbkw.cn/Article/details/gpyhxbqlw.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.tarul.cn/Article/details/gqrlhgpzj.sHtML

[R46] 递归替换文件内容
来源：http://blog.epnwcf.com/Article/details/gtisrqijk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.sjlbkw.cn/Article/details/gffqbcwli.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gvyptkdtf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/gtvhzfwri.sHtML

[R48] awk 取指定列
来源：http://www.m.share.yfazqb.com/Article/details/gqwugvkgs.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.vehdjk.com/Article/details/gcczexbou.sHtML

[R49] awk 带条件
来源：http://blog.vehdjk.com/Article/details/gacxfchff.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fktsv.cn/Article/details/gurbpehor.sHtML

[R50] awk 求和
来源：http://www.blog.sjlbkw.cn/Article/details/gchfvyueh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.tarul.cn/Article/details/guxfcruvc.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/glwbofhew.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.sjlbkw.cn/Article/details/grearfsqy.sHtML

[R52] 统计行数
来源：http://blog.bbcook.cn/Article/details/gghwlipgt.sHtML

wc -l a.txt
来源：http://baike.yfazqb.com/Article/details/gbqgpqkgb.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.bbcook.cn/Article/details/gbwnjfyuu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.vehdjk.com/Article/details/gzaylodzt.sHtML

[R54] 比较两个文件
来源：http://wap.fktsv.cn/Article/details/gbhmijper.sHtML

diff a.txt b.txt
来源：http://baike.tarul.cn/Article/details/ghiepyjov.sHtML

[R55] 压缩与解压
来源：http://read.share.vehdjk.com/Article/details/gcyzwdmtq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.yfazqb.com/Article/details/gnpccyiwc.sHtML

[R56] 远程拷贝
来源：http://www.blog.bbcook.cn/Article/details/gvqlvazfy.sHtML

scp file user@host:/path/
来源：http://mobile.bbcook.cn/Article/details/gotqmwrin.sHtML

[R57] 远程执行命令
来源：http://baike.tarul.cn/Article/details/godjuedeh.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.vehdjk.com/Article/details/gnxodzwvw.sHtML

[R58] 下载文件
来源：http://wap.yfazqb.com/Article/details/gyablachi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.epnwcf.com/Article/details/gzahnkszy.sHtML

[R59] 发 POST JSON
来源：http://read.share.bbcook.cn/Article/details/gplxlbeyy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.yfazqb.com/Article/details/gfpsnezoo.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/glwbrmqui.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fktsv.cn/Article/details/gtspobrfw.sHtML

[R61] 磁盘占用
来源：http://blog.vehdjk.com/Article/details/gftiltikn.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/geqsxmfyq.sHtML

[R62] 找最占空间的文件
来源：http://wap.vehdjk.com/Article/details/gyjhnlnsx.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.tarul.cn/Article/details/gcorvaiil.sHtML

[R63] 内存与进程
来源：http://www.m.share.epnwcf.com/Article/details/gqlphegmy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fktsv.cn/Article/details/gjzvvyift.sHtML

[R64] 结束进程
来源：http://m.share.tarul.cn/Article/details/gjrpxmnxg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.bbcook.cn/Article/details/gyjkefhtb.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fktsv.cn/Article/details/gbcfiubkg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fktsv.cn/Article/details/gztbllbuu.sHtML

[R66] 定时任务
来源：http://blog.fktsv.cn/Article/details/gnrxsrzni.sHtML

crontab -e;  crontab -l
来源：http://blog.yfazqb.com/Article/details/gfigblkth.sHtML

[R67] 生成随机十六进制串
来源：http://blog.vehdjk.com/Article/details/gwztchebr.sHtML

openssl rand -hex 16
来源：http://www.blog.yfazqb.com/Article/details/gpgvnebsu.sHtML

[R68] 计算文件校验值
来源：http://www.share.tarul.cn/Article/details/gzclzvasi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.bbcook.cn/Article/details/giumzmsik.sHtML

[R69] 生成随机密码
来源：http://www.blog.vehdjk.com/Article/details/gktnkqqvo.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.epnwcf.com/Article/details/gpkvljgrv.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/gtjsexevm.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fktsv.cn/Article/details/gwppoxglt.sHtML

[R71] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/ghmgkouip.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.vehdjk.com/Article/details/gimstpwza.sHtML

[R72] 等待端口就绪
来源：http://baike.epnwcf.com/Article/details/gxgkuviyl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gnmwkhpap.sHtML

[R73] 分割大日志
来源：http://read.share.yfazqb.com/Article/details/gfhsynhlh.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fktsv.cn/Article/details/gyaolpbst.sHtML

[R74] 批量重命名
来源：http://mobile.sjlbkw.cn/Article/details/gznccijuu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/gboifqxxz.sHtML

[R75] 导出环境变量
来源：http://3g.sjlbkw.cn/Article/details/gwozbuqpp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.vehdjk.com/Article/details/gdiasbcbu.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/gomalbciu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gnsyjtira.sHtML

[R77] 读取用户输入
来源：http://baike.epnwcf.com/Article/details/gbttxicpo.sHtML

read -rp "请输入: " ans
来源：http://wap.yfazqb.com/Article/details/gjeibqbca.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/gyigdwqcj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.sjlbkw.cn/Article/details/gdpxqglbz.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/glnwukpzv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.sjlbkw.cn/Article/details/glrppksid.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.bbcook.cn/Article/details/gsbvabtnt.sHtML

time ./run.sh
来源：http://wap.bbcook.cn/Article/details/ghmvlcvum.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gtfzkexkd.sHtML

S. C / C++ 专题
来源：http://www.share.tarul.cn/Article/details/gxpxkxead.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gomqrtdkf.sHtML

[S01] C：Hello World
来源：http://mobile.epnwcf.com/Article/details/gjldshpkd.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/gcnlbjhbt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.yfazqb.com/Article/details/gyryplfdr.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.tarul.cn/Article/details/gsowmqgji.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.yfazqb.com/Article/details/gaasazcnx.sHtML

[S03] C：读入整数
来源：http://blog.fktsv.cn/Article/details/gaqnlwnse.sHtML

int x; scanf("%d", &x);
来源：http://www.share.vehdjk.com/Article/details/gufyxtmcx.sHtML

[S04] C：字符串复制
来源：http://read.share.vehdjk.com/Article/details/gryzndmdg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.yfazqb.com/Article/details/gwmpedqyz.sHtML

[S05] C：字符串长度
来源：http://mobile.vehdjk.com/Article/details/gymtnbbdp.sHtML

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/gofkveaav.sHtML

[S06] C：字符串比较
来源：http://m.share.yfazqb.com/Article/details/guxwancxw.sHtML

strcmp(a, b) == 0
来源：http://baike.vehdjk.com/Article/details/gqchlehpk.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/ghzgvqxow.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.tarul.cn/Article/details/ggfwubbmx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.yfazqb.com/Article/details/gimgnscom.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.vehdjk.com/Article/details/gxleettyj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.vehdjk.com/Article/details/gmehnsvgz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.bbcook.cn/Article/details/gefdcxmum.sHtML

[S10] C：指针与解引用
来源：http://blog.sjlbkw.cn/Article/details/goestwvil.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fktsv.cn/Article/details/gtliqvssv.sHtML

[S11] C：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gyfapewgx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.sjlbkw.cn/Article/details/gqkkvykmd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.yfazqb.com/Article/details/goqgslbau.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/gexfqqprp.sHtML

[S12] C：写文件
来源：http://read.share.vehdjk.com/Article/details/gtjwxhibe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gmumuspar.sHtML

[S13] C：宏定义
来源：http://baike.sjlbkw.cn/Article/details/gvlpxyixf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fktsv.cn/Article/details/gohzgxtah.sHtML

[S14] C：枚举
来源：http://www.blog.tarul.cn/Article/details/gcdahqnbf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.yfazqb.com/Article/details/gpvolskpp.sHtML

[S15] C：类型转换
来源：http://3g.vehdjk.com/Article/details/gbzafeaki.sHtML

(double) a / b
来源：http://baike.bbcook.cn/Article/details/gjmzrikti.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/gtiyupdpd.sHtML

x |= (1 << 3);
来源：http://wap.fktsv.cn/Article/details/gsanatthq.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gvmljodwg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.epnwcf.com/Article/details/gafbvshaa.sHtML

[S18] C：命令行参数
来源：http://3g.tarul.cn/Article/details/gakefscob.sHtML

int main(int argc, char **argv)
来源：http://read.share.bbcook.cn/Article/details/gvmxnijmu.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/gydtcgkzd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gltmejfmx.sHtML

[S20] C：二分查找
来源：http://www.blog.vehdjk.com/Article/details/gujiyclcg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gkajyawxi.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/ghehctdop.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fktsv.cn/Article/details/giybmsycr.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.bbcook.cn/Article/details/gfjxveenz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.epnwcf.com/Article/details/gggjwjenh.sHtML

[S23] C：随机数
来源：http://3g.vehdjk.com/Article/details/gvwxyqabg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.vehdjk.com/Article/details/gundqgerg.sHtML

[S24] C：获取本地时间
来源：http://read.share.vehdjk.com/Article/details/gufisnsrt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/gbonbrlrb.sHtML

[S25] C：内存拷贝
来源：http://mobile.yfazqb.com/Article/details/gqdqdojex.sHtML

memcpy(dst, src, n);
来源：http://www.share.sjlbkw.cn/Article/details/gmolrfwon.sHtML

[S26] C：内存清零
来源：http://baike.vehdjk.com/Article/details/grwilkach.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gbgdxcdco.sHtML

[S27] C：定义常量
来源：http://mobile.fktsv.cn/Article/details/gqfbzdqfa.sHtML

const double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gyrkmcten.sHtML

[S28] C：静态变量
来源：http://www.share.sjlbkw.cn/Article/details/gpaarbnqq.sHtML

static int counter = 0;
来源：http://www.m.share.fktsv.cn/Article/details/gmcehxuah.sHtML

[S29] C：变参函数
来源：http://www.share.sjlbkw.cn/Article/details/gjumlyfaz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.bbcook.cn/Article/details/gjzbriblt.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/gwmojqfwo.sHtML

#ifndef X_H
来源：http://read.share.bbcook.cn/Article/details/gazhrujcf.sHtML

#define X_H
来源：http://read.share.epnwcf.com/Article/details/gjndqsond.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/glicmioar.sHtML

[S31] C++：Hello World
来源：http://www.m.share.tarul.cn/Article/details/guulovzcn.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gnqvdgqep.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/gkhcctzqy.sHtML

[S32] C++：字符串
来源：http://blog.yfazqb.com/Article/details/gxsolddst.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.bbcook.cn/Article/details/gjscwrwhk.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/gotmjiybf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/goxjgfezx.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.yfazqb.com/Article/details/gwymoraej.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.tarul.cn/Article/details/gipbgqpwt.sHtML

[S35] C++：map
来源：http://3g.epnwcf.com/Article/details/gqetqjsiu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/glytsbsqt.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/gapbbhkzb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrnilbef.sHtML

[S37] C++：set
来源：http://www.blog.yfazqb.com/Article/details/guesybtls.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.sjlbkw.cn/Article/details/ghddmaxqh.sHtML

[S38] C++：排序
来源：http://read.share.tarul.cn/Article/details/gyytgntgy.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fktsv.cn/Article/details/gmxltivuo.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.bbcook.cn/Article/details/gsldtuoxf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.vehdjk.com/Article/details/gggchkmjg.sHtML

[S40] C++：查找元素
来源：http://baike.yfazqb.com/Article/details/gornepqou.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.epnwcf.com/Article/details/glwkpimxe.sHtML

[S41] C++：类与构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gtnqxmqyi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.epnwcf.com/Article/details/gslwryocn.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.sjlbkw.cn/Article/details/gkmyxtiju.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.bbcook.cn/Article/details/gtgggxqhv.sHtML

[S43] C++：智能指针
来源：http://3g.bbcook.cn/Article/details/glqtxvfms.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.epnwcf.com/Article/details/glqavibdt.sHtML

[S44] C++：引用传参
来源：http://blog.tarul.cn/Article/details/gmpzdxgnm.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.sjlbkw.cn/Article/details/gsmhnbopr.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/gjcyyusjv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.vehdjk.com/Article/details/gcdfokoez.sHtML

[S46] C++：函数模板
来源：http://read.share.bbcook.cn/Article/details/giypooomk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.sjlbkw.cn/Article/details/gzofkvpqp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.tarul.cn/Article/details/gjygqtneo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.epnwcf.com/Article/details/gbyojxbaz.sHtML

[S48] C++：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/grexpizgq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.tarul.cn/Article/details/gtzybcbfb.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gwgxcxhbr.sHtML

[S49] C++：写文件
来源：http://www.blog.fktsv.cn/Article/details/gnmwwqjxi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fktsv.cn/Article/details/gegfqsnet.sHtML

[S50] C++：格式化数字
来源：http://read.share.bbcook.cn/Article/details/gnmrujqxf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.epnwcf.com/Article/details/gpfmkrebt.sHtML

[S51] C++：显式类型转换
来源：http://www.share.epnwcf.com/Article/details/gwednvjkw.sHtML

static_cast<double>(a) / b
来源：http://www.share.fktsv.cn/Article/details/goizaztfu.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.yfazqb.com/Article/details/gwajhwdzd.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.sjlbkw.cn/Article/details/gpmawsvma.sHtML

[S53] C++：移动语义
来源：http://baike.fktsv.cn/Article/details/gozunqblj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.epnwcf.com/Article/details/ghbtjnspm.sHtML

[S54] C++：异常处理
来源：http://m.share.epnwcf.com/Article/details/gvrwejlhh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.yfazqb.com/Article/details/gngdkvxzl.sHtML

[S55] C++：结构化绑定
来源：http://mobile.yfazqb.com/Article/details/gqhhjmnld.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gtpxciycg.sHtML

[S56] C++：optional
来源：http://3g.bbcook.cn/Article/details/grxawhamk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.yfazqb.com/Article/details/gwmqaheqx.sHtML

[S57] C++：编译期常量
来源：http://www.share.epnwcf.com/Article/details/gnjnketsz.sHtML

constexpr int N = 10;
来源：http://www.share.yfazqb.com/Article/details/gozgnhqun.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/ghuezmist.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.bbcook.cn/Article/details/ggljapfbl.sHtML

[S59] C++：静态断言
来源：http://read.share.fktsv.cn/Article/details/gncmyerur.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fktsv.cn/Article/details/gijbsyfxj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/gokcbvmbk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.epnwcf.com/Article/details/gtdbqhfhc.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gioyrohxj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gezfnomoe.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gcjngjcii.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gcnkfxbia.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/gycpuhidf.sHtML

[T02] Kotlin：变量
来源：http://baike.fktsv.cn/Article/details/gnjqenhji.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.epnwcf.com/Article/details/gweftgmzj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.epnwcf.com/Article/details/grwesznob.sHtML

"值: $b"
来源：http://read.share.epnwcf.com/Article/details/glumnzdah.sHtML

[T04] Kotlin：空安全
来源：http://blog.vehdjk.com/Article/details/gnwkzisjh.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gvubrjnxe.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.vehdjk.com/Article/details/ggwzvaoyl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fktsv.cn/Article/details/gysnikoxg.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/glsrmkeai.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/goytzztvs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gzrcpglay.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.vehdjk.com/Article/details/gcgjoiuin.sHtML

[T08] Kotlin：数据类
来源：http://wap.bbcook.cn/Article/details/gejowrlyf.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.epnwcf.com/Article/details/grzmvmnlf.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.epnwcf.com/Article/details/gpxlkcwcs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.sjlbkw.cn/Article/details/gkrhlstsz.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.vehdjk.com/Article/details/gyyhfvmcp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.tarul.cn/Article/details/gaagnuogg.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.vehdjk.com/Article/details/ghvknqpur.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fktsv.cn/Article/details/ghnfxwcvz.sHtML

[T12] Kotlin：解构声明
来源：http://blog.vehdjk.com/Article/details/gsqpgohnc.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.tarul.cn/Article/details/glasvsrlt.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.tarul.cn/Article/details/gfxlmqvqe.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.epnwcf.com/Article/details/grqroydtc.sHtML

[T14] Kotlin：循环
来源：http://3g.bbcook.cn/Article/details/gmlsvljbt.sHtML

for (i in 1..10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gvafcchcg.sHtML

[T15] Kotlin：接口
来源：http://www.share.sjlbkw.cn/Article/details/gnhbbaorl.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gpfxkkofz.sHtML

[T16] Swift：Hello World
来源：http://blog.vehdjk.com/Article/details/grzleytoy.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/ggpoeilmg.sHtML

[T17] Swift：变量与常量
来源：http://3g.vehdjk.com/Article/details/gbpuvpzvp.sHtML

var a = 1;  let b = 2
来源：http://wap.epnwcf.com/Article/details/gfkelreez.sHtML

[T18] Swift：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gydzjfrhm.sHtML

"值: \(b)"
来源：http://baike.epnwcf.com/Article/details/gvfmfyidg.sHtML

[T19] Swift：可选绑定
来源：http://mobile.sjlbkw.cn/Article/details/ghzgpvycf.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gckzbyabo.sHtML

[T20] Swift：数组操作
来源：http://www.share.epnwcf.com/Article/details/gaznmahlb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.vehdjk.com/Article/details/gxvnfuive.sHtML

[T21] Swift：遍历
来源：http://read.share.fktsv.cn/Article/details/ggdjehsxi.sHtML

for x in a { print(x) }
来源：http://mobile.sjlbkw.cn/Article/details/genxtdslw.sHtML

[T22] Swift：字典
来源：http://wap.fktsv.cn/Article/details/gqzkwnwpn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.sjlbkw.cn/Article/details/grldxjdzl.sHtML

[T23] Swift：函数
来源：http://www.share.tarul.cn/Article/details/gsljzxvft.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fktsv.cn/Article/details/gnfbziete.sHtML

[T24] Swift：闭包
来源：http://www.share.sjlbkw.cn/Article/details/gpxjicbtu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/ghenhbmpd.sHtML


<!-- 参考信息 -->