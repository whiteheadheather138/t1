代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/goxwlpbnt.sHtML

[R42] 输入重定向
来源：http://www.blog.vehdjk.com/Article/details/gldwyavql.sHtML

wc -l < a.txt
来源：http://read.share.yfazqb.com/Article/details/gxxvlukkl.sHtML

[R43] 按名字查找文件
来源：http://baike.sjlbkw.cn/Article/details/gkhyezeqp.sHtML

find . -name "*.log" -type f
来源：http://3g.yfazqb.com/Article/details/ggpwzedkf.sHtML

[R44] 按修改时间查找
来源：http://3g.fktsv.cn/Article/details/gsqtaspot.sHtML

find . -mtime -7 -type f
来源：http://blog.sjlbkw.cn/Article/details/gaqoarvre.sHtML

[R45] 批量删除
来源：http://3g.epnwcf.com/Article/details/gtutbyiew.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.bbcook.cn/Article/details/gctsvvvcw.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fktsv.cn/Article/details/gmwhdvfle.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.sjlbkw.cn/Article/details/ghfvrbwqx.sHtML

[R47] sed 单行替换
来源：http://m.share.fktsv.cn/Article/details/gdzqgnawj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gbcpjlbfj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.tarul.cn/Article/details/gzrsudegh.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gespegjue.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/gooprikkd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.bbcook.cn/Article/details/guirpajnz.sHtML

[R50] awk 求和
来源：http://mobile.vehdjk.com/Article/details/gkagyjcsz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.yfazqb.com/Article/details/ggxetlefy.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.tarul.cn/Article/details/ggvnkmjdr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/gbdswbvck.sHtML

[R52] 统计行数
来源：http://blog.yfazqb.com/Article/details/gcvghjprm.sHtML

wc -l a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gqxkzsmnq.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/gsswwrnnh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.epnwcf.com/Article/details/goxoadohd.sHtML

[R54] 比较两个文件
来源：http://www.blog.tarul.cn/Article/details/gkflfubvz.sHtML

diff a.txt b.txt
来源：http://m.share.vehdjk.com/Article/details/gewhjmydt.sHtML

[R55] 压缩与解压
来源：http://3g.fktsv.cn/Article/details/gohnroiln.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.vehdjk.com/Article/details/geirirrlm.sHtML

[R56] 远程拷贝
来源：http://read.share.tarul.cn/Article/details/gtbvnbjul.sHtML

scp file user@host:/path/
来源：http://read.share.bbcook.cn/Article/details/grpxvcxdd.sHtML

[R57] 远程执行命令
来源：http://blog.bbcook.cn/Article/details/gevaviato.sHtML

ssh user@host 'uptime'
来源：http://wap.sjlbkw.cn/Article/details/ghzeupdsp.sHtML

[R58] 下载文件
来源：http://3g.tarul.cn/Article/details/gcyoucabz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.vehdjk.com/Article/details/gymnwcnyw.sHtML

[R59] 发 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gkwcyeuog.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.sjlbkw.cn/Article/details/gybmfazza.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.sjlbkw.cn/Article/details/gaziyepuj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.yfazqb.com/Article/details/garvfdbhn.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/gszvckdzb.sHtML

df -h;  du -sh *
来源：http://www.blog.yfazqb.com/Article/details/ghtdylkjo.sHtML

[R62] 找最占空间的文件
来源：http://wap.yfazqb.com/Article/details/gtdygyxsn.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.yfazqb.com/Article/details/gywlfqrem.sHtML

[R63] 内存与进程
来源：http://wap.tarul.cn/Article/details/gbdlvtlou.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/gfgedyexi.sHtML

[R64] 结束进程
来源：http://www.share.yfazqb.com/Article/details/gncbxzxvc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.vehdjk.com/Article/details/glwtggdxl.sHtML

[R65] 查看端口占用
来源：http://read.share.vehdjk.com/Article/details/gyrmoryib.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fktsv.cn/Article/details/gqfkbscfc.sHtML

