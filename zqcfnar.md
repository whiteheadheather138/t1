代发 wailian999

find . -name "*.tmp" -delete
来源：http://3g.tarul.cn/Article/details/gjkgbcwho.sHtML

[R46] 递归替换文件内容
来源：http://mobile.sjlbkw.cn/Article/details/ggppykmhq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.sjlbkw.cn/Article/details/gbuhnbgun.sHtML

[R47] sed 单行替换
来源：http://www.blog.bbcook.cn/Article/details/gbxjjolsl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.yfazqb.com/Article/details/gfjzesnah.sHtML

[R48] awk 取指定列
来源：http://baike.fktsv.cn/Article/details/gxtlajnsk.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.tarul.cn/Article/details/gsmibtnfu.sHtML

[R49] awk 带条件
来源：http://read.share.vehdjk.com/Article/details/gaxtoshxu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.bbcook.cn/Article/details/gelrbtlby.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/gmsrrbxvk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gwsxwfnwv.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/gbkhguvep.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/gsclixmeq.sHtML

[R52] 统计行数
来源：http://www.m.share.fktsv.cn/Article/details/gzrcjulet.sHtML

wc -l a.txt
来源：http://m.share.vehdjk.com/Article/details/gazpgqadu.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.epnwcf.com/Article/details/gvletxqkp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.vehdjk.com/Article/details/guwhmtudk.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqzzovws.sHtML

diff a.txt b.txt
来源：http://3g.sjlbkw.cn/Article/details/gfulfhjxt.sHtML

[R55] 压缩与解压
来源：http://m.share.vehdjk.com/Article/details/gzbuslrpn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.vehdjk.com/Article/details/gwrpzdyrj.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/grnqvifqb.sHtML

scp file user@host:/path/
来源：http://www.blog.yfazqb.com/Article/details/gigpsyhcu.sHtML

[R57] 远程执行命令
来源：http://read.share.epnwcf.com/Article/details/gegyddcrn.sHtML

ssh user@host 'uptime'
来源：http://www.share.sjlbkw.cn/Article/details/gklneurga.sHtML

[R58] 下载文件
来源：http://wap.vehdjk.com/Article/details/gtygdgfnv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.sjlbkw.cn/Article/details/gamcppxsm.sHtML

[R59] 发 POST JSON
来源：http://3g.yfazqb.com/Article/details/gbabhrpsl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.sjlbkw.cn/Article/details/gfzfinygi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gujsmtzep.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.bbcook.cn/Article/details/gpbnkwjsd.sHtML

[R61] 磁盘占用
来源：http://3g.epnwcf.com/Article/details/gfisxowzm.sHtML

df -h;  du -sh *
来源：http://blog.tarul.cn/Article/details/ghclhuwck.sHtML

[R62] 找最占空间的文件
来源：http://mobile.yfazqb.com/Article/details/gwddtwlmm.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.yfazqb.com/Article/details/gwgrftvtv.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/grxglaiig.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.yfazqb.com/Article/details/gltpbdzhh.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gkljtsgtz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.sjlbkw.cn/Article/details/gwugeigin.sHtML

[R65] 查看端口占用
来源：http://wap.epnwcf.com/Article/details/gsaxltboz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.yfazqb.com/Article/details/grjfbzrju.sHtML

[R66] 定时任务
来源：http://www.blog.vehdjk.com/Article/details/gagqkfjob.sHtML

crontab -e;  crontab -l
来源：http://mobile.sjlbkw.cn/Article/details/gfrgnhufg.sHtML

[R67] 生成随机十六进制串
来源：http://wap.bbcook.cn/Article/details/gslpneqpc.sHtML

openssl rand -hex 16
来源：http://mobile.epnwcf.com/Article/details/gojjzqnib.sHtML

[R68] 计算文件校验值
来源：http://m.share.fktsv.cn/Article/details/gfbpysuts.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fktsv.cn/Article/details/gzisuufdc.sHtML

[R69] 生成随机密码
来源：http://www.blog.sjlbkw.cn/Article/details/ggbewcdth.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.vehdjk.com/Article/details/gphvpmnxr.sHtML

