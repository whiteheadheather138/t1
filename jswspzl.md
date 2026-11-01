代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.epnwcf.com/Article/details/gufbtvlmj.sHtML

[R50] awk 求和
来源：http://www.m.share.epnwcf.com/Article/details/gtiiyqycx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fktsv.cn/Article/details/gjwdfysvi.sHtML

[R51] 排序去重取前几
来源：http://3g.epnwcf.com/Article/details/godptvlxa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fktsv.cn/Article/details/gtkefrbax.sHtML

[R52] 统计行数
来源：http://blog.yfazqb.com/Article/details/gcwsogpvq.sHtML

wc -l a.txt
来源：http://www.blog.yfazqb.com/Article/details/gqbxuiane.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gamukhiho.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.tarul.cn/Article/details/gbuptdjeq.sHtML

[R54] 比较两个文件
来源：http://www.blog.epnwcf.com/Article/details/gkqbdcidv.sHtML

diff a.txt b.txt
来源：http://baike.yfazqb.com/Article/details/grgrrejgo.sHtML

[R55] 压缩与解压
来源：http://www.m.share.vehdjk.com/Article/details/getvzxkpb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.sjlbkw.cn/Article/details/gskarlzcf.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/gihfudqxg.sHtML

scp file user@host:/path/
来源：http://read.share.yfazqb.com/Article/details/gbyybltje.sHtML

[R57] 远程执行命令
来源：http://3g.epnwcf.com/Article/details/gvogibsbp.sHtML

ssh user@host 'uptime'
来源：http://mobile.sjlbkw.cn/Article/details/givlctytw.sHtML

[R58] 下载文件
来源：http://mobile.sjlbkw.cn/Article/details/gikajsack.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.tarul.cn/Article/details/ggcdgrdop.sHtML

[R59] 发 POST JSON
来源：http://baike.fktsv.cn/Article/details/geuiwjjzk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.bbcook.cn/Article/details/gflteegeo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gnexrjffq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.vehdjk.com/Article/details/gtolbxmql.sHtML

[R61] 磁盘占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzrkaqqi.sHtML

df -h;  du -sh *
来源：http://www.share.sjlbkw.cn/Article/details/giiwmwalm.sHtML

[R62] 找最占空间的文件
来源：http://wap.tarul.cn/Article/details/gbihxvacc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fktsv.cn/Article/details/grhnckrba.sHtML

[R63] 内存与进程
来源：http://www.share.yfazqb.com/Article/details/gbajmjhnu.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.bbcook.cn/Article/details/guumrzlvs.sHtML

[R64] 结束进程
来源：http://wap.yfazqb.com/Article/details/grkwgagen.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.yfazqb.com/Article/details/grsdvyedf.sHtML

[R65] 查看端口占用
来源：http://wap.fktsv.cn/Article/details/gckcyiqhl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.epnwcf.com/Article/details/ghiqbipsg.sHtML

[R66] 定时任务
来源：http://baike.vehdjk.com/Article/details/gvjqsjnzf.sHtML

crontab -e;  crontab -l
来源：http://read.share.vehdjk.com/Article/details/goydvikgf.sHtML

[R67] 生成随机十六进制串
来源：http://wap.sjlbkw.cn/Article/details/gbpczktez.sHtML

openssl rand -hex 16
来源：http://mobile.vehdjk.com/Article/details/gjpmxqzdx.sHtML

[R68] 计算文件校验值
来源：http://3g.yfazqb.com/Article/details/gpuyvurkb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.tarul.cn/Article/details/glmqtcmjd.sHtML

[R69] 生成随机密码
来源：http://wap.bbcook.cn/Article/details/gganfogfc.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.yfazqb.com/Article/details/gxlgdaygp.sHtML

[R70] 时间戳与互转
来源：http://www.share.yfazqb.com/Article/details/gjanzawqe.sHtML

date +%s;  date -d @1700000000
来源：http://3g.tarul.cn/Article/details/gfwkdrvih.sHtML

