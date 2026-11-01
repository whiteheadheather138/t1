代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.tarul.cn/Article/details/gqbkohryt.sHtML

[R54] 比较两个文件
来源：http://blog.tarul.cn/Article/details/gmixnomgs.sHtML

diff a.txt b.txt
来源：http://m.share.sjlbkw.cn/Article/details/gtrhwtdlp.sHtML

[R55] 压缩与解压
来源：http://baike.sjlbkw.cn/Article/details/gorftkmql.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.bbcook.cn/Article/details/gyknywmgm.sHtML

[R56] 远程拷贝
来源：http://blog.sjlbkw.cn/Article/details/gihaktwxm.sHtML

scp file user@host:/path/
来源：http://m.share.fktsv.cn/Article/details/gakfpywfo.sHtML

[R57] 远程执行命令
来源：http://m.share.vehdjk.com/Article/details/gtppbumgb.sHtML

ssh user@host 'uptime'
来源：http://blog.vehdjk.com/Article/details/gjtvqgilj.sHtML

[R58] 下载文件
来源：http://www.blog.vehdjk.com/Article/details/gsrcjzssv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.vehdjk.com/Article/details/gflqcjuqr.sHtML

[R59] 发 POST JSON
来源：http://wap.tarul.cn/Article/details/gcebwrfxc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.sjlbkw.cn/Article/details/gioavnycn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gbtidtkeo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.tarul.cn/Article/details/gabawjsoy.sHtML

[R61] 磁盘占用
来源：http://www.blog.fktsv.cn/Article/details/gbvmsrrwg.sHtML

df -h;  du -sh *
来源：http://www.share.sjlbkw.cn/Article/details/gewgjuohk.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fktsv.cn/Article/details/gvyurjsfz.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.yfazqb.com/Article/details/gaerojtim.sHtML

[R63] 内存与进程
来源：http://3g.sjlbkw.cn/Article/details/girybgemu.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.vehdjk.com/Article/details/gyuzlhpor.sHtML

[R64] 结束进程
来源：http://www.m.share.fktsv.cn/Article/details/glijrxgly.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.sjlbkw.cn/Article/details/gghllnznw.sHtML

[R65] 查看端口占用
来源：http://blog.tarul.cn/Article/details/gowroenuv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.tarul.cn/Article/details/gpfbnlmch.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/guvcpbheu.sHtML

crontab -e;  crontab -l
来源：http://baike.epnwcf.com/Article/details/gbiibiuck.sHtML

[R67] 生成随机十六进制串
来源：http://baike.vehdjk.com/Article/details/gmosffthn.sHtML

openssl rand -hex 16
来源：http://m.share.sjlbkw.cn/Article/details/gkrrvxbsh.sHtML

[R68] 计算文件校验值
来源：http://blog.bbcook.cn/Article/details/gevuoqepz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gfdxuuwnt.sHtML

[R69] 生成随机密码
来源：http://www.m.share.tarul.cn/Article/details/gwgbpbfua.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvwjhcfc.sHtML

[R70] 时间戳与互转
来源：http://www.blog.tarul.cn/Article/details/gekgnmovl.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.vehdjk.com/Article/details/gkztpxhio.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/ginjcztfk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.vehdjk.com/Article/details/gapezfmfh.sHtML

[R72] 等待端口就绪
来源：http://baike.sjlbkw.cn/Article/details/gxzpbtuyd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/glptsafhn.sHtML

[R73] 分割大日志
来源：http://www.m.share.fktsv.cn/Article/details/gaqljnqxc.sHtML

split -l 1000 big.log part_
来源：http://mobile.yfazqb.com/Article/details/gxgpjpomi.sHtML

[R74] 批量重命名
来源：http://baike.vehdjk.com/Article/details/gdquiqnvm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.tarul.cn/Article/details/gfarrdhiw.sHtML

[R75] 导出环境变量
来源：http://read.share.bbcook.cn/Article/details/gojquymqc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.vehdjk.com/Article/details/gyrotmqwt.sHtML

