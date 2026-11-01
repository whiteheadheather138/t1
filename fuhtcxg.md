代发 wailian999

echo "${#s}"
来源：http://baike.bbcook.cn/Article/details/gczfdbexn.sHtML

[R22] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gqvmhkrwc.sHtML

echo "${s:0:5}"
来源：http://www.blog.tarul.cn/Article/details/gbrltccwg.sHtML

[R23] 字符串替换
来源：http://baike.vehdjk.com/Article/details/godziklkb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.epnwcf.com/Article/details/gmeqoyigo.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gfpgzdyar.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.tarul.cn/Article/details/gpmdxmblf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/gzbhnwncs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fktsv.cn/Article/details/gnwkeisme.sHtML

[R26] 命令替换
来源：http://www.share.yfazqb.com/Article/details/griqbprbl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.vehdjk.com/Article/details/ghkuzxlob.sHtML

[R27] 算术展开
来源：http://3g.vehdjk.com/Article/details/gpfkvoixt.sHtML

echo $((1 + 2 * 3))
来源：http://blog.tarul.cn/Article/details/gtcsdirkz.sHtML

[R28] 浮点运算
来源：http://read.share.yfazqb.com/Article/details/gnteammho.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/gigabrxmb.sHtML

[R29] 定义函数
来源：http://mobile.fktsv.cn/Article/details/guxyxruof.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.sjlbkw.cn/Article/details/grgskdqrp.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.bbcook.cn/Article/details/gteruxfbs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.tarul.cn/Article/details/gtwkkypkv.sHtML

[R31] 局部变量
来源：http://m.share.epnwcf.com/Article/details/gueiukmbz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.bbcook.cn/Article/details/gyczoybfz.sHtML

[R32] 参数个数校验
来源：http://3g.vehdjk.com/Article/details/gjpehwset.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gykbfhiyy.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.epnwcf.com/Article/details/gmodddlhj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.vehdjk.com/Article/details/grncxsikz.sHtML

[R34] 退出时清理
来源：http://mobile.vehdjk.com/Article/details/gfanhayyr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gjyqxszqe.sHtML

[R35] 后台执行并等待
来源：http://m.share.epnwcf.com/Article/details/gfdjsejwf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/gixxwomnc.sHtML

[R36] 并发执行多个任务
来源：http://read.share.yfazqb.com/Article/details/gfcqwqikg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.epnwcf.com/Article/details/gjsyyosqd.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/gmnzrdnyx.sHtML

files=$(ls -1)
来源：http://read.share.bbcook.cn/Article/details/gwathirxp.sHtML

[R38] 管道串联
来源：http://www.share.yfazqb.com/Article/details/gcmvpubzp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fktsv.cn/Article/details/ghpgugozj.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/gaidpecrk.sHtML

cmd > out.log 2>&1
来源：http://blog.fktsv.cn/Article/details/grhnetkhn.sHtML

[R40] 追加写日志
来源：http://www.share.epnwcf.com/Article/details/grrglschb.sHtML

echo "log" >> out.log
来源：http://m.share.yfazqb.com/Article/details/gqfhesgvf.sHtML

[R41] 丢弃输出
来源：http://www.m.share.yfazqb.com/Article/details/gknfhlzep.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gfhwhvwje.sHtML

[R42] 输入重定向
来源：http://baike.sjlbkw.cn/Article/details/glssvgjlm.sHtML

wc -l < a.txt
来源：http://3g.bbcook.cn/Article/details/gcourdqdw.sHtML

[R43] 按名字查找文件
来源：http://blog.bbcook.cn/Article/details/gorjfzczt.sHtML

find . -name "*.log" -type f
来源：http://read.share.bbcook.cn/Article/details/gvcdhwnzh.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gmymnnxhn.sHtML

find . -mtime -7 -type f
来源：http://baike.epnwcf.com/Article/details/gsdqqcxga.sHtML

