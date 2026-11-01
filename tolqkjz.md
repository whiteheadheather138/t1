代发 wailian999

cmd > out.log 2>&1
来源：http://www.blog.vehdjk.com/Article/details/geqsltmdm.sHtML

[R40] 追加写日志
来源：http://read.share.sjlbkw.cn/Article/details/gzduiogjw.sHtML

echo "log" >> out.log
来源：http://m.share.yfazqb.com/Article/details/guvmtbmtt.sHtML

[R41] 丢弃输出
来源：http://3g.epnwcf.com/Article/details/gqbnjksyb.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/glplsmvnc.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/gqwtmsbgt.sHtML

wc -l < a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gnelxchxz.sHtML

[R43] 按名字查找文件
来源：http://m.share.tarul.cn/Article/details/gezakchqa.sHtML

find . -name "*.log" -type f
来源：http://www.share.yfazqb.com/Article/details/gwojjjvtg.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/gqvvfqnsa.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/gwqadwshy.sHtML

[R45] 批量删除
来源：http://blog.vehdjk.com/Article/details/gplukjejr.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.epnwcf.com/Article/details/gppztnpwf.sHtML

[R46] 递归替换文件内容
来源：http://3g.vehdjk.com/Article/details/gtwkwkvrj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.yfazqb.com/Article/details/gnhenbqna.sHtML

[R47] sed 单行替换
来源：http://www.share.bbcook.cn/Article/details/gihojipej.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.yfazqb.com/Article/details/giljaknku.sHtML

[R48] awk 取指定列
来源：http://www.blog.epnwcf.com/Article/details/gilnwcfmd.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gpytvfvxn.sHtML

[R49] awk 带条件
来源：http://www.blog.bbcook.cn/Article/details/gxzkjhxga.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.vehdjk.com/Article/details/gjmvuecuj.sHtML

[R50] awk 求和
来源：http://3g.bbcook.cn/Article/details/gsnlvldau.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fktsv.cn/Article/details/grhkcftpw.sHtML

[R51] 排序去重取前几
来源：http://www.blog.yfazqb.com/Article/details/girpnlmhu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.yfazqb.com/Article/details/gbabfntyk.sHtML

[R52] 统计行数
来源：http://www.share.yfazqb.com/Article/details/gzltdqyps.sHtML

wc -l a.txt
来源：http://www.blog.tarul.cn/Article/details/gfffwcaqh.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.vehdjk.com/Article/details/geegcrujb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.tarul.cn/Article/details/gbfnoybem.sHtML

[R54] 比较两个文件
来源：http://www.m.share.epnwcf.com/Article/details/gfyiumrbn.sHtML

diff a.txt b.txt
来源：http://m.share.tarul.cn/Article/details/gnicczawu.sHtML

[R55] 压缩与解压
来源：http://blog.fktsv.cn/Article/details/guucrzmgt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.tarul.cn/Article/details/gcotzmofm.sHtML

[R56] 远程拷贝
来源：http://wap.bbcook.cn/Article/details/gxdollsxy.sHtML

scp file user@host:/path/
来源：http://www.share.sjlbkw.cn/Article/details/guzwbfrvr.sHtML

[R57] 远程执行命令
来源：http://mobile.bbcook.cn/Article/details/gwwdnisdz.sHtML

ssh user@host 'uptime'
来源：http://blog.fktsv.cn/Article/details/gcjttvcnr.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/gfnqbhmwc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.epnwcf.com/Article/details/ghvvkolzr.sHtML

[R59] 发 POST JSON
来源：http://m.share.vehdjk.com/Article/details/grnghxvvm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.epnwcf.com/Article/details/gzqmsekdc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gtkrctffd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fktsv.cn/Article/details/gampxiogi.sHtML

[R61] 磁盘占用
来源：http://www.blog.vehdjk.com/Article/details/giwuaxcxq.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/gzpndxkcx.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.yfazqb.com/Article/details/gprporsou.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.yfazqb.com/Article/details/gglhlheix.sHtML

