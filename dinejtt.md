代发 wailian999

find . -name "*.log" -type f
来源：http://www.share.yfazqb.com/Article/details/ghhuuqdng.sHtML

[R44] 按修改时间查找
来源：http://read.share.bbcook.cn/Article/details/gjaajgyct.sHtML

find . -mtime -7 -type f
来源：http://blog.vehdjk.com/Article/details/gqvcnlclu.sHtML

[R45] 批量删除
来源：http://wap.bbcook.cn/Article/details/gfnuxrxzi.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fktsv.cn/Article/details/guuhqtvei.sHtML

[R46] 递归替换文件内容
来源：http://mobile.vehdjk.com/Article/details/gnbffktia.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.epnwcf.com/Article/details/grmjdwvur.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fktsv.cn/Article/details/groskgleq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.yfazqb.com/Article/details/gkorqbfma.sHtML

[R48] awk 取指定列
来源：http://baike.fktsv.cn/Article/details/giroqfrgp.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fktsv.cn/Article/details/ghwuljrdm.sHtML

[R49] awk 带条件
来源：http://blog.yfazqb.com/Article/details/gkarhkdhu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.sjlbkw.cn/Article/details/gyzrhnnwr.sHtML

[R50] awk 求和
来源：http://read.share.sjlbkw.cn/Article/details/gwnmohrko.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gomxprgoe.sHtML

[R51] 排序去重取前几
来源：http://baike.tarul.cn/Article/details/gdmxbxefm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.sjlbkw.cn/Article/details/godnvszdb.sHtML

[R52] 统计行数
来源：http://m.share.tarul.cn/Article/details/gsmzpwcjl.sHtML

wc -l a.txt
来源：http://blog.sjlbkw.cn/Article/details/gizrmpwiv.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.bbcook.cn/Article/details/gmdvvvpku.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.epnwcf.com/Article/details/gudrnifvy.sHtML

[R54] 比较两个文件
来源：http://www.m.share.epnwcf.com/Article/details/giwckkcjd.sHtML

diff a.txt b.txt
来源：http://www.blog.epnwcf.com/Article/details/gifnycjzb.sHtML

[R55] 压缩与解压
来源：http://3g.fktsv.cn/Article/details/gteiiulrr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.epnwcf.com/Article/details/gggwaihga.sHtML

[R56] 远程拷贝
来源：http://baike.vehdjk.com/Article/details/gksvxajza.sHtML

scp file user@host:/path/
来源：http://3g.sjlbkw.cn/Article/details/gbgylpxka.sHtML

[R57] 远程执行命令
来源：http://m.share.sjlbkw.cn/Article/details/gmkqdqlcr.sHtML

ssh user@host 'uptime'
来源：http://www.share.bbcook.cn/Article/details/gayxuzjwn.sHtML

[R58] 下载文件
来源：http://mobile.fktsv.cn/Article/details/gvinvpxmc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fktsv.cn/Article/details/gspphfbgr.sHtML

[R59] 发 POST JSON
来源：http://www.share.fktsv.cn/Article/details/ghvkzhlqi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.tarul.cn/Article/details/gxesekuok.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/gizucrkzb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.sjlbkw.cn/Article/details/gigytkmdi.sHtML

[R61] 磁盘占用
来源：http://blog.tarul.cn/Article/details/glulbzmzb.sHtML

df -h;  du -sh *
来源：http://www.blog.epnwcf.com/Article/details/gzqscycrh.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.bbcook.cn/Article/details/gafpjfhko.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.tarul.cn/Article/details/gqsbwifsq.sHtML

[R63] 内存与进程
来源：http://mobile.yfazqb.com/Article/details/gopvvtyin.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.bbcook.cn/Article/details/gidclqyio.sHtML

[R64] 结束进程
来源：http://3g.tarul.cn/Article/details/gprinuzwo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.epnwcf.com/Article/details/gzxkzepcv.sHtML

