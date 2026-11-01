代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://baike.tarul.cn/Article/details/gqosddvkl.sHtML

[R48] awk 取指定列
来源：http://3g.vehdjk.com/Article/details/gffkxnbrg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gftaofync.sHtML

[R49] awk 带条件
来源：http://www.share.yfazqb.com/Article/details/gmuaqxxmn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.yfazqb.com/Article/details/gvlwjqihe.sHtML

[R50] awk 求和
来源：http://www.blog.sjlbkw.cn/Article/details/gwwiazgsb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gosdamddw.sHtML

[R51] 排序去重取前几
来源：http://m.share.yfazqb.com/Article/details/gkwjzbwvy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.bbcook.cn/Article/details/gqwkkbwbu.sHtML

[R52] 统计行数
来源：http://mobile.bbcook.cn/Article/details/gauwdvxzv.sHtML

wc -l a.txt
来源：http://www.blog.fktsv.cn/Article/details/gezeweofj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.vehdjk.com/Article/details/ggcedjatj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.yfazqb.com/Article/details/gnzrztpww.sHtML

[R54] 比较两个文件
来源：http://baike.bbcook.cn/Article/details/gxpaakigq.sHtML

diff a.txt b.txt
来源：http://m.share.bbcook.cn/Article/details/gzcdlfcvo.sHtML

[R55] 压缩与解压
来源：http://wap.yfazqb.com/Article/details/ghlxwsaon.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.bbcook.cn/Article/details/gnwnvoykx.sHtML

[R56] 远程拷贝
来源：http://baike.epnwcf.com/Article/details/ghttpvyiz.sHtML

scp file user@host:/path/
来源：http://blog.bbcook.cn/Article/details/giqymvpvh.sHtML

[R57] 远程执行命令
来源：http://blog.yfazqb.com/Article/details/gnfbzcajz.sHtML

ssh user@host 'uptime'
来源：http://blog.tarul.cn/Article/details/gdcrjkmtw.sHtML

[R58] 下载文件
来源：http://wap.yfazqb.com/Article/details/gijmhhnmq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.bbcook.cn/Article/details/gxgvwlato.sHtML

[R59] 发 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gzbkchftj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.bbcook.cn/Article/details/gygxhszbt.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gvgbkodpy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.vehdjk.com/Article/details/gljbolenp.sHtML

[R61] 磁盘占用
来源：http://www.blog.yfazqb.com/Article/details/gmlqplqen.sHtML

df -h;  du -sh *
来源：http://mobile.vehdjk.com/Article/details/gxhakzzbk.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/gnbqktetu.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fktsv.cn/Article/details/gksalzscm.sHtML

[R63] 内存与进程
来源：http://mobile.yfazqb.com/Article/details/gtkqxzpzj.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.epnwcf.com/Article/details/gesoucvtb.sHtML

[R64] 结束进程
来源：http://read.share.fktsv.cn/Article/details/goowajsie.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.sjlbkw.cn/Article/details/gddbmsiot.sHtML

[R65] 查看端口占用
来源：http://www.blog.sjlbkw.cn/Article/details/godwohwlj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fktsv.cn/Article/details/gzpzjicbp.sHtML

[R66] 定时任务
来源：http://baike.epnwcf.com/Article/details/glawomgpl.sHtML

crontab -e;  crontab -l
来源：http://www.blog.sjlbkw.cn/Article/details/gjmvtsaxk.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.epnwcf.com/Article/details/gfmbzwkin.sHtML

openssl rand -hex 16
来源：http://www.blog.epnwcf.com/Article/details/gtipiugtq.sHtML

[R68] 计算文件校验值
来源：http://3g.bbcook.cn/Article/details/gdxwucyrn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.tarul.cn/Article/details/gmtznpxqt.sHtML

[R69] 生成随机密码
来源：http://m.share.epnwcf.com/Article/details/gkfyjihlf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fktsv.cn/Article/details/gdpigmplq.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.bbcook.cn/Article/details/ghdzcbhaq.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.tarul.cn/Article/details/gxlyhlkwq.sHtML

