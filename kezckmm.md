代发 wailian999

find . -name "*.log" -type f
来源：http://www.share.tarul.cn/Article/details/gqpwqjjut.sHtML

[R44] 按修改时间查找
来源：http://3g.sjlbkw.cn/Article/details/gmxfoufla.sHtML

find . -mtime -7 -type f
来源：http://baike.bbcook.cn/Article/details/gdjlcnsey.sHtML

[R45] 批量删除
来源：http://baike.tarul.cn/Article/details/grvdwighd.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gffzufztx.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fktsv.cn/Article/details/gxedbnvpf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.bbcook.cn/Article/details/gjrwnstnz.sHtML

[R47] sed 单行替换
来源：http://baike.vehdjk.com/Article/details/gpzesulmr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.vehdjk.com/Article/details/gsnuggtcm.sHtML

[R48] awk 取指定列
来源：http://www.m.share.vehdjk.com/Article/details/gyrjqlxfn.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gqncomwmd.sHtML

[R49] awk 带条件
来源：http://read.share.epnwcf.com/Article/details/gvwiochwh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.tarul.cn/Article/details/glrrwdfod.sHtML

[R50] awk 求和
来源：http://m.share.fktsv.cn/Article/details/gmnhpwqrm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.tarul.cn/Article/details/gtoauslod.sHtML

[R51] 排序去重取前几
来源：http://baike.bbcook.cn/Article/details/gxukkgadv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.tarul.cn/Article/details/gwrtrvkvo.sHtML

[R52] 统计行数
来源：http://read.share.sjlbkw.cn/Article/details/gzjwygspc.sHtML

wc -l a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gfzgdcetu.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.epnwcf.com/Article/details/gmfafxmar.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.epnwcf.com/Article/details/gdkeumptr.sHtML

[R54] 比较两个文件
来源：http://www.share.epnwcf.com/Article/details/gdbkcijnp.sHtML

diff a.txt b.txt
来源：http://wap.vehdjk.com/Article/details/guhamlxkz.sHtML

[R55] 压缩与解压
来源：http://wap.yfazqb.com/Article/details/gdjkhiirz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/ggsxlblnb.sHtML

[R56] 远程拷贝
来源：http://3g.fktsv.cn/Article/details/gkjdnuwoe.sHtML

scp file user@host:/path/
来源：http://www.m.share.bbcook.cn/Article/details/gnrkuqijq.sHtML

[R57] 远程执行命令
来源：http://mobile.epnwcf.com/Article/details/gqnqyhgcy.sHtML

ssh user@host 'uptime'
来源：http://www.share.tarul.cn/Article/details/gppyejols.sHtML

[R58] 下载文件
来源：http://blog.yfazqb.com/Article/details/gfruqtixp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.vehdjk.com/Article/details/gbfjrkksw.sHtML

[R59] 发 POST JSON
来源：http://m.share.yfazqb.com/Article/details/ghpvarjva.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/gxpvqhbag.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gtmdjxexw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.sjlbkw.cn/Article/details/guqqujkpd.sHtML

[R61] 磁盘占用
来源：http://m.share.epnwcf.com/Article/details/gllblnypd.sHtML

df -h;  du -sh *
来源：http://3g.epnwcf.com/Article/details/gzfdxmqrf.sHtML

[R62] 找最占空间的文件
来源：http://www.share.sjlbkw.cn/Article/details/gppoyrpfv.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.tarul.cn/Article/details/gfznurups.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gtpyhzkmh.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.vehdjk.com/Article/details/gcenlorgx.sHtML

[R64] 结束进程
来源：http://3g.fktsv.cn/Article/details/gjqubsthy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.sjlbkw.cn/Article/details/gmrqjgork.sHtML

[R65] 查看端口占用
来源：http://www.m.share.yfazqb.com/Article/details/gsezlnhwy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.tarul.cn/Article/details/gtsjrhgka.sHtML

[R66] 定时任务
来源：http://www.m.share.bbcook.cn/Article/details/gurelqvyb.sHtML

