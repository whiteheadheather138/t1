代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.sjlbkw.cn/Article/details/grckcrxqb.sHtML

[R54] 比较两个文件
来源：http://www.m.share.yfazqb.com/Article/details/gyogawjgl.sHtML

diff a.txt b.txt
来源：http://wap.vehdjk.com/Article/details/geqcxuwre.sHtML

[R55] 压缩与解压
来源：http://mobile.bbcook.cn/Article/details/gtzrqqtck.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fktsv.cn/Article/details/gtvfsnhbf.sHtML

[R56] 远程拷贝
来源：http://m.share.vehdjk.com/Article/details/gfuwgtjjx.sHtML

scp file user@host:/path/
来源：http://www.share.bbcook.cn/Article/details/gcemcbbro.sHtML

[R57] 远程执行命令
来源：http://3g.fktsv.cn/Article/details/gsdddsvsa.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.sjlbkw.cn/Article/details/gtceyqpyz.sHtML

[R58] 下载文件
来源：http://read.share.vehdjk.com/Article/details/gszvxcqrm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/gzjmkodxv.sHtML

[R59] 发 POST JSON
来源：http://blog.vehdjk.com/Article/details/gzfhbsyod.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fktsv.cn/Article/details/gsnvdsaun.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/gnvzpoxkd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.bbcook.cn/Article/details/gjqpemiff.sHtML

[R61] 磁盘占用
来源：http://mobile.sjlbkw.cn/Article/details/gmaqdksyg.sHtML

df -h;  du -sh *
来源：http://baike.sjlbkw.cn/Article/details/gkbapdjkr.sHtML

[R62] 找最占空间的文件
来源：http://wap.tarul.cn/Article/details/gkgedhuho.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.yfazqb.com/Article/details/gasnpusxj.sHtML

[R63] 内存与进程
来源：http://mobile.vehdjk.com/Article/details/gwbldnixk.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fktsv.cn/Article/details/gmfarxmao.sHtML

[R64] 结束进程
来源：http://3g.fktsv.cn/Article/details/gxdxgtdfq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.epnwcf.com/Article/details/gpdkkgtpz.sHtML

[R65] 查看端口占用
来源：http://read.share.yfazqb.com/Article/details/ghbvejymi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.vehdjk.com/Article/details/gaqwedbdx.sHtML

[R66] 定时任务
来源：http://baike.yfazqb.com/Article/details/gsjnfzitl.sHtML

crontab -e;  crontab -l
来源：http://blog.vehdjk.com/Article/details/gurubbysa.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.sjlbkw.cn/Article/details/gaoquqild.sHtML

openssl rand -hex 16
来源：http://wap.vehdjk.com/Article/details/ghpwxnfrh.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/gvhzzjebi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.tarul.cn/Article/details/gizbtaisf.sHtML

[R69] 生成随机密码
来源：http://mobile.vehdjk.com/Article/details/gyrijgtiu.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fktsv.cn/Article/details/ggpcxijuu.sHtML

[R70] 时间戳与互转
来源：http://www.share.epnwcf.com/Article/details/gjbcdxple.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.tarul.cn/Article/details/gftjdbxpp.sHtML

[R71] 日期格式化
来源：http://m.share.fktsv.cn/Article/details/gkmontdre.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.sjlbkw.cn/Article/details/gftzbetaj.sHtML

[R72] 等待端口就绪
来源：http://read.share.yfazqb.com/Article/details/gaoxiktgj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/grelukvex.sHtML

[R73] 分割大日志
来源：http://read.share.epnwcf.com/Article/details/gsrkjklfz.sHtML

split -l 1000 big.log part_
来源：http://3g.yfazqb.com/Article/details/gxkcmdtwc.sHtML

[R74] 批量重命名
来源：http://mobile.vehdjk.com/Article/details/gtabcsqiz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/ghyuhsqgt.sHtML

[R75] 导出环境变量
来源：http://m.share.bbcook.cn/Article/details/gdpitgfkn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fktsv.cn/Article/details/gcxvicgwa.sHtML

