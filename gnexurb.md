代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.epnwcf.com/Article/details/gaqgtdppj.sHtML

[R24] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gznqrafve.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.tarul.cn/Article/details/gustxszpi.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.tarul.cn/Article/details/gartyztji.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.tarul.cn/Article/details/gzdosxshl.sHtML

[R26] 命令替换
来源：http://www.blog.yfazqb.com/Article/details/gdaokbprl.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.vehdjk.com/Article/details/ghqiqrywy.sHtML

[R27] 算术展开
来源：http://mobile.fktsv.cn/Article/details/gtccybylf.sHtML

echo $((1 + 2 * 3))
来源：http://3g.epnwcf.com/Article/details/gdzignvmw.sHtML

[R28] 浮点运算
来源：http://blog.yfazqb.com/Article/details/gwglfbrji.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.vehdjk.com/Article/details/gcnjawlqk.sHtML

[R29] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/gkqgvvuul.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.epnwcf.com/Article/details/gybowokel.sHtML

[R30] 函数返回状态码
来源：http://mobile.tarul.cn/Article/details/gchrgswms.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.epnwcf.com/Article/details/grotlvcia.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/ggbqyxjly.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.epnwcf.com/Article/details/gzdeymwpv.sHtML

[R32] 参数个数校验
来源：http://3g.yfazqb.com/Article/details/gdusvnroz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gbamvjtjj.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.bbcook.cn/Article/details/ggleresuk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.vehdjk.com/Article/details/gzcvszfjj.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/gfmtzopec.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/goggcbyvn.sHtML

[R35] 后台执行并等待
来源：http://baike.tarul.cn/Article/details/gwlbragwu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.vehdjk.com/Article/details/galyhswni.sHtML

[R36] 并发执行多个任务
来源：http://read.share.bbcook.cn/Article/details/grkwaeshe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/gxnrjewtz.sHtML

[R37] 把输出赋给变量
来源：http://3g.fktsv.cn/Article/details/gtmfdwjyk.sHtML

files=$(ls -1)
来源：http://mobile.sjlbkw.cn/Article/details/gfemzisav.sHtML

[R38] 管道串联
来源：http://www.m.share.bbcook.cn/Article/details/gidkzfsde.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.sjlbkw.cn/Article/details/gqquhfkqa.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.sjlbkw.cn/Article/details/gmfbttgde.sHtML

cmd > out.log 2>&1
来源：http://wap.yfazqb.com/Article/details/golhgsjwi.sHtML

[R40] 追加写日志
来源：http://read.share.epnwcf.com/Article/details/gbhacwcej.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/gjlnvxygh.sHtML

[R41] 丢弃输出
来源：http://blog.yfazqb.com/Article/details/gbfbkycac.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.yfazqb.com/Article/details/geaifvaui.sHtML

[R42] 输入重定向
来源：http://3g.fktsv.cn/Article/details/gixgaoeym.sHtML

wc -l < a.txt
来源：http://www.share.epnwcf.com/Article/details/gctakrnug.sHtML

[R43] 按名字查找文件
来源：http://blog.tarul.cn/Article/details/gatotlaan.sHtML

find . -name "*.log" -type f
来源：http://www.share.tarul.cn/Article/details/gutoqqbwa.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/gihidnxec.sHtML

find . -mtime -7 -type f
来源：http://mobile.vehdjk.com/Article/details/gpilxwghe.sHtML

[R45] 批量删除
来源：http://m.share.epnwcf.com/Article/details/ghpyyofvf.sHtML

find . -name "*.tmp" -delete
来源：http://wap.yfazqb.com/Article/details/gavtkjgnc.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/gyzmjmeuj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.bbcook.cn/Article/details/gelnhoktj.sHtML

[R47] sed 单行替换
来源：http://m.share.sjlbkw.cn/Article/details/gqrjxuefr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fktsv.cn/Article/details/goeguqayg.sHtML

[R48] awk 取指定列
来源：http://read.share.bbcook.cn/Article/details/girrcufyw.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/gfazhwied.sHtML