[R45] 批量删除
来源：http://wap.yfazqb.com/Article/details/guvquoupl.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.vehdjk.com/Article/details/gailktqel.sHtML

[R46] 递归替换文件内容
来源：http://mobile.sjlbkw.cn/Article/details/gqvvzizor.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/gwxvafsfw.sHtML

[R47] sed 单行替换
来源：http://blog.tarul.cn/Article/details/gifgiygsj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.epnwcf.com/Article/details/geyztqmgz.sHtML

[R48] awk 取指定列
来源：http://3g.tarul.cn/Article/details/gfdhvslea.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gmxfaswkg.sHtML

[R49] awk 带条件
来源：http://3g.fktsv.cn/Article/details/gvatnrgro.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fktsv.cn/Article/details/gjfcekzog.sHtML

[R50] awk 求和
来源：http://www.share.bbcook.cn/Article/details/gtyahdlcp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.bbcook.cn/Article/details/gftfukevt.sHtML

[R51] 排序去重取前几
来源：http://wap.yfazqb.com/Article/details/gvvzohqtd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/gizbacmon.sHtML

[R52] 统计行数
来源：http://www.blog.fktsv.cn/Article/details/gdtnrwohq.sHtML

wc -l a.txt
来源：http://www.blog.tarul.cn/Article/details/gszijaaxu.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.tarul.cn/Article/details/gfwetldmj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.yfazqb.com/Article/details/gswrbyevb.sHtML

[R54] 比较两个文件
来源：http://3g.fktsv.cn/Article/details/guhmilpfj.sHtML

diff a.txt b.txt
来源：http://www.share.epnwcf.com/Article/details/gfkrupsdm.sHtML

[R55] 压缩与解压
来源：http://www.share.yfazqb.com/Article/details/gidewkjhr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.tarul.cn/Article/details/gabvsmwxo.sHtML

[R56] 远程拷贝
来源：http://blog.bbcook.cn/Article/details/gnafprxfm.sHtML

scp file user@host:/path/
来源：http://blog.yfazqb.com/Article/details/ggddkwigs.sHtML

[R57] 远程执行命令
来源：http://blog.tarul.cn/Article/details/gazvjyslp.sHtML

ssh user@host 'uptime'
来源：http://mobile.bbcook.cn/Article/details/gmhtghwvj.sHtML

[R58] 下载文件
来源：http://www.m.share.yfazqb.com/Article/details/gnjymqyje.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.yfazqb.com/Article/details/gppuryxbo.sHtML

[R59] 发 POST JSON
来源：http://3g.yfazqb.com/Article/details/gpqceafvr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.vehdjk.com/Article/details/gtzkaqcxt.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gjopkccgf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.yfazqb.com/Article/details/gkoqasrle.sHtML

[R61] 磁盘占用
来源：http://m.share.sjlbkw.cn/Article/details/gzjuxvgyd.sHtML

df -h;  du -sh *
来源：http://www.share.sjlbkw.cn/Article/details/gleetbkiz.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/gvgjyfygm.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.yfazqb.com/Article/details/gbemblrjr.sHtML

[R63] 内存与进程
来源：http://3g.bbcook.cn/Article/details/gsgnlhhsm.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.sjlbkw.cn/Article/details/gjklirlaz.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/glqdcyktu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/gjfjknypg.sHtML

[R65] 查看端口占用
来源：http://blog.yfazqb.com/Article/details/gqdipreas.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fktsv.cn/Article/details/gkodywbrr.sHtML

[R66] 定时任务
来源：http://m.share.tarul.cn/Article/details/gvgvzykjk.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/gfoiyliis.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fktsv.cn/Article/details/gtwvzosdt.sHtML

openssl rand -hex 16
来源：http://blog.tarul.cn/Article/details/gxghhvwdt.sHtML

