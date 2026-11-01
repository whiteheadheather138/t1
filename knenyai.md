代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.share.tarul.cn/Article/details/gikhxvttw.sHtML

[R46] 递归替换文件内容
来源：http://baike.sjlbkw.cn/Article/details/gvaffajrh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.epnwcf.com/Article/details/gxinnvyud.sHtML

[R47] sed 单行替换
来源：http://3g.fktsv.cn/Article/details/gndzmqttp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gjjuffzcq.sHtML

[R48] awk 取指定列
来源：http://m.share.fktsv.cn/Article/details/gsskojhqz.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gjqkywkmt.sHtML

[R49] awk 带条件
来源：http://3g.vehdjk.com/Article/details/gdmjxtdte.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.vehdjk.com/Article/details/grkvnwtyu.sHtML

[R50] awk 求和
来源：http://m.share.sjlbkw.cn/Article/details/gljslgghe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gqrejdyag.sHtML

[R51] 排序去重取前几
来源：http://3g.tarul.cn/Article/details/ghgxqeqta.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fktsv.cn/Article/details/gbohqjkxy.sHtML

[R52] 统计行数
来源：http://blog.yfazqb.com/Article/details/gqciazget.sHtML

wc -l a.txt
来源：http://baike.vehdjk.com/Article/details/ggvwtzbic.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.epnwcf.com/Article/details/gdbwsuxxb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.yfazqb.com/Article/details/gqxkvjlkb.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/ganwkxllp.sHtML

diff a.txt b.txt
来源：http://blog.tarul.cn/Article/details/gjvswygri.sHtML

[R55] 压缩与解压
来源：http://3g.vehdjk.com/Article/details/gvrtkklor.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fktsv.cn/Article/details/gmifekixh.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/gqcoikndo.sHtML

scp file user@host:/path/
来源：http://baike.yfazqb.com/Article/details/gltskvcwv.sHtML

[R57] 远程执行命令
来源：http://baike.bbcook.cn/Article/details/gapxwzwtw.sHtML

ssh user@host 'uptime'
来源：http://3g.vehdjk.com/Article/details/gdqjsxzck.sHtML

[R58] 下载文件
来源：http://read.share.fktsv.cn/Article/details/gjeigknis.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.vehdjk.com/Article/details/ggzvskufh.sHtML

[R59] 发 POST JSON
来源：http://blog.vehdjk.com/Article/details/gasexuhvx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.sjlbkw.cn/Article/details/gfyoylilc.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gkznuewwq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.tarul.cn/Article/details/ggchfecmn.sHtML

[R61] 磁盘占用
来源：http://www.m.share.tarul.cn/Article/details/guqpjxaqg.sHtML

df -h;  du -sh *
来源：http://wap.vehdjk.com/Article/details/geolyfoit.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/gjhaehxwa.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.tarul.cn/Article/details/gkvfxlfhr.sHtML

[R63] 内存与进程
来源：http://read.share.tarul.cn/Article/details/gtoettwnl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fktsv.cn/Article/details/gntindnwz.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzlwedfz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.vehdjk.com/Article/details/grovepohu.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/glcbyzzzg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.bbcook.cn/Article/details/gpdysrjhd.sHtML

[R66] 定时任务
来源：http://www.m.share.fktsv.cn/Article/details/grvryrazm.sHtML

crontab -e;  crontab -l
来源：http://m.share.tarul.cn/Article/details/gfiohosmi.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.bbcook.cn/Article/details/gzihfqtiv.sHtML

openssl rand -hex 16
来源：http://blog.sjlbkw.cn/Article/details/gqbmbabdh.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/gogahfhgv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.tarul.cn/Article/details/ggrzijwad.sHtML

[R69] 生成随机密码
来源：http://m.share.epnwcf.com/Article/details/gckqhyhlh.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.tarul.cn/Article/details/gchesrgmh.sHtML

[R70] 时间戳与互转
来源：http://blog.vehdjk.com/Article/details/gcxgmyauy.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/gzwnkivfl.sHtML