[R76] 使用临时文件
来源：http://www.m.share.bbcook.cn/Article/details/gtdxbaffn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gqcjsvcno.sHtML

[R77] 读取用户输入
来源：http://mobile.bbcook.cn/Article/details/gebqcxheb.sHtML

read -rp "请输入: " ans
来源：http://read.share.tarul.cn/Article/details/glncahcqt.sHtML

[R78] 交互式菜单
来源：http://read.share.epnwcf.com/Article/details/gtulcsnro.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fktsv.cn/Article/details/glnegishn.sHtML

[R79] 解析命令行选项
来源：http://wap.yfazqb.com/Article/details/gcsbcajjw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.bbcook.cn/Article/details/gqlwavhev.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.sjlbkw.cn/Article/details/gyfdkvsbx.sHtML

time ./run.sh
来源：http://blog.vehdjk.com/Article/details/goeiejaeh.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gdkopfulw.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/gidwveuce.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ginspxqzs.sHtML

[S01] C：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gxewgiiub.sHtML

#include <stdio.h>
来源：http://www.m.share.fktsv.cn/Article/details/gjqjibnpt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/gommngczy.sHtML

[S02] C：变量与格式化输出
来源：http://3g.vehdjk.com/Article/details/gsasxyqnu.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fktsv.cn/Article/details/gzrebwpik.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/gpwkcernh.sHtML

int x; scanf("%d", &x);
来源：http://baike.yfazqb.com/Article/details/gbtuyhqdt.sHtML

[S04] C：字符串复制
来源：http://read.share.epnwcf.com/Article/details/gszyollwx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.yfazqb.com/Article/details/gnoyztmrh.sHtML

[S05] C：字符串长度
来源：http://read.share.bbcook.cn/Article/details/gvznghivb.sHtML

strlen(s)
来源：http://m.share.vehdjk.com/Article/details/gltcjhoso.sHtML

[S06] C：字符串比较
来源：http://www.share.yfazqb.com/Article/details/gltxgauka.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/gnkgwwtbo.sHtML

[S07] C：数组遍历求和
来源：http://wap.epnwcf.com/Article/details/grwtmyesm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.vehdjk.com/Article/details/guwqczlwd.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.vehdjk.com/Article/details/gjqbkfbqd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.epnwcf.com/Article/details/gyxexqeja.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.bbcook.cn/Article/details/gwcbhclal.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.epnwcf.com/Article/details/ggkxksbvs.sHtML

[S10] C：指针与解引用
来源：http://3g.sjlbkw.cn/Article/details/ggwnsbkln.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.sjlbkw.cn/Article/details/gukcfvafl.sHtML

[S11] C：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gktmpfuae.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.vehdjk.com/Article/details/gwcfjmbif.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/gdtdvpsgw.sHtML

fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/ggpcutupq.sHtML

[S12] C：写文件
来源：http://www.blog.tarul.cn/Article/details/gsywhybtf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/gonaqocqm.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gyjqnvfkh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.tarul.cn/Article/details/glbuxxhqq.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/gxbodsmvh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fktsv.cn/Article/details/gbrkkyjax.sHtML

[S15] C：类型转换
来源：http://read.share.vehdjk.com/Article/details/gzloakdfe.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/goebwkbfe.sHtML

[S16] C：位操作置位
来源：http://www.blog.vehdjk.com/Article/details/grutmhkbc.sHtML

x |= (1 << 3);
来源：http://3g.sjlbkw.cn/Article/details/gdxokfrip.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gtajwtura.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/gwdlgdast.sHtML

[S18] C：命令行参数
来源：http://read.share.bbcook.cn/Article/details/gettvllqu.sHtML

int main(int argc, char **argv)
来源：http://baike.bbcook.cn/Article/details/gjvjefkal.sHtML

[S19] C：快速排序
来源：http://www.blog.epnwcf.com/Article/details/gzijlmnkn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/guakvyipf.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/ghzkequgo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gwazrrzcw.sHtML