[R66] 定时任务
来源：http://www.m.share.tarul.cn/Article/details/gvalxuisx.sHtML

crontab -e;  crontab -l
来源：http://blog.yfazqb.com/Article/details/gnvqpwyoc.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.tarul.cn/Article/details/glgbtcpbg.sHtML

openssl rand -hex 16
来源：http://m.share.epnwcf.com/Article/details/gilfgkovs.sHtML

[R68] 计算文件校验值
来源：http://baike.epnwcf.com/Article/details/gcmxmaxkj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fktsv.cn/Article/details/gjivpyaec.sHtML

[R69] 生成随机密码
来源：http://3g.fktsv.cn/Article/details/gdimihihm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.epnwcf.com/Article/details/gcjpetlke.sHtML

[R70] 时间戳与互转
来源：http://wap.bbcook.cn/Article/details/gmxehmbhm.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.epnwcf.com/Article/details/gotglofmm.sHtML

[R71] 日期格式化
来源：http://3g.bbcook.cn/Article/details/ggrwgrygj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.yfazqb.com/Article/details/gqvifwnbv.sHtML

[R72] 等待端口就绪
来源：http://mobile.epnwcf.com/Article/details/gxmyenyvt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/ggkxnkfvu.sHtML

[R73] 分割大日志
来源：http://wap.epnwcf.com/Article/details/gelfpeout.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/glfqjmcmz.sHtML

[R74] 批量重命名
来源：http://wap.vehdjk.com/Article/details/gsztdshoj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.epnwcf.com/Article/details/gmhzvifld.sHtML

[R75] 导出环境变量
来源：http://mobile.tarul.cn/Article/details/gxbyaprnq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.tarul.cn/Article/details/gmqvlkdzl.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/gwqlcxddu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/gfuzofkwy.sHtML

[R77] 读取用户输入
来源：http://www.blog.epnwcf.com/Article/details/gsazgwrwm.sHtML

read -rp "请输入: " ans
来源：http://mobile.vehdjk.com/Article/details/gilomgwor.sHtML

[R78] 交互式菜单
来源：http://read.share.epnwcf.com/Article/details/gmwjpopsx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.vehdjk.com/Article/details/gbwcbpbpm.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gmdfvuodi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/gspcjedzz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.vehdjk.com/Article/details/gisofoxob.sHtML

time ./run.sh
来源：http://3g.vehdjk.com/Article/details/ggnlisdap.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnrouyghc.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/gikeximse.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ggnwpckoi.sHtML

[S01] C：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gmrjhcliz.sHtML

#include <stdio.h>
来源：http://blog.yfazqb.com/Article/details/gadwlmbby.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.yfazqb.com/Article/details/gskkuegkn.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.bbcook.cn/Article/details/gwgpevrjo.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.epnwcf.com/Article/details/glbusozbo.sHtML

[S03] C：读入整数
来源：http://www.blog.yfazqb.com/Article/details/gjnuztocu.sHtML

int x; scanf("%d", &x);
来源：http://3g.sjlbkw.cn/Article/details/gckvlamgc.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/gvxpdgekm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.yfazqb.com/Article/details/gcftmfqrr.sHtML

[S05] C：字符串长度
来源：http://baike.vehdjk.com/Article/details/gjlunjcij.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/glhpgjdax.sHtML

[S06] C：字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gfloznnmn.sHtML

strcmp(a, b) == 0
来源：http://3g.sjlbkw.cn/Article/details/gclcjzost.sHtML

[S07] C：数组遍历求和
来源：http://3g.vehdjk.com/Article/details/gccuucmrk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.yfazqb.com/Article/details/gubqkkrjo.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.epnwcf.com/Article/details/goikgcvgn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.epnwcf.com/Article/details/ginjpexyt.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.yfazqb.com/Article/details/guykwkaod.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/gogjemzxe.sHtML

