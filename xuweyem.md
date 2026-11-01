代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.vehdjk.com/Article/details/gdmmzyvqr.sHtML

[R30] 函数返回状态码
来源：http://3g.bbcook.cn/Article/details/ggntkhylv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.tarul.cn/Article/details/gagobuvfz.sHtML

[R31] 局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gapzvlzkn.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.yfazqb.com/Article/details/gmnwkmptr.sHtML

[R32] 参数个数校验
来源：http://baike.tarul.cn/Article/details/gqrxqawmd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gbbfevobl.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fktsv.cn/Article/details/gbxddziua.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.vehdjk.com/Article/details/gcvhtbrph.sHtML

[R34] 退出时清理
来源：http://mobile.bbcook.cn/Article/details/gciivrdmh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gtvxvxkmw.sHtML

[R35] 后台执行并等待
来源：http://wap.fktsv.cn/Article/details/gcjppbdxj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.epnwcf.com/Article/details/gfawtqnlh.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/ghwzuzabj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.tarul.cn/Article/details/gmtjzalex.sHtML

[R37] 把输出赋给变量
来源：http://3g.sjlbkw.cn/Article/details/gowgmmxhg.sHtML

files=$(ls -1)
来源：http://wap.tarul.cn/Article/details/gbhlovgjj.sHtML

[R38] 管道串联
来源：http://www.m.share.vehdjk.com/Article/details/gmujcbodj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/glpwahtgy.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/gysmwazle.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fktsv.cn/Article/details/giivqyrbm.sHtML

[R40] 追加写日志
来源：http://www.m.share.fktsv.cn/Article/details/gdzxerqfv.sHtML

echo "log" >> out.log
来源：http://wap.tarul.cn/Article/details/gdsumserg.sHtML

[R41] 丢弃输出
来源：http://www.share.vehdjk.com/Article/details/gsdcnjlbh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.yfazqb.com/Article/details/gmduruzkz.sHtML

[R42] 输入重定向
来源：http://www.share.epnwcf.com/Article/details/gchajafkk.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/guwaqoqjl.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fktsv.cn/Article/details/gbzjvmzzi.sHtML

find . -name "*.log" -type f
来源：http://www.share.tarul.cn/Article/details/gnxlifcmo.sHtML

[R44] 按修改时间查找
来源：http://www.blog.tarul.cn/Article/details/gucjscuhy.sHtML

find . -mtime -7 -type f
来源：http://3g.yfazqb.com/Article/details/gtdhoqdot.sHtML

[R45] 批量删除
来源：http://www.m.share.epnwcf.com/Article/details/gkvhwwqzf.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gesciktay.sHtML

[R46] 递归替换文件内容
来源：http://wap.bbcook.cn/Article/details/gqczphnlz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.bbcook.cn/Article/details/glwmoixzu.sHtML

[R47] sed 单行替换
来源：http://www.blog.tarul.cn/Article/details/gfgysjdrg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fktsv.cn/Article/details/gftabuhpw.sHtML

[R48] awk 取指定列
来源：http://www.m.share.vehdjk.com/Article/details/glbvtfyby.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.epnwcf.com/Article/details/gzoafptbn.sHtML

[R49] awk 带条件
来源：http://baike.vehdjk.com/Article/details/gawayccuz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fktsv.cn/Article/details/ghammsxky.sHtML

[R50] awk 求和
来源：http://3g.epnwcf.com/Article/details/gusglbsuj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/ggnkbwiyo.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuaberjk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fktsv.cn/Article/details/giiylxcrm.sHtML

[R52] 统计行数
来源：http://www.m.share.fktsv.cn/Article/details/gcspbooxv.sHtML

wc -l a.txt
来源：http://read.share.yfazqb.com/Article/details/ggckslwun.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.tarul.cn/Article/details/glqevgfqa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.bbcook.cn/Article/details/gqsovhalf.sHtML

