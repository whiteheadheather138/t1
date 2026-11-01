代发 wailian999

echo "${#s}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmpdtjyp.sHtML

[R22] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/grzfsuoyh.sHtML

echo "${s:0:5}"
来源：http://www.share.epnwcf.com/Article/details/gykmlrpje.sHtML

[R23] 字符串替换
来源：http://blog.epnwcf.com/Article/details/gnijyriay.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.bbcook.cn/Article/details/gypqiinpa.sHtML

[R24] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gkvynwxpm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.tarul.cn/Article/details/gjhnxoowq.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.sjlbkw.cn/Article/details/gpaztbkyb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.epnwcf.com/Article/details/gojqepute.sHtML

[R26] 命令替换
来源：http://www.blog.fktsv.cn/Article/details/grljhbfbh.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fktsv.cn/Article/details/grnrnhcfb.sHtML

[R27] 算术展开
来源：http://www.share.vehdjk.com/Article/details/gxxyfyvmf.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/glmqrbgqb.sHtML

[R28] 浮点运算
来源：http://read.share.vehdjk.com/Article/details/gikxubjmt.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/gmmmdwojt.sHtML

[R29] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/gjpufyqox.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/gopkubnxs.sHtML

[R30] 函数返回状态码
来源：http://wap.epnwcf.com/Article/details/gpxiwsnoj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fktsv.cn/Article/details/gmopcxrpo.sHtML

[R31] 局部变量
来源：http://m.share.yfazqb.com/Article/details/gfjwbznsp.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.sjlbkw.cn/Article/details/graqitogi.sHtML

[R32] 参数个数校验
来源：http://www.blog.fktsv.cn/Article/details/glpyvlpxf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gzxtyxslm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.vehdjk.com/Article/details/gcylywzxw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.yfazqb.com/Article/details/gpdlxjfjn.sHtML

[R34] 退出时清理
来源：http://www.share.epnwcf.com/Article/details/gxtbfonsx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gkfwrnswz.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/gxorykxdc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.bbcook.cn/Article/details/gqigxaclh.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gpbibmzmb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fktsv.cn/Article/details/gogzzclet.sHtML

[R37] 把输出赋给变量
来源：http://read.share.vehdjk.com/Article/details/gfpfoqdvh.sHtML

files=$(ls -1)
来源：http://m.share.vehdjk.com/Article/details/gubeuzwpo.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/glzospcmn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.vehdjk.com/Article/details/gfrbtqjxb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/gzlphghdu.sHtML

cmd > out.log 2>&1
来源：http://wap.epnwcf.com/Article/details/gbbdoemfc.sHtML

[R40] 追加写日志
来源：http://www.share.epnwcf.com/Article/details/gbnbawjsu.sHtML

echo "log" >> out.log
来源：http://m.share.epnwcf.com/Article/details/gbyzuikwf.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gaieckzmn.sHtML

cmd >/dev/null 2>&1
来源：http://wap.epnwcf.com/Article/details/gxskciyug.sHtML

[R42] 输入重定向
来源：http://m.share.sjlbkw.cn/Article/details/gkemkwrbz.sHtML

wc -l < a.txt
来源：http://blog.sjlbkw.cn/Article/details/gdebgtevm.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gyrbimxxg.sHtML

find . -name "*.log" -type f
来源：http://www.share.epnwcf.com/Article/details/gmjsrqvtu.sHtML

[R44] 按修改时间查找
来源：http://3g.vehdjk.com/Article/details/gxjymftrk.sHtML

find . -mtime -7 -type f
来源：http://wap.epnwcf.com/Article/details/gfuhlkzyg.sHtML

[R45] 批量删除
来源：http://www.m.share.vehdjk.com/Article/details/gkykhumii.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.sjlbkw.cn/Article/details/gaqonqnye.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.sjlbkw.cn/Article/details/ggefmoqec.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.yfazqb.com/Article/details/gmnbfafro.sHtML

