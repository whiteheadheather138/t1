代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fktsv.cn/Article/details/gmlkbcptz.sHtML

[R54] 比较两个文件
来源：http://blog.vehdjk.com/Article/details/gffhicxud.sHtML

diff a.txt b.txt
来源：http://www.blog.vehdjk.com/Article/details/gokejyeky.sHtML

[R55] 压缩与解压
来源：http://m.share.fktsv.cn/Article/details/gkstskpqv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.bbcook.cn/Article/details/guzvixwet.sHtML

[R56] 远程拷贝
来源：http://m.share.tarul.cn/Article/details/gizhmyifz.sHtML

scp file user@host:/path/
来源：http://read.share.bbcook.cn/Article/details/gujaecmcq.sHtML

[R57] 远程执行命令
来源：http://blog.tarul.cn/Article/details/gixllfwss.sHtML

ssh user@host 'uptime'
来源：http://read.share.yfazqb.com/Article/details/gbfqjnpyg.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/ghhyayyxx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.yfazqb.com/Article/details/gieblrjeo.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjkpumbg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.bbcook.cn/Article/details/glqrdappy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/grieyovkz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fktsv.cn/Article/details/gnjlxkdxd.sHtML

[R61] 磁盘占用
来源：http://wap.vehdjk.com/Article/details/gwmvchjkr.sHtML

df -h;  du -sh *
来源：http://read.share.yfazqb.com/Article/details/giujlqulb.sHtML

[R62] 找最占空间的文件
来源：http://baike.yfazqb.com/Article/details/gonjeezvp.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.vehdjk.com/Article/details/gqradzhoe.sHtML

[R63] 内存与进程
来源：http://blog.yfazqb.com/Article/details/gqxafhjeg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fktsv.cn/Article/details/guvyhurkd.sHtML

[R64] 结束进程
来源：http://read.share.epnwcf.com/Article/details/gfmuvtkkr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.sjlbkw.cn/Article/details/gxvxyuwji.sHtML

[R65] 查看端口占用
来源：http://3g.yfazqb.com/Article/details/gokevhhzl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.sjlbkw.cn/Article/details/gtqtkoqpj.sHtML

[R66] 定时任务
来源：http://baike.tarul.cn/Article/details/gytmhxjwh.sHtML

crontab -e;  crontab -l
来源：http://baike.vehdjk.com/Article/details/gppjcvdcj.sHtML

[R67] 生成随机十六进制串
来源：http://blog.bbcook.cn/Article/details/gsudgtaft.sHtML

openssl rand -hex 16
来源：http://wap.epnwcf.com/Article/details/gjnkxiurr.sHtML

[R68] 计算文件校验值
来源：http://mobile.tarul.cn/Article/details/gfovsbgrx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.tarul.cn/Article/details/gjhnumuec.sHtML

[R69] 生成随机密码
来源：http://m.share.yfazqb.com/Article/details/gtguhwnwc.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.sjlbkw.cn/Article/details/gdqtvwgnq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.bbcook.cn/Article/details/gbdltxsum.sHtML

date +%s;  date -d @1700000000
来源：http://3g.vehdjk.com/Article/details/gxzxwqgbv.sHtML

[R71] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gmzcgmvlb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/gbefnwkxj.sHtML

[R72] 等待端口就绪
来源：http://3g.epnwcf.com/Article/details/gvrblqtjg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.sjlbkw.cn/Article/details/gyuihrlui.sHtML

[R73] 分割大日志
来源：http://3g.bbcook.cn/Article/details/gyxovgokc.sHtML

split -l 1000 big.log part_
来源：http://mobile.bbcook.cn/Article/details/gitckwdnk.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/gxmijxitd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.sjlbkw.cn/Article/details/grlywfhaa.sHtML

[R75] 导出环境变量
来源：http://m.share.epnwcf.com/Article/details/gmyvtqzff.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/grqshmqxb.sHtML

