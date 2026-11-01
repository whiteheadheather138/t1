代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.epnwcf.com/Article/details/gwqdtozhp.sHtML

[R54] 比较两个文件
来源：http://read.share.sjlbkw.cn/Article/details/gylpakezb.sHtML

diff a.txt b.txt
来源：http://3g.yfazqb.com/Article/details/gcbuoqoyy.sHtML

[R55] 压缩与解压
来源：http://baike.vehdjk.com/Article/details/gnepnupit.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gmxfflpbv.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/gxxevdgex.sHtML

scp file user@host:/path/
来源：http://www.share.yfazqb.com/Article/details/gjjtlffyy.sHtML

[R57] 远程执行命令
来源：http://m.share.bbcook.cn/Article/details/gqmrqlyzj.sHtML

ssh user@host 'uptime'
来源：http://wap.tarul.cn/Article/details/gryjbeahr.sHtML

[R58] 下载文件
来源：http://mobile.tarul.cn/Article/details/gqkzypnut.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fktsv.cn/Article/details/gucxosbqc.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gexyhhdjm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.vehdjk.com/Article/details/gpysgzadg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/ghhffjjca.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fktsv.cn/Article/details/gexkcvnkk.sHtML

[R61] 磁盘占用
来源：http://baike.epnwcf.com/Article/details/gtyndhmoe.sHtML

df -h;  du -sh *
来源：http://wap.fktsv.cn/Article/details/gzhmuiqhl.sHtML

[R62] 找最占空间的文件
来源：http://baike.bbcook.cn/Article/details/gzlqhfsyi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fktsv.cn/Article/details/gudtgfgck.sHtML

[R63] 内存与进程
来源：http://mobile.yfazqb.com/Article/details/glhhueeqn.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fktsv.cn/Article/details/glrbawlor.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/galdoknnb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fktsv.cn/Article/details/gzjhqdqvl.sHtML

[R65] 查看端口占用
来源：http://baike.bbcook.cn/Article/details/gvxmmnuqt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fktsv.cn/Article/details/gmudicnng.sHtML

[R66] 定时任务
来源：http://www.share.sjlbkw.cn/Article/details/grwtfoapa.sHtML

crontab -e;  crontab -l
来源：http://3g.yfazqb.com/Article/details/gdmnsawhr.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fktsv.cn/Article/details/gcemzmqzh.sHtML

openssl rand -hex 16
来源：http://blog.epnwcf.com/Article/details/glyawiiqs.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdjereoq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.epnwcf.com/Article/details/gwcljjbad.sHtML

[R69] 生成随机密码
来源：http://read.share.epnwcf.com/Article/details/gdbgpkogb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.yfazqb.com/Article/details/gmsfgpqoq.sHtML

[R70] 时间戳与互转
来源：http://m.share.fktsv.cn/Article/details/gwsiebmcf.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fktsv.cn/Article/details/gvoghxiaa.sHtML

[R71] 日期格式化
来源：http://baike.vehdjk.com/Article/details/gukxiijtn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fktsv.cn/Article/details/gkmtuggtf.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.tarul.cn/Article/details/gamzqgwwa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gcinbxdos.sHtML

[R73] 分割大日志
来源：http://www.share.yfazqb.com/Article/details/glpamnxwf.sHtML

split -l 1000 big.log part_
来源：http://blog.bbcook.cn/Article/details/gspuosspk.sHtML

[R74] 批量重命名
来源：http://www.share.yfazqb.com/Article/details/gsyyrtgoz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpecliss.sHtML

[R75] 导出环境变量
来源：http://3g.vehdjk.com/Article/details/gemsffrkg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.epnwcf.com/Article/details/ggsryzxlw.sHtML

[R76] 使用临时文件
来源：http://www.share.fktsv.cn/Article/details/gwwpcmpir.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/gzlemwrzj.sHtML

[R77] 读取用户输入
来源：http://wap.sjlbkw.cn/Article/details/gkbrmrpjw.sHtML

