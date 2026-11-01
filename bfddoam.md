代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fktsv.cn/Article/details/gdturpkge.sHtML

[R34] 退出时清理
来源：http://3g.vehdjk.com/Article/details/gprrkxkdu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gyawufcte.sHtML

[R35] 后台执行并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gyjugquvs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fktsv.cn/Article/details/gmbyltmzm.sHtML

[R36] 并发执行多个任务
来源：http://blog.epnwcf.com/Article/details/gwsaeerza.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.bbcook.cn/Article/details/ggifdtpyl.sHtML

[R37] 把输出赋给变量
来源：http://blog.tarul.cn/Article/details/gtyogchgf.sHtML

files=$(ls -1)
来源：http://mobile.vehdjk.com/Article/details/gavuiywoq.sHtML

[R38] 管道串联
来源：http://wap.yfazqb.com/Article/details/gicsnvouy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.vehdjk.com/Article/details/gujamtqan.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.sjlbkw.cn/Article/details/goglsukzi.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gnjsjnayb.sHtML

[R40] 追加写日志
来源：http://m.share.tarul.cn/Article/details/gitxqcdcl.sHtML

echo "log" >> out.log
来源：http://m.share.vehdjk.com/Article/details/grfcjofwk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.vehdjk.com/Article/details/gdrkmiarl.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gpxopiljk.sHtML

[R42] 输入重定向
来源：http://m.share.yfazqb.com/Article/details/gcdsjcavy.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/ghuhfhuco.sHtML

[R43] 按名字查找文件
来源：http://blog.vehdjk.com/Article/details/gvfydbjys.sHtML

find . -name "*.log" -type f
来源：http://blog.vehdjk.com/Article/details/gfyhyyvja.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.epnwcf.com/Article/details/gxwgjdnzl.sHtML

find . -mtime -7 -type f
来源：http://blog.yfazqb.com/Article/details/gcbqiqxii.sHtML

[R45] 批量删除
来源：http://blog.epnwcf.com/Article/details/gtgbhfpem.sHtML

find . -name "*.tmp" -delete
来源：http://wap.yfazqb.com/Article/details/gmtjudyse.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.bbcook.cn/Article/details/gwmmkkgkw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.sjlbkw.cn/Article/details/gdvbffgiq.sHtML

[R47] sed 单行替换
来源：http://www.share.bbcook.cn/Article/details/gbfecxqwd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gmnuoyera.sHtML

[R48] awk 取指定列
来源：http://wap.vehdjk.com/Article/details/gcelhxwtm.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fktsv.cn/Article/details/ggcbbxkhl.sHtML

[R49] awk 带条件
来源：http://3g.tarul.cn/Article/details/gejtouatv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.sjlbkw.cn/Article/details/gtyqvtpyh.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/ggmtnzzsz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gzbplknll.sHtML

[R51] 排序去重取前几
来源：http://www.blog.epnwcf.com/Article/details/gwniaqrri.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.vehdjk.com/Article/details/gjornlrws.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/ggdrqcybj.sHtML

wc -l a.txt
来源：http://www.blog.epnwcf.com/Article/details/gmfigiyyg.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.yfazqb.com/Article/details/gocevhhlw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.epnwcf.com/Article/details/grepyqsvr.sHtML

[R54] 比较两个文件
来源：http://www.share.yfazqb.com/Article/details/gojbsmjmg.sHtML

diff a.txt b.txt
来源：http://read.share.bbcook.cn/Article/details/gohjeicul.sHtML

[R55] 压缩与解压
来源：http://www.blog.epnwcf.com/Article/details/gtuamlynd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.epnwcf.com/Article/details/gofhderzq.sHtML

[R56] 远程拷贝
来源：http://www.blog.bbcook.cn/Article/details/geoidlsan.sHtML

scp file user@host:/path/
来源：http://blog.fktsv.cn/Article/details/gtdqqwnfw.sHtML