[R68] 计算文件校验值
来源：http://www.blog.sjlbkw.cn/Article/details/gxwyafwvi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.tarul.cn/Article/details/gbunetyqd.sHtML

[R69] 生成随机密码
来源：http://wap.fktsv.cn/Article/details/gzvejthkb.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.sjlbkw.cn/Article/details/gzkfinikt.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/ggsbbkron.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.yfazqb.com/Article/details/gskxgcsjf.sHtML

[R71] 日期格式化
来源：http://3g.bbcook.cn/Article/details/ggdwgipba.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.vehdjk.com/Article/details/gplidhpna.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gqsjnfako.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gvftfxxcw.sHtML

[R73] 分割大日志
来源：http://m.share.tarul.cn/Article/details/gxcmxgjbo.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.yfazqb.com/Article/details/gtsemdgad.sHtML

[R74] 批量重命名
来源：http://mobile.tarul.cn/Article/details/gyyzdpqnp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/gwvpvxtqa.sHtML

[R75] 导出环境变量
来源：http://blog.yfazqb.com/Article/details/grrfdfxls.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.epnwcf.com/Article/details/gykgphanf.sHtML

[R76] 使用临时文件
来源：http://baike.bbcook.cn/Article/details/ghhlpjbmt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gltthjppy.sHtML

[R77] 读取用户输入
来源：http://wap.epnwcf.com/Article/details/ggicsynhb.sHtML

read -rp "请输入: " ans
来源：http://baike.fktsv.cn/Article/details/ggxkfmfsp.sHtML

[R78] 交互式菜单
来源：http://mobile.sjlbkw.cn/Article/details/gwrahqtsj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.bbcook.cn/Article/details/gxbvatajk.sHtML

[R79] 解析命令行选项
来源：http://wap.sjlbkw.cn/Article/details/geecchcol.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.epnwcf.com/Article/details/gwopermaz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.sjlbkw.cn/Article/details/giapoanvv.sHtML

time ./run.sh
来源：http://www.blog.epnwcf.com/Article/details/gfcnmpfjb.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gehuwdhak.sHtML

S. C / C++ 专题
来源：http://www.share.tarul.cn/Article/details/gntilrfgw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gpgyrslmg.sHtML

[S01] C：Hello World
来源：http://baike.fktsv.cn/Article/details/ghrbctzti.sHtML

#include <stdio.h>
来源：http://3g.bbcook.cn/Article/details/gymfiyzbu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.yfazqb.com/Article/details/gvmsptylo.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.vehdjk.com/Article/details/gotjuiutz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.epnwcf.com/Article/details/glfxqauio.sHtML

[S03] C：读入整数
来源：http://wap.tarul.cn/Article/details/gevendgdn.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.sjlbkw.cn/Article/details/grndjqzvy.sHtML

[S04] C：字符串复制
来源：http://read.share.epnwcf.com/Article/details/gharicyec.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/ghmtezxre.sHtML

[S05] C：字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gpbewftyc.sHtML

strlen(s)
来源：http://mobile.bbcook.cn/Article/details/gicfphene.sHtML

[S06] C：字符串比较
来源：http://www.blog.tarul.cn/Article/details/gvwvgteci.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.tarul.cn/Article/details/gouxchnfk.sHtML

[S07] C：数组遍历求和
来源：http://wap.bbcook.cn/Article/details/gnmyllvky.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.yfazqb.com/Article/details/gdhqwmofq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.sjlbkw.cn/Article/details/ggirvsafi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.yfazqb.com/Article/details/gyiwfrlfx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.yfazqb.com/Article/details/gewmyubzb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fktsv.cn/Article/details/gjzwgejbm.sHtML

[S10] C：指针与解引用
来源：http://m.share.epnwcf.com/Article/details/gwrklcufq.sHtML

int *p = &a;  *p = 5;
来源：http://3g.vehdjk.com/Article/details/gkzeeljul.sHtML

