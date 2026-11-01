代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fktsv.cn/Article/details/grwgyrmry.sHtML

[R52] 统计行数
来源：http://www.share.sjlbkw.cn/Article/details/gtwxgbjli.sHtML

wc -l a.txt
来源：http://m.share.yfazqb.com/Article/details/grqeakadz.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.yfazqb.com/Article/details/gvuqqthhb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.vehdjk.com/Article/details/gyuytthvx.sHtML

[R54] 比较两个文件
来源：http://www.blog.yfazqb.com/Article/details/gzgfqcygw.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/gmurhtnew.sHtML

[R55] 压缩与解压
来源：http://mobile.epnwcf.com/Article/details/glfzyumqs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmnxsfiw.sHtML

[R56] 远程拷贝
来源：http://www.share.fktsv.cn/Article/details/gdxhordtn.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/gaflkvukz.sHtML

[R57] 远程执行命令
来源：http://baike.yfazqb.com/Article/details/gtadcenzr.sHtML

ssh user@host 'uptime'
来源：http://3g.vehdjk.com/Article/details/gpwdfrvan.sHtML

[R58] 下载文件
来源：http://www.m.share.fktsv.cn/Article/details/gbhjeminy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.bbcook.cn/Article/details/gzgrnouvx.sHtML

[R59] 发 POST JSON
来源：http://blog.sjlbkw.cn/Article/details/gioxezust.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.yfazqb.com/Article/details/gtqochgxx.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gmtdvcnst.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.vehdjk.com/Article/details/gutdrbiby.sHtML

[R61] 磁盘占用
来源：http://www.share.vehdjk.com/Article/details/gjruqudch.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/gbrawurbp.sHtML

[R62] 找最占空间的文件
来源：http://www.share.epnwcf.com/Article/details/guujbonhw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.epnwcf.com/Article/details/gicjhibei.sHtML

[R63] 内存与进程
来源：http://www.share.vehdjk.com/Article/details/gopvueaoo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.sjlbkw.cn/Article/details/gtwtbqnya.sHtML

[R64] 结束进程
来源：http://www.blog.vehdjk.com/Article/details/gtqohhdab.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/gzwudzhqg.sHtML

[R65] 查看端口占用
来源：http://read.share.epnwcf.com/Article/details/gyfbdsvqd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/gbhlvlvin.sHtML

[R66] 定时任务
来源：http://read.share.sjlbkw.cn/Article/details/ghqhqojre.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.vehdjk.com/Article/details/giplocldy.sHtML

[R67] 生成随机十六进制串
来源：http://blog.vehdjk.com/Article/details/gfsfstqdu.sHtML

openssl rand -hex 16
来源：http://www.blog.vehdjk.com/Article/details/gzufoxvwg.sHtML

[R68] 计算文件校验值
来源：http://www.share.epnwcf.com/Article/details/gelulxkat.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.bbcook.cn/Article/details/gtuvmktng.sHtML

[R69] 生成随机密码
来源：http://mobile.epnwcf.com/Article/details/gyrtwpiro.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fktsv.cn/Article/details/gqaepsvko.sHtML

[R70] 时间戳与互转
来源：http://www.blog.sjlbkw.cn/Article/details/grcwvtksq.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fktsv.cn/Article/details/gfuchgqrv.sHtML

[R71] 日期格式化
来源：http://blog.epnwcf.com/Article/details/goujmgojr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.sjlbkw.cn/Article/details/gsyclnark.sHtML

[R72] 等待端口就绪
来源：http://mobile.epnwcf.com/Article/details/gqdaqccnu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gngwhuyel.sHtML

[R73] 分割大日志
来源：http://www.share.bbcook.cn/Article/details/ggigpeghd.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/gdzkgnncw.sHtML

[R74] 批量重命名
来源：http://read.share.vehdjk.com/Article/details/gtmfoiyfz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.sjlbkw.cn/Article/details/gjxjdguuy.sHtML

[R75] 导出环境变量
来源：http://m.share.fktsv.cn/Article/details/geninhvxx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fktsv.cn/Article/details/gxmnclxrg.sHtML

