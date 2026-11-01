代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.epnwcf.com/Article/details/gsfbjijil.sHtML

[R54] 比较两个文件
来源：http://www.share.sjlbkw.cn/Article/details/gmdsstsga.sHtML

diff a.txt b.txt
来源：http://www.share.yfazqb.com/Article/details/gmrvtfaqv.sHtML

[R55] 压缩与解压
来源：http://wap.sjlbkw.cn/Article/details/gemqgqzxe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.sjlbkw.cn/Article/details/ghpiivoby.sHtML

[R56] 远程拷贝
来源：http://mobile.bbcook.cn/Article/details/geyqiqcru.sHtML

scp file user@host:/path/
来源：http://read.share.bbcook.cn/Article/details/gdnazhuxn.sHtML

[R57] 远程执行命令
来源：http://wap.sjlbkw.cn/Article/details/gubkzajez.sHtML

ssh user@host 'uptime'
来源：http://mobile.sjlbkw.cn/Article/details/gvqffxyro.sHtML

[R58] 下载文件
来源：http://read.share.bbcook.cn/Article/details/gkymppwpn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.bbcook.cn/Article/details/gxkbajazf.sHtML

[R59] 发 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gmgiyubee.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.tarul.cn/Article/details/gutbaqrzo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gplhwbgux.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fktsv.cn/Article/details/gyvyzwffj.sHtML

[R61] 磁盘占用
来源：http://read.share.bbcook.cn/Article/details/gkaehlkwm.sHtML

df -h;  du -sh *
来源：http://www.blog.yfazqb.com/Article/details/gyhavjpxb.sHtML

[R62] 找最占空间的文件
来源：http://www.share.bbcook.cn/Article/details/gczluvopn.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.vehdjk.com/Article/details/geqxdmtek.sHtML

[R63] 内存与进程
来源：http://m.share.fktsv.cn/Article/details/gsgmlkdrm.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.sjlbkw.cn/Article/details/givjombio.sHtML

[R64] 结束进程
来源：http://baike.fktsv.cn/Article/details/gfyzqgffj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.sjlbkw.cn/Article/details/gduarbxik.sHtML

[R65] 查看端口占用
来源：http://blog.bbcook.cn/Article/details/gkgfugmnk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.epnwcf.com/Article/details/gsrlbzans.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/gbuuxefcd.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.epnwcf.com/Article/details/gtslptgaf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fktsv.cn/Article/details/gawfvgcke.sHtML

openssl rand -hex 16
来源：http://www.m.share.sjlbkw.cn/Article/details/grftmffqa.sHtML

[R68] 计算文件校验值
来源：http://m.share.bbcook.cn/Article/details/gabjngaod.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.bbcook.cn/Article/details/gpjvvjtoc.sHtML

[R69] 生成随机密码
来源：http://wap.epnwcf.com/Article/details/gserttpwu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gwcrqkljz.sHtML

[R70] 时间戳与互转
来源：http://read.share.vehdjk.com/Article/details/ghlwjvxwt.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fktsv.cn/Article/details/grxfustin.sHtML

[R71] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/glxskjfyp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.tarul.cn/Article/details/ghwxcrono.sHtML

[R72] 等待端口就绪
来源：http://www.blog.bbcook.cn/Article/details/gagmxtcpt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.sjlbkw.cn/Article/details/gcnnbfzgd.sHtML

[R73] 分割大日志
来源：http://wap.sjlbkw.cn/Article/details/gcrdqxhfk.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/gvknqcjzv.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/gieyzwizq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.epnwcf.com/Article/details/gektkjrae.sHtML

[R75] 导出环境变量
来源：http://blog.sjlbkw.cn/Article/details/guoxvbyqq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fktsv.cn/Article/details/gpfggcsmf.sHtML

[R76] 使用临时文件
来源：http://wap.vehdjk.com/Article/details/gfiwkwwjk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gbbauwqey.sHtML

