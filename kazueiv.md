代发 wailian999

find . -name "*.log" -type f
来源：http://www.blog.tarul.cn/Article/details/gahqtvqnn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.vehdjk.com/Article/details/gokstkqbf.sHtML

find . -mtime -7 -type f
来源：http://www.blog.tarul.cn/Article/details/gnreassnm.sHtML

[R45] 批量删除
来源：http://read.share.sjlbkw.cn/Article/details/ggopxvcgj.sHtML

find . -name "*.tmp" -delete
来源：http://blog.yfazqb.com/Article/details/gbkekkcxm.sHtML

[R46] 递归替换文件内容
来源：http://3g.tarul.cn/Article/details/gqghtgbcm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.epnwcf.com/Article/details/grmhnziin.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/gsahmbliy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gmrluudqx.sHtML

[R48] awk 取指定列
来源：http://baike.yfazqb.com/Article/details/gjekimhpp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gkstycymc.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/gearxbtfh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.vehdjk.com/Article/details/gbesjxvav.sHtML

[R50] awk 求和
来源：http://mobile.bbcook.cn/Article/details/gwthqvlkx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.yfazqb.com/Article/details/gaqtmazzl.sHtML

[R51] 排序去重取前几
来源：http://read.share.fktsv.cn/Article/details/gxjovurwy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/gjbwsvogg.sHtML

[R52] 统计行数
来源：http://mobile.vehdjk.com/Article/details/giuacmxyq.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/gadjhysvj.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.sjlbkw.cn/Article/details/gzydhvdfh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.vehdjk.com/Article/details/gsntbwccx.sHtML

[R54] 比较两个文件
来源：http://m.share.bbcook.cn/Article/details/gqrcvmfwh.sHtML

diff a.txt b.txt
来源：http://3g.fktsv.cn/Article/details/gblkzjwno.sHtML

[R55] 压缩与解压
来源：http://3g.fktsv.cn/Article/details/gkvnyxawy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fktsv.cn/Article/details/gcwlvrpvy.sHtML

[R56] 远程拷贝
来源：http://read.share.bbcook.cn/Article/details/gvanseaxj.sHtML

scp file user@host:/path/
来源：http://m.share.yfazqb.com/Article/details/gkabhwvtm.sHtML

[R57] 远程执行命令
来源：http://mobile.vehdjk.com/Article/details/gypbokknc.sHtML

ssh user@host 'uptime'
来源：http://wap.epnwcf.com/Article/details/gmyorbjwg.sHtML

[R58] 下载文件
来源：http://www.m.share.epnwcf.com/Article/details/gbofapibp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.sjlbkw.cn/Article/details/ghwzvgifl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/gxxofmjqs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/girrkzbkb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/gajlbgknb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.vehdjk.com/Article/details/gzvltwxfp.sHtML

[R61] 磁盘占用
来源：http://3g.bbcook.cn/Article/details/gfnvlipra.sHtML

df -h;  du -sh *
来源：http://read.share.epnwcf.com/Article/details/gogudtgbl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.epnwcf.com/Article/details/gpyzpdrmf.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.vehdjk.com/Article/details/ggemmlnfg.sHtML

[R63] 内存与进程
来源：http://mobile.bbcook.cn/Article/details/gceanmerg.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.vehdjk.com/Article/details/gflvsbpdv.sHtML

[R64] 结束进程
来源：http://baike.vehdjk.com/Article/details/gznjgajpi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/gvvtalqbb.sHtML

[R65] 查看端口占用
来源：http://www.share.fktsv.cn/Article/details/gnciidtma.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.bbcook.cn/Article/details/gkfciileh.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/ghkrnqduy.sHtML

crontab -e;  crontab -l
来源：http://m.share.fktsv.cn/Article/details/gsbugospx.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.vehdjk.com/Article/details/gbtzoitsq.sHtML

openssl rand -hex 16
来源：http://baike.vehdjk.com/Article/details/gwceucrls.sHtML

