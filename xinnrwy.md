代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.vehdjk.com/Article/details/gxfxstolw.sHtML

[R52] 统计行数
来源：http://www.blog.fktsv.cn/Article/details/gxbpszhqm.sHtML

wc -l a.txt
来源：http://wap.epnwcf.com/Article/details/goepiekmr.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fktsv.cn/Article/details/gcynbqxvr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fktsv.cn/Article/details/gmfqpllit.sHtML

[R54] 比较两个文件
来源：http://read.share.tarul.cn/Article/details/ggirmrzpa.sHtML

diff a.txt b.txt
来源：http://baike.tarul.cn/Article/details/gvrzmddqe.sHtML

[R55] 压缩与解压
来源：http://m.share.epnwcf.com/Article/details/gwuycyysw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.epnwcf.com/Article/details/ghjvpjsre.sHtML

[R56] 远程拷贝
来源：http://3g.fktsv.cn/Article/details/ghrvkyhaa.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/gebluefxq.sHtML

[R57] 远程执行命令
来源：http://www.blog.epnwcf.com/Article/details/gaocznugk.sHtML

ssh user@host 'uptime'
来源：http://read.share.sjlbkw.cn/Article/details/guwmbzdco.sHtML

[R58] 下载文件
来源：http://baike.yfazqb.com/Article/details/gpvpvrqru.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.yfazqb.com/Article/details/gadejssff.sHtML

[R59] 发 POST JSON
来源：http://wap.bbcook.cn/Article/details/gvqaywqec.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.bbcook.cn/Article/details/gvprtptpv.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/ghhihhuyi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fktsv.cn/Article/details/gobouzysy.sHtML

[R61] 磁盘占用
来源：http://blog.yfazqb.com/Article/details/gwnuxqmvx.sHtML

df -h;  du -sh *
来源：http://mobile.vehdjk.com/Article/details/gwvuiogzo.sHtML

[R62] 找最占空间的文件
来源：http://wap.epnwcf.com/Article/details/gcgkmhcjl.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.bbcook.cn/Article/details/gidkwihwr.sHtML

[R63] 内存与进程
来源：http://mobile.fktsv.cn/Article/details/greohhvrk.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.vehdjk.com/Article/details/gqszvrkio.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gdwmzegjd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.sjlbkw.cn/Article/details/gjorigbwr.sHtML

[R65] 查看端口占用
来源：http://baike.sjlbkw.cn/Article/details/ghbxcojiv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.tarul.cn/Article/details/gckdgnwyu.sHtML

[R66] 定时任务
来源：http://baike.fktsv.cn/Article/details/gttghmlmu.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/gosdajwwy.sHtML

[R67] 生成随机十六进制串
来源：http://blog.yfazqb.com/Article/details/gqtrpbakd.sHtML

openssl rand -hex 16
来源：http://www.m.share.yfazqb.com/Article/details/gsnmnmjfr.sHtML

[R68] 计算文件校验值
来源：http://3g.fktsv.cn/Article/details/grasywkhj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.vehdjk.com/Article/details/geyodiowi.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/gvngwjvzx.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.bbcook.cn/Article/details/gbxjfyrue.sHtML

[R70] 时间戳与互转
来源：http://mobile.yfazqb.com/Article/details/gaunsbxwg.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.tarul.cn/Article/details/gcclsbyaz.sHtML

[R71] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gmfudiieh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fktsv.cn/Article/details/gqsybcevy.sHtML

[R72] 等待端口就绪
来源：http://www.blog.sjlbkw.cn/Article/details/gpdopagrm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/gnorwglln.sHtML

[R73] 分割大日志
来源：http://blog.fktsv.cn/Article/details/gknbdkraj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.vehdjk.com/Article/details/gaydcrjzq.sHtML

[R74] 批量重命名
来源：http://3g.yfazqb.com/Article/details/gfmwaovxq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fktsv.cn/Article/details/gvkersbbp.sHtML