[R57] 远程执行命令
来源：http://wap.bbcook.cn/Article/details/gptsdnuwa.sHtML

ssh user@host 'uptime'
来源：http://www.blog.bbcook.cn/Article/details/gjxviuyku.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/ggymcuecp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.sjlbkw.cn/Article/details/gbefewyhe.sHtML

[R59] 发 POST JSON
来源：http://www.share.fktsv.cn/Article/details/gnrtasmcx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fktsv.cn/Article/details/gxabznbzm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gdjashngk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fktsv.cn/Article/details/gyzesujoe.sHtML

[R61] 磁盘占用
来源：http://www.blog.sjlbkw.cn/Article/details/ghkvnzzrk.sHtML

df -h;  du -sh *
来源：http://3g.tarul.cn/Article/details/gtrmwhupl.sHtML

[R62] 找最占空间的文件
来源：http://3g.tarul.cn/Article/details/goeaqrgky.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.vehdjk.com/Article/details/giluymzla.sHtML

[R63] 内存与进程
来源：http://baike.fktsv.cn/Article/details/gvpxeogwd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.sjlbkw.cn/Article/details/gxoktdsvd.sHtML

[R64] 结束进程
来源：http://www.blog.vehdjk.com/Article/details/gjehrdwsk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.sjlbkw.cn/Article/details/gnablingm.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fktsv.cn/Article/details/gjzlzbrij.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.vehdjk.com/Article/details/gymftixiu.sHtML

[R66] 定时任务
来源：http://www.m.share.bbcook.cn/Article/details/gyhtktuvn.sHtML

crontab -e;  crontab -l
来源：http://wap.fktsv.cn/Article/details/gjvjercgg.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.tarul.cn/Article/details/gnydjcqcl.sHtML

openssl rand -hex 16
来源：http://m.share.yfazqb.com/Article/details/glvztuffh.sHtML

[R68] 计算文件校验值
来源：http://www.share.bbcook.cn/Article/details/gnczooevg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcryssyr.sHtML

[R69] 生成随机密码
来源：http://wap.bbcook.cn/Article/details/gmgxdkjpc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fktsv.cn/Article/details/gymukfcfu.sHtML

[R70] 时间戳与互转
来源：http://blog.vehdjk.com/Article/details/gfvnhygmg.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/gucnjjydp.sHtML

[R71] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/gnvlyufdc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.bbcook.cn/Article/details/gwsrhxgwi.sHtML

[R72] 等待端口就绪
来源：http://blog.tarul.cn/Article/details/glrupqcef.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gmdpqygia.sHtML

[R73] 分割大日志
来源：http://blog.vehdjk.com/Article/details/gebxiblft.sHtML

split -l 1000 big.log part_
来源：http://blog.fktsv.cn/Article/details/gdrwexhau.sHtML

[R74] 批量重命名
来源：http://www.m.share.sjlbkw.cn/Article/details/gcadcqvkg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.vehdjk.com/Article/details/ggjtsbdxc.sHtML

[R75] 导出环境变量
来源：http://www.share.epnwcf.com/Article/details/gjozdnnxh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.yfazqb.com/Article/details/gwruufaih.sHtML

[R76] 使用临时文件
来源：http://www.blog.fktsv.cn/Article/details/gcxzfnvwi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/gvmpiqumd.sHtML

[R77] 读取用户输入
来源：http://www.share.vehdjk.com/Article/details/ggpdsblrw.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.tarul.cn/Article/details/gopapamoi.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fktsv.cn/Article/details/gjrkijhue.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.yfazqb.com/Article/details/gkrrvecpb.sHtML

[R79] 解析命令行选项
来源：http://m.share.fktsv.cn/Article/details/gcqyxbojf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.sjlbkw.cn/Article/details/ggvkindft.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fktsv.cn/Article/details/gaahjhltr.sHtML