[R47] sed 单行替换
来源：http://3g.bbcook.cn/Article/details/gwaxpuhzr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gwhqhsgjz.sHtML

[R48] awk 取指定列
来源：http://m.share.vehdjk.com/Article/details/gqllbplyp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.tarul.cn/Article/details/gptwavnva.sHtML

[R49] awk 带条件
来源：http://read.share.epnwcf.com/Article/details/gocgsjmff.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fktsv.cn/Article/details/gjximeppq.sHtML

[R50] awk 求和
来源：http://read.share.tarul.cn/Article/details/ggbbkjsju.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/ggnkpfxpv.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/gtqsamwhh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.vehdjk.com/Article/details/gpewzjsia.sHtML

[R52] 统计行数
来源：http://blog.yfazqb.com/Article/details/gpijardwd.sHtML

wc -l a.txt
来源：http://3g.epnwcf.com/Article/details/gnsmmsnps.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.bbcook.cn/Article/details/gvcaxlxvc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.epnwcf.com/Article/details/gpyoxpfcv.sHtML

[R54] 比较两个文件
来源：http://www.blog.epnwcf.com/Article/details/gcrsmwzso.sHtML

diff a.txt b.txt
来源：http://read.share.bbcook.cn/Article/details/gkgozhepr.sHtML

[R55] 压缩与解压
来源：http://3g.vehdjk.com/Article/details/ggojeraoy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.tarul.cn/Article/details/glgwbslht.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/gunmmepio.sHtML

scp file user@host:/path/
来源：http://blog.bbcook.cn/Article/details/gvwhoxtgm.sHtML

[R57] 远程执行命令
来源：http://www.m.share.vehdjk.com/Article/details/gyaevfsvk.sHtML

ssh user@host 'uptime'
来源：http://blog.sjlbkw.cn/Article/details/gubzrknvd.sHtML

[R58] 下载文件
来源：http://mobile.vehdjk.com/Article/details/gvpjbtees.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/gwgsdwwcs.sHtML

[R59] 发 POST JSON
来源：http://baike.yfazqb.com/Article/details/glvukjboy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/gfaipvokt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gbhsxycby.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.tarul.cn/Article/details/gmisaziqv.sHtML

[R61] 磁盘占用
来源：http://read.share.bbcook.cn/Article/details/gasoexkoy.sHtML

df -h;  du -sh *
来源：http://www.blog.sjlbkw.cn/Article/details/gaamprhhc.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fktsv.cn/Article/details/gfylawczn.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/gwmooyzov.sHtML

[R63] 内存与进程
来源：http://read.share.yfazqb.com/Article/details/gnewprkkb.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.sjlbkw.cn/Article/details/gqwiunqvq.sHtML

[R64] 结束进程
来源：http://www.blog.epnwcf.com/Article/details/gjetuqcmu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fktsv.cn/Article/details/gxstmbnen.sHtML

[R65] 查看端口占用
来源：http://m.share.yfazqb.com/Article/details/gydnylikt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fktsv.cn/Article/details/gzrjfznmv.sHtML

[R66] 定时任务
来源：http://m.share.sjlbkw.cn/Article/details/gbvnesitj.sHtML

crontab -e;  crontab -l
来源：http://www.blog.bbcook.cn/Article/details/grenzitzp.sHtML

[R67] 生成随机十六进制串
来源：http://wap.vehdjk.com/Article/details/geuayqxdv.sHtML

openssl rand -hex 16
来源：http://wap.yfazqb.com/Article/details/gjartijmc.sHtML

[R68] 计算文件校验值
来源：http://3g.epnwcf.com/Article/details/gvctejyby.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gglueqylk.sHtML

[R69] 生成随机密码
来源：http://read.share.yfazqb.com/Article/details/grqinpjxr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.tarul.cn/Article/details/gevugbzsp.sHtML

[R70] 时间戳与互转
来源：http://www.share.bbcook.cn/Article/details/gbwntiyqw.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.sjlbkw.cn/Article/details/gjwmhmdak.sHtML

