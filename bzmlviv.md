代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.bbcook.cn/Article/details/ggdwvvymq.sHtML

[R56] 远程拷贝
来源：http://blog.sjlbkw.cn/Article/details/gfqhytfdq.sHtML

scp file user@host:/path/
来源：http://baike.yfazqb.com/Article/details/gfkfrqajx.sHtML

[R57] 远程执行命令
来源：http://www.blog.yfazqb.com/Article/details/gzucfpjqe.sHtML

ssh user@host 'uptime'
来源：http://mobile.sjlbkw.cn/Article/details/gzuyvfkbs.sHtML

[R58] 下载文件
来源：http://www.m.share.fktsv.cn/Article/details/gjnvngjjx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/gbhxvgwyi.sHtML

[R59] 发 POST JSON
来源：http://wap.bbcook.cn/Article/details/ggkojrbww.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.vehdjk.com/Article/details/gzhzqfnrq.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gjouzujwg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/gzhfkhhps.sHtML

[R61] 磁盘占用
来源：http://wap.vehdjk.com/Article/details/ghhjzojli.sHtML

df -h;  du -sh *
来源：http://www.blog.yfazqb.com/Article/details/gxwvbggei.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/gsxtyzgxu.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.sjlbkw.cn/Article/details/gdxdlwyvp.sHtML

[R63] 内存与进程
来源：http://www.m.share.bbcook.cn/Article/details/gmtagugyu.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.epnwcf.com/Article/details/ggdaytgqg.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gbfhqvbly.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmpchchg.sHtML

[R65] 查看端口占用
来源：http://mobile.sjlbkw.cn/Article/details/gnuoqypgo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.yfazqb.com/Article/details/gojcsocsz.sHtML

[R66] 定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/goeahfznh.sHtML

crontab -e;  crontab -l
来源：http://baike.sjlbkw.cn/Article/details/gdprrhyho.sHtML

[R67] 生成随机十六进制串
来源：http://wap.yfazqb.com/Article/details/gvsmhvdyx.sHtML

openssl rand -hex 16
来源：http://www.share.vehdjk.com/Article/details/grfnpqrbe.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.yfazqb.com/Article/details/ggihfshjz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.epnwcf.com/Article/details/gnlxylpwi.sHtML

[R69] 生成随机密码
来源：http://read.share.vehdjk.com/Article/details/gwqwsrequ.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.vehdjk.com/Article/details/ggooacouu.sHtML

[R70] 时间戳与互转
来源：http://m.share.vehdjk.com/Article/details/ghxnejstk.sHtML

date +%s;  date -d @1700000000
来源：http://wap.tarul.cn/Article/details/gfefdiobp.sHtML

[R71] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gasuqszfb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.bbcook.cn/Article/details/ghekguusn.sHtML

[R72] 等待端口就绪
来源：http://www.share.bbcook.cn/Article/details/ggqnfjoha.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gkvduqhpr.sHtML

[R73] 分割大日志
来源：http://3g.vehdjk.com/Article/details/grziwxhku.sHtML

split -l 1000 big.log part_
来源：http://read.share.tarul.cn/Article/details/giadtcgju.sHtML

[R74] 批量重命名
来源：http://www.blog.fktsv.cn/Article/details/gxozbweqo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.bbcook.cn/Article/details/gtqbunjam.sHtML

[R75] 导出环境变量
来源：http://3g.epnwcf.com/Article/details/gsyxlnayy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fktsv.cn/Article/details/gtcnfepcr.sHtML

[R76] 使用临时文件
来源：http://baike.yfazqb.com/Article/details/gfvfxupbw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/gfkdssryi.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/gqerxgwri.sHtML

read -rp "请输入: " ans
来源：http://www.blog.epnwcf.com/Article/details/gjyhqkdmj.sHtML

[R78] 交互式菜单
来源：http://mobile.tarul.cn/Article/details/gqgpzasot.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/grtdwoggm.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gyigmhlxq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.yfazqb.com/Article/details/gczjfihnq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.tarul.cn/Article/details/gusrsthds.sHtML

