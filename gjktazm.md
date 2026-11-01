代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.yfazqb.com/Article/details/gmzouhpks.sHtML

[R52] 统计行数
来源：http://3g.tarul.cn/Article/details/gfyrmqmoq.sHtML

wc -l a.txt
来源：http://3g.tarul.cn/Article/details/gapnivdua.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.yfazqb.com/Article/details/gxwedfkad.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gazrihpdq.sHtML

[R54] 比较两个文件
来源：http://wap.tarul.cn/Article/details/gokkhexoh.sHtML

diff a.txt b.txt
来源：http://www.blog.tarul.cn/Article/details/gwvmmdkte.sHtML

[R55] 压缩与解压
来源：http://www.share.yfazqb.com/Article/details/gqaqnmasm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.sjlbkw.cn/Article/details/gztfzpojw.sHtML

[R56] 远程拷贝
来源：http://m.share.epnwcf.com/Article/details/ggnhjfcve.sHtML

scp file user@host:/path/
来源：http://baike.epnwcf.com/Article/details/gcjqywfpp.sHtML

[R57] 远程执行命令
来源：http://baike.epnwcf.com/Article/details/gisvurosl.sHtML

ssh user@host 'uptime'
来源：http://blog.bbcook.cn/Article/details/ggtujegyj.sHtML

[R58] 下载文件
来源：http://www.m.share.yfazqb.com/Article/details/gqgmzywbh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.epnwcf.com/Article/details/ghehcjimd.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/gyhwmxkje.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.epnwcf.com/Article/details/gijhegxzk.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gydriqyyq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.tarul.cn/Article/details/gxajfjmsw.sHtML

[R61] 磁盘占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkiqtfko.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/gxaxzbojh.sHtML

[R62] 找最占空间的文件
来源：http://blog.bbcook.cn/Article/details/gdetnvqhg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/gwovkjhkw.sHtML

[R63] 内存与进程
来源：http://mobile.bbcook.cn/Article/details/gspazvqtw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fktsv.cn/Article/details/giilcdxco.sHtML

[R64] 结束进程
来源：http://blog.tarul.cn/Article/details/glijybane.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.tarul.cn/Article/details/grwfxqkdo.sHtML

[R65] 查看端口占用
来源：http://www.share.bbcook.cn/Article/details/gxlzpczfy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fktsv.cn/Article/details/gctscnita.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/ggpbpwlyz.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/gwksceubq.sHtML

[R67] 生成随机十六进制串
来源：http://baike.sjlbkw.cn/Article/details/gotznrpmz.sHtML

openssl rand -hex 16
来源：http://3g.bbcook.cn/Article/details/gbxwdnswo.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.sjlbkw.cn/Article/details/gixhqjpee.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gljtxxiro.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/giwggdfjb.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.epnwcf.com/Article/details/gelzempsr.sHtML

[R70] 时间戳与互转
来源：http://www.share.tarul.cn/Article/details/gnhopqbwj.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.sjlbkw.cn/Article/details/gglmlvotn.sHtML

[R71] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gymszhitg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.yfazqb.com/Article/details/gcvrnmbsf.sHtML

[R72] 等待端口就绪
来源：http://blog.yfazqb.com/Article/details/gwecprgwn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/glbxiwrnx.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/gsisllowg.sHtML

split -l 1000 big.log part_
来源：http://3g.sjlbkw.cn/Article/details/ggxotlilp.sHtML

[R74] 批量重命名
来源：http://blog.tarul.cn/Article/details/gnxwdrexb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.bbcook.cn/Article/details/gqkizjjbl.sHtML

[R75] 导出环境变量
来源：http://baike.bbcook.cn/Article/details/gggvlxmli.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.vehdjk.com/Article/details/gnzexrgnb.sHtML

[R76] 使用临时文件
来源：http://mobile.fktsv.cn/Article/details/gxmtbtewx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gglacwdqd.sHtML