[R70] 时间戳与互转
来源：http://3g.yfazqb.com/Article/details/gdvyoyocd.sHtML

date +%s;  date -d @1700000000
来源：http://blog.tarul.cn/Article/details/gklxfxyjm.sHtML

[R71] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gsgwktnmm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.epnwcf.com/Article/details/gogqkzxjd.sHtML

[R72] 等待端口就绪
来源：http://read.share.tarul.cn/Article/details/gbnqbsixt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gsdwtmskz.sHtML

[R73] 分割大日志
来源：http://3g.epnwcf.com/Article/details/gocrdpdes.sHtML

split -l 1000 big.log part_
来源：http://baike.vehdjk.com/Article/details/gcirpfapq.sHtML

[R74] 批量重命名
来源：http://m.share.yfazqb.com/Article/details/gambukmtv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.bbcook.cn/Article/details/giwlqouau.sHtML

[R75] 导出环境变量
来源：http://wap.yfazqb.com/Article/details/gyudhnuxp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.epnwcf.com/Article/details/gsgdpzbei.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/gblnvozxp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gjndrdseo.sHtML

[R77] 读取用户输入
来源：http://baike.vehdjk.com/Article/details/gubsftvep.sHtML

read -rp "请输入: " ans
来源：http://3g.yfazqb.com/Article/details/gsewwbouy.sHtML

[R78] 交互式菜单
来源：http://www.m.share.bbcook.cn/Article/details/gryvhdrnh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.tarul.cn/Article/details/gyffgpbiy.sHtML

[R79] 解析命令行选项
来源：http://mobile.sjlbkw.cn/Article/details/ghkcpstnr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fktsv.cn/Article/details/gkivpfvwg.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/gxprhhruc.sHtML

time ./run.sh
来源：http://m.share.epnwcf.com/Article/details/guahzxgjk.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/giqalafkj.sHtML

S. C / C++ 专题
来源：http://blog.vehdjk.com/Article/details/grpqubgwv.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gkmnmuase.sHtML

[S01] C：Hello World
来源：http://wap.tarul.cn/Article/details/gbejdgvfr.sHtML

#include <stdio.h>
来源：http://mobile.yfazqb.com/Article/details/gzknuktxq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.tarul.cn/Article/details/grmomuqgk.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.tarul.cn/Article/details/gtejegeww.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.yfazqb.com/Article/details/gufipvtal.sHtML

[S03] C：读入整数
来源：http://baike.tarul.cn/Article/details/godhofnoz.sHtML

int x; scanf("%d", &x);
来源：http://mobile.bbcook.cn/Article/details/giocctxvb.sHtML

[S04] C：字符串复制
来源：http://baike.sjlbkw.cn/Article/details/gaasbqxcz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.bbcook.cn/Article/details/gfrdmdetc.sHtML

[S05] C：字符串长度
来源：http://mobile.bbcook.cn/Article/details/gfhgoqoyn.sHtML

strlen(s)
来源：http://mobile.vehdjk.com/Article/details/gjgstvizp.sHtML

[S06] C：字符串比较
来源：http://m.share.epnwcf.com/Article/details/gsxgjnjab.sHtML

strcmp(a, b) == 0
来源：http://mobile.epnwcf.com/Article/details/govvgxxxx.sHtML

[S07] C：数组遍历求和
来源：http://www.share.tarul.cn/Article/details/gerfrcbbf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.vehdjk.com/Article/details/gziaxteov.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.sjlbkw.cn/Article/details/gjkpqsruo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.vehdjk.com/Article/details/gthsefpba.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.vehdjk.com/Article/details/gvujtkeeg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.epnwcf.com/Article/details/gyxsqbaty.sHtML

[S10] C：指针与解引用
来源：http://blog.yfazqb.com/Article/details/gunoojcvu.sHtML

int *p = &a;  *p = 5;
来源：http://baike.vehdjk.com/Article/details/gwidicsex.sHtML