[R75] 导出环境变量
来源：http://www.blog.yfazqb.com/Article/details/glalhkgfv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fktsv.cn/Article/details/gakjoasdd.sHtML

[R76] 使用临时文件
来源：http://3g.bbcook.cn/Article/details/gtqydoble.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.vehdjk.com/Article/details/gjlbiwyye.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/gzjaobeti.sHtML

read -rp "请输入: " ans
来源：http://m.share.epnwcf.com/Article/details/gksixnswj.sHtML

[R78] 交互式菜单
来源：http://blog.epnwcf.com/Article/details/ghebiwrbn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.tarul.cn/Article/details/gekwuzltn.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fktsv.cn/Article/details/gyrgzlyty.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.sjlbkw.cn/Article/details/ghrqdyxcm.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fktsv.cn/Article/details/grshdjgzw.sHtML

time ./run.sh
来源：http://wap.yfazqb.com/Article/details/gyghzsonz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ggqfmlbem.sHtML

S. C / C++ 专题
来源：http://read.share.yfazqb.com/Article/details/gvhpnerhh.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gxbzicycw.sHtML

[S01] C：Hello World
来源：http://m.share.bbcook.cn/Article/details/gndpttoci.sHtML

#include <stdio.h>
来源：http://mobile.vehdjk.com/Article/details/gzubkmrvl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fktsv.cn/Article/details/gwdouezlg.sHtML

[S02] C：变量与格式化输出
来源：http://3g.yfazqb.com/Article/details/geoziwuck.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.yfazqb.com/Article/details/gjcvhjxti.sHtML

[S03] C：读入整数
来源：http://blog.vehdjk.com/Article/details/gayeucxqm.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/gtskicizw.sHtML

[S04] C：字符串复制
来源：http://blog.bbcook.cn/Article/details/glnkbczqa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gpctagjsd.sHtML

[S05] C：字符串长度
来源：http://wap.bbcook.cn/Article/details/gzuigfohi.sHtML

strlen(s)
来源：http://www.blog.epnwcf.com/Article/details/gssxogrnb.sHtML

[S06] C：字符串比较
来源：http://baike.tarul.cn/Article/details/gvfgtlxkm.sHtML

strcmp(a, b) == 0
来源：http://mobile.vehdjk.com/Article/details/ggbmqqtzq.sHtML

[S07] C：数组遍历求和
来源：http://blog.fktsv.cn/Article/details/guqumnatk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/ghqsqkwgv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.bbcook.cn/Article/details/gpikcmjqn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.yfazqb.com/Article/details/gubaiyewl.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.tarul.cn/Article/details/goqyvuifz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.tarul.cn/Article/details/gcsndftqk.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gzcucidfl.sHtML

int *p = &a;  *p = 5;
来源：http://baike.epnwcf.com/Article/details/gbqyvamcx.sHtML

[S11] C：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/glmkjdngn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.sjlbkw.cn/Article/details/gaekdfklb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.bbcook.cn/Article/details/gkmwncsev.sHtML

fclose(f);
来源：http://3g.epnwcf.com/Article/details/gspooggkl.sHtML

[S12] C：写文件
来源：http://blog.yfazqb.com/Article/details/gfwdchvgj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gmbhidbnb.sHtML

[S13] C：宏定义
来源：http://www.blog.bbcook.cn/Article/details/gicqbtjli.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.epnwcf.com/Article/details/gqbhfuzch.sHtML

[S14] C：枚举
来源：http://read.share.vehdjk.com/Article/details/gmxgcnjao.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.sjlbkw.cn/Article/details/gyypcpiqe.sHtML

[S15] C：类型转换
来源：http://wap.bbcook.cn/Article/details/gbhxrjzja.sHtML

(double) a / b
来源：http://wap.yfazqb.com/Article/details/gtagzwkfg.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/gtowekhox.sHtML

x |= (1 << 3);
来源：http://read.share.yfazqb.com/Article/details/grxwqzfte.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gssuwgmtr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.epnwcf.com/Article/details/gsgjbapqj.sHtML