[R77] 读取用户输入
来源：http://m.share.yfazqb.com/Article/details/gzaxzduma.sHtML

read -rp "请输入: " ans
来源：http://3g.tarul.cn/Article/details/geqidsaqm.sHtML

[R78] 交互式菜单
来源：http://blog.tarul.cn/Article/details/gharrnltp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.epnwcf.com/Article/details/gjmwbhryf.sHtML

[R79] 解析命令行选项
来源：http://m.share.fktsv.cn/Article/details/gplnbuppz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.yfazqb.com/Article/details/gewkujkoa.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.yfazqb.com/Article/details/gerylislr.sHtML

time ./run.sh
来源：http://blog.fktsv.cn/Article/details/gvkpxwods.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grjhwdbrf.sHtML

S. C / C++ 专题
来源：http://m.share.vehdjk.com/Article/details/gsnjirnmg.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gsnjzlkzg.sHtML

[S01] C：Hello World
来源：http://3g.fktsv.cn/Article/details/gxhewggih.sHtML

#include <stdio.h>
来源：http://mobile.fktsv.cn/Article/details/ghrcejlfh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.epnwcf.com/Article/details/gmwluqkuo.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fktsv.cn/Article/details/gkmsrgglb.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.sjlbkw.cn/Article/details/gjvbvhcmg.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/ggvokghuo.sHtML

int x; scanf("%d", &x);
来源：http://read.share.yfazqb.com/Article/details/gdisttugz.sHtML

[S04] C：字符串复制
来源：http://www.m.share.yfazqb.com/Article/details/ggnnvhqdv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.tarul.cn/Article/details/gyxwfltgh.sHtML

[S05] C：字符串长度
来源：http://www.blog.epnwcf.com/Article/details/goffrewjk.sHtML

strlen(s)
来源：http://www.blog.vehdjk.com/Article/details/gcyigrihk.sHtML

[S06] C：字符串比较
来源：http://wap.yfazqb.com/Article/details/gapweidia.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.vehdjk.com/Article/details/glqnjtxsl.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gqsixtkja.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.yfazqb.com/Article/details/gizlnrzaa.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.tarul.cn/Article/details/gywweessp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fktsv.cn/Article/details/gafxpihpd.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.epnwcf.com/Article/details/gkmwowywj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.vehdjk.com/Article/details/gwsvjaauc.sHtML

[S10] C：指针与解引用
来源：http://blog.tarul.cn/Article/details/gdhnoqwqb.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.sjlbkw.cn/Article/details/gbuxrbhqx.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gqaquvjyy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.tarul.cn/Article/details/glbjbhucl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.sjlbkw.cn/Article/details/gcgugydku.sHtML

fclose(f);
来源：http://wap.vehdjk.com/Article/details/gozjlifes.sHtML

[S12] C：写文件
来源：http://baike.fktsv.cn/Article/details/gfcgnxiyo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gkqmpjndg.sHtML

[S13] C：宏定义
来源：http://www.m.share.epnwcf.com/Article/details/gavvtytgr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.tarul.cn/Article/details/grkgmkhhf.sHtML

[S14] C：枚举
来源：http://www.blog.vehdjk.com/Article/details/gvmuqmsuw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.vehdjk.com/Article/details/ghksmbska.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/gqzttrqwn.sHtML

(double) a / b
来源：http://baike.tarul.cn/Article/details/gtglgevfy.sHtML

[S16] C：位操作置位
来源：http://m.share.vehdjk.com/Article/details/gqufonnff.sHtML

x |= (1 << 3);
来源：http://www.m.share.bbcook.cn/Article/details/gdhwsjfgu.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gskwfqzwt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.tarul.cn/Article/details/grquixuts.sHtML

[S18] C：命令行参数
来源：http://mobile.vehdjk.com/Article/details/gmhjsrcoe.sHtML