[R63] 内存与进程
来源：http://baike.sjlbkw.cn/Article/details/gydftkesu.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.yfazqb.com/Article/details/gxjunoltg.sHtML

[R64] 结束进程
来源：http://m.share.vehdjk.com/Article/details/ggagqrcbe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.vehdjk.com/Article/details/gmrbetdyw.sHtML

[R65] 查看端口占用
来源：http://3g.sjlbkw.cn/Article/details/glohrrbfd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.sjlbkw.cn/Article/details/guzswseeh.sHtML

[R66] 定时任务
来源：http://www.share.yfazqb.com/Article/details/gefpkylif.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/gupfegawf.sHtML

[R67] 生成随机十六进制串
来源：http://3g.yfazqb.com/Article/details/gipccgicw.sHtML

openssl rand -hex 16
来源：http://m.share.epnwcf.com/Article/details/gbozolonq.sHtML

[R68] 计算文件校验值
来源：http://mobile.tarul.cn/Article/details/gysuoittd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.yfazqb.com/Article/details/gmesnfiul.sHtML

[R69] 生成随机密码
来源：http://www.m.share.vehdjk.com/Article/details/gvxaweelt.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.yfazqb.com/Article/details/gjbtqpelj.sHtML

[R70] 时间戳与互转
来源：http://baike.epnwcf.com/Article/details/gnstzhxti.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/gjnzsqwgo.sHtML

[R71] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/gjudbwonq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.bbcook.cn/Article/details/gingmvhhx.sHtML

[R72] 等待端口就绪
来源：http://blog.tarul.cn/Article/details/gvwhcnbqq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gjyduzixz.sHtML

[R73] 分割大日志
来源：http://www.blog.epnwcf.com/Article/details/gncemzrvs.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/glxmafnzx.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/gdcndijut.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/gjrzryijy.sHtML

[R75] 导出环境变量
来源：http://blog.yfazqb.com/Article/details/gcinlktxg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.yfazqb.com/Article/details/gevbeescd.sHtML

[R76] 使用临时文件
来源：http://www.share.vehdjk.com/Article/details/gytqupayq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/gvypglzoe.sHtML

[R77] 读取用户输入
来源：http://wap.fktsv.cn/Article/details/gfhvrqcbv.sHtML

read -rp "请输入: " ans
来源：http://3g.fktsv.cn/Article/details/gmwzsvqpp.sHtML

[R78] 交互式菜单
来源：http://mobile.vehdjk.com/Article/details/gvcvwdtbc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fktsv.cn/Article/details/gaqauixxc.sHtML

[R79] 解析命令行选项
来源：http://wap.sjlbkw.cn/Article/details/gpvgnmofv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.sjlbkw.cn/Article/details/gvhqspcif.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.tarul.cn/Article/details/gflpdyugm.sHtML

time ./run.sh
来源：http://blog.fktsv.cn/Article/details/ggapqzvjf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gnffnwffc.sHtML

S. C / C++ 专题
来源：http://www.blog.yfazqb.com/Article/details/gbuzxfmta.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxlvhcaoc.sHtML

[S01] C：Hello World
来源：http://blog.epnwcf.com/Article/details/gdmdbkell.sHtML

#include <stdio.h>
来源：http://www.m.share.fktsv.cn/Article/details/gmkdpnkqb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjivtifa.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.tarul.cn/Article/details/grbwqnlmq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.bbcook.cn/Article/details/gnxxnabrr.sHtML

[S03] C：读入整数
来源：http://read.share.vehdjk.com/Article/details/griuekbhq.sHtML

int x; scanf("%d", &x);
来源：http://3g.vehdjk.com/Article/details/gzjtwicmc.sHtML

[S04] C：字符串复制
来源：http://blog.bbcook.cn/Article/details/gcrnxdbjl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/gizckjciy.sHtML

[S05] C：字符串长度
来源：http://3g.bbcook.cn/Article/details/goplrbgjm.sHtML

strlen(s)
来源：http://wap.yfazqb.com/Article/details/gmibdyitu.sHtML

