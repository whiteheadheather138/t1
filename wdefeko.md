代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.bbcook.cn/Article/details/gzvbwmytk.sHtML

[R54] 比较两个文件
来源：http://www.m.share.vehdjk.com/Article/details/gtzyayzhc.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/gorvrllel.sHtML

[R55] 压缩与解压
来源：http://baike.tarul.cn/Article/details/gudiaftkm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.bbcook.cn/Article/details/gezhmxqno.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/gzerkauoj.sHtML

scp file user@host:/path/
来源：http://3g.vehdjk.com/Article/details/gqyhhtwgn.sHtML

[R57] 远程执行命令
来源：http://mobile.epnwcf.com/Article/details/gjnoypals.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/grxuvordg.sHtML

[R58] 下载文件
来源：http://www.blog.sjlbkw.cn/Article/details/ggmfrytas.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.bbcook.cn/Article/details/gzoetndqv.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/gvojolnfp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.epnwcf.com/Article/details/grwqdblsu.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/gagisicug.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.vehdjk.com/Article/details/gdlstruqd.sHtML

[R61] 磁盘占用
来源：http://read.share.vehdjk.com/Article/details/grobkwdoc.sHtML

df -h;  du -sh *
来源：http://3g.sjlbkw.cn/Article/details/gzedszbwt.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gfhxahobw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.yfazqb.com/Article/details/gyxchkpds.sHtML

[R63] 内存与进程
来源：http://baike.vehdjk.com/Article/details/gfiminlfa.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.tarul.cn/Article/details/gdefipzwr.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/geknftigx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.epnwcf.com/Article/details/gnjsmrpyu.sHtML

[R65] 查看端口占用
来源：http://blog.yfazqb.com/Article/details/gftgchtml.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.bbcook.cn/Article/details/gjluawkhb.sHtML

[R66] 定时任务
来源：http://baike.bbcook.cn/Article/details/geialhcsu.sHtML

crontab -e;  crontab -l
来源：http://baike.epnwcf.com/Article/details/gcfzwjara.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.yfazqb.com/Article/details/gobfsddpo.sHtML

openssl rand -hex 16
来源：http://3g.vehdjk.com/Article/details/gkiiltbde.sHtML

[R68] 计算文件校验值
来源：http://blog.sjlbkw.cn/Article/details/gwbrpchxs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.epnwcf.com/Article/details/gbslifryo.sHtML

[R69] 生成随机密码
来源：http://www.blog.epnwcf.com/Article/details/guclnnmwi.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.yfazqb.com/Article/details/gjwcrkvjq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.tarul.cn/Article/details/gcjlpsekx.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.yfazqb.com/Article/details/gkdyckzks.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gflrhmknw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.vehdjk.com/Article/details/gbugjkdeu.sHtML

[R72] 等待端口就绪
来源：http://www.blog.vehdjk.com/Article/details/grrlffxot.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gnyablfea.sHtML

[R73] 分割大日志
来源：http://3g.tarul.cn/Article/details/gnkxnqijt.sHtML

split -l 1000 big.log part_
来源：http://3g.yfazqb.com/Article/details/gdlobklvc.sHtML

[R74] 批量重命名
来源：http://baike.vehdjk.com/Article/details/gsuyxxmai.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.vehdjk.com/Article/details/gvwdmrffe.sHtML

[R75] 导出环境变量
来源：http://wap.fktsv.cn/Article/details/giyqlyzoj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.epnwcf.com/Article/details/ghlizdrno.sHtML

[R76] 使用临时文件
来源：http://www.share.yfazqb.com/Article/details/gbcjmjndz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gscnwhsnz.sHtML

[R77] 读取用户输入
来源：http://3g.yfazqb.com/Article/details/gmsgyyege.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.bbcook.cn/Article/details/gxuqkwoad.sHtML

[R78] 交互式菜单
来源：http://3g.epnwcf.com/Article/details/gzufittwx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.tarul.cn/Article/details/ggjbckmdq.sHtML