int main(int argc, char **argv)
来源：http://m.share.bbcook.cn/Article/details/gqyyxpdvn.sHtML

[S19] C：快速排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrobpjsi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/gtugdbieq.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/gfjhalzng.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gsweajdic.sHtML

[S21] C：字符类别判断
来源：http://m.share.epnwcf.com/Article/details/gflshqwgu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.bbcook.cn/Article/details/gzxauxaqe.sHtML

[S22] C：字符串转数字
来源：http://blog.sjlbkw.cn/Article/details/gpluusrru.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fktsv.cn/Article/details/gygunkfct.sHtML

[S23] C：随机数
来源：http://baike.fktsv.cn/Article/details/gvdfekvgd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.yfazqb.com/Article/details/glcbeqxmj.sHtML

[S24] C：获取本地时间
来源：http://blog.bbcook.cn/Article/details/gvjyjusuk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.sjlbkw.cn/Article/details/goqvkimwh.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/gbkapwidb.sHtML

memcpy(dst, src, n);
来源：http://www.share.vehdjk.com/Article/details/gbasmwhbf.sHtML

[S26] C：内存清零
来源：http://3g.vehdjk.com/Article/details/gcnfserpk.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fktsv.cn/Article/details/gexidxzqv.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/gwjfdyfeh.sHtML

const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gsjrwtqrv.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/gacsdwnwn.sHtML

static int counter = 0;
来源：http://3g.tarul.cn/Article/details/gcytfwmgl.sHtML

[S29] C：变参函数
来源：http://www.blog.tarul.cn/Article/details/gejreeexz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fktsv.cn/Article/details/gyqcppzhf.sHtML

[S30] C：头文件保护
来源：http://m.share.bbcook.cn/Article/details/gxrtkmgdk.sHtML

#ifndef X_H
来源：http://www.m.share.yfazqb.com/Article/details/gfvvspkyg.sHtML

#define X_H
来源：http://www.share.sjlbkw.cn/Article/details/gkwpjpgnp.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/gdgjlmqos.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/gpfhslubv.sHtML

#include <iostream>
来源：http://www.share.bbcook.cn/Article/details/gmthijcrz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.epnwcf.com/Article/details/graolpsdx.sHtML

[S32] C++：字符串
来源：http://blog.fktsv.cn/Article/details/gpntswxtw.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fktsv.cn/Article/details/gxenjokoq.sHtML

[S33] C++：vector 增删
来源：http://3g.sjlbkw.cn/Article/details/gvqdytptr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/guibhdkah.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/goiexdmtm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.tarul.cn/Article/details/gfdccarmb.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gzthrndgl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gkkghblfc.sHtML

[S36] C++：unordered_map
来源：http://3g.bbcook.cn/Article/details/gmfbcawwy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/gtmuxssmd.sHtML

[S37] C++：set
来源：http://m.share.fktsv.cn/Article/details/gfjqksnvf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.sjlbkw.cn/Article/details/gtfvywoea.sHtML

[S38] C++：排序
来源：http://wap.sjlbkw.cn/Article/details/gxxbbsali.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/gtkstimku.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.yfazqb.com/Article/details/gylkihyxr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.bbcook.cn/Article/details/gocyaogkq.sHtML

[S40] C++：查找元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrpokagm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.sjlbkw.cn/Article/details/glomjzozx.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gxaebkwma.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsskzzcj.sHtML

[S42] C++：继承与虚函数
来源：http://baike.epnwcf.com/Article/details/gxtvlqfcl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.vehdjk.com/Article/details/gjjnpqcgu.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmxyoczg.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.tarul.cn/Article/details/gxeiphwwc.sHtML

[S44] C++：引用传参
来源：http://www.share.fktsv.cn/Article/details/gexcdeyat.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/gtvpyjnip.sHtML

[S45] C++：lambda
来源：http://mobile.bbcook.cn/Article/details/gshideipn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fktsv.cn/Article/details/gzklycrth.sHtML

