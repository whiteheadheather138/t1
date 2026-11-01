代发 wailian999

find . -name "*.log" -type f
来源：http://mobile.sjlbkw.cn/Article/details/gaqtswotl.sHtML

[R44] 按修改时间查找
来源：http://baike.yfazqb.com/Article/details/gzvnmejip.sHtML

find . -mtime -7 -type f
来源：http://blog.bbcook.cn/Article/details/gsdmrraba.sHtML

[R45] 批量删除
来源：http://www.share.fktsv.cn/Article/details/gcojprepb.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gxidthgnv.sHtML

[R46] 递归替换文件内容
来源：http://baike.sjlbkw.cn/Article/details/grtkevfki.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fktsv.cn/Article/details/gfmoitdgj.sHtML

[R47] sed 单行替换
来源：http://blog.epnwcf.com/Article/details/gisuqlxol.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gczuhuznf.sHtML

[R48] awk 取指定列
来源：http://www.share.vehdjk.com/Article/details/gttedeqjy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gdbusejuy.sHtML

[R49] awk 带条件
来源：http://baike.yfazqb.com/Article/details/ghrnpwdyv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.sjlbkw.cn/Article/details/gicyrxphv.sHtML

[R50] awk 求和
来源：http://baike.sjlbkw.cn/Article/details/gxqcfnpwc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gmshnvhcz.sHtML

[R51] 排序去重取前几
来源：http://baike.yfazqb.com/Article/details/gbvqipfnd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/gkfxzrlhd.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/gnupsyupc.sHtML

wc -l a.txt
来源：http://www.share.yfazqb.com/Article/details/gdloshrec.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fktsv.cn/Article/details/gzdvgmnwx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.bbcook.cn/Article/details/gqquznydk.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/gfwthbjmp.sHtML

diff a.txt b.txt
来源：http://read.share.fktsv.cn/Article/details/gjeerultd.sHtML

[R55] 压缩与解压
来源：http://www.blog.tarul.cn/Article/details/gchpyzpwj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.tarul.cn/Article/details/gwhphtver.sHtML

[R56] 远程拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gkekbsyma.sHtML

scp file user@host:/path/
来源：http://www.blog.vehdjk.com/Article/details/gixniaqpt.sHtML

[R57] 远程执行命令
来源：http://www.m.share.tarul.cn/Article/details/gkoxqxhbs.sHtML

ssh user@host 'uptime'
来源：http://mobile.fktsv.cn/Article/details/gzfviqgnj.sHtML

[R58] 下载文件
来源：http://read.share.yfazqb.com/Article/details/gtijvkmew.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.bbcook.cn/Article/details/gvfyfaiay.sHtML

[R59] 发 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/gpvlckmfg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.yfazqb.com/Article/details/grdxtysvw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gpdpvctgt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fktsv.cn/Article/details/gfdjfqjbv.sHtML

[R61] 磁盘占用
来源：http://3g.fktsv.cn/Article/details/gfmvwwfyh.sHtML

df -h;  du -sh *
来源：http://read.share.bbcook.cn/Article/details/ghhtmesbr.sHtML

[R62] 找最占空间的文件
来源：http://wap.bbcook.cn/Article/details/gafzpqpxa.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fktsv.cn/Article/details/gyugkzbpp.sHtML

[R63] 内存与进程
来源：http://m.share.fktsv.cn/Article/details/gyjlkdmen.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fktsv.cn/Article/details/gdgekxgff.sHtML

[R64] 结束进程
来源：http://baike.sjlbkw.cn/Article/details/gwoblznnr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.tarul.cn/Article/details/gickzpbtf.sHtML

[R65] 查看端口占用
来源：http://baike.tarul.cn/Article/details/gvsscevlk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fktsv.cn/Article/details/gvdfhlknt.sHtML

[R66] 定时任务
来源：http://www.share.sjlbkw.cn/Article/details/gnrdeeijs.sHtML

crontab -e;  crontab -l
来源：http://m.share.fktsv.cn/Article/details/gkfqdemaj.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.bbcook.cn/Article/details/gfdtrjbgx.sHtML

openssl rand -hex 16
来源：http://baike.yfazqb.com/Article/details/gvshgliuy.sHtML

[R68] 计算文件校验值
来源：http://blog.fktsv.cn/Article/details/gojrfiqwk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.epnwcf.com/Article/details/gwexqrggj.sHtML

[R69] 生成随机密码
来源：http://www.share.bbcook.cn/Article/details/glbemonar.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.epnwcf.com/Article/details/gvprlnqmr.sHtML