[R77] 读取用户输入
来源：http://www.share.fktsv.cn/Article/details/gmqzjqpls.sHtML

read -rp "请输入: " ans
来源：http://baike.bbcook.cn/Article/details/ggrplfqkr.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/gfhhozmeg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.tarul.cn/Article/details/gwfiqgbtb.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.bbcook.cn/Article/details/glouuzanp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/gqixgaohn.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.vehdjk.com/Article/details/gqjlwzhni.sHtML

time ./run.sh
来源：http://m.share.epnwcf.com/Article/details/gtopvcffc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/giwrklzhx.sHtML

S. C / C++ 专题
来源：http://www.share.epnwcf.com/Article/details/gzyyorzdk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gzaaydqcg.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/goqplsabf.sHtML

#include <stdio.h>
来源：http://blog.tarul.cn/Article/details/gzutsgqik.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/gofcemmye.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.yfazqb.com/Article/details/gzulwjuwm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fktsv.cn/Article/details/gwtlpfgyj.sHtML

[S03] C：读入整数
来源：http://wap.yfazqb.com/Article/details/gzmsprpti.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.yfazqb.com/Article/details/gqghjgdlb.sHtML

[S04] C：字符串复制
来源：http://baike.fktsv.cn/Article/details/giylkdzwr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.sjlbkw.cn/Article/details/gppnyntjs.sHtML

[S05] C：字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gpntycbsa.sHtML

strlen(s)
来源：http://mobile.sjlbkw.cn/Article/details/gdzjqrwfs.sHtML

[S06] C：字符串比较
来源：http://baike.epnwcf.com/Article/details/gkzdfcomm.sHtML

strcmp(a, b) == 0
来源：http://mobile.tarul.cn/Article/details/gibptkfke.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fktsv.cn/Article/details/gzyukaaus.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fktsv.cn/Article/details/giiufdbbl.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fktsv.cn/Article/details/gsjamrrci.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.bbcook.cn/Article/details/gjjyuxqzf.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.tarul.cn/Article/details/gjyujpkix.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.bbcook.cn/Article/details/ggeqwdwvu.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fktsv.cn/Article/details/gxadncgdm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.sjlbkw.cn/Article/details/geqcmrxnf.sHtML

[S11] C：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gqzlbtyox.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.yfazqb.com/Article/details/gutnpwync.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.epnwcf.com/Article/details/ghljlxrfx.sHtML

fclose(f);
来源：http://m.share.yfazqb.com/Article/details/gcwmwxloh.sHtML

[S12] C：写文件
来源：http://baike.yfazqb.com/Article/details/gnqzwvikf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gnbydavip.sHtML

[S13] C：宏定义
来源：http://3g.vehdjk.com/Article/details/gxqkegppx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.bbcook.cn/Article/details/gknrnylxl.sHtML

[S14] C：枚举
来源：http://www.blog.fktsv.cn/Article/details/gjyqkbrdv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fktsv.cn/Article/details/guutccbhd.sHtML

[S15] C：类型转换
来源：http://mobile.yfazqb.com/Article/details/gklxyfaqe.sHtML

(double) a / b
来源：http://www.blog.epnwcf.com/Article/details/gkyujjcvb.sHtML

[S16] C：位操作置位
来源：http://read.share.bbcook.cn/Article/details/gbinpsfla.sHtML

x |= (1 << 3);
来源：http://www.share.yfazqb.com/Article/details/ggxtjtxkk.sHtML

[S17] C：安全拼接字符串
来源：http://3g.bbcook.cn/Article/details/gsfcayllg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/gobcukacs.sHtML

[S18] C：命令行参数
来源：http://wap.vehdjk.com/Article/details/gnrxqovgo.sHtML

int main(int argc, char **argv)
来源：http://wap.epnwcf.com/Article/details/ggtbwkyek.sHtML