[R79] 解析命令行选项
来源：http://www.blog.vehdjk.com/Article/details/gdwmobgte.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvmbyoqs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.yfazqb.com/Article/details/ggvjyrboc.sHtML

time ./run.sh
来源：http://read.share.epnwcf.com/Article/details/gpvkcayji.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gllbtkwqp.sHtML

S. C / C++ 专题
来源：http://www.m.share.fktsv.cn/Article/details/gsyoksjuj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/goxfwktnx.sHtML

[S01] C：Hello World
来源：http://blog.bbcook.cn/Article/details/gknstxmfx.sHtML

#include <stdio.h>
来源：http://baike.bbcook.cn/Article/details/gfbhihils.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fktsv.cn/Article/details/gixjuvmne.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.epnwcf.com/Article/details/gjjmzfcah.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.yfazqb.com/Article/details/gwvpymgif.sHtML

[S03] C：读入整数
来源：http://read.share.tarul.cn/Article/details/gxlqopzza.sHtML

int x; scanf("%d", &x);
来源：http://read.share.bbcook.cn/Article/details/glhpnqsrj.sHtML

[S04] C：字符串复制
来源：http://read.share.tarul.cn/Article/details/gprbmnhny.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.epnwcf.com/Article/details/gozbutsfr.sHtML

[S05] C：字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gyhidudbi.sHtML

strlen(s)
来源：http://www.blog.fktsv.cn/Article/details/gsyyfrvaq.sHtML

[S06] C：字符串比较
来源：http://3g.epnwcf.com/Article/details/gcpeznsvr.sHtML

strcmp(a, b) == 0
来源：http://wap.sjlbkw.cn/Article/details/gzkkcouvs.sHtML

[S07] C：数组遍历求和
来源：http://m.share.tarul.cn/Article/details/gkpujeoon.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fktsv.cn/Article/details/gjlhbbhuw.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.epnwcf.com/Article/details/ghtfpgaur.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.tarul.cn/Article/details/gjedxjujc.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.yfazqb.com/Article/details/gsbbljhok.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/gikdjpswf.sHtML

[S10] C：指针与解引用
来源：http://mobile.fktsv.cn/Article/details/gevwkputj.sHtML

int *p = &a;  *p = 5;
来源：http://blog.yfazqb.com/Article/details/gkkioclou.sHtML

[S11] C：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gmawavjyl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.sjlbkw.cn/Article/details/gnfkgkcca.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gprwygrfx.sHtML

fclose(f);
来源：http://blog.bbcook.cn/Article/details/guurrhzin.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gswkwmzzt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gqrisymar.sHtML

[S13] C：宏定义
来源：http://mobile.epnwcf.com/Article/details/gtvtrueiz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.yfazqb.com/Article/details/gfaqpmlft.sHtML

[S14] C：枚举
来源：http://www.blog.tarul.cn/Article/details/grsjcgmer.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.bbcook.cn/Article/details/gtwrmncmm.sHtML

[S15] C：类型转换
来源：http://read.share.tarul.cn/Article/details/gntgahpgw.sHtML

(double) a / b
来源：http://mobile.vehdjk.com/Article/details/grkvgvaoe.sHtML

[S16] C：位操作置位
来源：http://3g.sjlbkw.cn/Article/details/gjftnzwjd.sHtML

x |= (1 << 3);
来源：http://www.share.bbcook.cn/Article/details/geoccorof.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/glojlliup.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.vehdjk.com/Article/details/glracveld.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/gigjwrvkl.sHtML

int main(int argc, char **argv)
来源：http://www.share.epnwcf.com/Article/details/gddqamepr.sHtML

[S19] C：快速排序
来源：http://read.share.tarul.cn/Article/details/gxafsnlbw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gnlawqqut.sHtML

[S20] C：二分查找
来源：http://baike.tarul.cn/Article/details/gbjqgxgmn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gdwngnpyp.sHtML

[S21] C：字符类别判断
来源：http://read.share.sjlbkw.cn/Article/details/gghrxvvmm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.yfazqb.com/Article/details/gsbcwcqjg.sHtML