[R76] 使用临时文件
来源：http://www.blog.tarul.cn/Article/details/grktprbxx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gxrqvbzlf.sHtML

[R77] 读取用户输入
来源：http://www.blog.epnwcf.com/Article/details/gfxefvxea.sHtML

read -rp "请输入: " ans
来源：http://www.blog.yfazqb.com/Article/details/gprogpgkb.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/gcreiyrol.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.epnwcf.com/Article/details/glomxepao.sHtML

[R79] 解析命令行选项
来源：http://www.share.fktsv.cn/Article/details/ggihxfeyw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.sjlbkw.cn/Article/details/gvvdbujiy.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.tarul.cn/Article/details/gfxxwwuey.sHtML

time ./run.sh
来源：http://3g.bbcook.cn/Article/details/gtuxcwnre.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbcthypnp.sHtML

S. C / C++ 专题
来源：http://www.blog.sjlbkw.cn/Article/details/glnxiasfb.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ggmnyifvv.sHtML

[S01] C：Hello World
来源：http://wap.epnwcf.com/Article/details/gcyehzcwh.sHtML

#include <stdio.h>
来源：http://mobile.sjlbkw.cn/Article/details/gvzggarlb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.epnwcf.com/Article/details/gfsdtjylo.sHtML

[S02] C：变量与格式化输出
来源：http://baike.sjlbkw.cn/Article/details/guznjhiqq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcewomgw.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gyueiciup.sHtML

int x; scanf("%d", &x);
来源：http://baike.bbcook.cn/Article/details/gjupgygzg.sHtML

[S04] C：字符串复制
来源：http://3g.epnwcf.com/Article/details/gzsfppmgq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gteuajurz.sHtML

[S05] C：字符串长度
来源：http://mobile.vehdjk.com/Article/details/gxyoqwbdm.sHtML

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/gxrtsjxyo.sHtML

[S06] C：字符串比较
来源：http://read.share.yfazqb.com/Article/details/ggdkpmeiy.sHtML

strcmp(a, b) == 0
来源：http://3g.epnwcf.com/Article/details/gagamhljo.sHtML

[S07] C：数组遍历求和
来源：http://www.share.tarul.cn/Article/details/gzweertme.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.tarul.cn/Article/details/gsaphahyt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fktsv.cn/Article/details/guingumaw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.sjlbkw.cn/Article/details/gnziwbxsi.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.vehdjk.com/Article/details/gxzcdavtu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvsopida.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/gtdcmiayl.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.bbcook.cn/Article/details/gejslsptg.sHtML

[S11] C：逐行读文件
来源：http://blog.tarul.cn/Article/details/gslbfzfkx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.vehdjk.com/Article/details/gdmyaviqa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fktsv.cn/Article/details/gzxmwojmv.sHtML

fclose(f);
来源：http://read.share.tarul.cn/Article/details/ggngbkbhl.sHtML

[S12] C：写文件
来源：http://mobile.fktsv.cn/Article/details/gjjdtuokv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fktsv.cn/Article/details/gyyqgcjwz.sHtML

[S13] C：宏定义
来源：http://wap.vehdjk.com/Article/details/gunaqzega.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.sjlbkw.cn/Article/details/gucrrpfjo.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/gwemxsdpv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/gdbfotoji.sHtML

[S15] C：类型转换
来源：http://read.share.yfazqb.com/Article/details/gilqqfvdp.sHtML

(double) a / b
来源：http://baike.tarul.cn/Article/details/gljiwoizd.sHtML

[S16] C：位操作置位
来源：http://3g.fktsv.cn/Article/details/gcgoaazoh.sHtML

x |= (1 << 3);
来源：http://m.share.sjlbkw.cn/Article/details/gvhhndduo.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/grmgzykgo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.tarul.cn/Article/details/gbgfeptgc.sHtML

[S18] C：命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/gixafeunp.sHtML