[S46] C++：函数模板
来源：http://m.share.epnwcf.com/Article/details/gxesgherz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fktsv.cn/Article/details/glpkcqxod.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gzgxhewdq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.tarul.cn/Article/details/gcslqupha.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gwgqswdrw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.vehdjk.com/Article/details/gsmvljqoy.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.sjlbkw.cn/Article/details/gjbqtlazi.sHtML

[S49] C++：写文件
来源：http://wap.vehdjk.com/Article/details/gmzpxbyrc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.vehdjk.com/Article/details/gxevkkncq.sHtML

[S50] C++：格式化数字
来源：http://mobile.fktsv.cn/Article/details/grvotacwx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gqwknapdy.sHtML

[S51] C++：显式类型转换
来源：http://www.share.bbcook.cn/Article/details/ggwhjcwwg.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gwatbumvt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.epnwcf.com/Article/details/gzsefvwph.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.sjlbkw.cn/Article/details/gpuplnvsf.sHtML

[S53] C++：移动语义
来源：http://www.blog.epnwcf.com/Article/details/gszjkaxrj.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.yfazqb.com/Article/details/gnfazlmuw.sHtML

[S54] C++：异常处理
来源：http://blog.yfazqb.com/Article/details/gftnglhsz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.yfazqb.com/Article/details/geusoobza.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/gapfleilg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/giohcewsg.sHtML

[S56] C++：optional
来源：http://m.share.bbcook.cn/Article/details/gsmunqrxn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/gwwfwlonb.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.vehdjk.com/Article/details/gejqtfmfr.sHtML

constexpr int N = 10;
来源：http://www.blog.bbcook.cn/Article/details/gpzqxfxko.sHtML

[S58] C++：命名空间
来源：http://read.share.bbcook.cn/Article/details/grocxmvvg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.bbcook.cn/Article/details/gvkdukfdz.sHtML

[S59] C++：静态断言
来源：http://mobile.sjlbkw.cn/Article/details/gpjmgiiob.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fktsv.cn/Article/details/gugorvalt.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.tarul.cn/Article/details/glnqaolia.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.vehdjk.com/Article/details/gnxrivhlo.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gggryjuwg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.tarul.cn/Article/details/ghtojdsgb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbomzuhvx.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/ghmuwfyzh.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/gjwozosjw.sHtML

[T02] Kotlin：变量
来源：http://read.share.yfazqb.com/Article/details/gcyebctks.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.vehdjk.com/Article/details/gkszycvml.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.sjlbkw.cn/Article/details/gzdqqjpvf.sHtML

"值: $b"
来源：http://m.share.epnwcf.com/Article/details/gkprpuhxv.sHtML

[T04] Kotlin：空安全
来源：http://baike.tarul.cn/Article/details/grtvqitkq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.tarul.cn/Article/details/ggkdiauht.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.epnwcf.com/Article/details/gzemmgabp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.vehdjk.com/Article/details/gswizxxrk.sHtML

[T06] Kotlin：集合映射
来源：http://3g.tarul.cn/Article/details/gvnwywpjj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fktsv.cn/Article/details/gqtytijmr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gajhkazjr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.epnwcf.com/Article/details/gtmxjtcfz.sHtML

[T08] Kotlin：数据类
来源：http://3g.yfazqb.com/Article/details/gstdegtnk.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.bbcook.cn/Article/details/gafkbytkz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.epnwcf.com/Article/details/gkzyoepwo.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.vehdjk.com/Article/details/gkyfqtpzk.sHtML

[T10] Kotlin：默认参数
来源：http://wap.epnwcf.com/Article/details/gahtiyoly.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.vehdjk.com/Article/details/glrwzpaut.sHtML