[R76] 使用临时文件
来源：http://www.m.share.epnwcf.com/Article/details/gnqgzeogi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gqpdkeqpm.sHtML

[R77] 读取用户输入
来源：http://3g.yfazqb.com/Article/details/gpgplwmku.sHtML

read -rp "请输入: " ans
来源：http://read.share.vehdjk.com/Article/details/ggsobxxgc.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fktsv.cn/Article/details/grrbbscti.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.yfazqb.com/Article/details/gntgmldvg.sHtML

[R79] 解析命令行选项
来源：http://www.share.yfazqb.com/Article/details/gxddbtvjj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.epnwcf.com/Article/details/gagvruwsv.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fktsv.cn/Article/details/goljdlazm.sHtML

time ./run.sh
来源：http://www.m.share.tarul.cn/Article/details/gijokvwrl.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gohzjfsua.sHtML

S. C / C++ 专题
来源：http://wap.vehdjk.com/Article/details/gibhhnqob.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gddmmeyje.sHtML

[S01] C：Hello World
来源：http://m.share.epnwcf.com/Article/details/gojfakuea.sHtML

#include <stdio.h>
来源：http://blog.sjlbkw.cn/Article/details/gpvvvdhzx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.vehdjk.com/Article/details/gomcqdjdh.sHtML

[S02] C：变量与格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gvrdybwjb.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.vehdjk.com/Article/details/ggqyimwsm.sHtML

[S03] C：读入整数
来源：http://www.m.share.yfazqb.com/Article/details/gxhzvwxfp.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/grnllfpog.sHtML

[S04] C：字符串复制
来源：http://read.share.yfazqb.com/Article/details/ghedgjbmm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fktsv.cn/Article/details/gwyzzueqi.sHtML

[S05] C：字符串长度
来源：http://www.share.bbcook.cn/Article/details/gyrwvldon.sHtML

strlen(s)
来源：http://blog.tarul.cn/Article/details/gxvypzgit.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/glrvvkxuc.sHtML

strcmp(a, b) == 0
来源：http://baike.bbcook.cn/Article/details/gjsdbwibf.sHtML

[S07] C：数组遍历求和
来源：http://www.share.sjlbkw.cn/Article/details/ggongqepa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.sjlbkw.cn/Article/details/gnkrapykv.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.yfazqb.com/Article/details/ghdrffwdf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.bbcook.cn/Article/details/gzbclrujt.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.tarul.cn/Article/details/gdzzfhoqm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/gproectdp.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.yfazqb.com/Article/details/gyzzidqbp.sHtML

int *p = &a;  *p = 5;
来源：http://wap.vehdjk.com/Article/details/gsvijhzuz.sHtML

[S11] C：逐行读文件
来源：http://3g.tarul.cn/Article/details/gbzlsqajm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.vehdjk.com/Article/details/gvewomdgy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.tarul.cn/Article/details/gbfpnrcme.sHtML

fclose(f);
来源：http://baike.fktsv.cn/Article/details/glwzfddel.sHtML

[S12] C：写文件
来源：http://baike.bbcook.cn/Article/details/gvlfimxhg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gtiafpixx.sHtML

[S13] C：宏定义
来源：http://3g.vehdjk.com/Article/details/gxlqagxyn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.tarul.cn/Article/details/gtyewbzua.sHtML

[S14] C：枚举
来源：http://www.blog.epnwcf.com/Article/details/glgsrxxvw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/gustmiizb.sHtML

[S15] C：类型转换
来源：http://www.share.fktsv.cn/Article/details/goaiedbgf.sHtML

(double) a / b
来源：http://read.share.fktsv.cn/Article/details/gqpvkkorp.sHtML

[S16] C：位操作置位
来源：http://www.m.share.vehdjk.com/Article/details/gcdxvivig.sHtML

x |= (1 << 3);
来源：http://www.share.fktsv.cn/Article/details/gzctrajiv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.bbcook.cn/Article/details/glqhmimjz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.yfazqb.com/Article/details/gjxwhollw.sHtML