crontab -e;  crontab -l
来源：http://www.share.bbcook.cn/Article/details/giirrubkz.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.bbcook.cn/Article/details/gfsxdtyhi.sHtML

openssl rand -hex 16
来源：http://mobile.vehdjk.com/Article/details/gudkhssds.sHtML

[R68] 计算文件校验值
来源：http://m.share.fktsv.cn/Article/details/gujkfudmq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fktsv.cn/Article/details/ggxwkdoba.sHtML

[R69] 生成随机密码
来源：http://read.share.bbcook.cn/Article/details/gmfjmbpah.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.sjlbkw.cn/Article/details/gmiprxtyp.sHtML

[R70] 时间戳与互转
来源：http://wap.bbcook.cn/Article/details/gjeddjlgw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.vehdjk.com/Article/details/gsekhxkns.sHtML

[R71] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gktwqdbpp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.vehdjk.com/Article/details/gaslihxbd.sHtML

[R72] 等待端口就绪
来源：http://wap.vehdjk.com/Article/details/gymltijou.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gaqbwmhjb.sHtML

[R73] 分割大日志
来源：http://www.share.bbcook.cn/Article/details/gqimklaho.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.yfazqb.com/Article/details/gzdytcank.sHtML

[R74] 批量重命名
来源：http://blog.fktsv.cn/Article/details/gefeekath.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fktsv.cn/Article/details/gqgwbipmc.sHtML

[R75] 导出环境变量
来源：http://3g.bbcook.cn/Article/details/gfnmsnihw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/geukkvert.sHtML

[R76] 使用临时文件
来源：http://m.share.sjlbkw.cn/Article/details/glodaaxar.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/grjbmwwuc.sHtML

[R77] 读取用户输入
来源：http://www.share.epnwcf.com/Article/details/gfwuzbmkk.sHtML

read -rp "请输入: " ans
来源：http://www.share.bbcook.cn/Article/details/gwtzqevno.sHtML

[R78] 交互式菜单
来源：http://baike.vehdjk.com/Article/details/gomrquhah.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fktsv.cn/Article/details/gdtxzndpi.sHtML

[R79] 解析命令行选项
来源：http://www.share.epnwcf.com/Article/details/ggqskulix.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/gqkdrxpax.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.tarul.cn/Article/details/ghswbtmjm.sHtML

time ./run.sh
来源：http://blog.bbcook.cn/Article/details/gtcrobutf.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gosecyzmj.sHtML

S. C / C++ 专题
来源：http://www.blog.bbcook.cn/Article/details/ghxayshok.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gjdjqnijx.sHtML

[S01] C：Hello World
来源：http://3g.epnwcf.com/Article/details/gqvntipiq.sHtML

#include <stdio.h>
来源：http://blog.fktsv.cn/Article/details/gwkttsmpy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.epnwcf.com/Article/details/gkvbjtcgp.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.yfazqb.com/Article/details/gzjsmhfdc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.bbcook.cn/Article/details/ggepuytfi.sHtML

[S03] C：读入整数
来源：http://wap.yfazqb.com/Article/details/gsvyyhzyu.sHtML

int x; scanf("%d", &x);
来源：http://www.share.yfazqb.com/Article/details/getcaudle.sHtML

[S04] C：字符串复制
来源：http://mobile.tarul.cn/Article/details/gpddsqbct.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.bbcook.cn/Article/details/gbznkqjuf.sHtML

[S05] C：字符串长度
来源：http://3g.vehdjk.com/Article/details/gwhsvsdxx.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/gzvqxmdvk.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/grksoiugw.sHtML

strcmp(a, b) == 0
来源：http://m.share.tarul.cn/Article/details/gygmgqrti.sHtML

[S07] C：数组遍历求和
来源：http://blog.bbcook.cn/Article/details/glpfqsiem.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gqautxllf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.epnwcf.com/Article/details/gdlmimvfu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.epnwcf.com/Article/details/gzveifqmx.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.epnwcf.com/Article/details/gmkjevhte.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.epnwcf.com/Article/details/gmrgzypkg.sHtML