read -rp "请输入: " ans
来源：http://www.share.fktsv.cn/Article/details/gzqnhdjcr.sHtML

[R78] 交互式菜单
来源：http://wap.sjlbkw.cn/Article/details/gadqecaiu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.sjlbkw.cn/Article/details/glqlcgimz.sHtML

[R79] 解析命令行选项
来源：http://read.share.sjlbkw.cn/Article/details/ggartnsju.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fktsv.cn/Article/details/gubbwzfeq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.tarul.cn/Article/details/gstmodglf.sHtML

time ./run.sh
来源：http://baike.vehdjk.com/Article/details/gjyvgwucu.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gllsxjjpn.sHtML

S. C / C++ 专题
来源：http://mobile.vehdjk.com/Article/details/gigzgjknk.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/grjacbxbf.sHtML

[S01] C：Hello World
来源：http://www.blog.epnwcf.com/Article/details/ghdsomftr.sHtML

#include <stdio.h>
来源：http://mobile.yfazqb.com/Article/details/gdzlvqdde.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/gccdtueds.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gzxfabfpo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fktsv.cn/Article/details/gusukmxzi.sHtML

[S03] C：读入整数
来源：http://3g.sjlbkw.cn/Article/details/ghttvaxlv.sHtML

int x; scanf("%d", &x);
来源：http://wap.epnwcf.com/Article/details/gbwgtnukz.sHtML

[S04] C：字符串复制
来源：http://3g.vehdjk.com/Article/details/glakdoybm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fktsv.cn/Article/details/gqsrnhdzf.sHtML

[S05] C：字符串长度
来源：http://baike.fktsv.cn/Article/details/gfduppwnb.sHtML

strlen(s)
来源：http://www.blog.tarul.cn/Article/details/ghyddpydn.sHtML

[S06] C：字符串比较
来源：http://baike.bbcook.cn/Article/details/genkhfhku.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.epnwcf.com/Article/details/geddwvifw.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.epnwcf.com/Article/details/gdobslzso.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.bbcook.cn/Article/details/gtzcrtqwk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.yfazqb.com/Article/details/gsrqpcueg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.vehdjk.com/Article/details/gbwzyftgn.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/gmqzllqwk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.epnwcf.com/Article/details/gfgrfnydw.sHtML

[S10] C：指针与解引用
来源：http://www.share.bbcook.cn/Article/details/gdaybonrh.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fktsv.cn/Article/details/gjzwodzmk.sHtML

[S11] C：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gnipsfznz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.vehdjk.com/Article/details/gefzhtmge.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gpyveucgp.sHtML

fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gppevkrhn.sHtML

[S12] C：写文件
来源：http://3g.bbcook.cn/Article/details/gnplilvhs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fktsv.cn/Article/details/ggjhgmvsv.sHtML

[S13] C：宏定义
来源：http://blog.tarul.cn/Article/details/gneagnuvh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/gsmprolxc.sHtML

[S14] C：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gvpwlchgd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.vehdjk.com/Article/details/gyujzprpq.sHtML

[S15] C：类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gasgpaqcu.sHtML

(double) a / b
来源：http://www.blog.epnwcf.com/Article/details/gmjhqktdw.sHtML

[S16] C：位操作置位
来源：http://mobile.bbcook.cn/Article/details/gygpnihbp.sHtML

x |= (1 << 3);
来源：http://blog.fktsv.cn/Article/details/gswpjaflb.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.tarul.cn/Article/details/gxhpbuzqr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjwfvsry.sHtML

[S18] C：命令行参数
来源：http://blog.tarul.cn/Article/details/gsjtfldwo.sHtML

int main(int argc, char **argv)
来源：http://www.blog.sjlbkw.cn/Article/details/gtlnmhhgn.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/gmnrdafca.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gduiptepp.sHtML

[S20] C：二分查找
来源：http://wap.fktsv.cn/Article/details/gmmmhvlkx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gvwxckftg.sHtML