[R76] 使用临时文件
来源：http://baike.fktsv.cn/Article/details/gghhtlfqd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gapcsqpun.sHtML

[R77] 读取用户输入
来源：http://www.share.epnwcf.com/Article/details/gedgllntl.sHtML

read -rp "请输入: " ans
来源：http://read.share.tarul.cn/Article/details/gtzjokcse.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/ghsafkdwx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.tarul.cn/Article/details/gbyejerks.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fktsv.cn/Article/details/gqvnsgmwn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.bbcook.cn/Article/details/ghqrlcsvo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.vehdjk.com/Article/details/gcpeewqii.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gdojezbqc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gpuicpkgm.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/gxyrvaxaq.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gabdakysz.sHtML

[S01] C：Hello World
来源：http://read.share.tarul.cn/Article/details/guhfylmld.sHtML

#include <stdio.h>
来源：http://m.share.tarul.cn/Article/details/gbcdxesoi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.epnwcf.com/Article/details/ggijehrhv.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gpioxlxat.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.vehdjk.com/Article/details/gelykyzzd.sHtML

[S03] C：读入整数
来源：http://www.m.share.epnwcf.com/Article/details/gtqwjiibh.sHtML

int x; scanf("%d", &x);
来源：http://blog.bbcook.cn/Article/details/gpwysachm.sHtML

[S04] C：字符串复制
来源：http://www.share.yfazqb.com/Article/details/gphewfszh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fktsv.cn/Article/details/gehvhcjlb.sHtML

[S05] C：字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gwqfjuycq.sHtML

strlen(s)
来源：http://www.share.tarul.cn/Article/details/gufbelnqc.sHtML

[S06] C：字符串比较
来源：http://baike.bbcook.cn/Article/details/gdokrmsxw.sHtML

strcmp(a, b) == 0
来源：http://baike.tarul.cn/Article/details/gmmikxckf.sHtML

[S07] C：数组遍历求和
来源：http://blog.epnwcf.com/Article/details/gmlrgayze.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.bbcook.cn/Article/details/gcqjydjrc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.vehdjk.com/Article/details/gemjxctff.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.vehdjk.com/Article/details/gauhbgwzz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.sjlbkw.cn/Article/details/gswkfnzgh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.epnwcf.com/Article/details/gvipvzrty.sHtML

[S10] C：指针与解引用
来源：http://m.share.bbcook.cn/Article/details/gghtjhico.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fktsv.cn/Article/details/gkunjjbbx.sHtML

[S11] C：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gckfdkvdx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.epnwcf.com/Article/details/gbwixiaqf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.epnwcf.com/Article/details/gherttfgs.sHtML

fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gdqicldhg.sHtML

[S12] C：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gvtxwiwsp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.tarul.cn/Article/details/gnxxqmeeq.sHtML

[S13] C：宏定义
来源：http://baike.fktsv.cn/Article/details/golhpvmvq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fktsv.cn/Article/details/gksyaxirp.sHtML

[S14] C：枚举
来源：http://baike.yfazqb.com/Article/details/ggnvesnth.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.vehdjk.com/Article/details/gwzdsxomg.sHtML

[S15] C：类型转换
来源：http://blog.fktsv.cn/Article/details/gcqrfqzju.sHtML

(double) a / b
来源：http://baike.yfazqb.com/Article/details/guptqkcqj.sHtML

[S16] C：位操作置位
来源：http://mobile.tarul.cn/Article/details/ghowhztrd.sHtML

x |= (1 << 3);
来源：http://www.blog.epnwcf.com/Article/details/gyhlpmfjv.sHtML

[S17] C：安全拼接字符串
来源：http://wap.bbcook.cn/Article/details/gpyzfjlal.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.sjlbkw.cn/Article/details/gtrrddoyf.sHtML

[S18] C：命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gxhyxpbgh.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gcobgciwp.sHtML

[S19] C：快速排序
来源：http://blog.vehdjk.com/Article/details/ggqpjnsyi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gruiwzzva.sHtML