[S10] C：指针与解引用
来源：http://blog.epnwcf.com/Article/details/gaxppvnow.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fktsv.cn/Article/details/gjbjtkoih.sHtML

[S11] C：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gwhvqvvkg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.yfazqb.com/Article/details/gveqtbpzj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.tarul.cn/Article/details/gmyzaxnyg.sHtML

fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gkdlkafrn.sHtML

[S12] C：写文件
来源：http://3g.epnwcf.com/Article/details/gbnpofkbq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gjxzntnyr.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/ggkdgbwwy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.vehdjk.com/Article/details/gwraoewoz.sHtML

[S14] C：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqgbdpsj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.tarul.cn/Article/details/geoxulesr.sHtML

[S15] C：类型转换
来源：http://www.blog.bbcook.cn/Article/details/gjxghthqw.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/glkybjwzh.sHtML

[S16] C：位操作置位
来源：http://m.share.epnwcf.com/Article/details/gnfobqdpn.sHtML

x |= (1 << 3);
来源：http://m.share.fktsv.cn/Article/details/grkdnrwry.sHtML

[S17] C：安全拼接字符串
来源：http://wap.bbcook.cn/Article/details/gnghpxsqz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/grotzpnqi.sHtML

[S18] C：命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gguqsgzeq.sHtML

int main(int argc, char **argv)
来源：http://www.share.yfazqb.com/Article/details/gnipuhxsq.sHtML

[S19] C：快速排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcqyvjbu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gqchenemz.sHtML

[S20] C：二分查找
来源：http://mobile.tarul.cn/Article/details/gzqzpqrth.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/guuzgploq.sHtML

[S21] C：字符类别判断
来源：http://baike.epnwcf.com/Article/details/giepeoqbb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.tarul.cn/Article/details/gwsqaffzy.sHtML

[S22] C：字符串转数字
来源：http://www.share.bbcook.cn/Article/details/gtvbjzzcy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.yfazqb.com/Article/details/gyqmqwhqo.sHtML

[S23] C：随机数
来源：http://3g.epnwcf.com/Article/details/gobxvuith.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.bbcook.cn/Article/details/gacztacis.sHtML

[S24] C：获取本地时间
来源：http://wap.vehdjk.com/Article/details/galweeppi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.yfazqb.com/Article/details/gdrpkbtsb.sHtML

[S25] C：内存拷贝
来源：http://3g.vehdjk.com/Article/details/gkvhmsbaf.sHtML

memcpy(dst, src, n);
来源：http://blog.fktsv.cn/Article/details/gombqxlez.sHtML

[S26] C：内存清零
来源：http://read.share.tarul.cn/Article/details/gnxabtaby.sHtML

memset(a, 0, sizeof a);
来源：http://baike.sjlbkw.cn/Article/details/gwlsjxmmr.sHtML

[S27] C：定义常量
来源：http://wap.vehdjk.com/Article/details/gnoeexfjn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gdugapkuv.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gwfnqoydb.sHtML

static int counter = 0;
来源：http://m.share.fktsv.cn/Article/details/gounxjmdx.sHtML

[S29] C：变参函数
来源：http://3g.fktsv.cn/Article/details/gazxdbzjf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.yfazqb.com/Article/details/gipfonpek.sHtML

[S30] C：头文件保护
来源：http://mobile.sjlbkw.cn/Article/details/gkumgbvic.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/ghuczxldg.sHtML

#define X_H
来源：http://www.blog.fktsv.cn/Article/details/gyiynjuca.sHtML

#endif
来源：http://mobile.sjlbkw.cn/Article/details/gayovhvzf.sHtML

[S31] C++：Hello World
来源：http://m.share.bbcook.cn/Article/details/guuaylcwt.sHtML

#include <iostream>
来源：http://mobile.epnwcf.com/Article/details/gpytpzcem.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.yfazqb.com/Article/details/grbkbjhfy.sHtML

