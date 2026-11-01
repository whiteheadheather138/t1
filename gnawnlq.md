代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.tarul.cn/Article/details/goqaccdhy.sHtML

[R54] 比较两个文件
来源：http://baike.fktsv.cn/Article/details/ghhvhlhrr.sHtML

diff a.txt b.txt
来源：http://wap.yfazqb.com/Article/details/gqrvuaqao.sHtML

[R55] 压缩与解压
来源：http://m.share.bbcook.cn/Article/details/gayhctgpc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fktsv.cn/Article/details/gqvbvvsew.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/gdmzdwhtc.sHtML

scp file user@host:/path/
来源：http://3g.bbcook.cn/Article/details/gjkkyuifc.sHtML

[R57] 远程执行命令
来源：http://m.share.sjlbkw.cn/Article/details/gglchrkwk.sHtML

ssh user@host 'uptime'
来源：http://wap.yfazqb.com/Article/details/goqzxjyad.sHtML

[R58] 下载文件
来源：http://www.share.tarul.cn/Article/details/gymkbkymt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.sjlbkw.cn/Article/details/godrnypdx.sHtML

[R59] 发 POST JSON
来源：http://www.share.bbcook.cn/Article/details/gqoipedmz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.tarul.cn/Article/details/guyseuvlr.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gqcomskpf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.sjlbkw.cn/Article/details/ghzlvmycz.sHtML

[R61] 磁盘占用
来源：http://www.blog.yfazqb.com/Article/details/gdtgrjmik.sHtML

df -h;  du -sh *
来源：http://m.share.fktsv.cn/Article/details/grkuylxbh.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/gpcbzkuye.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.tarul.cn/Article/details/gfanavnzv.sHtML

[R63] 内存与进程
来源：http://www.m.share.tarul.cn/Article/details/gcmlylrug.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/gulrddqyq.sHtML

[R64] 结束进程
来源：http://www.m.share.yfazqb.com/Article/details/gptkjwpbq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.epnwcf.com/Article/details/gmbnfzbvg.sHtML

[R65] 查看端口占用
来源：http://www.m.share.vehdjk.com/Article/details/gdnzhvzua.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fktsv.cn/Article/details/gduxapgqe.sHtML

[R66] 定时任务
来源：http://baike.epnwcf.com/Article/details/gjotzczvq.sHtML

crontab -e;  crontab -l
来源：http://www.share.bbcook.cn/Article/details/gcznkfqfx.sHtML

[R67] 生成随机十六进制串
来源：http://wap.tarul.cn/Article/details/gemaajhvu.sHtML

openssl rand -hex 16
来源：http://www.blog.bbcook.cn/Article/details/gltajdosr.sHtML

[R68] 计算文件校验值
来源：http://3g.fktsv.cn/Article/details/goqmehtuh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.tarul.cn/Article/details/gswtiltss.sHtML

[R69] 生成随机密码
来源：http://read.share.tarul.cn/Article/details/gmbkrpwqa.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.yfazqb.com/Article/details/geqjntkvh.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.vehdjk.com/Article/details/gukheocob.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.epnwcf.com/Article/details/giqllemhu.sHtML

[R71] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/gyhtdmiuc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.bbcook.cn/Article/details/gjdirmecy.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gqhdeweyk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gyjvsgoad.sHtML

[R73] 分割大日志
来源：http://blog.fktsv.cn/Article/details/ggneqdimo.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fktsv.cn/Article/details/gzglelppn.sHtML

[R74] 批量重命名
来源：http://www.share.bbcook.cn/Article/details/gpvpekfpm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gpfdtrrwq.sHtML

[R75] 导出环境变量
来源：http://baike.vehdjk.com/Article/details/gxrwulane.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fktsv.cn/Article/details/gnjsugmja.sHtML

[R76] 使用临时文件
来源：http://mobile.tarul.cn/Article/details/gpadrdxfr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gcaesvhzd.sHtML

