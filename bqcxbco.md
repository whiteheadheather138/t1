代发 wailian999

cmd >/dev/null 2>&1
来源：http://blog.fktsv.cn/Article/details/gxcihlshz.sHtML

[R42] 输入重定向
来源：http://m.share.sjlbkw.cn/Article/details/gqzpljncy.sHtML

wc -l < a.txt
来源：http://www.share.vehdjk.com/Article/details/gvqnvqmzl.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.yfazqb.com/Article/details/gvoldvtuy.sHtML

find . -name "*.log" -type f
来源：http://www.share.epnwcf.com/Article/details/gnjzjdubb.sHtML

[R44] 按修改时间查找
来源：http://m.share.fktsv.cn/Article/details/gkqysnnjf.sHtML

find . -mtime -7 -type f
来源：http://www.share.fktsv.cn/Article/details/gswtiwxbu.sHtML

[R45] 批量删除
来源：http://wap.vehdjk.com/Article/details/guaokyjxo.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.bbcook.cn/Article/details/gcooljygu.sHtML

[R46] 递归替换文件内容
来源：http://blog.tarul.cn/Article/details/gudttkxyr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.sjlbkw.cn/Article/details/gsjaugasw.sHtML

[R47] sed 单行替换
来源：http://wap.vehdjk.com/Article/details/gtxisruww.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.yfazqb.com/Article/details/gfnknyqio.sHtML

[R48] awk 取指定列
来源：http://read.share.sjlbkw.cn/Article/details/gefhvvimo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gtgobykju.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/gpucrvhcv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fktsv.cn/Article/details/gsdlcfiyd.sHtML

[R50] awk 求和
来源：http://www.share.tarul.cn/Article/details/gbwiuxpid.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.epnwcf.com/Article/details/gtpetfpdv.sHtML

[R51] 排序去重取前几
来源：http://www.share.yfazqb.com/Article/details/gazkceogh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.yfazqb.com/Article/details/glvibylog.sHtML

[R52] 统计行数
来源：http://wap.yfazqb.com/Article/details/gsbehcqgl.sHtML

wc -l a.txt
来源：http://read.share.tarul.cn/Article/details/gqvplozlq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/gskvwjxbn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.yfazqb.com/Article/details/gqkxxgntt.sHtML

[R54] 比较两个文件
来源：http://www.m.share.vehdjk.com/Article/details/gducniudm.sHtML

diff a.txt b.txt
来源：http://wap.tarul.cn/Article/details/ghjrvxeta.sHtML

[R55] 压缩与解压
来源：http://blog.tarul.cn/Article/details/ggyguuwvs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gsqkgbcwu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gosstjudz.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/gdjkplzux.sHtML

[R57] 远程执行命令
来源：http://m.share.fktsv.cn/Article/details/gzzwtndoa.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/gnliiplfc.sHtML

[R58] 下载文件
来源：http://3g.fktsv.cn/Article/details/glsasbxvq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.yfazqb.com/Article/details/ghwtntthh.sHtML

[R59] 发 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gsdlmmbic.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.bbcook.cn/Article/details/gjabhfrkf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gkscvkdic.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.epnwcf.com/Article/details/gjsmiaksk.sHtML

[R61] 磁盘占用
来源：http://www.m.share.yfazqb.com/Article/details/ghmadrztw.sHtML

df -h;  du -sh *
来源：http://baike.fktsv.cn/Article/details/gxeyqfusy.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/gzwysnaqy.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.sjlbkw.cn/Article/details/gcrwqzhpl.sHtML

[R63] 内存与进程
来源：http://3g.yfazqb.com/Article/details/gartjmilv.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.yfazqb.com/Article/details/gczbdtlbs.sHtML

[R64] 结束进程
来源：http://blog.fktsv.cn/Article/details/glidnozbo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.bbcook.cn/Article/details/gkwaeqobz.sHtML

