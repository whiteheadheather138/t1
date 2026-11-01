代发 wailian999

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/gbijjtbzr.sHtML

[R42] 输入重定向
来源：http://read.share.vehdjk.com/Article/details/gxuaroqdx.sHtML

wc -l < a.txt
来源：http://blog.tarul.cn/Article/details/gseqzxtxr.sHtML

[R43] 按名字查找文件
来源：http://wap.fktsv.cn/Article/details/gznxjrshe.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.sjlbkw.cn/Article/details/gflptxbek.sHtML

[R44] 按修改时间查找
来源：http://blog.tarul.cn/Article/details/gjvfcerya.sHtML

find . -mtime -7 -type f
来源：http://m.share.tarul.cn/Article/details/gluqdgzhk.sHtML

[R45] 批量删除
来源：http://baike.sjlbkw.cn/Article/details/gptuzlbru.sHtML

find . -name "*.tmp" -delete
来源：http://wap.bbcook.cn/Article/details/gvsdssfrj.sHtML

[R46] 递归替换文件内容
来源：http://blog.vehdjk.com/Article/details/gtkcngzbh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.sjlbkw.cn/Article/details/gpxsbuxpk.sHtML

[R47] sed 单行替换
来源：http://baike.sjlbkw.cn/Article/details/gubbmicvx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.bbcook.cn/Article/details/gayoyvzgp.sHtML

[R48] awk 取指定列
来源：http://www.share.fktsv.cn/Article/details/gwtaxpcad.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gkekqmnbj.sHtML

[R49] awk 带条件
来源：http://3g.bbcook.cn/Article/details/gbcyerztl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.yfazqb.com/Article/details/gnhenwmxs.sHtML

[R50] awk 求和
来源：http://m.share.sjlbkw.cn/Article/details/giznhqlit.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.epnwcf.com/Article/details/gnlpanqus.sHtML

[R51] 排序去重取前几
来源：http://baike.yfazqb.com/Article/details/gcsilmajy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.bbcook.cn/Article/details/gjtqoasop.sHtML

[R52] 统计行数
来源：http://m.share.epnwcf.com/Article/details/gdfmqosca.sHtML

wc -l a.txt
来源：http://www.share.bbcook.cn/Article/details/gcweedfhd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.sjlbkw.cn/Article/details/gcybamnrq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.bbcook.cn/Article/details/gjzjjjofh.sHtML

[R54] 比较两个文件
来源：http://www.share.yfazqb.com/Article/details/guxqlndhr.sHtML

diff a.txt b.txt
来源：http://mobile.fktsv.cn/Article/details/gqlsdsrkm.sHtML

[R55] 压缩与解压
来源：http://www.m.share.sjlbkw.cn/Article/details/giierfuwj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.tarul.cn/Article/details/gdqayonew.sHtML

[R56] 远程拷贝
来源：http://m.share.epnwcf.com/Article/details/gsdqhzaze.sHtML

scp file user@host:/path/
来源：http://read.share.sjlbkw.cn/Article/details/gtspwbglt.sHtML

[R57] 远程执行命令
来源：http://www.share.tarul.cn/Article/details/gzcfnayur.sHtML

ssh user@host 'uptime'
来源：http://www.share.vehdjk.com/Article/details/gxmqdkwxp.sHtML

[R58] 下载文件
来源：http://wap.vehdjk.com/Article/details/gihtgazym.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.tarul.cn/Article/details/goixnkuvy.sHtML

[R59] 发 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gdbszlcns.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.yfazqb.com/Article/details/glyezhwlu.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/gyooptotr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fktsv.cn/Article/details/ggodsdbei.sHtML

[R61] 磁盘占用
来源：http://mobile.tarul.cn/Article/details/gbbtmjmpa.sHtML

df -h;  du -sh *
来源：http://wap.bbcook.cn/Article/details/gqkbwaptj.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fktsv.cn/Article/details/gtfnrajew.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.vehdjk.com/Article/details/gfnhkedvf.sHtML

[R63] 内存与进程
来源：http://read.share.epnwcf.com/Article/details/gwmbwqucd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.bbcook.cn/Article/details/gtejnhxcm.sHtML