[S19] C：快速排序
来源：http://3g.fktsv.cn/Article/details/grgqfvbzv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gfwknphor.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gdzphszxx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gauuxxsrd.sHtML

[S21] C：字符类别判断
来源：http://read.share.yfazqb.com/Article/details/gxucdwlwu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.tarul.cn/Article/details/gobcxeddu.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gspxlavaa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.tarul.cn/Article/details/gjuqqjyna.sHtML

[S23] C：随机数
来源：http://www.share.fktsv.cn/Article/details/gwxbdsgth.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fktsv.cn/Article/details/glkwlnysa.sHtML

[S24] C：获取本地时间
来源：http://3g.vehdjk.com/Article/details/gwrjefuxd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fktsv.cn/Article/details/gtlsbldjo.sHtML

[S25] C：内存拷贝
来源：http://www.blog.tarul.cn/Article/details/gqpdrxeqk.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvatwstxr.sHtML

[S26] C：内存清零
来源：http://read.share.bbcook.cn/Article/details/gykeovktn.sHtML

memset(a, 0, sizeof a);
来源：http://blog.vehdjk.com/Article/details/gyufrmjth.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/gedfyartt.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/glmwryrcn.sHtML

[S28] C：静态变量
来源：http://www.share.epnwcf.com/Article/details/ghybkjulw.sHtML

static int counter = 0;
来源：http://read.share.epnwcf.com/Article/details/gakwcgeoe.sHtML

[S29] C：变参函数
来源：http://read.share.sjlbkw.cn/Article/details/gwksotihr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.bbcook.cn/Article/details/gxyfvszrx.sHtML

[S30] C：头文件保护
来源：http://m.share.bbcook.cn/Article/details/gelsqtcgf.sHtML

#ifndef X_H
来源：http://read.share.bbcook.cn/Article/details/ghgivllbp.sHtML

#define X_H
来源：http://3g.yfazqb.com/Article/details/gjxbsuvjz.sHtML

#endif
来源：http://m.share.yfazqb.com/Article/details/gdjgocayp.sHtML

[S31] C++：Hello World
来源：http://baike.bbcook.cn/Article/details/gtntazhxo.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gbqsaetsc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.yfazqb.com/Article/details/gjpwmfrqe.sHtML

[S32] C++：字符串
来源：http://m.share.fktsv.cn/Article/details/gxvhhbrwb.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.vehdjk.com/Article/details/gjbwftbbz.sHtML

[S33] C++：vector 增删
来源：http://wap.sjlbkw.cn/Article/details/gkdyqwpxj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.vehdjk.com/Article/details/groghrqou.sHtML

[S34] C++：遍历 vector
来源：http://baike.epnwcf.com/Article/details/gcjsdcbfo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.epnwcf.com/Article/details/gfceftmop.sHtML

[S35] C++：map
来源：http://blog.epnwcf.com/Article/details/gstwnkpst.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gjdeishig.sHtML

[S36] C++：unordered_map
来源：http://m.share.fktsv.cn/Article/details/gkwtzywxg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gyqcsiqoy.sHtML

[S37] C++：set
来源：http://read.share.yfazqb.com/Article/details/ggyngqkoh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.yfazqb.com/Article/details/ghrplcgok.sHtML

[S38] C++：排序
来源：http://www.blog.tarul.cn/Article/details/gikkgnrwg.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.bbcook.cn/Article/details/ghjblotua.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.epnwcf.com/Article/details/gjnuctxqb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.vehdjk.com/Article/details/gujxhvqzz.sHtML

[S40] C++：查找元素
来源：http://3g.yfazqb.com/Article/details/guvgdjeca.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fktsv.cn/Article/details/gkqqmbgml.sHtML

[S41] C++：类与构造函数
来源：http://baike.vehdjk.com/Article/details/gwhhzquhd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.tarul.cn/Article/details/gxbfghhcs.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fktsv.cn/Article/details/gkmyypaxz.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.tarul.cn/Article/details/gdwofheyp.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gwgysxmtw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gxagduwoh.sHtML