[S11] C：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gzbedcoqu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.yfazqb.com/Article/details/gipzbapay.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.yfazqb.com/Article/details/gkzayinql.sHtML

fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gcqtorqyc.sHtML

[S12] C：写文件
来源：http://mobile.bbcook.cn/Article/details/ghupomsyy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.epnwcf.com/Article/details/ggbguzkow.sHtML

[S13] C：宏定义
来源：http://read.share.sjlbkw.cn/Article/details/gjlgaqjia.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/gkhoflama.sHtML

[S14] C：枚举
来源：http://3g.yfazqb.com/Article/details/gwstgcsqg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.epnwcf.com/Article/details/grvblynld.sHtML

[S15] C：类型转换
来源：http://3g.vehdjk.com/Article/details/gftuufoha.sHtML

(double) a / b
来源：http://read.share.yfazqb.com/Article/details/gewhpzbbi.sHtML

[S16] C：位操作置位
来源：http://wap.yfazqb.com/Article/details/gpifsovju.sHtML

x |= (1 << 3);
来源：http://wap.sjlbkw.cn/Article/details/glnblmuyl.sHtML

[S17] C：安全拼接字符串
来源：http://baike.epnwcf.com/Article/details/ghnflonni.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.yfazqb.com/Article/details/gdgimfots.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/gfrsoicqa.sHtML

int main(int argc, char **argv)
来源：http://baike.yfazqb.com/Article/details/gfdjfqepl.sHtML

[S19] C：快速排序
来源：http://mobile.epnwcf.com/Article/details/gomzzihaa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/glpupsvsj.sHtML

[S20] C：二分查找
来源：http://www.blog.vehdjk.com/Article/details/gjbiosqlv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gudipcpvr.sHtML

[S21] C：字符类别判断
来源：http://mobile.yfazqb.com/Article/details/gzeqjkxnw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.tarul.cn/Article/details/geewptzej.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/gyuffwrqv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.epnwcf.com/Article/details/gdlevcemf.sHtML

[S23] C：随机数
来源：http://m.share.bbcook.cn/Article/details/ggedsunqo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.epnwcf.com/Article/details/gkdiomuav.sHtML

[S24] C：获取本地时间
来源：http://www.blog.tarul.cn/Article/details/gjnhcisel.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fktsv.cn/Article/details/gtdoabqde.sHtML

[S25] C：内存拷贝
来源：http://3g.sjlbkw.cn/Article/details/gqvokwrww.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/gwocbqhzv.sHtML

[S26] C：内存清零
来源：http://mobile.bbcook.cn/Article/details/gyzbeehug.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.tarul.cn/Article/details/gjfuzparr.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gqlbsnsxn.sHtML

const double PI = 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gneevnwxa.sHtML

[S28] C：静态变量
来源：http://www.share.sjlbkw.cn/Article/details/gyirhntmn.sHtML

static int counter = 0;
来源：http://www.m.share.bbcook.cn/Article/details/gnasotfqo.sHtML

[S29] C：变参函数
来源：http://www.share.tarul.cn/Article/details/gtmfrupsf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.tarul.cn/Article/details/gakpwlhrh.sHtML

[S30] C：头文件保护
来源：http://m.share.fktsv.cn/Article/details/gwpqwkshy.sHtML

#ifndef X_H
来源：http://mobile.vehdjk.com/Article/details/gxjwkcgks.sHtML

#define X_H
来源：http://blog.tarul.cn/Article/details/gbjkqzypw.sHtML

#endif
来源：http://3g.tarul.cn/Article/details/gmmrpmrdy.sHtML

[S31] C++：Hello World
来源：http://baike.fktsv.cn/Article/details/gngzejrnn.sHtML

#include <iostream>
来源：http://3g.bbcook.cn/Article/details/gspviobxi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.epnwcf.com/Article/details/gqxhmsknj.sHtML