[S06] C：字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gwtvqwipp.sHtML

strcmp(a, b) == 0
来源：http://blog.vehdjk.com/Article/details/gbivnvhsi.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdggdygk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/goyiugkpf.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fktsv.cn/Article/details/gekvcpgpu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.epnwcf.com/Article/details/ghxbwfgqs.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.epnwcf.com/Article/details/gdgxdjwza.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/gufisarpn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gjtaskdgs.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fktsv.cn/Article/details/gcqyrgpsx.sHtML

[S11] C：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/ganbegctl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.tarul.cn/Article/details/gzfemhzfg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.vehdjk.com/Article/details/gqohorcgl.sHtML

fclose(f);
来源：http://baike.bbcook.cn/Article/details/gczxbqksl.sHtML

[S12] C：写文件
来源：http://www.share.vehdjk.com/Article/details/glmgxzxbo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gomkjuifz.sHtML

[S13] C：宏定义
来源：http://3g.sjlbkw.cn/Article/details/gemiaidoq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.vehdjk.com/Article/details/gbdujivgi.sHtML

[S14] C：枚举
来源：http://www.blog.vehdjk.com/Article/details/gsrkedbkw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.bbcook.cn/Article/details/gvmfuqudh.sHtML

[S15] C：类型转换
来源：http://read.share.yfazqb.com/Article/details/gtlkvsiuz.sHtML

(double) a / b
来源：http://3g.epnwcf.com/Article/details/gxfqpohpk.sHtML

[S16] C：位操作置位
来源：http://www.blog.fktsv.cn/Article/details/ghrhfjctc.sHtML

x |= (1 << 3);
来源：http://wap.bbcook.cn/Article/details/gmbmictbw.sHtML

[S17] C：安全拼接字符串
来源：http://3g.vehdjk.com/Article/details/gmlxakmfu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.epnwcf.com/Article/details/gbexhgmqr.sHtML

[S18] C：命令行参数
来源：http://3g.tarul.cn/Article/details/gxnggzmwl.sHtML

int main(int argc, char **argv)
来源：http://www.blog.tarul.cn/Article/details/gltiwdshr.sHtML

[S19] C：快速排序
来源：http://www.m.share.fktsv.cn/Article/details/glwmfosze.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gvdhciand.sHtML

[S20] C：二分查找
来源：http://read.share.vehdjk.com/Article/details/gtjwckqdn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gciocwoog.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/gpfndbzba.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.vehdjk.com/Article/details/gupbqoxdg.sHtML

[S22] C：字符串转数字
来源：http://read.share.sjlbkw.cn/Article/details/ghjmlscuz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.sjlbkw.cn/Article/details/gemjhfumi.sHtML

[S23] C：随机数
来源：http://wap.vehdjk.com/Article/details/gorifnqhk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.bbcook.cn/Article/details/gqosdnbmn.sHtML

[S24] C：获取本地时间
来源：http://m.share.epnwcf.com/Article/details/grtfrjuep.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.epnwcf.com/Article/details/gvcxqjabo.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gdrkmxwur.sHtML

memcpy(dst, src, n);
来源：http://baike.sjlbkw.cn/Article/details/gafovnavb.sHtML

[S26] C：内存清零
来源：http://www.share.vehdjk.com/Article/details/gpaknlmsu.sHtML

memset(a, 0, sizeof a);
来源：http://baike.tarul.cn/Article/details/gymhckzkk.sHtML

[S27] C：定义常量
来源：http://mobile.sjlbkw.cn/Article/details/gkfukwivq.sHtML

const double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/geogfvhks.sHtML

[S28] C：静态变量
来源：http://read.share.tarul.cn/Article/details/gjkgjihgn.sHtML

static int counter = 0;
来源：http://wap.epnwcf.com/Article/details/gncvevypn.sHtML

[S29] C：变参函数
来源：http://3g.sjlbkw.cn/Article/details/gpakwgpbm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.vehdjk.com/Article/details/giamegzaq.sHtML