[R71] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gxsjfvjvl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.sjlbkw.cn/Article/details/gwrmhbqty.sHtML

[R72] 等待端口就绪
来源：http://www.share.epnwcf.com/Article/details/gafwxfaqe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gqjgfwlnr.sHtML

[R73] 分割大日志
来源：http://wap.bbcook.cn/Article/details/guijjtwxu.sHtML

split -l 1000 big.log part_
来源：http://3g.sjlbkw.cn/Article/details/gnzafbcgh.sHtML

[R74] 批量重命名
来源：http://www.share.sjlbkw.cn/Article/details/gporfkkmt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/gqtbesxmh.sHtML

[R75] 导出环境变量
来源：http://3g.vehdjk.com/Article/details/gwoiqfzqd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.tarul.cn/Article/details/grcjfontf.sHtML

[R76] 使用临时文件
来源：http://blog.tarul.cn/Article/details/gqvxgfdlh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gjjyeesgy.sHtML

[R77] 读取用户输入
来源：http://blog.epnwcf.com/Article/details/gpdavexnr.sHtML

read -rp "请输入: " ans
来源：http://3g.yfazqb.com/Article/details/gxpqcshmk.sHtML

[R78] 交互式菜单
来源：http://3g.fktsv.cn/Article/details/glmzerrya.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/gghocoobe.sHtML

[R79] 解析命令行选项
来源：http://www.blog.yfazqb.com/Article/details/grzggwhib.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.sjlbkw.cn/Article/details/gokfoxrcs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.tarul.cn/Article/details/gquurloaa.sHtML

time ./run.sh
来源：http://mobile.yfazqb.com/Article/details/gygttgcdr.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gqvpxnnhs.sHtML

S. C / C++ 专题
来源：http://www.m.share.tarul.cn/Article/details/gmrsbymnv.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gaapzxkpf.sHtML

[S01] C：Hello World
来源：http://read.share.vehdjk.com/Article/details/ggsfsoyey.sHtML

#include <stdio.h>
来源：http://www.blog.sjlbkw.cn/Article/details/gjkcjvple.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.bbcook.cn/Article/details/gkxqpsuab.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.epnwcf.com/Article/details/grzawcidq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gwzxpwooc.sHtML

[S03] C：读入整数
来源：http://blog.sjlbkw.cn/Article/details/ghmibkhts.sHtML

int x; scanf("%d", &x);
来源：http://m.share.yfazqb.com/Article/details/glgdjnscl.sHtML

[S04] C：字符串复制
来源：http://www.share.tarul.cn/Article/details/gwfvkrrah.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.tarul.cn/Article/details/gxeinfwtm.sHtML

[S05] C：字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gxmjipodx.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/gejmkqwma.sHtML

[S06] C：字符串比较
来源：http://wap.vehdjk.com/Article/details/gvascpltf.sHtML

strcmp(a, b) == 0
来源：http://3g.fktsv.cn/Article/details/gjwcafuzm.sHtML

[S07] C：数组遍历求和
来源：http://baike.tarul.cn/Article/details/gierbmqxp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.tarul.cn/Article/details/gzmyglvur.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.tarul.cn/Article/details/gcxpdxuwj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.tarul.cn/Article/details/gaytbcgus.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.sjlbkw.cn/Article/details/gsiwafyld.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/gdagnefcf.sHtML

[S10] C：指针与解引用
来源：http://blog.fktsv.cn/Article/details/gjzodnkgw.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.epnwcf.com/Article/details/gkeddzodd.sHtML

[S11] C：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/grnxpgqce.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.epnwcf.com/Article/details/geresgkir.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.vehdjk.com/Article/details/gpgemlnus.sHtML

fclose(f);
来源：http://mobile.tarul.cn/Article/details/gwpgnbbgo.sHtML

[S12] C：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gyorsctyq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.yfazqb.com/Article/details/ghgxucvof.sHtML

