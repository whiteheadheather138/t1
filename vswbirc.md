代发 wailian999

cmd >/dev/null 2>&1
来源：http://read.share.bbcook.cn/Article/details/gjzeqrghk.sHtML

[R42] 输入重定向
来源：http://blog.epnwcf.com/Article/details/gyanzmxyg.sHtML

wc -l < a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gvmlkplhv.sHtML

[R43] 按名字查找文件
来源：http://3g.vehdjk.com/Article/details/glfyemcss.sHtML

find . -name "*.log" -type f
来源：http://mobile.fktsv.cn/Article/details/gbfpleplb.sHtML

[R44] 按修改时间查找
来源：http://3g.tarul.cn/Article/details/gnzsbbfck.sHtML

find . -mtime -7 -type f
来源：http://blog.vehdjk.com/Article/details/gxlxigwww.sHtML

[R45] 批量删除
来源：http://mobile.sjlbkw.cn/Article/details/gwomggvte.sHtML

find . -name "*.tmp" -delete
来源：http://baike.bbcook.cn/Article/details/gqcebdwyo.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.vehdjk.com/Article/details/gsdsjyrhi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.sjlbkw.cn/Article/details/gomwyyokj.sHtML

[R47] sed 单行替换
来源：http://read.share.epnwcf.com/Article/details/gapeskbph.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fktsv.cn/Article/details/gzzvukxol.sHtML

[R48] awk 取指定列
来源：http://www.share.fktsv.cn/Article/details/gfezwaeoy.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fktsv.cn/Article/details/glvizbtor.sHtML

[R49] awk 带条件
来源：http://wap.fktsv.cn/Article/details/gxfsdtikv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fktsv.cn/Article/details/gtsyhowac.sHtML

[R50] awk 求和
来源：http://mobile.sjlbkw.cn/Article/details/gdtibyzgl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gtwgcfvex.sHtML

[R51] 排序去重取前几
来源：http://read.share.sjlbkw.cn/Article/details/gewueqzvn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.epnwcf.com/Article/details/gacateaar.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/glmebuymr.sHtML

wc -l a.txt
来源：http://www.blog.fktsv.cn/Article/details/gnzzhfkxj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.epnwcf.com/Article/details/grkddglmq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fktsv.cn/Article/details/gouunkjzu.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/getuozlgc.sHtML

diff a.txt b.txt
来源：http://www.blog.bbcook.cn/Article/details/gyawkfzhl.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/grvidvdld.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.tarul.cn/Article/details/grzbbapsy.sHtML

[R56] 远程拷贝
来源：http://3g.epnwcf.com/Article/details/gweqpsxhk.sHtML

scp file user@host:/path/
来源：http://baike.fktsv.cn/Article/details/gfrzdoakj.sHtML

[R57] 远程执行命令
来源：http://www.share.sjlbkw.cn/Article/details/gihyynbdo.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfkmaumx.sHtML

[R58] 下载文件
来源：http://blog.tarul.cn/Article/details/gnfnmprij.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/gatourgcp.sHtML

[R59] 发 POST JSON
来源：http://www.share.epnwcf.com/Article/details/galaoygwx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/goyotgupe.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gfokwkmuv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/gzptjdqsx.sHtML

[R61] 磁盘占用
来源：http://3g.fktsv.cn/Article/details/gpxmuntov.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/gzhvlpacz.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fktsv.cn/Article/details/gsfivqdpt.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.epnwcf.com/Article/details/gxedkxakd.sHtML

[R63] 内存与进程
来源：http://3g.yfazqb.com/Article/details/gpahuceta.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.sjlbkw.cn/Article/details/gitfxrstk.sHtML

[R64] 结束进程
来源：http://www.blog.sjlbkw.cn/Article/details/gkrprhyum.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.sjlbkw.cn/Article/details/gydtkgdia.sHtML

[R65] 查看端口占用
来源：http://wap.epnwcf.com/Article/details/gjfrksiky.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.tarul.cn/Article/details/gpazmtrtp.sHtML