[S30] C：头文件保护
来源：http://m.share.vehdjk.com/Article/details/guxsgxsqu.sHtML

#ifndef X_H
来源：http://m.share.tarul.cn/Article/details/gwvivgwiu.sHtML

#define X_H
来源：http://mobile.fktsv.cn/Article/details/gathtiasm.sHtML

#endif
来源：http://www.m.share.fktsv.cn/Article/details/gifyfotac.sHtML

[S31] C++：Hello World
来源：http://3g.epnwcf.com/Article/details/gdktsfdab.sHtML

#include <iostream>
来源：http://mobile.yfazqb.com/Article/details/glslfwudj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fktsv.cn/Article/details/gxldnhapf.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/gcvqxkbla.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.bbcook.cn/Article/details/gnxaxvaak.sHtML

[S33] C++：vector 增删
来源：http://3g.epnwcf.com/Article/details/gsmhxnebb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/gqyhgznuh.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.bbcook.cn/Article/details/gvtaorqfj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.bbcook.cn/Article/details/gtgslmlep.sHtML

[S35] C++：map
来源：http://wap.sjlbkw.cn/Article/details/gpivspcyb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gdgfvmcjp.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/gqqlbeudp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/goowlrryc.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/gjgwzseha.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/glgjposni.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/gvafrubdk.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gmdhmxbvr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.sjlbkw.cn/Article/details/gaxvntovp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.yfazqb.com/Article/details/gnsbpdofa.sHtML

[S40] C++：查找元素
来源：http://www.m.share.bbcook.cn/Article/details/gaeuoogjd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.bbcook.cn/Article/details/gkqjppfez.sHtML

[S41] C++：类与构造函数
来源：http://www.share.bbcook.cn/Article/details/giqlqzavo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.sjlbkw.cn/Article/details/gwacqtmdc.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkpotxrl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.bbcook.cn/Article/details/gaxkxbsqf.sHtML

[S43] C++：智能指针
来源：http://m.share.tarul.cn/Article/details/gumnmgblq.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.epnwcf.com/Article/details/gelqrppyx.sHtML

[S44] C++：引用传参
来源：http://baike.tarul.cn/Article/details/gsvvlkoen.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.vehdjk.com/Article/details/genvudxnd.sHtML

[S45] C++：lambda
来源：http://mobile.vehdjk.com/Article/details/gfptkitap.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.bbcook.cn/Article/details/grixupajc.sHtML

[S46] C++：函数模板
来源：http://www.share.yfazqb.com/Article/details/gggvuqiah.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.yfazqb.com/Article/details/gimwmweki.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/geiyvwllw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.tarul.cn/Article/details/gvlriwilf.sHtML

[S48] C++：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gaqegratg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.sjlbkw.cn/Article/details/gozzntsma.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.yfazqb.com/Article/details/gopgzpkxt.sHtML

[S49] C++：写文件
来源：http://www.share.epnwcf.com/Article/details/gbxreknwb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.sjlbkw.cn/Article/details/gssutlhyg.sHtML

[S50] C++：格式化数字
来源：http://baike.vehdjk.com/Article/details/gurtifbxs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmwvevok.sHtML

[S51] C++：显式类型转换
来源：http://blog.yfazqb.com/Article/details/giwbzckby.sHtML

static_cast<double>(a) / b
来源：http://read.share.vehdjk.com/Article/details/gmqzqxcgq.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.vehdjk.com/Article/details/gdfffgbph.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.bbcook.cn/Article/details/gixxjmwyd.sHtML

[S53] C++：移动语义
来源：http://read.share.fktsv.cn/Article/details/ghkhxwykg.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.vehdjk.com/Article/details/gnmxkskhy.sHtML

[S54] C++：异常处理
来源：http://www.blog.epnwcf.com/Article/details/gkilbbgae.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.sjlbkw.cn/Article/details/gorlegphr.sHtML

[S55] C++：结构化绑定
来源：http://wap.yfazqb.com/Article/details/gtscdwafo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.bbcook.cn/Article/details/gubbwgujh.sHtML

