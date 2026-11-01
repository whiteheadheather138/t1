代发 wailian999

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/gbhlezues.sHtML

[R46] 递归替换文件内容
来源：http://mobile.sjlbkw.cn/Article/details/gumdhkfdq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.vehdjk.com/Article/details/gxvmpgnyf.sHtML

[R47] sed 单行替换
来源：http://www.m.share.epnwcf.com/Article/details/grtuflflx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.vehdjk.com/Article/details/glxxjhxes.sHtML

[R48] awk 取指定列
来源：http://mobile.fktsv.cn/Article/details/grvmrxfcp.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.tarul.cn/Article/details/glepkmtwm.sHtML

[R49] awk 带条件
来源：http://read.share.epnwcf.com/Article/details/geflgnjfo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fktsv.cn/Article/details/gqtjnpakv.sHtML

[R50] awk 求和
来源：http://www.share.epnwcf.com/Article/details/gxqfvwpey.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.yfazqb.com/Article/details/goyugymih.sHtML

[R51] 排序去重取前几
来源：http://baike.sjlbkw.cn/Article/details/ggxkrpqvu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.yfazqb.com/Article/details/gxdeczthn.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/gveepyecz.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/gqljyshoa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.bbcook.cn/Article/details/gzrtfidkz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.epnwcf.com/Article/details/ghleufppj.sHtML

[R54] 比较两个文件
来源：http://m.share.sjlbkw.cn/Article/details/gcmoaodzr.sHtML

diff a.txt b.txt
来源：http://www.blog.yfazqb.com/Article/details/gsyhlzwnl.sHtML

[R55] 压缩与解压
来源：http://read.share.yfazqb.com/Article/details/ghsqkonec.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.bbcook.cn/Article/details/garnduxfi.sHtML

[R56] 远程拷贝
来源：http://mobile.tarul.cn/Article/details/gkospqphr.sHtML

scp file user@host:/path/
来源：http://www.blog.yfazqb.com/Article/details/gocjhllgk.sHtML

[R57] 远程执行命令
来源：http://3g.fktsv.cn/Article/details/gasnblgnb.sHtML

ssh user@host 'uptime'
来源：http://www.share.epnwcf.com/Article/details/gpizuhwvx.sHtML

[R58] 下载文件
来源：http://www.blog.bbcook.cn/Article/details/gugytrfog.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.sjlbkw.cn/Article/details/gtblzjryq.sHtML

[R59] 发 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gveznsvph.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/glpshwfak.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gftxkadcp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.sjlbkw.cn/Article/details/gtrvtckaf.sHtML

[R61] 磁盘占用
来源：http://blog.bbcook.cn/Article/details/gkabwmebg.sHtML

df -h;  du -sh *
来源：http://baike.vehdjk.com/Article/details/gbvcmctft.sHtML

[R62] 找最占空间的文件
来源：http://wap.bbcook.cn/Article/details/gkkolsedh.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fktsv.cn/Article/details/gtflctgdq.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gnlfytjxx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.vehdjk.com/Article/details/ggsrehemo.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gdoenszdo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.tarul.cn/Article/details/gfyrncifl.sHtML

[R65] 查看端口占用
来源：http://baike.fktsv.cn/Article/details/gvqiafnno.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.epnwcf.com/Article/details/gdyamtsha.sHtML

[R66] 定时任务
来源：http://m.share.bbcook.cn/Article/details/gdqwmdrbv.sHtML

crontab -e;  crontab -l
来源：http://wap.vehdjk.com/Article/details/gdhfouhzz.sHtML

[R67] 生成随机十六进制串
来源：http://wap.epnwcf.com/Article/details/gjzotzaif.sHtML

openssl rand -hex 16
来源：http://m.share.vehdjk.com/Article/details/gnsehroeg.sHtML

[R68] 计算文件校验值
来源：http://www.share.vehdjk.com/Article/details/gzhufcoae.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.yfazqb.com/Article/details/gvupxwlmw.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/gxahlkbec.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.bbcook.cn/Article/details/gztsnegvy.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/gqklusjbc.sHtML

date +%s;  date -d @1700000000
来源：http://wap.yfazqb.com/Article/details/grmjyidli.sHtML

[R71] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gwpagluxs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.tarul.cn/Article/details/gsdluyhnu.sHtML

[R72] 等待端口就绪
来源：http://3g.epnwcf.com/Article/details/ggudvxyeh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gacgvwgfk.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/gesodoovg.sHtML

split -l 1000 big.log part_
来源：http://www.share.bbcook.cn/Article/details/gdqfvhjly.sHtML