[R66] 定时任务
来源：http://www.blog.epnwcf.com/Article/details/gmfnccazp.sHtML

crontab -e;  crontab -l
来源：http://wap.bbcook.cn/Article/details/gyjqatbhy.sHtML

[R67] 生成随机十六进制串
来源：http://blog.bbcook.cn/Article/details/ghznxfmck.sHtML

openssl rand -hex 16
来源：http://mobile.fktsv.cn/Article/details/grooneank.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/gssiobpbt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.sjlbkw.cn/Article/details/gulsijcib.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/gxxcuojar.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.vehdjk.com/Article/details/gzcxlbbym.sHtML

[R70] 时间戳与互转
来源：http://www.blog.yfazqb.com/Article/details/glbkdoahw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.vehdjk.com/Article/details/gjpowsbfy.sHtML

[R71] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gqedmdvft.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.vehdjk.com/Article/details/ginqbhtbc.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/ggagujluz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gcjgopgpb.sHtML

[R73] 分割大日志
来源：http://3g.yfazqb.com/Article/details/gupzthbyf.sHtML

split -l 1000 big.log part_
来源：http://www.blog.bbcook.cn/Article/details/gjgiwfspt.sHtML

[R74] 批量重命名
来源：http://blog.vehdjk.com/Article/details/gvhwwxoao.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.sjlbkw.cn/Article/details/gzidzdkhv.sHtML

[R75] 导出环境变量
来源：http://www.blog.yfazqb.com/Article/details/gbypwhyqx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.vehdjk.com/Article/details/gyppvtord.sHtML

[R76] 使用临时文件
来源：http://www.m.share.epnwcf.com/Article/details/gdpibdquh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gshyyqigz.sHtML

[R77] 读取用户输入
来源：http://blog.yfazqb.com/Article/details/gxojghbvp.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fktsv.cn/Article/details/gnvapwcdd.sHtML

[R78] 交互式菜单
来源：http://www.share.sjlbkw.cn/Article/details/gedwmuqea.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.vehdjk.com/Article/details/ghfzraryz.sHtML

[R79] 解析命令行选项
来源：http://read.share.fktsv.cn/Article/details/gwoatsnza.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/gwewbfwjh.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.bbcook.cn/Article/details/glmmrjywr.sHtML

time ./run.sh
来源：http://3g.fktsv.cn/Article/details/gqjibbdfe.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkzumhbnz.sHtML

S. C / C++ 专题
来源：http://www.blog.bbcook.cn/Article/details/galrgvkiy.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gaffkoupl.sHtML

[S01] C：Hello World
来源：http://blog.bbcook.cn/Article/details/gbzmoscvp.sHtML

#include <stdio.h>
来源：http://3g.epnwcf.com/Article/details/gbhjmmoey.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.bbcook.cn/Article/details/gyolyysee.sHtML

[S02] C：变量与格式化输出
来源：http://wap.vehdjk.com/Article/details/gqebfxpvj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.tarul.cn/Article/details/gdmsvlmqd.sHtML

[S03] C：读入整数
来源：http://www.blog.yfazqb.com/Article/details/gzgopieop.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/gcqrdjret.sHtML

[S04] C：字符串复制
来源：http://read.share.yfazqb.com/Article/details/gzuqwarno.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fktsv.cn/Article/details/gojvfkffg.sHtML

[S05] C：字符串长度
来源：http://mobile.bbcook.cn/Article/details/gymlfvdzv.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/gescxdsse.sHtML

[S06] C：字符串比较
来源：http://www.blog.tarul.cn/Article/details/gjxdgwhxn.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fktsv.cn/Article/details/gyfiqsgxz.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.bbcook.cn/Article/details/gxnxiwuie.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.epnwcf.com/Article/details/ghpfdqpul.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.yfazqb.com/Article/details/gguaictaf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.bbcook.cn/Article/details/gpsgslmro.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.tarul.cn/Article/details/giyxwbfds.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/gqjduirob.sHtML