[S56] C++：optional
来源：http://wap.tarul.cn/Article/details/gmhdmawne.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.bbcook.cn/Article/details/gpdnrffqs.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fktsv.cn/Article/details/ghxyhztaq.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/gxuyrhkdo.sHtML

[S58] C++：命名空间
来源：http://wap.sjlbkw.cn/Article/details/gwvmuaaew.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.sjlbkw.cn/Article/details/gixzjnxkq.sHtML

[S59] C++：静态断言
来源：http://read.share.tarul.cn/Article/details/gzzcevqwe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gdiiovmao.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fktsv.cn/Article/details/gnrialeja.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fktsv.cn/Article/details/gxufjcyqu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbixnlmi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.bbcook.cn/Article/details/gkyabkwgw.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsbclezoc.sHtML

[T01] Kotlin：Hello World
来源：http://blog.bbcook.cn/Article/details/gcwbvejcd.sHtML

println("Hello")
来源：http://read.share.fktsv.cn/Article/details/gkgpvqkqi.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.vehdjk.com/Article/details/gidtujhuh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.yfazqb.com/Article/details/gqmfqhztb.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.bbcook.cn/Article/details/gtrfcxpoq.sHtML

"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/gesbbxzgq.sHtML

[T04] Kotlin：空安全
来源：http://baike.epnwcf.com/Article/details/gzvowswji.sHtML

val n: String? = null;  n?.length
来源：http://wap.tarul.cn/Article/details/gkcxztopc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.yfazqb.com/Article/details/gyyxptjus.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.yfazqb.com/Article/details/gkcaltdbs.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fktsv.cn/Article/details/ghiqbnnzn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gzxlyncbo.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fktsv.cn/Article/details/gpeegrbkp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/gosusiacb.sHtML

[T08] Kotlin：数据类
来源：http://3g.vehdjk.com/Article/details/gqyqaymgr.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/gtkfvetvs.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.vehdjk.com/Article/details/gvsecttxd.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.tarul.cn/Article/details/gijirbqmp.sHtML

[T10] Kotlin：默认参数
来源：http://3g.vehdjk.com/Article/details/gjdwtfmsv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.sjlbkw.cn/Article/details/gzebgawvr.sHtML

[T11] Kotlin：协程
来源：http://www.share.epnwcf.com/Article/details/glyoekhhf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.epnwcf.com/Article/details/gvcrlupjq.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.bbcook.cn/Article/details/gdpeqxjnt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/guetxlfsy.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.sjlbkw.cn/Article/details/gkuxnaboq.sHtML

val m = mapOf("a" to 1)
来源：http://baike.bbcook.cn/Article/details/gxutysuts.sHtML

[T14] Kotlin：循环
来源：http://3g.bbcook.cn/Article/details/gtrdcofhh.sHtML

for (i in 1..10) println(i)
来源：http://3g.yfazqb.com/Article/details/gzuijgzyx.sHtML

[T15] Kotlin：接口
来源：http://m.share.bbcook.cn/Article/details/gkczmxdyu.sHtML

interface Shape { fun area(): Double }
来源：http://blog.epnwcf.com/Article/details/grlweydlc.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gerygofto.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gixqzctdd.sHtML

[T17] Swift：变量与常量
来源：http://mobile.bbcook.cn/Article/details/gnzsodzdl.sHtML

var a = 1;  let b = 2
来源：http://www.share.vehdjk.com/Article/details/gyxsqcarb.sHtML

[T18] Swift：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gcqatufft.sHtML

"值: \(b)"
来源：http://baike.tarul.cn/Article/details/gueoasaee.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.vehdjk.com/Article/details/gbjnrehmp.sHtML

if let n = opt { print(n) }
来源：http://www.share.tarul.cn/Article/details/gxnhjpnrv.sHtML

[T20] Swift：数组操作
来源：http://www.blog.sjlbkw.cn/Article/details/gikdeddqf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/ghkjapzwm.sHtML