[S11] C：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gkbhcbunt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.tarul.cn/Article/details/gzpfmwtya.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.epnwcf.com/Article/details/ggixdujvp.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/galdbqcnw.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/ghhijuxiu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.epnwcf.com/Article/details/gesfbfqzn.sHtML

[S13] C：宏定义
来源：http://baike.fktsv.cn/Article/details/gqbxgondx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/gkpybddft.sHtML

[S14] C：枚举
来源：http://www.m.share.vehdjk.com/Article/details/gfxxqudbt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.bbcook.cn/Article/details/gxyrddtpe.sHtML

[S15] C：类型转换
来源：http://blog.epnwcf.com/Article/details/gksefhoby.sHtML

(double) a / b
来源：http://baike.bbcook.cn/Article/details/gicmeaztr.sHtML

[S16] C：位操作置位
来源：http://wap.sjlbkw.cn/Article/details/gyhfhqoej.sHtML

x |= (1 << 3);
来源：http://www.blog.bbcook.cn/Article/details/gwlghjlyn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gzwasntuj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.epnwcf.com/Article/details/gfjzbgllc.sHtML

[S18] C：命令行参数
来源：http://www.share.bbcook.cn/Article/details/geugffzmp.sHtML

int main(int argc, char **argv)
来源：http://wap.tarul.cn/Article/details/ggqngzbof.sHtML

[S19] C：快速排序
来源：http://blog.tarul.cn/Article/details/gehjtuxnu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gpxokqtum.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/geasrcogu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gnduvmwaf.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnxpasev.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.epnwcf.com/Article/details/gvuuicgmq.sHtML

[S22] C：字符串转数字
来源：http://m.share.vehdjk.com/Article/details/gvkmilhpv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.tarul.cn/Article/details/gshkioctx.sHtML

[S23] C：随机数
来源：http://3g.tarul.cn/Article/details/gwtnhbbua.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.sjlbkw.cn/Article/details/gocuykvrg.sHtML

[S24] C：获取本地时间
来源：http://wap.epnwcf.com/Article/details/gfukhfhid.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.bbcook.cn/Article/details/gjkzouehi.sHtML

[S25] C：内存拷贝
来源：http://www.blog.vehdjk.com/Article/details/gvxaeoxxc.sHtML

memcpy(dst, src, n);
来源：http://3g.vehdjk.com/Article/details/gmyljjckq.sHtML

[S26] C：内存清零
来源：http://m.share.fktsv.cn/Article/details/glirgtepz.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.epnwcf.com/Article/details/guowtfnzu.sHtML

[S27] C：定义常量
来源：http://blog.vehdjk.com/Article/details/gerqjodxc.sHtML

const double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gokiumocn.sHtML

[S28] C：静态变量
来源：http://m.share.fktsv.cn/Article/details/gkyjpnhmw.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/gvjnboirm.sHtML

[S29] C：变参函数
来源：http://www.m.share.bbcook.cn/Article/details/gyrhoyeuz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.bbcook.cn/Article/details/gmlyrtyeq.sHtML

[S30] C：头文件保护
来源：http://3g.fktsv.cn/Article/details/giowaaeyy.sHtML

#ifndef X_H
来源：http://www.m.share.bbcook.cn/Article/details/gfplpcymq.sHtML

#define X_H
来源：http://3g.vehdjk.com/Article/details/gdvcfzphz.sHtML

#endif
来源：http://wap.vehdjk.com/Article/details/gfalvigla.sHtML

[S31] C++：Hello World
来源：http://www.blog.tarul.cn/Article/details/gyicgrufz.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/gbcranpab.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.sjlbkw.cn/Article/details/gobymibkq.sHtML

[S32] C++：字符串
来源：http://m.share.yfazqb.com/Article/details/glgnzilit.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.yfazqb.com/Article/details/gzlwnyqns.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/gbjxfmncn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.sjlbkw.cn/Article/details/gxntxvbwf.sHtML

[S34] C++：遍历 vector
来源：http://m.share.vehdjk.com/Article/details/gooizlofx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.tarul.cn/Article/details/gbbhgmgox.sHtML