[R71] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gxhvtqijw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.vehdjk.com/Article/details/ghzthqrad.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fktsv.cn/Article/details/gkycrxfju.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gntjxxdcg.sHtML

[R73] 分割大日志
来源：http://www.m.share.bbcook.cn/Article/details/gcxgqheqp.sHtML

split -l 1000 big.log part_
来源：http://m.share.sjlbkw.cn/Article/details/gtgnaxwqz.sHtML

[R74] 批量重命名
来源：http://blog.epnwcf.com/Article/details/geqxlshcr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/gveuwcjcw.sHtML

[R75] 导出环境变量
来源：http://wap.fktsv.cn/Article/details/guirqxdpi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.sjlbkw.cn/Article/details/gdkrbqsqy.sHtML

[R76] 使用临时文件
来源：http://wap.bbcook.cn/Article/details/gwbodsgcn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/gzezrhzbv.sHtML

[R77] 读取用户输入
来源：http://mobile.fktsv.cn/Article/details/ghprljsrg.sHtML

read -rp "请输入: " ans
来源：http://blog.tarul.cn/Article/details/gleelbotb.sHtML

[R78] 交互式菜单
来源：http://3g.epnwcf.com/Article/details/gzaxpzebt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.tarul.cn/Article/details/gtopxbvzg.sHtML

[R79] 解析命令行选项
来源：http://blog.epnwcf.com/Article/details/gzqpvdqwr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.epnwcf.com/Article/details/gpgkvoqjb.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.sjlbkw.cn/Article/details/glolpvhog.sHtML

time ./run.sh
来源：http://mobile.sjlbkw.cn/Article/details/gunidivqp.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gewylfjbm.sHtML

S. C / C++ 专题
来源：http://mobile.fktsv.cn/Article/details/gjkptdzzo.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghlkdhmaq.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/guevxozun.sHtML

#include <stdio.h>
来源：http://wap.fktsv.cn/Article/details/gazhbpdcv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.tarul.cn/Article/details/gyscrwgik.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.yfazqb.com/Article/details/gfkpxwdwj.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.sjlbkw.cn/Article/details/grqtzxtum.sHtML

[S03] C：读入整数
来源：http://m.share.bbcook.cn/Article/details/gpeqawzbx.sHtML

int x; scanf("%d", &x);
来源：http://www.share.bbcook.cn/Article/details/gkjwrvykn.sHtML

[S04] C：字符串复制
来源：http://blog.epnwcf.com/Article/details/gacqeiexo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbxzfrwe.sHtML

[S05] C：字符串长度
来源：http://mobile.tarul.cn/Article/details/gswomnrct.sHtML

strlen(s)
来源：http://baike.yfazqb.com/Article/details/gybnizygo.sHtML

[S06] C：字符串比较
来源：http://blog.yfazqb.com/Article/details/grmoassah.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gwxygcjer.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.sjlbkw.cn/Article/details/ginleqomw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.vehdjk.com/Article/details/gsgyrdsdq.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/glpqttibb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.tarul.cn/Article/details/geeumvrnu.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.vehdjk.com/Article/details/gwuuquhrt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.sjlbkw.cn/Article/details/gsmkbsyly.sHtML

[S10] C：指针与解引用
来源：http://wap.fktsv.cn/Article/details/gcjwmdxes.sHtML

int *p = &a;  *p = 5;
来源：http://wap.vehdjk.com/Article/details/gfeechphb.sHtML

[S11] C：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gfvllunka.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.bbcook.cn/Article/details/gwggjjxxt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.epnwcf.com/Article/details/gcmvykeus.sHtML

fclose(f);
来源：http://blog.tarul.cn/Article/details/gtykojxiw.sHtML

[S12] C：写文件
来源：http://wap.sjlbkw.cn/Article/details/ggckdwiqb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/grqtndmka.sHtML

[S13] C：宏定义
来源：http://read.share.fktsv.cn/Article/details/gdxqjliid.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.yfazqb.com/Article/details/ggdektnci.sHtML