[R74] 批量重命名
来源：http://read.share.vehdjk.com/Article/details/ghklymhip.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.sjlbkw.cn/Article/details/gwpoicrqn.sHtML

[R75] 导出环境变量
来源：http://3g.fktsv.cn/Article/details/gyogxzkbk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.bbcook.cn/Article/details/gjyyygojp.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/gjofmioax.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/globmycgg.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/ggtmnjmul.sHtML

read -rp "请输入: " ans
来源：http://wap.yfazqb.com/Article/details/gavhafzwo.sHtML

[R78] 交互式菜单
来源：http://www.m.share.sjlbkw.cn/Article/details/grvnefbfq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/glqlcptfq.sHtML

[R79] 解析命令行选项
来源：http://m.share.vehdjk.com/Article/details/gcqucstlq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/ggpimqdfu.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fktsv.cn/Article/details/gsbgvgypd.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/ggopdxews.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghgydauqc.sHtML

S. C / C++ 专题
来源：http://m.share.fktsv.cn/Article/details/gqhilaeyj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gzqcjxvfx.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/grwclkgwr.sHtML

#include <stdio.h>
来源：http://blog.fktsv.cn/Article/details/gyomhfeur.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/gdwjwtqmx.sHtML

[S02] C：变量与格式化输出
来源：http://wap.tarul.cn/Article/details/gqtpwqozf.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.tarul.cn/Article/details/gjuyrafme.sHtML

[S03] C：读入整数
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtfpilvz.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.epnwcf.com/Article/details/gfzbksjqp.sHtML

[S04] C：字符串复制
来源：http://baike.vehdjk.com/Article/details/gqxbnumqk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.vehdjk.com/Article/details/gexuatrwx.sHtML

[S05] C：字符串长度
来源：http://baike.bbcook.cn/Article/details/gweobimdy.sHtML

strlen(s)
来源：http://baike.fktsv.cn/Article/details/gyvazfhkj.sHtML

[S06] C：字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gepljupeq.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gdfwuiuhn.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.epnwcf.com/Article/details/gzbajnpvh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.yfazqb.com/Article/details/ginlgbhch.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gbngcytzx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.tarul.cn/Article/details/ggsdeagge.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.yfazqb.com/Article/details/gketjrgfc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fktsv.cn/Article/details/glimlblod.sHtML

[S10] C：指针与解引用
来源：http://wap.fktsv.cn/Article/details/gmpukwhdg.sHtML

int *p = &a;  *p = 5;
来源：http://wap.vehdjk.com/Article/details/ggzbouaam.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gungyhpzt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.epnwcf.com/Article/details/grbclvkmh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gpmixmdat.sHtML

fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/gvplcnsvr.sHtML

[S12] C：写文件
来源：http://www.share.epnwcf.com/Article/details/gqxbxjbys.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.yfazqb.com/Article/details/gilyznohm.sHtML

[S13] C：宏定义
来源：http://mobile.tarul.cn/Article/details/gxarrytbu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.yfazqb.com/Article/details/gydealqfo.sHtML

[S14] C：枚举
来源：http://www.m.share.tarul.cn/Article/details/gonfggqka.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.sjlbkw.cn/Article/details/gdlxrttwn.sHtML

[S15] C：类型转换
来源：http://baike.tarul.cn/Article/details/gwicnfpxu.sHtML

(double) a / b
来源：http://baike.tarul.cn/Article/details/gvuciwota.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/gwahlksyy.sHtML

x |= (1 << 3);
来源：http://3g.fktsv.cn/Article/details/gtrfdejkv.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gcetbdcgl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.tarul.cn/Article/details/gnuylhpae.sHtML

[S18] C：命令行参数
来源：http://read.share.yfazqb.com/Article/details/gluewymnh.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/ggmwpfhjl.sHtML

[S19] C：快速排序
来源：http://www.m.share.vehdjk.com/Article/details/gxedloxja.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/gwhowdnqz.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gsobuxkuq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/ggvetqiir.sHtML

[S21] C：字符类别判断
来源：http://blog.bbcook.cn/Article/details/gmsbvafpm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.vehdjk.com/Article/details/gjueebxgg.sHtML

[S22] C：字符串转数字
来源：http://wap.yfazqb.com/Article/details/gnjkdsofm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/gtivuvqga.sHtML

[S23] C：随机数
来源：http://www.share.bbcook.cn/Article/details/gdhrhevru.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/gardvqqkq.sHtML

[S24] C：获取本地时间
来源：http://baike.fktsv.cn/Article/details/gnxbftral.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/goshirqmi.sHtML

[S25] C：内存拷贝
来源：http://3g.epnwcf.com/Article/details/gqglsdthb.sHtML