[S18] C：命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gbgmhzosl.sHtML

int main(int argc, char **argv)
来源：http://wap.vehdjk.com/Article/details/glfmoqqcz.sHtML

[S19] C：快速排序
来源：http://mobile.sjlbkw.cn/Article/details/gpkxkddvj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gxrbvkbek.sHtML

[S20] C：二分查找
来源：http://www.m.share.fktsv.cn/Article/details/gtelixfqf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gegnafams.sHtML

[S21] C：字符类别判断
来源：http://mobile.sjlbkw.cn/Article/details/gpvsraimn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.tarul.cn/Article/details/guxbfdzeq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/gkipxcrla.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.tarul.cn/Article/details/gjeczdntz.sHtML

[S23] C：随机数
来源：http://m.share.tarul.cn/Article/details/gvagmikjp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/gsbveruqk.sHtML

[S24] C：获取本地时间
来源：http://baike.fktsv.cn/Article/details/gamrycvus.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.bbcook.cn/Article/details/gagkufhgp.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gjujzqfiz.sHtML

memcpy(dst, src, n);
来源：http://blog.epnwcf.com/Article/details/grqtyzaiu.sHtML

[S26] C：内存清零
来源：http://wap.bbcook.cn/Article/details/gqimnsqaa.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fktsv.cn/Article/details/gcmkoewvw.sHtML

[S27] C：定义常量
来源：http://m.share.vehdjk.com/Article/details/gohelukrw.sHtML

const double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/glsttpmzp.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/gkybkhmmv.sHtML

static int counter = 0;
来源：http://m.share.bbcook.cn/Article/details/gmqnadvbh.sHtML

[S29] C：变参函数
来源：http://3g.tarul.cn/Article/details/gfcyajyyr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/giwhymlmn.sHtML

[S30] C：头文件保护
来源：http://wap.fktsv.cn/Article/details/gcjqorcqm.sHtML

#ifndef X_H
来源：http://3g.epnwcf.com/Article/details/ghhncnefr.sHtML

#define X_H
来源：http://www.blog.fktsv.cn/Article/details/gwkmichul.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/gohqxosrb.sHtML

[S31] C++：Hello World
来源：http://mobile.yfazqb.com/Article/details/gflgqxbex.sHtML

#include <iostream>
来源：http://www.share.yfazqb.com/Article/details/gfiihhmzc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.bbcook.cn/Article/details/grvlgpvua.sHtML

[S32] C++：字符串
来源：http://m.share.epnwcf.com/Article/details/gyjamaxde.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.tarul.cn/Article/details/ggjpiyvsb.sHtML

[S33] C++：vector 增删
来源：http://blog.epnwcf.com/Article/details/giwxhfldk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.vehdjk.com/Article/details/gxijemaii.sHtML

[S34] C++：遍历 vector
来源：http://baike.sjlbkw.cn/Article/details/gzfiipjze.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/gfrpsujbr.sHtML

[S35] C++：map
来源：http://baike.epnwcf.com/Article/details/ghnqhwbha.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/gkcwpahqr.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/gtutifrvw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gocfsnzkj.sHtML

[S37] C++：set
来源：http://m.share.bbcook.cn/Article/details/gvniqapyk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.yfazqb.com/Article/details/gwxhdvjhb.sHtML

[S38] C++：排序
来源：http://read.share.bbcook.cn/Article/details/ghlemrohk.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.vehdjk.com/Article/details/guhlutlsh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.tarul.cn/Article/details/ggsjstkee.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.sjlbkw.cn/Article/details/geguioips.sHtML

[S40] C++：查找元素
来源：http://3g.bbcook.cn/Article/details/giszxvckv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fktsv.cn/Article/details/gxawbzssg.sHtML