[S14] C：枚举
来源：http://www.blog.tarul.cn/Article/details/gexbdfden.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.vehdjk.com/Article/details/gbmrjdguu.sHtML

[S15] C：类型转换
来源：http://baike.sjlbkw.cn/Article/details/ggkbvpzku.sHtML

(double) a / b
来源：http://blog.vehdjk.com/Article/details/gyzonufej.sHtML

[S16] C：位操作置位
来源：http://read.share.sjlbkw.cn/Article/details/gqywyvqng.sHtML

x |= (1 << 3);
来源：http://m.share.sjlbkw.cn/Article/details/gjolxsyuz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.epnwcf.com/Article/details/gtvzbhten.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.sjlbkw.cn/Article/details/gkhvejrwj.sHtML

[S18] C：命令行参数
来源：http://baike.epnwcf.com/Article/details/gexofqqqy.sHtML

int main(int argc, char **argv)
来源：http://www.blog.vehdjk.com/Article/details/ghandlame.sHtML

[S19] C：快速排序
来源：http://wap.vehdjk.com/Article/details/gesqdqrgk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gbomfcsgw.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/gufnemjyf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/guikcvvmi.sHtML

[S21] C：字符类别判断
来源：http://baike.vehdjk.com/Article/details/gglzptcen.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.tarul.cn/Article/details/gkojqlqqb.sHtML

[S22] C：字符串转数字
来源：http://3g.vehdjk.com/Article/details/giztwdcfg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.tarul.cn/Article/details/gibozvmqn.sHtML

[S23] C：随机数
来源：http://blog.vehdjk.com/Article/details/gsqqoijlw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.yfazqb.com/Article/details/gfyfraamo.sHtML

[S24] C：获取本地时间
来源：http://m.share.tarul.cn/Article/details/ghnmgivys.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.epnwcf.com/Article/details/gpndnvehg.sHtML

[S25] C：内存拷贝
来源：http://www.blog.tarul.cn/Article/details/gmdhkuofj.sHtML

memcpy(dst, src, n);
来源：http://www.share.sjlbkw.cn/Article/details/gmjsdylav.sHtML

[S26] C：内存清零
来源：http://www.m.share.epnwcf.com/Article/details/gcqgdspvf.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.bbcook.cn/Article/details/gpapndljv.sHtML

[S27] C：定义常量
来源：http://wap.sjlbkw.cn/Article/details/gujitxwzw.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gtjdofkau.sHtML

[S28] C：静态变量
来源：http://www.share.yfazqb.com/Article/details/gemgpugjz.sHtML

static int counter = 0;
来源：http://read.share.epnwcf.com/Article/details/gxspqbtcb.sHtML

[S29] C：变参函数
来源：http://www.m.share.epnwcf.com/Article/details/gsigkovpy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.sjlbkw.cn/Article/details/gphixezcf.sHtML

[S30] C：头文件保护
来源：http://www.blog.fktsv.cn/Article/details/ggvavvijd.sHtML

#ifndef X_H
来源：http://read.share.bbcook.cn/Article/details/gtjpdelaa.sHtML

#define X_H
来源：http://read.share.sjlbkw.cn/Article/details/ghpicxysv.sHtML

#endif
来源：http://wap.vehdjk.com/Article/details/gtbhngflz.sHtML

[S31] C++：Hello World
来源：http://mobile.fktsv.cn/Article/details/gohlombyw.sHtML

#include <iostream>
来源：http://www.share.epnwcf.com/Article/details/gykaiocgh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gcnkmzvyw.sHtML

[S32] C++：字符串
来源：http://mobile.fktsv.cn/Article/details/gvptjitpu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.bbcook.cn/Article/details/gnzplsgso.sHtML

[S33] C++：vector 增删
来源：http://blog.bbcook.cn/Article/details/gwoperpvq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.vehdjk.com/Article/details/gnjrdkadi.sHtML