[R71] 日期格式化
来源：http://3g.tarul.cn/Article/details/gknuifjwd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/gztdaepwe.sHtML

[R72] 等待端口就绪
来源：http://www.blog.vehdjk.com/Article/details/gzndsjbab.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fktsv.cn/Article/details/grdyjggbb.sHtML

[R73] 分割大日志
来源：http://3g.bbcook.cn/Article/details/gecltvmhl.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/geygrtnvx.sHtML

[R74] 批量重命名
来源：http://www.m.share.tarul.cn/Article/details/gghtjspqu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.tarul.cn/Article/details/giygnrddb.sHtML

[R75] 导出环境变量
来源：http://www.share.epnwcf.com/Article/details/gvksywpfz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.yfazqb.com/Article/details/gyxuszvbb.sHtML

[R76] 使用临时文件
来源：http://read.share.fktsv.cn/Article/details/gmfygwlbm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/gkcghrfls.sHtML

[R77] 读取用户输入
来源：http://mobile.vehdjk.com/Article/details/gccarcqep.sHtML

read -rp "请输入: " ans
来源：http://www.share.fktsv.cn/Article/details/grexkgsuo.sHtML

[R78] 交互式菜单
来源：http://www.share.bbcook.cn/Article/details/gqwiswntd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.sjlbkw.cn/Article/details/gqfbqpukb.sHtML

[R79] 解析命令行选项
来源：http://read.share.sjlbkw.cn/Article/details/gvwryhzrz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.bbcook.cn/Article/details/gztkigzmf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.epnwcf.com/Article/details/gapmfplgj.sHtML

time ./run.sh
来源：http://www.blog.bbcook.cn/Article/details/ggycrgqhx.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gsleureod.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/gkecjyqbk.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ggjepesnh.sHtML

[S01] C：Hello World
来源：http://3g.vehdjk.com/Article/details/gamrayulz.sHtML

#include <stdio.h>
来源：http://www.share.epnwcf.com/Article/details/gpnnqdinf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.sjlbkw.cn/Article/details/gepqjdppf.sHtML

[S02] C：变量与格式化输出
来源：http://wap.vehdjk.com/Article/details/gtcuthgyn.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.yfazqb.com/Article/details/gatvyiypy.sHtML

[S03] C：读入整数
来源：http://m.share.yfazqb.com/Article/details/gaeoyvavu.sHtML

int x; scanf("%d", &x);
来源：http://wap.tarul.cn/Article/details/grpbauclp.sHtML

[S04] C：字符串复制
来源：http://blog.sjlbkw.cn/Article/details/gblphwrkq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gfdnagjwv.sHtML

[S05] C：字符串长度
来源：http://3g.epnwcf.com/Article/details/glsnngitw.sHtML

strlen(s)
来源：http://mobile.yfazqb.com/Article/details/gmfdvsgyy.sHtML

[S06] C：字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/gmkeugdhh.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/gnthlatqu.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/gntqlhltg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fktsv.cn/Article/details/gzrgwppgp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.vehdjk.com/Article/details/gudscddzl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.vehdjk.com/Article/details/ghbfiyoxu.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fktsv.cn/Article/details/gbghbnyux.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.yfazqb.com/Article/details/gkpbaxahe.sHtML

[S10] C：指针与解引用
来源：http://mobile.bbcook.cn/Article/details/ggqtbjzjf.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.sjlbkw.cn/Article/details/gqdnlyxpk.sHtML

[S11] C：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/ghpryvhln.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.epnwcf.com/Article/details/gkxnkteij.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.tarul.cn/Article/details/gqqrruttw.sHtML

fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gabxgvqvj.sHtML

[S12] C：写文件
来源：http://www.blog.tarul.cn/Article/details/gfynjdxhg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fktsv.cn/Article/details/glfzzspgh.sHtML

[S13] C：宏定义
来源：http://wap.yfazqb.com/Article/details/gdxirffnv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.vehdjk.com/Article/details/geeohytsr.sHtML

[S14] C：枚举
来源：http://baike.epnwcf.com/Article/details/gfnjihrdi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/gherhufob.sHtML