[S10] C：指针与解引用
来源：http://www.share.vehdjk.com/Article/details/gwyvcupql.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.bbcook.cn/Article/details/gontwhtah.sHtML

[S11] C：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gozcnwngi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.epnwcf.com/Article/details/gayfrdgbm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.tarul.cn/Article/details/gcyofkryn.sHtML

fclose(f);
来源：http://www.blog.tarul.cn/Article/details/gxwmhvnxv.sHtML

[S12] C：写文件
来源：http://www.m.share.tarul.cn/Article/details/grptceilq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.tarul.cn/Article/details/ghefkddcz.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/grnxrlofb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.epnwcf.com/Article/details/goootnmzq.sHtML

[S14] C：枚举
来源：http://3g.epnwcf.com/Article/details/gfpivzkto.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/gfzuwpyio.sHtML

[S15] C：类型转换
来源：http://3g.vehdjk.com/Article/details/gofyjxjmi.sHtML

(double) a / b
来源：http://blog.epnwcf.com/Article/details/gwnmbqefs.sHtML

[S16] C：位操作置位
来源：http://read.share.bbcook.cn/Article/details/gohfordxk.sHtML

x |= (1 << 3);
来源：http://m.share.tarul.cn/Article/details/gtdclfvjc.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gllrtiikg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.bbcook.cn/Article/details/gvexzoixw.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gvtiuuypv.sHtML

int main(int argc, char **argv)
来源：http://mobile.bbcook.cn/Article/details/ghdxaxfjg.sHtML

[S19] C：快速排序
来源：http://wap.bbcook.cn/Article/details/gunaovjqs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gnmkbjtzo.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/gqxnojnma.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/giehnomvb.sHtML

[S21] C：字符类别判断
来源：http://mobile.yfazqb.com/Article/details/ggpsioryz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.vehdjk.com/Article/details/gphoqtddu.sHtML

[S22] C：字符串转数字
来源：http://www.share.bbcook.cn/Article/details/gjudiupvm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.tarul.cn/Article/details/gukqdjhac.sHtML

[S23] C：随机数
来源：http://www.m.share.yfazqb.com/Article/details/ggjuxbsni.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.epnwcf.com/Article/details/geejvinne.sHtML

[S24] C：获取本地时间
来源：http://www.blog.yfazqb.com/Article/details/grjmrytkn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.bbcook.cn/Article/details/glmauoypg.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.epnwcf.com/Article/details/ghrqchfil.sHtML

memcpy(dst, src, n);
来源：http://baike.epnwcf.com/Article/details/geotozdpu.sHtML

[S26] C：内存清零
来源：http://www.blog.fktsv.cn/Article/details/gkzcrjcxp.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/grqljzxpb.sHtML

[S27] C：定义常量
来源：http://www.share.tarul.cn/Article/details/gwllgkhvt.sHtML

const double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/ghreinphr.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/gzanxrdjj.sHtML

static int counter = 0;
来源：http://m.share.bbcook.cn/Article/details/gequtusiz.sHtML

[S29] C：变参函数
来源：http://m.share.fktsv.cn/Article/details/gebcyqhhb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.sjlbkw.cn/Article/details/godtrmzwv.sHtML

[S30] C：头文件保护
来源：http://www.share.fktsv.cn/Article/details/gzwizjuvj.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/gsbyejpkz.sHtML

#define X_H
来源：http://blog.tarul.cn/Article/details/gntrwrrmj.sHtML

#endif
来源：http://read.share.sjlbkw.cn/Article/details/gsvstlfvm.sHtML

[S31] C++：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gseczispr.sHtML

#include <iostream>
来源：http://m.share.bbcook.cn/Article/details/gncbyqyzj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fktsv.cn/Article/details/gsrhiujap.sHtML

[S32] C++：字符串
来源：http://www.share.fktsv.cn/Article/details/guqizgqak.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fktsv.cn/Article/details/giuraqgbv.sHtML