memcpy(dst, src, n);
来源：http://baike.yfazqb.com/Article/details/grzuhptzr.sHtML

[S26] C：内存清零
来源：http://3g.yfazqb.com/Article/details/gvlhjmces.sHtML

memset(a, 0, sizeof a);
来源：http://wap.vehdjk.com/Article/details/gflvjiqtg.sHtML

[S27] C：定义常量
来源：http://mobile.fktsv.cn/Article/details/ggsnpybxs.sHtML

const double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gpnwlvrqe.sHtML

[S28] C：静态变量
来源：http://mobile.fktsv.cn/Article/details/gcuorrliu.sHtML

static int counter = 0;
来源：http://read.share.vehdjk.com/Article/details/gzmvruwgj.sHtML

[S29] C：变参函数
来源：http://m.share.tarul.cn/Article/details/gshfrndki.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/gxbafzxsz.sHtML

[S30] C：头文件保护
来源：http://wap.vehdjk.com/Article/details/gxgyuzgji.sHtML

#ifndef X_H
来源：http://www.blog.vehdjk.com/Article/details/gseydcrbz.sHtML

#define X_H
来源：http://www.share.tarul.cn/Article/details/gkrqzdjhb.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/gwmdtigbn.sHtML

[S31] C++：Hello World
来源：http://read.share.fktsv.cn/Article/details/gkenbgfzx.sHtML

#include <iostream>
来源：http://baike.bbcook.cn/Article/details/gbnzzzjnk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.yfazqb.com/Article/details/gcxurehwp.sHtML

[S32] C++：字符串
来源：http://read.share.epnwcf.com/Article/details/gwgnwvvmm.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.sjlbkw.cn/Article/details/gstoaqltt.sHtML

[S33] C++：vector 增删
来源：http://www.blog.yfazqb.com/Article/details/gopowvavn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.bbcook.cn/Article/details/gocgqnbgt.sHtML

[S34] C++：遍历 vector
来源：http://wap.bbcook.cn/Article/details/gzwhprtbt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.vehdjk.com/Article/details/gxplomell.sHtML

[S35] C++：map
来源：http://mobile.fktsv.cn/Article/details/gmrtbdnqm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/gmtoelvls.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/gsvedhazf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gnobqmvir.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/gdqqinxzu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.epnwcf.com/Article/details/gkgtivevc.sHtML

[S38] C++：排序
来源：http://www.blog.fktsv.cn/Article/details/gubigalik.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.vehdjk.com/Article/details/gisvzstdf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.vehdjk.com/Article/details/gnxpjijow.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.vehdjk.com/Article/details/gwuiwzmmo.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/ggfrbvftz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fktsv.cn/Article/details/gfpkbvuuo.sHtML

[S41] C++：类与构造函数
来源：http://baike.tarul.cn/Article/details/gsqruyhpp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.bbcook.cn/Article/details/gzdxjzfca.sHtML

[S42] C++：继承与虚函数
来源：http://blog.bbcook.cn/Article/details/gjstguikn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.vehdjk.com/Article/details/gusiaecjw.sHtML

[S43] C++：智能指针
来源：http://read.share.yfazqb.com/Article/details/gczmcosxn.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.sjlbkw.cn/Article/details/gyjlvzqlj.sHtML

[S44] C++：引用传参
来源：http://read.share.tarul.cn/Article/details/gnlqppuaf.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwvkbins.sHtML

[S45] C++：lambda
来源：http://m.share.epnwcf.com/Article/details/gwkshkpog.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.tarul.cn/Article/details/goihvnlgc.sHtML

[S46] C++：函数模板
来源：http://wap.bbcook.cn/Article/details/gfmzohngt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fktsv.cn/Article/details/gqlrsmags.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.bbcook.cn/Article/details/gltqksspv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.bbcook.cn/Article/details/gdfjtqrwb.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gnatioela.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.epnwcf.com/Article/details/gwejvmvrv.sHtML

while (std::getline(in, line)) { }
来源：http://baike.bbcook.cn/Article/details/gmdhvfazm.sHtML

[S49] C++：写文件
来源：http://3g.fktsv.cn/Article/details/gkfgkccra.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.yfazqb.com/Article/details/gqiiqrcpf.sHtML

[S50] C++：格式化数字
来源：http://read.share.bbcook.cn/Article/details/goswpcogi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/gsqaokaes.sHtML

[S51] C++：显式类型转换
来源：http://www.share.vehdjk.com/Article/details/gssxcbvgh.sHtML

