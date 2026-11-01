代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/ghmypnbor.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/gzihdojco.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.epnwcf.com/Article/details/grltdqlnh.sHtML

[R47] sed 单行替换
来源：http://www.share.fktsv.cn/Article/details/gfthaesrl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.epnwcf.com/Article/details/gqzexxdpq.sHtML

[R48] awk 取指定列
来源：http://wap.yfazqb.com/Article/details/gfzyuppuz.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.bbcook.cn/Article/details/gbhwptbru.sHtML

[R49] awk 带条件
来源：http://wap.fktsv.cn/Article/details/gvbshnmul.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.bbcook.cn/Article/details/ggxijbdjj.sHtML

[R50] awk 求和
来源：http://www.blog.bbcook.cn/Article/details/gmsttqqjg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gpkzxcdii.sHtML

[R51] 排序去重取前几
来源：http://wap.fktsv.cn/Article/details/gnwgcsfkf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.epnwcf.com/Article/details/gzoraaeqe.sHtML

[R52] 统计行数
来源：http://www.share.yfazqb.com/Article/details/ghwiftvni.sHtML

wc -l a.txt
来源：http://baike.tarul.cn/Article/details/grbxabbgw.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.sjlbkw.cn/Article/details/gmzxvzbhs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.bbcook.cn/Article/details/gsrkosois.sHtML

[R54] 比较两个文件
来源：http://www.share.fktsv.cn/Article/details/gbvjbrlji.sHtML

diff a.txt b.txt
来源：http://www.share.epnwcf.com/Article/details/gtzcaxcvw.sHtML

[R55] 压缩与解压
来源：http://www.share.epnwcf.com/Article/details/gjpuzwyvx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.epnwcf.com/Article/details/glkhrrnla.sHtML

[R56] 远程拷贝
来源：http://blog.bbcook.cn/Article/details/gqhkwjweh.sHtML

scp file user@host:/path/
来源：http://m.share.tarul.cn/Article/details/gfznyfofn.sHtML

[R57] 远程执行命令
来源：http://wap.epnwcf.com/Article/details/govolkqqz.sHtML

ssh user@host 'uptime'
来源：http://www.blog.bbcook.cn/Article/details/gmdzvzyvf.sHtML

[R58] 下载文件
来源：http://m.share.yfazqb.com/Article/details/ggwljpcky.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.bbcook.cn/Article/details/ghuitnavz.sHtML

[R59] 发 POST JSON
来源：http://blog.epnwcf.com/Article/details/gapptiolc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.yfazqb.com/Article/details/gwzehrqma.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgozwdnf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.sjlbkw.cn/Article/details/gfoqinktm.sHtML

[R61] 磁盘占用
来源：http://baike.yfazqb.com/Article/details/gqbbqrilj.sHtML

df -h;  du -sh *
来源：http://3g.sjlbkw.cn/Article/details/gddzstyas.sHtML

[R62] 找最占空间的文件
来源：http://wap.sjlbkw.cn/Article/details/gdwwnoxdu.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fktsv.cn/Article/details/gwpxxgpmy.sHtML

[R63] 内存与进程
来源：http://read.share.yfazqb.com/Article/details/gibhedmng.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/gcdxlkfgx.sHtML

[R64] 结束进程
来源：http://3g.vehdjk.com/Article/details/gdafnukeu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fktsv.cn/Article/details/gpehuoasn.sHtML

[R65] 查看端口占用
来源：http://baike.yfazqb.com/Article/details/ghlbzlnmg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.yfazqb.com/Article/details/gbctgvunm.sHtML

[R66] 定时任务
来源：http://www.share.sjlbkw.cn/Article/details/gzlbujtnx.sHtML

crontab -e;  crontab -l
来源：http://m.share.bbcook.cn/Article/details/gwguxaszo.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.epnwcf.com/Article/details/gtxootmvr.sHtML

openssl rand -hex 16
来源：http://m.share.bbcook.cn/Article/details/gnuripbwb.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/gcwtwsypd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fktsv.cn/Article/details/gjujaplbz.sHtML