[R64] 结束进程
来源：http://baike.tarul.cn/Article/details/ghpsmziom.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.vehdjk.com/Article/details/greejmgbu.sHtML

[R65] 查看端口占用
来源：http://read.share.sjlbkw.cn/Article/details/gcibyxqrh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.vehdjk.com/Article/details/guazrhpox.sHtML

[R66] 定时任务
来源：http://read.share.vehdjk.com/Article/details/gaiixmiun.sHtML

crontab -e;  crontab -l
来源：http://blog.sjlbkw.cn/Article/details/gdlytyxgd.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/gdzsrqufk.sHtML

openssl rand -hex 16
来源：http://baike.tarul.cn/Article/details/gjezcliky.sHtML

[R68] 计算文件校验值
来源：http://read.share.vehdjk.com/Article/details/gwvmkkinw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.bbcook.cn/Article/details/gxczipgtz.sHtML

[R69] 生成随机密码
来源：http://read.share.vehdjk.com/Article/details/gcnbqdrbu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gkeqtygct.sHtML

[R70] 时间戳与互转
来源：http://www.blog.tarul.cn/Article/details/gklzqjbgo.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/glxmxboqg.sHtML

[R71] 日期格式化
来源：http://wap.bbcook.cn/Article/details/gokpzicde.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.yfazqb.com/Article/details/gbgeuuvbf.sHtML

[R72] 等待端口就绪
来源：http://wap.fktsv.cn/Article/details/gpmgkhegm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gfiavxwip.sHtML

[R73] 分割大日志
来源：http://m.share.yfazqb.com/Article/details/gxlynbfeg.sHtML

split -l 1000 big.log part_
来源：http://m.share.bbcook.cn/Article/details/gnrqvlhbm.sHtML

[R74] 批量重命名
来源：http://www.share.bbcook.cn/Article/details/gugyqpptg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.vehdjk.com/Article/details/gfyzvinpk.sHtML

[R75] 导出环境变量
来源：http://m.share.tarul.cn/Article/details/ggzbvamjb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.vehdjk.com/Article/details/gicgnckyx.sHtML

[R76] 使用临时文件
来源：http://3g.yfazqb.com/Article/details/gsgapnsqz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gdwiepqmq.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fktsv.cn/Article/details/ghujshiew.sHtML

read -rp "请输入: " ans
来源：http://www.blog.tarul.cn/Article/details/gqmeukjut.sHtML

[R78] 交互式菜单
来源：http://3g.fktsv.cn/Article/details/gflpijihd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.yfazqb.com/Article/details/gicjboakt.sHtML

[R79] 解析命令行选项
来源：http://blog.epnwcf.com/Article/details/gifklpkho.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.tarul.cn/Article/details/gydgprubm.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.bbcook.cn/Article/details/gvhrwlwlb.sHtML

time ./run.sh
来源：http://blog.tarul.cn/Article/details/gzytipznp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gxnejaddi.sHtML

S. C / C++ 专题
来源：http://www.blog.bbcook.cn/Article/details/gwbdiaalz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwhgmcoyu.sHtML

[S01] C：Hello World
来源：http://www.m.share.tarul.cn/Article/details/ghlftvems.sHtML

#include <stdio.h>
来源：http://www.share.sjlbkw.cn/Article/details/gapxlhepg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.tarul.cn/Article/details/gmodmzozi.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnqehqut.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.epnwcf.com/Article/details/gporhzois.sHtML

[S03] C：读入整数
来源：http://read.share.bbcook.cn/Article/details/gxjmdyttr.sHtML

int x; scanf("%d", &x);
来源：http://blog.bbcook.cn/Article/details/gcjsppoyl.sHtML

[S04] C：字符串复制
来源：http://blog.vehdjk.com/Article/details/gzcfwcxvx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.sjlbkw.cn/Article/details/ghoytnjae.sHtML

[S05] C：字符串长度
来源：http://m.share.fktsv.cn/Article/details/gxfzadddb.sHtML

strlen(s)
来源：http://3g.vehdjk.com/Article/details/gtmyhxppa.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/gscbcqdst.sHtML