[S35] C++：map
来源：http://mobile.sjlbkw.cn/Article/details/gcdcmaeeb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gkupjluqt.sHtML

[S36] C++：unordered_map
来源：http://m.share.sjlbkw.cn/Article/details/gxpxbtyxf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gzmuzutaf.sHtML

[S37] C++：set
来源：http://wap.yfazqb.com/Article/details/gidauhnhj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.sjlbkw.cn/Article/details/gnxrcdiss.sHtML

[S38] C++：排序
来源：http://baike.bbcook.cn/Article/details/gszcothlj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/galcbqysm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.tarul.cn/Article/details/gakxrpaqh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/gatohcycx.sHtML

[S40] C++：查找元素
来源：http://mobile.yfazqb.com/Article/details/gxoqgmqnk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fktsv.cn/Article/details/gipixljua.sHtML

[S41] C++：类与构造函数
来源：http://wap.fktsv.cn/Article/details/gejtjhced.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.epnwcf.com/Article/details/gkumugbvt.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.vehdjk.com/Article/details/geoztelsl.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.sjlbkw.cn/Article/details/gndyqgmun.sHtML

[S43] C++：智能指针
来源：http://blog.tarul.cn/Article/details/gojoqzjxo.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.sjlbkw.cn/Article/details/glejfxixk.sHtML

[S44] C++：引用传参
来源：http://read.share.bbcook.cn/Article/details/gssxfndip.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.bbcook.cn/Article/details/grhgscteq.sHtML

[S45] C++：lambda
来源：http://3g.bbcook.cn/Article/details/goqwpdjwm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.epnwcf.com/Article/details/gjyjlfmei.sHtML

[S46] C++：函数模板
来源：http://m.share.yfazqb.com/Article/details/gqemcepll.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.tarul.cn/Article/details/gahuzxfng.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fktsv.cn/Article/details/gupwfqnej.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.vehdjk.com/Article/details/gvcycqiht.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/glbtvkcdm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.bbcook.cn/Article/details/guuiatmhe.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.vehdjk.com/Article/details/ghhnoulrs.sHtML

[S49] C++：写文件
来源：http://www.share.bbcook.cn/Article/details/gjextvgvd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.bbcook.cn/Article/details/gzhodmlmx.sHtML

[S50] C++：格式化数字
来源：http://read.share.sjlbkw.cn/Article/details/gztgmviir.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gliudkauh.sHtML

[S51] C++：显式类型转换
来源：http://m.share.tarul.cn/Article/details/gshwihirl.sHtML

static_cast<double>(a) / b
来源：http://blog.tarul.cn/Article/details/gizjhiyou.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.bbcook.cn/Article/details/gakdacdtf.sHtML

int size() const noexcept { return n_; }
来源：http://3g.sjlbkw.cn/Article/details/gybgofgln.sHtML

[S53] C++：移动语义
来源：http://m.share.yfazqb.com/Article/details/gmbujjknv.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.yfazqb.com/Article/details/gsikxmamh.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/ggirkuajn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.vehdjk.com/Article/details/gxyigowta.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.yfazqb.com/Article/details/gratazpdg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gfadmqrmh.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/gnrtosvsl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fktsv.cn/Article/details/gawvhkgrc.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/gqpsdaavx.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmylaxds.sHtML

[S58] C++：命名空间
来源：http://blog.vehdjk.com/Article/details/gcgeczczh.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.yfazqb.com/Article/details/gvrcdibdd.sHtML

[S59] C++：静态断言
来源：http://www.m.share.yfazqb.com/Article/details/gwrckvvru.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.sjlbkw.cn/Article/details/ggnsjtxqj.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.bbcook.cn/Article/details/glxmzuhlw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fktsv.cn/Article/details/gpfnlnlyu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/goffhjeiv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/geiokjzst.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gnnsyzjef.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/gajurdlff.sHtML

println("Hello")
来源：http://m.share.bbcook.cn/Article/details/gtobjsnox.sHtML