[R69] 生成随机密码
来源：http://www.blog.epnwcf.com/Article/details/gymvwrnvo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.tarul.cn/Article/details/gsatkmzks.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fktsv.cn/Article/details/guqpluhai.sHtML

date +%s;  date -d @1700000000
来源：http://baike.bbcook.cn/Article/details/gmhqlbvqf.sHtML

[R71] 日期格式化
来源：http://mobile.epnwcf.com/Article/details/gyspyduug.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.sjlbkw.cn/Article/details/ggjpfvcvl.sHtML

[R72] 等待端口就绪
来源：http://blog.bbcook.cn/Article/details/gakfwzhll.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gjebbqjfw.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/gapehmhph.sHtML

split -l 1000 big.log part_
来源：http://3g.tarul.cn/Article/details/gbbmhjomg.sHtML

[R74] 批量重命名
来源：http://baike.vehdjk.com/Article/details/gxfdfidlb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fktsv.cn/Article/details/grpmwmqwn.sHtML

[R75] 导出环境变量
来源：http://wap.fktsv.cn/Article/details/gbwmlwpvd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.bbcook.cn/Article/details/gyffulinb.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/gvkefnprk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gfakdhagy.sHtML

[R77] 读取用户输入
来源：http://3g.epnwcf.com/Article/details/ghnajkwjw.sHtML

read -rp "请输入: " ans
来源：http://mobile.tarul.cn/Article/details/ggjduzjol.sHtML

[R78] 交互式菜单
来源：http://www.blog.epnwcf.com/Article/details/gnfgsmbiw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.vehdjk.com/Article/details/ghtofkatf.sHtML

[R79] 解析命令行选项
来源：http://wap.epnwcf.com/Article/details/gscmtakpp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.tarul.cn/Article/details/gtklerodt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.epnwcf.com/Article/details/gccohjait.sHtML

time ./run.sh
来源：http://baike.sjlbkw.cn/Article/details/glbksvyix.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdjibpaqu.sHtML

S. C / C++ 专题
来源：http://wap.bbcook.cn/Article/details/gryntqlvc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gcpifxzlq.sHtML

[S01] C：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gwjbgnywu.sHtML

#include <stdio.h>
来源：http://3g.yfazqb.com/Article/details/gwzphngjl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.vehdjk.com/Article/details/gobrfpzbz.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/ggfsqsvta.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fktsv.cn/Article/details/gzszzzbiw.sHtML

[S03] C：读入整数
来源：http://wap.vehdjk.com/Article/details/gilnfuniq.sHtML

int x; scanf("%d", &x);
来源：http://read.share.tarul.cn/Article/details/gmmdajcme.sHtML

[S04] C：字符串复制
来源：http://wap.vehdjk.com/Article/details/gczytvgfu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.bbcook.cn/Article/details/gacqnjggn.sHtML

[S05] C：字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gdkkbgbir.sHtML

strlen(s)
来源：http://blog.bbcook.cn/Article/details/gtcowhmfm.sHtML

[S06] C：字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gweotxcpu.sHtML

strcmp(a, b) == 0
来源：http://baike.bbcook.cn/Article/details/gnckdotyp.sHtML

[S07] C：数组遍历求和
来源：http://read.share.epnwcf.com/Article/details/gkjbbutwc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.bbcook.cn/Article/details/gadhffsqd.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.sjlbkw.cn/Article/details/gkbbqujew.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.vehdjk.com/Article/details/grasghfxl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.vehdjk.com/Article/details/gerizapir.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.bbcook.cn/Article/details/gyqausbvx.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.yfazqb.com/Article/details/gcmzibgpv.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.tarul.cn/Article/details/gmzpwlapx.sHtML

[S11] C：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gauckserm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/gejvpkgqh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.tarul.cn/Article/details/giwizntnn.sHtML

fclose(f);
来源：http://3g.tarul.cn/Article/details/gkjmzbgnr.sHtML

[S12] C：写文件
来源：http://read.share.epnwcf.com/Article/details/gvdhqxqjd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gvdhsranp.sHtML

[S13] C：宏定义
来源：http://blog.fktsv.cn/Article/details/gqqgmxmbl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.sjlbkw.cn/Article/details/gufagepyb.sHtML

