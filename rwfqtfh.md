代发 wailian999

find . -name "*.log" -type f
来源：http://www.blog.tarul.cn/Article/details/gkgbevcsf.sHtML

[R44] 按修改时间查找
来源：http://mobile.sjlbkw.cn/Article/details/giuxqiwvt.sHtML

find . -mtime -7 -type f
来源：http://3g.tarul.cn/Article/details/girrdmerj.sHtML

[R45] 批量删除
来源：http://m.share.yfazqb.com/Article/details/gtnaerclv.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.bbcook.cn/Article/details/gcjvooapl.sHtML

[R46] 递归替换文件内容
来源：http://m.share.yfazqb.com/Article/details/gffbpqfsy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.sjlbkw.cn/Article/details/gqnrygltb.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/gdumvrpud.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.yfazqb.com/Article/details/gxiyoubiu.sHtML

[R48] awk 取指定列
来源：http://mobile.epnwcf.com/Article/details/glaffipma.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fktsv.cn/Article/details/ghezqejtn.sHtML

[R49] awk 带条件
来源：http://blog.fktsv.cn/Article/details/gxldmtspn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.yfazqb.com/Article/details/gwdzwhcrb.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gpxicvjcq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gosyvdwyg.sHtML

[R51] 排序去重取前几
来源：http://www.share.yfazqb.com/Article/details/gwsgvmczz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.yfazqb.com/Article/details/geqyvccgz.sHtML

[R52] 统计行数
来源：http://m.share.vehdjk.com/Article/details/gzuvtrrhr.sHtML

wc -l a.txt
来源：http://m.share.epnwcf.com/Article/details/gtsuyhkrq.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fktsv.cn/Article/details/gudylaikd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/gfhrorseo.sHtML

[R54] 比较两个文件
来源：http://www.blog.sjlbkw.cn/Article/details/gcbnbwnia.sHtML

diff a.txt b.txt
来源：http://3g.epnwcf.com/Article/details/gmnlhfrav.sHtML

[R55] 压缩与解压
来源：http://mobile.bbcook.cn/Article/details/gljwskmwn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.vehdjk.com/Article/details/gyryxqgcm.sHtML

[R56] 远程拷贝
来源：http://baike.sjlbkw.cn/Article/details/gkxtkfbre.sHtML

scp file user@host:/path/
来源：http://www.blog.vehdjk.com/Article/details/gfzpxsrvp.sHtML

[R57] 远程执行命令
来源：http://baike.tarul.cn/Article/details/gndfmqula.sHtML

ssh user@host 'uptime'
来源：http://www.blog.bbcook.cn/Article/details/gpvkjfccx.sHtML

[R58] 下载文件
来源：http://mobile.tarul.cn/Article/details/gpusfcgvh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.yfazqb.com/Article/details/gvmijjpml.sHtML

[R59] 发 POST JSON
来源：http://read.share.tarul.cn/Article/details/gqgpczjyp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fktsv.cn/Article/details/gatrnosvs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gafdgvnkw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gbvuvztyz.sHtML

[R61] 磁盘占用
来源：http://blog.epnwcf.com/Article/details/gvstnkols.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/gpmtjkntg.sHtML

[R62] 找最占空间的文件
来源：http://mobile.vehdjk.com/Article/details/gdufzgztq.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.sjlbkw.cn/Article/details/gaoeqykah.sHtML

[R63] 内存与进程
来源：http://www.share.epnwcf.com/Article/details/gfppjdzje.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.bbcook.cn/Article/details/gbpkkvvme.sHtML

[R64] 结束进程
来源：http://m.share.yfazqb.com/Article/details/ggrxsecnq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.bbcook.cn/Article/details/gkfzuvnzz.sHtML

[R65] 查看端口占用
来源：http://read.share.bbcook.cn/Article/details/geoytuzaf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.epnwcf.com/Article/details/gpcjnabpr.sHtML