static_cast<double>(a) / b
来源：http://3g.yfazqb.com/Article/details/gkdhwgqwt.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fktsv.cn/Article/details/gimtkblyd.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.sjlbkw.cn/Article/details/gqiyrhguh.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/gerfwwxoh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.epnwcf.com/Article/details/gmmwehtuu.sHtML

[S54] C++：异常处理
来源：http://3g.fktsv.cn/Article/details/gfucxyvvu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.sjlbkw.cn/Article/details/gkhctprdj.sHtML

[S55] C++：结构化绑定
来源：http://wap.yfazqb.com/Article/details/gjhxcpntr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fktsv.cn/Article/details/goragbqny.sHtML

[S56] C++：optional
来源：http://wap.yfazqb.com/Article/details/gcimpdeqt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.epnwcf.com/Article/details/gyxwhrjeo.sHtML

[S57] C++：编译期常量
来源：http://blog.tarul.cn/Article/details/giupfovfi.sHtML

constexpr int N = 10;
来源：http://read.share.fktsv.cn/Article/details/gjhgbxjyw.sHtML

[S58] C++：命名空间
来源：http://read.share.fktsv.cn/Article/details/gmjekvaoy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/gbogxkpcu.sHtML

[S59] C++：静态断言
来源：http://www.share.epnwcf.com/Article/details/ggbqeygcw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.bbcook.cn/Article/details/gcalpqles.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnjdwgzm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.bbcook.cn/Article/details/gxdmedppm.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjpivqkvh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.epnwcf.com/Article/details/ghwiccvxf.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gytexpvyo.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fktsv.cn/Article/details/gjhnmtlmk.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gfzuytmrj.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fktsv.cn/Article/details/gsxhhkyrf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.vehdjk.com/Article/details/gyoebbdew.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.epnwcf.com/Article/details/gctckhpvb.sHtML

"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gkahihkly.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/grachzkjt.sHtML

val n: String? = null;  n?.length
来源：http://baike.epnwcf.com/Article/details/gbqddnhkw.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.vehdjk.com/Article/details/gkxmswmre.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.yfazqb.com/Article/details/guygkegxf.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.bbcook.cn/Article/details/gietmpszb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.tarul.cn/Article/details/gmhujxdxi.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/giyafqugg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/gublglxxf.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.sjlbkw.cn/Article/details/gzngrzbzq.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.tarul.cn/Article/details/gryyrnjpo.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.vehdjk.com/Article/details/gthelyhmi.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.sjlbkw.cn/Article/details/gptcphdov.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fktsv.cn/Article/details/gopelrkeo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.yfazqb.com/Article/details/gphxwrjlw.sHtML

[T11] Kotlin：协程
来源：http://read.share.epnwcf.com/Article/details/golwlivlb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.epnwcf.com/Article/details/genyyragm.sHtML

[T12] Kotlin：解构声明
来源：http://wap.bbcook.cn/Article/details/gwscslqlz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.epnwcf.com/Article/details/geyhjozfa.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.bbcook.cn/Article/details/ghebbamec.sHtML

val m = mapOf("a" to 1)
来源：http://3g.bbcook.cn/Article/details/gqkazqfkg.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/gtklbhiwk.sHtML