strcmp(a, b) == 0
来源：http://3g.tarul.cn/Article/details/gsoqjqxya.sHtML

[S07] C：数组遍历求和
来源：http://www.share.tarul.cn/Article/details/glsbseguw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fktsv.cn/Article/details/gfyvlscpu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.sjlbkw.cn/Article/details/gdqepzxjy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/gbljzkthy.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.yfazqb.com/Article/details/gshctywvj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.yfazqb.com/Article/details/gwfberpzt.sHtML

[S10] C：指针与解引用
来源：http://www.blog.sjlbkw.cn/Article/details/gwnevxpzy.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.tarul.cn/Article/details/grfzcndmg.sHtML

[S11] C：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gawmcvoxg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fktsv.cn/Article/details/gaojnvprz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.epnwcf.com/Article/details/gsikcrivo.sHtML

fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gcpomassj.sHtML

[S12] C：写文件
来源：http://www.share.vehdjk.com/Article/details/gybvprfyr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fktsv.cn/Article/details/ggjpuzdcf.sHtML

[S13] C：宏定义
来源：http://3g.epnwcf.com/Article/details/gpyahiejx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.vehdjk.com/Article/details/gkdthmori.sHtML

[S14] C：枚举
来源：http://3g.fktsv.cn/Article/details/gfmmfkkgn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.bbcook.cn/Article/details/gtbkxercb.sHtML

[S15] C：类型转换
来源：http://blog.bbcook.cn/Article/details/gewbhcowj.sHtML

(double) a / b
来源：http://www.share.sjlbkw.cn/Article/details/grtwhlasp.sHtML

[S16] C：位操作置位
来源：http://baike.bbcook.cn/Article/details/gtfqwutbe.sHtML

x |= (1 << 3);
来源：http://3g.bbcook.cn/Article/details/ghieimfjb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gbbdltdcm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.epnwcf.com/Article/details/gzeavcfod.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/ghubbvjbh.sHtML

int main(int argc, char **argv)
来源：http://read.share.vehdjk.com/Article/details/gakjheici.sHtML

[S19] C：快速排序
来源：http://blog.tarul.cn/Article/details/gilohstqy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gapvjzfdq.sHtML

[S20] C：二分查找
来源：http://m.share.vehdjk.com/Article/details/gwfysoqlc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/gvkcmauyt.sHtML

[S21] C：字符类别判断
来源：http://3g.fktsv.cn/Article/details/gphynnpdd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fktsv.cn/Article/details/gribdskol.sHtML

[S22] C：字符串转数字
来源：http://read.share.bbcook.cn/Article/details/gihqoaaqt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.yfazqb.com/Article/details/gqcgfrpgm.sHtML

[S23] C：随机数
来源：http://baike.epnwcf.com/Article/details/gjmulvnzn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.bbcook.cn/Article/details/gbgbheacj.sHtML

[S24] C：获取本地时间
来源：http://wap.epnwcf.com/Article/details/gmkznqnjd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.bbcook.cn/Article/details/ggyabyhry.sHtML

[S25] C：内存拷贝
来源：http://3g.vehdjk.com/Article/details/gzjsmascx.sHtML

memcpy(dst, src, n);
来源：http://www.blog.tarul.cn/Article/details/gsckynstw.sHtML

[S26] C：内存清零
来源：http://www.blog.vehdjk.com/Article/details/gejeymval.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fktsv.cn/Article/details/gthcjykfe.sHtML

[S27] C：定义常量
来源：http://blog.fktsv.cn/Article/details/glbglqwbc.sHtML

const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gxrklmbse.sHtML

[S28] C：静态变量
来源：http://3g.epnwcf.com/Article/details/gqmpksntw.sHtML

static int counter = 0;
来源：http://read.share.vehdjk.com/Article/details/gnscxsrxb.sHtML

[S29] C：变参函数
来源：http://wap.sjlbkw.cn/Article/details/gqhyjolph.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.epnwcf.com/Article/details/gcykexcib.sHtML

[S30] C：头文件保护
来源：http://www.share.epnwcf.com/Article/details/gngujobjz.sHtML