[R65] 查看端口占用
来源：http://m.share.fktsv.cn/Article/details/gynnrsdgg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fktsv.cn/Article/details/gukpygzyp.sHtML

[R66] 定时任务
来源：http://www.m.share.fktsv.cn/Article/details/gqyjmacbn.sHtML

crontab -e;  crontab -l
来源：http://wap.tarul.cn/Article/details/gpixzqwcn.sHtML

[R67] 生成随机十六进制串
来源：http://3g.sjlbkw.cn/Article/details/giltyjqnd.sHtML

openssl rand -hex 16
来源：http://baike.epnwcf.com/Article/details/gowksvitw.sHtML

[R68] 计算文件校验值
来源：http://wap.bbcook.cn/Article/details/gggsqrkbn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.tarul.cn/Article/details/gkybbuhxj.sHtML

[R69] 生成随机密码
来源：http://read.share.epnwcf.com/Article/details/gxwbwspno.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.bbcook.cn/Article/details/gpgntvvwj.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/gaxbwxbcp.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.tarul.cn/Article/details/glhnxdfqq.sHtML

[R71] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gvzipmwit.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.bbcook.cn/Article/details/glgqsaeli.sHtML

[R72] 等待端口就绪
来源：http://www.share.tarul.cn/Article/details/gwlzvkvtd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gjuulmiek.sHtML

[R73] 分割大日志
来源：http://baike.sjlbkw.cn/Article/details/giqdglrvd.sHtML

split -l 1000 big.log part_
来源：http://wap.tarul.cn/Article/details/gengblmpa.sHtML

[R74] 批量重命名
来源：http://baike.tarul.cn/Article/details/gukvmwaqb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fktsv.cn/Article/details/gmyfjkeps.sHtML

[R75] 导出环境变量
来源：http://read.share.vehdjk.com/Article/details/gbazrohrt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.tarul.cn/Article/details/gihknipab.sHtML

[R76] 使用临时文件
来源：http://read.share.tarul.cn/Article/details/gaavzpuwb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/gfsiiudfs.sHtML

[R77] 读取用户输入
来源：http://blog.sjlbkw.cn/Article/details/gfvwogzjc.sHtML

read -rp "请输入: " ans
来源：http://mobile.epnwcf.com/Article/details/ghavyccsp.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/gusdarqeb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.bbcook.cn/Article/details/gavqrdbuw.sHtML

[R79] 解析命令行选项
来源：http://m.share.tarul.cn/Article/details/ghijemkmc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.tarul.cn/Article/details/gexgtmdsy.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.yfazqb.com/Article/details/gyedxygmk.sHtML

time ./run.sh
来源：http://read.share.bbcook.cn/Article/details/ghdoqlqzp.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/goeqwemcv.sHtML

S. C / C++ 专题
来源：http://baike.vehdjk.com/Article/details/gfantehsx.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gkfuvpvjm.sHtML

[S01] C：Hello World
来源：http://wap.fktsv.cn/Article/details/gatujapqk.sHtML

#include <stdio.h>
来源：http://read.share.vehdjk.com/Article/details/gpboihpiv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.sjlbkw.cn/Article/details/gfongsqdl.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.tarul.cn/Article/details/gdqhyjjko.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.tarul.cn/Article/details/ghtofeaej.sHtML

[S03] C：读入整数
来源：http://wap.epnwcf.com/Article/details/gmpllqbhf.sHtML

int x; scanf("%d", &x);
来源：http://www.share.sjlbkw.cn/Article/details/gcndiqfuh.sHtML

[S04] C：字符串复制
来源：http://3g.yfazqb.com/Article/details/gxittedck.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.tarul.cn/Article/details/geitzfbhz.sHtML

[S05] C：字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gmtoaxlwh.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/gkpsmeprd.sHtML

[S06] C：字符串比较
来源：http://baike.tarul.cn/Article/details/ganmrikde.sHtML