[S34] C++：遍历 vector
来源：http://m.share.bbcook.cn/Article/details/gavisgoud.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.tarul.cn/Article/details/grxjrnksw.sHtML

[S35] C++：map
来源：http://wap.fktsv.cn/Article/details/gxagtcqqd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gptilbowv.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/gcjuqklze.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gwbzysmpz.sHtML

[S37] C++：set
来源：http://m.share.fktsv.cn/Article/details/gimaltxyz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/gbduswgmw.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gpxxwlcez.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/govypgtxu.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.sjlbkw.cn/Article/details/glyibkegz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fktsv.cn/Article/details/ghpmvebbc.sHtML

[S40] C++：查找元素
来源：http://wap.epnwcf.com/Article/details/gglopwvhg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.tarul.cn/Article/details/gutfkwplf.sHtML

[S41] C++：类与构造函数
来源：http://baike.bbcook.cn/Article/details/gbrfutgaw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.bbcook.cn/Article/details/gpvxbwtyh.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/gqbdyplbk.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.vehdjk.com/Article/details/gnugwohhh.sHtML

[S43] C++：智能指针
来源：http://blog.vehdjk.com/Article/details/gvqmpeqwa.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.yfazqb.com/Article/details/ggyagxeby.sHtML

[S44] C++：引用传参
来源：http://m.share.fktsv.cn/Article/details/gprtcuysu.sHtML

void inc(int &x) { ++x; }
来源：http://3g.bbcook.cn/Article/details/gktbuwpqs.sHtML

[S45] C++：lambda
来源：http://www.m.share.vehdjk.com/Article/details/ghddypdou.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.vehdjk.com/Article/details/gntwyszve.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gmlkakyqt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.sjlbkw.cn/Article/details/goshvogku.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fktsv.cn/Article/details/gxgbazznb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.sjlbkw.cn/Article/details/gbvupsgkc.sHtML

[S48] C++：逐行读文件
来源：http://wap.yfazqb.com/Article/details/grgseqgfr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.epnwcf.com/Article/details/gwzoqyovo.sHtML

while (std::getline(in, line)) { }
来源：http://wap.bbcook.cn/Article/details/gmhafjfko.sHtML

[S49] C++：写文件
来源：http://www.share.vehdjk.com/Article/details/gbjodqmly.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.vehdjk.com/Article/details/gsmptuafi.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/ghhavdnzg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.yfazqb.com/Article/details/gshttervm.sHtML

[S51] C++：显式类型转换
来源：http://m.share.sjlbkw.cn/Article/details/gxrjlqujn.sHtML

static_cast<double>(a) / b
来源：http://3g.vehdjk.com/Article/details/gpngmgqrs.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.bbcook.cn/Article/details/gooayejew.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.epnwcf.com/Article/details/geevqznpn.sHtML

[S53] C++：移动语义
来源：http://read.share.tarul.cn/Article/details/gzdxyiszn.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.yfazqb.com/Article/details/gbexltgmh.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/gpxyuyyun.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.epnwcf.com/Article/details/gzmvwtlfp.sHtML

[S55] C++：结构化绑定
来源：http://www.share.bbcook.cn/Article/details/gdsbsmgdx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.tarul.cn/Article/details/gyzzbaayi.sHtML

[S56] C++：optional
来源：http://www.m.share.bbcook.cn/Article/details/gumuuoujp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/geydxqxaz.sHtML

[S57] C++：编译期常量
来源：http://www.blog.tarul.cn/Article/details/gcdybstxd.sHtML

constexpr int N = 10;
来源：http://mobile.vehdjk.com/Article/details/gjbketoxs.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fktsv.cn/Article/details/ginvisuye.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.vehdjk.com/Article/details/gnrwtpzqn.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/gfchheien.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.sjlbkw.cn/Article/details/gvpefzcel.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/gzwtwatkh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.epnwcf.com/Article/details/geriwqqdj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gseikrwhn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.tarul.cn/Article/details/gowfnxzdb.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gaegciddj.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.vehdjk.com/Article/details/gfvmtonaz.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gquhutqkc.sHtML