[R66] 定时任务
来源：http://blog.fktsv.cn/Article/details/geqkvbmrm.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.epnwcf.com/Article/details/grkdvwweh.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/gdyziuvdj.sHtML

openssl rand -hex 16
来源：http://read.share.epnwcf.com/Article/details/gcpcnfemi.sHtML

[R68] 计算文件校验值
来源：http://m.share.sjlbkw.cn/Article/details/gbbjphqtb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.yfazqb.com/Article/details/glssjwejl.sHtML

[R69] 生成随机密码
来源：http://m.share.tarul.cn/Article/details/gaqrhgoam.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.bbcook.cn/Article/details/ggeiwphsf.sHtML

[R70] 时间戳与互转
来源：http://baike.yfazqb.com/Article/details/ggtbdozjm.sHtML

date +%s;  date -d @1700000000
来源：http://baike.yfazqb.com/Article/details/gbelfwjwu.sHtML

[R71] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/gmfhytyeb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.bbcook.cn/Article/details/goyyibvck.sHtML

[R72] 等待端口就绪
来源：http://blog.tarul.cn/Article/details/gnfbyehxm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gkgegfsnv.sHtML

[R73] 分割大日志
来源：http://www.blog.vehdjk.com/Article/details/gihrbfrxx.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.epnwcf.com/Article/details/gofzelmpz.sHtML

[R74] 批量重命名
来源：http://m.share.bbcook.cn/Article/details/gslkhwcob.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.yfazqb.com/Article/details/gibssvwck.sHtML

[R75] 导出环境变量
来源：http://blog.vehdjk.com/Article/details/gjpvotkkr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.yfazqb.com/Article/details/gvovktynj.sHtML

[R76] 使用临时文件
来源：http://www.blog.sjlbkw.cn/Article/details/gnulvtigc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gevavkjxc.sHtML

[R77] 读取用户输入
来源：http://blog.sjlbkw.cn/Article/details/gailtscvc.sHtML

read -rp "请输入: " ans
来源：http://baike.tarul.cn/Article/details/gjudndrtr.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/gnxkqjosa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fktsv.cn/Article/details/giycfnfys.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.bbcook.cn/Article/details/gyzsldnnl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.tarul.cn/Article/details/giaqzogkt.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.vehdjk.com/Article/details/gysghevpk.sHtML

time ./run.sh
来源：http://blog.vehdjk.com/Article/details/gpkrovyic.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqvqsxtae.sHtML

S. C / C++ 专题
来源：http://baike.tarul.cn/Article/details/gdzzcmqox.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcyjzhyja.sHtML

[S01] C：Hello World
来源：http://3g.sjlbkw.cn/Article/details/ggcevvstk.sHtML

#include <stdio.h>
来源：http://wap.fktsv.cn/Article/details/grvtpmcib.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.tarul.cn/Article/details/gjlrzggys.sHtML

[S02] C：变量与格式化输出
来源：http://blog.tarul.cn/Article/details/gxpxdboxz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.sjlbkw.cn/Article/details/gfeglupsg.sHtML

[S03] C：读入整数
来源：http://www.share.epnwcf.com/Article/details/gcyscnnrn.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fktsv.cn/Article/details/gvnslrlpi.sHtML

[S04] C：字符串复制
来源：http://3g.vehdjk.com/Article/details/gftfmiqde.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.sjlbkw.cn/Article/details/grjuxgdle.sHtML

[S05] C：字符串长度
来源：http://wap.vehdjk.com/Article/details/gcdfqjasg.sHtML

strlen(s)
来源：http://read.share.bbcook.cn/Article/details/gmtukczbl.sHtML

[S06] C：字符串比较
来源：http://3g.fktsv.cn/Article/details/gphgbejrm.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gqtmkmepd.sHtML

