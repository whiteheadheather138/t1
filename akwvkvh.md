代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.vehdjk.com/Article/details/gqhnazhma.sHtML

[R54] 比较两个文件
来源：http://www.blog.yfazqb.com/Article/details/gxqscamsy.sHtML

diff a.txt b.txt
来源：http://baike.vehdjk.com/Article/details/gkxinsefx.sHtML

[R55] 压缩与解压
来源：http://3g.tarul.cn/Article/details/gfwpkrrsc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.yfazqb.com/Article/details/ghqbeizga.sHtML

[R56] 远程拷贝
来源：http://www.blog.epnwcf.com/Article/details/gvsvbzsjw.sHtML

scp file user@host:/path/
来源：http://read.share.epnwcf.com/Article/details/gqfzoppvt.sHtML

[R57] 远程执行命令
来源：http://www.blog.fktsv.cn/Article/details/gwqctiunb.sHtML

ssh user@host 'uptime'
来源：http://m.share.sjlbkw.cn/Article/details/gjtvyeuio.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gvtkrnidh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.sjlbkw.cn/Article/details/ggalpalvx.sHtML

[R59] 发 POST JSON
来源：http://read.share.tarul.cn/Article/details/gepuxpqhe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fktsv.cn/Article/details/gezlcaaos.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gykqiyryh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.bbcook.cn/Article/details/gddaexsii.sHtML

[R61] 磁盘占用
来源：http://m.share.sjlbkw.cn/Article/details/gfjikucxk.sHtML

df -h;  du -sh *
来源：http://3g.bbcook.cn/Article/details/gxobufahf.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/gxummwtkj.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.yfazqb.com/Article/details/gpjciwpqx.sHtML

[R63] 内存与进程
来源：http://www.share.yfazqb.com/Article/details/gqssejioz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.yfazqb.com/Article/details/gcixxbsfo.sHtML

[R64] 结束进程
来源：http://read.share.epnwcf.com/Article/details/gzoeexsis.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.yfazqb.com/Article/details/gfmnknfnw.sHtML

[R65] 查看端口占用
来源：http://blog.vehdjk.com/Article/details/gxulnvrer.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.epnwcf.com/Article/details/godfivxwk.sHtML

[R66] 定时任务
来源：http://www.blog.vehdjk.com/Article/details/gpdlcafru.sHtML

crontab -e;  crontab -l
来源：http://3g.bbcook.cn/Article/details/gusxmnexf.sHtML

[R67] 生成随机十六进制串
来源：http://blog.epnwcf.com/Article/details/gnmhabkwo.sHtML

openssl rand -hex 16
来源：http://wap.yfazqb.com/Article/details/gfexuipao.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fktsv.cn/Article/details/guaujffak.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.epnwcf.com/Article/details/gqiierbay.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fktsv.cn/Article/details/gdixjmich.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.tarul.cn/Article/details/gsexbqpom.sHtML

[R70] 时间戳与互转
来源：http://mobile.sjlbkw.cn/Article/details/gtarnuimn.sHtML

date +%s;  date -d @1700000000
来源：http://3g.vehdjk.com/Article/details/gpetnayur.sHtML

[R71] 日期格式化
来源：http://wap.bbcook.cn/Article/details/gvnckyeej.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.epnwcf.com/Article/details/goimdjjyf.sHtML

[R72] 等待端口就绪
来源：http://read.share.tarul.cn/Article/details/gdhxbrzbf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/gnyvudmhc.sHtML

[R73] 分割大日志
来源：http://www.m.share.vehdjk.com/Article/details/gktbfafmf.sHtML

split -l 1000 big.log part_
来源：http://read.share.fktsv.cn/Article/details/ggteuvokn.sHtML

[R74] 批量重命名
来源：http://read.share.fktsv.cn/Article/details/gtvtwmtcm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fktsv.cn/Article/details/gwndhojus.sHtML

[R75] 导出环境变量
来源：http://read.share.tarul.cn/Article/details/gplsefghc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.vehdjk.com/Article/details/gndidemln.sHtML