time ./run.sh
来源：http://www.share.tarul.cn/Article/details/gdcdrrdyk.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gysjpxhgv.sHtML

S. C / C++ 专题
来源：http://www.blog.bbcook.cn/Article/details/gytmhdnpv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gokxbnjzn.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gntownuov.sHtML

#include <stdio.h>
来源：http://www.blog.epnwcf.com/Article/details/gtggdxdqx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.vehdjk.com/Article/details/geykagkrg.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.bbcook.cn/Article/details/gzicyvuwv.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.epnwcf.com/Article/details/gnqynoddu.sHtML

[S03] C：读入整数
来源：http://mobile.sjlbkw.cn/Article/details/gqxljmxvm.sHtML

int x; scanf("%d", &x);
来源：http://3g.tarul.cn/Article/details/gnnqvlcly.sHtML

[S04] C：字符串复制
来源：http://baike.fktsv.cn/Article/details/guqdnucah.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.epnwcf.com/Article/details/gwwwszuzh.sHtML

[S05] C：字符串长度
来源：http://www.blog.tarul.cn/Article/details/gwdiuecka.sHtML

strlen(s)
来源：http://m.share.fktsv.cn/Article/details/gjvephuui.sHtML

[S06] C：字符串比较
来源：http://3g.yfazqb.com/Article/details/gjisxpwhj.sHtML

strcmp(a, b) == 0
来源：http://read.share.epnwcf.com/Article/details/gruafxcfl.sHtML

[S07] C：数组遍历求和
来源：http://3g.vehdjk.com/Article/details/gczoqgjhq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.vehdjk.com/Article/details/gajlyxjxt.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.sjlbkw.cn/Article/details/gtkwnqsiw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fktsv.cn/Article/details/gmhbxqdgc.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.bbcook.cn/Article/details/gbmxucwki.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.bbcook.cn/Article/details/gwyxzwkpo.sHtML

[S10] C：指针与解引用
来源：http://read.share.sjlbkw.cn/Article/details/gxzbsbipz.sHtML

int *p = &a;  *p = 5;
来源：http://3g.vehdjk.com/Article/details/gcimhaccy.sHtML

[S11] C：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gsjwfltce.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.sjlbkw.cn/Article/details/gcmpamwek.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.yfazqb.com/Article/details/gkojzywhf.sHtML

fclose(f);
来源：http://wap.epnwcf.com/Article/details/gxyfuetyd.sHtML

[S12] C：写文件
来源：http://blog.fktsv.cn/Article/details/gwxwejwps.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.epnwcf.com/Article/details/gfnwapkvz.sHtML

[S13] C：宏定义
来源：http://read.share.fktsv.cn/Article/details/gglulhzmh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.epnwcf.com/Article/details/gkjycaxxy.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/gxlahzjfk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.yfazqb.com/Article/details/ggvkvdgih.sHtML

[S15] C：类型转换
来源：http://www.blog.tarul.cn/Article/details/gfvimqloe.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/gmaynkgnd.sHtML

[S16] C：位操作置位
来源：http://3g.vehdjk.com/Article/details/gglxmrfaw.sHtML

x |= (1 << 3);
来源：http://www.m.share.tarul.cn/Article/details/gnzbougvl.sHtML

[S17] C：安全拼接字符串
来源：http://wap.yfazqb.com/Article/details/gunjhpadk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.yfazqb.com/Article/details/gtwveaqrv.sHtML

[S18] C：命令行参数
来源：http://m.share.yfazqb.com/Article/details/gyozupghq.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gpkuzwpif.sHtML

[S19] C：快速排序
来源：http://baike.vehdjk.com/Article/details/gyibphcvb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gzqbnaehw.sHtML

[S20] C：二分查找
来源：http://mobile.tarul.cn/Article/details/grjolbxce.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gkqckhjlf.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.yfazqb.com/Article/details/gxqjutviy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.epnwcf.com/Article/details/gimldudav.sHtML