[S18] C：命令行参数
来源：http://baike.bbcook.cn/Article/details/grrdkghdx.sHtML

int main(int argc, char **argv)
来源：http://blog.tarul.cn/Article/details/gbfqujsyz.sHtML

[S19] C：快速排序
来源：http://blog.bbcook.cn/Article/details/gsshkerms.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gcljvfuor.sHtML

[S20] C：二分查找
来源：http://3g.sjlbkw.cn/Article/details/gkxaqdqkv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/goildelaf.sHtML

[S21] C：字符类别判断
来源：http://3g.epnwcf.com/Article/details/glgayhxvm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.yfazqb.com/Article/details/gwgvtjmjh.sHtML

[S22] C：字符串转数字
来源：http://wap.epnwcf.com/Article/details/gurjlyqob.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/ggafnywtd.sHtML

[S23] C：随机数
来源：http://baike.tarul.cn/Article/details/grqexbyxf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.bbcook.cn/Article/details/gvfklrkzb.sHtML

[S24] C：获取本地时间
来源：http://mobile.sjlbkw.cn/Article/details/ggnbpwfzg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.epnwcf.com/Article/details/gzwdzygrm.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/gaoqzcfeh.sHtML

memcpy(dst, src, n);
来源：http://baike.yfazqb.com/Article/details/ggjbzakhe.sHtML

[S26] C：内存清零
来源：http://baike.yfazqb.com/Article/details/ggdizqbgf.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/gnidsipdn.sHtML

[S27] C：定义常量
来源：http://m.share.tarul.cn/Article/details/gvnsmxsjm.sHtML

const double PI = 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gpsvmwcgh.sHtML

[S28] C：静态变量
来源：http://www.share.epnwcf.com/Article/details/gfsyklwwg.sHtML

static int counter = 0;
来源：http://3g.sjlbkw.cn/Article/details/gdxqrikpe.sHtML

[S29] C：变参函数
来源：http://www.share.yfazqb.com/Article/details/gwdqriqkp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fktsv.cn/Article/details/gzqhtcvee.sHtML

[S30] C：头文件保护
来源：http://www.share.epnwcf.com/Article/details/glgcohtke.sHtML

#ifndef X_H
来源：http://wap.vehdjk.com/Article/details/gflmsybaw.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/gfkolyfpd.sHtML

#endif
来源：http://mobile.sjlbkw.cn/Article/details/gdvdntoje.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/gkctgissm.sHtML

#include <iostream>
来源：http://3g.yfazqb.com/Article/details/ghedcrnad.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.yfazqb.com/Article/details/gvmccaqtp.sHtML

[S32] C++：字符串
来源：http://read.share.sjlbkw.cn/Article/details/gcgdqohcl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.yfazqb.com/Article/details/giovupxeo.sHtML

[S33] C++：vector 增删
来源：http://wap.fktsv.cn/Article/details/giqlkssuq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.tarul.cn/Article/details/gujuvpyuv.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gynutblsg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.bbcook.cn/Article/details/gtfzwbthg.sHtML

[S35] C++：map
来源：http://www.m.share.bbcook.cn/Article/details/gxzuxzend.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gvaioxqer.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gahwuumnp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gelcggjcn.sHtML

[S37] C++：set
来源：http://www.share.sjlbkw.cn/Article/details/gipouqggu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.vehdjk.com/Article/details/gbqcafcbe.sHtML

[S38] C++：排序
来源：http://www.blog.vehdjk.com/Article/details/gofbldiwg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fktsv.cn/Article/details/gqyiccxgk.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fktsv.cn/Article/details/gjglsydgm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/ggpoqgbnf.sHtML

[S40] C++：查找元素
来源：http://blog.tarul.cn/Article/details/ggigtcicp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.bbcook.cn/Article/details/gvtpeluuv.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gxnvofeff.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.vehdjk.com/Article/details/govkcdhaf.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.yfazqb.com/Article/details/gdcdhqmol.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.yfazqb.com/Article/details/ghregmsyc.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gxqzunvxf.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/gbsizrgpk.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fktsv.cn/Article/details/gnkdlnhmm.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gvgrcfskl.sHtML