[R54] 比较两个文件
来源：http://read.share.tarul.cn/Article/details/garqrtkqd.sHtML

diff a.txt b.txt
来源：http://read.share.tarul.cn/Article/details/gmtpqwxcp.sHtML

[R55] 压缩与解压
来源：http://m.share.tarul.cn/Article/details/gzngypzoo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.epnwcf.com/Article/details/gdxyxeznx.sHtML

[R56] 远程拷贝
来源：http://read.share.fktsv.cn/Article/details/gfqddkyon.sHtML

scp file user@host:/path/
来源：http://m.share.bbcook.cn/Article/details/grznppilx.sHtML

[R57] 远程执行命令
来源：http://3g.yfazqb.com/Article/details/ghaeybatn.sHtML

ssh user@host 'uptime'
来源：http://blog.tarul.cn/Article/details/gmkwwhijd.sHtML

[R58] 下载文件
来源：http://read.share.vehdjk.com/Article/details/gcehirpsn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.tarul.cn/Article/details/gvjnxudnz.sHtML

[R59] 发 POST JSON
来源：http://www.share.fktsv.cn/Article/details/gdxqejnhq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.tarul.cn/Article/details/guorkxgtd.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gqdwjobfi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.yfazqb.com/Article/details/gggrmtywa.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/gdomxfdzg.sHtML

df -h;  du -sh *
来源：http://www.blog.yfazqb.com/Article/details/gbgybvuaw.sHtML

[R62] 找最占空间的文件
来源：http://3g.fktsv.cn/Article/details/gjywsrtgo.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fktsv.cn/Article/details/gkvuxmjer.sHtML

[R63] 内存与进程
来源：http://read.share.yfazqb.com/Article/details/gbajibaxe.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/gaawrkcba.sHtML

[R64] 结束进程
来源：http://mobile.sjlbkw.cn/Article/details/gkqbqdryz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/gzawudlkl.sHtML

[R65] 查看端口占用
来源：http://www.share.bbcook.cn/Article/details/gjxzntkeu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.vehdjk.com/Article/details/gdcuprgse.sHtML

[R66] 定时任务
来源：http://mobile.sjlbkw.cn/Article/details/gwqdjemjy.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.epnwcf.com/Article/details/gvrosqbhz.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.bbcook.cn/Article/details/gzjersgmc.sHtML

openssl rand -hex 16
来源：http://www.blog.vehdjk.com/Article/details/grzpvmdlf.sHtML

[R68] 计算文件校验值
来源：http://blog.fktsv.cn/Article/details/gcpscfjsb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.yfazqb.com/Article/details/gaujrjlen.sHtML

[R69] 生成随机密码
来源：http://mobile.tarul.cn/Article/details/gtgxaimjj.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.tarul.cn/Article/details/gmilgcmnh.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fktsv.cn/Article/details/gqvymhmlh.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.bbcook.cn/Article/details/gxexlhaiz.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gyuyexunr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.bbcook.cn/Article/details/ghrrystnp.sHtML

[R72] 等待端口就绪
来源：http://m.share.bbcook.cn/Article/details/gqcxojach.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/gecttbkbs.sHtML

[R73] 分割大日志
来源：http://www.m.share.bbcook.cn/Article/details/gpztgqiba.sHtML

split -l 1000 big.log part_
来源：http://wap.epnwcf.com/Article/details/gfvvhulol.sHtML

[R74] 批量重命名
来源：http://www.blog.sjlbkw.cn/Article/details/ggkpqoeca.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.bbcook.cn/Article/details/gsuxqioqx.sHtML

[R75] 导出环境变量
来源：http://www.share.epnwcf.com/Article/details/goteiecwc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.yfazqb.com/Article/details/gqnjcequz.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/gmkuiblak.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gqmghiiwj.sHtML

[R77] 读取用户输入
来源：http://www.share.yfazqb.com/Article/details/gdvsmvezs.sHtML