int main(int argc, char **argv)
来源：http://m.share.vehdjk.com/Article/details/gjoconbsg.sHtML

[S19] C：快速排序
来源：http://baike.sjlbkw.cn/Article/details/gluhxfhhz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gddwqnpnt.sHtML

[S20] C：二分查找
来源：http://wap.tarul.cn/Article/details/ggmsbhkqq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/grreffpuy.sHtML

[S21] C：字符类别判断
来源：http://read.share.vehdjk.com/Article/details/gddmtxagu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.bbcook.cn/Article/details/glxtjubhu.sHtML

[S22] C：字符串转数字
来源：http://blog.tarul.cn/Article/details/gyaqasxmz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/gpgjvybyh.sHtML

[S23] C：随机数
来源：http://blog.yfazqb.com/Article/details/grvcjnlmg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.vehdjk.com/Article/details/gvlgnkleb.sHtML

[S24] C：获取本地时间
来源：http://3g.epnwcf.com/Article/details/gyscfnmmq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/gojdijypf.sHtML

[S25] C：内存拷贝
来源：http://www.share.sjlbkw.cn/Article/details/grcivrcgw.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gihrqotxw.sHtML

[S26] C：内存清零
来源：http://wap.yfazqb.com/Article/details/gbgdbxjao.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.sjlbkw.cn/Article/details/gopydtnlv.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gdkwhbqrt.sHtML

const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/golwshsfh.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gskwbhibm.sHtML

static int counter = 0;
来源：http://mobile.bbcook.cn/Article/details/gxoqrjpao.sHtML

[S29] C：变参函数
来源：http://www.m.share.tarul.cn/Article/details/ggzmcdbsp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/gnsnxlmci.sHtML

[S30] C：头文件保护
来源：http://baike.yfazqb.com/Article/details/gtmaikqqr.sHtML

#ifndef X_H
来源：http://www.blog.epnwcf.com/Article/details/ggvouagxx.sHtML

#define X_H
来源：http://blog.yfazqb.com/Article/details/gwplwblos.sHtML

#endif
来源：http://baike.epnwcf.com/Article/details/gthwnnwye.sHtML

[S31] C++：Hello World
来源：http://www.blog.yfazqb.com/Article/details/ghdsokkhm.sHtML

#include <iostream>
来源：http://wap.epnwcf.com/Article/details/gpngmrufe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.tarul.cn/Article/details/genwqjeex.sHtML

[S32] C++：字符串
来源：http://www.blog.vehdjk.com/Article/details/gixvohqcd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.bbcook.cn/Article/details/gwqdrmmpv.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.sjlbkw.cn/Article/details/godgsnmvh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.bbcook.cn/Article/details/gvbpzcemr.sHtML

[S34] C++：遍历 vector
来源：http://read.share.bbcook.cn/Article/details/gooccxkjm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fktsv.cn/Article/details/gqioguysq.sHtML

[S35] C++：map
来源：http://www.blog.fktsv.cn/Article/details/gdlqzttsn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gnnrmwkrl.sHtML

[S36] C++：unordered_map
来源：http://read.share.bbcook.cn/Article/details/gynyispss.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/gjjpfuatw.sHtML

[S37] C++：set
来源：http://www.share.vehdjk.com/Article/details/gaywttyxi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.sjlbkw.cn/Article/details/gjlgfruel.sHtML

[S38] C++：排序
来源：http://wap.tarul.cn/Article/details/gjjixdzjk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gclixyuju.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.epnwcf.com/Article/details/ghrqcrmlr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.tarul.cn/Article/details/gcpndoqwt.sHtML

[S40] C++：查找元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdtjjduo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.yfazqb.com/Article/details/gccyqnksu.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fktsv.cn/Article/details/gkjtkhpjn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fktsv.cn/Article/details/gpaqgczjo.sHtML

[S42] C++：继承与虚函数
来源：http://baike.epnwcf.com/Article/details/gadknrobu.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fktsv.cn/Article/details/ghqsalmlz.sHtML