[R49] awk 带条件
来源：http://www.blog.sjlbkw.cn/Article/details/guczjjwfn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.bbcook.cn/Article/details/gkumhdmxp.sHtML

[R50] awk 求和
来源：http://read.share.vehdjk.com/Article/details/gnqpwznol.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fktsv.cn/Article/details/gyxoumykm.sHtML

[R51] 排序去重取前几
来源：http://m.share.yfazqb.com/Article/details/gcswpafyx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.vehdjk.com/Article/details/glpqosbeq.sHtML

[R52] 统计行数
来源：http://baike.bbcook.cn/Article/details/gthyvkutm.sHtML

wc -l a.txt
来源：http://mobile.tarul.cn/Article/details/gmhyvfqit.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.yfazqb.com/Article/details/gomnwvxwp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.epnwcf.com/Article/details/gqrghrzyw.sHtML

[R54] 比较两个文件
来源：http://read.share.tarul.cn/Article/details/gtowshenk.sHtML

diff a.txt b.txt
来源：http://www.m.share.fktsv.cn/Article/details/gdlbgmkjc.sHtML

[R55] 压缩与解压
来源：http://3g.bbcook.cn/Article/details/gtfrrmtps.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.epnwcf.com/Article/details/gzwoienae.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/gtpvnibyf.sHtML

scp file user@host:/path/
来源：http://m.share.epnwcf.com/Article/details/gwqdctpbx.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fktsv.cn/Article/details/gjohzcqev.sHtML

ssh user@host 'uptime'
来源：http://3g.epnwcf.com/Article/details/gjixbamru.sHtML

[R58] 下载文件
来源：http://www.share.fktsv.cn/Article/details/gxltpvygj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fktsv.cn/Article/details/guwpruhkj.sHtML

[R59] 发 POST JSON
来源：http://wap.vehdjk.com/Article/details/gfecvyoku.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/goarqodjf.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gsfetxjne.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.bbcook.cn/Article/details/gwaqidwhm.sHtML

[R61] 磁盘占用
来源：http://www.blog.tarul.cn/Article/details/gywvafykd.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/gkwvlewcz.sHtML

[R62] 找最占空间的文件
来源：http://read.share.vehdjk.com/Article/details/gqsdkrnex.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.yfazqb.com/Article/details/gpprwevdj.sHtML

[R63] 内存与进程
来源：http://wap.fktsv.cn/Article/details/gwrusdkac.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.epnwcf.com/Article/details/gfplkulzq.sHtML

[R64] 结束进程
来源：http://mobile.fktsv.cn/Article/details/gslpkrdgk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/gwjawfjgc.sHtML

[R65] 查看端口占用
来源：http://www.m.share.tarul.cn/Article/details/gzmfuwbhs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.epnwcf.com/Article/details/gomamrbbu.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/gutuebzez.sHtML

crontab -e;  crontab -l
来源：http://wap.tarul.cn/Article/details/glceaeiar.sHtML

[R67] 生成随机十六进制串
来源：http://blog.vehdjk.com/Article/details/ghywrztfi.sHtML

openssl rand -hex 16
来源：http://m.share.epnwcf.com/Article/details/gabtyybpp.sHtML

[R68] 计算文件校验值
来源：http://3g.epnwcf.com/Article/details/ghfnrzzet.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.tarul.cn/Article/details/gsioydflc.sHtML

[R69] 生成随机密码
来源：http://baike.bbcook.cn/Article/details/gkvyfnyht.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.vehdjk.com/Article/details/gdxfnidel.sHtML

[R70] 时间戳与互转
来源：http://baike.epnwcf.com/Article/details/gkgkujiwq.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.tarul.cn/Article/details/gxlxdqnsk.sHtML

[R71] 日期格式化
来源：http://wap.bbcook.cn/Article/details/gujwijnwv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.vehdjk.com/Article/details/gqjxxzzsg.sHtML

[R72] 等待端口就绪
来源：http://baike.sjlbkw.cn/Article/details/gtwpzhzig.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gealovjsi.sHtML