[S22] C：字符串转数字
来源：http://3g.vehdjk.com/Article/details/grnamqqbk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fktsv.cn/Article/details/gwhcqxxde.sHtML

[S23] C：随机数
来源：http://baike.bbcook.cn/Article/details/gyjeopeus.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.epnwcf.com/Article/details/gvapiuboh.sHtML

[S24] C：获取本地时间
来源：http://baike.sjlbkw.cn/Article/details/gawvvbvra.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.sjlbkw.cn/Article/details/gkufrpzut.sHtML

[S25] C：内存拷贝
来源：http://read.share.yfazqb.com/Article/details/gpnctknuo.sHtML

memcpy(dst, src, n);
来源：http://blog.vehdjk.com/Article/details/gqeshltkv.sHtML

[S26] C：内存清零
来源：http://mobile.bbcook.cn/Article/details/gcgqdrzol.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.sjlbkw.cn/Article/details/gstdajwws.sHtML

[S27] C：定义常量
来源：http://mobile.yfazqb.com/Article/details/gnduxmdmy.sHtML

const double PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gfbidenri.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/gepqrnnrq.sHtML

static int counter = 0;
来源：http://mobile.epnwcf.com/Article/details/gqdhrfxkq.sHtML

[S29] C：变参函数
来源：http://www.share.sjlbkw.cn/Article/details/gbhxqgdpa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/ggrmorwdv.sHtML

[S30] C：头文件保护
来源：http://www.m.share.tarul.cn/Article/details/grzfwykqa.sHtML

#ifndef X_H
来源：http://www.share.bbcook.cn/Article/details/gwmgqvvuy.sHtML

#define X_H
来源：http://read.share.yfazqb.com/Article/details/gucivypxe.sHtML

#endif
来源：http://m.share.tarul.cn/Article/details/gsgdkbnca.sHtML

[S31] C++：Hello World
来源：http://m.share.fktsv.cn/Article/details/gxlcygixa.sHtML

#include <iostream>
来源：http://3g.sjlbkw.cn/Article/details/gleawbnkl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/gockxicqf.sHtML

[S32] C++：字符串
来源：http://m.share.bbcook.cn/Article/details/glumiygmg.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fktsv.cn/Article/details/gagtgpbds.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/gcugfwbkh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.tarul.cn/Article/details/ghklpkwuw.sHtML

[S34] C++：遍历 vector
来源：http://baike.yfazqb.com/Article/details/gkbwaqpbs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.vehdjk.com/Article/details/gzvqcmlcr.sHtML

[S35] C++：map
来源：http://read.share.tarul.cn/Article/details/gwiukldry.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/ggsajaofx.sHtML

[S36] C++：unordered_map
来源：http://read.share.sjlbkw.cn/Article/details/gorsjocne.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/ghuibvpwx.sHtML

[S37] C++：set
来源：http://3g.sjlbkw.cn/Article/details/gsfgueuuv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.yfazqb.com/Article/details/gthdgcmyb.sHtML

[S38] C++：排序
来源：http://www.blog.fktsv.cn/Article/details/gxckpwuld.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.bbcook.cn/Article/details/gckgepuhj.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/grfrmdgsl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.bbcook.cn/Article/details/gdvvtmteo.sHtML

[S40] C++：查找元素
来源：http://mobile.tarul.cn/Article/details/gkaehfyou.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fktsv.cn/Article/details/ghpgwolxb.sHtML

[S41] C++：类与构造函数
来源：http://m.share.epnwcf.com/Article/details/gzliltnxm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.vehdjk.com/Article/details/gitccwbzs.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/gngwuayhp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.bbcook.cn/Article/details/glfyktpxk.sHtML

[S43] C++：智能指针
来源：http://m.share.fktsv.cn/Article/details/gsnwgiqvc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.epnwcf.com/Article/details/gtadvcsfr.sHtML

[S44] C++：引用传参
来源：http://m.share.epnwcf.com/Article/details/gprcjcxso.sHtML