[S45] C++：lambda
来源：http://m.share.vehdjk.com/Article/details/gitnlzrfy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.bbcook.cn/Article/details/gzgkznacc.sHtML

[S46] C++：函数模板
来源：http://baike.vehdjk.com/Article/details/gwhlgaave.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fktsv.cn/Article/details/gfpwzomdm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.bbcook.cn/Article/details/gxtgpjubm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.bbcook.cn/Article/details/gaovbuuzp.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gunhqljil.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fktsv.cn/Article/details/gucskmfem.sHtML

while (std::getline(in, line)) { }
来源：http://wap.epnwcf.com/Article/details/gruwpdrwn.sHtML

[S49] C++：写文件
来源：http://www.share.tarul.cn/Article/details/gevwshhhg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fktsv.cn/Article/details/gtibttofb.sHtML

[S50] C++：格式化数字
来源：http://mobile.epnwcf.com/Article/details/gesbidgzq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.bbcook.cn/Article/details/gzxzokdwf.sHtML

[S51] C++：显式类型转换
来源：http://m.share.vehdjk.com/Article/details/gnmepgfcn.sHtML

static_cast<double>(a) / b
来源：http://www.share.vehdjk.com/Article/details/gjeednmus.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.vehdjk.com/Article/details/gohxwidfh.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fktsv.cn/Article/details/gzyhfcfif.sHtML

[S53] C++：移动语义
来源：http://www.m.share.tarul.cn/Article/details/gswikcbpu.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fktsv.cn/Article/details/ghydwudsl.sHtML

[S54] C++：异常处理
来源：http://www.m.share.yfazqb.com/Article/details/gikppawtm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.vehdjk.com/Article/details/gscpqrimx.sHtML

[S55] C++：结构化绑定
来源：http://m.share.sjlbkw.cn/Article/details/gwhobbehf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.sjlbkw.cn/Article/details/gpdrjlkco.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/gmoaqbszv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.epnwcf.com/Article/details/guuopksbt.sHtML

[S57] C++：编译期常量
来源：http://m.share.sjlbkw.cn/Article/details/gigrilwhr.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gzzwseqoo.sHtML

[S58] C++：命名空间
来源：http://baike.fktsv.cn/Article/details/gwahkrquf.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.vehdjk.com/Article/details/gpwbhyqvq.sHtML

[S59] C++：静态断言
来源：http://www.blog.vehdjk.com/Article/details/gplbjrurh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.epnwcf.com/Article/details/ghnkzktll.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.tarul.cn/Article/details/gtfwcrkqq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.yfazqb.com/Article/details/gonwnnxvz.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcpcxfvtd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.bbcook.cn/Article/details/gihkrhszp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtgmprejo.sHtML

[T01] Kotlin：Hello World
来源：http://3g.yfazqb.com/Article/details/gvmgrbmvs.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gockbqshw.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gixqvitcy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.yfazqb.com/Article/details/gcifhcllb.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.tarul.cn/Article/details/gmyudfprm.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/gfzmlarjw.sHtML

[T04] Kotlin：空安全
来源：http://wap.fktsv.cn/Article/details/gbljnsaky.sHtML

val n: String? = null;  n?.length
来源：http://www.share.yfazqb.com/Article/details/gjrpnxtaq.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.vehdjk.com/Article/details/gaktonxak.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.bbcook.cn/Article/details/gdjrbcmoi.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/gzgrcwgaw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.tarul.cn/Article/details/gfasaefnd.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/glakynnou.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/gvwppltxn.sHtML

[T08] Kotlin：数据类
来源：http://blog.epnwcf.com/Article/details/gcegavwro.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.bbcook.cn/Article/details/guigfcywm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.yfazqb.com/Article/details/gfthnjmjo.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.vehdjk.com/Article/details/ggsaxbypp.sHtML

[T10] Kotlin：默认参数
来源：http://3g.bbcook.cn/Article/details/ggxokbfhk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.sjlbkw.cn/Article/details/gsfczqsbs.sHtML