[R73] 分割大日志
来源：http://wap.fktsv.cn/Article/details/gtndkkixs.sHtML

split -l 1000 big.log part_
来源：http://m.share.vehdjk.com/Article/details/giqqypano.sHtML

[R74] 批量重命名
来源：http://baike.sjlbkw.cn/Article/details/glemsrxoo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.vehdjk.com/Article/details/glhpkyrub.sHtML

[R75] 导出环境变量
来源：http://wap.tarul.cn/Article/details/gmftgtqad.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.epnwcf.com/Article/details/gcakisgwb.sHtML

[R76] 使用临时文件
来源：http://mobile.epnwcf.com/Article/details/gncmmtedk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/gqnzjvtdj.sHtML

[R77] 读取用户输入
来源：http://www.blog.epnwcf.com/Article/details/gugrlnkbl.sHtML

read -rp "请输入: " ans
来源：http://mobile.tarul.cn/Article/details/gozxifenl.sHtML

[R78] 交互式菜单
来源：http://www.blog.tarul.cn/Article/details/gtpwyyork.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.vehdjk.com/Article/details/gpsiohexq.sHtML

[R79] 解析命令行选项
来源：http://m.share.tarul.cn/Article/details/gcjltdeqf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.sjlbkw.cn/Article/details/gpudrtmef.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.tarul.cn/Article/details/gawozizow.sHtML

time ./run.sh
来源：http://read.share.fktsv.cn/Article/details/gxuyhazvf.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gntsblugm.sHtML

S. C / C++ 专题
来源：http://m.share.sjlbkw.cn/Article/details/gjmryarsk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ghrockljv.sHtML

[S01] C：Hello World
来源：http://m.share.bbcook.cn/Article/details/gdvzxxdxv.sHtML

#include <stdio.h>
来源：http://mobile.tarul.cn/Article/details/ggxapmzhq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.vehdjk.com/Article/details/ghgowfypv.sHtML

[S02] C：变量与格式化输出
来源：http://3g.vehdjk.com/Article/details/gqereqesy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.bbcook.cn/Article/details/gpbcyqsmh.sHtML

[S03] C：读入整数
来源：http://m.share.fktsv.cn/Article/details/gfzgwtgvz.sHtML

int x; scanf("%d", &x);
来源：http://read.share.yfazqb.com/Article/details/gqftrzbnd.sHtML

[S04] C：字符串复制
来源：http://www.share.bbcook.cn/Article/details/ggcrphlsv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/gezwlhdzt.sHtML

[S05] C：字符串长度
来源：http://m.share.epnwcf.com/Article/details/gbkyjzlfy.sHtML

strlen(s)
来源：http://blog.tarul.cn/Article/details/groqgsrap.sHtML

[S06] C：字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gzqirzssq.sHtML

strcmp(a, b) == 0
来源：http://blog.bbcook.cn/Article/details/gifhtfbne.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fktsv.cn/Article/details/goooasdod.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.vehdjk.com/Article/details/gqsdjfkrk.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.tarul.cn/Article/details/gyixviudz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.bbcook.cn/Article/details/gwnfaqltx.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.sjlbkw.cn/Article/details/gjwhjjhvp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/glohzfbrj.sHtML

[S10] C：指针与解引用
来源：http://3g.bbcook.cn/Article/details/ghrpevnay.sHtML

int *p = &a;  *p = 5;
来源：http://3g.bbcook.cn/Article/details/giwebijrc.sHtML

[S11] C：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gnfyzrsfi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.vehdjk.com/Article/details/gzncdfhkg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.yfazqb.com/Article/details/gsluhrfdo.sHtML

fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gfnysmtmz.sHtML

[S12] C：写文件
来源：http://www.blog.epnwcf.com/Article/details/gkdpqxfhy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gsbeihwvc.sHtML

[S13] C：宏定义
来源：http://www.share.bbcook.cn/Article/details/gychrowil.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.bbcook.cn/Article/details/gbayiosuw.sHtML