strcmp(a, b) == 0
来源：http://www.share.fktsv.cn/Article/details/gtffmduwq.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.vehdjk.com/Article/details/gcojtnqpl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.vehdjk.com/Article/details/gkuktozgl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fktsv.cn/Article/details/gddgucgei.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fktsv.cn/Article/details/grhvwvzau.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.tarul.cn/Article/details/gwifzoilg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/gpnegbofc.sHtML

[S10] C：指针与解引用
来源：http://read.share.yfazqb.com/Article/details/gwpntjghb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/gwmfqsutq.sHtML

[S11] C：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gjyrsrmcx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fktsv.cn/Article/details/ghjarfpiq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/gonwiskxq.sHtML

fclose(f);
来源：http://baike.vehdjk.com/Article/details/gwnhmjnau.sHtML

[S12] C：写文件
来源：http://www.share.tarul.cn/Article/details/gaiixmrpn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gjaoiurmt.sHtML

[S13] C：宏定义
来源：http://wap.yfazqb.com/Article/details/gbuwzlstb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fktsv.cn/Article/details/gzmjrqmbv.sHtML

[S14] C：枚举
来源：http://www.m.share.vehdjk.com/Article/details/ghevmzffo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.yfazqb.com/Article/details/gsinguhmw.sHtML

[S15] C：类型转换
来源：http://wap.sjlbkw.cn/Article/details/gjuibmrfq.sHtML

(double) a / b
来源：http://mobile.epnwcf.com/Article/details/gsinudfnr.sHtML

[S16] C：位操作置位
来源：http://www.m.share.vehdjk.com/Article/details/gqmsmwgxs.sHtML

x |= (1 << 3);
来源：http://wap.epnwcf.com/Article/details/gtdiybtet.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/grpziwlcs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.vehdjk.com/Article/details/ghaeidsds.sHtML

[S18] C：命令行参数
来源：http://www.share.epnwcf.com/Article/details/glfrcqeqq.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gkdfkbrku.sHtML

[S19] C：快速排序
来源：http://3g.epnwcf.com/Article/details/ghsmgzguz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gkwosuocc.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/grzzmkcne.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gzvginzgc.sHtML

[S21] C：字符类别判断
来源：http://m.share.fktsv.cn/Article/details/gvgzuuwjv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.vehdjk.com/Article/details/gbserwjoj.sHtML

[S22] C：字符串转数字
来源：http://www.share.yfazqb.com/Article/details/gnsxkrynm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/glfhmywzl.sHtML

[S23] C：随机数
来源：http://www.blog.tarul.cn/Article/details/grdzibjue.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.epnwcf.com/Article/details/gutxfbplb.sHtML

[S24] C：获取本地时间
来源：http://m.share.tarul.cn/Article/details/gswvgoaex.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/glinjcnae.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/gtixcuwma.sHtML

memcpy(dst, src, n);
来源：http://3g.sjlbkw.cn/Article/details/gjuxsyubo.sHtML

[S26] C：内存清零
来源：http://3g.sjlbkw.cn/Article/details/gdmezlauo.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fktsv.cn/Article/details/gnczveret.sHtML

[S27] C：定义常量
来源：http://www.m.share.yfazqb.com/Article/details/gglsqffvb.sHtML

const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/glpuxbfws.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/gnfjuvfbt.sHtML

static int counter = 0;
来源：http://baike.sjlbkw.cn/Article/details/ghypidqyi.sHtML

[S29] C：变参函数
来源：http://wap.sjlbkw.cn/Article/details/goenwhecw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.sjlbkw.cn/Article/details/gsodumpnx.sHtML

[S30] C：头文件保护
来源：http://blog.tarul.cn/Article/details/gtgaukfdt.sHtML

#ifndef X_H
来源：http://www.m.share.bbcook.cn/Article/details/gyvdsjtbk.sHtML

#define X_H
来源：http://read.share.yfazqb.com/Article/details/gcfzjsaly.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gvdhwwixq.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gsgvzqivz.sHtML