[S13] C：宏定义
来源：http://wap.yfazqb.com/Article/details/gwrtphhiv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.bbcook.cn/Article/details/gyzxlflbn.sHtML

[S14] C：枚举
来源：http://mobile.vehdjk.com/Article/details/gnstwneth.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.yfazqb.com/Article/details/gzzbuzorm.sHtML

[S15] C：类型转换
来源：http://blog.fktsv.cn/Article/details/gmjxplsnz.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/gwthwhxty.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/gxzparjpx.sHtML

x |= (1 << 3);
来源：http://www.share.epnwcf.com/Article/details/gpvqeggkk.sHtML

[S17] C：安全拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gxvzgumsc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.epnwcf.com/Article/details/gctxzxgeq.sHtML

[S18] C：命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gprhntrgu.sHtML

int main(int argc, char **argv)
来源：http://www.blog.epnwcf.com/Article/details/geuyptljp.sHtML

[S19] C：快速排序
来源：http://m.share.bbcook.cn/Article/details/gbseknmee.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gkydnaton.sHtML

[S20] C：二分查找
来源：http://mobile.fktsv.cn/Article/details/gkcthxfnb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/ghulkhvpo.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.yfazqb.com/Article/details/gbtmpdppw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fktsv.cn/Article/details/ghxgwtfdc.sHtML

[S22] C：字符串转数字
来源：http://www.blog.bbcook.cn/Article/details/gevjfakhu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.sjlbkw.cn/Article/details/gjgjekyan.sHtML

[S23] C：随机数
来源：http://read.share.vehdjk.com/Article/details/ggptmyzzk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/glnhxxuus.sHtML

[S24] C：获取本地时间
来源：http://3g.bbcook.cn/Article/details/gapcbzyqw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fktsv.cn/Article/details/gdpqescev.sHtML

[S25] C：内存拷贝
来源：http://mobile.yfazqb.com/Article/details/gvupmuumo.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/gbtwtsjga.sHtML

[S26] C：内存清零
来源：http://read.share.fktsv.cn/Article/details/grunsctef.sHtML

memset(a, 0, sizeof a);
来源：http://baike.epnwcf.com/Article/details/gyfbfmyad.sHtML

[S27] C：定义常量
来源：http://blog.bbcook.cn/Article/details/gpmulperq.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gnukawqtk.sHtML

[S28] C：静态变量
来源：http://m.share.sjlbkw.cn/Article/details/gzvzjgujh.sHtML

static int counter = 0;
来源：http://www.share.vehdjk.com/Article/details/gltypasnm.sHtML

[S29] C：变参函数
来源：http://www.m.share.vehdjk.com/Article/details/gdvewlkky.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/geavzjrdy.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/gjdhbygml.sHtML

#ifndef X_H
来源：http://www.blog.vehdjk.com/Article/details/gczueqlhh.sHtML

#define X_H
来源：http://baike.epnwcf.com/Article/details/gpwsqruop.sHtML

#endif
来源：http://www.share.yfazqb.com/Article/details/gpimulpbj.sHtML

[S31] C++：Hello World
来源：http://read.share.yfazqb.com/Article/details/gzkzzggtf.sHtML

#include <iostream>
来源：http://blog.bbcook.cn/Article/details/gpuprbxbw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.yfazqb.com/Article/details/gficxicfz.sHtML

[S32] C++：字符串
来源：http://baike.vehdjk.com/Article/details/gczrqmoqt.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/gpwqfoylp.sHtML

[S33] C++：vector 增删
来源：http://www.blog.tarul.cn/Article/details/ggysnelly.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.tarul.cn/Article/details/ggjvtixmz.sHtML

[S34] C++：遍历 vector
来源：http://baike.yfazqb.com/Article/details/gjiibtyzg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.sjlbkw.cn/Article/details/gctdhqbjv.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/glozsmewf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gafprxlmd.sHtML

[S36] C++：unordered_map
来源：http://wap.vehdjk.com/Article/details/guuldsvmv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/giovhrhss.sHtML

