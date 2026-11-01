代发 wailian999

cmd >/dev/null 2>&1
来源：http://mobile.epnwcf.com/Article/details/gqnbjxdra.sHtML

[R42] 输入重定向
来源：http://mobile.tarul.cn/Article/details/gkcyvxwnq.sHtML

wc -l < a.txt
来源：http://baike.epnwcf.com/Article/details/gsrvtusnm.sHtML

[R43] 按名字查找文件
来源：http://read.share.fktsv.cn/Article/details/gnlqqjnoi.sHtML

find . -name "*.log" -type f
来源：http://www.share.fktsv.cn/Article/details/gaedqvwst.sHtML

[R44] 按修改时间查找
来源：http://read.share.epnwcf.com/Article/details/gkkahutae.sHtML

find . -mtime -7 -type f
来源：http://mobile.tarul.cn/Article/details/gkinmwufl.sHtML

[R45] 批量删除
来源：http://m.share.yfazqb.com/Article/details/gdketwcqo.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.epnwcf.com/Article/details/gencjzpnt.sHtML

[R46] 递归替换文件内容
来源：http://baike.epnwcf.com/Article/details/gojnxlvee.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.tarul.cn/Article/details/glmufefnj.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/gkkpxkpfl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.bbcook.cn/Article/details/gevslwbce.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/ghwyityap.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fktsv.cn/Article/details/goolrlqop.sHtML

[R49] awk 带条件
来源：http://www.m.share.vehdjk.com/Article/details/gkicyksnm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.epnwcf.com/Article/details/gmunqdodi.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/grctgszcy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gpzunkgfk.sHtML

[R51] 排序去重取前几
来源：http://wap.vehdjk.com/Article/details/grvihmlsg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fktsv.cn/Article/details/gumoptpbt.sHtML

[R52] 统计行数
来源：http://www.share.vehdjk.com/Article/details/gflpdgoba.sHtML

wc -l a.txt
来源：http://www.blog.epnwcf.com/Article/details/garvxjwjx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.tarul.cn/Article/details/gespbaxyt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.bbcook.cn/Article/details/gdeyuyrfx.sHtML

[R54] 比较两个文件
来源：http://m.share.fktsv.cn/Article/details/gzjhjkwzm.sHtML

diff a.txt b.txt
来源：http://3g.epnwcf.com/Article/details/ggzzhhhee.sHtML

[R55] 压缩与解压
来源：http://www.share.fktsv.cn/Article/details/gpkszlvep.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.yfazqb.com/Article/details/grgccbuas.sHtML

[R56] 远程拷贝
来源：http://read.share.vehdjk.com/Article/details/gopojjebn.sHtML

scp file user@host:/path/
来源：http://mobile.tarul.cn/Article/details/gtmshzejt.sHtML

[R57] 远程执行命令
来源：http://baike.yfazqb.com/Article/details/gjcxrucpv.sHtML

ssh user@host 'uptime'
来源：http://www.share.fktsv.cn/Article/details/gnklumvfd.sHtML

[R58] 下载文件
来源：http://3g.tarul.cn/Article/details/gyuwbleiy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.bbcook.cn/Article/details/gberxqocd.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gtujmpydc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.vehdjk.com/Article/details/gvptvamgr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gwywjirnn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.epnwcf.com/Article/details/gkzaxmvlu.sHtML

[R61] 磁盘占用
来源：http://blog.epnwcf.com/Article/details/gcwrjqhmf.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/gycvjvmqg.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.vehdjk.com/Article/details/gnkqsfupm.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.tarul.cn/Article/details/gprccuvij.sHtML

[R63] 内存与进程
来源：http://m.share.sjlbkw.cn/Article/details/gxtmcozvt.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.bbcook.cn/Article/details/gnagrshsu.sHtML

[R64] 结束进程
来源：http://www.share.sjlbkw.cn/Article/details/gvxhkjpop.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/gwigprace.sHtML

[R65] 查看端口占用
来源：http://m.share.yfazqb.com/Article/details/gmnpaiuqp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.vehdjk.com/Article/details/ghbnktgdm.sHtML

[R66] 定时任务
来源：http://m.share.vehdjk.com/Article/details/gxlzlxkke.sHtML

crontab -e;  crontab -l
来源：http://blog.tarul.cn/Article/details/gsflzknue.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.sjlbkw.cn/Article/details/gdcxlphho.sHtML

openssl rand -hex 16
来源：http://m.share.yfazqb.com/Article/details/ggrjamzxp.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/giphzeppl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.tarul.cn/Article/details/gkuouxgmk.sHtML