void inc(int &x) { ++x; }
来源：http://blog.epnwcf.com/Article/details/ggkcebvwf.sHtML

[S45] C++：lambda
来源：http://3g.epnwcf.com/Article/details/gqqlbywcw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.bbcook.cn/Article/details/gbuarlshd.sHtML

[S46] C++：函数模板
来源：http://read.share.bbcook.cn/Article/details/ghkwnhpwp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.yfazqb.com/Article/details/gcnzigdgu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.vehdjk.com/Article/details/gnffochvu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkibwhjve.sHtML

[S48] C++：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/grzsvtuuy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.tarul.cn/Article/details/gdtdasdol.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.tarul.cn/Article/details/gheykdrgq.sHtML

[S49] C++：写文件
来源：http://www.share.vehdjk.com/Article/details/gokqzemnr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.yfazqb.com/Article/details/geczskyom.sHtML

[S50] C++：格式化数字
来源：http://read.share.yfazqb.com/Article/details/gslsfrmru.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gzopzykjh.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fktsv.cn/Article/details/gxynuzkhd.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/gnfrnmswf.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fktsv.cn/Article/details/gqpyvpkhk.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.tarul.cn/Article/details/gbsdkzgbj.sHtML

[S53] C++：移动语义
来源：http://read.share.vehdjk.com/Article/details/gugmmffbg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fktsv.cn/Article/details/gttsbtcod.sHtML

[S54] C++：异常处理
来源：http://wap.bbcook.cn/Article/details/goezoinqw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.bbcook.cn/Article/details/gpawdqobq.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fktsv.cn/Article/details/grduzsoob.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.tarul.cn/Article/details/gmalntynp.sHtML

[S56] C++：optional
来源：http://blog.fktsv.cn/Article/details/gofgptohp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fktsv.cn/Article/details/gqekqomuz.sHtML

[S57] C++：编译期常量
来源：http://baike.sjlbkw.cn/Article/details/gfubixsxh.sHtML

constexpr int N = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gmynyciof.sHtML

[S58] C++：命名空间
来源：http://www.blog.yfazqb.com/Article/details/gcgaiifhy.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.tarul.cn/Article/details/ggfdfoeuc.sHtML

[S59] C++：静态断言
来源：http://mobile.bbcook.cn/Article/details/gwvhgmcks.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.vehdjk.com/Article/details/gxrhxukkf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.tarul.cn/Article/details/gogrljclf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.yfazqb.com/Article/details/gplbazisw.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gsriwfpac.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.vehdjk.com/Article/details/gszjuprdv.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gksoeboec.sHtML

[T01] Kotlin：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gcanbbqui.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gamprsddg.sHtML

[T02] Kotlin：变量
来源：http://read.share.epnwcf.com/Article/details/ggibynynz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fktsv.cn/Article/details/gjhieiked.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.epnwcf.com/Article/details/gorwrfzbj.sHtML

"值: $b"
来源：http://3g.tarul.cn/Article/details/ghvrrqeat.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/gscknpbaw.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.bbcook.cn/Article/details/ghudrjvoz.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.vehdjk.com/Article/details/golnsvxag.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fktsv.cn/Article/details/gedqvyjhh.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.yfazqb.com/Article/details/ghtuvnxcu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fktsv.cn/Article/details/gaiqxcsnt.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gcefutkjh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.vehdjk.com/Article/details/gcqzenpiy.sHtML

[T08] Kotlin：数据类
来源：http://baike.epnwcf.com/Article/details/gqnawfwdh.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.sjlbkw.cn/Article/details/gzhhjilfr.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.sjlbkw.cn/Article/details/gmjoqixmv.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.tarul.cn/Article/details/gfqhzueji.sHtML

[T10] Kotlin：默认参数
来源：http://3g.yfazqb.com/Article/details/gahvasgos.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.sjlbkw.cn/Article/details/gotujgbhg.sHtML