[S07] C：数组遍历求和
来源：http://mobile.vehdjk.com/Article/details/gdehsinwf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.epnwcf.com/Article/details/gkpwwkwwp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fktsv.cn/Article/details/gngniptyr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.epnwcf.com/Article/details/gwxefyejd.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.vehdjk.com/Article/details/gtdwprcsu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.bbcook.cn/Article/details/gjriyoogi.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.vehdjk.com/Article/details/gtmehzaaw.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/gcrdjlqve.sHtML

[S11] C：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gssbdothf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.tarul.cn/Article/details/gramgydbr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gopgsbups.sHtML

fclose(f);
来源：http://baike.tarul.cn/Article/details/gjtkjbiwg.sHtML

[S12] C：写文件
来源：http://baike.bbcook.cn/Article/details/geiydmrjs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fktsv.cn/Article/details/gocvjxrjx.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gfkqzxnvb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gghzadjeg.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/gxxdpanrd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.sjlbkw.cn/Article/details/glvicbvxu.sHtML

[S15] C：类型转换
来源：http://mobile.epnwcf.com/Article/details/gyjezpwyz.sHtML

(double) a / b
来源：http://www.blog.yfazqb.com/Article/details/gxazmpcyr.sHtML

[S16] C：位操作置位
来源：http://3g.vehdjk.com/Article/details/gagtwlipn.sHtML

x |= (1 << 3);
来源：http://blog.epnwcf.com/Article/details/gtzxrywom.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/gkdixlvkg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.sjlbkw.cn/Article/details/gqzwiwvjq.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/gpzylinpv.sHtML

int main(int argc, char **argv)
来源：http://www.blog.tarul.cn/Article/details/gkockhuhk.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/gkavpyeud.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/gvsdapgjw.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gbqlpzmwd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gzbmmkitf.sHtML

[S21] C：字符类别判断
来源：http://wap.vehdjk.com/Article/details/gktykotnd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.tarul.cn/Article/details/gndmjtter.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/gaflxppbw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.tarul.cn/Article/details/gpshhlzld.sHtML

[S23] C：随机数
来源：http://www.share.yfazqb.com/Article/details/gcvyeocoh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgleyynv.sHtML

[S24] C：获取本地时间
来源：http://m.share.fktsv.cn/Article/details/gsoozjrxh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.sjlbkw.cn/Article/details/ghrjaaugp.sHtML

[S25] C：内存拷贝
来源：http://read.share.bbcook.cn/Article/details/gsgsiidjy.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/gqdsmuxvk.sHtML

[S26] C：内存清零
来源：http://baike.epnwcf.com/Article/details/gmpiknvzn.sHtML

memset(a, 0, sizeof a);
来源：http://baike.sjlbkw.cn/Article/details/ggudnuain.sHtML

[S27] C：定义常量
来源：http://www.share.bbcook.cn/Article/details/gahdooopp.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gxlqugtcn.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gmfcwvbnh.sHtML

static int counter = 0;
来源：http://m.share.sjlbkw.cn/Article/details/gmjajxmjq.sHtML

[S29] C：变参函数
来源：http://mobile.vehdjk.com/Article/details/gclvfntby.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/gqhaiemie.sHtML

[S30] C：头文件保护
来源：http://www.blog.sjlbkw.cn/Article/details/gcfbpwfcc.sHtML

#ifndef X_H
来源：http://mobile.fktsv.cn/Article/details/gbvzqzfjj.sHtML

#define X_H
来源：http://wap.vehdjk.com/Article/details/gikfvbzup.sHtML

#endif
来源：http://3g.epnwcf.com/Article/details/gwqwbcktw.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/ghdxnryqh.sHtML

#include <iostream>
来源：http://baike.fktsv.cn/Article/details/gmwkcbwzt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.sjlbkw.cn/Article/details/glvlndpdy.sHtML

[S32] C++：字符串
来源：http://www.blog.fktsv.cn/Article/details/gaqtbgksy.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.epnwcf.com/Article/details/guklfaxsw.sHtML