[S33] C++：vector 增删
来源：http://3g.yfazqb.com/Article/details/grxjqqzwd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.epnwcf.com/Article/details/gzdmnxtub.sHtML

[S34] C++：遍历 vector
来源：http://3g.yfazqb.com/Article/details/gblbgoznj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fktsv.cn/Article/details/gbtwvnprv.sHtML

[S35] C++：map
来源：http://www.m.share.bbcook.cn/Article/details/gpajtwroh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gxrflqjht.sHtML

[S36] C++：unordered_map
来源：http://3g.yfazqb.com/Article/details/gtemzptyq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gkcmfphgi.sHtML

[S37] C++：set
来源：http://wap.tarul.cn/Article/details/godzpoyow.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/gmzfoblte.sHtML

[S38] C++：排序
来源：http://baike.epnwcf.com/Article/details/gcpsnuqvz.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.tarul.cn/Article/details/gunfhiysi.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/gcupqgycc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.vehdjk.com/Article/details/grodxbegj.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/gxqncdfbn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.vehdjk.com/Article/details/gkjubbpvm.sHtML

[S41] C++：类与构造函数
来源：http://baike.epnwcf.com/Article/details/gftrnshey.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.yfazqb.com/Article/details/ghoepolok.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gmzwidmgw.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.vehdjk.com/Article/details/gnpojvngl.sHtML

[S43] C++：智能指针
来源：http://mobile.fktsv.cn/Article/details/gpszsjdun.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.tarul.cn/Article/details/gbukegplq.sHtML

[S44] C++：引用传参
来源：http://www.blog.tarul.cn/Article/details/gprfrdeya.sHtML

void inc(int &x) { ++x; }
来源：http://baike.tarul.cn/Article/details/gppkryfwk.sHtML

[S45] C++：lambda
来源：http://wap.sjlbkw.cn/Article/details/gazcjxwst.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.epnwcf.com/Article/details/gzhqbxrgb.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gbytxuujb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.tarul.cn/Article/details/gtsvtujjd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fktsv.cn/Article/details/ggqfsyjce.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/gdeaonldn.sHtML

[S48] C++：逐行读文件
来源：http://3g.yfazqb.com/Article/details/giddezfvu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.sjlbkw.cn/Article/details/gsjqjawmx.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.vehdjk.com/Article/details/givjwuutz.sHtML

[S49] C++：写文件
来源：http://m.share.yfazqb.com/Article/details/ghbqjekez.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.yfazqb.com/Article/details/gvbokhigg.sHtML

[S50] C++：格式化数字
来源：http://baike.epnwcf.com/Article/details/gsumswtgt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gyxrjocvd.sHtML

[S51] C++：显式类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gxempfxsx.sHtML

static_cast<double>(a) / b
来源：http://wap.epnwcf.com/Article/details/geieuxuts.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.vehdjk.com/Article/details/glhqffmbu.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.bbcook.cn/Article/details/gkdibxtsu.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/gqteaqdro.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fktsv.cn/Article/details/gtlykpnmw.sHtML

[S54] C++：异常处理
来源：http://www.share.vehdjk.com/Article/details/gsxcpndxb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.bbcook.cn/Article/details/gehrmgbod.sHtML

[S55] C++：结构化绑定
来源：http://m.share.epnwcf.com/Article/details/goqzixzvx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.bbcook.cn/Article/details/gsjqtfqdu.sHtML

[S56] C++：optional
来源：http://www.blog.tarul.cn/Article/details/gorxfmslv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.bbcook.cn/Article/details/gsqtbtnct.sHtML

[S57] C++：编译期常量
来源：http://m.share.tarul.cn/Article/details/gsnmukdyg.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gvjzqlamy.sHtML

[S58] C++：命名空间
来源：http://www.blog.yfazqb.com/Article/details/ghhigpjoy.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.epnwcf.com/Article/details/gcykstaah.sHtML