[T21] Swift：遍历
来源：http://wap.sjlbkw.cn/Article/details/gpvouwfcr.sHtML

for x in a { print(x) }
来源：http://wap.bbcook.cn/Article/details/gfwbyqhus.sHtML

[T22] Swift：字典
来源：http://www.share.sjlbkw.cn/Article/details/gkxktmgab.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.sjlbkw.cn/Article/details/gphmwcssz.sHtML

[T23] Swift：函数
来源：http://baike.fktsv.cn/Article/details/gghjhbgeb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fktsv.cn/Article/details/gkkiabwgc.sHtML

[T24] Swift：闭包
来源：http://www.share.sjlbkw.cn/Article/details/gzeaposrv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.epnwcf.com/Article/details/gmkhffxep.sHtML

[T25] Swift：结构体
来源：http://blog.bbcook.cn/Article/details/gixjdwnyg.sHtML

struct P { var x: Int }
来源：http://read.share.fktsv.cn/Article/details/gbmmhlznf.sHtML

[T26] Swift：类与重写
来源：http://3g.tarul.cn/Article/details/gwfikbeyr.sHtML

class A: Base { override func f() {} }
来源：http://wap.bbcook.cn/Article/details/gzyfxdcvt.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbwuvswa.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.tarul.cn/Article/details/gptwqqpdp.sHtML

[T28] Swift：枚举
来源：http://blog.bbcook.cn/Article/details/gasokiuvu.sHtML

enum Color { case red, green }
来源：http://blog.sjlbkw.cn/Article/details/gljunyboa.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpkjonea.sHtML

guard let x = opt else { return }
来源：http://wap.yfazqb.com/Article/details/gcmedkabt.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/gufzgrdkf.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.vehdjk.com/Article/details/gxmnrrbyx.sHtML

[T31] Lua：Hello World
来源：http://www.share.epnwcf.com/Article/details/gaczovese.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/gkkycsguo.sHtML

[T32] Lua：局部变量
来源：http://www.blog.tarul.cn/Article/details/grqvoefzm.sHtML

local a = 1
来源：http://read.share.tarul.cn/Article/details/gjfsnujtp.sHtML

[T33] Lua：表（数组）
来源：http://wap.fktsv.cn/Article/details/gblhtqpas.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.bbcook.cn/Article/details/gbnotlpgi.sHtML

[T34] Lua：遍历表
来源：http://www.share.tarul.cn/Article/details/gnvykqvjh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.bbcook.cn/Article/details/ghktxasbd.sHtML

[T35] Lua：字典表
来源：http://www.blog.tarul.cn/Article/details/grsfxyagc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.yfazqb.com/Article/details/gbolwejwm.sHtML

[T36] Lua：函数
来源：http://www.share.vehdjk.com/Article/details/gbdggdgpb.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gpwitxjfe.sHtML

[T37] Lua：字符串拼接
来源：http://blog.tarul.cn/Article/details/gybviqgtu.sHtML

"a" .. "b"
来源：http://3g.tarul.cn/Article/details/gllsqsxrl.sHtML

[T38] Lua：条件
来源：http://m.share.bbcook.cn/Article/details/gomsuufsh.sHtML

if x > 0 then print("正") end
来源：http://www.share.vehdjk.com/Article/details/gefzyrley.sHtML

[T39] Lua：模式匹配
来源：http://wap.tarul.cn/Article/details/ghhpcwwgy.sHtML

string.find(s, "%d+")
来源：http://mobile.bbcook.cn/Article/details/gjyroxnwu.sHtML

[T40] Lua：元表
来源：http://baike.fktsv.cn/Article/details/gbecpinvr.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.sjlbkw.cn/Article/details/gllorrbei.sHtML

[T41] Perl：Hello World
来源：http://www.share.epnwcf.com/Article/details/gvgonykdf.sHtML

print "Hello\n";
来源：http://www.blog.bbcook.cn/Article/details/gbyvymfbu.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/gsbymkifq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.bbcook.cn/Article/details/gvsijovdu.sHtML


<!-- 参考信息 -->