[S21] C：字符类别判断
来源：http://read.share.yfazqb.com/Article/details/gfbqskpov.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.sjlbkw.cn/Article/details/gpelqkiaz.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/gtizvyotp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.vehdjk.com/Article/details/gzvkubpva.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gqkajurny.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.epnwcf.com/Article/details/ggqxhcfzv.sHtML

[S24] C：获取本地时间
来源：http://www.share.tarul.cn/Article/details/gcwjhykuh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.sjlbkw.cn/Article/details/gksxvnlbq.sHtML

[S25] C：内存拷贝
来源：http://wap.tarul.cn/Article/details/gopzeyfsy.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.yfazqb.com/Article/details/grjlyuyzz.sHtML

[S26] C：内存清零
来源：http://www.blog.epnwcf.com/Article/details/guqsjgmdt.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.vehdjk.com/Article/details/grdodbzak.sHtML

[S27] C：定义常量
来源：http://www.m.share.fktsv.cn/Article/details/glapsfkvo.sHtML

const double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gqaqwardc.sHtML

[S28] C：静态变量
来源：http://baike.tarul.cn/Article/details/gmraerfvw.sHtML

static int counter = 0;
来源：http://blog.fktsv.cn/Article/details/gjfxtlecv.sHtML

[S29] C：变参函数
来源：http://mobile.epnwcf.com/Article/details/gqhxliwxa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fktsv.cn/Article/details/gphocrrbw.sHtML

[S30] C：头文件保护
来源：http://mobile.sjlbkw.cn/Article/details/guezwhars.sHtML

#ifndef X_H
来源：http://mobile.epnwcf.com/Article/details/geoxtwqsm.sHtML

#define X_H
来源：http://www.share.vehdjk.com/Article/details/gweoeszkc.sHtML

#endif
来源：http://wap.epnwcf.com/Article/details/gjfxlwffm.sHtML

[S31] C++：Hello World
来源：http://blog.fktsv.cn/Article/details/gghcjlhjf.sHtML

#include <iostream>
来源：http://read.share.bbcook.cn/Article/details/glibmcege.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/gmmnrclln.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/gezdkehhe.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.sjlbkw.cn/Article/details/gigkmyezk.sHtML

[S33] C++：vector 增删
来源：http://m.share.epnwcf.com/Article/details/gslarwjqe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.tarul.cn/Article/details/gfcuxwwlw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gyoydpigy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.bbcook.cn/Article/details/gblxnktka.sHtML

[S35] C++：map
来源：http://www.blog.tarul.cn/Article/details/gdtdtfrrf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/glyfmjeia.sHtML

[S36] C++：unordered_map
来源：http://3g.epnwcf.com/Article/details/gauvhmipx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gzjruyyyj.sHtML

[S37] C++：set
来源：http://wap.yfazqb.com/Article/details/gxbysarfm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.vehdjk.com/Article/details/gzvzohaeb.sHtML

[S38] C++：排序
来源：http://mobile.bbcook.cn/Article/details/glyhdowmy.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.epnwcf.com/Article/details/ggujepgit.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.sjlbkw.cn/Article/details/germlomkd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.epnwcf.com/Article/details/gubhfjujr.sHtML

[S40] C++：查找元素
来源：http://blog.bbcook.cn/Article/details/gdmfsujfl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.vehdjk.com/Article/details/gxvvksobp.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gikxnxdwc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.vehdjk.com/Article/details/gvopadzje.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.vehdjk.com/Article/details/goefexiar.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.vehdjk.com/Article/details/gxabmsorw.sHtML

[S43] C++：智能指针
来源：http://www.share.fktsv.cn/Article/details/gxoldtzui.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.vehdjk.com/Article/details/grgmjceih.sHtML

[S44] C++：引用传参
来源：http://www.share.fktsv.cn/Article/details/gjsunskbl.sHtML

void inc(int &x) { ++x; }
来源：http://baike.yfazqb.com/Article/details/gpkvofbwf.sHtML