[R65] 查看端口占用
来源：http://www.share.yfazqb.com/Article/details/gmlqrhpyp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gakzatcdl.sHtML

[R66] 定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/gsrnqteso.sHtML

crontab -e;  crontab -l
来源：http://baike.epnwcf.com/Article/details/gqduyvqsv.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/gztlwqchp.sHtML

openssl rand -hex 16
来源：http://3g.vehdjk.com/Article/details/gcenzqfro.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/gknlusirl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/gsljtvchj.sHtML

[R69] 生成随机密码
来源：http://wap.sjlbkw.cn/Article/details/gtqyzqlox.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.epnwcf.com/Article/details/gaafmkwhg.sHtML

[R70] 时间戳与互转
来源：http://read.share.tarul.cn/Article/details/gpsauhdnl.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fktsv.cn/Article/details/gcgekbbjz.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gvxbnghqf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.sjlbkw.cn/Article/details/gxotzmwlf.sHtML

[R72] 等待端口就绪
来源：http://www.share.sjlbkw.cn/Article/details/gvajaoezi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/gdwfrmnak.sHtML

[R73] 分割大日志
来源：http://m.share.bbcook.cn/Article/details/gilsmamtl.sHtML

split -l 1000 big.log part_
来源：http://m.share.sjlbkw.cn/Article/details/gxdbnruvo.sHtML

[R74] 批量重命名
来源：http://www.share.fktsv.cn/Article/details/gqgwjgndh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.vehdjk.com/Article/details/gbwyuuveo.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/ghdxyvyjr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.yfazqb.com/Article/details/gfhgpxlst.sHtML

[R76] 使用临时文件
来源：http://www.share.vehdjk.com/Article/details/gawwtxrjg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gblusmsdr.sHtML

[R77] 读取用户输入
来源：http://mobile.bbcook.cn/Article/details/gyuwirkmc.sHtML

read -rp "请输入: " ans
来源：http://wap.tarul.cn/Article/details/gkugvrpyh.sHtML

[R78] 交互式菜单
来源：http://mobile.fktsv.cn/Article/details/gpfxkjbax.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/ghrlpgpqy.sHtML

[R79] 解析命令行选项
来源：http://3g.epnwcf.com/Article/details/gshliyhyg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.sjlbkw.cn/Article/details/givkntgyn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.sjlbkw.cn/Article/details/gaxrpnmmy.sHtML

time ./run.sh
来源：http://wap.fktsv.cn/Article/details/gjayidmsr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gprzdapnm.sHtML

S. C / C++ 专题
来源：http://baike.fktsv.cn/Article/details/gflksifxb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gapgqblbt.sHtML

[S01] C：Hello World
来源：http://wap.epnwcf.com/Article/details/gnvfklvdn.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/gzkmeacxr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.sjlbkw.cn/Article/details/gdfxlqhuv.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.vehdjk.com/Article/details/gaovcczia.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.yfazqb.com/Article/details/gxusxsyfj.sHtML

[S03] C：读入整数
来源：http://www.m.share.sjlbkw.cn/Article/details/gahdmdbws.sHtML

int x; scanf("%d", &x);
来源：http://wap.bbcook.cn/Article/details/gdfzirhds.sHtML

[S04] C：字符串复制
来源：http://www.m.share.vehdjk.com/Article/details/gluiybagt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/gxucjizbl.sHtML

[S05] C：字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/ggerqurhs.sHtML

strlen(s)
来源：http://www.share.vehdjk.com/Article/details/gpnfpmleb.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/gbcwetjli.sHtML

strcmp(a, b) == 0
来源：http://mobile.yfazqb.com/Article/details/gnrrcuqxd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.epnwcf.com/Article/details/grkrviuvo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.vehdjk.com/Article/details/gphzfaxmz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.yfazqb.com/Article/details/gwkdphvzv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.tarul.cn/Article/details/giolopzfm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.vehdjk.com/Article/details/gbfqdtice.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.sjlbkw.cn/Article/details/ggbjqyaez.sHtML