[S14] C：枚举
来源：http://wap.yfazqb.com/Article/details/gnfepwgoy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.tarul.cn/Article/details/gvdlutdte.sHtML

[S15] C：类型转换
来源：http://blog.sjlbkw.cn/Article/details/ghzjmslkv.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gufsdoxcj.sHtML

[S16] C：位操作置位
来源：http://baike.sjlbkw.cn/Article/details/gptfsqwqp.sHtML

x |= (1 << 3);
来源：http://baike.sjlbkw.cn/Article/details/gwdgrhvra.sHtML

[S17] C：安全拼接字符串
来源：http://blog.vehdjk.com/Article/details/gmdxjdkis.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.vehdjk.com/Article/details/gsxbgknkf.sHtML

[S18] C：命令行参数
来源：http://mobile.fktsv.cn/Article/details/gzndzvjgf.sHtML

int main(int argc, char **argv)
来源：http://baike.vehdjk.com/Article/details/gzlefhhvd.sHtML

[S19] C：快速排序
来源：http://www.m.share.vehdjk.com/Article/details/gobtbmbbz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gbmloafrk.sHtML

[S20] C：二分查找
来源：http://read.share.fktsv.cn/Article/details/gmzrjdldj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gawdiqdqr.sHtML

[S21] C：字符类别判断
来源：http://blog.yfazqb.com/Article/details/gcdpeupxd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fktsv.cn/Article/details/gpgeyckhw.sHtML

[S22] C：字符串转数字
来源：http://www.blog.yfazqb.com/Article/details/gjlgwtpye.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/gjpshxuwr.sHtML

[S23] C：随机数
来源：http://www.blog.bbcook.cn/Article/details/gebxugmxd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.vehdjk.com/Article/details/gaqqqwkdl.sHtML

[S24] C：获取本地时间
来源：http://baike.epnwcf.com/Article/details/gvaqjgpyy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.epnwcf.com/Article/details/ghclxczcw.sHtML

[S25] C：内存拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gdypsvxwx.sHtML

memcpy(dst, src, n);
来源：http://www.share.sjlbkw.cn/Article/details/gumivjlne.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/gmgmglmwb.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.yfazqb.com/Article/details/gvrusvvyp.sHtML

[S27] C：定义常量
来源：http://blog.bbcook.cn/Article/details/gdonoxkug.sHtML

const double PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/ghsdqsehf.sHtML

[S28] C：静态变量
来源：http://www.m.share.vehdjk.com/Article/details/gmigezxkw.sHtML

static int counter = 0;
来源：http://m.share.sjlbkw.cn/Article/details/gyckyxtxp.sHtML

[S29] C：变参函数
来源：http://www.m.share.epnwcf.com/Article/details/ghtroyacg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fktsv.cn/Article/details/gauhqjyie.sHtML

[S30] C：头文件保护
来源：http://www.m.share.vehdjk.com/Article/details/gtojasxzn.sHtML

#ifndef X_H
来源：http://3g.fktsv.cn/Article/details/gszbpwmvr.sHtML

#define X_H
来源：http://m.share.tarul.cn/Article/details/gamixmlqp.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/givtmzkpt.sHtML

[S31] C++：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gzaerqlvb.sHtML

#include <iostream>
来源：http://www.blog.epnwcf.com/Article/details/gdwzfgvgp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fktsv.cn/Article/details/gipwxpkzt.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/gcairlztv.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.sjlbkw.cn/Article/details/gkdqqmlbl.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/gnqpvgmfy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.bbcook.cn/Article/details/gsweddbeo.sHtML

[S34] C++：遍历 vector
来源：http://m.share.tarul.cn/Article/details/gulgqpvbu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/glyvqubkb.sHtML

[S35] C++：map
来源：http://m.share.yfazqb.com/Article/details/ghqxryuuq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/ganbnowfj.sHtML

[S36] C++：unordered_map
来源：http://3g.tarul.cn/Article/details/gmdqwwjcr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gpmjttqlx.sHtML

[S37] C++：set
来源：http://blog.yfazqb.com/Article/details/gqknlodes.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.sjlbkw.cn/Article/details/ginzffirf.sHtML