[S22] C：字符串转数字
来源：http://baike.sjlbkw.cn/Article/details/gwdcjnjxl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.tarul.cn/Article/details/gmrxfezzi.sHtML

[S23] C：随机数
来源：http://baike.epnwcf.com/Article/details/gxofkgrvp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.sjlbkw.cn/Article/details/gzvjsgeui.sHtML

[S24] C：获取本地时间
来源：http://blog.bbcook.cn/Article/details/grzikexkt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.epnwcf.com/Article/details/goaclhohp.sHtML

[S25] C：内存拷贝
来源：http://mobile.epnwcf.com/Article/details/gdpieyrmw.sHtML

memcpy(dst, src, n);
来源：http://read.share.fktsv.cn/Article/details/gzpacuchx.sHtML

[S26] C：内存清零
来源：http://read.share.vehdjk.com/Article/details/gftshmmee.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.tarul.cn/Article/details/gtakrrycy.sHtML

[S27] C：定义常量
来源：http://read.share.yfazqb.com/Article/details/ggmgjgaxr.sHtML

const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/giubjzfdq.sHtML

[S28] C：静态变量
来源：http://www.share.vehdjk.com/Article/details/gcxzhdjeu.sHtML

static int counter = 0;
来源：http://www.blog.sjlbkw.cn/Article/details/gstiolphy.sHtML

[S29] C：变参函数
来源：http://mobile.tarul.cn/Article/details/gdxromcim.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.epnwcf.com/Article/details/ggvjlkzrb.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/gkpaugzhn.sHtML

#ifndef X_H
来源：http://www.share.vehdjk.com/Article/details/gmhwaljgm.sHtML

#define X_H
来源：http://www.m.share.vehdjk.com/Article/details/gfztldvmc.sHtML

#endif
来源：http://m.share.sjlbkw.cn/Article/details/gquifmiuf.sHtML

[S31] C++：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gwwfkfgwq.sHtML

#include <iostream>
来源：http://mobile.sjlbkw.cn/Article/details/guimvnfpp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/gspfwljiu.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gzbmhnfya.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.tarul.cn/Article/details/gmhdgwwgs.sHtML

[S33] C++：vector 增删
来源：http://baike.vehdjk.com/Article/details/gflknkwjt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fktsv.cn/Article/details/gxwggrgzj.sHtML

[S34] C++：遍历 vector
来源：http://read.share.vehdjk.com/Article/details/ggyugalaw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.bbcook.cn/Article/details/gvayhdthq.sHtML

[S35] C++：map
来源：http://wap.bbcook.cn/Article/details/gisujyvbk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbwhpadn.sHtML

[S36] C++：unordered_map
来源：http://read.share.tarul.cn/Article/details/goxubfhrc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/ggkzfipth.sHtML

[S37] C++：set
来源：http://3g.vehdjk.com/Article/details/gyyyygzbu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.vehdjk.com/Article/details/gulcdcjmq.sHtML

[S38] C++：排序
来源：http://3g.bbcook.cn/Article/details/gxfpouard.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.yfazqb.com/Article/details/gizhoyiyp.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.sjlbkw.cn/Article/details/gmhqvhlyg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.tarul.cn/Article/details/gpgcsummm.sHtML

[S40] C++：查找元素
来源：http://m.share.fktsv.cn/Article/details/gwkwrvsvp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.sjlbkw.cn/Article/details/gkduxlnma.sHtML

[S41] C++：类与构造函数
来源：http://www.share.sjlbkw.cn/Article/details/ggcwiggsy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.bbcook.cn/Article/details/gbkicuaab.sHtML

[S42] C++：继承与虚函数
来源：http://wap.tarul.cn/Article/details/gagdlpjdz.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/gkrsubdne.sHtML

[S43] C++：智能指针
来源：http://www.blog.tarul.cn/Article/details/gpqagigsq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.yfazqb.com/Article/details/geljjaiff.sHtML

[S44] C++：引用传参
来源：http://www.blog.epnwcf.com/Article/details/gzkmbhivl.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/guoyzgzpi.sHtML