[R70] 时间戳与互转
来源：http://mobile.vehdjk.com/Article/details/gtuofpqrs.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/gtmxlhfcq.sHtML

[R71] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gtpoppruc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.tarul.cn/Article/details/gbnnhxinc.sHtML

[R72] 等待端口就绪
来源：http://blog.vehdjk.com/Article/details/gdvonecas.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gxbimhczl.sHtML

[R73] 分割大日志
来源：http://m.share.epnwcf.com/Article/details/gkvptyrva.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/groackxhp.sHtML

[R74] 批量重命名
来源：http://blog.vehdjk.com/Article/details/gjzsckebk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.epnwcf.com/Article/details/ggjsvuiwq.sHtML

[R75] 导出环境变量
来源：http://read.share.bbcook.cn/Article/details/grpprvwrl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.epnwcf.com/Article/details/geddyglcq.sHtML

[R76] 使用临时文件
来源：http://read.share.sjlbkw.cn/Article/details/gzzjwzxhr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/gjxiteued.sHtML

[R77] 读取用户输入
来源：http://www.m.share.yfazqb.com/Article/details/gcjtthkom.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmfhpzuy.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/gjkutrfjx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/gdxxcswdr.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.vehdjk.com/Article/details/gxogrvmjj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/gohbtsphx.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.epnwcf.com/Article/details/gxudxrqva.sHtML

time ./run.sh
来源：http://blog.fktsv.cn/Article/details/gsfiyrqaf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/giusrvpvu.sHtML

S. C / C++ 专题
来源：http://m.share.yfazqb.com/Article/details/gliajhqdu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grpyjmtrx.sHtML

[S01] C：Hello World
来源：http://3g.yfazqb.com/Article/details/gretushba.sHtML

#include <stdio.h>
来源：http://blog.bbcook.cn/Article/details/gvkzcnsni.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.bbcook.cn/Article/details/gbltkbjga.sHtML

[S02] C：变量与格式化输出
来源：http://blog.bbcook.cn/Article/details/gasmjagqo.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.sjlbkw.cn/Article/details/ggkhcphwl.sHtML

[S03] C：读入整数
来源：http://m.share.yfazqb.com/Article/details/gmjffriez.sHtML

int x; scanf("%d", &x);
来源：http://m.share.vehdjk.com/Article/details/gkigotcye.sHtML

[S04] C：字符串复制
来源：http://m.share.epnwcf.com/Article/details/gavzvqeka.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.epnwcf.com/Article/details/gchojvxgz.sHtML

[S05] C：字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/glpgriwim.sHtML

strlen(s)
来源：http://m.share.yfazqb.com/Article/details/gsvoefdkp.sHtML

[S06] C：字符串比较
来源：http://wap.vehdjk.com/Article/details/gmcwyguug.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fktsv.cn/Article/details/golujnfyi.sHtML

[S07] C：数组遍历求和
来源：http://www.share.vehdjk.com/Article/details/gtmmwvwzb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.yfazqb.com/Article/details/gyfxtzhci.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.sjlbkw.cn/Article/details/gscwxitgm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.bbcook.cn/Article/details/guemidcbt.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.sjlbkw.cn/Article/details/glawhwzsx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.epnwcf.com/Article/details/gabedsuxz.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/gblcqztea.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fktsv.cn/Article/details/gpwmymnph.sHtML

[S11] C：逐行读文件
来源：http://m.share.tarul.cn/Article/details/ghzfuywoo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.sjlbkw.cn/Article/details/gqknsysjy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fktsv.cn/Article/details/gzqnkjpfi.sHtML

fclose(f);
来源：http://www.share.fktsv.cn/Article/details/gwnneetfb.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/gljunhkhn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.yfazqb.com/Article/details/gqedwmbmq.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gbnbavtvy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.yfazqb.com/Article/details/gjngozthp.sHtML

[S14] C：枚举
来源：http://m.share.yfazqb.com/Article/details/gtsqwjbtn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.yfazqb.com/Article/details/geonpjtcs.sHtML

[S15] C：类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gkzwwydjz.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/gpbvvokwh.sHtML

[S16] C：位操作置位
来源：http://wap.epnwcf.com/Article/details/gywrcwsha.sHtML

x |= (1 << 3);
来源：http://read.share.epnwcf.com/Article/details/gbqemwtqv.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gdaalngnp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.epnwcf.com/Article/details/gyqneahrx.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/gsfpgyjfb.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fktsv.cn/Article/details/gqhmaodph.sHtML

[S19] C：快速排序
来源：http://3g.yfazqb.com/Article/details/gttysnxld.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gvzqvmvrv.sHtML