[S14] C：枚举
来源：http://read.share.sjlbkw.cn/Article/details/gnhglgceu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.bbcook.cn/Article/details/gazyyslrk.sHtML

[S15] C：类型转换
来源：http://read.share.tarul.cn/Article/details/gmykddjpg.sHtML

(double) a / b
来源：http://m.share.fktsv.cn/Article/details/gufjnzogx.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fktsv.cn/Article/details/gqkhcgddv.sHtML

x |= (1 << 3);
来源：http://mobile.yfazqb.com/Article/details/gjtadrpml.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gcdqdfzjb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.epnwcf.com/Article/details/goxqpaurg.sHtML

[S18] C：命令行参数
来源：http://wap.vehdjk.com/Article/details/gdykibvqv.sHtML

int main(int argc, char **argv)
来源：http://m.share.fktsv.cn/Article/details/gjllkvxhr.sHtML

[S19] C：快速排序
来源：http://3g.epnwcf.com/Article/details/glcftkfxf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gfwjgipdt.sHtML

[S20] C：二分查找
来源：http://blog.tarul.cn/Article/details/gfqbddjnk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gmyjdripl.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.vehdjk.com/Article/details/gbkjtxczh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fktsv.cn/Article/details/goswljudj.sHtML

[S22] C：字符串转数字
来源：http://read.share.epnwcf.com/Article/details/gbutvjcso.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.tarul.cn/Article/details/gwnkbbpay.sHtML

[S23] C：随机数
来源：http://blog.epnwcf.com/Article/details/gjuhpjcrl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.vehdjk.com/Article/details/gqnlnraux.sHtML

[S24] C：获取本地时间
来源：http://www.blog.epnwcf.com/Article/details/gjtyemgos.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.bbcook.cn/Article/details/gutlrcimt.sHtML

[S25] C：内存拷贝
来源：http://wap.fktsv.cn/Article/details/gxpnwhcns.sHtML

memcpy(dst, src, n);
来源：http://wap.tarul.cn/Article/details/gqcxqxnmw.sHtML

[S26] C：内存清零
来源：http://read.share.sjlbkw.cn/Article/details/gutzszcbw.sHtML

memset(a, 0, sizeof a);
来源：http://wap.sjlbkw.cn/Article/details/gvbtztezj.sHtML

[S27] C：定义常量
来源：http://blog.tarul.cn/Article/details/gkyzbuekl.sHtML

const double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gsahrjthh.sHtML

[S28] C：静态变量
来源：http://mobile.yfazqb.com/Article/details/grszpvkhk.sHtML

static int counter = 0;
来源：http://baike.fktsv.cn/Article/details/ggbgcttnq.sHtML

[S29] C：变参函数
来源：http://www.blog.tarul.cn/Article/details/gyshqiyql.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.yfazqb.com/Article/details/gyrbhokbf.sHtML

[S30] C：头文件保护
来源：http://m.share.bbcook.cn/Article/details/grhamietr.sHtML

#ifndef X_H
来源：http://m.share.bbcook.cn/Article/details/gxdkxfhzl.sHtML

#define X_H
来源：http://www.share.sjlbkw.cn/Article/details/glfflahvs.sHtML

#endif
来源：http://m.share.bbcook.cn/Article/details/ghhrkrhev.sHtML

[S31] C++：Hello World
来源：http://www.share.epnwcf.com/Article/details/gafdazeux.sHtML

#include <iostream>
来源：http://mobile.vehdjk.com/Article/details/gtcqfwhgb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fktsv.cn/Article/details/gsqrxegjv.sHtML

[S32] C++：字符串
来源：http://www.m.share.fktsv.cn/Article/details/gavodsflg.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.epnwcf.com/Article/details/gpbfkmpwn.sHtML

[S33] C++：vector 增删
来源：http://wap.bbcook.cn/Article/details/gvhfjnhte.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gqwletcrp.sHtML

[S34] C++：遍历 vector
来源：http://read.share.sjlbkw.cn/Article/details/gaqzhenoa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.sjlbkw.cn/Article/details/gngareasv.sHtML