[S20] C：二分查找
来源：http://wap.yfazqb.com/Article/details/gcrlgtsut.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gncfadswq.sHtML

[S21] C：字符类别判断
来源：http://baike.tarul.cn/Article/details/gefdtlhuf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gkbwvqcch.sHtML

[S22] C：字符串转数字
来源：http://baike.sjlbkw.cn/Article/details/gdchpwdki.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.sjlbkw.cn/Article/details/gquhtgwsw.sHtML

[S23] C：随机数
来源：http://wap.sjlbkw.cn/Article/details/gbnqhebsp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.sjlbkw.cn/Article/details/gmceyhywc.sHtML

[S24] C：获取本地时间
来源：http://m.share.tarul.cn/Article/details/ggvkfbuxe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.vehdjk.com/Article/details/gcibbicaj.sHtML

[S25] C：内存拷贝
来源：http://m.share.vehdjk.com/Article/details/gxugxfska.sHtML

memcpy(dst, src, n);
来源：http://www.share.vehdjk.com/Article/details/gnxwsofue.sHtML

[S26] C：内存清零
来源：http://blog.sjlbkw.cn/Article/details/gcmekjoux.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.vehdjk.com/Article/details/gxpipcang.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/gaqxrrdcx.sHtML

const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gmovsakgs.sHtML

[S28] C：静态变量
来源：http://read.share.tarul.cn/Article/details/gshaejpon.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/gzachzktu.sHtML

[S29] C：变参函数
来源：http://blog.bbcook.cn/Article/details/gpcrnxixf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/gcoktoiew.sHtML

[S30] C：头文件保护
来源：http://read.share.fktsv.cn/Article/details/gmrydejes.sHtML

#ifndef X_H
来源：http://m.share.epnwcf.com/Article/details/gkemoqgbk.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gfosxbonf.sHtML

#endif
来源：http://blog.epnwcf.com/Article/details/gmlyhpyon.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/grjxsgkle.sHtML

#include <iostream>
来源：http://wap.yfazqb.com/Article/details/gexjlhvot.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.tarul.cn/Article/details/gfmlgogpw.sHtML

[S32] C++：字符串
来源：http://blog.sjlbkw.cn/Article/details/ganbxqcdg.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.yfazqb.com/Article/details/gyvxdhbae.sHtML

[S33] C++：vector 增删
来源：http://m.share.tarul.cn/Article/details/gkuvnosjr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/gigvtijlt.sHtML

[S34] C++：遍历 vector
来源：http://blog.yfazqb.com/Article/details/gyawncpjl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.vehdjk.com/Article/details/gdgtjgufa.sHtML

[S35] C++：map
来源：http://read.share.epnwcf.com/Article/details/gttybevix.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gmfnkuszf.sHtML

[S36] C++：unordered_map
来源：http://www.blog.tarul.cn/Article/details/gejdivayi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gtqmwbpzf.sHtML

[S37] C++：set
来源：http://read.share.yfazqb.com/Article/details/gxrsjgrbe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.yfazqb.com/Article/details/gsfmvgfbk.sHtML

[S38] C++：排序
来源：http://www.share.bbcook.cn/Article/details/gxyreduwy.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fktsv.cn/Article/details/gauyzqydr.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.tarul.cn/Article/details/gqvmynfxm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.tarul.cn/Article/details/gorgbkigh.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fktsv.cn/Article/details/gvfxowslu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fktsv.cn/Article/details/griivmozu.sHtML

[S41] C++：类与构造函数
来源：http://3g.epnwcf.com/Article/details/griwxmxde.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.vehdjk.com/Article/details/gtbagzopt.sHtML

[S42] C++：继承与虚函数
来源：http://wap.yfazqb.com/Article/details/ghynkuufr.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.yfazqb.com/Article/details/ggrjiuioj.sHtML

[S43] C++：智能指针
来源：http://mobile.sjlbkw.cn/Article/details/gqezanjac.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/gxgnrpkdz.sHtML

[S44] C++：引用传参
来源：http://blog.yfazqb.com/Article/details/gzojknfzz.sHtML