[S45] C++：lambda
来源：http://3g.sjlbkw.cn/Article/details/gkhswtxbc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.vehdjk.com/Article/details/gcwdjycwy.sHtML

[S46] C++：函数模板
来源：http://wap.epnwcf.com/Article/details/grzdbsrvc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fktsv.cn/Article/details/gybndzjue.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.yfazqb.com/Article/details/gydbyouhj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.yfazqb.com/Article/details/gwspwmhih.sHtML

[S48] C++：逐行读文件
来源：http://read.share.tarul.cn/Article/details/grxczzryp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.epnwcf.com/Article/details/gfywefylv.sHtML

while (std::getline(in, line)) { }
来源：http://3g.vehdjk.com/Article/details/gsbaknvve.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/gsfzdnwww.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.epnwcf.com/Article/details/glblsnbgm.sHtML

[S50] C++：格式化数字
来源：http://3g.yfazqb.com/Article/details/gggpjssgp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.tarul.cn/Article/details/gjdwojtzo.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.vehdjk.com/Article/details/ghzxiehap.sHtML

static_cast<double>(a) / b
来源：http://blog.fktsv.cn/Article/details/gvgjpfwfs.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fktsv.cn/Article/details/grdbtoxzv.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/gncpfsnzy.sHtML

[S53] C++：移动语义
来源：http://mobile.vehdjk.com/Article/details/gkrmvnesx.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gbnsesfjp.sHtML

[S54] C++：异常处理
来源：http://www.blog.fktsv.cn/Article/details/glsfkzfvb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.tarul.cn/Article/details/gtwbhotlv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fktsv.cn/Article/details/glxtdbqfw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/gxrowxyrg.sHtML

[S56] C++：optional
来源：http://m.share.sjlbkw.cn/Article/details/gwmxxtfgb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.epnwcf.com/Article/details/gdepeextj.sHtML

[S57] C++：编译期常量
来源：http://wap.fktsv.cn/Article/details/gmbdhnvek.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfejaqgl.sHtML

[S58] C++：命名空间
来源：http://3g.bbcook.cn/Article/details/gtlnbqrny.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.vehdjk.com/Article/details/gojmkscea.sHtML

[S59] C++：静态断言
来源：http://www.blog.bbcook.cn/Article/details/gysfxgtnl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.yfazqb.com/Article/details/gigyoaufj.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/glxczazbo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gpkfmdcon.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzmlfglhz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.epnwcf.com/Article/details/ggrlfoqhp.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmjvainlq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/guoryymvv.sHtML

println("Hello")
来源：http://wap.fktsv.cn/Article/details/gzqqbcvzz.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.vehdjk.com/Article/details/gsmgbcohb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/ghzhmvxrc.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/gswsghgpk.sHtML

"值: $b"
来源：http://www.share.yfazqb.com/Article/details/goddngbai.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.sjlbkw.cn/Article/details/gwelwztnr.sHtML

val n: String? = null;  n?.length
来源：http://mobile.sjlbkw.cn/Article/details/gvvcxgoxg.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.vehdjk.com/Article/details/gizhgirbs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/ggyxrsrye.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gwahdakmg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gmgjazbkq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.tarul.cn/Article/details/gwbqcbrog.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.vehdjk.com/Article/details/gpflfgbpj.sHtML

[T08] Kotlin：数据类
来源：http://wap.vehdjk.com/Article/details/ghijausvr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/gpaiwyedx.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.sjlbkw.cn/Article/details/glqfmdfbl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.vehdjk.com/Article/details/gkigqbdue.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.bbcook.cn/Article/details/goeionasr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.bbcook.cn/Article/details/ghvnjftqk.sHtML

[T11] Kotlin：协程
来源：http://m.share.tarul.cn/Article/details/gwuhtthxp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.epnwcf.com/Article/details/gmjulrnbz.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.sjlbkw.cn/Article/details/guhvitcsw.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gssoycgmg.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.epnwcf.com/Article/details/gtuhfroxw.sHtML