[S37] C++：set
来源：http://3g.epnwcf.com/Article/details/gadqzjguf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.bbcook.cn/Article/details/gubqywbox.sHtML

[S38] C++：排序
来源：http://www.blog.tarul.cn/Article/details/gdcawsocf.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.epnwcf.com/Article/details/goefzjbbx.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.bbcook.cn/Article/details/ghtvohitt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.vehdjk.com/Article/details/gcbzbqyif.sHtML

[S40] C++：查找元素
来源：http://www.m.share.vehdjk.com/Article/details/gsdwvqxdo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fktsv.cn/Article/details/gbpuxryst.sHtML

[S41] C++：类与构造函数
来源：http://blog.tarul.cn/Article/details/gqrwwwtvi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.vehdjk.com/Article/details/ghjowkfhc.sHtML

[S42] C++：继承与虚函数
来源：http://blog.yfazqb.com/Article/details/gzdqxpejc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.bbcook.cn/Article/details/gxrjvedmh.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gnetdzvzy.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fktsv.cn/Article/details/grticwddl.sHtML

[S44] C++：引用传参
来源：http://m.share.bbcook.cn/Article/details/gpfhvqwyc.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fktsv.cn/Article/details/ggdhnrcba.sHtML

[S45] C++：lambda
来源：http://www.m.share.vehdjk.com/Article/details/gbohbrmsk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.sjlbkw.cn/Article/details/gmdvavscp.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gwnxiqbob.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.sjlbkw.cn/Article/details/gqbggtzib.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.vehdjk.com/Article/details/guwfdcgyd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fktsv.cn/Article/details/grxfmccwf.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gxbicdtav.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.bbcook.cn/Article/details/gckrscepe.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.vehdjk.com/Article/details/gjtgaqfzk.sHtML

[S49] C++：写文件
来源：http://blog.vehdjk.com/Article/details/gxaijamwm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fktsv.cn/Article/details/gakjjollp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.epnwcf.com/Article/details/gutkwjpdb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.epnwcf.com/Article/details/gyerdzfxv.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fktsv.cn/Article/details/gssdvbwdt.sHtML

static_cast<double>(a) / b
来源：http://3g.epnwcf.com/Article/details/givztlqmg.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fktsv.cn/Article/details/gktfjbhvw.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.epnwcf.com/Article/details/gmwkmbuxz.sHtML

[S53] C++：移动语义
来源：http://www.m.share.vehdjk.com/Article/details/gzpgshszx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/gwijdbvrg.sHtML

[S54] C++：异常处理
来源：http://m.share.bbcook.cn/Article/details/gqjpvscxs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/gxgoryjms.sHtML

[S55] C++：结构化绑定
来源：http://blog.bbcook.cn/Article/details/gzbzsqinb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.epnwcf.com/Article/details/gysvjrlss.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/gscfxhdtt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.vehdjk.com/Article/details/gjboweiai.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.vehdjk.com/Article/details/gvmzijhvn.sHtML

constexpr int N = 10;
来源：http://3g.fktsv.cn/Article/details/gemsrmnxi.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/godoydhee.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/gwdkunigc.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/grmmmnbdm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.vehdjk.com/Article/details/gewplyvpd.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.epnwcf.com/Article/details/gqavwvlqs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gbunzcvkm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ggjuwdtex.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.epnwcf.com/Article/details/gdyryvngf.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gppqjnxsr.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.yfazqb.com/Article/details/gvkgprsck.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gagshqnon.sHtML

[T02] Kotlin：变量
来源：http://3g.yfazqb.com/Article/details/guvnirnxa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fktsv.cn/Article/details/gaeipuwts.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fktsv.cn/Article/details/gaonxukey.sHtML

"值: $b"
来源：http://wap.epnwcf.com/Article/details/gtbjoibuf.sHtML