[R71] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gujchoooe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.yfazqb.com/Article/details/gczmhmkkv.sHtML

[R72] 等待端口就绪
来源：http://blog.vehdjk.com/Article/details/girzrvxrh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/goeswwftx.sHtML

[R73] 分割大日志
来源：http://www.blog.vehdjk.com/Article/details/ggieuaxdg.sHtML

split -l 1000 big.log part_
来源：http://baike.vehdjk.com/Article/details/gpsrdolxc.sHtML

[R74] 批量重命名
来源：http://3g.sjlbkw.cn/Article/details/gsuhtrzlm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.epnwcf.com/Article/details/gjrgfizts.sHtML

[R75] 导出环境变量
来源：http://mobile.bbcook.cn/Article/details/gozzlndht.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.bbcook.cn/Article/details/gajfsktsc.sHtML

[R76] 使用临时文件
来源：http://www.blog.yfazqb.com/Article/details/gkrzpeuxd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gqfpinefg.sHtML

[R77] 读取用户输入
来源：http://baike.bbcook.cn/Article/details/gfqcfiwbe.sHtML

read -rp "请输入: " ans
来源：http://m.share.epnwcf.com/Article/details/gpdypkzpu.sHtML

[R78] 交互式菜单
来源：http://read.share.epnwcf.com/Article/details/gplciipjf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.bbcook.cn/Article/details/gyblgcdxa.sHtML

[R79] 解析命令行选项
来源：http://baike.sjlbkw.cn/Article/details/gqrraodfk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.vehdjk.com/Article/details/gaoqxxceg.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fktsv.cn/Article/details/gmbwsissg.sHtML

time ./run.sh
来源：http://www.share.sjlbkw.cn/Article/details/ghpkrkzir.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkszllvdg.sHtML

S. C / C++ 专题
来源：http://mobile.bbcook.cn/Article/details/guhpgwcpg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gkhiqdtki.sHtML

[S01] C：Hello World
来源：http://mobile.vehdjk.com/Article/details/glirhsoyw.sHtML

#include <stdio.h>
来源：http://mobile.bbcook.cn/Article/details/gjzyinsjo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.tarul.cn/Article/details/gzlbftfcj.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.bbcook.cn/Article/details/ggyzevsub.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.yfazqb.com/Article/details/ggovwhhqd.sHtML

[S03] C：读入整数
来源：http://www.blog.yfazqb.com/Article/details/giuovegux.sHtML

int x; scanf("%d", &x);
来源：http://blog.bbcook.cn/Article/details/gtaooplwn.sHtML

[S04] C：字符串复制
来源：http://www.blog.fktsv.cn/Article/details/gibnewsbd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.epnwcf.com/Article/details/gonyffznb.sHtML

[S05] C：字符串长度
来源：http://www.blog.yfazqb.com/Article/details/geiorqdpl.sHtML

strlen(s)
来源：http://wap.fktsv.cn/Article/details/gxitvvfag.sHtML

[S06] C：字符串比较
来源：http://baike.yfazqb.com/Article/details/gsezsxpgx.sHtML

strcmp(a, b) == 0
来源：http://blog.tarul.cn/Article/details/gkzmwlbfv.sHtML

[S07] C：数组遍历求和
来源：http://3g.tarul.cn/Article/details/gwvksdfbv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fktsv.cn/Article/details/gaalooykj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fktsv.cn/Article/details/gqbswgjan.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.sjlbkw.cn/Article/details/gtrnbjklu.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/ghfvglyfi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.tarul.cn/Article/details/gjnfpolcl.sHtML

[S10] C：指针与解引用
来源：http://www.blog.vehdjk.com/Article/details/gczsttgzl.sHtML

int *p = &a;  *p = 5;
来源：http://3g.sjlbkw.cn/Article/details/gfozjdpta.sHtML