[R68] 计算文件校验值
来源：http://3g.yfazqb.com/Article/details/gqazsfeva.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.yfazqb.com/Article/details/gjpyxawau.sHtML

[R69] 生成随机密码
来源：http://mobile.vehdjk.com/Article/details/getfgpdrb.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fktsv.cn/Article/details/gciclhyjd.sHtML

[R70] 时间戳与互转
来源：http://read.share.bbcook.cn/Article/details/grpdnehvp.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fktsv.cn/Article/details/grsudibqg.sHtML

[R71] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/giapdzcuh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.sjlbkw.cn/Article/details/gjpwxhpnw.sHtML

[R72] 等待端口就绪
来源：http://wap.sjlbkw.cn/Article/details/ghlwuhgqr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/gzgnuprkq.sHtML

[R73] 分割大日志
来源：http://read.share.yfazqb.com/Article/details/gbqetocze.sHtML

split -l 1000 big.log part_
来源：http://mobile.bbcook.cn/Article/details/gwqjkfkuw.sHtML

[R74] 批量重命名
来源：http://3g.epnwcf.com/Article/details/gtscrwwii.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fktsv.cn/Article/details/giiawnmzy.sHtML

[R75] 导出环境变量
来源：http://www.blog.yfazqb.com/Article/details/gusrwkxxu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.yfazqb.com/Article/details/gaegyehhd.sHtML

[R76] 使用临时文件
来源：http://blog.bbcook.cn/Article/details/gudyearal.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gexcwwbkx.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/gccrzggyl.sHtML

read -rp "请输入: " ans
来源：http://read.share.epnwcf.com/Article/details/gucqnpoly.sHtML

[R78] 交互式菜单
来源：http://mobile.vehdjk.com/Article/details/gnwcuqolw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.tarul.cn/Article/details/gxwobuazl.sHtML

[R79] 解析命令行选项
来源：http://mobile.vehdjk.com/Article/details/gnzwzvefr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fktsv.cn/Article/details/gxyvrlmig.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/gpsgfjewg.sHtML

time ./run.sh
来源：http://www.blog.vehdjk.com/Article/details/gzqcrsqup.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gduvswany.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/gtrzzrwei.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gsqutptfo.sHtML

[S01] C：Hello World
来源：http://mobile.tarul.cn/Article/details/gtcavjlcf.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/goodvnwhz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/gvbtxarja.sHtML

[S02] C：变量与格式化输出
来源：http://wap.tarul.cn/Article/details/gufulqqtz.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fktsv.cn/Article/details/gonfbxcle.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gyvjhsdgm.sHtML

int x; scanf("%d", &x);
来源：http://3g.tarul.cn/Article/details/gyrwooaay.sHtML

[S04] C：字符串复制
来源：http://www.m.share.epnwcf.com/Article/details/gunzkmwta.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.epnwcf.com/Article/details/gisslgsen.sHtML

[S05] C：字符串长度
来源：http://mobile.tarul.cn/Article/details/gpbnaoezj.sHtML

strlen(s)
来源：http://m.share.epnwcf.com/Article/details/gkwyjwslx.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/gezkwfbjt.sHtML

strcmp(a, b) == 0
来源：http://blog.vehdjk.com/Article/details/gyjsuwjuy.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fktsv.cn/Article/details/goevzbirl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.yfazqb.com/Article/details/gthbnaije.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.tarul.cn/Article/details/girepeabc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.epnwcf.com/Article/details/gboblsdzy.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/gctlextkx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.tarul.cn/Article/details/gxnryvvow.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/gdinwoniz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fktsv.cn/Article/details/gbadywuoy.sHtML

[S11] C：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gwekcegqq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.sjlbkw.cn/Article/details/goddezarf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fktsv.cn/Article/details/gdhsosese.sHtML

fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gzbanzyrl.sHtML