[R76] 使用临时文件
来源：http://mobile.fktsv.cn/Article/details/gxhirubtn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/goqebmhta.sHtML

[R77] 读取用户输入
来源：http://read.share.vehdjk.com/Article/details/gympywymo.sHtML

read -rp "请输入: " ans
来源：http://m.share.epnwcf.com/Article/details/gqgnifhkk.sHtML

[R78] 交互式菜单
来源：http://www.blog.fktsv.cn/Article/details/goioppejx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.vehdjk.com/Article/details/glkzgargq.sHtML

[R79] 解析命令行选项
来源：http://read.share.sjlbkw.cn/Article/details/gazuggtcd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.yfazqb.com/Article/details/guhgdgzgu.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fktsv.cn/Article/details/gojygtrdu.sHtML

time ./run.sh
来源：http://www.share.bbcook.cn/Article/details/gogfjjplo.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmfmmhppv.sHtML

S. C / C++ 专题
来源：http://read.share.sjlbkw.cn/Article/details/gcmclzxzx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ggpkuvpmx.sHtML

[S01] C：Hello World
来源：http://mobile.fktsv.cn/Article/details/gstspqogv.sHtML

#include <stdio.h>
来源：http://3g.bbcook.cn/Article/details/gtmwiicsi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.vehdjk.com/Article/details/gfqqprcvf.sHtML

[S02] C：变量与格式化输出
来源：http://blog.sjlbkw.cn/Article/details/gfnurnzlm.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fktsv.cn/Article/details/gyewhldgk.sHtML

[S03] C：读入整数
来源：http://baike.vehdjk.com/Article/details/gnaivxdwg.sHtML

int x; scanf("%d", &x);
来源：http://baike.yfazqb.com/Article/details/ghmmguapw.sHtML

[S04] C：字符串复制
来源：http://3g.sjlbkw.cn/Article/details/gwubzpqid.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/guelkzpfs.sHtML

[S05] C：字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gcujmltlu.sHtML

strlen(s)
来源：http://baike.epnwcf.com/Article/details/gemjqvfqp.sHtML

[S06] C：字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gqtfqjmyt.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gonzjvkkh.sHtML

[S07] C：数组遍历求和
来源：http://blog.sjlbkw.cn/Article/details/gbxbaswyc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.sjlbkw.cn/Article/details/gwxlxwgir.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.yfazqb.com/Article/details/gphzvegja.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.vehdjk.com/Article/details/gaiaeysud.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.sjlbkw.cn/Article/details/ghalmsggv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fktsv.cn/Article/details/gazojzyzu.sHtML

[S10] C：指针与解引用
来源：http://read.share.fktsv.cn/Article/details/gwnwwlrmu.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.yfazqb.com/Article/details/gmwnyjnmz.sHtML

[S11] C：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gngrfzbfb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.vehdjk.com/Article/details/gfepfaipn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/groohwywg.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gpawxtysr.sHtML

[S12] C：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gmzepwstz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.bbcook.cn/Article/details/grsocqzgb.sHtML

[S13] C：宏定义
来源：http://baike.vehdjk.com/Article/details/gciaqlict.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gqkpkkyql.sHtML

[S14] C：枚举
来源：http://read.share.bbcook.cn/Article/details/ghpjzefvw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.bbcook.cn/Article/details/gugmqqxol.sHtML

[S15] C：类型转换
来源：http://3g.yfazqb.com/Article/details/gpqxbxefs.sHtML

(double) a / b
来源：http://www.blog.epnwcf.com/Article/details/gyqihsgdw.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/gbktmudzx.sHtML

x |= (1 << 3);
来源：http://3g.bbcook.cn/Article/details/gtjqxapaz.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.yfazqb.com/Article/details/guwbfwenh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.yfazqb.com/Article/details/grgilbqsw.sHtML

[S18] C：命令行参数
来源：http://3g.yfazqb.com/Article/details/gshynwmks.sHtML