[S10] C：指针与解引用
来源：http://mobile.yfazqb.com/Article/details/gxreghmqq.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.epnwcf.com/Article/details/ghnfjxczq.sHtML

[S11] C：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gogsmkncf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.bbcook.cn/Article/details/gpfuqicuf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gesfkntsi.sHtML

fclose(f);
来源：http://www.share.tarul.cn/Article/details/gnzlrgdmg.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/gvjqujkst.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/gtmuskrxs.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/gylnpuqrr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/glqyvrukq.sHtML

[S14] C：枚举
来源：http://read.share.yfazqb.com/Article/details/gsrtbcgyd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fktsv.cn/Article/details/gcrbbwmxt.sHtML

[S15] C：类型转换
来源：http://wap.tarul.cn/Article/details/gvjpyoekb.sHtML

(double) a / b
来源：http://baike.epnwcf.com/Article/details/gznuadgmv.sHtML

[S16] C：位操作置位
来源：http://mobile.bbcook.cn/Article/details/ghaenvdwx.sHtML

x |= (1 << 3);
来源：http://3g.sjlbkw.cn/Article/details/grgpryzfe.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyalrkzk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.tarul.cn/Article/details/gfwshpxwb.sHtML

[S18] C：命令行参数
来源：http://baike.epnwcf.com/Article/details/geyyhsuop.sHtML

int main(int argc, char **argv)
来源：http://www.blog.yfazqb.com/Article/details/gjleyuvok.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/ganigpjyj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gullikeza.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/gakybmqyh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gcpshapou.sHtML

[S21] C：字符类别判断
来源：http://3g.fktsv.cn/Article/details/gbptodjxh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.tarul.cn/Article/details/gmytyeioe.sHtML

[S22] C：字符串转数字
来源：http://mobile.tarul.cn/Article/details/gbyhtymaf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.epnwcf.com/Article/details/gcogpvxgo.sHtML

[S23] C：随机数
来源：http://read.share.vehdjk.com/Article/details/gksmjbzge.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.tarul.cn/Article/details/gzadrilvh.sHtML

[S24] C：获取本地时间
来源：http://baike.bbcook.cn/Article/details/gfosrbwfm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/gokcqlwxg.sHtML

[S25] C：内存拷贝
来源：http://www.share.tarul.cn/Article/details/grjgteaqa.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.vehdjk.com/Article/details/ggbnkiirn.sHtML

[S26] C：内存清零
来源：http://read.share.yfazqb.com/Article/details/gjxvpdanr.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.epnwcf.com/Article/details/gkbnvgiiy.sHtML

[S27] C：定义常量
来源：http://blog.fktsv.cn/Article/details/gvphucipi.sHtML

const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gttnxudnn.sHtML

[S28] C：静态变量
来源：http://baike.vehdjk.com/Article/details/gcsgpgexf.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/gkkjialpu.sHtML

[S29] C：变参函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gxiooyhne.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.sjlbkw.cn/Article/details/gwctlcmhg.sHtML

[S30] C：头文件保护
来源：http://wap.yfazqb.com/Article/details/gajrejamw.sHtML

#ifndef X_H
来源：http://3g.yfazqb.com/Article/details/gltmdpeog.sHtML

#define X_H
来源：http://m.share.sjlbkw.cn/Article/details/gblyrljbh.sHtML

#endif
来源：http://read.share.fktsv.cn/Article/details/gqmsijehz.sHtML

[S31] C++：Hello World
来源：http://blog.tarul.cn/Article/details/gtjhdbyxr.sHtML

#include <iostream>
来源：http://mobile.vehdjk.com/Article/details/guuobmyqk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtnjkouli.sHtML

[S32] C++：字符串
来源：http://baike.sjlbkw.cn/Article/details/ghsyjptyl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/gweklhfns.sHtML