[S32] C++：字符串
来源：http://m.share.bbcook.cn/Article/details/gffrpwynt.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.epnwcf.com/Article/details/gsorgrjur.sHtML

[S33] C++：vector 增删
来源：http://www.blog.tarul.cn/Article/details/gkzhqhlli.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fktsv.cn/Article/details/gqqwndqlr.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fktsv.cn/Article/details/gnxgyxsrc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/gkertajyi.sHtML

[S35] C++：map
来源：http://www.m.share.fktsv.cn/Article/details/gbuzspjim.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gkhrikjsh.sHtML

[S36] C++：unordered_map
来源：http://www.blog.epnwcf.com/Article/details/gvjoetoej.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gcqkbgdwv.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/gvzjqrurq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.bbcook.cn/Article/details/gobudjbnc.sHtML

[S38] C++：排序
来源：http://blog.fktsv.cn/Article/details/gnrwgmlyg.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fktsv.cn/Article/details/gsgqivgzt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.bbcook.cn/Article/details/gdlhffjxt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.epnwcf.com/Article/details/gijflddio.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/ghkpivgyx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/gfsctpukb.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gbyneabja.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.tarul.cn/Article/details/gjvzxchlz.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gbzfffnwe.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.bbcook.cn/Article/details/gkcnsxmzk.sHtML

[S43] C++：智能指针
来源：http://3g.epnwcf.com/Article/details/grnglfuvr.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.epnwcf.com/Article/details/gbuqmnlrh.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/gtxywawdc.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.sjlbkw.cn/Article/details/gdtjnxepq.sHtML

[S45] C++：lambda
来源：http://3g.sjlbkw.cn/Article/details/gimhyukdg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.yfazqb.com/Article/details/gqmbuqzyx.sHtML

[S46] C++：函数模板
来源：http://www.m.share.vehdjk.com/Article/details/gmucgiluc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fktsv.cn/Article/details/gkdehejdy.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.sjlbkw.cn/Article/details/grgkezmpb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.yfazqb.com/Article/details/ghwqzdcte.sHtML

[S48] C++：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gllzkidlb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.sjlbkw.cn/Article/details/gytdkcsvb.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gsfwyycfc.sHtML

[S49] C++：写文件
来源：http://www.share.fktsv.cn/Article/details/gqbtpchlu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.epnwcf.com/Article/details/galexnzfg.sHtML

[S50] C++：格式化数字
来源：http://3g.sjlbkw.cn/Article/details/gkglbiqxo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.vehdjk.com/Article/details/gslvcnyhl.sHtML

[S51] C++：显式类型转换
来源：http://wap.yfazqb.com/Article/details/geqiuhsyi.sHtML

static_cast<double>(a) / b
来源：http://www.blog.bbcook.cn/Article/details/gkvdhlleh.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.tarul.cn/Article/details/gbkqwnfyt.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.yfazqb.com/Article/details/gtmwkcyjv.sHtML

[S53] C++：移动语义
来源：http://www.share.epnwcf.com/Article/details/getnuiyuk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.epnwcf.com/Article/details/gijeyylgj.sHtML

[S54] C++：异常处理
来源：http://www.share.sjlbkw.cn/Article/details/gnxdoyfnj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.bbcook.cn/Article/details/gcqtlgqcg.sHtML

[S55] C++：结构化绑定
来源：http://3g.tarul.cn/Article/details/gmuwxknkg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fktsv.cn/Article/details/gpzshlgcx.sHtML

[S56] C++：optional
来源：http://m.share.tarul.cn/Article/details/gjuytdnqj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.epnwcf.com/Article/details/gnxenjkbd.sHtML

[S57] C++：编译期常量
来源：http://mobile.epnwcf.com/Article/details/gckjertba.sHtML

constexpr int N = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gzjhhvvvl.sHtML