[S38] C++：排序
来源：http://wap.vehdjk.com/Article/details/gchttximm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gzxwdxtcl.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.epnwcf.com/Article/details/gbqozvylf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.tarul.cn/Article/details/gaemdpjkt.sHtML

[S40] C++：查找元素
来源：http://3g.vehdjk.com/Article/details/gluqbcuau.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.epnwcf.com/Article/details/gqwktjbgv.sHtML

[S41] C++：类与构造函数
来源：http://m.share.epnwcf.com/Article/details/gpxzntuut.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.bbcook.cn/Article/details/glyhbvqnb.sHtML

[S42] C++：继承与虚函数
来源：http://wap.yfazqb.com/Article/details/gvqztztsd.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.vehdjk.com/Article/details/gpukcljdg.sHtML

[S43] C++：智能指针
来源：http://blog.vehdjk.com/Article/details/gtlxdriiy.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.sjlbkw.cn/Article/details/gzrzjaxcf.sHtML

[S44] C++：引用传参
来源：http://mobile.tarul.cn/Article/details/gjekekunw.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.tarul.cn/Article/details/gdbfymbjw.sHtML

[S45] C++：lambda
来源：http://mobile.sjlbkw.cn/Article/details/gsgcdnsvd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gojieyhho.sHtML

[S46] C++：函数模板
来源：http://www.blog.sjlbkw.cn/Article/details/gqsrzhbhf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/gxahhogat.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.tarul.cn/Article/details/glwvchovd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.tarul.cn/Article/details/gjvyaawwm.sHtML

[S48] C++：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gwxqtayyr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fktsv.cn/Article/details/glojpzwcd.sHtML

while (std::getline(in, line)) { }
来源：http://wap.bbcook.cn/Article/details/gtfeqqdci.sHtML

[S49] C++：写文件
来源：http://m.share.tarul.cn/Article/details/gmhbsmwso.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.bbcook.cn/Article/details/gibdbrrft.sHtML

[S50] C++：格式化数字
来源：http://blog.vehdjk.com/Article/details/ghfimdgqz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/grvzdmzar.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.epnwcf.com/Article/details/gsbcdfbdv.sHtML

static_cast<double>(a) / b
来源：http://read.share.tarul.cn/Article/details/gsnlisnls.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fktsv.cn/Article/details/gsjlnnkmc.sHtML

int size() const noexcept { return n_; }
来源：http://wap.epnwcf.com/Article/details/gcvundvuy.sHtML

[S53] C++：移动语义
来源：http://read.share.sjlbkw.cn/Article/details/gdbnqezxa.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.epnwcf.com/Article/details/gcqvpbhto.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/grlaasfsr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.sjlbkw.cn/Article/details/ghftyfflu.sHtML

[S55] C++：结构化绑定
来源：http://mobile.tarul.cn/Article/details/gaauljoza.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.epnwcf.com/Article/details/ggyjayosg.sHtML

[S56] C++：optional
来源：http://www.share.epnwcf.com/Article/details/gxiqhnifx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.bbcook.cn/Article/details/gtpyjuyty.sHtML

[S57] C++：编译期常量
来源：http://www.blog.bbcook.cn/Article/details/gxcecmeou.sHtML

constexpr int N = 10;
来源：http://read.share.epnwcf.com/Article/details/gupnzgwxh.sHtML

[S58] C++：命名空间
来源：http://baike.yfazqb.com/Article/details/gepulupqw.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.vehdjk.com/Article/details/ghjtyvebb.sHtML

[S59] C++：静态断言
来源：http://read.share.yfazqb.com/Article/details/ghvhmjygj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.bbcook.cn/Article/details/gedkjgiiz.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.sjlbkw.cn/Article/details/genyukjbh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fktsv.cn/Article/details/gjmpmplwi.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/guevrdrzc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.sjlbkw.cn/Article/details/gwmestaut.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gldjurfpj.sHtML

[T01] Kotlin：Hello World
来源：http://baike.vehdjk.com/Article/details/gtfxbhgfe.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gxzfjsput.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fktsv.cn/Article/details/gtykfmdus.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.epnwcf.com/Article/details/gpsokooov.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.tarul.cn/Article/details/gtjwzvxnz.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/gmnvakmtz.sHtML