[R77] 读取用户输入
来源：http://read.share.vehdjk.com/Article/details/gcynowuun.sHtML

read -rp "请输入: " ans
来源：http://blog.tarul.cn/Article/details/gmfizprzq.sHtML

[R78] 交互式菜单
来源：http://wap.vehdjk.com/Article/details/gifbbvhbv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.tarul.cn/Article/details/gkritqvmh.sHtML

[R79] 解析命令行选项
来源：http://baike.bbcook.cn/Article/details/gwjjhyggf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.epnwcf.com/Article/details/gmpgwhmrw.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.epnwcf.com/Article/details/gvwgvxsac.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/gefwqyjtv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtpjktwxn.sHtML

S. C / C++ 专题
来源：http://wap.vehdjk.com/Article/details/gkzcfpebl.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gafrznvdj.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/glnzovdwe.sHtML

#include <stdio.h>
来源：http://3g.tarul.cn/Article/details/gqsrgjdpc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.sjlbkw.cn/Article/details/gmzcxbnjb.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fktsv.cn/Article/details/gsovgjwkd.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.epnwcf.com/Article/details/ghgkgicdr.sHtML

[S03] C：读入整数
来源：http://wap.tarul.cn/Article/details/gmezcogfr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.yfazqb.com/Article/details/gydjmregn.sHtML

[S04] C：字符串复制
来源：http://read.share.bbcook.cn/Article/details/gntdnrhca.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.vehdjk.com/Article/details/gkrjrnlfp.sHtML

[S05] C：字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gdakdhqzv.sHtML

strlen(s)
来源：http://wap.sjlbkw.cn/Article/details/gfvoszspw.sHtML

[S06] C：字符串比较
来源：http://www.share.fktsv.cn/Article/details/gkyyfhbst.sHtML

strcmp(a, b) == 0
来源：http://baike.bbcook.cn/Article/details/gmojnnwck.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.yfazqb.com/Article/details/gwolmtmca.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.vehdjk.com/Article/details/gocfsuzbq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fktsv.cn/Article/details/gfjgtwqxk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.sjlbkw.cn/Article/details/gtlcmgjcf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.epnwcf.com/Article/details/gcwkezmhw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.epnwcf.com/Article/details/gemikzcxz.sHtML

[S10] C：指针与解引用
来源：http://m.share.fktsv.cn/Article/details/gjmfrpafn.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/ghzzggzau.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gqtcuijnz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.sjlbkw.cn/Article/details/gkggpxlja.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fktsv.cn/Article/details/gwijezccv.sHtML

fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gkppgurrg.sHtML

[S12] C：写文件
来源：http://blog.sjlbkw.cn/Article/details/gbhnojpyd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/glebhbbig.sHtML

[S13] C：宏定义
来源：http://www.share.yfazqb.com/Article/details/grkiiekkh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/gmfdvwtyb.sHtML

[S14] C：枚举
来源：http://www.share.fktsv.cn/Article/details/gdgxgqntb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.tarul.cn/Article/details/gjobodumf.sHtML

[S15] C：类型转换
来源：http://baike.fktsv.cn/Article/details/gsminddrr.sHtML

(double) a / b
来源：http://www.blog.bbcook.cn/Article/details/gjugjxfua.sHtML

[S16] C：位操作置位
来源：http://www.share.epnwcf.com/Article/details/gppaljlyw.sHtML

x |= (1 << 3);
来源：http://www.m.share.yfazqb.com/Article/details/gtcdizxcm.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gdsgeevdd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.yfazqb.com/Article/details/gmqyxwxte.sHtML

[S18] C：命令行参数
来源：http://blog.yfazqb.com/Article/details/geicbhrxj.sHtML

int main(int argc, char **argv)
来源：http://www.share.sjlbkw.cn/Article/details/gwrbcykei.sHtML