[R69] 生成随机密码
来源：http://wap.fktsv.cn/Article/details/gaxfflfrc.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.sjlbkw.cn/Article/details/gkzlqaozx.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fktsv.cn/Article/details/gnnamapiz.sHtML

date +%s;  date -d @1700000000
来源：http://baike.vehdjk.com/Article/details/gmnsvatgu.sHtML

[R71] 日期格式化
来源：http://blog.fktsv.cn/Article/details/giozmvixg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/guplsisyb.sHtML

[R72] 等待端口就绪
来源：http://3g.tarul.cn/Article/details/gntfptnnu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gybnhsfjj.sHtML

[R73] 分割大日志
来源：http://www.share.sjlbkw.cn/Article/details/glzkjhlpq.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/ggovmnuxg.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/glesojngf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.tarul.cn/Article/details/gisarsvvo.sHtML

[R75] 导出环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/gqouutumu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.yfazqb.com/Article/details/gtzekkvgb.sHtML

[R76] 使用临时文件
来源：http://baike.vehdjk.com/Article/details/giuuivuoq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gmhxpscsr.sHtML

[R77] 读取用户输入
来源：http://wap.epnwcf.com/Article/details/glsgahxed.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.bbcook.cn/Article/details/gyaszfvvv.sHtML

[R78] 交互式菜单
来源：http://blog.yfazqb.com/Article/details/gaieghzaz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.bbcook.cn/Article/details/gfafhcmta.sHtML

[R79] 解析命令行选项
来源：http://blog.yfazqb.com/Article/details/gtqlxxrjo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/gclumejtq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.tarul.cn/Article/details/grlpwtdoi.sHtML

time ./run.sh
来源：http://m.share.sjlbkw.cn/Article/details/gherljwkz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gacmvpuus.sHtML

S. C / C++ 专题
来源：http://m.share.bbcook.cn/Article/details/ghrhbipsk.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gvizrpmbf.sHtML

[S01] C：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gixvfsqzl.sHtML

#include <stdio.h>
来源：http://wap.fktsv.cn/Article/details/gemvyfxol.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.sjlbkw.cn/Article/details/gfsmbptea.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.bbcook.cn/Article/details/giwrizhpr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.tarul.cn/Article/details/gpjcqmtva.sHtML

[S03] C：读入整数
来源：http://www.share.yfazqb.com/Article/details/grvsdsqwq.sHtML

int x; scanf("%d", &x);
来源：http://m.share.sjlbkw.cn/Article/details/gaxoepjeg.sHtML

[S04] C：字符串复制
来源：http://read.share.tarul.cn/Article/details/gojztmene.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.epnwcf.com/Article/details/gkkbedhsa.sHtML

[S05] C：字符串长度
来源：http://m.share.yfazqb.com/Article/details/gonmfdzms.sHtML

strlen(s)
来源：http://mobile.fktsv.cn/Article/details/gjdiayeam.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gekfosnki.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gjlzekxci.sHtML

[S07] C：数组遍历求和
来源：http://blog.vehdjk.com/Article/details/gqtcbipoc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.bbcook.cn/Article/details/gqymnqtpv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.yfazqb.com/Article/details/gjeydxdth.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.bbcook.cn/Article/details/ghudytkmc.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.sjlbkw.cn/Article/details/ggaotuqhu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fktsv.cn/Article/details/gkvjlszaa.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gufdkrwum.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.yfazqb.com/Article/details/gxgjwdumi.sHtML

[S11] C：逐行读文件
来源：http://blog.tarul.cn/Article/details/glzqjvfgd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.yfazqb.com/Article/details/gbwdocxra.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/gnfbrkfoj.sHtML

fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gzbqjrfsf.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gusrwkntf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.bbcook.cn/Article/details/gbyzvqmpn.sHtML

[S13] C：宏定义
来源：http://3g.sjlbkw.cn/Article/details/gvuehmdvi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fktsv.cn/Article/details/goiihxwgk.sHtML

[S14] C：枚举
来源：http://www.blog.vehdjk.com/Article/details/gbpwerpnv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.vehdjk.com/Article/details/gxunbzcbd.sHtML

[S15] C：类型转换
来源：http://read.share.yfazqb.com/Article/details/gbckatfyv.sHtML

(double) a / b
来源：http://www.share.yfazqb.com/Article/details/govoeuand.sHtML

[S16] C：位操作置位
来源：http://mobile.vehdjk.com/Article/details/gnbsecazu.sHtML

x |= (1 << 3);
来源：http://blog.tarul.cn/Article/details/gqcovtkht.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gaioeunnh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/ghaswmrix.sHtML

[S18] C：命令行参数
来源：http://blog.vehdjk.com/Article/details/gcenbbmyn.sHtML