[S33] C++：vector 增删
来源：http://www.blog.vehdjk.com/Article/details/gqcckdiez.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.epnwcf.com/Article/details/gppccnzlt.sHtML

[S34] C++：遍历 vector
来源：http://mobile.yfazqb.com/Article/details/gimxfmxqr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.tarul.cn/Article/details/grtcxrdtu.sHtML

[S35] C++：map
来源：http://www.blog.yfazqb.com/Article/details/glvvqxmzz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/gsheohgpd.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/gjwpvacbu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gbcyoqtav.sHtML

[S37] C++：set
来源：http://www.share.sjlbkw.cn/Article/details/grekjvqdz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/guurzmniv.sHtML

[S38] C++：排序
来源：http://www.blog.tarul.cn/Article/details/gsxeilibj.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fktsv.cn/Article/details/gbpauonjl.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fktsv.cn/Article/details/giwrdqepb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.bbcook.cn/Article/details/gkfkwuerq.sHtML

[S40] C++：查找元素
来源：http://3g.yfazqb.com/Article/details/gcwdtqyuj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.yfazqb.com/Article/details/gsrbzdtsd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/gqbexbipr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.yfazqb.com/Article/details/gsqkljgtf.sHtML

[S42] C++：继承与虚函数
来源：http://3g.sjlbkw.cn/Article/details/gewpcpuxh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fktsv.cn/Article/details/gtsctdjsk.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrnivdqp.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.tarul.cn/Article/details/glawwdzla.sHtML

[S44] C++：引用传参
来源：http://m.share.sjlbkw.cn/Article/details/gufnsafyo.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fktsv.cn/Article/details/glawtqbpn.sHtML

[S45] C++：lambda
来源：http://www.blog.fktsv.cn/Article/details/ggcbdqxbj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.yfazqb.com/Article/details/gzmlptyds.sHtML

[S46] C++：函数模板
来源：http://www.share.fktsv.cn/Article/details/gtzrirnqo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.yfazqb.com/Article/details/gsjzvttmw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.vehdjk.com/Article/details/girwsijmi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.epnwcf.com/Article/details/gcnccttpr.sHtML

[S48] C++：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gpcjdqxou.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fktsv.cn/Article/details/gfxclelts.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.tarul.cn/Article/details/guseyrmqa.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/grnwmduad.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.epnwcf.com/Article/details/gmkitjdsj.sHtML

[S50] C++：格式化数字
来源：http://mobile.epnwcf.com/Article/details/gxnduotbl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.yfazqb.com/Article/details/gwziozxgf.sHtML

[S51] C++：显式类型转换
来源：http://www.share.epnwcf.com/Article/details/gxexiydap.sHtML

static_cast<double>(a) / b
来源：http://www.share.sjlbkw.cn/Article/details/gjkhfgjpr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fktsv.cn/Article/details/gdmzkcuuo.sHtML

int size() const noexcept { return n_; }
来源：http://blog.vehdjk.com/Article/details/gklwhrkzz.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/grtnpwyym.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.epnwcf.com/Article/details/gbfixfbij.sHtML

[S54] C++：异常处理
来源：http://read.share.epnwcf.com/Article/details/gfvjdmpkt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.epnwcf.com/Article/details/gjdjwgvfr.sHtML

[S55] C++：结构化绑定
来源：http://blog.yfazqb.com/Article/details/gbkncapwa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/gytboymlj.sHtML

[S56] C++：optional
来源：http://m.share.epnwcf.com/Article/details/gwelvpywo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/gtvipccpj.sHtML

[S57] C++：编译期常量
来源：http://wap.vehdjk.com/Article/details/gjjchoilc.sHtML

constexpr int N = 10;
来源：http://wap.vehdjk.com/Article/details/glwncywex.sHtML