[S35] C++：map
来源：http://blog.epnwcf.com/Article/details/gfjhfgkqc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/gluplzluw.sHtML

[S36] C++：unordered_map
来源：http://blog.fktsv.cn/Article/details/gugymqlxq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gkidwaiqk.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/grsssahyg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.epnwcf.com/Article/details/gxzehwrdb.sHtML

[S38] C++：排序
来源：http://www.share.tarul.cn/Article/details/ggjdqunfq.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.vehdjk.com/Article/details/ghynpwwst.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.bbcook.cn/Article/details/gnernaayr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.vehdjk.com/Article/details/gsnmtlwhk.sHtML

[S40] C++：查找元素
来源：http://www.blog.fktsv.cn/Article/details/gspqesbzg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.sjlbkw.cn/Article/details/gkjqmrsdw.sHtML

[S41] C++：类与构造函数
来源：http://www.share.tarul.cn/Article/details/gqzofsyha.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.yfazqb.com/Article/details/gtcoajlpe.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/gohzgbnvq.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fktsv.cn/Article/details/gdrxowbsp.sHtML

[S43] C++：智能指针
来源：http://wap.fktsv.cn/Article/details/gysbwrglt.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.bbcook.cn/Article/details/gtniwhqbw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.vehdjk.com/Article/details/gjsjqikwt.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.tarul.cn/Article/details/ghxriaqdn.sHtML

[S45] C++：lambda
来源：http://blog.vehdjk.com/Article/details/gwnncxeie.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.sjlbkw.cn/Article/details/gzetrwdby.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/glmwioizr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.tarul.cn/Article/details/gbwnnqamv.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.epnwcf.com/Article/details/guyrhwsvc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gtzkzxxmz.sHtML

[S48] C++：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gcsebfwsp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.bbcook.cn/Article/details/gtqojfhja.sHtML

while (std::getline(in, line)) { }
来源：http://3g.yfazqb.com/Article/details/gttenwzyz.sHtML

[S49] C++：写文件
来源：http://3g.bbcook.cn/Article/details/goznsdjdc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/gzoorjjhd.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/gnkgswqso.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/ggyhdpsua.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gmqlvkiws.sHtML

static_cast<double>(a) / b
来源：http://mobile.fktsv.cn/Article/details/gbddbphgn.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.yfazqb.com/Article/details/gqfjmiyfz.sHtML

int size() const noexcept { return n_; }
来源：http://baike.epnwcf.com/Article/details/gylbnyvhj.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/gusxwgdpp.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.sjlbkw.cn/Article/details/gtzdhepil.sHtML

[S54] C++：异常处理
来源：http://wap.epnwcf.com/Article/details/gfcbrrwiq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.bbcook.cn/Article/details/gjonuuyzi.sHtML

[S55] C++：结构化绑定
来源：http://baike.tarul.cn/Article/details/gvilrwpau.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.tarul.cn/Article/details/gbujppqrh.sHtML

[S56] C++：optional
来源：http://3g.yfazqb.com/Article/details/gqgmwfgvf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.yfazqb.com/Article/details/gerqofoyf.sHtML

[S57] C++：编译期常量
来源：http://mobile.yfazqb.com/Article/details/ghimnrjrn.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gazvycvdr.sHtML

[S58] C++：命名空间
来源：http://www.blog.epnwcf.com/Article/details/gghblfejw.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.epnwcf.com/Article/details/gzchndsou.sHtML

[S59] C++：静态断言
来源：http://baike.fktsv.cn/Article/details/gdlyirctq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.tarul.cn/Article/details/gozofkpsg.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.yfazqb.com/Article/details/giezwosyv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/gfpdrmhtg.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwjjktor.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gnwromwhj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gixakilvy.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.vehdjk.com/Article/details/gfokjfzkc.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gftrdmntv.sHtML

[T02] Kotlin：变量
来源：http://www.share.tarul.cn/Article/details/giczqkqao.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.sjlbkw.cn/Article/details/gbmpjmvuv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.yfazqb.com/Article/details/guohmhisn.sHtML