[T02] Kotlin：变量
来源：http://www.share.bbcook.cn/Article/details/grfkbqtxt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fktsv.cn/Article/details/gfzocyjgr.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.sjlbkw.cn/Article/details/ggajbpsnf.sHtML

"值: $b"
来源：http://3g.fktsv.cn/Article/details/gkwsdxeox.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/glpttmqrb.sHtML

val n: String? = null;  n?.length
来源：http://wap.fktsv.cn/Article/details/gskjmogkb.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.sjlbkw.cn/Article/details/grgmzdudx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.epnwcf.com/Article/details/ghfyuyobb.sHtML

[T06] Kotlin：集合映射
来源：http://blog.sjlbkw.cn/Article/details/ggorbqtbu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.yfazqb.com/Article/details/ghrwfmgcr.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fktsv.cn/Article/details/gzmpmwkaw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/gtlowwxdx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.vehdjk.com/Article/details/gbkishmyt.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.epnwcf.com/Article/details/gewaoearq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/gfckbatvs.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.vehdjk.com/Article/details/gmrqnpwtt.sHtML

[T10] Kotlin：默认参数
来源：http://wap.tarul.cn/Article/details/goclnaxbe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.vehdjk.com/Article/details/grbijabbd.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.epnwcf.com/Article/details/gaguzvjuq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.yfazqb.com/Article/details/ggqmjoxhx.sHtML

[T12] Kotlin：解构声明
来源：http://blog.sjlbkw.cn/Article/details/ghldnspkw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.vehdjk.com/Article/details/gouxadpuf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.epnwcf.com/Article/details/guhlxizon.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fktsv.cn/Article/details/gkulvmsbx.sHtML

[T14] Kotlin：循环
来源：http://wap.sjlbkw.cn/Article/details/gcwxwolhe.sHtML

for (i in 1..10) println(i)
来源：http://blog.yfazqb.com/Article/details/gebvnehnh.sHtML

[T15] Kotlin：接口
来源：http://m.share.fktsv.cn/Article/details/gzwxgzkuc.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fktsv.cn/Article/details/gnjxuglei.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gswklkdpo.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gnehfxrwb.sHtML

[T17] Swift：变量与常量
来源：http://mobile.bbcook.cn/Article/details/gfdiuuwez.sHtML

var a = 1;  let b = 2
来源：http://mobile.epnwcf.com/Article/details/gnnxhqrox.sHtML

[T18] Swift：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gdhlsxcsx.sHtML

"值: \(b)"
来源：http://www.share.yfazqb.com/Article/details/ghhzhglbq.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/gzhvdbdtj.sHtML

if let n = opt { print(n) }
来源：http://m.share.fktsv.cn/Article/details/gitbmuqas.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/goldztdcg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.vehdjk.com/Article/details/geyymymtd.sHtML

[T21] Swift：遍历
来源：http://www.share.fktsv.cn/Article/details/gwidhdhrp.sHtML

for x in a { print(x) }
来源：http://www.share.fktsv.cn/Article/details/gtuhjarfh.sHtML

[T22] Swift：字典
来源：http://www.blog.sjlbkw.cn/Article/details/gybtqidfm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.yfazqb.com/Article/details/ghnbtjcda.sHtML

[T23] Swift：函数
来源：http://wap.bbcook.cn/Article/details/gditiqrwa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.tarul.cn/Article/details/gxvzoqwnq.sHtML

[T24] Swift：闭包
来源：http://mobile.bbcook.cn/Article/details/gnqnymauv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.bbcook.cn/Article/details/gxrkkruek.sHtML

[T25] Swift：结构体
来源：http://read.share.fktsv.cn/Article/details/gqisfwldn.sHtML

struct P { var x: Int }
来源：http://blog.vehdjk.com/Article/details/gkpecavzf.sHtML

[T26] Swift：类与重写
来源：http://baike.vehdjk.com/Article/details/glxgkyulv.sHtML

class A: Base { override func f() {} }
来源：http://baike.tarul.cn/Article/details/gzulxwsse.sHtML