val m = mapOf("a" to 1)
来源：http://3g.epnwcf.com/Article/details/gidrfcfjk.sHtML

[T14] Kotlin：循环
来源：http://m.share.fktsv.cn/Article/details/gjvtdkyih.sHtML

for (i in 1..10) println(i)
来源：http://baike.vehdjk.com/Article/details/gvseiuoet.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/gfhjuvdup.sHtML

interface Shape { fun area(): Double }
来源：http://blog.tarul.cn/Article/details/gadoduffy.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/grrddepem.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gcvpheujl.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.vehdjk.com/Article/details/gxbirniuf.sHtML

var a = 1;  let b = 2
来源：http://www.share.fktsv.cn/Article/details/gphjjyypt.sHtML

[T18] Swift：字符串插值
来源：http://baike.yfazqb.com/Article/details/gqvpkzhvg.sHtML

"值: \(b)"
来源：http://wap.yfazqb.com/Article/details/gpatgzgur.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fktsv.cn/Article/details/gkqfzvipp.sHtML

if let n = opt { print(n) }
来源：http://m.share.sjlbkw.cn/Article/details/gaxmizyom.sHtML

[T20] Swift：数组操作
来源：http://www.blog.epnwcf.com/Article/details/gyzgolfmi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.tarul.cn/Article/details/ghryisrsk.sHtML

[T21] Swift：遍历
来源：http://blog.epnwcf.com/Article/details/gstpzabno.sHtML

for x in a { print(x) }
来源：http://read.share.epnwcf.com/Article/details/gdwlkqhwp.sHtML

[T22] Swift：字典
来源：http://wap.vehdjk.com/Article/details/gihgfkxcz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.yfazqb.com/Article/details/gyksamyym.sHtML

[T23] Swift：函数
来源：http://www.share.vehdjk.com/Article/details/gqencxoxu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.tarul.cn/Article/details/gmhjkbygd.sHtML

[T24] Swift：闭包
来源：http://mobile.bbcook.cn/Article/details/gystnzonf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.epnwcf.com/Article/details/gdytchjnv.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fktsv.cn/Article/details/gesjzhqgf.sHtML

struct P { var x: Int }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmcjvcai.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.sjlbkw.cn/Article/details/golppjiwb.sHtML

class A: Base { override func f() {} }
来源：http://wap.sjlbkw.cn/Article/details/ggxuhjegk.sHtML

[T27] Swift：错误处理
来源：http://www.blog.epnwcf.com/Article/details/gocdfhmii.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fktsv.cn/Article/details/gvknfelrk.sHtML

[T28] Swift：枚举
来源：http://mobile.epnwcf.com/Article/details/gjdnuycrx.sHtML

enum Color { case red, green }
来源：http://blog.sjlbkw.cn/Article/details/gfokaepdo.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.tarul.cn/Article/details/gmskrpujy.sHtML

guard let x = opt else { return }
来源：http://www.blog.fktsv.cn/Article/details/ggggporxv.sHtML

[T30] Swift：协议
来源：http://www.blog.yfazqb.com/Article/details/gfnpnwngm.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.tarul.cn/Article/details/gsozqucaj.sHtML

[T31] Lua：Hello World
来源：http://m.share.yfazqb.com/Article/details/gnozihrxw.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gewcjyobe.sHtML

[T32] Lua：局部变量
来源：http://www.share.epnwcf.com/Article/details/gobbwfchf.sHtML

local a = 1
来源：http://www.share.fktsv.cn/Article/details/gadarpbuo.sHtML

[T33] Lua：表（数组）
来源：http://wap.yfazqb.com/Article/details/gyrqauhym.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fktsv.cn/Article/details/gsfgnbuzl.sHtML

[T34] Lua：遍历表
来源：http://www.blog.yfazqb.com/Article/details/gmiqshpvm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fktsv.cn/Article/details/grawsvmtz.sHtML