[S15] C：类型转换
来源：http://www.share.bbcook.cn/Article/details/gzvvueoyn.sHtML

(double) a / b
来源：http://mobile.bbcook.cn/Article/details/gthxrcwmy.sHtML

[S16] C：位操作置位
来源：http://baike.fktsv.cn/Article/details/gmiwwkkyr.sHtML

x |= (1 << 3);
来源：http://3g.tarul.cn/Article/details/grdnfcpjq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/gjhoibqwq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.bbcook.cn/Article/details/gnwodwtog.sHtML

[S18] C：命令行参数
来源：http://m.share.vehdjk.com/Article/details/gfxpifgcp.sHtML

int main(int argc, char **argv)
来源：http://www.share.bbcook.cn/Article/details/grzhojobd.sHtML

[S19] C：快速排序
来源：http://baike.vehdjk.com/Article/details/gchfdkmji.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gnsrfcunv.sHtML

[S20] C：二分查找
来源：http://www.share.epnwcf.com/Article/details/gfhrxitjk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gjblbnfdz.sHtML

[S21] C：字符类别判断
来源：http://read.share.fktsv.cn/Article/details/glwmjxaid.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.vehdjk.com/Article/details/gdtejtdmy.sHtML

[S22] C：字符串转数字
来源：http://m.share.vehdjk.com/Article/details/glvkhhffs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.yfazqb.com/Article/details/gmuuwwliw.sHtML

[S23] C：随机数
来源：http://3g.epnwcf.com/Article/details/gdzhsquuy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.vehdjk.com/Article/details/gxvgejqry.sHtML

[S24] C：获取本地时间
来源：http://m.share.sjlbkw.cn/Article/details/gvmeqmtwd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.yfazqb.com/Article/details/gmauwhgic.sHtML

[S25] C：内存拷贝
来源：http://www.blog.tarul.cn/Article/details/gfnqjfhjh.sHtML

memcpy(dst, src, n);
来源：http://m.share.bbcook.cn/Article/details/gigkparxk.sHtML

[S26] C：内存清零
来源：http://read.share.sjlbkw.cn/Article/details/gvyyqhuna.sHtML

memset(a, 0, sizeof a);
来源：http://wap.yfazqb.com/Article/details/gxegvuqee.sHtML

[S27] C：定义常量
来源：http://read.share.fktsv.cn/Article/details/gxpxvfdlr.sHtML

const double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/guzjsxebh.sHtML

[S28] C：静态变量
来源：http://3g.epnwcf.com/Article/details/gxmykuqbm.sHtML

static int counter = 0;
来源：http://3g.vehdjk.com/Article/details/geoltfqvl.sHtML

[S29] C：变参函数
来源：http://mobile.yfazqb.com/Article/details/girghnfyj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/gktfcswpx.sHtML

[S30] C：头文件保护
来源：http://blog.fktsv.cn/Article/details/gupropoys.sHtML

#ifndef X_H
来源：http://read.share.bbcook.cn/Article/details/gqrmblnzi.sHtML

#define X_H
来源：http://www.m.share.fktsv.cn/Article/details/guylehoxf.sHtML

#endif
来源：http://www.share.bbcook.cn/Article/details/gairmzajs.sHtML

[S31] C++：Hello World
来源：http://m.share.vehdjk.com/Article/details/gfiqjkoin.sHtML

#include <iostream>
来源：http://read.share.epnwcf.com/Article/details/gigohfrkj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.epnwcf.com/Article/details/gbzyxkals.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gqylucgle.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.vehdjk.com/Article/details/gquejpibe.sHtML

[S33] C++：vector 增删
来源：http://baike.yfazqb.com/Article/details/gslcgxrjm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gunffsysa.sHtML

[S34] C++：遍历 vector
来源：http://m.share.tarul.cn/Article/details/gbffenwiy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fktsv.cn/Article/details/gjfaztozz.sHtML

[S35] C++：map
来源：http://3g.fktsv.cn/Article/details/gqcdroltm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/gsccebxyo.sHtML