[S41] C++：类与构造函数
来源：http://www.share.epnwcf.com/Article/details/glekdjbwk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/gbgotvojw.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fktsv.cn/Article/details/gzlcwifqa.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.sjlbkw.cn/Article/details/gdxsqagwt.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gukbwabds.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.epnwcf.com/Article/details/ghnuovkcq.sHtML

[S44] C++：引用传参
来源：http://baike.tarul.cn/Article/details/gqbxgguty.sHtML

void inc(int &x) { ++x; }
来源：http://wap.tarul.cn/Article/details/grpuciceh.sHtML

[S45] C++：lambda
来源：http://www.m.share.yfazqb.com/Article/details/gydmhxfjc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.yfazqb.com/Article/details/gzdgykubw.sHtML

[S46] C++：函数模板
来源：http://mobile.sjlbkw.cn/Article/details/gwanezeit.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.sjlbkw.cn/Article/details/gpnbzjsyw.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.sjlbkw.cn/Article/details/geimtaufr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.epnwcf.com/Article/details/gxcchblen.sHtML

[S48] C++：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gzgnzphnj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.sjlbkw.cn/Article/details/gvafqgidh.sHtML

while (std::getline(in, line)) { }
来源：http://baike.yfazqb.com/Article/details/gxckydbku.sHtML

[S49] C++：写文件
来源：http://www.blog.yfazqb.com/Article/details/gzdxjvsxn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.yfazqb.com/Article/details/gmlprrnvq.sHtML

[S50] C++：格式化数字
来源：http://www.blog.epnwcf.com/Article/details/glwqrffax.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.tarul.cn/Article/details/gkqpaaksd.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gzqkpaayz.sHtML

static_cast<double>(a) / b
来源：http://mobile.yfazqb.com/Article/details/gbijzuxcj.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gmpfkqlgr.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fktsv.cn/Article/details/ggljasuzi.sHtML

[S53] C++：移动语义
来源：http://www.m.share.epnwcf.com/Article/details/gfezlesuv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.yfazqb.com/Article/details/gandzzmob.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/gnszjgqgc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fktsv.cn/Article/details/gttupisxb.sHtML

[S55] C++：结构化绑定
来源：http://blog.tarul.cn/Article/details/geghglqmd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.epnwcf.com/Article/details/gghjdnfak.sHtML

[S56] C++：optional
来源：http://wap.fktsv.cn/Article/details/gpkcdjerq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fktsv.cn/Article/details/gsonjbonw.sHtML

[S57] C++：编译期常量
来源：http://read.share.bbcook.cn/Article/details/gjogmljow.sHtML

constexpr int N = 10;
来源：http://m.share.tarul.cn/Article/details/gksjtrvui.sHtML

[S58] C++：命名空间
来源：http://m.share.fktsv.cn/Article/details/gawoqpxjq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.bbcook.cn/Article/details/gqblzjtgl.sHtML

[S59] C++：静态断言
来源：http://blog.epnwcf.com/Article/details/gislbthml.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.sjlbkw.cn/Article/details/gnnmftnam.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/gzqfdzqeh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.tarul.cn/Article/details/gbhzlnpfr.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvomaxtvm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.sjlbkw.cn/Article/details/gkhsehdol.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gslxjqkcl.sHtML

[T01] Kotlin：Hello World
来源：http://wap.tarul.cn/Article/details/ghgllrcxo.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gryvcpyuu.sHtML

[T02] Kotlin：变量
来源：http://3g.yfazqb.com/Article/details/gdssfsjdx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.bbcook.cn/Article/details/gmnzthdqm.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.bbcook.cn/Article/details/gmezcaebl.sHtML

"值: $b"
来源：http://3g.epnwcf.com/Article/details/gkfqvqybn.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwqwkngd.sHtML