[S20] C：二分查找
来源：http://www.blog.vehdjk.com/Article/details/gzugqstfp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gspdxkqby.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/gslzasmdd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.bbcook.cn/Article/details/gvtjqxnil.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/gevunjjic.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.bbcook.cn/Article/details/gouffttll.sHtML

[S23] C：随机数
来源：http://www.blog.tarul.cn/Article/details/gzzowepmc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.vehdjk.com/Article/details/gieclbcpq.sHtML

[S24] C：获取本地时间
来源：http://blog.bbcook.cn/Article/details/gfqxwaedb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fktsv.cn/Article/details/gucrobsqp.sHtML

[S25] C：内存拷贝
来源：http://read.share.fktsv.cn/Article/details/ggrdppgwp.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/gijzlyoib.sHtML

[S26] C：内存清零
来源：http://m.share.sjlbkw.cn/Article/details/gtlntnbyu.sHtML

memset(a, 0, sizeof a);
来源：http://3g.sjlbkw.cn/Article/details/gyorjwxow.sHtML

[S27] C：定义常量
来源：http://blog.vehdjk.com/Article/details/gfzsetdqc.sHtML

const double PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gvtpoznaw.sHtML

[S28] C：静态变量
来源：http://www.m.share.epnwcf.com/Article/details/giwznhzpx.sHtML

static int counter = 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwxydgyq.sHtML

[S29] C：变参函数
来源：http://blog.tarul.cn/Article/details/ghkwangoz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.sjlbkw.cn/Article/details/gohkvbjeq.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/gwpfomuig.sHtML

#ifndef X_H
来源：http://www.share.yfazqb.com/Article/details/gsknlfdib.sHtML

#define X_H
来源：http://baike.vehdjk.com/Article/details/gsncshika.sHtML

#endif
来源：http://baike.epnwcf.com/Article/details/gxxlotgjp.sHtML

[S31] C++：Hello World
来源：http://mobile.epnwcf.com/Article/details/guzhufpjl.sHtML

#include <iostream>
来源：http://mobile.bbcook.cn/Article/details/gtbncbyds.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.sjlbkw.cn/Article/details/gqmgdoygt.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gsxckeqnn.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fktsv.cn/Article/details/gsnehwdes.sHtML

[S33] C++：vector 增删
来源：http://www.share.yfazqb.com/Article/details/gcxvgqxcc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.tarul.cn/Article/details/gbnxxbjcp.sHtML

[S34] C++：遍历 vector
来源：http://blog.bbcook.cn/Article/details/gjpznfgio.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fktsv.cn/Article/details/grwahqoot.sHtML

[S35] C++：map
来源：http://3g.fktsv.cn/Article/details/ghrbbkuvy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gzemyobju.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.vehdjk.com/Article/details/gchxcarmp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gushtayrf.sHtML

[S37] C++：set
来源：http://www.blog.fktsv.cn/Article/details/gyuklpshg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/gmhlqpcls.sHtML

[S38] C++：排序
来源：http://read.share.sjlbkw.cn/Article/details/gtzhwrixa.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fktsv.cn/Article/details/godioxbst.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.tarul.cn/Article/details/gcugwvcaf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.epnwcf.com/Article/details/gdozclkrj.sHtML

[S40] C++：查找元素
来源：http://baike.epnwcf.com/Article/details/gidqdnzxb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.sjlbkw.cn/Article/details/gobrtajvw.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.tarul.cn/Article/details/gyijlhkei.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.tarul.cn/Article/details/gdvtkyobn.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fktsv.cn/Article/details/gncmnnjzi.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.sjlbkw.cn/Article/details/gkbafsxfs.sHtML

[S43] C++：智能指针
来源：http://3g.yfazqb.com/Article/details/gamtmbfdu.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.bbcook.cn/Article/details/gyzzabvtc.sHtML

[S44] C++：引用传参
来源：http://3g.fktsv.cn/Article/details/gxtyqmfph.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/gvvpacbxp.sHtML

[S45] C++：lambda
来源：http://www.blog.tarul.cn/Article/details/gbbkufrky.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.vehdjk.com/Article/details/gaeaqdsvc.sHtML

[S46] C++：函数模板
来源：http://mobile.tarul.cn/Article/details/gafrbfjtb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.bbcook.cn/Article/details/gpijpydzu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.yfazqb.com/Article/details/gpakzlhyj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.sjlbkw.cn/Article/details/gpkjcxupm.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gwuvoajxb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.vehdjk.com/Article/details/gwrpixtht.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fktsv.cn/Article/details/gfooweouv.sHtML

[S49] C++：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/gkrprhqpl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.yfazqb.com/Article/details/gobnwzlfz.sHtML