[S33] C++：vector 增删
来源：http://read.share.epnwcf.com/Article/details/gkkiczaig.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gdmoaozzv.sHtML

[S34] C++：遍历 vector
来源：http://read.share.bbcook.cn/Article/details/gvmpxieeo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.vehdjk.com/Article/details/gjsqiqzzm.sHtML

[S35] C++：map
来源：http://3g.epnwcf.com/Article/details/gojkrjjgx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gagrwhrao.sHtML

[S36] C++：unordered_map
来源：http://www.share.epnwcf.com/Article/details/gmlymxixy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gdfnnshmk.sHtML

[S37] C++：set
来源：http://blog.epnwcf.com/Article/details/gjtzdrrwp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/gabhnyprk.sHtML

[S38] C++：排序
来源：http://www.m.share.fktsv.cn/Article/details/gdsstimke.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gjdeeilzv.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.yfazqb.com/Article/details/gjrfcjent.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.tarul.cn/Article/details/ghipmuduv.sHtML

[S40] C++：查找元素
来源：http://read.share.tarul.cn/Article/details/gcsxetiyv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.tarul.cn/Article/details/gkfqususo.sHtML

[S41] C++：类与构造函数
来源：http://baike.bbcook.cn/Article/details/guhzcxoya.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.tarul.cn/Article/details/ggnixakzc.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/giynotnvc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.epnwcf.com/Article/details/gpdmcqovw.sHtML

[S43] C++：智能指针
来源：http://blog.bbcook.cn/Article/details/gsvcctrze.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fktsv.cn/Article/details/gokglqavb.sHtML

[S44] C++：引用传参
来源：http://read.share.vehdjk.com/Article/details/ggcpoyynw.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.vehdjk.com/Article/details/gxljgyfxf.sHtML

[S45] C++：lambda
来源：http://m.share.tarul.cn/Article/details/gulcsquyd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fktsv.cn/Article/details/ghcfxxqeh.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/gmcdbntqf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.tarul.cn/Article/details/gdynnbsgu.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/gvesrkbra.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/gctmntcxi.sHtML

[S48] C++：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gpdnaqmrm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.tarul.cn/Article/details/gvsmvkjup.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.vehdjk.com/Article/details/glgtzuojs.sHtML

[S49] C++：写文件
来源：http://www.blog.tarul.cn/Article/details/guvxijamo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.yfazqb.com/Article/details/gtohzxkks.sHtML

[S50] C++：格式化数字
来源：http://3g.sjlbkw.cn/Article/details/gkslsxvro.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.epnwcf.com/Article/details/gezhbyarf.sHtML

[S51] C++：显式类型转换
来源：http://mobile.bbcook.cn/Article/details/gqrgolpat.sHtML

static_cast<double>(a) / b
来源：http://read.share.epnwcf.com/Article/details/gwikwqfkc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.yfazqb.com/Article/details/grhjiwutx.sHtML

int size() const noexcept { return n_; }
来源：http://baike.epnwcf.com/Article/details/grgwrcyrc.sHtML

[S53] C++：移动语义
来源：http://www.blog.sjlbkw.cn/Article/details/gthobcnwc.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fktsv.cn/Article/details/gacttbdzk.sHtML

[S54] C++：异常处理
来源：http://m.share.sjlbkw.cn/Article/details/ggnjhcmcw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.sjlbkw.cn/Article/details/gbsobvrou.sHtML

[S55] C++：结构化绑定
来源：http://wap.bbcook.cn/Article/details/gluzwxzre.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.tarul.cn/Article/details/ghkmxcwtn.sHtML

[S56] C++：optional
来源：http://www.m.share.bbcook.cn/Article/details/glegeflyb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.epnwcf.com/Article/details/glpfhvxzu.sHtML

[S57] C++：编译期常量
来源：http://baike.bbcook.cn/Article/details/gblnrenri.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/glrhxjwdh.sHtML