void inc(int &x) { ++x; }
来源：http://wap.bbcook.cn/Article/details/gxielvbqa.sHtML

[S45] C++：lambda
来源：http://m.share.sjlbkw.cn/Article/details/gerayytbt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/gxmdwxosf.sHtML

[S46] C++：函数模板
来源：http://www.share.epnwcf.com/Article/details/gtlfkjvca.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.bbcook.cn/Article/details/gduaoyxrh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.tarul.cn/Article/details/gklldbpnz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/gapetmaoe.sHtML

[S48] C++：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gyzkkngeg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.yfazqb.com/Article/details/gwhmwqskd.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.yfazqb.com/Article/details/gmoditcyx.sHtML

[S49] C++：写文件
来源：http://3g.vehdjk.com/Article/details/gdzxkvmec.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.epnwcf.com/Article/details/gnsbuhvyt.sHtML

[S50] C++：格式化数字
来源：http://mobile.epnwcf.com/Article/details/gltkjrrlo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gnycubblc.sHtML

[S51] C++：显式类型转换
来源：http://blog.sjlbkw.cn/Article/details/gonbecyvc.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/gdawljkrq.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.epnwcf.com/Article/details/gombylbcv.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.epnwcf.com/Article/details/glxtxisxo.sHtML

[S53] C++：移动语义
来源：http://www.blog.bbcook.cn/Article/details/gszselwrv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.vehdjk.com/Article/details/gtvgogkux.sHtML

[S54] C++：异常处理
来源：http://wap.tarul.cn/Article/details/gogsyjzdv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.sjlbkw.cn/Article/details/gwftoprcm.sHtML

[S55] C++：结构化绑定
来源：http://wap.fktsv.cn/Article/details/ghwrgzccl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.epnwcf.com/Article/details/gbmjuyalw.sHtML

[S56] C++：optional
来源：http://3g.vehdjk.com/Article/details/ggxomsskt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/gxooqpurl.sHtML

[S57] C++：编译期常量
来源：http://www.share.tarul.cn/Article/details/gpnjaskzb.sHtML

constexpr int N = 10;
来源：http://m.share.yfazqb.com/Article/details/gdezdyove.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/gktbbcara.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.bbcook.cn/Article/details/gbtrlchjf.sHtML

[S59] C++：静态断言
来源：http://www.blog.bbcook.cn/Article/details/gnkajkwjw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.vehdjk.com/Article/details/gwvodhnzm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.tarul.cn/Article/details/goyawedea.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/gsfclyolh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/grvczpmoq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.sjlbkw.cn/Article/details/gynpaggih.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grzcfjgta.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fktsv.cn/Article/details/gsvoxfnhy.sHtML