[T11] Kotlin：协程
来源：http://wap.vehdjk.com/Article/details/gpjxvoxtx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.bbcook.cn/Article/details/ggsanogwm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.epnwcf.com/Article/details/gnxlxpgda.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fktsv.cn/Article/details/gthvgemfp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.yfazqb.com/Article/details/gxeuqxruy.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/gyilbreyt.sHtML

[T14] Kotlin：循环
来源：http://baike.epnwcf.com/Article/details/gqagigqoy.sHtML

for (i in 1..10) println(i)
来源：http://wap.bbcook.cn/Article/details/gykebuqfn.sHtML

[T15] Kotlin：接口
来源：http://blog.fktsv.cn/Article/details/grrlwpool.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.epnwcf.com/Article/details/gsnudskyq.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/gnawsatgw.sHtML

print("Hello")
来源：http://www.share.tarul.cn/Article/details/ganyhfsuu.sHtML

[T17] Swift：变量与常量
来源：http://blog.bbcook.cn/Article/details/gcmhsnwjx.sHtML

var a = 1;  let b = 2
来源：http://m.share.epnwcf.com/Article/details/gxmmxsium.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/geuelyexp.sHtML

"值: \(b)"
来源：http://blog.tarul.cn/Article/details/gauvytdln.sHtML

[T19] Swift：可选绑定
来源：http://mobile.vehdjk.com/Article/details/gawcyootx.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/ggbkmkexx.sHtML

[T20] Swift：数组操作
来源：http://www.blog.epnwcf.com/Article/details/gwddjpafe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.bbcook.cn/Article/details/gkvosfftr.sHtML

[T21] Swift：遍历
来源：http://3g.epnwcf.com/Article/details/gvcrwmfhi.sHtML

for x in a { print(x) }
来源：http://3g.yfazqb.com/Article/details/gayajkbre.sHtML

[T22] Swift：字典
来源：http://wap.bbcook.cn/Article/details/gzpsirefy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.tarul.cn/Article/details/gwjeyibpj.sHtML

[T23] Swift：函数
来源：http://www.blog.yfazqb.com/Article/details/gywuikhes.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.epnwcf.com/Article/details/ggihjjerb.sHtML

[T24] Swift：闭包
来源：http://mobile.fktsv.cn/Article/details/gysefoqch.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.epnwcf.com/Article/details/gzqmbuxqb.sHtML

[T25] Swift：结构体
来源：http://mobile.sjlbkw.cn/Article/details/gjhnneepa.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/gtsnupbtn.sHtML

[T26] Swift：类与重写
来源：http://read.share.fktsv.cn/Article/details/gnavxkggw.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.tarul.cn/Article/details/gqptjerjc.sHtML

[T27] Swift：错误处理
来源：http://wap.epnwcf.com/Article/details/gryqryztn.sHtML

do { try f() } catch { print(error) }
来源：http://wap.yfazqb.com/Article/details/gcxtgomyf.sHtML

[T28] Swift：枚举
来源：http://baike.bbcook.cn/Article/details/ghfidzusi.sHtML

enum Color { case red, green }
来源：http://mobile.vehdjk.com/Article/details/geexwyvvt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.vehdjk.com/Article/details/goxsflvmj.sHtML

guard let x = opt else { return }
来源：http://3g.sjlbkw.cn/Article/details/gyasewlqk.sHtML

[T30] Swift：协议
来源：http://www.blog.epnwcf.com/Article/details/gpweogtkq.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.sjlbkw.cn/Article/details/grrgprykz.sHtML

[T31] Lua：Hello World
来源：http://baike.fktsv.cn/Article/details/gptyslfld.sHtML

print("Hello")
来源：http://read.share.tarul.cn/Article/details/gdvstpagx.sHtML

[T32] Lua：局部变量
来源：http://blog.vehdjk.com/Article/details/ggbbnqqyl.sHtML

local a = 1
来源：http://baike.bbcook.cn/Article/details/gqacygkfg.sHtML