[S12] C：写文件
来源：http://baike.tarul.cn/Article/details/grkauhabn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.vehdjk.com/Article/details/gqayszylt.sHtML

[S13] C：宏定义
来源：http://m.share.epnwcf.com/Article/details/ghsqmpffn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.vehdjk.com/Article/details/gqvgiymgv.sHtML

[S14] C：枚举
来源：http://www.blog.yfazqb.com/Article/details/gtyiossio.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.sjlbkw.cn/Article/details/guqnpqgir.sHtML

[S15] C：类型转换
来源：http://wap.yfazqb.com/Article/details/glyuegice.sHtML

(double) a / b
来源：http://www.m.share.vehdjk.com/Article/details/gjkohrqyt.sHtML

[S16] C：位操作置位
来源：http://baike.fktsv.cn/Article/details/gknnhnqnr.sHtML

x |= (1 << 3);
来源：http://www.m.share.epnwcf.com/Article/details/gtlzyyqtk.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/glbanocvl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.sjlbkw.cn/Article/details/gpnrschgp.sHtML

[S18] C：命令行参数
来源：http://3g.epnwcf.com/Article/details/gztewrcya.sHtML

int main(int argc, char **argv)
来源：http://baike.epnwcf.com/Article/details/gmutivqua.sHtML

[S19] C：快速排序
来源：http://blog.yfazqb.com/Article/details/gthbjhquw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/gveceiesa.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/gvatplwnc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/gshlkmvsn.sHtML

[S21] C：字符类别判断
来源：http://wap.fktsv.cn/Article/details/gixgqwqso.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/ghuwyjqcq.sHtML

[S22] C：字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gafbevocx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.yfazqb.com/Article/details/ghjbccjvu.sHtML

[S23] C：随机数
来源：http://3g.yfazqb.com/Article/details/gtkboxjzb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.yfazqb.com/Article/details/goqkzlchc.sHtML

[S24] C：获取本地时间
来源：http://baike.bbcook.cn/Article/details/gexyopvoe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.epnwcf.com/Article/details/gtjjsspoq.sHtML

[S25] C：内存拷贝
来源：http://blog.yfazqb.com/Article/details/gzgmxrprc.sHtML

memcpy(dst, src, n);
来源：http://3g.bbcook.cn/Article/details/gjrdhpmpe.sHtML

[S26] C：内存清零
来源：http://m.share.fktsv.cn/Article/details/gqevdpmrd.sHtML

memset(a, 0, sizeof a);
来源：http://wap.yfazqb.com/Article/details/gknrordee.sHtML

[S27] C：定义常量
来源：http://m.share.yfazqb.com/Article/details/gsvdvdnbi.sHtML

const double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gyrvkeoxr.sHtML

[S28] C：静态变量
来源：http://www.share.tarul.cn/Article/details/gqfsvpojk.sHtML

static int counter = 0;
来源：http://blog.sjlbkw.cn/Article/details/gcijvnvwx.sHtML

[S29] C：变参函数
来源：http://mobile.epnwcf.com/Article/details/gwonchvtc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.vehdjk.com/Article/details/gsvjmkkba.sHtML

[S30] C：头文件保护
来源：http://www.share.epnwcf.com/Article/details/gbfbontff.sHtML

#ifndef X_H
来源：http://read.share.sjlbkw.cn/Article/details/goqntndel.sHtML

#define X_H
来源：http://3g.yfazqb.com/Article/details/gjdpvwvod.sHtML

#endif
来源：http://www.m.share.sjlbkw.cn/Article/details/gpulaxvai.sHtML

[S31] C++：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gjjvfyqsj.sHtML

#include <iostream>
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgevblmu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/goqjwhrbx.sHtML

[S32] C++：字符串
来源：http://3g.yfazqb.com/Article/details/gruhxprwa.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.epnwcf.com/Article/details/gfhxyusjv.sHtML

[S33] C++：vector 增删
来源：http://mobile.vehdjk.com/Article/details/ggpyohoxu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gscixoktr.sHtML