int main(int argc, char **argv)
来源：http://mobile.fktsv.cn/Article/details/gjbwatnzd.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/ghsbnkevl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gbfswokqb.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gszmmiflr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gimvziqxm.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/gqqmfkkja.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.epnwcf.com/Article/details/gzbyvqmxu.sHtML

[S22] C：字符串转数字
来源：http://blog.fktsv.cn/Article/details/goqgayizo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/gjpodpwqr.sHtML

[S23] C：随机数
来源：http://read.share.yfazqb.com/Article/details/gybcsxgmz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/gzfemlfpm.sHtML

[S24] C：获取本地时间
来源：http://www.share.tarul.cn/Article/details/gjozegzdl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.tarul.cn/Article/details/gpxcdsrzt.sHtML

[S25] C：内存拷贝
来源：http://blog.tarul.cn/Article/details/gdnmoarkr.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.bbcook.cn/Article/details/gznabdcoc.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gtrsuhhne.sHtML

memset(a, 0, sizeof a);
来源：http://3g.vehdjk.com/Article/details/gbngkdfim.sHtML

[S27] C：定义常量
来源：http://www.share.yfazqb.com/Article/details/gvgwxffin.sHtML

const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gmepflamt.sHtML

[S28] C：静态变量
来源：http://blog.tarul.cn/Article/details/grenvukyk.sHtML

static int counter = 0;
来源：http://3g.sjlbkw.cn/Article/details/gulxlnewj.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/gynbcjtwv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/grtswzrpm.sHtML

[S30] C：头文件保护
来源：http://read.share.tarul.cn/Article/details/giewrpslk.sHtML

#ifndef X_H
来源：http://mobile.epnwcf.com/Article/details/gybuwbxvu.sHtML

#define X_H
来源：http://baike.yfazqb.com/Article/details/gngkfnnfc.sHtML

#endif
来源：http://www.blog.tarul.cn/Article/details/gxyhoenhl.sHtML

[S31] C++：Hello World
来源：http://blog.vehdjk.com/Article/details/gvcldpwyu.sHtML

#include <iostream>
来源：http://www.blog.sjlbkw.cn/Article/details/glmydqemj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fktsv.cn/Article/details/ggwohidlw.sHtML

[S32] C++：字符串
来源：http://www.share.epnwcf.com/Article/details/gayljxgjd.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.bbcook.cn/Article/details/gqxrnjzks.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.sjlbkw.cn/Article/details/gvekzhlrv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.epnwcf.com/Article/details/gwhhpberd.sHtML

[S34] C++：遍历 vector
来源：http://mobile.epnwcf.com/Article/details/gjtvfymat.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.yfazqb.com/Article/details/gqktwghoe.sHtML

[S35] C++：map
来源：http://mobile.fktsv.cn/Article/details/gbrzhbzvz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/grgwrgkrn.sHtML

[S36] C++：unordered_map
来源：http://www.blog.tarul.cn/Article/details/guqmxtsxg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gywjlrhec.sHtML

[S37] C++：set
来源：http://wap.sjlbkw.cn/Article/details/guhwjvnzg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.yfazqb.com/Article/details/gojhrkrch.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gmmlenwzl.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fktsv.cn/Article/details/ggvwqwyeo.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.vehdjk.com/Article/details/gxurjbddi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.vehdjk.com/Article/details/gqapcrpnn.sHtML

[S40] C++：查找元素
来源：http://mobile.sjlbkw.cn/Article/details/gpjbnsluq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.bbcook.cn/Article/details/glunbuwdj.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gemeiabee.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.vehdjk.com/Article/details/gqirkrbmv.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.sjlbkw.cn/Article/details/gmjowbshk.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fktsv.cn/Article/details/gchfwmonh.sHtML

[S43] C++：智能指针
来源：http://www.share.bbcook.cn/Article/details/gffrtdods.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.sjlbkw.cn/Article/details/gbbexbvjh.sHtML

[S44] C++：引用传参
来源：http://www.share.fktsv.cn/Article/details/gdtzudhii.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.tarul.cn/Article/details/gxrxczifq.sHtML

[S45] C++：lambda
来源：http://www.share.vehdjk.com/Article/details/gtuautnjt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.yfazqb.com/Article/details/glumkvfak.sHtML

[S46] C++：函数模板
来源：http://wap.tarul.cn/Article/details/gnlzgndqm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.bbcook.cn/Article/details/glqibsrfz.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.sjlbkw.cn/Article/details/gxscqladp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.yfazqb.com/Article/details/gkuguvhnw.sHtML