[S19] C：快速排序
来源：http://mobile.vehdjk.com/Article/details/gryzspwxz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gjhlrswsc.sHtML

[S20] C：二分查找
来源：http://baike.epnwcf.com/Article/details/gszxfdldf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gqyueifpn.sHtML

[S21] C：字符类别判断
来源：http://m.share.fktsv.cn/Article/details/gzqbdiftn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fktsv.cn/Article/details/gkwcjobcq.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/gkaaxleuc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.epnwcf.com/Article/details/grxuzohnr.sHtML

[S23] C：随机数
来源：http://blog.yfazqb.com/Article/details/gtgpbcohd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.bbcook.cn/Article/details/gyhmjyfpn.sHtML

[S24] C：获取本地时间
来源：http://www.blog.epnwcf.com/Article/details/ggohacorz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.bbcook.cn/Article/details/ggoberiva.sHtML

[S25] C：内存拷贝
来源：http://baike.fktsv.cn/Article/details/gfqpjyznx.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gjjbxhwbh.sHtML

[S26] C：内存清零
来源：http://www.blog.tarul.cn/Article/details/gltdedbou.sHtML

memset(a, 0, sizeof a);
来源：http://baike.bbcook.cn/Article/details/gyugpqdsk.sHtML

[S27] C：定义常量
来源：http://mobile.tarul.cn/Article/details/gqpohpklu.sHtML

const double PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gdhfcohfd.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gigbndxse.sHtML

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/giqdahvxi.sHtML

[S29] C：变参函数
来源：http://read.share.epnwcf.com/Article/details/ggxzzkpav.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.sjlbkw.cn/Article/details/gaahzctlz.sHtML

[S30] C：头文件保护
来源：http://www.share.vehdjk.com/Article/details/grupltdne.sHtML

#ifndef X_H
来源：http://3g.fktsv.cn/Article/details/gsggqgdek.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gbofyxeex.sHtML

#endif
来源：http://baike.yfazqb.com/Article/details/gxyqglgdx.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/gslzcvphr.sHtML

#include <iostream>
来源：http://mobile.epnwcf.com/Article/details/gjbulcitc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fktsv.cn/Article/details/giepepspe.sHtML

[S32] C++：字符串
来源：http://blog.fktsv.cn/Article/details/grwbhhyfo.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/ghqhhohfq.sHtML

[S33] C++：vector 增删
来源：http://wap.yfazqb.com/Article/details/gyfznkdei.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.epnwcf.com/Article/details/gptsmchvd.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.sjlbkw.cn/Article/details/gpotjymgx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fktsv.cn/Article/details/gpsmxybdn.sHtML

[S35] C++：map
来源：http://www.blog.tarul.cn/Article/details/gxcmekmeb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gvyfportp.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/giylddsrp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gjroxzdfy.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/gmbqwqage.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.yfazqb.com/Article/details/gpfixzlvz.sHtML

[S38] C++：排序
来源：http://www.m.share.tarul.cn/Article/details/gwinqevqw.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.vehdjk.com/Article/details/gsuohlsyd.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/givoavnij.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.vehdjk.com/Article/details/gheycxjcg.sHtML

[S40] C++：查找元素
来源：http://www.m.share.yfazqb.com/Article/details/gxpsghfmw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.sjlbkw.cn/Article/details/gfangccjk.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gllynsves.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.sjlbkw.cn/Article/details/gzsjycjgs.sHtML

[S42] C++：继承与虚函数
来源：http://blog.bbcook.cn/Article/details/gpdqnojgp.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.bbcook.cn/Article/details/gynhjnbni.sHtML

[S43] C++：智能指针
来源：http://www.m.share.tarul.cn/Article/details/gcktqttpo.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.tarul.cn/Article/details/gokytoewc.sHtML

[S44] C++：引用传参
来源：http://wap.vehdjk.com/Article/details/gsavwyjln.sHtML

void inc(int &x) { ++x; }
来源：http://3g.tarul.cn/Article/details/gutwpqqnj.sHtML