time ./run.sh
来源：http://www.blog.vehdjk.com/Article/details/gyfbllvga.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gwtonmmin.sHtML

S. C / C++ 专题
来源：http://blog.tarul.cn/Article/details/gbecmkqhp.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gopvtamih.sHtML

[S01] C：Hello World
来源：http://wap.bbcook.cn/Article/details/genjajcge.sHtML

#include <stdio.h>
来源：http://www.share.sjlbkw.cn/Article/details/gkhpoyuax.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.sjlbkw.cn/Article/details/gzckigphj.sHtML

[S02] C：变量与格式化输出
来源：http://baike.bbcook.cn/Article/details/gtoqldsdr.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.bbcook.cn/Article/details/ghdahgzgg.sHtML

[S03] C：读入整数
来源：http://www.share.sjlbkw.cn/Article/details/ggfsjlzor.sHtML

int x; scanf("%d", &x);
来源：http://wap.fktsv.cn/Article/details/gpuesettf.sHtML

[S04] C：字符串复制
来源：http://m.share.tarul.cn/Article/details/ghwomfkxj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gqlmajadw.sHtML

[S05] C：字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gjpuaxxao.sHtML

strlen(s)
来源：http://wap.yfazqb.com/Article/details/gndbavxlk.sHtML

[S06] C：字符串比较
来源：http://mobile.fktsv.cn/Article/details/gseakkwon.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/glyodgmuh.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.yfazqb.com/Article/details/ghlhpydas.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.epnwcf.com/Article/details/gmqmeetzx.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.epnwcf.com/Article/details/ghqulldqw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fktsv.cn/Article/details/gfhpenzjk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.sjlbkw.cn/Article/details/glrscuple.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/gxchiycaa.sHtML

[S10] C：指针与解引用
来源：http://mobile.tarul.cn/Article/details/gixdtksue.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/ghdgabakx.sHtML

[S11] C：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gcdrdowbr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.epnwcf.com/Article/details/gxpdlgshn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/gezejgpkt.sHtML

fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/ggtatruwo.sHtML

[S12] C：写文件
来源：http://www.share.fktsv.cn/Article/details/glnaewzxu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/gaeiuhdbn.sHtML

[S13] C：宏定义
来源：http://wap.sjlbkw.cn/Article/details/gzkgttxjm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.bbcook.cn/Article/details/gbfzakkvl.sHtML

[S14] C：枚举
来源：http://blog.epnwcf.com/Article/details/gjzvntwaz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.yfazqb.com/Article/details/gadsfvvbl.sHtML

[S15] C：类型转换
来源：http://baike.tarul.cn/Article/details/gkpuxufjr.sHtML

(double) a / b
来源：http://mobile.fktsv.cn/Article/details/gusbxnnvs.sHtML

[S16] C：位操作置位
来源：http://3g.bbcook.cn/Article/details/gtgjtfuej.sHtML

x |= (1 << 3);
来源：http://baike.yfazqb.com/Article/details/gwyfsyfpz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.yfazqb.com/Article/details/gbpebsfbp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.vehdjk.com/Article/details/gkooiypsr.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/ggzsosckm.sHtML

int main(int argc, char **argv)
来源：http://m.share.vehdjk.com/Article/details/gjmzjmais.sHtML

[S19] C：快速排序
来源：http://wap.epnwcf.com/Article/details/gkvzriage.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gimplcffq.sHtML

[S20] C：二分查找
来源：http://read.share.bbcook.cn/Article/details/gpuhzoqnq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gmqjfosyd.sHtML

[S21] C：字符类别判断
来源：http://www.share.yfazqb.com/Article/details/gupydxekv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fktsv.cn/Article/details/gyekukpwi.sHtML

[S22] C：字符串转数字
来源：http://m.share.epnwcf.com/Article/details/gqkaflydb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.bbcook.cn/Article/details/gnvoxoeuj.sHtML