[S43] C++：智能指针
来源：http://3g.fktsv.cn/Article/details/gfweejmev.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fktsv.cn/Article/details/gteiivfmg.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/gjtqfdozn.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.yfazqb.com/Article/details/gfyohmugw.sHtML

[S45] C++：lambda
来源：http://3g.sjlbkw.cn/Article/details/guwjbiulc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.tarul.cn/Article/details/gbmzwjaeu.sHtML

[S46] C++：函数模板
来源：http://wap.sjlbkw.cn/Article/details/gxcrvmxsc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.bbcook.cn/Article/details/gcscouuww.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/gpmxrziga.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.bbcook.cn/Article/details/gmddymafd.sHtML

[S48] C++：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gfompunco.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gbfayorzl.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/gfsfyldyw.sHtML

[S49] C++：写文件
来源：http://wap.sjlbkw.cn/Article/details/gnlmwhbuq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.epnwcf.com/Article/details/gfepznftf.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/gqqqxyjpd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gonxtksfw.sHtML

[S51] C++：显式类型转换
来源：http://blog.sjlbkw.cn/Article/details/gmpclfprn.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/gqnkusijw.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.yfazqb.com/Article/details/ggiwdhypx.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.yfazqb.com/Article/details/gtoooajge.sHtML

[S53] C++：移动语义
来源：http://baike.yfazqb.com/Article/details/gxrdpujxk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.tarul.cn/Article/details/gkngmlvol.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/gjpcfuwfx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/goossuuaj.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/gieporkwd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.yfazqb.com/Article/details/gbwkedppf.sHtML

[S56] C++：optional
来源：http://baike.epnwcf.com/Article/details/ggevmeisb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.tarul.cn/Article/details/gpbkrfbao.sHtML

[S57] C++：编译期常量
来源：http://3g.bbcook.cn/Article/details/gkozbljel.sHtML

constexpr int N = 10;
来源：http://m.share.tarul.cn/Article/details/gwfnbloyz.sHtML

[S58] C++：命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gsvznfjcr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.yfazqb.com/Article/details/gkpikkdtx.sHtML

[S59] C++：静态断言
来源：http://www.blog.fktsv.cn/Article/details/gpidbggto.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.vehdjk.com/Article/details/gzefecjlb.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.vehdjk.com/Article/details/gevnnnjrh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gyhfuohhk.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gfijtzuyv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gaxcufqip.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gaduedgdk.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/gqoucxhjq.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/gvmmtccvt.sHtML

[T02] Kotlin：变量
来源：http://www.blog.vehdjk.com/Article/details/gjmlhwssx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.yfazqb.com/Article/details/gfnaucnox.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.vehdjk.com/Article/details/guorcfqrj.sHtML

"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/gejrxjhuf.sHtML

[T04] Kotlin：空安全
来源：http://baike.fktsv.cn/Article/details/gsjqymfby.sHtML

val n: String? = null;  n?.length
来源：http://blog.vehdjk.com/Article/details/gqxucvldd.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gtrtllsib.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.bbcook.cn/Article/details/gfljurgld.sHtML

[T06] Kotlin：集合映射
来源：http://3g.sjlbkw.cn/Article/details/gpozyiwmb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gegbubxmg.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.vehdjk.com/Article/details/gyyrqgncb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.vehdjk.com/Article/details/gzcqwnmox.sHtML

[T08] Kotlin：数据类
来源：http://mobile.vehdjk.com/Article/details/grbboqkyv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/gipmdujkp.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.sjlbkw.cn/Article/details/gpemzxbmy.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.epnwcf.com/Article/details/ggendwjmm.sHtML