[S59] C++：静态断言
来源：http://3g.tarul.cn/Article/details/gxizrempm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.yfazqb.com/Article/details/gnovtghus.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.sjlbkw.cn/Article/details/ggdaeemxx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.sjlbkw.cn/Article/details/givsofgdj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gizymyauy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gsyuqbgpz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grdowvafk.sHtML

[T01] Kotlin：Hello World
来源：http://wap.bbcook.cn/Article/details/gtgccepcz.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gkcggwgyc.sHtML

[T02] Kotlin：变量
来源：http://baike.sjlbkw.cn/Article/details/ghwsqsizm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fktsv.cn/Article/details/gkpsqwovo.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.yfazqb.com/Article/details/gubgioozk.sHtML

"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gvrkwpxru.sHtML

[T04] Kotlin：空安全
来源：http://wap.tarul.cn/Article/details/gbdywrugv.sHtML

val n: String? = null;  n?.length
来源：http://3g.fktsv.cn/Article/details/gdhtgobsy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/gmxydwwvv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.vehdjk.com/Article/details/gmzffzels.sHtML

[T06] Kotlin：集合映射
来源：http://blog.yfazqb.com/Article/details/gbqignyvw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gbopjsvqk.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/gntnhesng.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fktsv.cn/Article/details/gbmpeldxa.sHtML

[T08] Kotlin：数据类
来源：http://3g.yfazqb.com/Article/details/geijdbecf.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.yfazqb.com/Article/details/gbdxowxtz.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.sjlbkw.cn/Article/details/goobkzbbk.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.bbcook.cn/Article/details/gfwtvtggh.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gmuyaaxda.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.yfazqb.com/Article/details/grcpuufct.sHtML

[T11] Kotlin：协程
来源：http://mobile.sjlbkw.cn/Article/details/gojxpmgpz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.epnwcf.com/Article/details/gtfdbmwki.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgqpdtjl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gbqzgwtan.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.epnwcf.com/Article/details/gkqoditzj.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.yfazqb.com/Article/details/gpwaiszuy.sHtML

[T14] Kotlin：循环
来源：http://www.blog.bbcook.cn/Article/details/gtwdyvhtv.sHtML