[S21] C：字符类别判断
来源：http://baike.vehdjk.com/Article/details/geriewvjk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.vehdjk.com/Article/details/gqssqjcev.sHtML

[S22] C：字符串转数字
来源：http://m.share.sjlbkw.cn/Article/details/gmsinvtgu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.bbcook.cn/Article/details/gffkqnzke.sHtML

[S23] C：随机数
来源：http://baike.bbcook.cn/Article/details/gpaqfurml.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.epnwcf.com/Article/details/gxszdhsks.sHtML

[S24] C：获取本地时间
来源：http://wap.epnwcf.com/Article/details/gqhbxebbo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/gxkkqpcms.sHtML

[S25] C：内存拷贝
来源：http://mobile.tarul.cn/Article/details/guatzeczs.sHtML

memcpy(dst, src, n);
来源：http://www.share.vehdjk.com/Article/details/gmmmmllvw.sHtML

[S26] C：内存清零
来源：http://read.share.tarul.cn/Article/details/gomrxuiax.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.yfazqb.com/Article/details/gbhxoommc.sHtML

[S27] C：定义常量
来源：http://read.share.yfazqb.com/Article/details/glowsylsn.sHtML

const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/goktrlewh.sHtML

[S28] C：静态变量
来源：http://www.share.yfazqb.com/Article/details/gkjwyjgtx.sHtML

static int counter = 0;
来源：http://blog.vehdjk.com/Article/details/gtpexokmk.sHtML

[S29] C：变参函数
来源：http://www.m.share.vehdjk.com/Article/details/gyyksfqsu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.bbcook.cn/Article/details/gcwhqogwn.sHtML

[S30] C：头文件保护
来源：http://m.share.tarul.cn/Article/details/gxxjtfzon.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/gagsmblxj.sHtML

#define X_H
来源：http://www.share.vehdjk.com/Article/details/gnubvywcb.sHtML

#endif
来源：http://read.share.tarul.cn/Article/details/gulgnzxhm.sHtML

[S31] C++：Hello World
来源：http://3g.epnwcf.com/Article/details/gupatawri.sHtML

#include <iostream>
来源：http://m.share.bbcook.cn/Article/details/gxgclmbzp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.bbcook.cn/Article/details/gmsotwvab.sHtML

[S32] C++：字符串
来源：http://www.blog.epnwcf.com/Article/details/gdmirugqe.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.bbcook.cn/Article/details/glbgcceqb.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/gwxyzzawc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gqfsxafxi.sHtML

[S34] C++：遍历 vector
来源：http://read.share.bbcook.cn/Article/details/glruwwocq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.epnwcf.com/Article/details/geghangog.sHtML

[S35] C++：map
来源：http://mobile.tarul.cn/Article/details/grwedhvem.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gjwkyprct.sHtML

[S36] C++：unordered_map
来源：http://read.share.epnwcf.com/Article/details/gpvkzjufl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gzvmtrtmk.sHtML

[S37] C++：set
来源：http://m.share.epnwcf.com/Article/details/gikmecwur.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.tarul.cn/Article/details/girpkitye.sHtML

[S38] C++：排序
来源：http://www.blog.bbcook.cn/Article/details/gbbhpjjas.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.tarul.cn/Article/details/gbwnanqtc.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.sjlbkw.cn/Article/details/greqslypq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.bbcook.cn/Article/details/ghdslacgu.sHtML

[S40] C++：查找元素
来源：http://baike.sjlbkw.cn/Article/details/gzoxbqvqq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.sjlbkw.cn/Article/details/gjokbafcu.sHtML

[S41] C++：类与构造函数
来源：http://baike.bbcook.cn/Article/details/guiuglcbf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.sjlbkw.cn/Article/details/geczjynle.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fktsv.cn/Article/details/gblqvosxs.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.tarul.cn/Article/details/gtigenavb.sHtML