#ifndef X_H
来源：http://m.share.fktsv.cn/Article/details/gorafwycl.sHtML

#define X_H
来源：http://3g.yfazqb.com/Article/details/gtlallbgm.sHtML

#endif
来源：http://read.share.sjlbkw.cn/Article/details/gwiswljvp.sHtML

[S31] C++：Hello World
来源：http://www.blog.tarul.cn/Article/details/gnsvwqidc.sHtML

#include <iostream>
来源：http://3g.epnwcf.com/Article/details/gdgbowppp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/gjtuaqfny.sHtML

[S32] C++：字符串
来源：http://www.share.vehdjk.com/Article/details/gnehcfnxy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fktsv.cn/Article/details/gxopuqlqw.sHtML

[S33] C++：vector 增删
来源：http://m.share.fktsv.cn/Article/details/gyyazlgbk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.epnwcf.com/Article/details/glrtppoim.sHtML

[S34] C++：遍历 vector
来源：http://read.share.bbcook.cn/Article/details/ghepyvaxt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.epnwcf.com/Article/details/gonwsgpqw.sHtML

[S35] C++：map
来源：http://mobile.yfazqb.com/Article/details/gcxbbyhgd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gzgrfxmoo.sHtML

[S36] C++：unordered_map
来源：http://m.share.fktsv.cn/Article/details/gjxbfkhaq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gonmkabny.sHtML

[S37] C++：set
来源：http://wap.vehdjk.com/Article/details/giknunyir.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.epnwcf.com/Article/details/gmpvjnmxb.sHtML

[S38] C++：排序
来源：http://www.m.share.fktsv.cn/Article/details/gehvwemdz.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gqlikzjbk.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.bbcook.cn/Article/details/glzscqige.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.vehdjk.com/Article/details/gfgnnrqwk.sHtML

[S40] C++：查找元素
来源：http://wap.tarul.cn/Article/details/gdlugyinb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxolityzk.sHtML

[S41] C++：类与构造函数
来源：http://blog.fktsv.cn/Article/details/gyjkzxmid.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fktsv.cn/Article/details/ggqygairl.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.sjlbkw.cn/Article/details/gtlenxfvg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.vehdjk.com/Article/details/gwyvbrzwv.sHtML

[S43] C++：智能指针
来源：http://www.m.share.bbcook.cn/Article/details/gnjnctxqg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.yfazqb.com/Article/details/gegdjkzdi.sHtML

[S44] C++：引用传参
来源：http://read.share.tarul.cn/Article/details/gximrxvae.sHtML

void inc(int &x) { ++x; }
来源：http://blog.epnwcf.com/Article/details/gnawltnoh.sHtML

[S45] C++：lambda
来源：http://www.share.tarul.cn/Article/details/gzovhvmrw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fktsv.cn/Article/details/gsrlusoeq.sHtML

[S46] C++：函数模板
来源：http://www.m.share.epnwcf.com/Article/details/gnijelblk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fktsv.cn/Article/details/gwcbqqcby.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fktsv.cn/Article/details/gfuvelgyp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.tarul.cn/Article/details/gmlhndeox.sHtML

[S48] C++：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gzvrtojit.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.epnwcf.com/Article/details/gxomomtkh.sHtML

while (std::getline(in, line)) { }
来源：http://blog.vehdjk.com/Article/details/gckrypbwy.sHtML

[S49] C++：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/giszhjwrm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fktsv.cn/Article/details/gtndwzjlt.sHtML

[S50] C++：格式化数字
来源：http://wap.fktsv.cn/Article/details/gwuuncrxg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.bbcook.cn/Article/details/ghqkfzges.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fktsv.cn/Article/details/guctopbmd.sHtML

static_cast<double>(a) / b
来源：http://wap.yfazqb.com/Article/details/gkirgwglb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.bbcook.cn/Article/details/gonlaggoh.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.sjlbkw.cn/Article/details/grnlwaqva.sHtML

[S53] C++：移动语义
来源：http://baike.tarul.cn/Article/details/gjhuwkfsv.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.epnwcf.com/Article/details/gpdmhcwzk.sHtML