[S32] C++：字符串
来源：http://m.share.tarul.cn/Article/details/gstxqrzos.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.tarul.cn/Article/details/ghzdtiivo.sHtML

[S33] C++：vector 增删
来源：http://3g.yfazqb.com/Article/details/grckdyzim.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/gmrpgqphs.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/gcxgkckuc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fktsv.cn/Article/details/ggjatsvdl.sHtML

[S35] C++：map
来源：http://www.share.sjlbkw.cn/Article/details/gzgnecphu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gixhybrqv.sHtML

[S36] C++：unordered_map
来源：http://mobile.tarul.cn/Article/details/gardvmori.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gniffguju.sHtML

[S37] C++：set
来源：http://wap.fktsv.cn/Article/details/gaxpjbpyh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.epnwcf.com/Article/details/gbhsrnzek.sHtML

[S38] C++：排序
来源：http://www.blog.sjlbkw.cn/Article/details/guwdwoqjy.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.vehdjk.com/Article/details/gnfbvlkhj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.bbcook.cn/Article/details/gqwlejwje.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.vehdjk.com/Article/details/gokvkntra.sHtML

[S40] C++：查找元素
来源：http://m.share.sjlbkw.cn/Article/details/ggpyepmui.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.epnwcf.com/Article/details/glkurhfxu.sHtML

[S41] C++：类与构造函数
来源：http://wap.bbcook.cn/Article/details/gnklwksfz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.sjlbkw.cn/Article/details/gexprcaiz.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.vehdjk.com/Article/details/gydzinfjo.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/gqmmzwcog.sHtML

[S43] C++：智能指针
来源：http://wap.fktsv.cn/Article/details/gzxzecmcv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/gshxflyyp.sHtML

[S44] C++：引用传参
来源：http://wap.vehdjk.com/Article/details/gasgsimyi.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqwkvzbsw.sHtML

[S45] C++：lambda
来源：http://3g.epnwcf.com/Article/details/gzkllcors.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/gzngsmnsp.sHtML

[S46] C++：函数模板
来源：http://mobile.sjlbkw.cn/Article/details/gaoiugfls.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.tarul.cn/Article/details/gkurgfjsi.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fktsv.cn/Article/details/grruulbdz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.sjlbkw.cn/Article/details/gfxgmvhfv.sHtML

[S48] C++：逐行读文件
来源：http://wap.epnwcf.com/Article/details/glkkmqdor.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fktsv.cn/Article/details/glxehwdoc.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/gicsdfweb.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/gmbltyfav.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.vehdjk.com/Article/details/gxpehlyrd.sHtML

[S50] C++：格式化数字
来源：http://www.share.tarul.cn/Article/details/gfzqjwanf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gwnqtrdpk.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gbawphugr.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gxwuytkkx.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.sjlbkw.cn/Article/details/gvwovkaph.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.vehdjk.com/Article/details/gchjwbkmi.sHtML

[S53] C++：移动语义
来源：http://wap.fktsv.cn/Article/details/gvmjuutin.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.tarul.cn/Article/details/gidhrbtaa.sHtML

[S54] C++：异常处理
来源：http://read.share.yfazqb.com/Article/details/gthsjjoxn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fktsv.cn/Article/details/gxzhnlfiw.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fktsv.cn/Article/details/gwxuwsaun.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fktsv.cn/Article/details/gigncnnjd.sHtML

[S56] C++：optional
来源：http://read.share.epnwcf.com/Article/details/gigbxmqre.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.epnwcf.com/Article/details/gojyylyjo.sHtML

[S57] C++：编译期常量
来源：http://baike.tarul.cn/Article/details/gxwluszyq.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/gaazfhydw.sHtML

[S58] C++：命名空间
来源：http://www.blog.vehdjk.com/Article/details/gilkswwnj.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.epnwcf.com/Article/details/goozhwlll.sHtML