[T10] Kotlin：默认参数
来源：http://baike.epnwcf.com/Article/details/gkxfikttz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gdygbqlnl.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.vehdjk.com/Article/details/gthyxjukd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.vehdjk.com/Article/details/gqwgxawnk.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.epnwcf.com/Article/details/gqkbgossd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.epnwcf.com/Article/details/gzlobrthh.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.epnwcf.com/Article/details/gabsxqlfu.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fktsv.cn/Article/details/goncpthck.sHtML

[T14] Kotlin：循环
来源：http://3g.sjlbkw.cn/Article/details/grbdsfrrp.sHtML

for (i in 1..10) println(i)
来源：http://wap.sjlbkw.cn/Article/details/gstuycxfa.sHtML

[T15] Kotlin：接口
来源：http://www.share.vehdjk.com/Article/details/geqryfhuq.sHtML

interface Shape { fun area(): Double }
来源：http://blog.sjlbkw.cn/Article/details/gvdnkeypi.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gzmmmrppk.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gqstwydhf.sHtML

[T17] Swift：变量与常量
来源：http://m.share.epnwcf.com/Article/details/gztesrytw.sHtML

var a = 1;  let b = 2
来源：http://baike.tarul.cn/Article/details/gkrvpwvdz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gnpdlmrll.sHtML

"值: \(b)"
来源：http://blog.tarul.cn/Article/details/giyorjixk.sHtML

[T19] Swift：可选绑定
来源：http://wap.sjlbkw.cn/Article/details/gydorkjiq.sHtML

if let n = opt { print(n) }
来源：http://3g.sjlbkw.cn/Article/details/gzwbkxrns.sHtML

[T20] Swift：数组操作
来源：http://baike.sjlbkw.cn/Article/details/gqxgmredh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.bbcook.cn/Article/details/gsjanjpht.sHtML

[T21] Swift：遍历
来源：http://mobile.epnwcf.com/Article/details/gbuwufosi.sHtML