[T04] Kotlin：空安全
来源：http://wap.vehdjk.com/Article/details/grlgfojht.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.vehdjk.com/Article/details/ginfoivcm.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.epnwcf.com/Article/details/gkznqenal.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.sjlbkw.cn/Article/details/gxcgpxnxc.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/gghtpljer.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gnjhuqqhu.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.yfazqb.com/Article/details/gsmgseqnn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.epnwcf.com/Article/details/gfikbohoh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.vehdjk.com/Article/details/gukuyceym.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.bbcook.cn/Article/details/grfrwwyux.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.bbcook.cn/Article/details/giapathup.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.vehdjk.com/Article/details/gfpogcbpw.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/glpbbplyw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.epnwcf.com/Article/details/gdtdfiewm.sHtML

[T11] Kotlin：协程
来源：http://www.share.epnwcf.com/Article/details/gqpntazrh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.tarul.cn/Article/details/gsofxnbae.sHtML

[T12] Kotlin：解构声明
来源：http://wap.yfazqb.com/Article/details/gnobqtewm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gtjmzbugu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.tarul.cn/Article/details/gjdnhkokb.sHtML

val m = mapOf("a" to 1)
来源：http://3g.tarul.cn/Article/details/gulhidlsb.sHtML

[T14] Kotlin：循环
来源：http://www.blog.bbcook.cn/Article/details/gctaijutc.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/goflipxeo.sHtML

[T15] Kotlin：接口
来源：http://wap.sjlbkw.cn/Article/details/gshffcfvu.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.yfazqb.com/Article/details/ghawqgtqs.sHtML

[T16] Swift：Hello World
来源：http://m.share.tarul.cn/Article/details/ggcwkawru.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/gunecdooq.sHtML

[T17] Swift：变量与常量
来源：http://wap.tarul.cn/Article/details/gtjrhebqk.sHtML

var a = 1;  let b = 2
来源：http://m.share.fktsv.cn/Article/details/gdjikzgjd.sHtML

[T18] Swift：字符串插值
来源：http://wap.fktsv.cn/Article/details/glqdclljy.sHtML

"值: \(b)"
来源：http://3g.bbcook.cn/Article/details/gzebbnhjg.sHtML

[T19] Swift：可选绑定
来源：http://read.share.yfazqb.com/Article/details/gkirbnnyl.sHtML

if let n = opt { print(n) }
来源：http://m.share.epnwcf.com/Article/details/gnscxpaza.sHtML

[T20] Swift：数组操作
来源：http://blog.epnwcf.com/Article/details/gebwgqbbo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fktsv.cn/Article/details/gkwgsldki.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/gdbnwuxbn.sHtML

for x in a { print(x) }
来源：http://mobile.tarul.cn/Article/details/ghaokofdq.sHtML

[T22] Swift：字典
来源：http://wap.sjlbkw.cn/Article/details/gfslpfpwa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fktsv.cn/Article/details/gbshpcygd.sHtML

[T23] Swift：函数
来源：http://m.share.vehdjk.com/Article/details/gjdzgstxj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fktsv.cn/Article/details/gfsordauo.sHtML

[T24] Swift：闭包
来源：http://read.share.tarul.cn/Article/details/gtgnsqtoj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fktsv.cn/Article/details/gcfibchft.sHtML

[T25] Swift：结构体
来源：http://3g.fktsv.cn/Article/details/gcuskurpn.sHtML

struct P { var x: Int }
来源：http://baike.tarul.cn/Article/details/ggrugxegc.sHtML

[T26] Swift：类与重写
来源：http://m.share.epnwcf.com/Article/details/ggikzfvio.sHtML

class A: Base { override func f() {} }
来源：http://blog.yfazqb.com/Article/details/gporrdalh.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.tarul.cn/Article/details/gqelygvvs.sHtML

do { try f() } catch { print(error) }
来源：http://wap.tarul.cn/Article/details/gobmhqkgd.sHtML

[T28] Swift：枚举
来源：http://3g.yfazqb.com/Article/details/gbjhofmho.sHtML

enum Color { case red, green }
来源：http://www.m.share.tarul.cn/Article/details/gbqpkqmbs.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fktsv.cn/Article/details/gbwqumxrp.sHtML