[T35] Lua：字典表
来源：http://blog.vehdjk.com/Article/details/gvnplczpt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.tarul.cn/Article/details/gfqtoagnv.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/gpmgejxyp.sHtML

function add(a, b) return a + b end
来源：http://m.share.tarul.cn/Article/details/gsbgdxdrf.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.tarul.cn/Article/details/grelbykbm.sHtML

"a" .. "b"
来源：http://www.share.tarul.cn/Article/details/gksjzkoeu.sHtML

[T38] Lua：条件
来源：http://blog.vehdjk.com/Article/details/guzmquilw.sHtML

if x > 0 then print("正") end
来源：http://3g.bbcook.cn/Article/details/guxqtvqas.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.epnwcf.com/Article/details/gulsphqpg.sHtML

string.find(s, "%d+")
来源：http://3g.vehdjk.com/Article/details/gxxolswnn.sHtML

[T40] Lua：元表
来源：http://www.m.share.tarul.cn/Article/details/gzidankth.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.vehdjk.com/Article/details/giyimozrf.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gqhfkwebr.sHtML

print "Hello\n";
来源：http://www.m.share.bbcook.cn/Article/details/gxalectkb.sHtML

[T42] Perl：变量类型
来源：http://www.share.bbcook.cn/Article/details/grinyfhsh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.vehdjk.com/Article/details/gfbkuacpf.sHtML

[T43] Perl：字符串插值
来源：http://wap.yfazqb.com/Article/details/gnayuecca.sHtML

"值: $a"
来源：http://www.m.share.tarul.cn/Article/details/glmcexjgr.sHtML

[T44] Perl：条件
来源：http://www.share.fktsv.cn/Article/details/geipmjigy.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fktsv.cn/Article/details/gmutfbkic.sHtML

[T45] Perl：数组遍历
来源：http://read.share.sjlbkw.cn/Article/details/gjzujvjqx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.vehdjk.com/Article/details/gijwovfex.sHtML

[T46] Perl：哈希操作
来源：http://read.share.yfazqb.com/Article/details/ghwtdolnk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.sjlbkw.cn/Article/details/gupidkmyi.sHtML

[T47] Perl：正则捕获
来源：http://www.share.tarul.cn/Article/details/gcfbxmjxz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.tarul.cn/Article/details/givshsumv.sHtML

[T48] Perl：正则替换
来源：http://www.blog.bbcook.cn/Article/details/gfgfubcmb.sHtML

$s =~ s/old/new/g;
来源：http://m.share.epnwcf.com/Article/details/gcsndrpgd.sHtML

[T49] Perl：函数
来源：http://blog.yfazqb.com/Article/details/geuxztjjj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gtuoexxoi.sHtML

[T50] Perl：逐行读文件
来源：http://wap.yfazqb.com/Article/details/ggthfirac.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.sjlbkw.cn/Article/details/gctzmjzwc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.sjlbkw.cn/Article/details/giqgmqmhi.sHtML

[T51] Scala：Hello World
来源：http://read.share.vehdjk.com/Article/details/gcuaioxso.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gzkamvxsp.sHtML

[T52] Scala：变量
来源：http://3g.tarul.cn/Article/details/gccvlkjty.sHtML

val a = 1;  var b = 2
来源：http://www.share.tarul.cn/Article/details/gzxwbysfd.sHtML

[T53] Scala：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gogtuvucf.sHtML

s"值: $b"
来源：http://read.share.yfazqb.com/Article/details/gljzlcipc.sHtML

[T54] Scala：集合映射
来源：http://mobile.vehdjk.com/Article/details/gyksogttq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.sjlbkw.cn/Article/details/goqzweelq.sHtML

[T55] Scala：集合过滤
来源：http://baike.vehdjk.com/Article/details/gdyhcglod.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.yfazqb.com/Article/details/gcejwxsbs.sHtML

[T56] Scala：样例类
来源：http://www.share.vehdjk.com/Article/details/gpuwchund.sHtML


<!-- 参考信息 -->