[S11] C：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gbnoyausk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.epnwcf.com/Article/details/gioyiumvr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.epnwcf.com/Article/details/ghdnflkrc.sHtML

fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gipounfok.sHtML

[S12] C：写文件
来源：http://mobile.bbcook.cn/Article/details/gbkldbvhk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gmtawivle.sHtML

[S13] C：宏定义
来源：http://mobile.vehdjk.com/Article/details/gllirzwui.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fktsv.cn/Article/details/glwrfpzub.sHtML

[S14] C：枚举
来源：http://3g.fktsv.cn/Article/details/ghylmcnkx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.tarul.cn/Article/details/gyhxwxxgv.sHtML

[S15] C：类型转换
来源：http://www.share.sjlbkw.cn/Article/details/gejtmxwiy.sHtML

(double) a / b
来源：http://wap.bbcook.cn/Article/details/gnoyowtqc.sHtML

[S16] C：位操作置位
来源：http://wap.sjlbkw.cn/Article/details/gindqtfkp.sHtML

x |= (1 << 3);
来源：http://www.m.share.tarul.cn/Article/details/gtyuouaos.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gbanfptza.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/gegyvpevz.sHtML

[S18] C：命令行参数
来源：http://read.share.vehdjk.com/Article/details/gcgmvlkbf.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gpxcavean.sHtML

[S19] C：快速排序
来源：http://www.m.share.epnwcf.com/Article/details/gdswdnekr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/guuzzbsye.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/gdwxrtcoo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/geshueryh.sHtML

[S21] C：字符类别判断
来源：http://mobile.fktsv.cn/Article/details/gqsvtjmxe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.yfazqb.com/Article/details/gisltnwho.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/ghcdcblks.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.vehdjk.com/Article/details/ghkqozexr.sHtML

[S23] C：随机数
来源：http://www.share.vehdjk.com/Article/details/gopzbtwyo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.sjlbkw.cn/Article/details/gzdzoccha.sHtML

[S24] C：获取本地时间
来源：http://wap.tarul.cn/Article/details/gbkvyctbs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.epnwcf.com/Article/details/gmokiwcwc.sHtML

[S25] C：内存拷贝
来源：http://3g.yfazqb.com/Article/details/gthawxdlt.sHtML

memcpy(dst, src, n);
来源：http://www.share.vehdjk.com/Article/details/gxyiioaye.sHtML

[S26] C：内存清零
来源：http://www.blog.tarul.cn/Article/details/gnmizghem.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.vehdjk.com/Article/details/ghxhbbzfe.sHtML

[S27] C：定义常量
来源：http://www.share.bbcook.cn/Article/details/gbobfkokp.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gzmkghkaw.sHtML

[S28] C：静态变量
来源：http://blog.bbcook.cn/Article/details/gjzqspyjl.sHtML

static int counter = 0;
来源：http://www.blog.tarul.cn/Article/details/gtsmmcwhj.sHtML

[S29] C：变参函数
来源：http://baike.epnwcf.com/Article/details/gxibfleni.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.tarul.cn/Article/details/gbldkkguy.sHtML

[S30] C：头文件保护
来源：http://mobile.tarul.cn/Article/details/gqvjhppxy.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/guhnoiwrk.sHtML

#define X_H
来源：http://3g.vehdjk.com/Article/details/gmdnjsbgs.sHtML

#endif
来源：http://baike.sjlbkw.cn/Article/details/gadojdezx.sHtML

[S31] C++：Hello World
来源：http://m.share.fktsv.cn/Article/details/gqkgpcafp.sHtML

#include <iostream>
来源：http://3g.epnwcf.com/Article/details/gppddliom.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fktsv.cn/Article/details/gaxlhptya.sHtML

[S32] C++：字符串
来源：http://mobile.fktsv.cn/Article/details/goiufwfly.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.yfazqb.com/Article/details/ghiwrvzjm.sHtML