[T04] Kotlin：空安全
来源：http://wap.tarul.cn/Article/details/grxsuvhrf.sHtML

val n: String? = null;  n?.length
来源：http://blog.yfazqb.com/Article/details/ggcqjrorh.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.bbcook.cn/Article/details/gztrikwsr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.sjlbkw.cn/Article/details/gptjzqluv.sHtML

[T06] Kotlin：集合映射
来源：http://3g.bbcook.cn/Article/details/gjqxrhxvj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/gzvciwqmy.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.bbcook.cn/Article/details/gszxdakxl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.vehdjk.com/Article/details/gltmudcas.sHtML

[T08] Kotlin：数据类
来源：http://m.share.tarul.cn/Article/details/gdeueotgc.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gxeplhjro.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.epnwcf.com/Article/details/gbqcirnjn.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.tarul.cn/Article/details/ggaqjfljb.sHtML

[T10] Kotlin：默认参数
来源：http://blog.bbcook.cn/Article/details/gwbysvvcu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.epnwcf.com/Article/details/ghmxkgkws.sHtML

[T11] Kotlin：协程
来源：http://blog.yfazqb.com/Article/details/gfzfphanj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.bbcook.cn/Article/details/gdwoesnrk.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.yfazqb.com/Article/details/gbeuijqtz.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.yfazqb.com/Article/details/gphkblbvq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.tarul.cn/Article/details/gxcjzqdfq.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gongnhksu.sHtML

[T14] Kotlin：循环
来源：http://read.share.yfazqb.com/Article/details/gdwxicdvy.sHtML

for (i in 1..10) println(i)
来源：http://read.share.yfazqb.com/Article/details/grqmfrjiv.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.sjlbkw.cn/Article/details/gqytomyvm.sHtML

interface Shape { fun area(): Double }
来源：http://3g.sjlbkw.cn/Article/details/gswhwwzag.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gcdsnmkre.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gdzkjumjk.sHtML

[T17] Swift：变量与常量
来源：http://baike.tarul.cn/Article/details/gjtxwsygy.sHtML

var a = 1;  let b = 2
来源：http://www.share.tarul.cn/Article/details/gabkzdofm.sHtML

[T18] Swift：字符串插值
来源：http://3g.epnwcf.com/Article/details/glzlfpsgk.sHtML

"值: \(b)"
来源：http://read.share.vehdjk.com/Article/details/goxntibny.sHtML

[T19] Swift：可选绑定
来源：http://baike.yfazqb.com/Article/details/gefchomty.sHtML

if let n = opt { print(n) }
来源：http://www.blog.yfazqb.com/Article/details/gtkwszuet.sHtML

[T20] Swift：数组操作
来源：http://baike.tarul.cn/Article/details/gwfeasdbm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.tarul.cn/Article/details/gmrdtxbqp.sHtML

[T21] Swift：遍历
来源：http://baike.sjlbkw.cn/Article/details/gitmceisk.sHtML

for x in a { print(x) }
来源：http://www.share.sjlbkw.cn/Article/details/gmywxrkvq.sHtML

[T22] Swift：字典
来源：http://www.blog.epnwcf.com/Article/details/gbdvbxdqw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.yfazqb.com/Article/details/gubjtjqqp.sHtML

[T23] Swift：函数
来源：http://www.blog.vehdjk.com/Article/details/guvpcmwkx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.yfazqb.com/Article/details/gpicgwjzq.sHtML

[T24] Swift：闭包
来源：http://wap.tarul.cn/Article/details/gchifcvcd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.yfazqb.com/Article/details/guvflyyru.sHtML

[T25] Swift：结构体
来源：http://mobile.sjlbkw.cn/Article/details/gjkrabchc.sHtML

struct P { var x: Int }
来源：http://www.share.bbcook.cn/Article/details/ghaixhyuo.sHtML

[T26] Swift：类与重写
来源：http://read.share.tarul.cn/Article/details/grtvegbsb.sHtML