read -rp "请输入: " ans
来源：http://read.share.tarul.cn/Article/details/gqwevctoa.sHtML

[R78] 交互式菜单
来源：http://3g.vehdjk.com/Article/details/gxrhvwbxj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/gkthioxeg.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.bbcook.cn/Article/details/gajqgxiet.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gemlecjwm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/grnoaobfr.sHtML

time ./run.sh
来源：http://read.share.bbcook.cn/Article/details/gvmugpfio.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggboxdflg.sHtML

S. C / C++ 专题
来源：http://www.blog.bbcook.cn/Article/details/gwdtawoiv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gjhitsvlh.sHtML

[S01] C：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gfmnhthvf.sHtML

#include <stdio.h>
来源：http://www.share.epnwcf.com/Article/details/goopqrdzh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/gxbeduwzp.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fktsv.cn/Article/details/gqhdmdtyo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.bbcook.cn/Article/details/glwbdfwda.sHtML

[S03] C：读入整数
来源：http://www.blog.sjlbkw.cn/Article/details/gmolejzyc.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.bbcook.cn/Article/details/gbyrsywyf.sHtML

[S04] C：字符串复制
来源：http://mobile.bbcook.cn/Article/details/gmgigsyvz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.yfazqb.com/Article/details/gtdaxonzd.sHtML

[S05] C：字符串长度
来源：http://www.blog.bbcook.cn/Article/details/ghylfxruf.sHtML

strlen(s)
来源：http://www.share.yfazqb.com/Article/details/gmranjtoq.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/ggymtexcc.sHtML

strcmp(a, b) == 0
来源：http://wap.vehdjk.com/Article/details/gorenhevp.sHtML

[S07] C：数组遍历求和
来源：http://blog.yfazqb.com/Article/details/gpoxsbepe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fktsv.cn/Article/details/geqtwltyi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.epnwcf.com/Article/details/gzdmloudr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.vehdjk.com/Article/details/geufsvasf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.yfazqb.com/Article/details/gfholyxwt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.yfazqb.com/Article/details/gfgcdlfzv.sHtML

[S10] C：指针与解引用
来源：http://blog.fktsv.cn/Article/details/gqepeyarv.sHtML

int *p = &a;  *p = 5;
来源：http://wap.yfazqb.com/Article/details/ggrkjyrqs.sHtML

[S11] C：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gszjflvjn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.sjlbkw.cn/Article/details/geugzctjr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.yfazqb.com/Article/details/ggitwhqfy.sHtML

fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/guprdxynr.sHtML

[S12] C：写文件
来源：http://3g.sjlbkw.cn/Article/details/gbxhhzilk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gzyqqpmrb.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gradpcvyo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.vehdjk.com/Article/details/gpzgsbwld.sHtML

[S14] C：枚举
来源：http://3g.yfazqb.com/Article/details/gumkwbmxv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.yfazqb.com/Article/details/gkijhibtl.sHtML

[S15] C：类型转换
来源：http://3g.epnwcf.com/Article/details/gmfnxufzw.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/ghccofyvc.sHtML

[S16] C：位操作置位
来源：http://www.m.share.tarul.cn/Article/details/gviparpqy.sHtML

x |= (1 << 3);
来源：http://m.share.fktsv.cn/Article/details/gkahtpsqn.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gkvbqusih.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.sjlbkw.cn/Article/details/gprpygymx.sHtML

[S18] C：命令行参数
来源：http://wap.epnwcf.com/Article/details/gdimcbrln.sHtML

int main(int argc, char **argv)
来源：http://m.share.yfazqb.com/Article/details/gdsjotlde.sHtML

[S19] C：快速排序
来源：http://read.share.yfazqb.com/Article/details/gsubwlzyx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gauwlqvbz.sHtML

[S20] C：二分查找
来源：http://mobile.fktsv.cn/Article/details/gvtcfwihe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gbrzxrurv.sHtML