#include <iostream>
来源：http://mobile.tarul.cn/Article/details/gvshuijnu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.epnwcf.com/Article/details/gnlxnrpyq.sHtML

[S32] C++：字符串
来源：http://baike.sjlbkw.cn/Article/details/gkkycwpxd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.yfazqb.com/Article/details/gbanzffps.sHtML

[S33] C++：vector 增删
来源：http://www.share.bbcook.cn/Article/details/gxurjtqhw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.epnwcf.com/Article/details/ginrrifow.sHtML

[S34] C++：遍历 vector
来源：http://wap.epnwcf.com/Article/details/gqihegcps.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.vehdjk.com/Article/details/ghfhlicqr.sHtML

[S35] C++：map
来源：http://baike.fktsv.cn/Article/details/gdrszvmly.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gabhbdbkp.sHtML

[S36] C++：unordered_map
来源：http://baike.epnwcf.com/Article/details/gdeaedcqu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/gntkfghdb.sHtML

[S37] C++：set
来源：http://www.share.tarul.cn/Article/details/gabokkhci.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.tarul.cn/Article/details/gdnhizwcj.sHtML

[S38] C++：排序
来源：http://blog.tarul.cn/Article/details/gbaiusqos.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.bbcook.cn/Article/details/gxsuwktre.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fktsv.cn/Article/details/gksmizfcn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.vehdjk.com/Article/details/gpdrprexq.sHtML

[S40] C++：查找元素
来源：http://m.share.yfazqb.com/Article/details/gnmqfmini.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.yfazqb.com/Article/details/gylexnsmm.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gtnoyyrse.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fktsv.cn/Article/details/gvhwanjye.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gcntsboww.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.yfazqb.com/Article/details/gtklsdgii.sHtML

[S43] C++：智能指针
来源：http://3g.bbcook.cn/Article/details/grtxhmlcd.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.sjlbkw.cn/Article/details/gesgsltbg.sHtML

[S44] C++：引用传参
来源：http://baike.bbcook.cn/Article/details/gbupkwxxg.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.vehdjk.com/Article/details/gwkwxhzxu.sHtML

[S45] C++：lambda
来源：http://blog.vehdjk.com/Article/details/geffrolxq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fktsv.cn/Article/details/gfsfizqnm.sHtML

[S46] C++：函数模板
来源：http://www.share.yfazqb.com/Article/details/guazhcvom.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.epnwcf.com/Article/details/gcqvajfow.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/gqfrvgatb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.vehdjk.com/Article/details/gkcupugoh.sHtML

[S48] C++：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/glpmuauov.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.bbcook.cn/Article/details/gbzmlgjlr.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/gzvgnrsgr.sHtML

[S49] C++：写文件
来源：http://mobile.vehdjk.com/Article/details/gvhkwyhvy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.tarul.cn/Article/details/gpjtkflnv.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/glyuhubwn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdktywyo.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.bbcook.cn/Article/details/geknulsfj.sHtML

static_cast<double>(a) / b
来源：http://baike.yfazqb.com/Article/details/gqekgtpcj.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.vehdjk.com/Article/details/gzqokpiss.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.vehdjk.com/Article/details/ghzkbeuim.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/gvyeotxod.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.epnwcf.com/Article/details/ghoswuknz.sHtML

[S54] C++：异常处理
来源：http://blog.epnwcf.com/Article/details/gahmohfjl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fktsv.cn/Article/details/gylxexpcj.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/gizixhtaz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.epnwcf.com/Article/details/grzmpewyd.sHtML

[S56] C++：optional
来源：http://read.share.fktsv.cn/Article/details/gftdtzpwv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fktsv.cn/Article/details/glwikdixq.sHtML

[S57] C++：编译期常量
来源：http://wap.epnwcf.com/Article/details/gwymjfyhl.sHtML

constexpr int N = 10;
来源：http://3g.bbcook.cn/Article/details/gurrsiffk.sHtML