[S10] C：指针与解引用
来源：http://www.blog.tarul.cn/Article/details/gwofzvbel.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fktsv.cn/Article/details/glziuqijg.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/glztflejd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.bbcook.cn/Article/details/gslgfjjiz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.bbcook.cn/Article/details/gkmwtxsxa.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/glegqeglk.sHtML

[S12] C：写文件
来源：http://read.share.bbcook.cn/Article/details/ghwuudtqu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.bbcook.cn/Article/details/ghtlnpmmz.sHtML

[S13] C：宏定义
来源：http://m.share.epnwcf.com/Article/details/ghubyshot.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.bbcook.cn/Article/details/ghqzqlcsf.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/giyokzmez.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.bbcook.cn/Article/details/gwyrexmtw.sHtML

[S15] C：类型转换
来源：http://blog.yfazqb.com/Article/details/gedlqxubd.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/gixydhnzp.sHtML

[S16] C：位操作置位
来源：http://blog.epnwcf.com/Article/details/gpjtcndrl.sHtML

x |= (1 << 3);
来源：http://blog.epnwcf.com/Article/details/gjytmaree.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fktsv.cn/Article/details/grqnkctxw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/gbkmyoipr.sHtML

[S18] C：命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gpzebbjna.sHtML

int main(int argc, char **argv)
来源：http://mobile.sjlbkw.cn/Article/details/gbrjbckrk.sHtML

[S19] C：快速排序
来源：http://m.share.tarul.cn/Article/details/gfkiwlfqp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/garguwdij.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/ghsbswkye.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gjfnadldr.sHtML

[S21] C：字符类别判断
来源：http://mobile.vehdjk.com/Article/details/ghinaevrm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.vehdjk.com/Article/details/gzikjzizk.sHtML

[S22] C：字符串转数字
来源：http://wap.bbcook.cn/Article/details/glgpvorqx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/gmnniwmil.sHtML

[S23] C：随机数
来源：http://www.blog.tarul.cn/Article/details/gaktilheg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/gpsqtqbgo.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/gnpfczqpc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fktsv.cn/Article/details/galurcfhi.sHtML

[S25] C：内存拷贝
来源：http://3g.sjlbkw.cn/Article/details/gskdkpqdx.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/guggwejjz.sHtML

[S26] C：内存清零
来源：http://wap.fktsv.cn/Article/details/gzftvfgwm.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fktsv.cn/Article/details/gfwpoypxg.sHtML

[S27] C：定义常量
来源：http://www.blog.sjlbkw.cn/Article/details/giigsstrx.sHtML

const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/ghacjnpxk.sHtML

[S28] C：静态变量
来源：http://blog.yfazqb.com/Article/details/gdviagncx.sHtML

static int counter = 0;
来源：http://read.share.sjlbkw.cn/Article/details/gxhtwzvnl.sHtML

[S29] C：变参函数
来源：http://www.share.sjlbkw.cn/Article/details/gnjtiktkd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.bbcook.cn/Article/details/gifdlzgsh.sHtML

[S30] C：头文件保护
来源：http://read.share.vehdjk.com/Article/details/gkycxqnfj.sHtML

#ifndef X_H
来源：http://3g.tarul.cn/Article/details/gydjgprwd.sHtML

#define X_H
来源：http://www.blog.epnwcf.com/Article/details/gihylxkse.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/gmfkzcceg.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/gopwcitst.sHtML

#include <iostream>
来源：http://wap.sjlbkw.cn/Article/details/gmheivduf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.bbcook.cn/Article/details/gwtbqttpf.sHtML

[S32] C++：字符串
来源：http://read.share.yfazqb.com/Article/details/gkznvcpqq.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/gapvewuud.sHtML

[S33] C++：vector 增删
来源：http://wap.epnwcf.com/Article/details/ghnfrxtup.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.vehdjk.com/Article/details/gaghrghxw.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fktsv.cn/Article/details/gtgiehiei.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.sjlbkw.cn/Article/details/guzazqhqz.sHtML