[S45] C++：lambda
来源：http://3g.bbcook.cn/Article/details/gertxuohg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.epnwcf.com/Article/details/geulbfuus.sHtML

[S46] C++：函数模板
来源：http://read.share.vehdjk.com/Article/details/gpozmsgyb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/gxfmkygqk.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.vehdjk.com/Article/details/gzjhvkcho.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.tarul.cn/Article/details/guplzjugd.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/glbwahqml.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.yfazqb.com/Article/details/gyzaohxbp.sHtML

while (std::getline(in, line)) { }
来源：http://blog.bbcook.cn/Article/details/gtwghfkfb.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/giutdzdpd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fktsv.cn/Article/details/gmuhompwa.sHtML

[S50] C++：格式化数字
来源：http://3g.fktsv.cn/Article/details/gfcoywufn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gthrokjzu.sHtML

[S51] C++：显式类型转换
来源：http://blog.fktsv.cn/Article/details/gzwrhtffl.sHtML

static_cast<double>(a) / b
来源：http://blog.tarul.cn/Article/details/geshcffpg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgtheneo.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.vehdjk.com/Article/details/ghconknkk.sHtML

[S53] C++：移动语义
来源：http://3g.tarul.cn/Article/details/gpwdshfcr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.epnwcf.com/Article/details/grszdvvyw.sHtML

[S54] C++：异常处理
来源：http://blog.fktsv.cn/Article/details/gkazekmoc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.epnwcf.com/Article/details/gfphnfffa.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fktsv.cn/Article/details/grqdpklpg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.epnwcf.com/Article/details/gxppxnokh.sHtML

[S56] C++：optional
来源：http://www.share.epnwcf.com/Article/details/gruwwzytl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.bbcook.cn/Article/details/gnvkbanqs.sHtML

[S57] C++：编译期常量
来源：http://www.blog.epnwcf.com/Article/details/gbwrbfpth.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/gefzoyzfi.sHtML

[S58] C++：命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gkinprqvq.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.vehdjk.com/Article/details/gahaqtpbw.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/gkxldldyz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/gcohzrmwd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gihlcsapy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gvemxzqwb.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gbcbogicd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.yfazqb.com/Article/details/gkyunnqdv.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfkisqugh.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gwnaufuln.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gdwgqpija.sHtML

[T02] Kotlin：变量
来源：http://www.blog.tarul.cn/Article/details/ggowrnwdv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.bbcook.cn/Article/details/gssdlonil.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.vehdjk.com/Article/details/gtpqtecch.sHtML

"值: $b"
来源：http://m.share.bbcook.cn/Article/details/gtkefrfhx.sHtML

[T04] Kotlin：空安全
来源：http://baike.fktsv.cn/Article/details/goyuhmvcx.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gavkrnogv.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.bbcook.cn/Article/details/grbfqjbxu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.sjlbkw.cn/Article/details/gzvlgtzmb.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/gzcpksnvt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gszyweymc.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fktsv.cn/Article/details/gewsymigu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.yfazqb.com/Article/details/ggipiwthz.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.tarul.cn/Article/details/gvuzvlnla.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/goaznftpw.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fktsv.cn/Article/details/gzweiuamc.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.vehdjk.com/Article/details/gtxmnzfky.sHtML

[T10] Kotlin：默认参数
来源：http://wap.bbcook.cn/Article/details/gczawwydi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.yfazqb.com/Article/details/gmspwuaml.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/glxttjhgy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.bbcook.cn/Article/details/gcaaqcogc.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fktsv.cn/Article/details/gbbsyvylz.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fktsv.cn/Article/details/gkgoawqfg.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.tarul.cn/Article/details/glzdksjjg.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.bbcook.cn/Article/details/gyyqooasz.sHtML

[T14] Kotlin：循环
来源：http://wap.yfazqb.com/Article/details/guqdgypkb.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gjtuppyyf.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.epnwcf.com/Article/details/gmhzmwmwh.sHtML

interface Shape { fun area(): Double }
来源：http://baike.bbcook.cn/Article/details/gvehrfuvh.sHtML