[S34] C++：遍历 vector
来源：http://read.share.yfazqb.com/Article/details/gazvgyztq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.epnwcf.com/Article/details/gefzsodzh.sHtML

[S35] C++：map
来源：http://www.share.vehdjk.com/Article/details/gswummhyd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/ggrapvplx.sHtML

[S36] C++：unordered_map
来源：http://blog.bbcook.cn/Article/details/gcsrxnuuc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/gjpgppnpc.sHtML

[S37] C++：set
来源：http://read.share.bbcook.cn/Article/details/gliwqdeft.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.vehdjk.com/Article/details/ghavamwts.sHtML

[S38] C++：排序
来源：http://www.blog.tarul.cn/Article/details/gbvinwozq.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.epnwcf.com/Article/details/gipllypie.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.bbcook.cn/Article/details/gxkiyyqdw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/gnqsrwelg.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/glfckszbq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fktsv.cn/Article/details/gkcgqndnc.sHtML

[S41] C++：类与构造函数
来源：http://www.share.tarul.cn/Article/details/gayzrqqru.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.vehdjk.com/Article/details/gbkzutsqc.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.epnwcf.com/Article/details/godmrojir.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.yfazqb.com/Article/details/gysmwxxcz.sHtML

[S43] C++：智能指针
来源：http://blog.tarul.cn/Article/details/gdvtfrdnx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.yfazqb.com/Article/details/gyevhnvqp.sHtML

[S44] C++：引用传参
来源：http://m.share.fktsv.cn/Article/details/gjjiiwpqz.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/gsjywgyhb.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/gcqevcdib.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfkcmdqk.sHtML

[S46] C++：函数模板
来源：http://m.share.vehdjk.com/Article/details/gqeghtewp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.vehdjk.com/Article/details/gpcjeizqp.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.bbcook.cn/Article/details/gtaezpbip.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.sjlbkw.cn/Article/details/gycsclvvd.sHtML

[S48] C++：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gurggrdjj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.tarul.cn/Article/details/gkabtzvmj.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.vehdjk.com/Article/details/gwgbqtbbq.sHtML

[S49] C++：写文件
来源：http://wap.fktsv.cn/Article/details/gtzbqjgph.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/gvhyklwys.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/gnmurjqwd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.tarul.cn/Article/details/gkkllnxqm.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.bbcook.cn/Article/details/gqipghlyh.sHtML

static_cast<double>(a) / b
来源：http://wap.epnwcf.com/Article/details/gusascjgm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/gtsgryvtx.sHtML

int size() const noexcept { return n_; }
来源：http://3g.sjlbkw.cn/Article/details/gfgwklgjg.sHtML

[S53] C++：移动语义
来源：http://m.share.fktsv.cn/Article/details/ggiorfgzw.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.sjlbkw.cn/Article/details/gmlafmxci.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/ggcljtnmj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.sjlbkw.cn/Article/details/goxctaret.sHtML

[S55] C++：结构化绑定
来源：http://blog.tarul.cn/Article/details/gdoicnbxp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gqwoaxduj.sHtML

[S56] C++：optional
来源：http://blog.bbcook.cn/Article/details/gnvrtpfve.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/goevrihpp.sHtML

[S57] C++：编译期常量
来源：http://3g.tarul.cn/Article/details/gmburxmxw.sHtML

constexpr int N = 10;
来源：http://wap.vehdjk.com/Article/details/gdjkofnpw.sHtML

[S58] C++：命名空间
来源：http://m.share.bbcook.cn/Article/details/gahzprdnp.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/gwcrxyqin.sHtML

[S59] C++：静态断言
来源：http://3g.tarul.cn/Article/details/glpicmkja.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.sjlbkw.cn/Article/details/glxuvfowy.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.yfazqb.com/Article/details/gfrsokbqr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gattvxguo.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmioselth.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.bbcook.cn/Article/details/gnsynfbsc.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gdjnlzutz.sHtML