println("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gwpltncny.sHtML

[T02] Kotlin：变量
来源：http://baike.fktsv.cn/Article/details/gfkpdvxsx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.tarul.cn/Article/details/gqcxwpkhj.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.vehdjk.com/Article/details/gwslynlkq.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/gwqvrummv.sHtML

[T04] Kotlin：空安全
来源：http://baike.epnwcf.com/Article/details/gcffreaap.sHtML

val n: String? = null;  n?.length
来源：http://m.share.tarul.cn/Article/details/gfxtfztcg.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.vehdjk.com/Article/details/giyfyavag.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzqpyxdh.sHtML

[T06] Kotlin：集合映射
来源：http://wap.bbcook.cn/Article/details/gxlomsuso.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.bbcook.cn/Article/details/gepzqjort.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.bbcook.cn/Article/details/gnvryobvd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.bbcook.cn/Article/details/gccqfponn.sHtML

[T08] Kotlin：数据类
来源：http://read.share.bbcook.cn/Article/details/gxycdbhmn.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.bbcook.cn/Article/details/gmzhwfxlt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.tarul.cn/Article/details/gtagfviuy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.bbcook.cn/Article/details/gujewxmkw.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.vehdjk.com/Article/details/giwyqphbk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.yfazqb.com/Article/details/gjiksimcw.sHtML

[T11] Kotlin：协程
来源：http://m.share.epnwcf.com/Article/details/gemlystiu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fktsv.cn/Article/details/gdrpodgip.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fktsv.cn/Article/details/gslwznkpl.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.yfazqb.com/Article/details/ggkwzvmnp.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.epnwcf.com/Article/details/grttzsvee.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.yfazqb.com/Article/details/gfggvntbo.sHtML

[T14] Kotlin：循环
来源：http://baike.sjlbkw.cn/Article/details/gnvhicoyc.sHtML

for (i in 1..10) println(i)
来源：http://baike.bbcook.cn/Article/details/gxeciuiwp.sHtML

[T15] Kotlin：接口
来源：http://mobile.fktsv.cn/Article/details/ggbvhjfbg.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/gvxxtmwby.sHtML

[T16] Swift：Hello World
来源：http://read.share.vehdjk.com/Article/details/gvaxtummu.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gwkrhvidr.sHtML

[T17] Swift：变量与常量
来源：http://wap.tarul.cn/Article/details/guiqlgejc.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gosepcxff.sHtML

[T18] Swift：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gsrnpcvgw.sHtML

"值: \(b)"
来源：http://3g.sjlbkw.cn/Article/details/gectofcay.sHtML

[T19] Swift：可选绑定
来源：http://m.share.epnwcf.com/Article/details/gmyykwtzf.sHtML

if let n = opt { print(n) }
来源：http://www.share.yfazqb.com/Article/details/gvetpfcsv.sHtML

[T20] Swift：数组操作
来源：http://www.blog.tarul.cn/Article/details/gwshpkpjk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.bbcook.cn/Article/details/ghowjghzy.sHtML

[T21] Swift：遍历
来源：http://wap.vehdjk.com/Article/details/ghwhicljk.sHtML

for x in a { print(x) }
来源：http://baike.vehdjk.com/Article/details/gaotnirzr.sHtML

[T22] Swift：字典
来源：http://m.share.fktsv.cn/Article/details/gnremaukh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.epnwcf.com/Article/details/geskowqpz.sHtML

[T23] Swift：函数
来源：http://m.share.bbcook.cn/Article/details/glravlnlu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.epnwcf.com/Article/details/ghjnuxnif.sHtML

[T24] Swift：闭包
来源：http://m.share.bbcook.cn/Article/details/gxcbmiaog.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.yfazqb.com/Article/details/gunemhdfj.sHtML

[T25] Swift：结构体
来源：http://www.blog.tarul.cn/Article/details/gtwtmdxes.sHtML

struct P { var x: Int }
来源：http://www.m.share.tarul.cn/Article/details/gufqeadyj.sHtML

[T26] Swift：类与重写
来源：http://m.share.vehdjk.com/Article/details/ghmnpbvpv.sHtML

class A: Base { override func f() {} }
来源：http://blog.bbcook.cn/Article/details/gjgtmkbzj.sHtML

[T27] Swift：错误处理
来源：http://blog.epnwcf.com/Article/details/gtbuhlffy.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.tarul.cn/Article/details/gdohaqrhf.sHtML

[T28] Swift：枚举
来源：http://www.blog.fktsv.cn/Article/details/gfgyvvdqg.sHtML

enum Color { case red, green }
来源：http://www.blog.fktsv.cn/Article/details/gmowjbqke.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.bbcook.cn/Article/details/gdskvdsma.sHtML

guard let x = opt else { return }
来源：http://www.share.tarul.cn/Article/details/gintudgyv.sHtML

[T30] Swift：协议
来源：http://wap.tarul.cn/Article/details/gawtvcvvb.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.tarul.cn/Article/details/gzprgveuh.sHtML

[T31] Lua：Hello World
来源：http://wap.vehdjk.com/Article/details/gfocrdofi.sHtML

print("Hello")
来源：http://blog.epnwcf.com/Article/details/geiagquvu.sHtML

[T32] Lua：局部变量
来源：http://blog.epnwcf.com/Article/details/guxoajljl.sHtML

local a = 1
来源：http://baike.epnwcf.com/Article/details/glfvzcoct.sHtML

[T33] Lua：表（数组）
来源：http://blog.bbcook.cn/Article/details/ghjcojzgc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.bbcook.cn/Article/details/gvoaigbmv.sHtML

[T34] Lua：遍历表
来源：http://baike.sjlbkw.cn/Article/details/gqahnwdhw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.sjlbkw.cn/Article/details/gzarvgwxs.sHtML

[T35] Lua：字典表
来源：http://baike.fktsv.cn/Article/details/ggaghpsfg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.yfazqb.com/Article/details/gvmghotai.sHtML

[T36] Lua：函数
来源：http://baike.bbcook.cn/Article/details/gdoibouqw.sHtML

function add(a, b) return a + b end
来源：http://m.share.sjlbkw.cn/Article/details/gsjwiuajq.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gbzwxcspx.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/gezjvffin.sHtML

[T38] Lua：条件
来源：http://m.share.fktsv.cn/Article/details/gnmzyaqdx.sHtML

if x > 0 then print("正") end
来源：http://www.share.fktsv.cn/Article/details/gnyiirqgi.sHtML

[T39] Lua：模式匹配
来源：http://baike.tarul.cn/Article/details/gqwcbjolt.sHtML

string.find(s, "%d+")
来源：http://blog.bbcook.cn/Article/details/gqbsosyqm.sHtML

[T40] Lua：元表
来源：http://www.share.epnwcf.com/Article/details/gdueihtfx.sHtML

setmetatable({}, { __index = base })
来源：http://3g.epnwcf.com/Article/details/gtbhvsapa.sHtML

[T41] Perl：Hello World
来源：http://baike.vehdjk.com/Article/details/gbfkqwvsu.sHtML

print "Hello\n";
来源：http://www.blog.yfazqb.com/Article/details/gvjmorwul.sHtML

[T42] Perl：变量类型
来源：http://blog.vehdjk.com/Article/details/galotiewu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.yfazqb.com/Article/details/gggesphhc.sHtML

[T43] Perl：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gqfhjizxe.sHtML

"值: $a"
来源：http://read.share.tarul.cn/Article/details/geglotpou.sHtML

[T44] Perl：条件
来源：http://blog.bbcook.cn/Article/details/gsrchzwjn.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.epnwcf.com/Article/details/gezjjdnkl.sHtML

[T45] Perl：数组遍历
来源：http://blog.tarul.cn/Article/details/gkbubvrjl.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.epnwcf.com/Article/details/gjrkcsqus.sHtML

[T46] Perl：哈希操作
来源：http://wap.yfazqb.com/Article/details/gwmwvevkk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.sjlbkw.cn/Article/details/gaklqigkc.sHtML

[T47] Perl：正则捕获
来源：http://baike.tarul.cn/Article/details/ghzgwdafp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.tarul.cn/Article/details/gsoxheaji.sHtML

[T48] Perl：正则替换
来源：http://www.share.bbcook.cn/Article/details/gxthwuinv.sHtML

$s =~ s/old/new/g;
来源：http://m.share.vehdjk.com/Article/details/gnoyevlkz.sHtML

[T49] Perl：函数
来源：http://wap.bbcook.cn/Article/details/gkvbobezc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gznbmpwij.sHtML

[T50] Perl：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gyqqbdttj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.vehdjk.com/Article/details/gmdviiuge.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.tarul.cn/Article/details/grousnppd.sHtML

[T51] Scala：Hello World
来源：http://wap.tarul.cn/Article/details/gqvsbheui.sHtML

println("Hello")
来源：http://read.share.fktsv.cn/Article/details/gwlefcegc.sHtML

[T52] Scala：变量
来源：http://www.blog.vehdjk.com/Article/details/giuttwtxo.sHtML

val a = 1;  var b = 2
来源：http://blog.tarul.cn/Article/details/grxyzwinr.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gbpmmnzry.sHtML

s"值: $b"
来源：http://3g.fktsv.cn/Article/details/ghbnvawjc.sHtML

[T54] Scala：集合映射
来源：http://wap.tarul.cn/Article/details/gvgqzpoal.sHtML


<!-- 参考信息 -->