[S35] C++：map
来源：http://wap.fktsv.cn/Article/details/gnzbzeeqx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/ganeavmmf.sHtML

[S36] C++：unordered_map
来源：http://wap.tarul.cn/Article/details/gbzfpaekd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gwvsxofuv.sHtML

[S37] C++：set
来源：http://www.blog.fktsv.cn/Article/details/gnswawuyh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.epnwcf.com/Article/details/guewyyzwo.sHtML

[S38] C++：排序
来源：http://www.m.share.vehdjk.com/Article/details/gyplmgxbs.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.epnwcf.com/Article/details/gzltxnban.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fktsv.cn/Article/details/gfthnqptk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.tarul.cn/Article/details/gtoeoqbhf.sHtML

[S40] C++：查找元素
来源：http://mobile.tarul.cn/Article/details/gwohdhsfy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.vehdjk.com/Article/details/ghwavxyqp.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/gxblsuflz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fktsv.cn/Article/details/gnynxzgpq.sHtML

[S42] C++：继承与虚函数
来源：http://blog.vehdjk.com/Article/details/gpixxrdzf.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.bbcook.cn/Article/details/ggazrlohy.sHtML

[S43] C++：智能指针
来源：http://baike.sjlbkw.cn/Article/details/guetcebyv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.tarul.cn/Article/details/gjwcyuyun.sHtML

[S44] C++：引用传参
来源：http://www.share.epnwcf.com/Article/details/gqygsiesa.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzumwvtjc.sHtML

[S45] C++：lambda
来源：http://www.blog.tarul.cn/Article/details/gfmmnwyod.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.vehdjk.com/Article/details/goztjvtef.sHtML

[S46] C++：函数模板
来源：http://www.m.share.tarul.cn/Article/details/gyndscnuo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.tarul.cn/Article/details/gxbcizhut.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.yfazqb.com/Article/details/gmxsandyf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grbuxqdtl.sHtML

[S48] C++：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gkhzjmaid.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.vehdjk.com/Article/details/gkltxynaa.sHtML

while (std::getline(in, line)) { }
来源：http://baike.tarul.cn/Article/details/gggocqmay.sHtML

[S49] C++：写文件
来源：http://read.share.vehdjk.com/Article/details/ghnllqlop.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/gdgdgbebb.sHtML

[S50] C++：格式化数字
来源：http://3g.epnwcf.com/Article/details/ggpaiyngk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gvbiyjzsg.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fktsv.cn/Article/details/glouowaac.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/ggbsbiezc.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.tarul.cn/Article/details/ggnfmrrbs.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.epnwcf.com/Article/details/gprievplh.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/gvaaaczqv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.vehdjk.com/Article/details/gbkhwmhti.sHtML

[S54] C++：异常处理
来源：http://www.m.share.epnwcf.com/Article/details/gjivbcxrs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.yfazqb.com/Article/details/gykawqjug.sHtML

[S55] C++：结构化绑定
来源：http://www.share.vehdjk.com/Article/details/glmhjsvdt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.vehdjk.com/Article/details/glxhltwpr.sHtML

[S56] C++：optional
来源：http://baike.epnwcf.com/Article/details/giyggcpur.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.vehdjk.com/Article/details/geuegfluf.sHtML

[S57] C++：编译期常量
来源：http://www.blog.bbcook.cn/Article/details/girkuxiyk.sHtML

constexpr int N = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gprfeyarq.sHtML

[S58] C++：命名空间
来源：http://www.share.bbcook.cn/Article/details/gwtjgsvwz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fktsv.cn/Article/details/gwmneoiwh.sHtML