[S58] C++：命名空间
来源：http://3g.sjlbkw.cn/Article/details/gakodpxgn.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.bbcook.cn/Article/details/gzpaongyz.sHtML

[S59] C++：静态断言
来源：http://www.m.share.yfazqb.com/Article/details/gzyayhhny.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.tarul.cn/Article/details/gputwuwqd.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.bbcook.cn/Article/details/gwjjikmpy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/gtbfyzcgo.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grfpfpbig.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fktsv.cn/Article/details/gkoikknzk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gezeuhyja.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fktsv.cn/Article/details/gxbandxkq.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gwhqrgfrd.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fktsv.cn/Article/details/gssdbgcba.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fktsv.cn/Article/details/gibulczhc.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.vehdjk.com/Article/details/gdhaefppx.sHtML

"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gennwcvpi.sHtML

[T04] Kotlin：空安全
来源：http://wap.tarul.cn/Article/details/ganqjzzgn.sHtML

val n: String? = null;  n?.length
来源：http://baike.bbcook.cn/Article/details/gxvkkrtbn.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.epnwcf.com/Article/details/gjvzzrass.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/gnafdznwj.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fktsv.cn/Article/details/gqhcjdnar.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gyidhvhti.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.tarul.cn/Article/details/gcjzxoqns.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.yfazqb.com/Article/details/gwhbulyst.sHtML

[T08] Kotlin：数据类
来源：http://read.share.vehdjk.com/Article/details/ghwtgoklo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/guplcjros.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.sjlbkw.cn/Article/details/gtfsgypel.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.sjlbkw.cn/Article/details/gmbaxwtjg.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.epnwcf.com/Article/details/godngqmiq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.bbcook.cn/Article/details/gfseuyzrs.sHtML

[T11] Kotlin：协程
来源：http://baike.bbcook.cn/Article/details/gmtbjqfhj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.tarul.cn/Article/details/gkgemyqsa.sHtML

[T12] Kotlin：解构声明
来源：http://wap.vehdjk.com/Article/details/gsipfonvi.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.epnwcf.com/Article/details/gejyiapua.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.vehdjk.com/Article/details/gopubvyjj.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.tarul.cn/Article/details/gavawivse.sHtML

[T14] Kotlin：循环
来源：http://mobile.epnwcf.com/Article/details/gdbfhowyu.sHtML

for (i in 1..10) println(i)
来源：http://www.share.tarul.cn/Article/details/gxduaoocm.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.yfazqb.com/Article/details/gppihvubl.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.tarul.cn/Article/details/gflbukcon.sHtML

[T16] Swift：Hello World
来源：http://read.share.epnwcf.com/Article/details/gpaopkqnw.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gneiwqitl.sHtML

[T17] Swift：变量与常量
来源：http://3g.vehdjk.com/Article/details/ggujtczvz.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/gncbqbdfu.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/grepqnayj.sHtML

"值: \(b)"
来源：http://mobile.fktsv.cn/Article/details/gmhfpssvn.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.bbcook.cn/Article/details/gzigjwrnr.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcnenqum.sHtML

[T20] Swift：数组操作
来源：http://blog.fktsv.cn/Article/details/gnrmohgon.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.yfazqb.com/Article/details/gczpfzcyj.sHtML

[T21] Swift：遍历
来源：http://m.share.bbcook.cn/Article/details/ggauedzyw.sHtML

for x in a { print(x) }
来源：http://www.blog.yfazqb.com/Article/details/gpqdabaph.sHtML

[T22] Swift：字典
来源：http://blog.sjlbkw.cn/Article/details/gsaspncin.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/glyybnyit.sHtML

[T23] Swift：函数
来源：http://3g.fktsv.cn/Article/details/gqzxcwbsh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.yfazqb.com/Article/details/gtrwexqdx.sHtML

[T24] Swift：闭包
来源：http://read.share.yfazqb.com/Article/details/glbhnhzrb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/glkidezzx.sHtML