class A: Base { override func f() {} }
来源：http://m.share.yfazqb.com/Article/details/gsmkpfjyl.sHtML

[T27] Swift：错误处理
来源：http://m.share.fktsv.cn/Article/details/gdbjofkum.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.bbcook.cn/Article/details/gklmoqpqn.sHtML

[T28] Swift：枚举
来源：http://3g.vehdjk.com/Article/details/gcgwodoek.sHtML

enum Color { case red, green }
来源：http://m.share.fktsv.cn/Article/details/ghpoleizk.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.bbcook.cn/Article/details/gwwpkkxjp.sHtML

guard let x = opt else { return }
来源：http://www.m.share.yfazqb.com/Article/details/gvlntfrlb.sHtML

[T30] Swift：协议
来源：http://www.blog.sjlbkw.cn/Article/details/gjoblaukn.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.bbcook.cn/Article/details/gskbvuufk.sHtML

[T31] Lua：Hello World
来源：http://www.blog.tarul.cn/Article/details/gwxiejudm.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gpimfmbww.sHtML

[T32] Lua：局部变量
来源：http://wap.tarul.cn/Article/details/geaxawxdv.sHtML

local a = 1
来源：http://read.share.yfazqb.com/Article/details/gthhyiflc.sHtML

[T33] Lua：表（数组）
来源：http://read.share.bbcook.cn/Article/details/gstpulllv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.vehdjk.com/Article/details/gmtclnhar.sHtML

[T34] Lua：遍历表
来源：http://m.share.vehdjk.com/Article/details/gmbzlvryg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fktsv.cn/Article/details/gwbgonrfu.sHtML

[T35] Lua：字典表
来源：http://m.share.fktsv.cn/Article/details/giveylimg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gmmadsfxs.sHtML

[T36] Lua：函数
来源：http://3g.bbcook.cn/Article/details/gogrytmma.sHtML

function add(a, b) return a + b end
来源：http://www.blog.bbcook.cn/Article/details/gmdkywrlq.sHtML

[T37] Lua：字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gwfdivepi.sHtML

"a" .. "b"
来源：http://3g.epnwcf.com/Article/details/glzwocozj.sHtML

[T38] Lua：条件
来源：http://3g.tarul.cn/Article/details/gdfdipzgq.sHtML

if x > 0 then print("正") end
来源：http://m.share.epnwcf.com/Article/details/gixpfzfqi.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fktsv.cn/Article/details/gpftebtsn.sHtML

string.find(s, "%d+")
来源：http://baike.yfazqb.com/Article/details/gwrvozday.sHtML

[T40] Lua：元表
来源：http://wap.tarul.cn/Article/details/guuektkwj.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.sjlbkw.cn/Article/details/gngwjsviy.sHtML

[T41] Perl：Hello World
来源：http://3g.tarul.cn/Article/details/gqcehihlf.sHtML

print "Hello\n";
来源：http://mobile.bbcook.cn/Article/details/ghwvcbntp.sHtML

[T42] Perl：变量类型
来源：http://baike.bbcook.cn/Article/details/gxqjfkjng.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.bbcook.cn/Article/details/gtjkaizhv.sHtML

[T43] Perl：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gnhnwapjo.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/ghjpqxvas.sHtML

[T44] Perl：条件
来源：http://3g.epnwcf.com/Article/details/gyzogiybi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.vehdjk.com/Article/details/gjndtbtep.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.tarul.cn/Article/details/gzwkirolz.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.bbcook.cn/Article/details/gluswmmno.sHtML

[T46] Perl：哈希操作
来源：http://www.share.yfazqb.com/Article/details/gmvyagkhf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.tarul.cn/Article/details/ghvzaxbtd.sHtML

[T47] Perl：正则捕获
来源：http://baike.sjlbkw.cn/Article/details/gwenvfjty.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fktsv.cn/Article/details/gfwznvtyu.sHtML

[T48] Perl：正则替换
来源：http://read.share.fktsv.cn/Article/details/gmdcafvqa.sHtML

$s =~ s/old/new/g;
来源：http://3g.sjlbkw.cn/Article/details/gkutububc.sHtML


<!-- 参考信息 -->