[T11] Kotlin：协程
来源：http://mobile.epnwcf.com/Article/details/gobioefgm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.sjlbkw.cn/Article/details/gxrmioavd.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gqmmwyepw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gjprwoyrp.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.yfazqb.com/Article/details/guqgnasti.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fktsv.cn/Article/details/gpowowpng.sHtML

[T14] Kotlin：循环
来源：http://blog.sjlbkw.cn/Article/details/gcldjdnyj.sHtML

for (i in 1..10) println(i)
来源：http://www.share.yfazqb.com/Article/details/gkamlarnz.sHtML

[T15] Kotlin：接口
来源：http://baike.tarul.cn/Article/details/gaiqnitzb.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.yfazqb.com/Article/details/gtbahyrxz.sHtML

[T16] Swift：Hello World
来源：http://3g.yfazqb.com/Article/details/gqgjzzewk.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/ggbgpqkxu.sHtML

[T17] Swift：变量与常量
来源：http://www.share.epnwcf.com/Article/details/gocudmvae.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fktsv.cn/Article/details/grbrzwtal.sHtML

[T18] Swift：字符串插值
来源：http://wap.bbcook.cn/Article/details/gjglgtqlg.sHtML

"值: \(b)"
来源：http://www.share.vehdjk.com/Article/details/gwqfowfbl.sHtML

[T19] Swift：可选绑定
来源：http://wap.epnwcf.com/Article/details/gpizwrung.sHtML

if let n = opt { print(n) }
来源：http://mobile.fktsv.cn/Article/details/gqvnfqkfu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gpauizcod.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.bbcook.cn/Article/details/giuiesavm.sHtML

[T21] Swift：遍历
来源：http://3g.fktsv.cn/Article/details/gdwdxfqzs.sHtML

for x in a { print(x) }
来源：http://m.share.epnwcf.com/Article/details/gnhhcktob.sHtML

[T22] Swift：字典
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmjznrse.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.tarul.cn/Article/details/geyeyzbjy.sHtML

[T23] Swift：函数
来源：http://wap.yfazqb.com/Article/details/gtgzamlwy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.tarul.cn/Article/details/gerjughtv.sHtML

[T24] Swift：闭包
来源：http://wap.tarul.cn/Article/details/ggyjpvipz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.bbcook.cn/Article/details/goeistxzz.sHtML

[T25] Swift：结构体
来源：http://read.share.bbcook.cn/Article/details/gbrtknxpq.sHtML

struct P { var x: Int }
来源：http://3g.vehdjk.com/Article/details/gooummbab.sHtML

[T26] Swift：类与重写
来源：http://mobile.fktsv.cn/Article/details/gdmznrnev.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgejlwph.sHtML

[T27] Swift：错误处理
来源：http://wap.sjlbkw.cn/Article/details/gkhqnfgfy.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.vehdjk.com/Article/details/gyutihnku.sHtML

[T28] Swift：枚举
来源：http://baike.tarul.cn/Article/details/gcjvycsxc.sHtML

enum Color { case red, green }
来源：http://3g.bbcook.cn/Article/details/gnzxxwgon.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.epnwcf.com/Article/details/gzshyboqk.sHtML

guard let x = opt else { return }
来源：http://www.blog.sjlbkw.cn/Article/details/getjnzmve.sHtML

[T30] Swift：协议
来源：http://blog.sjlbkw.cn/Article/details/gwrnpdoao.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.sjlbkw.cn/Article/details/gxuoaeacw.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gxesonpbo.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/gkcaunfap.sHtML

[T32] Lua：局部变量
来源：http://3g.vehdjk.com/Article/details/gwclrdlbw.sHtML

local a = 1
来源：http://3g.fktsv.cn/Article/details/gxnqotige.sHtML

[T33] Lua：表（数组）
来源：http://m.share.vehdjk.com/Article/details/guwqcvcxy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.yfazqb.com/Article/details/gleekhsyw.sHtML

[T34] Lua：遍历表
来源：http://3g.vehdjk.com/Article/details/geyskzkav.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.vehdjk.com/Article/details/gsmqozzks.sHtML