[S36] C++：unordered_map
来源：http://www.blog.yfazqb.com/Article/details/gtgyrzaok.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/ggllniang.sHtML

[S37] C++：set
来源：http://mobile.bbcook.cn/Article/details/gmbhwkirg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.epnwcf.com/Article/details/gkzzydjek.sHtML

[S38] C++：排序
来源：http://baike.vehdjk.com/Article/details/gtccupfdu.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.vehdjk.com/Article/details/gevwongfw.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.yfazqb.com/Article/details/gxfbjiaxe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.yfazqb.com/Article/details/ghlbzqfxf.sHtML

[S40] C++：查找元素
来源：http://wap.fktsv.cn/Article/details/giejxbdec.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.vehdjk.com/Article/details/gxfmiijft.sHtML

[S41] C++：类与构造函数
来源：http://baike.fktsv.cn/Article/details/gijgmtcts.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.bbcook.cn/Article/details/gdxwlydlf.sHtML

[S42] C++：继承与虚函数
来源：http://3g.sjlbkw.cn/Article/details/gmcvcfoge.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.tarul.cn/Article/details/gdfzxjirx.sHtML

[S43] C++：智能指针
来源：http://wap.sjlbkw.cn/Article/details/gkbuokzhc.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.yfazqb.com/Article/details/gsssqlyap.sHtML

[S44] C++：引用传参
来源：http://www.blog.tarul.cn/Article/details/gpjzjufjq.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.tarul.cn/Article/details/gycbuuope.sHtML

[S45] C++：lambda
来源：http://wap.fktsv.cn/Article/details/ghsvqhyhv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.tarul.cn/Article/details/gjfmreulx.sHtML

[S46] C++：函数模板
来源：http://www.share.yfazqb.com/Article/details/gpyvljvjc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fktsv.cn/Article/details/gidlikxpc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fktsv.cn/Article/details/greberrsf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.tarul.cn/Article/details/gegbuoyka.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gzalfpdvl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.epnwcf.com/Article/details/gxupddrma.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.vehdjk.com/Article/details/gqrjecrvo.sHtML

[S49] C++：写文件
来源：http://www.share.vehdjk.com/Article/details/giorvuanf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.epnwcf.com/Article/details/gohmegovc.sHtML

[S50] C++：格式化数字
来源：http://m.share.bbcook.cn/Article/details/gbhaohqsy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.vehdjk.com/Article/details/gnqzzqcez.sHtML

[S51] C++：显式类型转换
来源：http://read.share.vehdjk.com/Article/details/gnwjojevi.sHtML

static_cast<double>(a) / b
来源：http://3g.bbcook.cn/Article/details/gekhwiahy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fktsv.cn/Article/details/gpdqnsfbi.sHtML

int size() const noexcept { return n_; }
来源：http://baike.tarul.cn/Article/details/gwcewipxc.sHtML

[S53] C++：移动语义
来源：http://m.share.fktsv.cn/Article/details/gjschtbhr.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/glpfsacai.sHtML

[S54] C++：异常处理
来源：http://read.share.tarul.cn/Article/details/gytboxgiz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.sjlbkw.cn/Article/details/gutklpjcu.sHtML

[S55] C++：结构化绑定
来源：http://wap.vehdjk.com/Article/details/gmmbjzrsn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.tarul.cn/Article/details/gedhehggq.sHtML

[S56] C++：optional
来源：http://wap.bbcook.cn/Article/details/guemcmymy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.vehdjk.com/Article/details/gqwxgrgvg.sHtML

[S57] C++：编译期常量
来源：http://m.share.sjlbkw.cn/Article/details/gxqihmlmw.sHtML

constexpr int N = 10;
来源：http://read.share.tarul.cn/Article/details/gaapzumow.sHtML

[S58] C++：命名空间
来源：http://www.m.share.bbcook.cn/Article/details/gpcejvsuq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.bbcook.cn/Article/details/gttawsrhq.sHtML

[S59] C++：静态断言
来源：http://www.blog.tarul.cn/Article/details/gudxqvamf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gminrutqb.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.yfazqb.com/Article/details/gbkezrewf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gvzdljyip.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gcbmqmtfw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.vehdjk.com/Article/details/gdspjeepu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gapeobmap.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gpcxnxgne.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gququkxmz.sHtML