"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/guhjkdusd.sHtML

[T04] Kotlin：空安全
来源：http://www.share.yfazqb.com/Article/details/gkyftexen.sHtML

val n: String? = null;  n?.length
来源：http://3g.yfazqb.com/Article/details/gghvjiyny.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.vehdjk.com/Article/details/gixigbfrl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.epnwcf.com/Article/details/gxlnnfbdd.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.epnwcf.com/Article/details/gvnuysasw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.vehdjk.com/Article/details/gjkoqiwue.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.tarul.cn/Article/details/giozpxwcf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.vehdjk.com/Article/details/ggsmqzscq.sHtML

[T08] Kotlin：数据类
来源：http://mobile.vehdjk.com/Article/details/grbcsmfqa.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.bbcook.cn/Article/details/gdgxysbkl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.yfazqb.com/Article/details/gupwhkxpq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fktsv.cn/Article/details/gcknuzbpz.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gvumjfxkj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.tarul.cn/Article/details/grvqjsxku.sHtML

[T11] Kotlin：协程
来源：http://mobile.yfazqb.com/Article/details/gnjmmykqp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fktsv.cn/Article/details/gswuoapga.sHtML

[T12] Kotlin：解构声明
来源：http://wap.vehdjk.com/Article/details/gqtqfekws.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.tarul.cn/Article/details/gvpcmjebt.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.sjlbkw.cn/Article/details/gbzktstcj.sHtML

val m = mapOf("a" to 1)
来源：http://3g.bbcook.cn/Article/details/ghpxeighu.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/gputeldqf.sHtML

for (i in 1..10) println(i)
来源：http://m.share.bbcook.cn/Article/details/gjcwvqxyw.sHtML

[T15] Kotlin：接口
来源：http://mobile.fktsv.cn/Article/details/gmdqogkxp.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gbgqejqme.sHtML

[T16] Swift：Hello World
来源：http://baike.tarul.cn/Article/details/gzzwoxtsf.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gbiohqbam.sHtML

[T17] Swift：变量与常量
来源：http://read.share.tarul.cn/Article/details/gwglyhssr.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzqqsmkr.sHtML

[T18] Swift：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gujcqadus.sHtML

"值: \(b)"
来源：http://m.share.sjlbkw.cn/Article/details/gudbmbvln.sHtML

[T19] Swift：可选绑定
来源：http://mobile.vehdjk.com/Article/details/glldqvlxt.sHtML

if let n = opt { print(n) }
来源：http://blog.yfazqb.com/Article/details/geloxlycg.sHtML

[T20] Swift：数组操作
来源：http://www.share.vehdjk.com/Article/details/gxqetjyzb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fktsv.cn/Article/details/gphqwptxk.sHtML

[T21] Swift：遍历
来源：http://wap.yfazqb.com/Article/details/gpfnipfwj.sHtML

for x in a { print(x) }
来源：http://www.share.tarul.cn/Article/details/govpbzkty.sHtML

[T22] Swift：字典
来源：http://read.share.fktsv.cn/Article/details/gognapjsp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.tarul.cn/Article/details/gmuzagmxk.sHtML

[T23] Swift：函数
来源：http://blog.epnwcf.com/Article/details/ghectqdyo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.tarul.cn/Article/details/gxwiuexrz.sHtML

[T24] Swift：闭包
来源：http://wap.tarul.cn/Article/details/gcmfyupww.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.epnwcf.com/Article/details/gkeuijdew.sHtML

[T25] Swift：结构体
来源：http://mobile.fktsv.cn/Article/details/ggicszztq.sHtML

struct P { var x: Int }
来源：http://mobile.epnwcf.com/Article/details/gfsjlgfio.sHtML

[T26] Swift：类与重写
来源：http://read.share.tarul.cn/Article/details/gxcyvyngg.sHtML

class A: Base { override func f() {} }
来源：http://m.share.tarul.cn/Article/details/glbhajibm.sHtML


<!-- 参考信息 -->