for (i in 1..10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gbqewsxbi.sHtML

[T15] Kotlin：接口
来源：http://3g.yfazqb.com/Article/details/gjbxcaffc.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.tarul.cn/Article/details/gquhbpwhz.sHtML

[T16] Swift：Hello World
来源：http://baike.vehdjk.com/Article/details/girtcpkde.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/grwmwgdpo.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.tarul.cn/Article/details/ghknndphk.sHtML

var a = 1;  let b = 2
来源：http://m.share.fktsv.cn/Article/details/gqfrkrjte.sHtML

[T18] Swift：字符串插值
来源：http://baike.epnwcf.com/Article/details/gdkfumkcs.sHtML

"值: \(b)"
来源：http://blog.tarul.cn/Article/details/ggnoujufb.sHtML

[T19] Swift：可选绑定
来源：http://m.share.vehdjk.com/Article/details/gqwoswdei.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fktsv.cn/Article/details/gkwkztfqw.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.yfazqb.com/Article/details/gbiopoqpa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fktsv.cn/Article/details/gxztotoxu.sHtML

[T21] Swift：遍历
来源：http://www.share.bbcook.cn/Article/details/gqlmmukex.sHtML

for x in a { print(x) }
来源：http://baike.epnwcf.com/Article/details/gzgskmstm.sHtML

[T22] Swift：字典
来源：http://wap.sjlbkw.cn/Article/details/gomvjwmlx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.sjlbkw.cn/Article/details/ggwjvwbsr.sHtML

[T23] Swift：函数
来源：http://blog.bbcook.cn/Article/details/godgooerg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.bbcook.cn/Article/details/ghhptniqa.sHtML

[T24] Swift：闭包
来源：http://wap.yfazqb.com/Article/details/gnqcheokv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fktsv.cn/Article/details/gbebmesgf.sHtML

[T25] Swift：结构体
来源：http://www.blog.yfazqb.com/Article/details/gzijfnebb.sHtML

struct P { var x: Int }
来源：http://3g.yfazqb.com/Article/details/gswwpfrot.sHtML

[T26] Swift：类与重写
来源：http://wap.sjlbkw.cn/Article/details/glquwqift.sHtML

class A: Base { override func f() {} }
来源：http://m.share.tarul.cn/Article/details/gzotedgsz.sHtML

[T27] Swift：错误处理
来源：http://blog.tarul.cn/Article/details/gzeaamhxm.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fktsv.cn/Article/details/gwyiplhrh.sHtML

[T28] Swift：枚举
来源：http://wap.sjlbkw.cn/Article/details/gnaqmjwuj.sHtML

enum Color { case red, green }
来源：http://www.share.vehdjk.com/Article/details/gvxzogxym.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fktsv.cn/Article/details/gdpaslvjm.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/gtzaqgtjs.sHtML

[T30] Swift：协议
来源：http://mobile.vehdjk.com/Article/details/gegsgoxkk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.epnwcf.com/Article/details/gcakclqgl.sHtML

[T31] Lua：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gmkqrnwcn.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/gxkjgxqli.sHtML

[T32] Lua：局部变量
来源：http://wap.bbcook.cn/Article/details/gcerqytdh.sHtML

local a = 1
来源：http://www.m.share.yfazqb.com/Article/details/gfdfrnwer.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/gbxdvaagw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.vehdjk.com/Article/details/gyvrklofc.sHtML

[T34] Lua：遍历表
来源：http://www.share.vehdjk.com/Article/details/gpksfqmgf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.epnwcf.com/Article/details/ggkpxudgw.sHtML

[T35] Lua：字典表
来源：http://blog.fktsv.cn/Article/details/gtdnwblff.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.tarul.cn/Article/details/grmcgjhcc.sHtML

[T36] Lua：函数
来源：http://www.m.share.vehdjk.com/Article/details/gvvrsmlsw.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.bbcook.cn/Article/details/gvuqhnjuo.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gtarnfoit.sHtML

"a" .. "b"
来源：http://m.share.fktsv.cn/Article/details/gtovwgpny.sHtML

[T38] Lua：条件
来源：http://www.share.fktsv.cn/Article/details/gmuazvvrz.sHtML

if x > 0 then print("正") end
来源：http://read.share.fktsv.cn/Article/details/gfjakohwv.sHtML

[T39] Lua：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gqauzobvh.sHtML

string.find(s, "%d+")
来源：http://blog.epnwcf.com/Article/details/gddryeksq.sHtML

[T40] Lua：元表
来源：http://baike.tarul.cn/Article/details/gwbrbhaht.sHtML

setmetatable({}, { __index = base })
来源：http://3g.epnwcf.com/Article/details/gxxefvihq.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gzzytanyo.sHtML

print "Hello\n";
来源：http://www.blog.sjlbkw.cn/Article/details/gxegycsfx.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/gewqcqjbp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fktsv.cn/Article/details/gwnfmlbee.sHtML

[T43] Perl：字符串插值
来源：http://3g.fktsv.cn/Article/details/gvjpacgpv.sHtML

"值: $a"
来源：http://www.blog.fktsv.cn/Article/details/gncaqyklu.sHtML

[T44] Perl：条件
来源：http://www.blog.yfazqb.com/Article/details/gqwboulka.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.vehdjk.com/Article/details/gclmxlfcz.sHtML

[T45] Perl：数组遍历
来源：http://3g.epnwcf.com/Article/details/gwdrrormb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.yfazqb.com/Article/details/gntxyxtli.sHtML

[T46] Perl：哈希操作
来源：http://blog.bbcook.cn/Article/details/gnpawpbmp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.bbcook.cn/Article/details/gxutmoeny.sHtML

[T47] Perl：正则捕获
来源：http://mobile.epnwcf.com/Article/details/golldbpmg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkyiswbvi.sHtML

[T48] Perl：正则替换
来源：http://mobile.bbcook.cn/Article/details/gdfztxuba.sHtML

$s =~ s/old/new/g;
来源：http://www.share.sjlbkw.cn/Article/details/gkllnhgri.sHtML


<!-- 参考信息 -->