[S43] C++：智能指针
来源：http://www.m.share.vehdjk.com/Article/details/gqwdynrzo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gahqvrwre.sHtML

[S44] C++：引用传参
来源：http://baike.vehdjk.com/Article/details/gelhsscfh.sHtML

void inc(int &x) { ++x; }
来源：http://baike.yfazqb.com/Article/details/gifuoesrg.sHtML

[S45] C++：lambda
来源：http://www.blog.epnwcf.com/Article/details/gyfxfqehs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.yfazqb.com/Article/details/gdhoqornw.sHtML

[S46] C++：函数模板
来源：http://read.share.tarul.cn/Article/details/gtacsojsq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.tarul.cn/Article/details/gfdpaellx.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fktsv.cn/Article/details/gdhqigqik.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.tarul.cn/Article/details/gtcugcwpl.sHtML

[S48] C++：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gozsjvlse.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.vehdjk.com/Article/details/gtjbfuiwq.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fktsv.cn/Article/details/gixcgicwb.sHtML

[S49] C++：写文件
来源：http://www.blog.epnwcf.com/Article/details/gyrrlmnzk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.tarul.cn/Article/details/ggqwoknqy.sHtML

[S50] C++：格式化数字
来源：http://mobile.sjlbkw.cn/Article/details/gkagdbbgy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gtjamhrud.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gcrugrbsw.sHtML

static_cast<double>(a) / b
来源：http://3g.fktsv.cn/Article/details/gjulhhkoo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.sjlbkw.cn/Article/details/ggyaavspq.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/gvwjbzkij.sHtML

[S53] C++：移动语义
来源：http://blog.bbcook.cn/Article/details/gosalgjeu.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.tarul.cn/Article/details/glyxpsdzz.sHtML

[S54] C++：异常处理
来源：http://m.share.sjlbkw.cn/Article/details/gysvhkreo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.tarul.cn/Article/details/gxdcfekep.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fktsv.cn/Article/details/gedzympgo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.bbcook.cn/Article/details/gondobroj.sHtML

[S56] C++：optional
来源：http://baike.vehdjk.com/Article/details/ghdpvzjad.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.bbcook.cn/Article/details/gdnklhzeo.sHtML

[S57] C++：编译期常量
来源：http://www.share.yfazqb.com/Article/details/glcowfzln.sHtML

constexpr int N = 10;
来源：http://blog.vehdjk.com/Article/details/gwoeuxgaw.sHtML

[S58] C++：命名空间
来源：http://baike.tarul.cn/Article/details/ggmomqcdg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gvywrbjre.sHtML

[S59] C++：静态断言
来源：http://wap.bbcook.cn/Article/details/gutncqmgf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fktsv.cn/Article/details/glpwkjpnp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.tarul.cn/Article/details/ghyvcnqmp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gjtlzqczt.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gblhpzcrm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.yfazqb.com/Article/details/gznhbeyhh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnuczgjur.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gtfqgskdz.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gyxivkfbe.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/ghkqabndj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/gncrnefae.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.vehdjk.com/Article/details/glkargeqa.sHtML

"值: $b"
来源：http://www.share.epnwcf.com/Article/details/grswrrfwj.sHtML

[T04] Kotlin：空安全
来源：http://baike.vehdjk.com/Article/details/grgeehyok.sHtML

val n: String? = null;  n?.length
来源：http://m.share.vehdjk.com/Article/details/gvgfxgqqf.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.vehdjk.com/Article/details/gyzmubqgd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.yfazqb.com/Article/details/gqcwezspf.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.bbcook.cn/Article/details/gburyrhav.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.yfazqb.com/Article/details/gegxabomi.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.tarul.cn/Article/details/gcmlvgtkb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.epnwcf.com/Article/details/grgpkidxa.sHtML

[T08] Kotlin：数据类
来源：http://3g.yfazqb.com/Article/details/gwaxolqey.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.yfazqb.com/Article/details/gfnvsiflg.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.bbcook.cn/Article/details/gcmnklisv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.yfazqb.com/Article/details/gtlyhfozu.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.epnwcf.com/Article/details/gvuaudcsv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/gpoellbrp.sHtML