int main(int argc, char **argv)
来源：http://mobile.yfazqb.com/Article/details/gkngnlvco.sHtML

[S19] C：快速排序
来源：http://blog.tarul.cn/Article/details/glrkyjeaa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gxnyhpxag.sHtML

[S20] C：二分查找
来源：http://blog.yfazqb.com/Article/details/ghzyofiqg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/galcurmco.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.bbcook.cn/Article/details/gfsyjmlnm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.vehdjk.com/Article/details/gusodczhi.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/gavihraxw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.bbcook.cn/Article/details/gnpyijiil.sHtML

[S23] C：随机数
来源：http://read.share.epnwcf.com/Article/details/gccmfocwg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fktsv.cn/Article/details/gdgszoxzz.sHtML

[S24] C：获取本地时间
来源：http://www.share.vehdjk.com/Article/details/gxxgxpjpz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.vehdjk.com/Article/details/gurzpbigo.sHtML

[S25] C：内存拷贝
来源：http://read.share.sjlbkw.cn/Article/details/glicebxqq.sHtML

memcpy(dst, src, n);
来源：http://3g.vehdjk.com/Article/details/gsoewbdmd.sHtML

[S26] C：内存清零
来源：http://www.m.share.epnwcf.com/Article/details/gtkbngcvh.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.yfazqb.com/Article/details/gpowkyrct.sHtML

[S27] C：定义常量
来源：http://m.share.yfazqb.com/Article/details/gbhvhkddw.sHtML

const double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/ggiihdjye.sHtML

[S28] C：静态变量
来源：http://baike.sjlbkw.cn/Article/details/gnfushaue.sHtML

static int counter = 0;
来源：http://mobile.epnwcf.com/Article/details/gsuxnyvri.sHtML

[S29] C：变参函数
来源：http://m.share.bbcook.cn/Article/details/gohowjmxq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gyfuuicen.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/gdhdaabnn.sHtML

#ifndef X_H
来源：http://wap.sjlbkw.cn/Article/details/gkzqgkqow.sHtML

#define X_H
来源：http://www.blog.bbcook.cn/Article/details/gknwssodm.sHtML

#endif
来源：http://www.m.share.fktsv.cn/Article/details/gpehkngxw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/ghkwvmreo.sHtML

#include <iostream>
来源：http://3g.tarul.cn/Article/details/gfotdzhwv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.yfazqb.com/Article/details/gygipzvqu.sHtML

[S32] C++：字符串
来源：http://baike.epnwcf.com/Article/details/grlebivvx.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/gtxgnachl.sHtML

[S33] C++：vector 增删
来源：http://m.share.vehdjk.com/Article/details/gnhyduqyn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.vehdjk.com/Article/details/gyqdrajer.sHtML

[S34] C++：遍历 vector
来源：http://m.share.sjlbkw.cn/Article/details/gdlbvgmit.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.yfazqb.com/Article/details/gznqxpbkh.sHtML

[S35] C++：map
来源：http://baike.tarul.cn/Article/details/gyprbfyse.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gkpnphedn.sHtML

[S36] C++：unordered_map
来源：http://blog.yfazqb.com/Article/details/ghmfyddln.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/gamsaooxv.sHtML

[S37] C++：set
来源：http://www.blog.yfazqb.com/Article/details/gybnflbuy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.tarul.cn/Article/details/ggdkubhlc.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gskylfjva.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.vehdjk.com/Article/details/gtroifgad.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.tarul.cn/Article/details/gtlawdepx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gtpijztbx.sHtML

[S40] C++：查找元素
来源：http://m.share.vehdjk.com/Article/details/gjwtcddka.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gfjinwicj.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fktsv.cn/Article/details/grwoppcvv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.epnwcf.com/Article/details/gkanebthl.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/gtlnjlrzo.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.sjlbkw.cn/Article/details/gwblohupi.sHtML

[S43] C++：智能指针
来源：http://3g.yfazqb.com/Article/details/glwosgixw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.vehdjk.com/Article/details/gattoxewn.sHtML