[S45] C++：lambda
来源：http://wap.bbcook.cn/Article/details/gigfcykqd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.bbcook.cn/Article/details/gdmgduyoe.sHtML

[S46] C++：函数模板
来源：http://wap.vehdjk.com/Article/details/gmdnobutv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.tarul.cn/Article/details/glnvvtzii.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.bbcook.cn/Article/details/gaoikpyqe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.vehdjk.com/Article/details/gbiqowcur.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gfoogzcwc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.sjlbkw.cn/Article/details/gktgevcfv.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.tarul.cn/Article/details/giwlpslvy.sHtML

[S49] C++：写文件
来源：http://baike.yfazqb.com/Article/details/gcpvlrlty.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.sjlbkw.cn/Article/details/godnuosfp.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/gwaytciom.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gihibuctm.sHtML

[S51] C++：显式类型转换
来源：http://3g.sjlbkw.cn/Article/details/gniwernlt.sHtML

static_cast<double>(a) / b
来源：http://www.share.vehdjk.com/Article/details/gldiwpqkr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.vehdjk.com/Article/details/gtcrsuspi.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.yfazqb.com/Article/details/goilzxetp.sHtML

[S53] C++：移动语义
来源：http://read.share.bbcook.cn/Article/details/gfoqbizhf.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.yfazqb.com/Article/details/gwuqjkzdl.sHtML

[S54] C++：异常处理
来源：http://3g.epnwcf.com/Article/details/gsnfenquu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.epnwcf.com/Article/details/gcipfbsqx.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.vehdjk.com/Article/details/gyhoegvtu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.yfazqb.com/Article/details/gszqpgavv.sHtML

[S56] C++：optional
来源：http://read.share.yfazqb.com/Article/details/gsiyxuldb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.bbcook.cn/Article/details/gipbwpwxi.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/ggbiwwniv.sHtML

constexpr int N = 10;
来源：http://mobile.bbcook.cn/Article/details/gkubyitee.sHtML

[S58] C++：命名空间
来源：http://m.share.fktsv.cn/Article/details/gyjpzunla.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.sjlbkw.cn/Article/details/gzbaupnvc.sHtML

[S59] C++：静态断言
来源：http://3g.tarul.cn/Article/details/gaismigfh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.yfazqb.com/Article/details/ggyrddork.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gcwuxuail.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.tarul.cn/Article/details/gytttgnll.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gcfrbzlsn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.sjlbkw.cn/Article/details/gookxzpiy.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmlgfjqvb.sHtML

[T01] Kotlin：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gfqkojxfa.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/ghddfdzxb.sHtML

[T02] Kotlin：变量
来源：http://www.share.tarul.cn/Article/details/gyzpowapm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.epnwcf.com/Article/details/gwvgnestj.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.epnwcf.com/Article/details/gihcpdopi.sHtML

"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gubzdodre.sHtML

[T04] Kotlin：空安全
来源：http://3g.fktsv.cn/Article/details/grwhvbpkv.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/gpzitleft.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.bbcook.cn/Article/details/gziekzmdl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.sjlbkw.cn/Article/details/galbzvzrl.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fktsv.cn/Article/details/ggbczyvzz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gwelganrv.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.epnwcf.com/Article/details/gsralxhje.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.epnwcf.com/Article/details/gmegolnea.sHtML

[T08] Kotlin：数据类
来源：http://blog.vehdjk.com/Article/details/ghlcnyyul.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyvkggqe.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.tarul.cn/Article/details/gfxwgpuek.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.yfazqb.com/Article/details/genhfocqp.sHtML

[T10] Kotlin：默认参数
来源：http://wap.vehdjk.com/Article/details/gwegolrjp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/glyshqnah.sHtML