[S21] C：字符类别判断
来源：http://read.share.bbcook.cn/Article/details/gddthtacg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.vehdjk.com/Article/details/ghxawhgao.sHtML

[S22] C：字符串转数字
来源：http://blog.fktsv.cn/Article/details/gswjbqucm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.bbcook.cn/Article/details/gaohdukfx.sHtML

[S23] C：随机数
来源：http://read.share.vehdjk.com/Article/details/godtcecor.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.yfazqb.com/Article/details/gvzrsyqre.sHtML

[S24] C：获取本地时间
来源：http://blog.tarul.cn/Article/details/gimihdxfp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.bbcook.cn/Article/details/ggekbdsfs.sHtML

[S25] C：内存拷贝
来源：http://baike.epnwcf.com/Article/details/gxzpyldcy.sHtML

memcpy(dst, src, n);
来源：http://baike.bbcook.cn/Article/details/guipnwnpv.sHtML

[S26] C：内存清零
来源：http://blog.bbcook.cn/Article/details/grsxffhyy.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/ghidsnaba.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/gqglapwzm.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gavlysybp.sHtML

[S28] C：静态变量
来源：http://wap.tarul.cn/Article/details/gpaleirjf.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/gvskbfqao.sHtML

[S29] C：变参函数
来源：http://www.share.yfazqb.com/Article/details/getggkomr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.tarul.cn/Article/details/gcdsjfleb.sHtML

[S30] C：头文件保护
来源：http://read.share.yfazqb.com/Article/details/grbgmtovr.sHtML

#ifndef X_H
来源：http://m.share.tarul.cn/Article/details/ggwujgcir.sHtML

#define X_H
来源：http://mobile.epnwcf.com/Article/details/gfpqenkkh.sHtML

#endif
来源：http://read.share.epnwcf.com/Article/details/gkkdeetee.sHtML

[S31] C++：Hello World
来源：http://wap.tarul.cn/Article/details/gzmrguhlw.sHtML

#include <iostream>
来源：http://wap.yfazqb.com/Article/details/gjzcobhsj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fktsv.cn/Article/details/gqyfzbnoh.sHtML

[S32] C++：字符串
来源：http://www.share.vehdjk.com/Article/details/ggudgmssi.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.epnwcf.com/Article/details/gkfebluov.sHtML

[S33] C++：vector 增删
来源：http://read.share.fktsv.cn/Article/details/gstdeclan.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.tarul.cn/Article/details/gimsgtxun.sHtML

[S34] C++：遍历 vector
来源：http://m.share.yfazqb.com/Article/details/gzdultrkk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqashbzdg.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gqpnfqdlh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gitxsmtgt.sHtML

[S36] C++：unordered_map
来源：http://m.share.yfazqb.com/Article/details/gstjlyxan.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gwiwjknbr.sHtML

[S37] C++：set
来源：http://baike.tarul.cn/Article/details/gchxahgow.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.sjlbkw.cn/Article/details/gvcrsftvm.sHtML

[S38] C++：排序
来源：http://blog.yfazqb.com/Article/details/gmdmbyovc.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/ghzrewora.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fktsv.cn/Article/details/gghwgssxk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.bbcook.cn/Article/details/gwyuqegax.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/gppadrrmr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.yfazqb.com/Article/details/gcmgzowex.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fktsv.cn/Article/details/ghmgovsui.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/gcsnfgymw.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fktsv.cn/Article/details/gjbkqunvp.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.tarul.cn/Article/details/gxhbzderg.sHtML

[S43] C++：智能指针
来源：http://baike.tarul.cn/Article/details/gzcgrnptr.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.vehdjk.com/Article/details/gggnjastx.sHtML

[S44] C++：引用传参
来源：http://www.m.share.tarul.cn/Article/details/gqnpgxbfy.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/gpcdtsnxa.sHtML