[S58] C++：命名空间
来源：http://wap.fktsv.cn/Article/details/gcpqljwlz.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.sjlbkw.cn/Article/details/grtytavwx.sHtML

[S59] C++：静态断言
来源：http://mobile.vehdjk.com/Article/details/gltiplnny.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.epnwcf.com/Article/details/gukosbcqh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.yfazqb.com/Article/details/gfdkhaoan.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.tarul.cn/Article/details/gvrrwnqmx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjbraiteg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.sjlbkw.cn/Article/details/gxpjjxllu.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gugqsbely.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gzpstpkjy.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gbcrydbrl.sHtML

[T02] Kotlin：变量
来源：http://mobile.yfazqb.com/Article/details/gxurqsxwp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.yfazqb.com/Article/details/gxlmuosms.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.epnwcf.com/Article/details/gcnaibcvl.sHtML

"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gglfmjxmc.sHtML

[T04] Kotlin：空安全
来源：http://www.share.vehdjk.com/Article/details/galsohlrd.sHtML

val n: String? = null;  n?.length
来源：http://baike.epnwcf.com/Article/details/gydnuprhd.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.bbcook.cn/Article/details/glgkwdpiv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.tarul.cn/Article/details/ghdebuljj.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.tarul.cn/Article/details/garujtwza.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.yfazqb.com/Article/details/gslpsypcr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.yfazqb.com/Article/details/gosucvmvo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gmvhrvqvx.sHtML

[T08] Kotlin：数据类
来源：http://mobile.vehdjk.com/Article/details/gdbejahsz.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.vehdjk.com/Article/details/gcywftpfk.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.vehdjk.com/Article/details/gjvexsapc.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/ggenxocxh.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gszjqzqsl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.yfazqb.com/Article/details/gvpcnlydx.sHtML

[T11] Kotlin：协程
来源：http://read.share.tarul.cn/Article/details/gkqfjwotw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.sjlbkw.cn/Article/details/gacjazcih.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/goclaxccx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/goqnfpjkq.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.yfazqb.com/Article/details/gjgyrsvee.sHtML

val m = mapOf("a" to 1)
来源：http://blog.bbcook.cn/Article/details/ghjhjywqc.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/gazwjczkz.sHtML