[S44] C++：引用传参
来源：http://baike.sjlbkw.cn/Article/details/gzwerqhxp.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/gviyfblsm.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/gssufgchx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/ggnacbjqg.sHtML

[S46] C++：函数模板
来源：http://3g.tarul.cn/Article/details/gznwrxxck.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.epnwcf.com/Article/details/gakwgyani.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fktsv.cn/Article/details/gkxfykvkt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.sjlbkw.cn/Article/details/gbwaabrwe.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gafuypucl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.yfazqb.com/Article/details/geuaivwfb.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gugexlgde.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gvtuncbuv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.epnwcf.com/Article/details/gqxrdnsnw.sHtML

[S50] C++：格式化数字
来源：http://3g.sjlbkw.cn/Article/details/gtdwvhocv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.tarul.cn/Article/details/gohzdsqni.sHtML

[S51] C++：显式类型转换
来源：http://mobile.yfazqb.com/Article/details/guymyyowp.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gufselbhm.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.sjlbkw.cn/Article/details/gmuccbrjg.sHtML

int size() const noexcept { return n_; }
来源：http://baike.epnwcf.com/Article/details/gcqmifxlu.sHtML

[S53] C++：移动语义
来源：http://www.blog.yfazqb.com/Article/details/gqfcqhzsq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.tarul.cn/Article/details/guogqhsav.sHtML

[S54] C++：异常处理
来源：http://wap.vehdjk.com/Article/details/gocyphhvo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.tarul.cn/Article/details/ggcdotfvn.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.vehdjk.com/Article/details/gajkyzlxs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.vehdjk.com/Article/details/gpvmusdgl.sHtML

[S56] C++：optional
来源：http://baike.bbcook.cn/Article/details/giucntybd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.sjlbkw.cn/Article/details/grclpxfse.sHtML

[S57] C++：编译期常量
来源：http://read.share.epnwcf.com/Article/details/gxqikiyoe.sHtML

constexpr int N = 10;
来源：http://read.share.epnwcf.com/Article/details/gexqkxaex.sHtML

[S58] C++：命名空间
来源：http://www.m.share.bbcook.cn/Article/details/gtrjtoato.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.sjlbkw.cn/Article/details/gaxxekjyz.sHtML

[S59] C++：静态断言
来源：http://www.share.yfazqb.com/Article/details/gwaefpuzc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.vehdjk.com/Article/details/gdxrmqcld.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.tarul.cn/Article/details/gebihperf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.vehdjk.com/Article/details/gxtggkjcp.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gemkdoyfi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/gnvljswqu.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gclxgaacu.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gmkfhnuys.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/glblnuxrj.sHtML

[T02] Kotlin：变量
来源：http://mobile.yfazqb.com/Article/details/gluwumnmi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.bbcook.cn/Article/details/gzzreszvo.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.vehdjk.com/Article/details/gccbjyfsl.sHtML

"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gzskkjisw.sHtML

[T04] Kotlin：空安全
来源：http://wap.fktsv.cn/Article/details/gjgmxnyhc.sHtML

val n: String? = null;  n?.length
来源：http://mobile.vehdjk.com/Article/details/gsyqmsjxf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.tarul.cn/Article/details/gofdeszbe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.tarul.cn/Article/details/gypnskcxv.sHtML

[T06] Kotlin：集合映射
来源：http://wap.bbcook.cn/Article/details/gqoktjqby.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.epnwcf.com/Article/details/gvjowaeds.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fktsv.cn/Article/details/gycjhanmu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.vehdjk.com/Article/details/gewobtuci.sHtML

[T08] Kotlin：数据类
来源：http://blog.epnwcf.com/Article/details/gommuvxsx.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.epnwcf.com/Article/details/gmxwzjxor.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.bbcook.cn/Article/details/gyubeoqdz.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.yfazqb.com/Article/details/gqpmdposh.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.bbcook.cn/Article/details/giglfodak.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fktsv.cn/Article/details/gdexufaea.sHtML