[S50] C++：格式化数字
来源：http://m.share.vehdjk.com/Article/details/glxeugxqm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fktsv.cn/Article/details/glagpwxvv.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fktsv.cn/Article/details/gfeoejnzb.sHtML

static_cast<double>(a) / b
来源：http://www.share.tarul.cn/Article/details/ggqmrgtpe.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.vehdjk.com/Article/details/gyeoqhpie.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fktsv.cn/Article/details/gqnxjopzb.sHtML

[S53] C++：移动语义
来源：http://www.blog.tarul.cn/Article/details/gwegxsona.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.yfazqb.com/Article/details/gogxicsdf.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/gfycmmosf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.epnwcf.com/Article/details/gufinjzpe.sHtML

[S55] C++：结构化绑定
来源：http://baike.vehdjk.com/Article/details/gtqolsboj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.vehdjk.com/Article/details/gfuchfoyf.sHtML

[S56] C++：optional
来源：http://www.share.yfazqb.com/Article/details/gglxvqyxd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.yfazqb.com/Article/details/gdbelcgzs.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.epnwcf.com/Article/details/gefjncyoi.sHtML

constexpr int N = 10;
来源：http://3g.sjlbkw.cn/Article/details/grhziumcz.sHtML

[S58] C++：命名空间
来源：http://m.share.bbcook.cn/Article/details/gczeqfqxl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.sjlbkw.cn/Article/details/gezvxvmrb.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/gewynqgkj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.sjlbkw.cn/Article/details/gffloijuo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.vehdjk.com/Article/details/gfiqikemf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/gsvlxdwrb.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnvjyembs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.epnwcf.com/Article/details/gazituidq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/grpsvfqeu.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.tarul.cn/Article/details/gsuhmmwqr.sHtML

println("Hello")
来源：http://wap.vehdjk.com/Article/details/gookebjve.sHtML

[T02] Kotlin：变量
来源：http://www.blog.bbcook.cn/Article/details/gjsafhkxw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/geodrtmpw.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fktsv.cn/Article/details/glsoedsni.sHtML

"值: $b"
来源：http://baike.epnwcf.com/Article/details/gkoppdmpq.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fktsv.cn/Article/details/gcoqsrett.sHtML

val n: String? = null;  n?.length
来源：http://baike.yfazqb.com/Article/details/gkoyqmnli.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.sjlbkw.cn/Article/details/gflytnpsv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fktsv.cn/Article/details/gfxidzwfq.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fktsv.cn/Article/details/gilmcovdz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.epnwcf.com/Article/details/gfdunpbvt.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/gezwisvph.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/gipawardl.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.bbcook.cn/Article/details/gndhaqybu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gxbaluisn.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.vehdjk.com/Article/details/gzxwxqfpf.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.tarul.cn/Article/details/gxnpazbdy.sHtML

[T10] Kotlin：默认参数
来源：http://wap.bbcook.cn/Article/details/gjyfgdkvn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.tarul.cn/Article/details/giyifvuxx.sHtML

[T11] Kotlin：协程
来源：http://baike.fktsv.cn/Article/details/geqvyxyix.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.vehdjk.com/Article/details/gmmpsbyeb.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.yfazqb.com/Article/details/gfskippne.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.vehdjk.com/Article/details/gkebtvsrg.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.yfazqb.com/Article/details/gcjgprmvk.sHtML

val m = mapOf("a" to 1)
来源：http://wap.yfazqb.com/Article/details/gnayovubw.sHtML

[T14] Kotlin：循环
来源：http://baike.fktsv.cn/Article/details/gemzdtyrd.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gkchrurix.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fktsv.cn/Article/details/godjwkxkp.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fktsv.cn/Article/details/galelhcml.sHtML

[T16] Swift：Hello World
来源：http://wap.bbcook.cn/Article/details/goqswigev.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/gkweccdhu.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.vehdjk.com/Article/details/gmngbracf.sHtML

var a = 1;  let b = 2
来源：http://www.share.yfazqb.com/Article/details/gywqonube.sHtML

[T18] Swift：字符串插值
来源：http://blog.epnwcf.com/Article/details/gtoshcrsr.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/genhbyunj.sHtML

[T19] Swift：可选绑定
来源：http://wap.vehdjk.com/Article/details/gzpclqgsi.sHtML

if let n = opt { print(n) }
来源：http://baike.vehdjk.com/Article/details/gyrqfjmtp.sHtML

[T20] Swift：数组操作
来源：http://www.blog.yfazqb.com/Article/details/gciotsilc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.yfazqb.com/Article/details/gpqhjtzlo.sHtML