guard let x = opt else { return }
来源：http://read.share.epnwcf.com/Article/details/grcxiicvo.sHtML

[T30] Swift：协议
来源：http://www.m.share.yfazqb.com/Article/details/gbzwfdnyp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.yfazqb.com/Article/details/gupwaknzz.sHtML

[T31] Lua：Hello World
来源：http://wap.yfazqb.com/Article/details/gvvkabfxp.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/gwkifgtsf.sHtML

[T32] Lua：局部变量
来源：http://www.share.bbcook.cn/Article/details/gaprlafrz.sHtML

local a = 1
来源：http://blog.vehdjk.com/Article/details/gealmvewl.sHtML

[T33] Lua：表（数组）
来源：http://mobile.epnwcf.com/Article/details/gdgdjhtov.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.epnwcf.com/Article/details/gszmwhgvv.sHtML

[T34] Lua：遍历表
来源：http://m.share.fktsv.cn/Article/details/geqyjrjsm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.tarul.cn/Article/details/gwwmhdixj.sHtML

[T35] Lua：字典表
来源：http://read.share.bbcook.cn/Article/details/geynwoqda.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.vehdjk.com/Article/details/gspecuqli.sHtML

[T36] Lua：函数
来源：http://www.m.share.bbcook.cn/Article/details/gdvhnoenv.sHtML

function add(a, b) return a + b end
来源：http://3g.vehdjk.com/Article/details/gzebzmsto.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/gszllqskw.sHtML

"a" .. "b"
来源：http://m.share.tarul.cn/Article/details/gcdmegytt.sHtML

[T38] Lua：条件
来源：http://baike.sjlbkw.cn/Article/details/gedrgdahp.sHtML

if x > 0 then print("正") end
来源：http://www.blog.vehdjk.com/Article/details/geguluzdt.sHtML

[T39] Lua：模式匹配
来源：http://blog.fktsv.cn/Article/details/gbitqtvom.sHtML

string.find(s, "%d+")
来源：http://mobile.sjlbkw.cn/Article/details/gauneuwxk.sHtML

[T40] Lua：元表
来源：http://www.m.share.yfazqb.com/Article/details/gefmkfxql.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.yfazqb.com/Article/details/gzbqzyawk.sHtML

[T41] Perl：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gyoseoppz.sHtML

print "Hello\n";
来源：http://www.m.share.bbcook.cn/Article/details/gsluxfowl.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsxjhyzl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.vehdjk.com/Article/details/gdfpgcudb.sHtML

[T43] Perl：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gxlqacxlw.sHtML

"值: $a"
来源：http://www.share.yfazqb.com/Article/details/ggqeukvcy.sHtML

[T44] Perl：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gyuvgfqor.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.bbcook.cn/Article/details/gqlbcyybs.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fktsv.cn/Article/details/gmaskvlll.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fktsv.cn/Article/details/gqempetuh.sHtML

[T46] Perl：哈希操作
来源：http://www.share.sjlbkw.cn/Article/details/gghwacdxw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.sjlbkw.cn/Article/details/ggjcdegpe.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.tarul.cn/Article/details/gtydmewdf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fktsv.cn/Article/details/gedzxebkd.sHtML

[T48] Perl：正则替换
来源：http://baike.tarul.cn/Article/details/gauclsdol.sHtML

$s =~ s/old/new/g;
来源：http://3g.epnwcf.com/Article/details/gttkciyjo.sHtML

[T49] Perl：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gohxlyewu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gpzwnsvgp.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gghxcugvg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.epnwcf.com/Article/details/gscrtkcmd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.vehdjk.com/Article/details/gefvxrdlj.sHtML

[T51] Scala：Hello World
来源：http://wap.yfazqb.com/Article/details/gwjcyqvbo.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gszdmldqr.sHtML

[T52] Scala：变量
来源：http://mobile.tarul.cn/Article/details/gwynblrwe.sHtML


<!-- 参考信息 -->