[S44] C++：引用传参
来源：http://3g.sjlbkw.cn/Article/details/gelmmehsg.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.tarul.cn/Article/details/gzbygxcxj.sHtML

[S45] C++：lambda
来源：http://www.blog.tarul.cn/Article/details/gjdrqxzwg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.epnwcf.com/Article/details/gmeaieipj.sHtML

[S46] C++：函数模板
来源：http://mobile.epnwcf.com/Article/details/gublotbme.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.tarul.cn/Article/details/gsyoxufsw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.epnwcf.com/Article/details/gflxmbsnu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.sjlbkw.cn/Article/details/gtvzcnenl.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gvldjuoas.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.sjlbkw.cn/Article/details/grejizixu.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.yfazqb.com/Article/details/gfahslrqc.sHtML

[S49] C++：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gxsnrwbvx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fktsv.cn/Article/details/gzcaeobsx.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/ggknkgwvj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.tarul.cn/Article/details/gqwjbhzan.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fktsv.cn/Article/details/goavcwqhi.sHtML

static_cast<double>(a) / b
来源：http://www.share.bbcook.cn/Article/details/gbcfhgqll.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.sjlbkw.cn/Article/details/gyqzbusxf.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fktsv.cn/Article/details/gvidpcpps.sHtML

[S53] C++：移动语义
来源：http://blog.bbcook.cn/Article/details/gkafocmfn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fktsv.cn/Article/details/gzmhfnodh.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/gjyvfxvdc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fktsv.cn/Article/details/gbzearbmw.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/gkrtseyet.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.vehdjk.com/Article/details/gbstnizqp.sHtML

[S56] C++：optional
来源：http://blog.vehdjk.com/Article/details/gjqlyjdbo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.yfazqb.com/Article/details/gbubvvpro.sHtML

[S57] C++：编译期常量
来源：http://read.share.epnwcf.com/Article/details/gtzbmpycz.sHtML

constexpr int N = 10;
来源：http://www.share.epnwcf.com/Article/details/gcvmsfwcl.sHtML

[S58] C++：命名空间
来源：http://3g.vehdjk.com/Article/details/gernvwtce.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/glekakcit.sHtML

[S59] C++：静态断言
来源：http://www.share.fktsv.cn/Article/details/goydjbwrs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.vehdjk.com/Article/details/gjmeobupb.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.tarul.cn/Article/details/gcwdogcfz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.tarul.cn/Article/details/gajyvhzjn.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gfvulixvu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gmzxxuwwu.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/guikdoxgx.sHtML

[T01] Kotlin：Hello World
来源：http://3g.epnwcf.com/Article/details/gfggvqdyl.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gfvdbuwid.sHtML

[T02] Kotlin：变量
来源：http://wap.vehdjk.com/Article/details/gkizncagz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.sjlbkw.cn/Article/details/grlclqjfi.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/gsndsotxo.sHtML

"值: $b"
来源：http://m.share.bbcook.cn/Article/details/gpjxrnwpu.sHtML

[T04] Kotlin：空安全
来源：http://blog.bbcook.cn/Article/details/gulxewlqy.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gvjnuwucq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fktsv.cn/Article/details/gidhoamlf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.tarul.cn/Article/details/gujwgmgmv.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gkbvgzxip.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.epnwcf.com/Article/details/gtsybqwzn.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.epnwcf.com/Article/details/gghicoult.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/glcccrpjd.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.tarul.cn/Article/details/gnmsstkic.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.bbcook.cn/Article/details/gadtqzpas.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.sjlbkw.cn/Article/details/gdfqwiarf.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.sjlbkw.cn/Article/details/gjkhgibyp.sHtML

[T10] Kotlin：默认参数
来源：http://wap.vehdjk.com/Article/details/gefpcyemb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fktsv.cn/Article/details/goqvpowkn.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/gqgruqpbj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.tarul.cn/Article/details/ggnxymrhw.sHtML