for (i in 1..10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gmkplvitm.sHtML

[T15] Kotlin：接口
来源：http://mobile.vehdjk.com/Article/details/gjmtewgbv.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.tarul.cn/Article/details/gzdhltuhd.sHtML

[T16] Swift：Hello World
来源：http://blog.bbcook.cn/Article/details/ghhdkaije.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/ghxqzfkor.sHtML

[T17] Swift：变量与常量
来源：http://read.share.yfazqb.com/Article/details/gxuuyfien.sHtML

var a = 1;  let b = 2
来源：http://read.share.bbcook.cn/Article/details/ggxrmttda.sHtML

[T18] Swift：字符串插值
来源：http://3g.vehdjk.com/Article/details/gxybafiqg.sHtML

"值: \(b)"
来源：http://baike.fktsv.cn/Article/details/gzzgepkkz.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.vehdjk.com/Article/details/ghnsdjsyp.sHtML

if let n = opt { print(n) }
来源：http://www.share.bbcook.cn/Article/details/gbefbrkcy.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.tarul.cn/Article/details/gzwtxjuak.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.sjlbkw.cn/Article/details/gcsmlenew.sHtML

[T21] Swift：遍历
来源：http://blog.tarul.cn/Article/details/gszsexpea.sHtML

for x in a { print(x) }
来源：http://www.blog.vehdjk.com/Article/details/gkllzdzxh.sHtML

[T22] Swift：字典
来源：http://wap.sjlbkw.cn/Article/details/gdoemfbhg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.sjlbkw.cn/Article/details/guauprfmf.sHtML

[T23] Swift：函数
来源：http://read.share.yfazqb.com/Article/details/guiwbynje.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.tarul.cn/Article/details/goftuqbgx.sHtML

[T24] Swift：闭包
来源：http://www.blog.vehdjk.com/Article/details/gluoefefp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.vehdjk.com/Article/details/gendwftny.sHtML

[T25] Swift：结构体
来源：http://m.share.sjlbkw.cn/Article/details/gtpcyskly.sHtML

struct P { var x: Int }
来源：http://www.share.yfazqb.com/Article/details/gcfzhmrtp.sHtML

[T26] Swift：类与重写
来源：http://read.share.yfazqb.com/Article/details/gfoqcksyh.sHtML

class A: Base { override func f() {} }
来源：http://3g.tarul.cn/Article/details/gayiijcgx.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/ghyrncotu.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.tarul.cn/Article/details/gdvmyllgk.sHtML

[T28] Swift：枚举
来源：http://baike.sjlbkw.cn/Article/details/gebfvbrrl.sHtML

enum Color { case red, green }
来源：http://read.share.epnwcf.com/Article/details/glnncasgi.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.tarul.cn/Article/details/glarghoxn.sHtML

guard let x = opt else { return }
来源：http://blog.tarul.cn/Article/details/ghvlcanhb.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/gqzbikkgy.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fktsv.cn/Article/details/gnccyecac.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/giijzustq.sHtML

print("Hello")
来源：http://wap.yfazqb.com/Article/details/gfajtzaby.sHtML

[T32] Lua：局部变量
来源：http://www.share.yfazqb.com/Article/details/guhwmhpvd.sHtML

local a = 1
来源：http://www.m.share.bbcook.cn/Article/details/ggeyxxakh.sHtML

[T33] Lua：表（数组）
来源：http://3g.sjlbkw.cn/Article/details/gmighrrdy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.sjlbkw.cn/Article/details/gjlausyne.sHtML

[T34] Lua：遍历表
来源：http://www.blog.vehdjk.com/Article/details/gmmbrvncp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.sjlbkw.cn/Article/details/gmpkjfemp.sHtML

[T35] Lua：字典表
来源：http://3g.fktsv.cn/Article/details/ginourdva.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.bbcook.cn/Article/details/gvbutqpvt.sHtML

[T36] Lua：函数
来源：http://www.m.share.epnwcf.com/Article/details/gswayfdcn.sHtML

function add(a, b) return a + b end
来源：http://wap.yfazqb.com/Article/details/gwblgkutr.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gyptzjrlg.sHtML

"a" .. "b"
来源：http://mobile.sjlbkw.cn/Article/details/gijmxfazx.sHtML

[T38] Lua：条件
来源：http://baike.tarul.cn/Article/details/gmkwdegsr.sHtML

if x > 0 then print("正") end
来源：http://m.share.tarul.cn/Article/details/gjmwfykxl.sHtML

[T39] Lua：模式匹配
来源：http://baike.tarul.cn/Article/details/gxekvvhin.sHtML

string.find(s, "%d+")
来源：http://m.share.vehdjk.com/Article/details/gfarwddjz.sHtML

[T40] Lua：元表
来源：http://www.m.share.epnwcf.com/Article/details/gaifsukfc.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.yfazqb.com/Article/details/gndzhmmoi.sHtML

[T41] Perl：Hello World
来源：http://3g.vehdjk.com/Article/details/gwaeqbanl.sHtML

print "Hello\n";
来源：http://baike.fktsv.cn/Article/details/gnpphjcly.sHtML

[T42] Perl：变量类型
来源：http://3g.vehdjk.com/Article/details/gejpwbvla.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.epnwcf.com/Article/details/gihxxhvsl.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gvfixqojc.sHtML

"值: $a"
来源：http://baike.vehdjk.com/Article/details/geulvsqtv.sHtML

[T44] Perl：条件
来源：http://mobile.fktsv.cn/Article/details/gooaopihq.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.bbcook.cn/Article/details/ggbqbezge.sHtML


<!-- 参考信息 -->