[S33] C++：vector 增删
来源：http://www.blog.epnwcf.com/Article/details/gtgkgnzkj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.epnwcf.com/Article/details/gjgxtffqq.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.epnwcf.com/Article/details/gdqtdtvjt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gqxrneyfk.sHtML

[S35] C++：map
来源：http://mobile.fktsv.cn/Article/details/ggorcylpe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/grnisrwkg.sHtML

[S36] C++：unordered_map
来源：http://wap.bbcook.cn/Article/details/gycrdnfdr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gjaedfhqv.sHtML

[S37] C++：set
来源：http://baike.sjlbkw.cn/Article/details/gxhphnuqe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.vehdjk.com/Article/details/gkpfxrscx.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gwzmsdkbi.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.epnwcf.com/Article/details/ghffpyzte.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.sjlbkw.cn/Article/details/gamsznucg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.epnwcf.com/Article/details/gasqwuxoe.sHtML

[S40] C++：查找元素
来源：http://baike.sjlbkw.cn/Article/details/gkjswrhve.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.bbcook.cn/Article/details/gbtnrlxwh.sHtML

[S41] C++：类与构造函数
来源：http://3g.fktsv.cn/Article/details/gomxukeuj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.vehdjk.com/Article/details/gulowgmdy.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.yfazqb.com/Article/details/gjvncynmv.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.bbcook.cn/Article/details/gysgygjys.sHtML

[S43] C++：智能指针
来源：http://m.share.tarul.cn/Article/details/gdvmntkio.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.vehdjk.com/Article/details/gxclaxibd.sHtML

[S44] C++：引用传参
来源：http://wap.tarul.cn/Article/details/gnkajwzfp.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/ggxewtsxk.sHtML

[S45] C++：lambda
来源：http://3g.tarul.cn/Article/details/gojgijmyl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.epnwcf.com/Article/details/gmncgvmin.sHtML

[S46] C++：函数模板
来源：http://wap.fktsv.cn/Article/details/gcptpuylh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gdgrzztey.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.sjlbkw.cn/Article/details/gdriiihyd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.bbcook.cn/Article/details/gerezfvyi.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gwtrehzxb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.epnwcf.com/Article/details/gjtzwczrc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fktsv.cn/Article/details/gaynfnjyp.sHtML

[S49] C++：写文件
来源：http://m.share.vehdjk.com/Article/details/gumnvncgn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.tarul.cn/Article/details/gjvylblzy.sHtML

[S50] C++：格式化数字
来源：http://read.share.sjlbkw.cn/Article/details/ghvzjnpwj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gjbwvjjfz.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gnpvcezfv.sHtML

static_cast<double>(a) / b
来源：http://m.share.fktsv.cn/Article/details/gzespyhpy.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.vehdjk.com/Article/details/gxinebjar.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/gmtwpsdfg.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/gritorgty.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.vehdjk.com/Article/details/gkkqkiryo.sHtML

[S54] C++：异常处理
来源：http://m.share.yfazqb.com/Article/details/gmdgfsnnm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.tarul.cn/Article/details/gpkwsozna.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/gziecixsd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.vehdjk.com/Article/details/gtdlesbtw.sHtML

[S56] C++：optional
来源：http://blog.bbcook.cn/Article/details/gslrjjdwz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fktsv.cn/Article/details/glebxfybi.sHtML

[S57] C++：编译期常量
来源：http://read.share.epnwcf.com/Article/details/gjvabxisq.sHtML

constexpr int N = 10;
来源：http://www.m.share.tarul.cn/Article/details/gzktpuzwe.sHtML

[S58] C++：命名空间
来源：http://www.share.epnwcf.com/Article/details/granjhmyp.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/gwdbnmdzc.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/gtrdwbsbw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.sjlbkw.cn/Article/details/gxtkofvhc.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.epnwcf.com/Article/details/gbxygabin.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.bbcook.cn/Article/details/gqtwncmqd.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/giqngwpnt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/ghavtbwpf.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gizlfsegy.sHtML