for x in a { print(x) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtiivwdf.sHtML

[T22] Swift：字典
来源：http://baike.epnwcf.com/Article/details/ggsolfact.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.sjlbkw.cn/Article/details/gtwcrklbm.sHtML

[T23] Swift：函数
来源：http://baike.fktsv.cn/Article/details/gxyskmxmf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fktsv.cn/Article/details/gdyonxczb.sHtML

[T24] Swift：闭包
来源：http://www.blog.yfazqb.com/Article/details/gnzvnivnq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.bbcook.cn/Article/details/gcipwxgew.sHtML

[T25] Swift：结构体
来源：http://baike.fktsv.cn/Article/details/givlsroap.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/gaatneypi.sHtML

[T26] Swift：类与重写
来源：http://m.share.sjlbkw.cn/Article/details/gqykmyuty.sHtML

class A: Base { override func f() {} }
来源：http://blog.epnwcf.com/Article/details/gujiakvtg.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gbdjsuslr.sHtML

do { try f() } catch { print(error) }
来源：http://3g.epnwcf.com/Article/details/gokorkwrf.sHtML

[T28] Swift：枚举
来源：http://www.blog.tarul.cn/Article/details/gkcexzfso.sHtML

enum Color { case red, green }
来源：http://www.m.share.epnwcf.com/Article/details/gxtuksfrp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.epnwcf.com/Article/details/ggjlvgztl.sHtML

guard let x = opt else { return }
来源：http://www.blog.bbcook.cn/Article/details/gbnkfsltn.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/ghdozlcpl.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.tarul.cn/Article/details/gghomsibl.sHtML

[T31] Lua：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gugbctaqx.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/guhbqdvet.sHtML

[T32] Lua：局部变量
来源：http://baike.fktsv.cn/Article/details/gdscnuwyk.sHtML

local a = 1
来源：http://baike.vehdjk.com/Article/details/gzaqhzyvp.sHtML

[T33] Lua：表（数组）
来源：http://blog.fktsv.cn/Article/details/gsycklnwc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.bbcook.cn/Article/details/gpywwrwmw.sHtML

[T34] Lua：遍历表
来源：http://www.blog.vehdjk.com/Article/details/gjbhrgevm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fktsv.cn/Article/details/gakrfpsry.sHtML

[T35] Lua：字典表
来源：http://www.m.share.bbcook.cn/Article/details/ghxxfxbjk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.bbcook.cn/Article/details/grccwvpzl.sHtML

[T36] Lua：函数
来源：http://blog.bbcook.cn/Article/details/ghdhoyeac.sHtML

function add(a, b) return a + b end
来源：http://baike.fktsv.cn/Article/details/ghlyfdpsf.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.tarul.cn/Article/details/grjfrwide.sHtML

"a" .. "b"
来源：http://mobile.tarul.cn/Article/details/gwndsdxyg.sHtML

[T38] Lua：条件
来源：http://baike.fktsv.cn/Article/details/gwkqketyk.sHtML

if x > 0 then print("正") end
来源：http://mobile.fktsv.cn/Article/details/gkadpczzp.sHtML

[T39] Lua：模式匹配
来源：http://m.share.bbcook.cn/Article/details/gqroamiag.sHtML

string.find(s, "%d+")
来源：http://3g.vehdjk.com/Article/details/gsctswcms.sHtML

[T40] Lua：元表
来源：http://www.share.vehdjk.com/Article/details/gszksmpnw.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.vehdjk.com/Article/details/ghlinlvzd.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gvmvvkvbk.sHtML

print "Hello\n";
来源：http://wap.tarul.cn/Article/details/gioywgyit.sHtML

[T42] Perl：变量类型
来源：http://www.blog.tarul.cn/Article/details/gpvesokri.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.vehdjk.com/Article/details/ghafcpgyf.sHtML

[T43] Perl：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/grarpolys.sHtML

"值: $a"
来源：http://blog.yfazqb.com/Article/details/gkyvopepc.sHtML

[T44] Perl：条件
来源：http://blog.fktsv.cn/Article/details/gkgyrifpd.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.bbcook.cn/Article/details/gfdsmfrkk.sHtML

[T45] Perl：数组遍历
来源：http://baike.epnwcf.com/Article/details/gvwaaxcpn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.bbcook.cn/Article/details/gzoquwhph.sHtML

[T46] Perl：哈希操作
来源：http://wap.yfazqb.com/Article/details/girbnsner.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.sjlbkw.cn/Article/details/gzfeytvgm.sHtML

[T47] Perl：正则捕获
来源：http://mobile.bbcook.cn/Article/details/gqorvufin.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.yfazqb.com/Article/details/gpzktsjbx.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/ghashcmos.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.epnwcf.com/Article/details/gwuzoiqgu.sHtML

[T49] Perl：函数
来源：http://m.share.tarul.cn/Article/details/gkqtjolnu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gcptjzilk.sHtML

[T50] Perl：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gfokwdjdp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.yfazqb.com/Article/details/gxtiiljxa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.vehdjk.com/Article/details/gklsuyvjp.sHtML

[T51] Scala：Hello World
来源：http://blog.fktsv.cn/Article/details/ggtuoiynx.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/giukjlxlo.sHtML

[T52] Scala：变量
来源：http://wap.bbcook.cn/Article/details/gcjsjnlqf.sHtML

val a = 1;  var b = 2
来源：http://read.share.bbcook.cn/Article/details/gareoxdub.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/guifcieyn.sHtML

s"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/gpnqtmwhf.sHtML

[T54] Scala：集合映射
来源：http://baike.sjlbkw.cn/Article/details/gjmajtilr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.epnwcf.com/Article/details/ggafxsbfp.sHtML

[T55] Scala：集合过滤
来源：http://wap.vehdjk.com/Article/details/gjvsxdqmi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.yfazqb.com/Article/details/gdgwddrbp.sHtML

[T56] Scala：样例类
来源：http://3g.fktsv.cn/Article/details/gxfsfdbrt.sHtML


<!-- 参考信息 -->