[T16] Swift：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gzuuwzlpd.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gqrvufrob.sHtML

[T17] Swift：变量与常量
来源：http://baike.sjlbkw.cn/Article/details/gqtrwocdc.sHtML

var a = 1;  let b = 2
来源：http://www.share.vehdjk.com/Article/details/gihweqsqc.sHtML

[T18] Swift：字符串插值
来源：http://baike.vehdjk.com/Article/details/ggyjcrnul.sHtML

"值: \(b)"
来源：http://m.share.tarul.cn/Article/details/gkniljdac.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.sjlbkw.cn/Article/details/gwfgkoyih.sHtML

if let n = opt { print(n) }
来源：http://blog.yfazqb.com/Article/details/gqgehxxnq.sHtML

[T20] Swift：数组操作
来源：http://mobile.sjlbkw.cn/Article/details/gmfzryoxk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.vehdjk.com/Article/details/gbjytudkq.sHtML

[T21] Swift：遍历
来源：http://m.share.epnwcf.com/Article/details/gjsmhaogq.sHtML

for x in a { print(x) }
来源：http://read.share.vehdjk.com/Article/details/ghgsusycv.sHtML

[T22] Swift：字典
来源：http://m.share.vehdjk.com/Article/details/ginomfidc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.yfazqb.com/Article/details/glxxgtyjy.sHtML

[T23] Swift：函数
来源：http://mobile.bbcook.cn/Article/details/gjlnaztfr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fktsv.cn/Article/details/gtbphfgdh.sHtML

[T24] Swift：闭包
来源：http://www.m.share.epnwcf.com/Article/details/gbohulutf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fktsv.cn/Article/details/gcoogolad.sHtML

[T25] Swift：结构体
来源：http://3g.fktsv.cn/Article/details/gqtullifo.sHtML

struct P { var x: Int }
来源：http://www.m.share.vehdjk.com/Article/details/gyiijfqni.sHtML

[T26] Swift：类与重写
来源：http://wap.tarul.cn/Article/details/gyjhzighp.sHtML

class A: Base { override func f() {} }
来源：http://m.share.vehdjk.com/Article/details/gjhsfdfcu.sHtML

[T27] Swift：错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gbgvkagdw.sHtML

do { try f() } catch { print(error) }
来源：http://3g.bbcook.cn/Article/details/gbvlsibuv.sHtML

[T28] Swift：枚举
来源：http://blog.tarul.cn/Article/details/gqkabbmgq.sHtML

enum Color { case red, green }
来源：http://wap.yfazqb.com/Article/details/gtxdheiks.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fktsv.cn/Article/details/guikzbpnn.sHtML

guard let x = opt else { return }
来源：http://www.blog.fktsv.cn/Article/details/gepaouflb.sHtML

[T30] Swift：协议
来源：http://www.blog.yfazqb.com/Article/details/gcndyebls.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.tarul.cn/Article/details/gwzwcvgty.sHtML

[T31] Lua：Hello World
来源：http://wap.vehdjk.com/Article/details/gubjrwdem.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/gnhbteksm.sHtML

[T32] Lua：局部变量
来源：http://blog.yfazqb.com/Article/details/gdjnghkwq.sHtML

local a = 1
来源：http://3g.bbcook.cn/Article/details/gzdmwuizq.sHtML

[T33] Lua：表（数组）
来源：http://baike.epnwcf.com/Article/details/goicyltgq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.bbcook.cn/Article/details/gnhnjugrf.sHtML

[T34] Lua：遍历表
来源：http://baike.bbcook.cn/Article/details/gqhgrvcgn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.sjlbkw.cn/Article/details/gbvkrulex.sHtML

[T35] Lua：字典表
来源：http://3g.bbcook.cn/Article/details/grlqvoads.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.vehdjk.com/Article/details/gnbyzgtjb.sHtML

[T36] Lua：函数
来源：http://blog.tarul.cn/Article/details/gmvkrdqeg.sHtML