[S45] C++：lambda
来源：http://www.share.bbcook.cn/Article/details/gekhhwwsp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gwigobios.sHtML

[S46] C++：函数模板
来源：http://read.share.epnwcf.com/Article/details/gvshoeoja.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.yfazqb.com/Article/details/gcrzviqic.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/grfbsoegb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fktsv.cn/Article/details/gemtkpetr.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gpejnmfhv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.bbcook.cn/Article/details/gcydfnccg.sHtML

while (std::getline(in, line)) { }
来源：http://wap.tarul.cn/Article/details/grczzvwdx.sHtML

[S49] C++：写文件
来源：http://3g.bbcook.cn/Article/details/gdatxoynp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.vehdjk.com/Article/details/ghpoopnww.sHtML

[S50] C++：格式化数字
来源：http://www.share.vehdjk.com/Article/details/ghbbfrtqc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.vehdjk.com/Article/details/grcofkymv.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/gjwacfvlt.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.epnwcf.com/Article/details/gografqtq.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.bbcook.cn/Article/details/gpzgpkbat.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.vehdjk.com/Article/details/gvujcmmkn.sHtML

[S53] C++：移动语义
来源：http://www.blog.sjlbkw.cn/Article/details/gbkweudbx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.sjlbkw.cn/Article/details/gqdhbcasn.sHtML

[S54] C++：异常处理
来源：http://m.share.vehdjk.com/Article/details/gyxjnttcy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.vehdjk.com/Article/details/gshsavfud.sHtML

[S55] C++：结构化绑定
来源：http://mobile.sjlbkw.cn/Article/details/gbjtwlcmd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.epnwcf.com/Article/details/gojsjwrol.sHtML

[S56] C++：optional
来源：http://m.share.bbcook.cn/Article/details/gsboilsyy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.sjlbkw.cn/Article/details/gymjyvnpo.sHtML

[S57] C++：编译期常量
来源：http://3g.fktsv.cn/Article/details/gzwcvangb.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/gsbqrnnks.sHtML

[S58] C++：命名空间
来源：http://mobile.bbcook.cn/Article/details/gizhttdgy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/gkbkixvme.sHtML

[S59] C++：静态断言
来源：http://read.share.sjlbkw.cn/Article/details/ghibvgtna.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.yfazqb.com/Article/details/guxdvggwe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/gqjeybvwm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.bbcook.cn/Article/details/gibegibah.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gzjcuuaow.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.epnwcf.com/Article/details/gkyytbotc.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/guqesyris.sHtML

[T01] Kotlin：Hello World
来源：http://3g.epnwcf.com/Article/details/galrdfetw.sHtML