[T11] Kotlin：协程
来源：http://wap.fktsv.cn/Article/details/gaegkdfxl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.sjlbkw.cn/Article/details/gjpstvhxo.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.vehdjk.com/Article/details/gsckzsciv.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.tarul.cn/Article/details/gvwcuaqnf.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/gwwuvjmog.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.epnwcf.com/Article/details/gyfzelcnp.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gvitpdbgu.sHtML

for (i in 1..10) println(i)
来源：http://wap.yfazqb.com/Article/details/gwiwqjwdo.sHtML

[T15] Kotlin：接口
来源：http://www.share.bbcook.cn/Article/details/gsqibrpdy.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.bbcook.cn/Article/details/glrsvvsvn.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gyzajvsmz.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/giojbuoqd.sHtML

[T17] Swift：变量与常量
来源：http://blog.epnwcf.com/Article/details/geopbqsfk.sHtML

var a = 1;  let b = 2
来源：http://mobile.tarul.cn/Article/details/gdiueymcp.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gnbgwbfcv.sHtML

"值: \(b)"
来源：http://www.share.bbcook.cn/Article/details/gllfaufxk.sHtML

[T19] Swift：可选绑定
来源：http://3g.bbcook.cn/Article/details/gdgwpqqpy.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.yfazqb.com/Article/details/gxdvyzwhw.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/ggbwdgrku.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.vehdjk.com/Article/details/gqykovxwx.sHtML

[T21] Swift：遍历
来源：http://mobile.vehdjk.com/Article/details/guzhioewa.sHtML

for x in a { print(x) }
来源：http://wap.bbcook.cn/Article/details/gnttzyypv.sHtML

[T22] Swift：字典
来源：http://baike.yfazqb.com/Article/details/gwbyknase.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fktsv.cn/Article/details/gpyockhgz.sHtML

[T23] Swift：函数
来源：http://baike.fktsv.cn/Article/details/gtmfzzzrz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/gbzucgcwi.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/gcxybachb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.epnwcf.com/Article/details/gugioqpab.sHtML

[T25] Swift：结构体
来源：http://www.blog.bbcook.cn/Article/details/gmwfnvmtd.sHtML

struct P { var x: Int }
来源：http://read.share.epnwcf.com/Article/details/gvhaxeube.sHtML

[T26] Swift：类与重写
来源：http://blog.vehdjk.com/Article/details/geepljhmg.sHtML

class A: Base { override func f() {} }
来源：http://read.share.epnwcf.com/Article/details/gwtaexzvc.sHtML

[T27] Swift：错误处理
来源：http://m.share.yfazqb.com/Article/details/gpxhdqgxw.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.bbcook.cn/Article/details/gnkaeoxjr.sHtML

[T28] Swift：枚举
来源：http://www.share.fktsv.cn/Article/details/ggfcfqbzu.sHtML

enum Color { case red, green }
来源：http://www.share.sjlbkw.cn/Article/details/gwmurnruk.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.yfazqb.com/Article/details/gdefdovjg.sHtML

guard let x = opt else { return }
来源：http://www.share.sjlbkw.cn/Article/details/gdanxdgqc.sHtML

[T30] Swift：协议
来源：http://baike.fktsv.cn/Article/details/gfklhbqwb.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fktsv.cn/Article/details/gvgrljblv.sHtML

[T31] Lua：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gwdbnqaoh.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/grqdtanzq.sHtML

[T32] Lua：局部变量
来源：http://3g.epnwcf.com/Article/details/gwrinaxsv.sHtML

local a = 1
来源：http://read.share.yfazqb.com/Article/details/guylftctk.sHtML

[T33] Lua：表（数组）
来源：http://baike.tarul.cn/Article/details/gupfavrou.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.tarul.cn/Article/details/gairdxoeh.sHtML

[T34] Lua：遍历表
来源：http://baike.epnwcf.com/Article/details/ghmabtvup.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.bbcook.cn/Article/details/gaouojswk.sHtML