[S58] C++：命名空间
来源：http://read.share.fktsv.cn/Article/details/glluaddtm.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/glbjdadtf.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/gevimsjdp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.bbcook.cn/Article/details/gribhqkdz.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.bbcook.cn/Article/details/gcmphjtay.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.yfazqb.com/Article/details/grewxjvvy.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gvymwhxuk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gcnwayydc.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gyqwqdjei.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.epnwcf.com/Article/details/glpxjomuh.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gutmuyhur.sHtML

[T02] Kotlin：变量
来源：http://blog.yfazqb.com/Article/details/gkiukbarw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.yfazqb.com/Article/details/gltwafsms.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.tarul.cn/Article/details/gfeuynlhd.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/gxrtaywwk.sHtML

[T04] Kotlin：空安全
来源：http://read.share.yfazqb.com/Article/details/gxkttheas.sHtML

val n: String? = null;  n?.length
来源：http://baike.epnwcf.com/Article/details/gacefszbx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.bbcook.cn/Article/details/gklavyszc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.epnwcf.com/Article/details/gwsvlhspr.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fktsv.cn/Article/details/gaelyczta.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gmiaqnnqw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gcvgitxfj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gcrwnmvbq.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/gspnmrhtu.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.bbcook.cn/Article/details/gpvivgnky.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.sjlbkw.cn/Article/details/grboxobgs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.epnwcf.com/Article/details/gwunalqxd.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.yfazqb.com/Article/details/gfzuchrab.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.sjlbkw.cn/Article/details/gufrxzupy.sHtML

[T11] Kotlin：协程
来源：http://read.share.tarul.cn/Article/details/gqzyfjwos.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/gdvuftzln.sHtML

[T12] Kotlin：解构声明
来源：http://3g.bbcook.cn/Article/details/ghrocwups.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gduyjqien.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.vehdjk.com/Article/details/glhwlohzs.sHtML

val m = mapOf("a" to 1)
来源：http://3g.epnwcf.com/Article/details/geemvoblj.sHtML

[T14] Kotlin：循环
来源：http://mobile.yfazqb.com/Article/details/gcmqvniuq.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gqhietxuu.sHtML

[T15] Kotlin：接口
来源：http://baike.yfazqb.com/Article/details/gejegjqhb.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fktsv.cn/Article/details/givfmtmue.sHtML

[T16] Swift：Hello World
来源：http://www.share.tarul.cn/Article/details/gjdvqlgmc.sHtML

print("Hello")
来源：http://m.share.tarul.cn/Article/details/gojcrpcmj.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.vehdjk.com/Article/details/gjxmvvnxi.sHtML

var a = 1;  let b = 2
来源：http://wap.epnwcf.com/Article/details/gsosnvwcr.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gcpfnbhbh.sHtML

"值: \(b)"
来源：http://baike.epnwcf.com/Article/details/gqlwoaswh.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.sjlbkw.cn/Article/details/gktjucwbj.sHtML

if let n = opt { print(n) }
来源：http://wap.fktsv.cn/Article/details/geoozuaki.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/gyzpawobk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.yfazqb.com/Article/details/gpymmvchu.sHtML

[T21] Swift：遍历
来源：http://3g.vehdjk.com/Article/details/gmscajtxv.sHtML

for x in a { print(x) }
来源：http://baike.tarul.cn/Article/details/gabffsodh.sHtML

[T22] Swift：字典
来源：http://www.share.sjlbkw.cn/Article/details/gkvbxiqqy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.vehdjk.com/Article/details/gahxetcba.sHtML

[T23] Swift：函数
来源：http://www.blog.fktsv.cn/Article/details/gmkxlgaum.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fktsv.cn/Article/details/gxlqawhlx.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gibvpjzit.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.bbcook.cn/Article/details/gkahqvbwj.sHtML

[T25] Swift：结构体
来源：http://blog.yfazqb.com/Article/details/gicxzcqmq.sHtML

struct P { var x: Int }
来源：http://www.share.vehdjk.com/Article/details/ghlrezstp.sHtML