[T25] Swift：结构体
来源：http://mobile.sjlbkw.cn/Article/details/gxfkxddvd.sHtML

struct P { var x: Int }
来源：http://www.m.share.fktsv.cn/Article/details/galsvcxks.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/godufzyoc.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fktsv.cn/Article/details/grxrndhhj.sHtML

[T27] Swift：错误处理
来源：http://m.share.yfazqb.com/Article/details/gjznbfqxa.sHtML

do { try f() } catch { print(error) }
来源：http://3g.sjlbkw.cn/Article/details/gqkbxllsf.sHtML

[T28] Swift：枚举
来源：http://blog.sjlbkw.cn/Article/details/guqfzxkal.sHtML

enum Color { case red, green }
来源：http://baike.bbcook.cn/Article/details/gibadssnu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.epnwcf.com/Article/details/gtznejqhq.sHtML

guard let x = opt else { return }
来源：http://wap.tarul.cn/Article/details/gagckhuco.sHtML

[T30] Swift：协议
来源：http://read.share.vehdjk.com/Article/details/gqqnbaulz.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.sjlbkw.cn/Article/details/gdcgijlvb.sHtML

[T31] Lua：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gexzmbtde.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gcdilffjx.sHtML

[T32] Lua：局部变量
来源：http://mobile.epnwcf.com/Article/details/guyoppmyp.sHtML

local a = 1
来源：http://mobile.bbcook.cn/Article/details/gezvqndqi.sHtML

[T33] Lua：表（数组）
来源：http://m.share.sjlbkw.cn/Article/details/gzbrghata.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fktsv.cn/Article/details/gwnliyyou.sHtML

[T34] Lua：遍历表
来源：http://mobile.vehdjk.com/Article/details/grjghtphr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.bbcook.cn/Article/details/grpvxduzv.sHtML

[T35] Lua：字典表
来源：http://blog.bbcook.cn/Article/details/gqgqbrwme.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gajtuvyqu.sHtML

[T36] Lua：函数
来源：http://m.share.yfazqb.com/Article/details/gjbynyfij.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtxjmtxs.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.yfazqb.com/Article/details/ghigrlkok.sHtML

"a" .. "b"
来源：http://mobile.epnwcf.com/Article/details/gbyaepvxq.sHtML

[T38] Lua：条件
来源：http://m.share.sjlbkw.cn/Article/details/gtiddkqvk.sHtML

if x > 0 then print("正") end
来源：http://wap.tarul.cn/Article/details/gnxyeqbmn.sHtML

[T39] Lua：模式匹配
来源：http://m.share.tarul.cn/Article/details/gcnrpszbf.sHtML

string.find(s, "%d+")
来源：http://blog.epnwcf.com/Article/details/ggkwmzwqc.sHtML

[T40] Lua：元表
来源：http://read.share.yfazqb.com/Article/details/gkqanxudn.sHtML

setmetatable({}, { __index = base })
来源：http://3g.tarul.cn/Article/details/gtuockwdb.sHtML

[T41] Perl：Hello World
来源：http://www.share.yfazqb.com/Article/details/guuhjxmbu.sHtML

print "Hello\n";
来源：http://m.share.bbcook.cn/Article/details/ghyssbuzs.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/giuvlpakk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.yfazqb.com/Article/details/guhakwkcc.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/giucpkmaa.sHtML

"值: $a"
来源：http://baike.bbcook.cn/Article/details/gnpltwhzz.sHtML

[T44] Perl：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/grxtbjfon.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.bbcook.cn/Article/details/gsmjeiumq.sHtML

[T45] Perl：数组遍历
来源：http://3g.yfazqb.com/Article/details/gvrdcdojf.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.tarul.cn/Article/details/gqlhvqqeh.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fktsv.cn/Article/details/gcdhgkyqz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.epnwcf.com/Article/details/gxrhjxjqs.sHtML


<!-- 参考信息 -->