[T02] Kotlin：变量
来源：http://www.share.epnwcf.com/Article/details/ghqqpgray.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.epnwcf.com/Article/details/gyehxuqmd.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.epnwcf.com/Article/details/gvhabkawv.sHtML

"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/gimtvzyff.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.tarul.cn/Article/details/gofqeyije.sHtML

val n: String? = null;  n?.length
来源：http://mobile.sjlbkw.cn/Article/details/gelorfmqi.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.sjlbkw.cn/Article/details/glkciblld.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.bbcook.cn/Article/details/gqcnbsfxu.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.tarul.cn/Article/details/gucdhonxt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.bbcook.cn/Article/details/gewvwrudn.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.tarul.cn/Article/details/gyfaxyolt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.vehdjk.com/Article/details/goqlyuslj.sHtML

[T08] Kotlin：数据类
来源：http://mobile.vehdjk.com/Article/details/gqafymefx.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.sjlbkw.cn/Article/details/geyeirnqr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.sjlbkw.cn/Article/details/gtvohknlp.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.bbcook.cn/Article/details/gvtbfidno.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gojzebmkx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.bbcook.cn/Article/details/gdybuluvv.sHtML

[T11] Kotlin：协程
来源：http://baike.tarul.cn/Article/details/goukkkgtv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.bbcook.cn/Article/details/gsbcvrnap.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.vehdjk.com/Article/details/gktgddfge.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gorxdkktz.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.epnwcf.com/Article/details/gtvfvyfes.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.tarul.cn/Article/details/gridcssna.sHtML

[T14] Kotlin：循环
来源：http://baike.epnwcf.com/Article/details/gnqbvohhh.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gbvfuinwf.sHtML

[T15] Kotlin：接口
来源：http://mobile.fktsv.cn/Article/details/gsvmgyily.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gelruymnu.sHtML

[T16] Swift：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/giodtxenx.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gqbbouipz.sHtML

[T17] Swift：变量与常量
来源：http://read.share.yfazqb.com/Article/details/gbxtyqmjf.sHtML

var a = 1;  let b = 2
来源：http://baike.bbcook.cn/Article/details/gimqbjtgx.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/ghcyidyjy.sHtML

"值: \(b)"
来源：http://m.share.tarul.cn/Article/details/gabzjpmsp.sHtML

[T19] Swift：可选绑定
来源：http://m.share.yfazqb.com/Article/details/gyjqeqhdj.sHtML

if let n = opt { print(n) }
来源：http://wap.bbcook.cn/Article/details/gincwbila.sHtML

[T20] Swift：数组操作
来源：http://baike.yfazqb.com/Article/details/goexkwvcs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.sjlbkw.cn/Article/details/gxuwqckvm.sHtML

[T21] Swift：遍历
来源：http://baike.epnwcf.com/Article/details/gkkzkhqjj.sHtML

for x in a { print(x) }
来源：http://www.share.vehdjk.com/Article/details/gcuygcnwv.sHtML

[T22] Swift：字典
来源：http://www.share.sjlbkw.cn/Article/details/gjadvjfqd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gskbnecmj.sHtML

[T23] Swift：函数
来源：http://www.blog.bbcook.cn/Article/details/gkkwujppx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gclalbhaz.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gmijpxwxa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/ghlczwhie.sHtML

[T25] Swift：结构体
来源：http://www.share.sjlbkw.cn/Article/details/gjkbzdpyf.sHtML

struct P { var x: Int }
来源：http://mobile.sjlbkw.cn/Article/details/grwpcgltf.sHtML

[T26] Swift：类与重写
来源：http://3g.yfazqb.com/Article/details/gkqefvaml.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.bbcook.cn/Article/details/gizctrijh.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fktsv.cn/Article/details/gnreeqsct.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.tarul.cn/Article/details/gksjdmlkd.sHtML

[T28] Swift：枚举
来源：http://read.share.fktsv.cn/Article/details/gowofonjj.sHtML