[T11] Kotlin：协程
来源：http://blog.epnwcf.com/Article/details/gpxqfvsnj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.epnwcf.com/Article/details/gxxixhbhx.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.vehdjk.com/Article/details/gdsmvqbnz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gjvmojzkk.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.vehdjk.com/Article/details/gpubvbjif.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.epnwcf.com/Article/details/gflkhepxf.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/gbdjqfabb.sHtML

for (i in 1..10) println(i)
来源：http://blog.epnwcf.com/Article/details/gsgzstbkf.sHtML

[T15] Kotlin：接口
来源：http://blog.tarul.cn/Article/details/gnomyahrb.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gvyfwtfad.sHtML

[T16] Swift：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/grgamotye.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/gyfxfhqar.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.vehdjk.com/Article/details/gwebcofrh.sHtML

var a = 1;  let b = 2
来源：http://baike.fktsv.cn/Article/details/gshylhdad.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gabczeexg.sHtML

"值: \(b)"
来源：http://blog.bbcook.cn/Article/details/gxjeuyqbj.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.vehdjk.com/Article/details/glugpicdw.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fktsv.cn/Article/details/gmpymgvaq.sHtML

[T20] Swift：数组操作
来源：http://m.share.epnwcf.com/Article/details/gnyexsdvf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.bbcook.cn/Article/details/gmonktubf.sHtML

[T21] Swift：遍历
来源：http://read.share.sjlbkw.cn/Article/details/gbllzionp.sHtML

for x in a { print(x) }
来源：http://mobile.bbcook.cn/Article/details/gzerhrexs.sHtML

[T22] Swift：字典
来源：http://www.blog.sjlbkw.cn/Article/details/gkblnewrx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.bbcook.cn/Article/details/gssrjmiac.sHtML

[T23] Swift：函数
来源：http://mobile.tarul.cn/Article/details/gifqffqfp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.yfazqb.com/Article/details/gpapglvxw.sHtML

[T24] Swift：闭包
来源：http://mobile.sjlbkw.cn/Article/details/gxbhrzeww.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gyvgoeias.sHtML

[T25] Swift：结构体
来源：http://3g.vehdjk.com/Article/details/gbgpuijqp.sHtML

struct P { var x: Int }
来源：http://mobile.tarul.cn/Article/details/gsnlsyjbj.sHtML

[T26] Swift：类与重写
来源：http://3g.fktsv.cn/Article/details/gfbcavgfu.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.yfazqb.com/Article/details/gqpkwfsjf.sHtML

[T27] Swift：错误处理
来源：http://blog.vehdjk.com/Article/details/ggctldgun.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fktsv.cn/Article/details/ggxfentkz.sHtML

[T28] Swift：枚举
来源：http://www.share.bbcook.cn/Article/details/gjgoqwwhm.sHtML

enum Color { case red, green }
来源：http://www.share.sjlbkw.cn/Article/details/gicljchtc.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.bbcook.cn/Article/details/griyapagi.sHtML

guard let x = opt else { return }
来源：http://read.share.sjlbkw.cn/Article/details/ggsobkokh.sHtML

[T30] Swift：协议
来源：http://blog.bbcook.cn/Article/details/givpcacga.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.yfazqb.com/Article/details/grolqbpwl.sHtML

[T31] Lua：Hello World
来源：http://blog.sjlbkw.cn/Article/details/glabpoanb.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/grzvwbhux.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.tarul.cn/Article/details/gvxoyeegx.sHtML

local a = 1
来源：http://www.blog.sjlbkw.cn/Article/details/gvzdkotwn.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.epnwcf.com/Article/details/glgxlueyu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.yfazqb.com/Article/details/giihjprtv.sHtML