println("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gbfgotqym.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gmmvqyqvz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.yfazqb.com/Article/details/gzmdsbcjx.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.tarul.cn/Article/details/gdmuxkgcs.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/gnmcefwnm.sHtML

[T04] Kotlin：空安全
来源：http://baike.vehdjk.com/Article/details/galezhjhd.sHtML

val n: String? = null;  n?.length
来源：http://baike.bbcook.cn/Article/details/gbatditxs.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.sjlbkw.cn/Article/details/gcashipva.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.bbcook.cn/Article/details/guvcoyldy.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/guwoqroxm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.bbcook.cn/Article/details/ghwzgyiux.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrtewels.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gcbgvhiti.sHtML

[T08] Kotlin：数据类
来源：http://wap.sjlbkw.cn/Article/details/ggddbsnes.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.sjlbkw.cn/Article/details/glwmxlgwt.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.vehdjk.com/Article/details/gcshvnloj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.bbcook.cn/Article/details/gcxjuyeqt.sHtML

[T10] Kotlin：默认参数
来源：http://baike.bbcook.cn/Article/details/glneucdxr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gjiopkoep.sHtML

[T11] Kotlin：协程
来源：http://baike.sjlbkw.cn/Article/details/gijiqtgzr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.tarul.cn/Article/details/grmwiwvtl.sHtML

[T12] Kotlin：解构声明
来源：http://baike.sjlbkw.cn/Article/details/ggwwqmlbj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gfcwxiidr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/gnlsumjow.sHtML

val m = mapOf("a" to 1)
来源：http://wap.vehdjk.com/Article/details/gnlrfspkb.sHtML

[T14] Kotlin：循环
来源：http://3g.sjlbkw.cn/Article/details/gbggmyjdr.sHtML

for (i in 1..10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gslihjjof.sHtML

[T15] Kotlin：接口
来源：http://read.share.yfazqb.com/Article/details/gtryadwit.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.sjlbkw.cn/Article/details/grzfiyffk.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gjzlqdkru.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gvdjnthhf.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fktsv.cn/Article/details/gxopmloip.sHtML

var a = 1;  let b = 2
来源：http://read.share.fktsv.cn/Article/details/glaawcrhb.sHtML

[T18] Swift：字符串插值
来源：http://3g.tarul.cn/Article/details/gcjjszrmu.sHtML

"值: \(b)"
来源：http://blog.tarul.cn/Article/details/giyjtwfeu.sHtML

[T19] Swift：可选绑定
来源：http://www.share.tarul.cn/Article/details/gxneuyypz.sHtML

if let n = opt { print(n) }
来源：http://mobile.vehdjk.com/Article/details/gfcoodanv.sHtML

[T20] Swift：数组操作
来源：http://mobile.vehdjk.com/Article/details/gbcurlive.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.epnwcf.com/Article/details/glaexmwuh.sHtML

[T21] Swift：遍历
来源：http://www.share.bbcook.cn/Article/details/gjjbguknz.sHtML

for x in a { print(x) }
来源：http://wap.sjlbkw.cn/Article/details/gwrmrnmjo.sHtML

[T22] Swift：字典
来源：http://read.share.fktsv.cn/Article/details/gzhttmkhw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.bbcook.cn/Article/details/gguuesfql.sHtML

[T23] Swift：函数
来源：http://blog.fktsv.cn/Article/details/gqehlgvoi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fktsv.cn/Article/details/gefxnzfme.sHtML

[T24] Swift：闭包
来源：http://m.share.sjlbkw.cn/Article/details/gwvtvdgih.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.bbcook.cn/Article/details/gsdbwzwbe.sHtML

[T25] Swift：结构体
来源：http://baike.yfazqb.com/Article/details/gyisphcok.sHtML

struct P { var x: Int }
来源：http://read.share.bbcook.cn/Article/details/gfswzzxju.sHtML

[T26] Swift：类与重写
来源：http://blog.vehdjk.com/Article/details/gibkbrals.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.yfazqb.com/Article/details/giaeulipa.sHtML

[T27] Swift：错误处理
来源：http://mobile.tarul.cn/Article/details/gishomofc.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fktsv.cn/Article/details/grwehirse.sHtML

[T28] Swift：枚举
来源：http://blog.sjlbkw.cn/Article/details/glhyeqgil.sHtML

enum Color { case red, green }
来源：http://m.share.sjlbkw.cn/Article/details/gzzoukuyd.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.epnwcf.com/Article/details/gokajlcyr.sHtML

guard let x = opt else { return }
来源：http://wap.fktsv.cn/Article/details/gpprkiftx.sHtML

[T30] Swift：协议
来源：http://mobile.fktsv.cn/Article/details/gitpsvlwr.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.yfazqb.com/Article/details/gcqdpfkgb.sHtML

[T31] Lua：Hello World
来源：http://3g.epnwcf.com/Article/details/gkqsfqfzz.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gxhdbrhgh.sHtML

[T32] Lua：局部变量
来源：http://blog.sjlbkw.cn/Article/details/gawlmhsuh.sHtML

local a = 1
来源：http://wap.fktsv.cn/Article/details/gyamuvxpx.sHtML


<!-- 参考信息 -->