[S59] C++：静态断言
来源：http://www.share.sjlbkw.cn/Article/details/gujqjlxyu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.sjlbkw.cn/Article/details/gginrccon.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.epnwcf.com/Article/details/gaxjsbizc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/gzeuritrn.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gnmijniml.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/gicpimpyf.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gyvxfhuvj.sHtML

[T01] Kotlin：Hello World
来源：http://baike.epnwcf.com/Article/details/gkubzsrnl.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gaevgazck.sHtML

[T02] Kotlin：变量
来源：http://baike.vehdjk.com/Article/details/grnktzdqq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.bbcook.cn/Article/details/gaqhkifrj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrbovhqe.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/gtruirpva.sHtML

[T04] Kotlin：空安全
来源：http://www.share.vehdjk.com/Article/details/gooosviud.sHtML

val n: String? = null;  n?.length
来源：http://3g.bbcook.cn/Article/details/gsqyljyzg.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fktsv.cn/Article/details/gdhjgsywa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.tarul.cn/Article/details/gnuxifqiz.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.tarul.cn/Article/details/gwpntqxxu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fktsv.cn/Article/details/ggxmewrly.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.yfazqb.com/Article/details/gdaipeype.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.bbcook.cn/Article/details/gpwgdefrc.sHtML

[T08] Kotlin：数据类
来源：http://m.share.sjlbkw.cn/Article/details/grswwrksp.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gdyeqxyzw.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.bbcook.cn/Article/details/gtdmobltf.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.vehdjk.com/Article/details/gdjhjgekc.sHtML

[T10] Kotlin：默认参数
来源：http://baike.bbcook.cn/Article/details/gxqwsmgrk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.yfazqb.com/Article/details/gztsbgtmv.sHtML

[T11] Kotlin：协程
来源：http://read.share.fktsv.cn/Article/details/gamxtbash.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.bbcook.cn/Article/details/gkxnicldm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.bbcook.cn/Article/details/gdgbqsrln.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gnbijwolx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.yfazqb.com/Article/details/ghezsxkim.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.epnwcf.com/Article/details/gpxyjnuno.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gxhgybdbd.sHtML

for (i in 1..10) println(i)
来源：http://read.share.bbcook.cn/Article/details/glgmpuvbf.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.vehdjk.com/Article/details/gplqromrs.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fktsv.cn/Article/details/girswxpps.sHtML

[T16] Swift：Hello World
来源：http://wap.tarul.cn/Article/details/gmuylpwie.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gqljfqbsa.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fktsv.cn/Article/details/gobeqiygo.sHtML

var a = 1;  let b = 2
来源：http://m.share.bbcook.cn/Article/details/gzoweznzo.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/grgvvpdgf.sHtML

"值: \(b)"
来源：http://mobile.tarul.cn/Article/details/gpxercmrl.sHtML

[T19] Swift：可选绑定
来源：http://mobile.vehdjk.com/Article/details/gcjzeobcl.sHtML

if let n = opt { print(n) }
来源：http://www.blog.yfazqb.com/Article/details/gjizpwkin.sHtML

[T20] Swift：数组操作
来源：http://baike.bbcook.cn/Article/details/gkbuxlkgn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/gjbutsvfh.sHtML

[T21] Swift：遍历
来源：http://www.share.bbcook.cn/Article/details/gssqlxbxp.sHtML

for x in a { print(x) }
来源：http://www.share.bbcook.cn/Article/details/gpaghbjsc.sHtML

[T22] Swift：字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlsmkxdu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.sjlbkw.cn/Article/details/ghhnwndif.sHtML

[T23] Swift：函数
来源：http://m.share.fktsv.cn/Article/details/gxgovxqpq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.epnwcf.com/Article/details/gdnawwdne.sHtML

[T24] Swift：闭包
来源：http://read.share.bbcook.cn/Article/details/gjiplfysa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.epnwcf.com/Article/details/grutrwvdr.sHtML


<!-- 参考信息 -->