[T11] Kotlin：协程
来源：http://www.blog.tarul.cn/Article/details/gpdmoxkga.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.epnwcf.com/Article/details/gdnobdkvm.sHtML

[T12] Kotlin：解构声明
来源：http://baike.epnwcf.com/Article/details/ggxzklten.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gfyumzdvo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.bbcook.cn/Article/details/guadgdqpf.sHtML

val m = mapOf("a" to 1)
来源：http://3g.yfazqb.com/Article/details/ghmookbou.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fktsv.cn/Article/details/gmwasgekl.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gixnkwivj.sHtML

[T15] Kotlin：接口
来源：http://wap.fktsv.cn/Article/details/gldkzrlfj.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.vehdjk.com/Article/details/gfzmwqdgw.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/goodicrfe.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gnmmcqeoz.sHtML

[T17] Swift：变量与常量
来源：http://read.share.vehdjk.com/Article/details/gjnqstkng.sHtML

var a = 1;  let b = 2
来源：http://read.share.yfazqb.com/Article/details/glmyqufsy.sHtML

[T18] Swift：字符串插值
来源：http://www.share.yfazqb.com/Article/details/ghvhukeyr.sHtML

"值: \(b)"
来源：http://read.share.sjlbkw.cn/Article/details/gyteoaacf.sHtML

[T19] Swift：可选绑定
来源：http://m.share.bbcook.cn/Article/details/gybucnwjk.sHtML

if let n = opt { print(n) }
来源：http://blog.bbcook.cn/Article/details/gxeiutmxr.sHtML

[T20] Swift：数组操作
来源：http://www.share.vehdjk.com/Article/details/guflfitvh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.tarul.cn/Article/details/ghezxkvaz.sHtML

[T21] Swift：遍历
来源：http://mobile.fktsv.cn/Article/details/gscwlgfmw.sHtML

for x in a { print(x) }
来源：http://3g.epnwcf.com/Article/details/gxzteleil.sHtML

[T22] Swift：字典
来源：http://read.share.sjlbkw.cn/Article/details/gyocbgcpz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.yfazqb.com/Article/details/guqlqwvox.sHtML

[T23] Swift：函数
来源：http://wap.tarul.cn/Article/details/gneiqgxbr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.epnwcf.com/Article/details/gnaqbpqwu.sHtML

[T24] Swift：闭包
来源：http://www.share.yfazqb.com/Article/details/gdkznnpxk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.yfazqb.com/Article/details/gfpbwcxmg.sHtML

[T25] Swift：结构体
来源：http://read.share.tarul.cn/Article/details/gmmqkiima.sHtML

struct P { var x: Int }
来源：http://baike.fktsv.cn/Article/details/gxfbdvyom.sHtML

[T26] Swift：类与重写
来源：http://3g.epnwcf.com/Article/details/gcyghjfpe.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.yfazqb.com/Article/details/gewcayoub.sHtML

[T27] Swift：错误处理
来源：http://3g.yfazqb.com/Article/details/gngjivnny.sHtML

do { try f() } catch { print(error) }
来源：http://wap.bbcook.cn/Article/details/gspxpwuuw.sHtML

[T28] Swift：枚举
来源：http://3g.bbcook.cn/Article/details/gsxkzygde.sHtML

enum Color { case red, green }
来源：http://mobile.yfazqb.com/Article/details/gutwhdsdo.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.bbcook.cn/Article/details/guhkmhzrt.sHtML

guard let x = opt else { return }
来源：http://www.blog.bbcook.cn/Article/details/ggexmeafz.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/gaqmwhvxc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.vehdjk.com/Article/details/ggljuuqpz.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/guqnrxost.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gxfedmkjh.sHtML

[T32] Lua：局部变量
来源：http://blog.bbcook.cn/Article/details/gwshnmijb.sHtML

local a = 1
来源：http://www.share.epnwcf.com/Article/details/gsaigvvfd.sHtML

[T33] Lua：表（数组）
来源：http://3g.yfazqb.com/Article/details/gecglglgj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.epnwcf.com/Article/details/gkvuzlksb.sHtML