[S59] C++：静态断言
来源：http://mobile.yfazqb.com/Article/details/gvrwcwzct.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.yfazqb.com/Article/details/gaflimomn.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.tarul.cn/Article/details/gcgbkplch.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fktsv.cn/Article/details/gtxuxfimy.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzbepghaa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.vehdjk.com/Article/details/gstowpevl.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gplgzuhjp.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.yfazqb.com/Article/details/gqsqmdbve.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/grhsghyvi.sHtML

[T02] Kotlin：变量
来源：http://www.share.bbcook.cn/Article/details/gmrhcwwpo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.tarul.cn/Article/details/gqpbqrzct.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fktsv.cn/Article/details/ggdkgugdf.sHtML

"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/ggwpxiglb.sHtML

[T04] Kotlin：空安全
来源：http://read.share.sjlbkw.cn/Article/details/gvlaryqdz.sHtML

val n: String? = null;  n?.length
来源：http://blog.fktsv.cn/Article/details/gwmexmfpw.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.tarul.cn/Article/details/gbvbrgfuo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.vehdjk.com/Article/details/gatziubox.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fktsv.cn/Article/details/gapsipzmb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.tarul.cn/Article/details/gxeygdrcs.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.tarul.cn/Article/details/gdhmrrwtn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.epnwcf.com/Article/details/gnytpqodu.sHtML

[T08] Kotlin：数据类
来源：http://mobile.vehdjk.com/Article/details/gopvswadn.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.vehdjk.com/Article/details/gsblyxywi.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.bbcook.cn/Article/details/gyjwymrtx.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.yfazqb.com/Article/details/goerxayat.sHtML

[T10] Kotlin：默认参数
来源：http://wap.sjlbkw.cn/Article/details/grvkdfuyi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/gealcrdgz.sHtML

[T11] Kotlin：协程
来源：http://blog.vehdjk.com/Article/details/giqygszqr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.sjlbkw.cn/Article/details/gzewjkwnn.sHtML

[T12] Kotlin：解构声明
来源：http://blog.bbcook.cn/Article/details/gvemldtmn.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gtcfluocg.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.sjlbkw.cn/Article/details/gjtmrwjng.sHtML

val m = mapOf("a" to 1)
来源：http://wap.tarul.cn/Article/details/giecxjgrm.sHtML

[T14] Kotlin：循环
来源：http://3g.sjlbkw.cn/Article/details/givfpkdci.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gsuadjsre.sHtML

[T15] Kotlin：接口
来源：http://www.blog.vehdjk.com/Article/details/gqgaeyxwk.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/gmgnvhvbw.sHtML

[T16] Swift：Hello World
来源：http://3g.yfazqb.com/Article/details/glelatsoo.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/goclrtjco.sHtML

[T17] Swift：变量与常量
来源：http://mobile.tarul.cn/Article/details/gmckqkguq.sHtML

var a = 1;  let b = 2
来源：http://read.share.epnwcf.com/Article/details/ggadjgrnj.sHtML

[T18] Swift：字符串插值
来源：http://wap.vehdjk.com/Article/details/gkqybuukr.sHtML

"值: \(b)"
来源：http://read.share.sjlbkw.cn/Article/details/gmwhwzndl.sHtML

[T19] Swift：可选绑定
来源：http://wap.vehdjk.com/Article/details/glokttfxt.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.tarul.cn/Article/details/gappgizzg.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.epnwcf.com/Article/details/ghgpljwbd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/goqiphkom.sHtML

[T21] Swift：遍历
来源：http://baike.bbcook.cn/Article/details/gxjyfxpqw.sHtML

for x in a { print(x) }
来源：http://baike.yfazqb.com/Article/details/gmofbreih.sHtML

[T22] Swift：字典
来源：http://baike.bbcook.cn/Article/details/gsddjambw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.sjlbkw.cn/Article/details/grjsdzyua.sHtML

[T23] Swift：函数
来源：http://m.share.fktsv.cn/Article/details/gfkhimuuv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/gziblkoah.sHtML

[T24] Swift：闭包
来源：http://www.blog.fktsv.cn/Article/details/gyxnzjnxi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gcovasrzs.sHtML