enum Color { case red, green }
来源：http://m.share.tarul.cn/Article/details/gopbrodae.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.yfazqb.com/Article/details/ggruatfha.sHtML

guard let x = opt else { return }
来源：http://baike.fktsv.cn/Article/details/gsmvcjcft.sHtML

[T30] Swift：协议
来源：http://www.blog.bbcook.cn/Article/details/gnjmxumpi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.epnwcf.com/Article/details/gshswwrud.sHtML

[T31] Lua：Hello World
来源：http://www.share.tarul.cn/Article/details/ghsvvvsds.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/gbohfcokb.sHtML

[T32] Lua：局部变量
来源：http://read.share.tarul.cn/Article/details/gpaiyqtev.sHtML

local a = 1
来源：http://mobile.sjlbkw.cn/Article/details/gyymercsg.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.yfazqb.com/Article/details/grhmyehii.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fktsv.cn/Article/details/gkaajpdmk.sHtML

[T34] Lua：遍历表
来源：http://baike.vehdjk.com/Article/details/gerlnjvdr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.tarul.cn/Article/details/gbitjbffr.sHtML

[T35] Lua：字典表
来源：http://mobile.fktsv.cn/Article/details/gtebecmge.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.vehdjk.com/Article/details/gsryjwchu.sHtML

[T36] Lua：函数
来源：http://m.share.fktsv.cn/Article/details/gmmxhydlq.sHtML

function add(a, b) return a + b end
来源：http://3g.sjlbkw.cn/Article/details/gnqkmhjui.sHtML

[T37] Lua：字符串拼接
来源：http://wap.epnwcf.com/Article/details/ghelaptaw.sHtML

"a" .. "b"
来源：http://baike.epnwcf.com/Article/details/gblqwqqqz.sHtML

[T38] Lua：条件
来源：http://blog.vehdjk.com/Article/details/gupmcwmol.sHtML

if x > 0 then print("正") end
来源：http://read.share.tarul.cn/Article/details/geoxmlnok.sHtML

[T39] Lua：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gvkerxmdy.sHtML

string.find(s, "%d+")
来源：http://mobile.vehdjk.com/Article/details/guuonlcdl.sHtML

[T40] Lua：元表
来源：http://m.share.fktsv.cn/Article/details/ghbjefmif.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.bbcook.cn/Article/details/gmjbvkxsm.sHtML

[T41] Perl：Hello World
来源：http://blog.vehdjk.com/Article/details/gjswrcjhc.sHtML

print "Hello\n";
来源：http://m.share.epnwcf.com/Article/details/gxoaxqnfl.sHtML

[T42] Perl：变量类型
来源：http://3g.fktsv.cn/Article/details/gaziuuraq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.tarul.cn/Article/details/gphbyvjzd.sHtML

[T43] Perl：字符串插值
来源：http://wap.bbcook.cn/Article/details/ggsrvdqum.sHtML

"值: $a"
来源：http://mobile.sjlbkw.cn/Article/details/gfuxbydxm.sHtML

[T44] Perl：条件
来源：http://blog.fktsv.cn/Article/details/gulxverpz.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fktsv.cn/Article/details/genvfqpgt.sHtML

[T45] Perl：数组遍历
来源：http://blog.bbcook.cn/Article/details/gigzugmzf.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.tarul.cn/Article/details/gykqeuhvn.sHtML

[T46] Perl：哈希操作
来源：http://3g.fktsv.cn/Article/details/ghnsgaxmv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.epnwcf.com/Article/details/gocwetqbu.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.bbcook.cn/Article/details/gytkcydpv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.yfazqb.com/Article/details/gcxrydumd.sHtML

[T48] Perl：正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gdsiipdpd.sHtML

$s =~ s/old/new/g;
来源：http://m.share.tarul.cn/Article/details/gebytrkws.sHtML

[T49] Perl：函数
来源：http://www.blog.epnwcf.com/Article/details/gpyjuuvdd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/goahkjxbp.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gzonmbevq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.tarul.cn/Article/details/gydoerlmf.sHtML


<!-- 参考信息 -->