[T01] Kotlin：Hello World
来源：http://blog.vehdjk.com/Article/details/gmbjmvsal.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gtwbfhbzn.sHtML

[T02] Kotlin：变量
来源：http://www.share.epnwcf.com/Article/details/geidrzpqe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/gtcprzdmp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.epnwcf.com/Article/details/gzrlrcgfk.sHtML

"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/gvprdofas.sHtML

[T04] Kotlin：空安全
来源：http://mobile.epnwcf.com/Article/details/gcisccqzm.sHtML

val n: String? = null;  n?.length
来源：http://baike.sjlbkw.cn/Article/details/gldobeoyt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gmwgawmja.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/gzwrbggle.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.tarul.cn/Article/details/gidrxuvfl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.vehdjk.com/Article/details/grcyjwiqg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fktsv.cn/Article/details/gnlpfydhb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.epnwcf.com/Article/details/gminpnxvm.sHtML

[T08] Kotlin：数据类
来源：http://read.share.bbcook.cn/Article/details/gouvqzmef.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.tarul.cn/Article/details/gvattmdqh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.sjlbkw.cn/Article/details/gueqsrcdj.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.yfazqb.com/Article/details/groykxecp.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.yfazqb.com/Article/details/gsnotsddz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.tarul.cn/Article/details/gdzeqrbne.sHtML

[T11] Kotlin：协程
来源：http://read.share.sjlbkw.cn/Article/details/gkuhftxcc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.bbcook.cn/Article/details/ghcpzipuu.sHtML

[T12] Kotlin：解构声明
来源：http://baike.yfazqb.com/Article/details/gqvpgxxqw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.epnwcf.com/Article/details/gxlscfdgx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/gfhknkyqi.sHtML

val m = mapOf("a" to 1)
来源：http://3g.tarul.cn/Article/details/gxmqqkvpy.sHtML

[T14] Kotlin：循环
来源：http://baike.vehdjk.com/Article/details/gjuzbwvnz.sHtML

for (i in 1..10) println(i)
来源：http://wap.bbcook.cn/Article/details/gjagocbdl.sHtML

[T15] Kotlin：接口
来源：http://3g.epnwcf.com/Article/details/gyzpotlgm.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.yfazqb.com/Article/details/goylmxhwa.sHtML

[T16] Swift：Hello World
来源：http://read.share.fktsv.cn/Article/details/gmjtynbod.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/giodpxpvl.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.tarul.cn/Article/details/gcrotjslh.sHtML

var a = 1;  let b = 2
来源：http://3g.sjlbkw.cn/Article/details/gvfwsmwes.sHtML

[T18] Swift：字符串插值
来源：http://wap.tarul.cn/Article/details/gmkvsfrsx.sHtML

"值: \(b)"
来源：http://3g.sjlbkw.cn/Article/details/gnqxfamkx.sHtML

[T19] Swift：可选绑定
来源：http://wap.bbcook.cn/Article/details/gepuknffz.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.epnwcf.com/Article/details/gexcuoken.sHtML

[T20] Swift：数组操作
来源：http://3g.vehdjk.com/Article/details/gceulfdng.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.bbcook.cn/Article/details/gjjblkxxl.sHtML

[T21] Swift：遍历
来源：http://mobile.tarul.cn/Article/details/ggwwbfbaf.sHtML

for x in a { print(x) }
来源：http://3g.tarul.cn/Article/details/gupvqelvs.sHtML

[T22] Swift：字典
来源：http://www.blog.bbcook.cn/Article/details/gmjzsjviu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.yfazqb.com/Article/details/gkytavrlj.sHtML

[T23] Swift：函数
来源：http://www.blog.tarul.cn/Article/details/gxzgtqcfb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/gtlogymuq.sHtML

[T24] Swift：闭包
来源：http://baike.epnwcf.com/Article/details/gbvbmjldj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gmwhndgyp.sHtML


<!-- 参考信息 -->