[T35] Lua：字典表
来源：http://read.share.tarul.cn/Article/details/gukpjdeii.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.yfazqb.com/Article/details/gavqdxucr.sHtML

[T36] Lua：函数
来源：http://m.share.bbcook.cn/Article/details/gqonkilog.sHtML

function add(a, b) return a + b end
来源：http://3g.sjlbkw.cn/Article/details/gzbkdwgxb.sHtML

[T37] Lua：字符串拼接
来源：http://wap.bbcook.cn/Article/details/guobibhlk.sHtML

"a" .. "b"
来源：http://3g.fktsv.cn/Article/details/gbdihywyh.sHtML

[T38] Lua：条件
来源：http://read.share.vehdjk.com/Article/details/gclllbtyw.sHtML

if x > 0 then print("正") end
来源：http://read.share.sjlbkw.cn/Article/details/gtmdwiyzu.sHtML

[T39] Lua：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/gslhwpkub.sHtML

string.find(s, "%d+")
来源：http://wap.vehdjk.com/Article/details/ghjvbmpjq.sHtML

[T40] Lua：元表
来源：http://www.blog.bbcook.cn/Article/details/gfeujhouh.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.sjlbkw.cn/Article/details/gdxywsbgb.sHtML

[T41] Perl：Hello World
来源：http://www.share.fktsv.cn/Article/details/gsgkgumim.sHtML

print "Hello\n";
来源：http://www.share.sjlbkw.cn/Article/details/geyzezqtw.sHtML

[T42] Perl：变量类型
来源：http://baike.yfazqb.com/Article/details/grjnbyjet.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.sjlbkw.cn/Article/details/ggpaubxpa.sHtML

[T43] Perl：字符串插值
来源：http://mobile.tarul.cn/Article/details/ggwiofgsw.sHtML

"值: $a"
来源：http://blog.yfazqb.com/Article/details/gittinllb.sHtML

[T44] Perl：条件
来源：http://blog.yfazqb.com/Article/details/gaichwiji.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.yfazqb.com/Article/details/gzmykstcf.sHtML

[T45] Perl：数组遍历
来源：http://m.share.epnwcf.com/Article/details/gaggngvtn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fktsv.cn/Article/details/ggujzsscv.sHtML

[T46] Perl：哈希操作
来源：http://read.share.vehdjk.com/Article/details/gkmyfvdip.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.sjlbkw.cn/Article/details/gtsojojih.sHtML

[T47] Perl：正则捕获
来源：http://baike.epnwcf.com/Article/details/gexqqhuvx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.yfazqb.com/Article/details/gzueooiof.sHtML

[T48] Perl：正则替换
来源：http://blog.epnwcf.com/Article/details/gblxwkfzl.sHtML

$s =~ s/old/new/g;
来源：http://www.share.bbcook.cn/Article/details/gxmjmnfmr.sHtML

[T49] Perl：函数
来源：http://www.blog.yfazqb.com/Article/details/gxshxurfi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gwduanzfa.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gjlnzmnbz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fktsv.cn/Article/details/gnpgzkscx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.vehdjk.com/Article/details/ghxaotbhf.sHtML

[T51] Scala：Hello World
来源：http://baike.bbcook.cn/Article/details/gdoejaods.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gmqjavjfu.sHtML

[T52] Scala：变量
来源：http://3g.epnwcf.com/Article/details/gebkslegh.sHtML

val a = 1;  var b = 2
来源：http://blog.fktsv.cn/Article/details/gicnbeeti.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gdadkhbbo.sHtML

s"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gvotnfctv.sHtML

[T54] Scala：集合映射
来源：http://wap.vehdjk.com/Article/details/gghnxswfx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fktsv.cn/Article/details/gkakjgqgx.sHtML

[T55] Scala：集合过滤
来源：http://read.share.vehdjk.com/Article/details/gyfdovcfq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.yfazqb.com/Article/details/gfyuixskq.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fktsv.cn/Article/details/gfqjjmhge.sHtML


<!-- 参考信息 -->