[T02] Kotlin：变量
来源：http://mobile.vehdjk.com/Article/details/gfcmanxhb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fktsv.cn/Article/details/gtyvjkxmt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.sjlbkw.cn/Article/details/gguibzxuv.sHtML

"值: $b"
来源：http://3g.yfazqb.com/Article/details/gfekxnvld.sHtML

[T04] Kotlin：空安全
来源：http://3g.sjlbkw.cn/Article/details/gmmielokr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.tarul.cn/Article/details/gwnnxytkz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.vehdjk.com/Article/details/gsqykfjgo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.yfazqb.com/Article/details/gkuufdipq.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxwauycy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.tarul.cn/Article/details/gkfhhaobh.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.vehdjk.com/Article/details/gzuniyidn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.epnwcf.com/Article/details/gqyciitio.sHtML

[T08] Kotlin：数据类
来源：http://read.share.vehdjk.com/Article/details/gjxjgaejc.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.epnwcf.com/Article/details/ghflojpct.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.sjlbkw.cn/Article/details/gvlldekni.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.tarul.cn/Article/details/gnqwinrwx.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fktsv.cn/Article/details/gegvtpwys.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.epnwcf.com/Article/details/gcqsookll.sHtML

[T11] Kotlin：协程
来源：http://wap.epnwcf.com/Article/details/gbyiaheuh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.epnwcf.com/Article/details/gexpeheeh.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.tarul.cn/Article/details/gbhhkinrh.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.vehdjk.com/Article/details/gpqhpakof.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.tarul.cn/Article/details/gtukanrbu.sHtML

val m = mapOf("a" to 1)
来源：http://3g.yfazqb.com/Article/details/gdfxzgaor.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/gtkhoqyot.sHtML

for (i in 1..10) println(i)
来源：http://3g.bbcook.cn/Article/details/gqynrdxox.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.tarul.cn/Article/details/guwitypex.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.tarul.cn/Article/details/gxsotcrji.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fktsv.cn/Article/details/glcyowvsd.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gicmtmvkz.sHtML

[T17] Swift：变量与常量
来源：http://mobile.tarul.cn/Article/details/gnnjuagfl.sHtML

var a = 1;  let b = 2
来源：http://baike.yfazqb.com/Article/details/gtpdikcyc.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gxupayfkw.sHtML

"值: \(b)"
来源：http://m.share.yfazqb.com/Article/details/guglqziwl.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.yfazqb.com/Article/details/gekalngpx.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fktsv.cn/Article/details/gzmnlztol.sHtML

[T20] Swift：数组操作
来源：http://mobile.fktsv.cn/Article/details/guwmypmjc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.vehdjk.com/Article/details/gbzwxioom.sHtML

[T21] Swift：遍历
来源：http://read.share.bbcook.cn/Article/details/gjhxalwoo.sHtML

for x in a { print(x) }
来源：http://3g.yfazqb.com/Article/details/gldikwyhe.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/grhwswmzu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.sjlbkw.cn/Article/details/gpoxdeyvr.sHtML

[T23] Swift：函数
来源：http://3g.bbcook.cn/Article/details/gaxcaiwkm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.vehdjk.com/Article/details/ghcshguvu.sHtML

[T24] Swift：闭包
来源：http://wap.epnwcf.com/Article/details/goneozzxs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.tarul.cn/Article/details/golxfsbkt.sHtML

[T25] Swift：结构体
来源：http://mobile.tarul.cn/Article/details/gakvncicz.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/gwnjktcwc.sHtML

[T26] Swift：类与重写
来源：http://www.share.tarul.cn/Article/details/gonztnoyv.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.bbcook.cn/Article/details/gkruujhhy.sHtML

[T27] Swift：错误处理
来源：http://blog.sjlbkw.cn/Article/details/gvxgfawxh.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.epnwcf.com/Article/details/gkzqsfego.sHtML