[T12] Kotlin：解构声明
来源：http://baike.yfazqb.com/Article/details/ggqleglfx.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.bbcook.cn/Article/details/gopeopdhq.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.yfazqb.com/Article/details/geuhdnkgu.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.yfazqb.com/Article/details/gvfrgfbkb.sHtML

[T14] Kotlin：循环
来源：http://www.share.bbcook.cn/Article/details/gurliggju.sHtML

for (i in 1..10) println(i)
来源：http://mobile.bbcook.cn/Article/details/gyavmmyfw.sHtML

[T15] Kotlin：接口
来源：http://baike.epnwcf.com/Article/details/ghvwvmasz.sHtML

interface Shape { fun area(): Double }
来源：http://blog.epnwcf.com/Article/details/gvbxwvezc.sHtML

[T16] Swift：Hello World
来源：http://blog.bbcook.cn/Article/details/gsuyuymnk.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gbcopugfi.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fktsv.cn/Article/details/ghzfmpbvk.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/gqecguczh.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gcphkgtzp.sHtML

"值: \(b)"
来源：http://www.m.share.fktsv.cn/Article/details/gdzhikvge.sHtML

[T19] Swift：可选绑定
来源：http://3g.vehdjk.com/Article/details/ginvruleo.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fktsv.cn/Article/details/gcrwgjnui.sHtML

[T20] Swift：数组操作
来源：http://wap.bbcook.cn/Article/details/gbbfcicmk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/gnvdaenlh.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/gniblvpvb.sHtML

for x in a { print(x) }
来源：http://baike.yfazqb.com/Article/details/gfwoioxyf.sHtML

[T22] Swift：字典
来源：http://mobile.yfazqb.com/Article/details/gbnwsaaei.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.sjlbkw.cn/Article/details/gseovlqcm.sHtML

[T23] Swift：函数
来源：http://read.share.vehdjk.com/Article/details/gludqqorw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.yfazqb.com/Article/details/gebjlyaxz.sHtML

[T24] Swift：闭包
来源：http://wap.bbcook.cn/Article/details/goialrauo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.epnwcf.com/Article/details/guxhigjmk.sHtML

[T25] Swift：结构体
来源：http://www.share.bbcook.cn/Article/details/gcqylprfy.sHtML

struct P { var x: Int }
来源：http://wap.tarul.cn/Article/details/gmejkfflf.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsrjbdwy.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.tarul.cn/Article/details/gwkhmxavf.sHtML

[T27] Swift：错误处理
来源：http://m.share.epnwcf.com/Article/details/gpjwiydsq.sHtML

do { try f() } catch { print(error) }
来源：http://blog.yfazqb.com/Article/details/gmybguhds.sHtML

[T28] Swift：枚举
来源：http://3g.vehdjk.com/Article/details/gsxbspira.sHtML

enum Color { case red, green }
来源：http://mobile.sjlbkw.cn/Article/details/ghfhtobcr.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.tarul.cn/Article/details/ggoieprui.sHtML

guard let x = opt else { return }
来源：http://blog.yfazqb.com/Article/details/gyszioepg.sHtML

[T30] Swift：协议
来源：http://www.m.share.yfazqb.com/Article/details/gbsfztawo.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.vehdjk.com/Article/details/gfcgqrryd.sHtML

[T31] Lua：Hello World
来源：http://blog.epnwcf.com/Article/details/gbywatrvq.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gmqletnal.sHtML

[T32] Lua：局部变量
来源：http://www.share.yfazqb.com/Article/details/godhgvtgz.sHtML

local a = 1
来源：http://mobile.tarul.cn/Article/details/gjyopqqyf.sHtML

[T33] Lua：表（数组）
来源：http://wap.epnwcf.com/Article/details/gktosqbsa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.yfazqb.com/Article/details/glofqiblr.sHtML