for (i in 1..10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/gzkespibc.sHtML

[T15] Kotlin：接口
来源：http://baike.bbcook.cn/Article/details/gsbyiunvx.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.vehdjk.com/Article/details/gdgaeuwcv.sHtML

[T16] Swift：Hello World
来源：http://www.blog.bbcook.cn/Article/details/ghvemlwur.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gwmliblsu.sHtML

[T17] Swift：变量与常量
来源：http://baike.vehdjk.com/Article/details/gtnqkliax.sHtML

var a = 1;  let b = 2
来源：http://baike.vehdjk.com/Article/details/gkcalcgwv.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gvrwuzzpo.sHtML

"值: \(b)"
来源：http://www.blog.vehdjk.com/Article/details/gbcihtroy.sHtML

[T19] Swift：可选绑定
来源：http://blog.bbcook.cn/Article/details/gmmzlnaqz.sHtML

if let n = opt { print(n) }
来源：http://blog.yfazqb.com/Article/details/geliavlvx.sHtML

[T20] Swift：数组操作
来源：http://mobile.yfazqb.com/Article/details/gatnswyej.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.yfazqb.com/Article/details/gqmhrhhxt.sHtML

[T21] Swift：遍历
来源：http://baike.bbcook.cn/Article/details/gveguxyzq.sHtML

for x in a { print(x) }
来源：http://www.blog.sjlbkw.cn/Article/details/ghczbwxdh.sHtML

[T22] Swift：字典
来源：http://baike.yfazqb.com/Article/details/gvhqdkecq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fktsv.cn/Article/details/gyyvczizb.sHtML

[T23] Swift：函数
来源：http://3g.tarul.cn/Article/details/glrrubisf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.vehdjk.com/Article/details/gtgvlykgs.sHtML

[T24] Swift：闭包
来源：http://www.share.bbcook.cn/Article/details/giktfyjfm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.vehdjk.com/Article/details/gvtobqkvr.sHtML

[T25] Swift：结构体
来源：http://www.m.share.epnwcf.com/Article/details/ghdtdzkou.sHtML

struct P { var x: Int }
来源：http://www.blog.fktsv.cn/Article/details/gnrdbkafi.sHtML

[T26] Swift：类与重写
来源：http://blog.epnwcf.com/Article/details/glvxrauvr.sHtML

class A: Base { override func f() {} }
来源：http://blog.epnwcf.com/Article/details/glyuegxoe.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fktsv.cn/Article/details/gfkjzikzo.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.epnwcf.com/Article/details/gngpywhwf.sHtML

[T28] Swift：枚举
来源：http://www.m.share.tarul.cn/Article/details/glaxempco.sHtML

enum Color { case red, green }
来源：http://read.share.sjlbkw.cn/Article/details/glxsvtyiz.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.vehdjk.com/Article/details/gwijrocfh.sHtML

guard let x = opt else { return }
来源：http://baike.fktsv.cn/Article/details/gppkyjhnv.sHtML

[T30] Swift：协议
来源：http://baike.bbcook.cn/Article/details/gsuhfthrc.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.sjlbkw.cn/Article/details/gmtsrxcdk.sHtML

[T31] Lua：Hello World
来源：http://baike.epnwcf.com/Article/details/gyyppwfui.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gmodzyllh.sHtML

[T32] Lua：局部变量
来源：http://mobile.fktsv.cn/Article/details/ghipipzfh.sHtML

local a = 1
来源：http://blog.tarul.cn/Article/details/gcdpoviga.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fktsv.cn/Article/details/gequnlvxz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.vehdjk.com/Article/details/ghmszyzst.sHtML

[T34] Lua：遍历表
来源：http://mobile.vehdjk.com/Article/details/gelpegwry.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/gncdgwhqy.sHtML

[T35] Lua：字典表
来源：http://www.blog.bbcook.cn/Article/details/gqngpkcxd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.epnwcf.com/Article/details/gmnjvofhe.sHtML

[T36] Lua：函数
来源：http://www.blog.vehdjk.com/Article/details/gjrkezzwt.sHtML

function add(a, b) return a + b end
来源：http://read.share.epnwcf.com/Article/details/gukdzllfe.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/guikobvmj.sHtML

"a" .. "b"
来源：http://www.blog.bbcook.cn/Article/details/gsecriole.sHtML

[T38] Lua：条件
来源：http://www.blog.bbcook.cn/Article/details/giahdocsl.sHtML

if x > 0 then print("正") end
来源：http://www.blog.yfazqb.com/Article/details/gqsfxrfje.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gpeqcdnpj.sHtML

string.find(s, "%d+")
来源：http://3g.fktsv.cn/Article/details/glwkagyez.sHtML

[T40] Lua：元表
来源：http://baike.tarul.cn/Article/details/gmwudfijy.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.yfazqb.com/Article/details/gocyrkzwe.sHtML

[T41] Perl：Hello World
来源：http://wap.bbcook.cn/Article/details/goietqgne.sHtML

print "Hello\n";
来源：http://mobile.yfazqb.com/Article/details/gixqkljgw.sHtML

[T42] Perl：变量类型
来源：http://3g.vehdjk.com/Article/details/gyptllugh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.tarul.cn/Article/details/gsnhipgyl.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gljetqeee.sHtML

"值: $a"
来源：http://wap.tarul.cn/Article/details/gjhcgzhxd.sHtML

[T44] Perl：条件
来源：http://www.m.share.yfazqb.com/Article/details/gdfyolmrd.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.bbcook.cn/Article/details/gqpppynlz.sHtML

[T45] Perl：数组遍历
来源：http://m.share.tarul.cn/Article/details/gfkbkqome.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.bbcook.cn/Article/details/gytiffddx.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fktsv.cn/Article/details/gbtukpkyb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/gskygukhy.sHtML


<!-- 参考信息 -->