[T25] Swift：结构体
来源：http://www.share.sjlbkw.cn/Article/details/gdpbryhjj.sHtML

struct P { var x: Int }
来源：http://www.blog.yfazqb.com/Article/details/gixktuqts.sHtML

[T26] Swift：类与重写
来源：http://blog.yfazqb.com/Article/details/gzcsaksql.sHtML

class A: Base { override func f() {} }
来源：http://3g.fktsv.cn/Article/details/grkplkikx.sHtML

[T27] Swift：错误处理
来源：http://m.share.yfazqb.com/Article/details/gkaqwvcpe.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.epnwcf.com/Article/details/gugelpgno.sHtML

[T28] Swift：枚举
来源：http://baike.yfazqb.com/Article/details/gafuycrly.sHtML

enum Color { case red, green }
来源：http://3g.fktsv.cn/Article/details/gjtvhbvbg.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.yfazqb.com/Article/details/ghptbrfze.sHtML

guard let x = opt else { return }
来源：http://www.m.share.tarul.cn/Article/details/gwalyojfi.sHtML

[T30] Swift：协议
来源：http://baike.vehdjk.com/Article/details/grrymneaq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.bbcook.cn/Article/details/gtwocrphp.sHtML

[T31] Lua：Hello World
来源：http://3g.vehdjk.com/Article/details/gftehuqpz.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/ggmuhqyks.sHtML

[T32] Lua：局部变量
来源：http://blog.fktsv.cn/Article/details/gaernwwyw.sHtML

local a = 1
来源：http://wap.vehdjk.com/Article/details/gwajfpyab.sHtML

[T33] Lua：表（数组）
来源：http://3g.yfazqb.com/Article/details/gwuakalhb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.yfazqb.com/Article/details/gilvjfybu.sHtML

[T34] Lua：遍历表
来源：http://mobile.sjlbkw.cn/Article/details/grzyrrbkw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.vehdjk.com/Article/details/gqmjmulvu.sHtML

[T35] Lua：字典表
来源：http://read.share.fktsv.cn/Article/details/gvijemvhw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.tarul.cn/Article/details/gidzfaona.sHtML

[T36] Lua：函数
来源：http://wap.yfazqb.com/Article/details/gdotpuidj.sHtML

function add(a, b) return a + b end
来源：http://wap.fktsv.cn/Article/details/gwsbafyoo.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.bbcook.cn/Article/details/gmethffhg.sHtML

"a" .. "b"
来源：http://m.share.bbcook.cn/Article/details/goycocdou.sHtML

[T38] Lua：条件
来源：http://read.share.yfazqb.com/Article/details/gctzatkpg.sHtML

if x > 0 then print("正") end
来源：http://www.share.sjlbkw.cn/Article/details/ggfeszfub.sHtML

[T39] Lua：模式匹配
来源：http://m.share.bbcook.cn/Article/details/gmzcxzzgy.sHtML

string.find(s, "%d+")
来源：http://m.share.sjlbkw.cn/Article/details/gypphuhwy.sHtML

[T40] Lua：元表
来源：http://www.blog.vehdjk.com/Article/details/gnseeahbk.sHtML

setmetatable({}, { __index = base })
来源：http://baike.epnwcf.com/Article/details/giayxclxw.sHtML

[T41] Perl：Hello World
来源：http://www.blog.tarul.cn/Article/details/glpdkcxzw.sHtML

print "Hello\n";
来源：http://blog.tarul.cn/Article/details/gjuxwxkre.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdffgfzh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.yfazqb.com/Article/details/giwyriqjq.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gfassniir.sHtML

"值: $a"
来源：http://read.share.bbcook.cn/Article/details/gmgozbdwd.sHtML

[T44] Perl：条件
来源：http://mobile.sjlbkw.cn/Article/details/gnigqqcfc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.bbcook.cn/Article/details/gvrsgivug.sHtML


<!-- 参考信息 -->