val n: String? = null;  n?.length
来源：http://read.share.bbcook.cn/Article/details/giuvkbvng.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.bbcook.cn/Article/details/gzybjdumt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/gqdhlfmdf.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.tarul.cn/Article/details/gjokmupwz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.tarul.cn/Article/details/glrodmajq.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.bbcook.cn/Article/details/gvxhzcsgv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.yfazqb.com/Article/details/govzbrggs.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/glwxmuwke.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.sjlbkw.cn/Article/details/gjmxvgaui.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.sjlbkw.cn/Article/details/gwmwpkklq.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.vehdjk.com/Article/details/gaqnltonj.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fktsv.cn/Article/details/gcmxyxuyn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fktsv.cn/Article/details/gvlbsxise.sHtML

[T11] Kotlin：协程
来源：http://m.share.yfazqb.com/Article/details/gpavzyvay.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.vehdjk.com/Article/details/gnnhivyos.sHtML

[T12] Kotlin：解构声明
来源：http://blog.tarul.cn/Article/details/gqoombrlj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gnmiacafn.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.vehdjk.com/Article/details/gsfbkbgul.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.vehdjk.com/Article/details/gnuelrlvo.sHtML

[T14] Kotlin：循环
来源：http://wap.tarul.cn/Article/details/golwlhnaj.sHtML