[T33] Lua：表（数组）
来源：http://www.share.tarul.cn/Article/details/gtbfqohcw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.sjlbkw.cn/Article/details/gtxemjico.sHtML

[T34] Lua：遍历表
来源：http://read.share.vehdjk.com/Article/details/gyzqrbzpz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.vehdjk.com/Article/details/gknvvokjf.sHtML

[T35] Lua：字典表
来源：http://www.share.vehdjk.com/Article/details/giqlxrwjh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fktsv.cn/Article/details/gibmykkgr.sHtML

[T36] Lua：函数
来源：http://wap.epnwcf.com/Article/details/gdnmfilez.sHtML

function add(a, b) return a + b end
来源：http://blog.fktsv.cn/Article/details/gywlkmlim.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.tarul.cn/Article/details/gqwoghbbo.sHtML

"a" .. "b"
来源：http://mobile.epnwcf.com/Article/details/glpqqgkgr.sHtML

[T38] Lua：条件
来源：http://read.share.epnwcf.com/Article/details/geihrdjos.sHtML

if x > 0 then print("正") end
来源：http://blog.vehdjk.com/Article/details/gfxwgusoi.sHtML

[T39] Lua：模式匹配
来源：http://read.share.tarul.cn/Article/details/grezmklav.sHtML

string.find(s, "%d+")
来源：http://baike.fktsv.cn/Article/details/gjhxenxbg.sHtML

[T40] Lua：元表
来源：http://www.blog.vehdjk.com/Article/details/gbnzwdayk.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjplohhp.sHtML

[T41] Perl：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gayhbqrmq.sHtML

print "Hello\n";
来源：http://wap.yfazqb.com/Article/details/gfndwmnbh.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/guslijqkl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.bbcook.cn/Article/details/gmrzwzazs.sHtML

[T43] Perl：字符串插值
来源：http://m.share.tarul.cn/Article/details/gvriblvmj.sHtML

"值: $a"
来源：http://www.m.share.epnwcf.com/Article/details/gfxldsvtu.sHtML

[T44] Perl：条件
来源：http://www.blog.bbcook.cn/Article/details/gqhatqtfc.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fktsv.cn/Article/details/gynyvrhdd.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gayqpomri.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.epnwcf.com/Article/details/gjvkpiwwn.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fktsv.cn/Article/details/garoudqfn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/gyppfvwus.sHtML

[T47] Perl：正则捕获
来源：http://blog.fktsv.cn/Article/details/grjclfiri.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.tarul.cn/Article/details/ggjjydtbw.sHtML

[T48] Perl：正则替换
来源：http://blog.fktsv.cn/Article/details/ggptnixwe.sHtML

$s =~ s/old/new/g;
来源：http://3g.sjlbkw.cn/Article/details/gnuzimgao.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/gvjagdzxt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gcgusyluq.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.tarul.cn/Article/details/gazltxljy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.yfazqb.com/Article/details/gwhmwmmus.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.epnwcf.com/Article/details/gwpywqfbx.sHtML

[T51] Scala：Hello World
来源：http://read.share.epnwcf.com/Article/details/gauoikemc.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/gzyqtyqiz.sHtML

[T52] Scala：变量
来源：http://www.blog.sjlbkw.cn/Article/details/goxyrbqjr.sHtML

val a = 1;  var b = 2
来源：http://baike.bbcook.cn/Article/details/gletasquu.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gimyoqhyb.sHtML

s"值: $b"
来源：http://www.share.epnwcf.com/Article/details/gvnqcyeow.sHtML

[T54] Scala：集合映射
来源：http://wap.bbcook.cn/Article/details/gabwvxfzb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fktsv.cn/Article/details/ggxshlgtb.sHtML

[T55] Scala：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gfiubylqb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.vehdjk.com/Article/details/gyttkaeex.sHtML

[T56] Scala：样例类
来源：http://blog.yfazqb.com/Article/details/ghpiibolo.sHtML


<!-- 参考信息 -->