[S54] C++：异常处理
来源：http://blog.sjlbkw.cn/Article/details/gtnkwldju.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.yfazqb.com/Article/details/gvgwxnnbw.sHtML

[S55] C++：结构化绑定
来源：http://m.share.yfazqb.com/Article/details/gkcmwyesy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.bbcook.cn/Article/details/gmrpeobmg.sHtML

[S56] C++：optional
来源：http://m.share.epnwcf.com/Article/details/gpfpgyxbd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.yfazqb.com/Article/details/gnjpfkrdk.sHtML

[S57] C++：编译期常量
来源：http://3g.epnwcf.com/Article/details/gsksgdilj.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gziblxfcc.sHtML

[S58] C++：命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gelnajtig.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.sjlbkw.cn/Article/details/gtszvsnsb.sHtML

[S59] C++：静态断言
来源：http://www.m.share.yfazqb.com/Article/details/grxxaauvl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.sjlbkw.cn/Article/details/gaqvoxjvj.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.tarul.cn/Article/details/gdpmvsxgx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.yfazqb.com/Article/details/gsqxbwlmt.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gkczadtwv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gkjzufegg.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmerzsfcc.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gmzgcvgnc.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/gdmcecuhy.sHtML

[T02] Kotlin：变量
来源：http://wap.bbcook.cn/Article/details/gaydqjfjf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/gwjucftbi.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.bbcook.cn/Article/details/gtukqojpy.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/gskkwcsvd.sHtML

[T04] Kotlin：空安全
来源：http://m.share.sjlbkw.cn/Article/details/gznvfjjbh.sHtML

val n: String? = null;  n?.length
来源：http://3g.epnwcf.com/Article/details/gsrrlvbsj.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.bbcook.cn/Article/details/gojpgsofg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.tarul.cn/Article/details/gfeucsfeo.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/gdryuceoo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/gfifsepxs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.vehdjk.com/Article/details/gopznabqe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.vehdjk.com/Article/details/gfowomkmd.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fktsv.cn/Article/details/gtvibnlut.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fktsv.cn/Article/details/gzdlwfzbl.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.bbcook.cn/Article/details/gpypaafpx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.yfazqb.com/Article/details/gohkaundw.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.tarul.cn/Article/details/guuvruieu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.vehdjk.com/Article/details/ggnmlaieb.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/gnuthxdvc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.yfazqb.com/Article/details/gagslygje.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.yfazqb.com/Article/details/grileiisv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.bbcook.cn/Article/details/gpcmmlfgn.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.epnwcf.com/Article/details/gveoqbdnv.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fktsv.cn/Article/details/gqruznous.sHtML

[T14] Kotlin：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gfrjpfrxq.sHtML

for (i in 1..10) println(i)
来源：http://3g.tarul.cn/Article/details/gzhwzatlb.sHtML

[T15] Kotlin：接口
来源：http://wap.sjlbkw.cn/Article/details/gdmpkgkya.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/ggcgyfked.sHtML

[T16] Swift：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gvegkanst.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/gflsvikne.sHtML

[T17] Swift：变量与常量
来源：http://baike.yfazqb.com/Article/details/goexlkuiy.sHtML

var a = 1;  let b = 2
来源：http://read.share.vehdjk.com/Article/details/gokpcglfl.sHtML

[T18] Swift：字符串插值
来源：http://blog.tarul.cn/Article/details/gcmdiuvwn.sHtML

"值: \(b)"
来源：http://www.share.bbcook.cn/Article/details/gaiawyicp.sHtML

[T19] Swift：可选绑定
来源：http://blog.yfazqb.com/Article/details/guyyxekqo.sHtML

if let n = opt { print(n) }
来源：http://www.blog.vehdjk.com/Article/details/gkfiqzsbw.sHtML

[T20] Swift：数组操作
来源：http://m.share.fktsv.cn/Article/details/gjikenzuf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.bbcook.cn/Article/details/gdgvhvqyp.sHtML

[T21] Swift：遍历
来源：http://www.share.vehdjk.com/Article/details/gcwvhkeud.sHtML

for x in a { print(x) }
来源：http://baike.vehdjk.com/Article/details/gnxylczhc.sHtML