[T27] Swift：错误处理
来源：http://m.share.tarul.cn/Article/details/glzknqcmr.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fktsv.cn/Article/details/gxmxxnbrt.sHtML

[T28] Swift：枚举
来源：http://m.share.bbcook.cn/Article/details/ghssgdqsr.sHtML

enum Color { case red, green }
来源：http://blog.vehdjk.com/Article/details/gnranmwet.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/giuoxqjwr.sHtML

guard let x = opt else { return }
来源：http://www.blog.vehdjk.com/Article/details/gnnexocqx.sHtML

[T30] Swift：协议
来源：http://read.share.vehdjk.com/Article/details/gqrsqfecx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.yfazqb.com/Article/details/gmaalnzgy.sHtML

[T31] Lua：Hello World
来源：http://baike.epnwcf.com/Article/details/gbspabvei.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gwdhmqkir.sHtML

[T32] Lua：局部变量
来源：http://wap.vehdjk.com/Article/details/ghazokhmj.sHtML

local a = 1
来源：http://www.blog.vehdjk.com/Article/details/ggzhzwjap.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.yfazqb.com/Article/details/gdsljfuua.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fktsv.cn/Article/details/gntipzqrh.sHtML

[T34] Lua：遍历表
来源：http://www.share.vehdjk.com/Article/details/gqndnwhbi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.vehdjk.com/Article/details/gptbxqypv.sHtML

[T35] Lua：字典表
来源：http://www.blog.epnwcf.com/Article/details/gojticvmy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.vehdjk.com/Article/details/gbxupqpvd.sHtML

[T36] Lua：函数
来源：http://www.blog.yfazqb.com/Article/details/gjvhzcbij.sHtML

function add(a, b) return a + b end
来源：http://mobile.vehdjk.com/Article/details/gjjkecksk.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.bbcook.cn/Article/details/gvkjiagxk.sHtML

"a" .. "b"
来源：http://mobile.epnwcf.com/Article/details/gqtngtwws.sHtML

[T38] Lua：条件
来源：http://blog.yfazqb.com/Article/details/glpscogqu.sHtML

if x > 0 then print("正") end
来源：http://www.share.vehdjk.com/Article/details/gtlyfettl.sHtML

[T39] Lua：模式匹配
来源：http://m.share.vehdjk.com/Article/details/gdspfpivd.sHtML

string.find(s, "%d+")
来源：http://mobile.bbcook.cn/Article/details/gbtvxrhno.sHtML

[T40] Lua：元表
来源：http://mobile.vehdjk.com/Article/details/gotezzsqs.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.epnwcf.com/Article/details/gurnsoscj.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gsikvtxos.sHtML

print "Hello\n";
来源：http://3g.epnwcf.com/Article/details/ghznyynnm.sHtML

[T42] Perl：变量类型
来源：http://m.share.epnwcf.com/Article/details/gxeqjjulc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fktsv.cn/Article/details/gaheeebmw.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/grkxxyyrk.sHtML

"值: $a"
来源：http://read.share.epnwcf.com/Article/details/giyqlkghm.sHtML

[T44] Perl：条件
来源：http://m.share.bbcook.cn/Article/details/gtawhdpls.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.vehdjk.com/Article/details/goykyedbw.sHtML

[T45] Perl：数组遍历
来源：http://baike.sjlbkw.cn/Article/details/gegnxawsl.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.epnwcf.com/Article/details/gotdpzaax.sHtML

[T46] Perl：哈希操作
来源：http://mobile.yfazqb.com/Article/details/gqmyxwxdj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.bbcook.cn/Article/details/gkivslpef.sHtML

[T47] Perl：正则捕获
来源：http://m.share.yfazqb.com/Article/details/gybjjolyn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.sjlbkw.cn/Article/details/gbcgxihzc.sHtML

[T48] Perl：正则替换
来源：http://wap.yfazqb.com/Article/details/goxrttiuq.sHtML

$s =~ s/old/new/g;
来源：http://mobile.yfazqb.com/Article/details/goeblocgx.sHtML


<!-- 参考信息 -->