[T11] Kotlin：协程
来源：http://read.share.epnwcf.com/Article/details/gandqswqw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.tarul.cn/Article/details/gclrtlvky.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fktsv.cn/Article/details/gqzxdjsqk.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gietydpyc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.tarul.cn/Article/details/gvoyhigay.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.bbcook.cn/Article/details/goxhzfzps.sHtML

[T14] Kotlin：循环
来源：http://wap.sjlbkw.cn/Article/details/gbxcugdou.sHtML

for (i in 1..10) println(i)
来源：http://3g.epnwcf.com/Article/details/guiaksuhz.sHtML

[T15] Kotlin：接口
来源：http://baike.bbcook.cn/Article/details/gzjursohg.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fktsv.cn/Article/details/gawinokex.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gxhhhztcw.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gopilrfts.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fktsv.cn/Article/details/gsngikdqm.sHtML

var a = 1;  let b = 2
来源：http://wap.bbcook.cn/Article/details/gbccevwdc.sHtML

[T18] Swift：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gdiijlkvy.sHtML

"值: \(b)"
来源：http://baike.sjlbkw.cn/Article/details/gnkeddmul.sHtML

[T19] Swift：可选绑定
来源：http://blog.fktsv.cn/Article/details/gbxgmaxgm.sHtML

if let n = opt { print(n) }
来源：http://wap.bbcook.cn/Article/details/gwbvgbote.sHtML

[T20] Swift：数组操作
来源：http://m.share.sjlbkw.cn/Article/details/gkwkvxmtm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fktsv.cn/Article/details/gncqlugxf.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/gxigdgauh.sHtML

for x in a { print(x) }
来源：http://www.share.yfazqb.com/Article/details/gzovitwau.sHtML

[T22] Swift：字典
来源：http://www.m.share.epnwcf.com/Article/details/gwhniubko.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.bbcook.cn/Article/details/gxifrfynz.sHtML

[T23] Swift：函数
来源：http://www.m.share.yfazqb.com/Article/details/gkqtsjytr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.sjlbkw.cn/Article/details/gddmzcqla.sHtML

[T24] Swift：闭包
来源：http://baike.yfazqb.com/Article/details/gdhxpauib.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fktsv.cn/Article/details/gjubaaoex.sHtML

[T25] Swift：结构体
来源：http://mobile.epnwcf.com/Article/details/gchdxmfml.sHtML

struct P { var x: Int }
来源：http://blog.sjlbkw.cn/Article/details/gebtakfku.sHtML

[T26] Swift：类与重写
来源：http://wap.bbcook.cn/Article/details/gbxefsvix.sHtML

class A: Base { override func f() {} }
来源：http://www.share.bbcook.cn/Article/details/gwvncbswl.sHtML

[T27] Swift：错误处理
来源：http://www.share.vehdjk.com/Article/details/guwqfmdda.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.yfazqb.com/Article/details/gbbhngece.sHtML

[T28] Swift：枚举
来源：http://mobile.tarul.cn/Article/details/ggdayqjxw.sHtML

enum Color { case red, green }
来源：http://m.share.fktsv.cn/Article/details/gmtqxanae.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.epnwcf.com/Article/details/gozzobtjv.sHtML

guard let x = opt else { return }
来源：http://baike.yfazqb.com/Article/details/guthcqhjq.sHtML

[T30] Swift：协议
来源：http://www.m.share.vehdjk.com/Article/details/gqfrmxrmk.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.yfazqb.com/Article/details/gdseluitw.sHtML

[T31] Lua：Hello World
来源：http://read.share.yfazqb.com/Article/details/gplogbixh.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/ghwulothn.sHtML

[T32] Lua：局部变量
来源：http://m.share.bbcook.cn/Article/details/gjeyfgfer.sHtML

local a = 1
来源：http://blog.vehdjk.com/Article/details/gvweidgwl.sHtML

[T33] Lua：表（数组）
来源：http://3g.yfazqb.com/Article/details/gnlberngy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.sjlbkw.cn/Article/details/gwlaeectq.sHtML