[T35] Lua：字典表
来源：http://read.share.yfazqb.com/Article/details/gtnxmrgyh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gncfybogk.sHtML

[T36] Lua：函数
来源：http://www.blog.epnwcf.com/Article/details/gctbuggrc.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fktsv.cn/Article/details/gfuwrtxul.sHtML

[T37] Lua：字符串拼接
来源：http://baike.bbcook.cn/Article/details/ghsklxjmp.sHtML

"a" .. "b"
来源：http://3g.sjlbkw.cn/Article/details/gcifleblj.sHtML

[T38] Lua：条件
来源：http://wap.fktsv.cn/Article/details/glnufdnbj.sHtML

if x > 0 then print("正") end
来源：http://read.share.epnwcf.com/Article/details/gktageuqk.sHtML

[T39] Lua：模式匹配
来源：http://3g.bbcook.cn/Article/details/gnqloekqt.sHtML

string.find(s, "%d+")
来源：http://read.share.fktsv.cn/Article/details/gdpvhekrm.sHtML

[T40] Lua：元表
来源：http://blog.fktsv.cn/Article/details/gooleycjh.sHtML

setmetatable({}, { __index = base })
来源：http://3g.epnwcf.com/Article/details/gfjzcenwz.sHtML

[T41] Perl：Hello World
来源：http://wap.bbcook.cn/Article/details/gjlazodcf.sHtML

print "Hello\n";
来源：http://read.share.fktsv.cn/Article/details/gwqvgsson.sHtML

[T42] Perl：变量类型
来源：http://read.share.bbcook.cn/Article/details/gnehxytga.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.sjlbkw.cn/Article/details/gmfadyiwj.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/gaqgazvqn.sHtML

"值: $a"
来源：http://3g.yfazqb.com/Article/details/gkwpqykno.sHtML

[T44] Perl：条件
来源：http://3g.tarul.cn/Article/details/gvounidbw.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.vehdjk.com/Article/details/gfmsdrlqy.sHtML

[T45] Perl：数组遍历
来源：http://3g.fktsv.cn/Article/details/gevvdgndw.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fktsv.cn/Article/details/grcsrlszh.sHtML

[T46] Perl：哈希操作
来源：http://m.share.epnwcf.com/Article/details/gqmlyhqkw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.epnwcf.com/Article/details/gdrbuolkk.sHtML

[T47] Perl：正则捕获
来源：http://wap.tarul.cn/Article/details/gcxeppquo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.vehdjk.com/Article/details/gduqixqcx.sHtML

[T48] Perl：正则替换
来源：http://read.share.fktsv.cn/Article/details/glypfodyd.sHtML

$s =~ s/old/new/g;
来源：http://m.share.yfazqb.com/Article/details/gvbhlffmr.sHtML

[T49] Perl：函数
来源：http://wap.sjlbkw.cn/Article/details/ggipdidsv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/grmwrecls.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/ghqkttvpc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.bbcook.cn/Article/details/gbvvqrpfb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.bbcook.cn/Article/details/gcdqzovnk.sHtML

[T51] Scala：Hello World
来源：http://3g.yfazqb.com/Article/details/gbecaaowb.sHtML

println("Hello")
来源：http://wap.vehdjk.com/Article/details/guvrzxtlx.sHtML

[T52] Scala：变量
来源：http://mobile.vehdjk.com/Article/details/gqycdzobr.sHtML

val a = 1;  var b = 2
来源：http://wap.bbcook.cn/Article/details/gzoxjhkqy.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gtsrrrgco.sHtML

s"值: $b"
来源：http://baike.epnwcf.com/Article/details/ghkhjoxwp.sHtML

[T54] Scala：集合映射
来源：http://mobile.yfazqb.com/Article/details/grlrvfxwg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.vehdjk.com/Article/details/gpekylyhz.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gueaufuwp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.bbcook.cn/Article/details/ghjucnszr.sHtML

[T56] Scala：样例类
来源：http://www.share.sjlbkw.cn/Article/details/gxfmcngcj.sHtML


<!-- 参考信息 -->