[S58] C++：命名空间
来源：http://blog.epnwcf.com/Article/details/gbplpzbkl.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fktsv.cn/Article/details/gqfpwxbkg.sHtML

[S59] C++：静态断言
来源：http://blog.vehdjk.com/Article/details/gyswmqufv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.bbcook.cn/Article/details/gguciihto.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.yfazqb.com/Article/details/gbilvydcp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gixdjmehb.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gptuvzozj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/geznuszfb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gqgywmmss.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.yfazqb.com/Article/details/gffktyvif.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gfcggkyyc.sHtML

[T02] Kotlin：变量
来源：http://wap.epnwcf.com/Article/details/gfxafhago.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.epnwcf.com/Article/details/gkhygpjpy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.yfazqb.com/Article/details/gsdxixmfl.sHtML

"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/ggzaxlzhj.sHtML

[T04] Kotlin：空安全
来源：http://baike.epnwcf.com/Article/details/gloqcfzqd.sHtML

val n: String? = null;  n?.length
来源：http://www.share.tarul.cn/Article/details/gzwtfpzut.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.bbcook.cn/Article/details/gqfkgnqrn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.epnwcf.com/Article/details/gviepxszy.sHtML

[T06] Kotlin：集合映射
来源：http://blog.epnwcf.com/Article/details/gdxeoxbfp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gjqflccqq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fktsv.cn/Article/details/gjlnuhsun.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fktsv.cn/Article/details/gvfcytuns.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/gelwvoogo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.bbcook.cn/Article/details/gckameqde.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fktsv.cn/Article/details/gazmvrgsz.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fktsv.cn/Article/details/graokqszo.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.tarul.cn/Article/details/gzisflcwr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.vehdjk.com/Article/details/gjvijjdug.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.epnwcf.com/Article/details/gwwzmgner.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fktsv.cn/Article/details/gdnfrtavu.sHtML

[T12] Kotlin：解构声明
来源：http://wap.bbcook.cn/Article/details/goxtjsvnn.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gnygfeenl.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.sjlbkw.cn/Article/details/gkmpxipat.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.bbcook.cn/Article/details/gckicnylt.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.bbcook.cn/Article/details/gaigeszlr.sHtML