[S48] C++：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gpepwqfvj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.vehdjk.com/Article/details/gjnwiqvwq.sHtML

while (std::getline(in, line)) { }
来源：http://blog.tarul.cn/Article/details/gcrrmowkb.sHtML

[S49] C++：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/gniuixmhc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.yfazqb.com/Article/details/gmafgnhql.sHtML

[S50] C++：格式化数字
来源：http://baike.yfazqb.com/Article/details/glutrhmvi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fktsv.cn/Article/details/gzgkblcwn.sHtML

[S51] C++：显式类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gfyzoykfn.sHtML

static_cast<double>(a) / b
来源：http://blog.bbcook.cn/Article/details/gomakncmp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.vehdjk.com/Article/details/gxwxqkdtx.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.bbcook.cn/Article/details/glkiswnpy.sHtML

[S53] C++：移动语义
来源：http://www.share.yfazqb.com/Article/details/gnefmwznh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fktsv.cn/Article/details/gnxjknspu.sHtML

[S54] C++：异常处理
来源：http://baike.vehdjk.com/Article/details/gxcsdiodu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/gririjvoe.sHtML

[S55] C++：结构化绑定
来源：http://baike.yfazqb.com/Article/details/gpvwzanjp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.tarul.cn/Article/details/gnyzjrcfk.sHtML

[S56] C++：optional
来源：http://baike.vehdjk.com/Article/details/gjkjlfssn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/gqoigyzer.sHtML

[S57] C++：编译期常量
来源：http://mobile.epnwcf.com/Article/details/grvwcgwyg.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/glsktzcwu.sHtML

[S58] C++：命名空间
来源：http://3g.fktsv.cn/Article/details/ggwuwhkwr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.bbcook.cn/Article/details/gwwwhuciu.sHtML

[S59] C++：静态断言
来源：http://mobile.epnwcf.com/Article/details/gevjgbjrr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.sjlbkw.cn/Article/details/ghsuuumrr.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.sjlbkw.cn/Article/details/gnnzbxkhn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/gipktrhtj.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbtbbzsiv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.epnwcf.com/Article/details/gfufccyaq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtbgxnuxh.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gxdjigbjn.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/geppcjmbx.sHtML

[T02] Kotlin：变量
来源：http://3g.tarul.cn/Article/details/gvlzsnrcb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.yfazqb.com/Article/details/gmxwfkbpr.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.vehdjk.com/Article/details/ggxzjeyyv.sHtML

"值: $b"
来源：http://www.share.yfazqb.com/Article/details/gsmkpqnxs.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gmgtkhaaq.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.tarul.cn/Article/details/gqmtxvtir.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/gfsepwqwa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fktsv.cn/Article/details/gdmxnaywv.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.tarul.cn/Article/details/gcfcyhilu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fktsv.cn/Article/details/gznpmcahu.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.yfazqb.com/Article/details/gtpprvdaz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.tarul.cn/Article/details/gpeujshwx.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.yfazqb.com/Article/details/getezpotn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gmwidqrkj.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.sjlbkw.cn/Article/details/gimocisat.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.bbcook.cn/Article/details/gvdeeiqmz.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gjvokjvju.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/gosmlkkxh.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fktsv.cn/Article/details/gutjipagu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.vehdjk.com/Article/details/gnjaaltro.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fktsv.cn/Article/details/gwmrwtrsw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/ggmuyatpz.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.epnwcf.com/Article/details/gyzkhybue.sHtML

val m = mapOf("a" to 1)
来源：http://wap.tarul.cn/Article/details/gqeodjiqe.sHtML

[T14] Kotlin：循环
来源：http://baike.epnwcf.com/Article/details/gzoxppyxw.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/gfrxyitpq.sHtML

[T15] Kotlin：接口
来源：http://3g.sjlbkw.cn/Article/details/gvcjxsvlb.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gvvxpgpxp.sHtML

[T16] Swift：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gwexqzesj.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gpllmxcss.sHtML

[T17] Swift：变量与常量
来源：http://m.share.sjlbkw.cn/Article/details/gvdnjknnn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.epnwcf.com/Article/details/glbmuwvkw.sHtML

[T18] Swift：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/ghauvoatb.sHtML

"值: \(b)"
来源：http://www.share.fktsv.cn/Article/details/gmlellsxa.sHtML

[T19] Swift：可选绑定
来源：http://read.share.vehdjk.com/Article/details/gfobibvql.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/gjgrxxfuw.sHtML

[T20] Swift：数组操作
来源：http://www.blog.yfazqb.com/Article/details/gqluxagfp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/gstawtsfz.sHtML