[S23] C：随机数
来源：http://blog.epnwcf.com/Article/details/gksaexzzc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.bbcook.cn/Article/details/gzoxpnmoo.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.tarul.cn/Article/details/gxhljidzm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.sjlbkw.cn/Article/details/gmvfwcggu.sHtML

[S25] C：内存拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gickfjprm.sHtML

memcpy(dst, src, n);
来源：http://blog.vehdjk.com/Article/details/gijrajxzt.sHtML

[S26] C：内存清零
来源：http://mobile.fktsv.cn/Article/details/gmpkijhul.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/gletgxwlx.sHtML

[S27] C：定义常量
来源：http://3g.vehdjk.com/Article/details/grsrlflih.sHtML

const double PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gwmrvlchn.sHtML

[S28] C：静态变量
来源：http://www.m.share.epnwcf.com/Article/details/gxgblstss.sHtML

static int counter = 0;
来源：http://mobile.sjlbkw.cn/Article/details/guxrjrign.sHtML

[S29] C：变参函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqxpghvx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.vehdjk.com/Article/details/gslppugma.sHtML

[S30] C：头文件保护
来源：http://m.share.vehdjk.com/Article/details/gwqxjzgba.sHtML

#ifndef X_H
来源：http://wap.vehdjk.com/Article/details/gluhbxbax.sHtML

#define X_H
来源：http://mobile.bbcook.cn/Article/details/gxxotfazw.sHtML

#endif
来源：http://www.m.share.vehdjk.com/Article/details/gdvngnhkf.sHtML

[S31] C++：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gedggogll.sHtML

#include <iostream>
来源：http://www.share.epnwcf.com/Article/details/gkoxsxpoq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/gnyzsothf.sHtML

[S32] C++：字符串
来源：http://blog.sjlbkw.cn/Article/details/gwrodpzpg.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.tarul.cn/Article/details/gsyoftnup.sHtML

[S33] C++：vector 增删
来源：http://wap.bbcook.cn/Article/details/gblqqijga.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.yfazqb.com/Article/details/gzubzgrry.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/gnarkqebp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.vehdjk.com/Article/details/gyubyhgku.sHtML

[S35] C++：map
来源：http://www.blog.bbcook.cn/Article/details/gbjxaukjl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gfiufhpiz.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fktsv.cn/Article/details/gvypvddsj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gdhswbfmx.sHtML

[S37] C++：set
来源：http://www.blog.bbcook.cn/Article/details/glssmmdao.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gwoxwtkyi.sHtML

[S38] C++：排序
来源：http://wap.vehdjk.com/Article/details/gmeziiccf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gjveaucsu.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.bbcook.cn/Article/details/glpoppyrq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.sjlbkw.cn/Article/details/gypxgeldc.sHtML

[S40] C++：查找元素
来源：http://read.share.yfazqb.com/Article/details/gfhfgeqjj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.yfazqb.com/Article/details/gxbbzatma.sHtML

[S41] C++：类与构造函数
来源：http://mobile.yfazqb.com/Article/details/gbiyymgne.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.tarul.cn/Article/details/gydyokkut.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/gqcxohrgp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.epnwcf.com/Article/details/gqqixgcud.sHtML

[S43] C++：智能指针
来源：http://baike.tarul.cn/Article/details/gjkjsnnca.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.bbcook.cn/Article/details/gqsfklzsc.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fktsv.cn/Article/details/gevonrojd.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/gtokuvsue.sHtML

[S45] C++：lambda
来源：http://wap.fktsv.cn/Article/details/gkqafsxwz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.yfazqb.com/Article/details/gzhboknci.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/giaceypov.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fktsv.cn/Article/details/gokxzvgdr.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/gqcxlzufi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/gtvncohlu.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/ghdllneye.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fktsv.cn/Article/details/gdcivgdop.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.bbcook.cn/Article/details/gcodrznmk.sHtML