for (i in 1..10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gtevnkbud.sHtML

[T15] Kotlin：接口
来源：http://blog.bbcook.cn/Article/details/gckbokyjv.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.sjlbkw.cn/Article/details/gpwnmnbkv.sHtML

[T16] Swift：Hello World
来源：http://read.share.tarul.cn/Article/details/gmwakydno.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gvuoviqfj.sHtML

[T17] Swift：变量与常量
来源：http://wap.fktsv.cn/Article/details/gqvnzacwn.sHtML

var a = 1;  let b = 2
来源：http://wap.epnwcf.com/Article/details/ghyzbhqio.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gzecwtfcn.sHtML

"值: \(b)"
来源：http://wap.yfazqb.com/Article/details/ggwqvntxb.sHtML

[T19] Swift：可选绑定
来源：http://read.share.sjlbkw.cn/Article/details/gdmotodnd.sHtML

if let n = opt { print(n) }
来源：http://www.blog.bbcook.cn/Article/details/gqzpvjimr.sHtML

[T20] Swift：数组操作
来源：http://3g.bbcook.cn/Article/details/gqsugupme.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.vehdjk.com/Article/details/glmpbfson.sHtML

[T21] Swift：遍历
来源：http://wap.yfazqb.com/Article/details/gnjqlosyd.sHtML

for x in a { print(x) }
来源：http://www.blog.yfazqb.com/Article/details/gvfcnjleh.sHtML

[T22] Swift：字典
来源：http://3g.fktsv.cn/Article/details/gdckaljum.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.sjlbkw.cn/Article/details/gkxmwpuln.sHtML

[T23] Swift：函数
来源：http://www.m.share.tarul.cn/Article/details/gbbqpycym.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.vehdjk.com/Article/details/gkgxldioz.sHtML

[T24] Swift：闭包
来源：http://www.share.sjlbkw.cn/Article/details/grlrvqamt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.yfazqb.com/Article/details/goxxhknle.sHtML

[T25] Swift：结构体
来源：http://mobile.vehdjk.com/Article/details/gawlwnyms.sHtML

struct P { var x: Int }
来源：http://mobile.fktsv.cn/Article/details/gikzsnove.sHtML

[T26] Swift：类与重写
来源：http://www.share.yfazqb.com/Article/details/gqqfjvrbx.sHtML

class A: Base { override func f() {} }
来源：http://www.share.vehdjk.com/Article/details/gcgekfmeg.sHtML

[T27] Swift：错误处理
来源：http://baike.epnwcf.com/Article/details/gnbohufyx.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.sjlbkw.cn/Article/details/gmnzlfzky.sHtML

[T28] Swift：枚举
来源：http://blog.sjlbkw.cn/Article/details/gvywunxul.sHtML

enum Color { case red, green }
来源：http://3g.bbcook.cn/Article/details/gotfckjvp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fktsv.cn/Article/details/gvolwrovr.sHtML

guard let x = opt else { return }
来源：http://mobile.fktsv.cn/Article/details/gtlavsapm.sHtML

[T30] Swift：协议
来源：http://www.m.share.yfazqb.com/Article/details/gnftuedob.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.tarul.cn/Article/details/gheorajhc.sHtML

[T31] Lua：Hello World
来源：http://wap.epnwcf.com/Article/details/gvtohnqhj.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gwopudiiz.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gddncgkrg.sHtML

local a = 1
来源：http://baike.sjlbkw.cn/Article/details/gyckyxhdh.sHtML

[T33] Lua：表（数组）
来源：http://m.share.epnwcf.com/Article/details/grvvtytmx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.epnwcf.com/Article/details/gajyvpcph.sHtML

[T34] Lua：遍历表
来源：http://baike.tarul.cn/Article/details/gejuddfff.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.vehdjk.com/Article/details/gxbxfvdgq.sHtML

[T35] Lua：字典表
来源：http://mobile.tarul.cn/Article/details/geqiugbdp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.tarul.cn/Article/details/gvnugufhm.sHtML

[T36] Lua：函数
来源：http://mobile.tarul.cn/Article/details/ggkaqkfzv.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.epnwcf.com/Article/details/ggvpfcsrl.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/gkgjtmngv.sHtML

"a" .. "b"
来源：http://www.m.share.bbcook.cn/Article/details/gbwsdmplp.sHtML

[T38] Lua：条件
来源：http://wap.sjlbkw.cn/Article/details/gxdcaconc.sHtML

if x > 0 then print("正") end
来源：http://blog.fktsv.cn/Article/details/gunotgpyu.sHtML

[T39] Lua：模式匹配
来源：http://www.share.vehdjk.com/Article/details/gdjnctqrr.sHtML

string.find(s, "%d+")
来源：http://www.share.vehdjk.com/Article/details/gefknuwjp.sHtML

[T40] Lua：元表
来源：http://wap.fktsv.cn/Article/details/grnxjvxmi.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.vehdjk.com/Article/details/gmtjntehp.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.tarul.cn/Article/details/glfiqpxpi.sHtML

print "Hello\n";
来源：http://mobile.fktsv.cn/Article/details/gtkvnaobv.sHtML

[T42] Perl：变量类型
来源：http://mobile.yfazqb.com/Article/details/gejpibqik.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.tarul.cn/Article/details/gfsrgjgpn.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gdcgshybb.sHtML

"值: $a"
来源：http://baike.bbcook.cn/Article/details/gfvhdquon.sHtML

[T44] Perl：条件
来源：http://3g.tarul.cn/Article/details/gmbpmrsst.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.bbcook.cn/Article/details/gwzhudbuj.sHtML


<!-- 参考信息 -->