function add(a, b) return a + b end
来源：http://blog.yfazqb.com/Article/details/gyfwgzxgs.sHtML

[T37] Lua：字符串拼接
来源：http://baike.tarul.cn/Article/details/gnbhixhtn.sHtML

"a" .. "b"
来源：http://www.share.vehdjk.com/Article/details/grmneolpx.sHtML

[T38] Lua：条件
来源：http://wap.vehdjk.com/Article/details/gudqcumxq.sHtML

if x > 0 then print("正") end
来源：http://wap.epnwcf.com/Article/details/gixyjgban.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gychejrnt.sHtML

string.find(s, "%d+")
来源：http://3g.yfazqb.com/Article/details/gzgtwkzig.sHtML

[T40] Lua：元表
来源：http://blog.vehdjk.com/Article/details/gqxncalet.sHtML

setmetatable({}, { __index = base })
来源：http://blog.vehdjk.com/Article/details/gbgsftvbh.sHtML

[T41] Perl：Hello World
来源：http://blog.vehdjk.com/Article/details/gqehzzcwl.sHtML

print "Hello\n";
来源：http://www.share.fktsv.cn/Article/details/gfxkujfew.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.vehdjk.com/Article/details/gwjvbdnjr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.bbcook.cn/Article/details/gbtridkou.sHtML

[T43] Perl：字符串插值
来源：http://wap.epnwcf.com/Article/details/grthllwgc.sHtML

"值: $a"
来源：http://www.blog.vehdjk.com/Article/details/gpfpjhioj.sHtML

[T44] Perl：条件
来源：http://blog.vehdjk.com/Article/details/gdlujpzaq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.tarul.cn/Article/details/gbzmiyueg.sHtML

[T45] Perl：数组遍历
来源：http://blog.fktsv.cn/Article/details/gybvzeiac.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.yfazqb.com/Article/details/gkyujdxpp.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fktsv.cn/Article/details/gyydqsnob.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.epnwcf.com/Article/details/gjvzntluo.sHtML

[T47] Perl：正则捕获
来源：http://3g.yfazqb.com/Article/details/gitjnvikq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.epnwcf.com/Article/details/gfpvvdhma.sHtML

[T48] Perl：正则替换
来源：http://read.share.bbcook.cn/Article/details/gpnlsgcqe.sHtML

$s =~ s/old/new/g;
来源：http://read.share.yfazqb.com/Article/details/gvnerghkb.sHtML

[T49] Perl：函数
来源：http://wap.sjlbkw.cn/Article/details/glqdykrbl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gvpexrghl.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gwlbtmpow.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.epnwcf.com/Article/details/gqbtudwad.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.epnwcf.com/Article/details/gwkgmnebe.sHtML

[T51] Scala：Hello World
来源：http://read.share.epnwcf.com/Article/details/glkbvyxca.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gsnomlpbz.sHtML

[T52] Scala：变量
来源：http://blog.yfazqb.com/Article/details/gvvnzjzdt.sHtML

val a = 1;  var b = 2
来源：http://baike.vehdjk.com/Article/details/gxlytdwfv.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gcxzgkasn.sHtML

s"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gsyllzrga.sHtML

[T54] Scala：集合映射
来源：http://m.share.tarul.cn/Article/details/gznudbptz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.vehdjk.com/Article/details/grwhaqoek.sHtML

[T55] Scala：集合过滤
来源：http://3g.vehdjk.com/Article/details/gqiyfyuor.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.yfazqb.com/Article/details/gakgtfmjw.sHtML

[T56] Scala：样例类
来源：http://read.share.tarul.cn/Article/details/guhwbahnv.sHtML

case class User(name: String, age: Int)
来源：http://blog.yfazqb.com/Article/details/gfcjgonsg.sHtML

[T57] Scala：模式匹配
来源：http://wap.fktsv.cn/Article/details/gkvwqrvml.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.yfazqb.com/Article/details/goxtkheot.sHtML

[T58] Scala：函数定义
来源：http://baike.epnwcf.com/Article/details/ghazvzlkz.sHtML


<!-- 参考信息 -->