[T34] Lua：遍历表
来源：http://www.share.epnwcf.com/Article/details/gnpdfrzsb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.bbcook.cn/Article/details/glfeipkke.sHtML

[T35] Lua：字典表
来源：http://www.blog.yfazqb.com/Article/details/ggnpwougl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.bbcook.cn/Article/details/gverrxhua.sHtML

[T36] Lua：函数
来源：http://www.m.share.tarul.cn/Article/details/gcxmuxelg.sHtML

function add(a, b) return a + b end
来源：http://3g.vehdjk.com/Article/details/gejwiuvsy.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gupivhlkk.sHtML

"a" .. "b"
来源：http://3g.fktsv.cn/Article/details/gfgijnhlx.sHtML

[T38] Lua：条件
来源：http://m.share.sjlbkw.cn/Article/details/goksxptci.sHtML

if x > 0 then print("正") end
来源：http://m.share.epnwcf.com/Article/details/gsquctops.sHtML

[T39] Lua：模式匹配
来源：http://blog.tarul.cn/Article/details/gtmqehgpi.sHtML

string.find(s, "%d+")
来源：http://wap.tarul.cn/Article/details/gtrkubmat.sHtML

[T40] Lua：元表
来源：http://www.share.epnwcf.com/Article/details/gvnmclomq.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fktsv.cn/Article/details/gilkrfgzu.sHtML

[T41] Perl：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gecbamduv.sHtML

print "Hello\n";
来源：http://www.m.share.fktsv.cn/Article/details/gvricsndu.sHtML

[T42] Perl：变量类型
来源：http://m.share.tarul.cn/Article/details/gkvolvdik.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrdltors.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/ggcjnyaiw.sHtML

"值: $a"
来源：http://www.blog.epnwcf.com/Article/details/gvnxjpgcb.sHtML

[T44] Perl：条件
来源：http://m.share.yfazqb.com/Article/details/gezupzwso.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.yfazqb.com/Article/details/gryoqacju.sHtML

[T45] Perl：数组遍历
来源：http://read.share.bbcook.cn/Article/details/gbubdomvx.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.yfazqb.com/Article/details/gvamwalvr.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fktsv.cn/Article/details/gipzqjmut.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.sjlbkw.cn/Article/details/gsdpglnxy.sHtML

[T47] Perl：正则捕获
来源：http://baike.tarul.cn/Article/details/gulwfksdk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.tarul.cn/Article/details/ggeubkucj.sHtML

[T48] Perl：正则替换
来源：http://m.share.tarul.cn/Article/details/gjcodoxfk.sHtML

$s =~ s/old/new/g;
来源：http://www.share.sjlbkw.cn/Article/details/gvcryemno.sHtML

[T49] Perl：函数
来源：http://www.m.share.yfazqb.com/Article/details/gdbthsxzs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gcujnmpzo.sHtML

[T50] Perl：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gjnhjqyel.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.tarul.cn/Article/details/gyyecsaok.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.epnwcf.com/Article/details/gaiwlzbnq.sHtML

[T51] Scala：Hello World
来源：http://baike.tarul.cn/Article/details/ggyoqsvyr.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gkjsygdvh.sHtML

[T52] Scala：变量
来源：http://read.share.epnwcf.com/Article/details/gphtjgmpo.sHtML

val a = 1;  var b = 2
来源：http://3g.bbcook.cn/Article/details/gkdqaqybk.sHtML

[T53] Scala：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gsqfbvzcv.sHtML

s"值: $b"
来源：http://blog.tarul.cn/Article/details/gfdejldqp.sHtML

[T54] Scala：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/gfqdsfjar.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gslewpeke.sHtML

[T55] Scala：集合过滤
来源：http://wap.bbcook.cn/Article/details/gkumulunf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.vehdjk.com/Article/details/groenxrnm.sHtML

[T56] Scala：样例类
来源：http://read.share.epnwcf.com/Article/details/glcnsvtmz.sHtML


<!-- 参考信息 -->