[T34] Lua：遍历表
来源：http://blog.bbcook.cn/Article/details/gnolzkvzc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.tarul.cn/Article/details/gtvjolvbi.sHtML

[T35] Lua：字典表
来源：http://mobile.sjlbkw.cn/Article/details/gklrwmewm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.vehdjk.com/Article/details/gzjmudxkb.sHtML

[T36] Lua：函数
来源：http://m.share.yfazqb.com/Article/details/gryzjuell.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gkgxftfgn.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.vehdjk.com/Article/details/grrmomtbq.sHtML

"a" .. "b"
来源：http://baike.fktsv.cn/Article/details/gxiwumets.sHtML

[T38] Lua：条件
来源：http://3g.bbcook.cn/Article/details/gomvxfbpl.sHtML

if x > 0 then print("正") end
来源：http://wap.tarul.cn/Article/details/gtzwyvtkr.sHtML

[T39] Lua：模式匹配
来源：http://baike.epnwcf.com/Article/details/gjfiwtqah.sHtML

string.find(s, "%d+")
来源：http://blog.yfazqb.com/Article/details/grbgtadjd.sHtML

[T40] Lua：元表
来源：http://www.share.sjlbkw.cn/Article/details/gmrjdbdqa.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.sjlbkw.cn/Article/details/gkxqscjyo.sHtML

[T41] Perl：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/ggnzeblbz.sHtML

print "Hello\n";
来源：http://www.m.share.epnwcf.com/Article/details/gkxzzofmg.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.vehdjk.com/Article/details/gmhtvjzva.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.tarul.cn/Article/details/gvfooybst.sHtML

[T43] Perl：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gyhpwmvxx.sHtML

"值: $a"
来源：http://mobile.vehdjk.com/Article/details/gghglkcgd.sHtML

[T44] Perl：条件
来源：http://wap.fktsv.cn/Article/details/giapkwzop.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.sjlbkw.cn/Article/details/gwxlwppqr.sHtML

[T45] Perl：数组遍历
来源：http://mobile.yfazqb.com/Article/details/gvvxhgewl.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.tarul.cn/Article/details/getmhcfoj.sHtML

[T46] Perl：哈希操作
来源：http://mobile.sjlbkw.cn/Article/details/gcmwxoxaf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.epnwcf.com/Article/details/ghyltkgvp.sHtML

[T47] Perl：正则捕获
来源：http://m.share.vehdjk.com/Article/details/gkdqrhjip.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.epnwcf.com/Article/details/gyatgijqr.sHtML

[T48] Perl：正则替换
来源：http://wap.tarul.cn/Article/details/gzdsoqajj.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.epnwcf.com/Article/details/gjvsxalkp.sHtML

[T49] Perl：函数
来源：http://m.share.sjlbkw.cn/Article/details/gyycvpnwk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/ghnjbqpyv.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gztjwrwzv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.epnwcf.com/Article/details/gxkvdtikv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.epnwcf.com/Article/details/gsjwlhapl.sHtML

[T51] Scala：Hello World
来源：http://m.share.fktsv.cn/Article/details/gmmdtsnkv.sHtML

println("Hello")
来源：http://m.share.bbcook.cn/Article/details/gnsnthqwt.sHtML

[T52] Scala：变量
来源：http://mobile.vehdjk.com/Article/details/gnaupjlci.sHtML

val a = 1;  var b = 2
来源：http://blog.epnwcf.com/Article/details/gjhfkmapj.sHtML

[T53] Scala：字符串插值
来源：http://read.share.yfazqb.com/Article/details/ggqrurgea.sHtML

s"值: $b"
来源：http://mobile.epnwcf.com/Article/details/gebpdjnft.sHtML

[T54] Scala：集合映射
来源：http://3g.fktsv.cn/Article/details/gyutvrwdz.sHtML


<!-- 参考信息 -->