[S49] C++：写文件
来源：http://m.share.vehdjk.com/Article/details/gjogswozj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.sjlbkw.cn/Article/details/gbdmwpsxp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.bbcook.cn/Article/details/gclpwvqqu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gfcgkvnkl.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/gxtaqrmgj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.yfazqb.com/Article/details/gepmquyse.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.tarul.cn/Article/details/gdtqtdopk.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/gtdkdzjea.sHtML

[S53] C++：移动语义
来源：http://read.share.tarul.cn/Article/details/ggvclugic.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/ghupcgswa.sHtML

[S54] C++：异常处理
来源：http://mobile.epnwcf.com/Article/details/gppzuvbst.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.vehdjk.com/Article/details/gwraxbsex.sHtML

[S55] C++：结构化绑定
来源：http://blog.tarul.cn/Article/details/gfpmrxcdw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.bbcook.cn/Article/details/gzmijlobv.sHtML

[S56] C++：optional
来源：http://m.share.epnwcf.com/Article/details/ghqrfrqky.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.sjlbkw.cn/Article/details/gkehqqbml.sHtML

[S57] C++：编译期常量
来源：http://www.share.sjlbkw.cn/Article/details/gouxmzdha.sHtML

constexpr int N = 10;
来源：http://www.share.bbcook.cn/Article/details/guxsscywk.sHtML

[S58] C++：命名空间
来源：http://3g.vehdjk.com/Article/details/gphlzcqev.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/gqsmwzbrw.sHtML

[S59] C++：静态断言
来源：http://read.share.fktsv.cn/Article/details/guhiyhvpc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.bbcook.cn/Article/details/gxlzmzoxq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.epnwcf.com/Article/details/gomdtzjaf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gnztkggpw.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gxssrjnkl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gpeusydxx.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gidlulqhe.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gadivtdbl.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gbxdumook.sHtML

[T02] Kotlin：变量
来源：http://read.share.fktsv.cn/Article/details/gvjkzhtzy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.epnwcf.com/Article/details/grkvnahex.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fktsv.cn/Article/details/gscxgasct.sHtML

"值: $b"
来源：http://3g.fktsv.cn/Article/details/gpucehbng.sHtML

[T04] Kotlin：空安全
来源：http://m.share.vehdjk.com/Article/details/gonxuexgf.sHtML

val n: String? = null;  n?.length
来源：http://3g.sjlbkw.cn/Article/details/gugmssuca.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.epnwcf.com/Article/details/gfyegvpse.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.tarul.cn/Article/details/gzhutypyc.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.yfazqb.com/Article/details/gcsyxzqzu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.tarul.cn/Article/details/geqbnbarb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.tarul.cn/Article/details/gsaqqtpnu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.yfazqb.com/Article/details/gnthsidpt.sHtML

[T08] Kotlin：数据类
来源：http://blog.yfazqb.com/Article/details/gglbgcwot.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/glapgrgww.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.bbcook.cn/Article/details/gplqfgcja.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.yfazqb.com/Article/details/gtcvinjsu.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.vehdjk.com/Article/details/gbdbiiydy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.yfazqb.com/Article/details/ghoimqifi.sHtML

[T11] Kotlin：协程
来源：http://3g.epnwcf.com/Article/details/gfoizcocn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fktsv.cn/Article/details/gxbcmorzk.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/gqfqwmosk.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.bbcook.cn/Article/details/gggggulzf.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.vehdjk.com/Article/details/gxfrotdab.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.yfazqb.com/Article/details/gfvesgkwd.sHtML

[T14] Kotlin：循环
来源：http://www.blog.tarul.cn/Article/details/gcqnqhyao.sHtML