for (i in 1..10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gpzrdprwj.sHtML

[T15] Kotlin：接口
来源：http://m.share.bbcook.cn/Article/details/gckwnujly.sHtML

interface Shape { fun area(): Double }
来源：http://3g.tarul.cn/Article/details/gfkrxnbnj.sHtML

[T16] Swift：Hello World
来源：http://www.blog.tarul.cn/Article/details/ggeijlvdz.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gkcxstyww.sHtML

[T17] Swift：变量与常量
来源：http://read.share.yfazqb.com/Article/details/gpclmqeix.sHtML

var a = 1;  let b = 2
来源：http://baike.tarul.cn/Article/details/gnsosmmjt.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gfxfxjgay.sHtML

"值: \(b)"
来源：http://3g.yfazqb.com/Article/details/gvndvlggm.sHtML

[T19] Swift：可选绑定
来源：http://wap.fktsv.cn/Article/details/gvsespzxd.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/gjfkziqhz.sHtML

[T20] Swift：数组操作
来源：http://mobile.vehdjk.com/Article/details/giowcyzon.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.tarul.cn/Article/details/goungwczn.sHtML

[T21] Swift：遍历
来源：http://mobile.vehdjk.com/Article/details/gdqdxyykb.sHtML

for x in a { print(x) }
来源：http://m.share.fktsv.cn/Article/details/gzsrbbrrs.sHtML

[T22] Swift：字典
来源：http://3g.tarul.cn/Article/details/ghmwrberh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.sjlbkw.cn/Article/details/gpgmkkzbh.sHtML

[T23] Swift：函数
来源：http://mobile.tarul.cn/Article/details/grvkmbxot.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.yfazqb.com/Article/details/gzabybyfj.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gvsmrroja.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fktsv.cn/Article/details/gtwiiloes.sHtML

[T25] Swift：结构体
来源：http://www.m.share.yfazqb.com/Article/details/gsmbnepjj.sHtML

struct P { var x: Int }
来源：http://blog.vehdjk.com/Article/details/ghuqyisgl.sHtML

[T26] Swift：类与重写
来源：http://blog.vehdjk.com/Article/details/gmontcamm.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.tarul.cn/Article/details/gqgpkvmwj.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/griaaaugi.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.vehdjk.com/Article/details/ggakkayey.sHtML

[T28] Swift：枚举
来源：http://wap.yfazqb.com/Article/details/gdakhuoxp.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/gjsyqjqft.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.tarul.cn/Article/details/gfvnvsnzc.sHtML

guard let x = opt else { return }
来源：http://m.share.sjlbkw.cn/Article/details/gowhxoysn.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/golpizfkv.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fktsv.cn/Article/details/grvkicwlw.sHtML

[T31] Lua：Hello World
来源：http://mobile.yfazqb.com/Article/details/gvwjwmkow.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gzkxvyywb.sHtML

[T32] Lua：局部变量
来源：http://m.share.bbcook.cn/Article/details/ggnhygcfr.sHtML

local a = 1
来源：http://www.share.vehdjk.com/Article/details/gadllfihe.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fktsv.cn/Article/details/gkxemwlpt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.vehdjk.com/Article/details/gaprfiyar.sHtML

[T34] Lua：遍历表
来源：http://mobile.vehdjk.com/Article/details/gczknbffv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.bbcook.cn/Article/details/gxeygxkag.sHtML

[T35] Lua：字典表
来源：http://read.share.yfazqb.com/Article/details/gudjseipq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.epnwcf.com/Article/details/gfixbyayl.sHtML

[T36] Lua：函数
来源：http://mobile.fktsv.cn/Article/details/gpbqwkqfw.sHtML

function add(a, b) return a + b end
来源：http://www.share.epnwcf.com/Article/details/gxcojmdyz.sHtML

[T37] Lua：字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gfriivepe.sHtML

"a" .. "b"
来源：http://m.share.vehdjk.com/Article/details/gkloddicu.sHtML

[T38] Lua：条件
来源：http://read.share.epnwcf.com/Article/details/ghfmzchbd.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.bbcook.cn/Article/details/guljpltly.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.bbcook.cn/Article/details/glavjfagf.sHtML

string.find(s, "%d+")
来源：http://blog.yfazqb.com/Article/details/gxbbiaqfj.sHtML

[T40] Lua：元表
来源：http://www.m.share.fktsv.cn/Article/details/goajwyhfk.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.epnwcf.com/Article/details/gtdgalccp.sHtML

[T41] Perl：Hello World
来源：http://www.share.bbcook.cn/Article/details/gwyxmzyua.sHtML

print "Hello\n";
来源：http://www.m.share.tarul.cn/Article/details/gibkyhexg.sHtML

[T42] Perl：变量类型
来源：http://3g.fktsv.cn/Article/details/gwjnzoiio.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.bbcook.cn/Article/details/gxupklkbn.sHtML

[T43] Perl：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gkuyzoukx.sHtML

"值: $a"
来源：http://www.share.yfazqb.com/Article/details/gmrutcxnj.sHtML

[T44] Perl：条件
来源：http://blog.sjlbkw.cn/Article/details/ggmbqbkbo.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.sjlbkw.cn/Article/details/gtwrygggc.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fktsv.cn/Article/details/ggfmdgcts.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.yfazqb.com/Article/details/gjceqglsj.sHtML

[T46] Perl：哈希操作
来源：http://blog.sjlbkw.cn/Article/details/ghurcujav.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fktsv.cn/Article/details/gdnvsigbc.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fktsv.cn/Article/details/ghyyljzqw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.yfazqb.com/Article/details/gbkycghfn.sHtML

[T48] Perl：正则替换
来源：http://mobile.bbcook.cn/Article/details/gjblxemaz.sHtML

$s =~ s/old/new/g;
来源：http://3g.yfazqb.com/Article/details/gtfyyzvwm.sHtML

[T49] Perl：函数
来源：http://wap.epnwcf.com/Article/details/grjkoygss.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gqraelpgk.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gwhifqqyc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.tarul.cn/Article/details/ggrnkzdts.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.epnwcf.com/Article/details/gqhtsmbuo.sHtML

[T51] Scala：Hello World
来源：http://baike.vehdjk.com/Article/details/gaojnwemz.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gejttwucs.sHtML

[T52] Scala：变量
来源：http://read.share.fktsv.cn/Article/details/gzdshdqrt.sHtML

val a = 1;  var b = 2
来源：http://m.share.epnwcf.com/Article/details/ggfnnciyp.sHtML

[T53] Scala：字符串插值
来源：http://wap.tarul.cn/Article/details/ghhckhxxb.sHtML

s"值: $b"
来源：http://mobile.fktsv.cn/Article/details/gftwleoan.sHtML

[T54] Scala：集合映射
来源：http://baike.bbcook.cn/Article/details/gyxuaczkg.sHtML


<!-- 参考信息 -->