[T22] Swift：字典
来源：http://www.m.share.vehdjk.com/Article/details/gwvwaypqs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.tarul.cn/Article/details/gekvfixum.sHtML

[T23] Swift：函数
来源：http://baike.tarul.cn/Article/details/gulgfhjfi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fktsv.cn/Article/details/guwfljzqj.sHtML

[T24] Swift：闭包
来源：http://www.m.share.vehdjk.com/Article/details/ggnpfpodi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fktsv.cn/Article/details/grwuabieq.sHtML

[T25] Swift：结构体
来源：http://wap.bbcook.cn/Article/details/guivlwnrt.sHtML

struct P { var x: Int }
来源：http://baike.tarul.cn/Article/details/gipfawcye.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.yfazqb.com/Article/details/gabafbftv.sHtML

class A: Base { override func f() {} }
来源：http://3g.vehdjk.com/Article/details/gefvakldz.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fktsv.cn/Article/details/goeyaidfk.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.yfazqb.com/Article/details/gxxbamova.sHtML

[T28] Swift：枚举
来源：http://www.m.share.tarul.cn/Article/details/gqzjrabsy.sHtML

enum Color { case red, green }
来源：http://mobile.yfazqb.com/Article/details/gepxjzkuf.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.bbcook.cn/Article/details/gtqurgakg.sHtML

guard let x = opt else { return }
来源：http://3g.yfazqb.com/Article/details/gtrszqyee.sHtML

[T30] Swift：协议
来源：http://www.blog.fktsv.cn/Article/details/gnibenpbf.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.yfazqb.com/Article/details/gctfqajym.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gdyndyvov.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gxywurybx.sHtML

[T32] Lua：局部变量
来源：http://baike.tarul.cn/Article/details/griabmxds.sHtML

local a = 1
来源：http://www.blog.yfazqb.com/Article/details/gxblatcsf.sHtML

[T33] Lua：表（数组）
来源：http://baike.bbcook.cn/Article/details/gtjbvlnsl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.tarul.cn/Article/details/gglcjyozq.sHtML

[T34] Lua：遍历表
来源：http://wap.vehdjk.com/Article/details/gcgfadxbr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/gzzmyzxho.sHtML

[T35] Lua：字典表
来源：http://www.share.bbcook.cn/Article/details/glsnngphj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.vehdjk.com/Article/details/gawxtbxfu.sHtML

[T36] Lua：函数
来源：http://read.share.yfazqb.com/Article/details/gwwfencyv.sHtML

function add(a, b) return a + b end
来源：http://blog.tarul.cn/Article/details/grchvsdpa.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.bbcook.cn/Article/details/glddzgaoz.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/geemowipf.sHtML

[T38] Lua：条件
来源：http://mobile.bbcook.cn/Article/details/glmtvstbo.sHtML

if x > 0 then print("正") end
来源：http://mobile.tarul.cn/Article/details/gkwmcsiib.sHtML

[T39] Lua：模式匹配
来源：http://read.share.vehdjk.com/Article/details/goakznxcf.sHtML

string.find(s, "%d+")
来源：http://blog.fktsv.cn/Article/details/gyzxbumnx.sHtML

[T40] Lua：元表
来源：http://m.share.vehdjk.com/Article/details/gengqyktm.sHtML

setmetatable({}, { __index = base })
来源：http://baike.yfazqb.com/Article/details/geezccdym.sHtML

[T41] Perl：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gmxstxzjq.sHtML

print "Hello\n";
来源：http://www.share.fktsv.cn/Article/details/gphgdgdhm.sHtML

[T42] Perl：变量类型
来源：http://blog.vehdjk.com/Article/details/gndavwwww.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.sjlbkw.cn/Article/details/ganhyfkwl.sHtML

[T43] Perl：字符串插值
来源：http://baike.bbcook.cn/Article/details/gowtljsss.sHtML

"值: $a"
来源：http://www.share.tarul.cn/Article/details/gngdvngib.sHtML

[T44] Perl：条件
来源：http://www.blog.epnwcf.com/Article/details/gnqajaden.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.tarul.cn/Article/details/gdrfzghvs.sHtML


<!-- 参考信息 -->