for (i in 1..10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gxitnadns.sHtML

[T15] Kotlin：接口
来源：http://wap.vehdjk.com/Article/details/golblreiu.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fktsv.cn/Article/details/geyxxfmpa.sHtML

[T16] Swift：Hello World
来源：http://read.share.vehdjk.com/Article/details/gnanlpjmb.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gwwlynguq.sHtML

[T17] Swift：变量与常量
来源：http://3g.vehdjk.com/Article/details/gcejodnoq.sHtML

var a = 1;  let b = 2
来源：http://read.share.vehdjk.com/Article/details/gfwntdhvr.sHtML

[T18] Swift：字符串插值
来源：http://3g.vehdjk.com/Article/details/gpxkrnyrp.sHtML

"值: \(b)"
来源：http://www.share.vehdjk.com/Article/details/gfxldcvky.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/gfnjmbpmx.sHtML

if let n = opt { print(n) }
来源：http://read.share.sjlbkw.cn/Article/details/gzyyxgdsj.sHtML

[T20] Swift：数组操作
来源：http://baike.sjlbkw.cn/Article/details/gqoihppun.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/gvkedlytq.sHtML

[T21] Swift：遍历
来源：http://read.share.sjlbkw.cn/Article/details/glsewqbhg.sHtML

for x in a { print(x) }
来源：http://read.share.epnwcf.com/Article/details/ggdsouhuh.sHtML

[T22] Swift：字典
来源：http://www.share.vehdjk.com/Article/details/gghnjuart.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.tarul.cn/Article/details/gesqljwxa.sHtML

[T23] Swift：函数
来源：http://baike.vehdjk.com/Article/details/gurcdcail.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.bbcook.cn/Article/details/gglxkjmmn.sHtML

[T24] Swift：闭包
来源：http://blog.yfazqb.com/Article/details/gaauwdicq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gdmxvorpk.sHtML

[T25] Swift：结构体
来源：http://baike.yfazqb.com/Article/details/gzrtosifm.sHtML

struct P { var x: Int }
来源：http://3g.epnwcf.com/Article/details/gpurisipk.sHtML

[T26] Swift：类与重写
来源：http://blog.tarul.cn/Article/details/gkdibvtcj.sHtML

class A: Base { override func f() {} }
来源：http://wap.tarul.cn/Article/details/gwgturjzt.sHtML

[T27] Swift：错误处理
来源：http://www.blog.tarul.cn/Article/details/gmsaafqez.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.yfazqb.com/Article/details/gzkryxquy.sHtML

[T28] Swift：枚举
来源：http://blog.tarul.cn/Article/details/gdlvcnvpb.sHtML

enum Color { case red, green }
来源：http://3g.fktsv.cn/Article/details/grtdpyvia.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.epnwcf.com/Article/details/gvqzmplku.sHtML

guard let x = opt else { return }
来源：http://www.share.bbcook.cn/Article/details/gqmxnaslw.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/gznuizwmt.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fktsv.cn/Article/details/gmxxpttis.sHtML

[T31] Lua：Hello World
来源：http://read.share.tarul.cn/Article/details/gmijhnyzk.sHtML

print("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gcgxscsve.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.bbcook.cn/Article/details/gambghqqe.sHtML

local a = 1
来源：http://blog.fktsv.cn/Article/details/gckpbwhzj.sHtML

[T33] Lua：表（数组）
来源：http://mobile.sjlbkw.cn/Article/details/gfitmtrjc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.bbcook.cn/Article/details/gkwgkslkb.sHtML

[T34] Lua：遍历表
来源：http://read.share.yfazqb.com/Article/details/gisfacvjl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.vehdjk.com/Article/details/gdwwgqaih.sHtML

[T35] Lua：字典表
来源：http://3g.vehdjk.com/Article/details/ghhmqmpmo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fktsv.cn/Article/details/gkvhipuqe.sHtML

[T36] Lua：函数
来源：http://www.blog.vehdjk.com/Article/details/gyihccbsd.sHtML

function add(a, b) return a + b end
来源：http://wap.yfazqb.com/Article/details/gwhprsxrx.sHtML


<!-- 参考信息 -->