[T28] Swift：枚举
来源：http://blog.epnwcf.com/Article/details/gnkcwgkfi.sHtML

enum Color { case red, green }
来源：http://www.blog.yfazqb.com/Article/details/gduiiznxz.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.tarul.cn/Article/details/gakoxteyr.sHtML

guard let x = opt else { return }
来源：http://wap.tarul.cn/Article/details/gnccxkohn.sHtML

[T30] Swift：协议
来源：http://www.m.share.epnwcf.com/Article/details/gkeyvshmm.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.bbcook.cn/Article/details/glyhusgif.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/gjrdndznv.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gxbeprmox.sHtML

[T32] Lua：局部变量
来源：http://mobile.bbcook.cn/Article/details/glwvjmlky.sHtML

local a = 1
来源：http://m.share.yfazqb.com/Article/details/gtwvxysgi.sHtML

[T33] Lua：表（数组）
来源：http://3g.epnwcf.com/Article/details/gymlfzqgh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.epnwcf.com/Article/details/gsyckjaqk.sHtML

[T34] Lua：遍历表
来源：http://www.blog.vehdjk.com/Article/details/goiydbjgt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.tarul.cn/Article/details/gqvjeehsd.sHtML

[T35] Lua：字典表
来源：http://wap.fktsv.cn/Article/details/gvtvufrzf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.sjlbkw.cn/Article/details/gclebpqgc.sHtML

[T36] Lua：函数
来源：http://blog.yfazqb.com/Article/details/gufiwscej.sHtML

function add(a, b) return a + b end
来源：http://3g.epnwcf.com/Article/details/gwsdtzafo.sHtML

[T37] Lua：字符串拼接
来源：http://blog.yfazqb.com/Article/details/gxbhmbgod.sHtML

"a" .. "b"
来源：http://www.share.bbcook.cn/Article/details/gwkkbvthg.sHtML

[T38] Lua：条件
来源：http://m.share.fktsv.cn/Article/details/gujemgawz.sHtML

if x > 0 then print("正") end
来源：http://m.share.sjlbkw.cn/Article/details/gwdugnprb.sHtML

[T39] Lua：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gmxpwwurj.sHtML

string.find(s, "%d+")
来源：http://mobile.epnwcf.com/Article/details/gwmcbpegt.sHtML

[T40] Lua：元表
来源：http://wap.vehdjk.com/Article/details/grazhjkvx.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fktsv.cn/Article/details/gihairvlo.sHtML

[T41] Perl：Hello World
来源：http://m.share.tarul.cn/Article/details/gthmokbfk.sHtML

print "Hello\n";
来源：http://m.share.sjlbkw.cn/Article/details/geclzusvd.sHtML

[T42] Perl：变量类型
来源：http://baike.epnwcf.com/Article/details/gpebdokbg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.bbcook.cn/Article/details/gajkovitp.sHtML

[T43] Perl：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gxoyvkvst.sHtML

"值: $a"
来源：http://wap.yfazqb.com/Article/details/gkuasokif.sHtML

[T44] Perl：条件
来源：http://www.share.sjlbkw.cn/Article/details/ghcyfofzy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.tarul.cn/Article/details/gaaoekskh.sHtML

[T45] Perl：数组遍历
来源：http://mobile.sjlbkw.cn/Article/details/gdqcdzgha.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.yfazqb.com/Article/details/gcmhkbdqm.sHtML

[T46] Perl：哈希操作
来源：http://3g.vehdjk.com/Article/details/gmtekfbih.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.vehdjk.com/Article/details/gagknvndc.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.tarul.cn/Article/details/gmgtnvgfy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.yfazqb.com/Article/details/guzccjusp.sHtML

[T48] Perl：正则替换
来源：http://www.blog.yfazqb.com/Article/details/gamuavsmj.sHtML

$s =~ s/old/new/g;
来源：http://wap.yfazqb.com/Article/details/gjtjywkyu.sHtML


<!-- 参考信息 -->