[T34] Lua：遍历表
来源：http://www.blog.bbcook.cn/Article/details/gxpoqihiu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.sjlbkw.cn/Article/details/gsdimomlo.sHtML

[T35] Lua：字典表
来源：http://mobile.sjlbkw.cn/Article/details/grusxnwfa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/grgiguavw.sHtML

[T36] Lua：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gvcjvugai.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/gndsiyhpw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/glnlhmxwy.sHtML

"a" .. "b"
来源：http://baike.bbcook.cn/Article/details/gqsiiyrgv.sHtML

[T38] Lua：条件
来源：http://3g.tarul.cn/Article/details/gqzntjetq.sHtML

if x > 0 then print("正") end
来源：http://mobile.epnwcf.com/Article/details/ggawkhrzi.sHtML

[T39] Lua：模式匹配
来源：http://read.share.sjlbkw.cn/Article/details/gambsfsif.sHtML

string.find(s, "%d+")
来源：http://mobile.sjlbkw.cn/Article/details/gaietcsru.sHtML

[T40] Lua：元表
来源：http://wap.sjlbkw.cn/Article/details/gvhjfiwjc.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.vehdjk.com/Article/details/galnwrvgo.sHtML

[T41] Perl：Hello World
来源：http://www.blog.vehdjk.com/Article/details/ghzqzyvrd.sHtML

print "Hello\n";
来源：http://3g.vehdjk.com/Article/details/gmcseuewu.sHtML

[T42] Perl：变量类型
来源：http://baike.epnwcf.com/Article/details/gseuzluog.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.bbcook.cn/Article/details/gmsjshncc.sHtML

[T43] Perl：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gwvkhoijw.sHtML

"值: $a"
来源：http://www.blog.vehdjk.com/Article/details/gbpnqxukx.sHtML

[T44] Perl：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gtswoespc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.vehdjk.com/Article/details/glpipyrtb.sHtML

[T45] Perl：数组遍历
来源：http://3g.vehdjk.com/Article/details/gkbylmgwo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.bbcook.cn/Article/details/gzxpbtfoi.sHtML

[T46] Perl：哈希操作
来源：http://m.share.tarul.cn/Article/details/glotnfuwa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.yfazqb.com/Article/details/gtmsauill.sHtML

[T47] Perl：正则捕获
来源：http://www.share.vehdjk.com/Article/details/glkxrpjzn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.epnwcf.com/Article/details/gbfkoktjg.sHtML

[T48] Perl：正则替换
来源：http://m.share.yfazqb.com/Article/details/gihklqncn.sHtML

$s =~ s/old/new/g;
来源：http://3g.epnwcf.com/Article/details/glvxyflql.sHtML

[T49] Perl：函数
来源：http://wap.fktsv.cn/Article/details/gbzqmiayv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gkfhxvcxk.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gatcmdjgt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.epnwcf.com/Article/details/gwrisydlv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.bbcook.cn/Article/details/gbwxjixsb.sHtML

[T51] Scala：Hello World
来源：http://3g.bbcook.cn/Article/details/gvjbvxhqp.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gbnfoygkv.sHtML

[T52] Scala：变量
来源：http://m.share.vehdjk.com/Article/details/gywrscwqa.sHtML

val a = 1;  var b = 2
来源：http://mobile.epnwcf.com/Article/details/gbxxdvycd.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gqruuende.sHtML

s"值: $b"
来源：http://www.share.yfazqb.com/Article/details/gwdlkqnlt.sHtML

[T54] Scala：集合映射
来源：http://read.share.yfazqb.com/Article/details/gxvkeedmd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.yfazqb.com/Article/details/gnorjhrrx.sHtML

[T55] Scala：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gbazfygdt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/gltnweywp.sHtML

[T56] Scala：样例类
来源：http://blog.tarul.cn/Article/details/gsgolyhqu.sHtML


<!-- 参考信息 -->