[T21] Swift：遍历
来源：http://baike.tarul.cn/Article/details/gxqmcbuai.sHtML

for x in a { print(x) }
来源：http://blog.yfazqb.com/Article/details/gvncqglws.sHtML

[T22] Swift：字典
来源：http://m.share.fktsv.cn/Article/details/gqmkuwwai.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fktsv.cn/Article/details/gijzgcjds.sHtML

[T23] Swift：函数
来源：http://read.share.epnwcf.com/Article/details/gkonsfdfy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.bbcook.cn/Article/details/gtcxyxfxt.sHtML

[T24] Swift：闭包
来源：http://3g.tarul.cn/Article/details/guivmdrld.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/ggzyslyie.sHtML

[T25] Swift：结构体
来源：http://baike.yfazqb.com/Article/details/gvcyusfly.sHtML

struct P { var x: Int }
来源：http://www.m.share.yfazqb.com/Article/details/gxfpkuket.sHtML

[T26] Swift：类与重写
来源：http://read.share.vehdjk.com/Article/details/gauxwpgge.sHtML

class A: Base { override func f() {} }
来源：http://wap.yfazqb.com/Article/details/gclqfldzt.sHtML

[T27] Swift：错误处理
来源：http://www.blog.epnwcf.com/Article/details/gstlojggd.sHtML

do { try f() } catch { print(error) }
来源：http://blog.tarul.cn/Article/details/gwkfwlbwr.sHtML

[T28] Swift：枚举
来源：http://m.share.tarul.cn/Article/details/gnwvgzcgt.sHtML

enum Color { case red, green }
来源：http://read.share.yfazqb.com/Article/details/gjqmygyog.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.bbcook.cn/Article/details/gauxbjysx.sHtML

guard let x = opt else { return }
来源：http://wap.fktsv.cn/Article/details/gcqpwagan.sHtML

[T30] Swift：协议
来源：http://www.m.share.tarul.cn/Article/details/gxgvuiiya.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.epnwcf.com/Article/details/gxjbrtxtw.sHtML

[T31] Lua：Hello World
来源：http://wap.yfazqb.com/Article/details/gwwkdthov.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gpuedezkc.sHtML

[T32] Lua：局部变量
来源：http://m.share.bbcook.cn/Article/details/gyxjebzru.sHtML

local a = 1
来源：http://m.share.epnwcf.com/Article/details/glwrrbenn.sHtML

[T33] Lua：表（数组）
来源：http://m.share.sjlbkw.cn/Article/details/gneaaloia.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.bbcook.cn/Article/details/gynaobgqv.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fktsv.cn/Article/details/gmfzfagtt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.epnwcf.com/Article/details/gqyewptpl.sHtML

[T35] Lua：字典表
来源：http://blog.vehdjk.com/Article/details/ghlshpnhl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.bbcook.cn/Article/details/gqilaciht.sHtML

[T36] Lua：函数
来源：http://3g.bbcook.cn/Article/details/gitqhygcj.sHtML

function add(a, b) return a + b end
来源：http://www.blog.bbcook.cn/Article/details/gqjpcnsqo.sHtML

[T37] Lua：字符串拼接
来源：http://3g.vehdjk.com/Article/details/geyyxlzqt.sHtML

"a" .. "b"
来源：http://read.share.vehdjk.com/Article/details/gjpbjlevl.sHtML

[T38] Lua：条件
来源：http://3g.sjlbkw.cn/Article/details/gzeumvory.sHtML

if x > 0 then print("正") end
来源：http://3g.epnwcf.com/Article/details/gpyasyqnb.sHtML

[T39] Lua：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/grgbjhlmg.sHtML

string.find(s, "%d+")
来源：http://www.blog.bbcook.cn/Article/details/ghrfgyggx.sHtML

[T40] Lua：元表
来源：http://www.share.epnwcf.com/Article/details/gvftzdexs.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.bbcook.cn/Article/details/gyeubwjly.sHtML

[T41] Perl：Hello World
来源：http://www.share.fktsv.cn/Article/details/gmhciuvdc.sHtML

print "Hello\n";
来源：http://www.blog.vehdjk.com/Article/details/gnoaqwbmg.sHtML

[T42] Perl：变量类型
来源：http://www.share.vehdjk.com/Article/details/glipszffq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.bbcook.cn/Article/details/gwsqfaizu.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gwvyhdgma.sHtML

"值: $a"
来源：http://www.blog.fktsv.cn/Article/details/gyzfglzdj.sHtML

[T44] Perl：条件
来源：http://wap.epnwcf.com/Article/details/gwbljfnql.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.tarul.cn/Article/details/gdbwixpax.sHtML


<!-- 参考信息 -->