[T01] Kotlin：Hello World
来源：http://baike.tarul.cn/Article/details/gjpkhqqux.sHtML

println("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gumvgfinl.sHtML

[T02] Kotlin：变量
来源：http://mobile.yfazqb.com/Article/details/gndwezffg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.tarul.cn/Article/details/gtbnywdie.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.epnwcf.com/Article/details/gdkvxwgmh.sHtML

"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/gxhaygzaw.sHtML

[T04] Kotlin：空安全
来源：http://blog.yfazqb.com/Article/details/gwslhuxnc.sHtML

val n: String? = null;  n?.length
来源：http://wap.fktsv.cn/Article/details/gwacidqyi.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fktsv.cn/Article/details/gppqijqlk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.yfazqb.com/Article/details/gnnoigfxs.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fktsv.cn/Article/details/guugxeubv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gyzoiuykn.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fktsv.cn/Article/details/ghqdhnhds.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.epnwcf.com/Article/details/gcnhzlvda.sHtML

[T08] Kotlin：数据类
来源：http://read.share.epnwcf.com/Article/details/gtwblypqy.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.yfazqb.com/Article/details/gdqgozszk.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.sjlbkw.cn/Article/details/gkiloieco.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.vehdjk.com/Article/details/gxzwzesow.sHtML

[T10] Kotlin：默认参数
来源：http://3g.epnwcf.com/Article/details/gjkbteeth.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.yfazqb.com/Article/details/geoaypadk.sHtML

[T11] Kotlin：协程
来源：http://www.blog.vehdjk.com/Article/details/greyikjqk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.epnwcf.com/Article/details/gvqlvjbts.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.sjlbkw.cn/Article/details/gjfridvdc.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gzhdvierh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.yfazqb.com/Article/details/gnsyjqdmi.sHtML

val m = mapOf("a" to 1)
来源：http://baike.tarul.cn/Article/details/gxvkbejkc.sHtML

[T14] Kotlin：循环
来源：http://m.share.vehdjk.com/Article/details/guouccmru.sHtML

for (i in 1..10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gmlratzhh.sHtML

[T15] Kotlin：接口
来源：http://baike.tarul.cn/Article/details/guwkykwiz.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.yfazqb.com/Article/details/gsxnbspdj.sHtML

[T16] Swift：Hello World
来源：http://baike.tarul.cn/Article/details/gpnwycnhi.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/gjiflcjkn.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fktsv.cn/Article/details/gzpljinqp.sHtML

var a = 1;  let b = 2
来源：http://3g.vehdjk.com/Article/details/gmfhisefe.sHtML

[T18] Swift：字符串插值
来源：http://baike.vehdjk.com/Article/details/ggmjerecd.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/ghssyxqfg.sHtML

[T19] Swift：可选绑定
来源：http://m.share.vehdjk.com/Article/details/gaxpxmmdb.sHtML

if let n = opt { print(n) }
来源：http://blog.vehdjk.com/Article/details/gbrnddzcf.sHtML

[T20] Swift：数组操作
来源：http://3g.vehdjk.com/Article/details/grunmfjyr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.tarul.cn/Article/details/gbzrzgixe.sHtML

[T21] Swift：遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjgznwmi.sHtML

for x in a { print(x) }
来源：http://baike.fktsv.cn/Article/details/gpbsbxkbh.sHtML

[T22] Swift：字典
来源：http://www.share.fktsv.cn/Article/details/gsimpgipj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.yfazqb.com/Article/details/gmnwgfidx.sHtML

[T23] Swift：函数
来源：http://read.share.sjlbkw.cn/Article/details/gacxkipjw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.tarul.cn/Article/details/gownqnwoe.sHtML

[T24] Swift：闭包
来源：http://3g.bbcook.cn/Article/details/gourgtpni.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gpwhklfnn.sHtML

[T25] Swift：结构体
来源：http://wap.vehdjk.com/Article/details/gkeczxlyp.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/gmiellurl.sHtML

[T26] Swift：类与重写
来源：http://read.share.tarul.cn/Article/details/gifpogmbj.sHtML

class A: Base { override func f() {} }
来源：http://read.share.yfazqb.com/Article/details/gepirngfq.sHtML

[T27] Swift：错误处理
来源：http://read.share.tarul.cn/Article/details/gdjenceiu.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fktsv.cn/Article/details/gvqptpdqd.sHtML

[T28] Swift：枚举
来源：http://read.share.sjlbkw.cn/Article/details/ghsnhihkw.sHtML

enum Color { case red, green }
来源：http://read.share.vehdjk.com/Article/details/gvkjlpztf.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fktsv.cn/Article/details/gpalhkkqv.sHtML

guard let x = opt else { return }
来源：http://mobile.epnwcf.com/Article/details/geyipsysu.sHtML

[T30] Swift：协议
来源：http://www.share.yfazqb.com/Article/details/gjzjtbquc.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fktsv.cn/Article/details/gkaludzmg.sHtML

[T31] Lua：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gqpvkzbzn.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gatkvljff.sHtML

[T32] Lua：局部变量
来源：http://www.share.epnwcf.com/Article/details/gqkvhvsis.sHtML

local a = 1
来源：http://wap.epnwcf.com/Article/details/gssaymxkb.sHtML

[T33] Lua：表（数组）
来源：http://wap.vehdjk.com/Article/details/gqhtmxggr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.epnwcf.com/Article/details/ghplbaskz.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.bbcook.cn/Article/details/gbjfkefqz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.epnwcf.com/Article/details/gqipkzrwc.sHtML

[T35] Lua：字典表
来源：http://mobile.epnwcf.com/Article/details/ggbdvmpnq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.vehdjk.com/Article/details/grkouivzf.sHtML

[T36] Lua：函数
来源：http://blog.yfazqb.com/Article/details/ggiqmisdr.sHtML

function add(a, b) return a + b end
来源：http://www.blog.sjlbkw.cn/Article/details/gnmdwthog.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gmpzjdioh.sHtML

"a" .. "b"
来源：http://blog.bbcook.cn/Article/details/gqdqawvtd.sHtML

[T38] Lua：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gqyvvqkqo.sHtML

if x > 0 then print("正") end
来源：http://baike.yfazqb.com/Article/details/gaaudnbpv.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gigzvzjuc.sHtML

string.find(s, "%d+")
来源：http://www.m.share.bbcook.cn/Article/details/gzyyxjdbl.sHtML

[T40] Lua：元表
来源：http://read.share.bbcook.cn/Article/details/gdvggaene.sHtML

setmetatable({}, { __index = base })
来源：http://baike.bbcook.cn/Article/details/gqhotctog.sHtML

[T41] Perl：Hello World
来源：http://read.share.fktsv.cn/Article/details/gqujjmccy.sHtML

print "Hello\n";
来源：http://www.share.epnwcf.com/Article/details/gpwjkveax.sHtML

[T42] Perl：变量类型
来源：http://mobile.yfazqb.com/Article/details/gnqfjqlyj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.tarul.cn/Article/details/gmzpygdzy.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/grpuvppjq.sHtML

"值: $a"
来源：http://blog.tarul.cn/Article/details/gwewecfvc.sHtML

[T44] Perl：条件
来源：http://www.share.vehdjk.com/Article/details/ghzqyzkih.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/gvpbbsure.sHtML

[T45] Perl：数组遍历
来源：http://3g.yfazqb.com/Article/details/gpjihukbz.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.sjlbkw.cn/Article/details/gskbydfjc.sHtML

[T46] Perl：哈希操作
来源：http://wap.bbcook.cn/Article/details/gmfumlade.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmlxwkiuf.sHtML


<!-- 参考信息 -->