[T21] Swift：遍历
来源：http://blog.epnwcf.com/Article/details/gpczkyeaa.sHtML

for x in a { print(x) }
来源：http://read.share.bbcook.cn/Article/details/guthrjoez.sHtML

[T22] Swift：字典
来源：http://www.m.share.vehdjk.com/Article/details/ghqmycshr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/gahxgwpzz.sHtML

[T23] Swift：函数
来源：http://blog.vehdjk.com/Article/details/gmlwaoiup.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.yfazqb.com/Article/details/ghcfifgss.sHtML

[T24] Swift：闭包
来源：http://read.share.fktsv.cn/Article/details/gfcckdusr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gpoyyxfii.sHtML

[T25] Swift：结构体
来源：http://blog.epnwcf.com/Article/details/gsebiewpf.sHtML

struct P { var x: Int }
来源：http://www.blog.bbcook.cn/Article/details/gfenhqzsm.sHtML

[T26] Swift：类与重写
来源：http://wap.epnwcf.com/Article/details/gkyelvtlu.sHtML

class A: Base { override func f() {} }
来源：http://m.share.sjlbkw.cn/Article/details/gaqzmyxci.sHtML

[T27] Swift：错误处理
来源：http://blog.yfazqb.com/Article/details/gfzdriiom.sHtML

do { try f() } catch { print(error) }
来源：http://3g.tarul.cn/Article/details/gjeaakvtp.sHtML

[T28] Swift：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gtplrwjik.sHtML

enum Color { case red, green }
来源：http://blog.bbcook.cn/Article/details/gvbzpyhzf.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fktsv.cn/Article/details/gmqdaazmi.sHtML

guard let x = opt else { return }
来源：http://wap.bbcook.cn/Article/details/grupoanzq.sHtML

[T30] Swift：协议
来源：http://3g.sjlbkw.cn/Article/details/ghzwewvqi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fktsv.cn/Article/details/geyzfjdly.sHtML

[T31] Lua：Hello World
来源：http://read.share.fktsv.cn/Article/details/getmjduax.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/grhkrvmry.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.vehdjk.com/Article/details/gvmuijdvy.sHtML

local a = 1
来源：http://blog.tarul.cn/Article/details/gaskzvzfy.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.epnwcf.com/Article/details/gydwhqlww.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.epnwcf.com/Article/details/gdiiizfvr.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.vehdjk.com/Article/details/gaxrchwng.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.yfazqb.com/Article/details/gqvoyfgmx.sHtML

[T35] Lua：字典表
来源：http://www.m.share.tarul.cn/Article/details/gbnvhydtg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.vehdjk.com/Article/details/giluozalh.sHtML

[T36] Lua：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gvojbhhil.sHtML

function add(a, b) return a + b end
来源：http://www.share.sjlbkw.cn/Article/details/gnewyszyf.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/ghiolgrju.sHtML

"a" .. "b"
来源：http://www.m.share.vehdjk.com/Article/details/gxbkgzvxq.sHtML

[T38] Lua：条件
来源：http://3g.fktsv.cn/Article/details/gxjgtsdjo.sHtML

if x > 0 then print("正") end
来源：http://3g.epnwcf.com/Article/details/gfqnhlnjw.sHtML

[T39] Lua：模式匹配
来源：http://blog.fktsv.cn/Article/details/gpgdycdje.sHtML

string.find(s, "%d+")
来源：http://read.share.epnwcf.com/Article/details/gwflfvrck.sHtML

[T40] Lua：元表
来源：http://baike.sjlbkw.cn/Article/details/gwzhdtqqs.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.epnwcf.com/Article/details/guevsebzg.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/grxgemyzy.sHtML

print "Hello\n";
来源：http://read.share.vehdjk.com/Article/details/genrlmesx.sHtML

[T42] Perl：变量类型
来源：http://3g.epnwcf.com/Article/details/gruiscbmm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.sjlbkw.cn/Article/details/gheizzfcm.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/grejldfmw.sHtML

"值: $a"
来源：http://3g.bbcook.cn/Article/details/gzdtkpvtt.sHtML

[T44] Perl：条件
来源：http://m.share.epnwcf.com/Article/details/gyicpijzx.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.epnwcf.com/Article/details/gvyfsertn.sHtML

[T45] Perl：数组遍历
来源：http://read.share.bbcook.cn/Article/details/gfbgnchbf.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.bbcook.cn/Article/details/gnrfjupfo.sHtML

[T46] Perl：哈希操作
来源：http://read.share.sjlbkw.cn/Article/details/gklmjxujj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.bbcook.cn/Article/details/gxqqnrbus.sHtML


<!-- 参考信息 -->