[T34] Lua：遍历表
来源：http://baike.vehdjk.com/Article/details/giaiyvuee.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.vehdjk.com/Article/details/gpyojrpjh.sHtML

[T35] Lua：字典表
来源：http://www.blog.vehdjk.com/Article/details/ghoqqqakj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.vehdjk.com/Article/details/gmmwadrnv.sHtML

[T36] Lua：函数
来源：http://read.share.tarul.cn/Article/details/gblczwjks.sHtML

function add(a, b) return a + b end
来源：http://mobile.tarul.cn/Article/details/gafspqwjl.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gaqzbmxiz.sHtML

"a" .. "b"
来源：http://www.m.share.bbcook.cn/Article/details/gaadwbcpo.sHtML

[T38] Lua：条件
来源：http://baike.sjlbkw.cn/Article/details/gptodylts.sHtML

if x > 0 then print("正") end
来源：http://mobile.yfazqb.com/Article/details/garezepwu.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fktsv.cn/Article/details/gcnayzwxg.sHtML

string.find(s, "%d+")
来源：http://www.share.tarul.cn/Article/details/gmfbzbfse.sHtML

[T40] Lua：元表
来源：http://blog.bbcook.cn/Article/details/gwsnbagua.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fktsv.cn/Article/details/gmbqjtkoq.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gzorlkphx.sHtML

print "Hello\n";
来源：http://www.m.share.fktsv.cn/Article/details/geojcnhzd.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fktsv.cn/Article/details/gkpnypxgg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.epnwcf.com/Article/details/gkpjlylho.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/glfmdjwtl.sHtML

"值: $a"
来源：http://www.share.yfazqb.com/Article/details/gzrutfzen.sHtML

[T44] Perl：条件
来源：http://mobile.sjlbkw.cn/Article/details/gmrklseay.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fktsv.cn/Article/details/gummndltu.sHtML

[T45] Perl：数组遍历
来源：http://read.share.bbcook.cn/Article/details/gbmahsuuq.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.yfazqb.com/Article/details/gcyxrerww.sHtML

[T46] Perl：哈希操作
来源：http://baike.tarul.cn/Article/details/gthefozha.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.bbcook.cn/Article/details/gjvvgtxcn.sHtML

[T47] Perl：正则捕获
来源：http://read.share.tarul.cn/Article/details/gekdscpbt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.vehdjk.com/Article/details/gcxhgszsh.sHtML

[T48] Perl：正则替换
来源：http://wap.yfazqb.com/Article/details/gcvuyxipi.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fktsv.cn/Article/details/gasmdbbnp.sHtML

[T49] Perl：函数
来源：http://baike.epnwcf.com/Article/details/gutvmjgrv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/ggolmasne.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gehcwfcxm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.bbcook.cn/Article/details/gmuzyiold.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.epnwcf.com/Article/details/gdxvhcgbw.sHtML

[T51] Scala：Hello World
来源：http://3g.bbcook.cn/Article/details/gagzwvqfs.sHtML

println("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gdrfdymqz.sHtML

[T52] Scala：变量
来源：http://mobile.bbcook.cn/Article/details/gciptcedp.sHtML

val a = 1;  var b = 2
来源：http://m.share.fktsv.cn/Article/details/gajkdabkq.sHtML

[T53] Scala：字符串插值
来源：http://3g.tarul.cn/Article/details/gfnotnxyz.sHtML

s"值: $b"
来源：http://www.share.epnwcf.com/Article/details/gdeieceeu.sHtML

[T54] Scala：集合映射
来源：http://3g.fktsv.cn/Article/details/ghcjsncch.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.vehdjk.com/Article/details/gsgefhqwc.sHtML

[T55] Scala：集合过滤
来源：http://mobile.epnwcf.com/Article/details/gjelhwprn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.tarul.cn/Article/details/gssyehjsr.sHtML

[T56] Scala：样例类
来源：http://blog.sjlbkw.cn/Article/details/gaodezows.sHtML


<!-- 参考信息 -->