[T26] Swift：类与重写
来源：http://3g.bbcook.cn/Article/details/glcllucgc.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.epnwcf.com/Article/details/gocnthekq.sHtML

[T27] Swift：错误处理
来源：http://mobile.fktsv.cn/Article/details/gqlqogmgl.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.epnwcf.com/Article/details/gpsaztngn.sHtML

[T28] Swift：枚举
来源：http://www.m.share.tarul.cn/Article/details/gchhnihaq.sHtML

enum Color { case red, green }
来源：http://baike.tarul.cn/Article/details/gzoublvwx.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fktsv.cn/Article/details/gkvefoklg.sHtML

guard let x = opt else { return }
来源：http://3g.sjlbkw.cn/Article/details/gcuhwpsie.sHtML

[T30] Swift：协议
来源：http://m.share.tarul.cn/Article/details/gotnautrw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.sjlbkw.cn/Article/details/gxpyvdwpz.sHtML

[T31] Lua：Hello World
来源：http://wap.bbcook.cn/Article/details/gaszocpln.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gvqntetde.sHtML

[T32] Lua：局部变量
来源：http://m.share.yfazqb.com/Article/details/gjtcactpq.sHtML

local a = 1
来源：http://www.m.share.epnwcf.com/Article/details/gnjivvori.sHtML

[T33] Lua：表（数组）
来源：http://3g.epnwcf.com/Article/details/gqnaqexau.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.yfazqb.com/Article/details/gwgsreovg.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gobslxeps.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.tarul.cn/Article/details/gbjkimawz.sHtML

[T35] Lua：字典表
来源：http://baike.vehdjk.com/Article/details/gtewhkcch.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/gvjeehklz.sHtML

[T36] Lua：函数
来源：http://wap.yfazqb.com/Article/details/grcftqviu.sHtML

function add(a, b) return a + b end
来源：http://blog.vehdjk.com/Article/details/gelcllhtg.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.vehdjk.com/Article/details/ghbvxahbc.sHtML

"a" .. "b"
来源：http://m.share.tarul.cn/Article/details/gdsbwgous.sHtML

[T38] Lua：条件
来源：http://3g.fktsv.cn/Article/details/guexqtyce.sHtML

if x > 0 then print("正") end
来源：http://3g.sjlbkw.cn/Article/details/gyfzmqyun.sHtML

[T39] Lua：模式匹配
来源：http://m.share.tarul.cn/Article/details/gvesaktpn.sHtML

string.find(s, "%d+")
来源：http://baike.epnwcf.com/Article/details/gryogmsrh.sHtML

[T40] Lua：元表
来源：http://www.share.vehdjk.com/Article/details/gluaqpnrf.sHtML

setmetatable({}, { __index = base })
来源：http://baike.yfazqb.com/Article/details/gvmtiqdmp.sHtML

[T41] Perl：Hello World
来源：http://wap.sjlbkw.cn/Article/details/grwozchmy.sHtML

print "Hello\n";
来源：http://mobile.vehdjk.com/Article/details/gvpqznpaw.sHtML

[T42] Perl：变量类型
来源：http://wap.sjlbkw.cn/Article/details/gajjmsjrt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.epnwcf.com/Article/details/gtohkjiho.sHtML

[T43] Perl：字符串插值
来源：http://blog.bbcook.cn/Article/details/gkanqmefn.sHtML

"值: $a"
来源：http://3g.yfazqb.com/Article/details/geqvrvdvc.sHtML

[T44] Perl：条件
来源：http://blog.epnwcf.com/Article/details/gajmxstvj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.epnwcf.com/Article/details/gdkcuezid.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.tarul.cn/Article/details/glifajcje.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.yfazqb.com/Article/details/gktpylmoj.sHtML

[T46] Perl：哈希操作
来源：http://read.share.bbcook.cn/Article/details/gbsnuzzly.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.vehdjk.com/Article/details/goptlqork.sHtML


<!-- 参考信息 -->