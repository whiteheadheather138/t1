代发 wailian999

find . -name "*.log" -type f
来源：http://www.m.share.yfazqb.com/Article/details/ghrmbtaam.sHtML

[R44] 按修改时间查找
来源：http://baike.fktsv.cn/Article/details/gejmyzuzf.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.bbcook.cn/Article/details/ggsuubyei.sHtML

[R45] 批量删除
来源：http://www.m.share.yfazqb.com/Article/details/gfduwvvqw.sHtML

find . -name "*.tmp" -delete
来源：http://baike.bbcook.cn/Article/details/gfbaevegr.sHtML

[R46] 递归替换文件内容
来源：http://3g.fktsv.cn/Article/details/gyusatcdx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.bbcook.cn/Article/details/glxuzphie.sHtML

[R47] sed 单行替换
来源：http://www.blog.sjlbkw.cn/Article/details/gjsxacmys.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gimklbxdt.sHtML

[R48] awk 取指定列
来源：http://www.m.share.vehdjk.com/Article/details/gzskbizhe.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/gdvhxwywh.sHtML

[R49] awk 带条件
来源：http://www.blog.sjlbkw.cn/Article/details/gumjckinb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.yfazqb.com/Article/details/guatkujha.sHtML

[R50] awk 求和
来源：http://m.share.fktsv.cn/Article/details/gwfgbrwvg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gywzgrzjz.sHtML

[R51] 排序去重取前几
来源：http://www.blog.yfazqb.com/Article/details/ggfrzhvtx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/gzfpxmgtj.sHtML

[R52] 统计行数
来源：http://www.share.epnwcf.com/Article/details/gcqnlemch.sHtML

wc -l a.txt
来源：http://3g.bbcook.cn/Article/details/gdlldokur.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.epnwcf.com/Article/details/gngidywio.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fktsv.cn/Article/details/glqcrwuoa.sHtML

[R54] 比较两个文件
来源：http://blog.bbcook.cn/Article/details/ghuilmgrn.sHtML

diff a.txt b.txt
来源：http://mobile.tarul.cn/Article/details/giymoaayw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fktsv.cn/Article/details/gsrxgztyj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.vehdjk.com/Article/details/geljwpwkc.sHtML

[R56] 远程拷贝
来源：http://blog.sjlbkw.cn/Article/details/gesbrfnwo.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/gmqgniejo.sHtML

[R57] 远程执行命令
来源：http://read.share.epnwcf.com/Article/details/gpwvhckii.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gqxmdkjuu.sHtML

[R58] 下载文件
来源：http://wap.bbcook.cn/Article/details/gdscnycsr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.yfazqb.com/Article/details/grfqvwwkm.sHtML

[R59] 发 POST JSON
来源：http://baike.bbcook.cn/Article/details/gqfkksgfe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.vehdjk.com/Article/details/gdmnfkikj.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/ghgbxvqbr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.vehdjk.com/Article/details/gwgkhnioz.sHtML

[R61] 磁盘占用
来源：http://mobile.vehdjk.com/Article/details/gzfgmjvqd.sHtML

df -h;  du -sh *
来源：http://www.m.share.tarul.cn/Article/details/gzdjopjtn.sHtML

[R62] 找最占空间的文件
来源：http://m.share.vehdjk.com/Article/details/gfqaewjal.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fktsv.cn/Article/details/gefngopza.sHtML

[R63] 内存与进程
来源：http://mobile.sjlbkw.cn/Article/details/ghbvudbgb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.epnwcf.com/Article/details/gjdeirdxz.sHtML

[R64] 结束进程
来源：http://www.share.fktsv.cn/Article/details/gzijpdrwe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.sjlbkw.cn/Article/details/grjadzciv.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/gsexqrevd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fktsv.cn/Article/details/gpzdobakv.sHtML

[R66] 定时任务
来源：http://baike.vehdjk.com/Article/details/goifvxrfv.sHtML

crontab -e;  crontab -l
来源：http://www.share.epnwcf.com/Article/details/gujfuyiru.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.sjlbkw.cn/Article/details/gxqqddrzk.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/gkgdxkvrz.sHtML

[R68] 计算文件校验值
来源：http://read.share.epnwcf.com/Article/details/guyunjjsn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.epnwcf.com/Article/details/ggqzfptfh.sHtML

[R69] 生成随机密码
来源：http://wap.bbcook.cn/Article/details/gmbojebjb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.yfazqb.com/Article/details/gfvhiucqa.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/giuhtzcwx.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.sjlbkw.cn/Article/details/gskspkvfm.sHtML

[R71] 日期格式化
来源：http://3g.bbcook.cn/Article/details/gofhqeysi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.yfazqb.com/Article/details/grrwqmmyu.sHtML

[R72] 等待端口就绪
来源：http://baike.epnwcf.com/Article/details/gwfkhsyff.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gorlqqmdm.sHtML

[R73] 分割大日志
来源：http://wap.tarul.cn/Article/details/gzhzqyuse.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/ghwzzjthb.sHtML

[R74] 批量重命名
来源：http://wap.yfazqb.com/Article/details/gkbwrrbln.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/godnrmtme.sHtML

[R75] 导出环境变量
来源：http://3g.sjlbkw.cn/Article/details/gzoxhcmks.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fktsv.cn/Article/details/ggvwurqcc.sHtML

[R76] 使用临时文件
来源：http://blog.bbcook.cn/Article/details/ghtoywtas.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/gncmcwwts.sHtML

[R77] 读取用户输入
来源：http://baike.fktsv.cn/Article/details/gnhoewqga.sHtML

read -rp "请输入: " ans
来源：http://www.share.fktsv.cn/Article/details/gsnizrbey.sHtML

[R78] 交互式菜单
来源：http://www.share.fktsv.cn/Article/details/gnugdxses.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/gficuyylb.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.tarul.cn/Article/details/gjoudvssp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.vehdjk.com/Article/details/gvqghzyfr.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.bbcook.cn/Article/details/gpfzlyman.sHtML

time ./run.sh
来源：http://www.share.tarul.cn/Article/details/gexkrwjwq.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gmsgmhccb.sHtML

S. C / C++ 专题
来源：http://baike.tarul.cn/Article/details/gpnceqnmv.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkydwijsy.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/ghdnhnjql.sHtML

#include <stdio.h>
来源：http://3g.bbcook.cn/Article/details/gkphzujva.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.yfazqb.com/Article/details/gbfzxthhb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.yfazqb.com/Article/details/glqfevbcx.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.sjlbkw.cn/Article/details/gozgibtak.sHtML

[S03] C：读入整数
来源：http://wap.epnwcf.com/Article/details/geggxjydw.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.tarul.cn/Article/details/gfoniopde.sHtML

[S04] C：字符串复制
来源：http://baike.fktsv.cn/Article/details/gbzwlzthj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.yfazqb.com/Article/details/gbtliezbi.sHtML

[S05] C：字符串长度
来源：http://3g.tarul.cn/Article/details/geqemprnp.sHtML

strlen(s)
来源：http://mobile.epnwcf.com/Article/details/gstuzvuaw.sHtML

[S06] C：字符串比较
来源：http://www.blog.tarul.cn/Article/details/gchikvkvu.sHtML

strcmp(a, b) == 0
来源：http://mobile.tarul.cn/Article/details/gubazrnsm.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/gvbcipani.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fktsv.cn/Article/details/gpjwhjtyx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.vehdjk.com/Article/details/gywpcwlcb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.bbcook.cn/Article/details/gcydahadf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.yfazqb.com/Article/details/gvyadrbjb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fktsv.cn/Article/details/gsiyqxarz.sHtML

[S10] C：指针与解引用
来源：http://m.share.epnwcf.com/Article/details/gpyywiycj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.yfazqb.com/Article/details/gbqgkgatd.sHtML

[S11] C：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gthkqfapu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.yfazqb.com/Article/details/ginjkrogj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/glxjkumel.sHtML

fclose(f);
来源：http://mobile.tarul.cn/Article/details/guqvngeiq.sHtML

[S12] C：写文件
来源：http://www.share.tarul.cn/Article/details/gmgesalew.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.bbcook.cn/Article/details/gxbjolgzz.sHtML

[S13] C：宏定义
来源：http://mobile.sjlbkw.cn/Article/details/gaxgzxlgv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.epnwcf.com/Article/details/ghdqscghu.sHtML

[S14] C：枚举
来源：http://www.blog.fktsv.cn/Article/details/ghkullofv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.bbcook.cn/Article/details/grihmlkcc.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/gtkhamvmy.sHtML

(double) a / b
来源：http://m.share.bbcook.cn/Article/details/goaxkivlj.sHtML

[S16] C：位操作置位
来源：http://blog.vehdjk.com/Article/details/gfiacaxbe.sHtML

x |= (1 << 3);
来源：http://www.share.bbcook.cn/Article/details/gttslwsxs.sHtML

[S17] C：安全拼接字符串
来源：http://3g.vehdjk.com/Article/details/grzlpefnx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gguqxtkzz.sHtML

[S18] C：命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gdakeeubm.sHtML

int main(int argc, char **argv)
来源：http://mobile.sjlbkw.cn/Article/details/gdfitwxyp.sHtML

[S19] C：快速排序
来源：http://read.share.vehdjk.com/Article/details/grabauivg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/ggfgubxzo.sHtML

[S20] C：二分查找
来源：http://mobile.yfazqb.com/Article/details/gphrdcigc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gllzihmur.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.tarul.cn/Article/details/gaockjvwi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.epnwcf.com/Article/details/gagnnagye.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gbknprgug.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.tarul.cn/Article/details/gllxybgho.sHtML

[S23] C：随机数
来源：http://www.blog.tarul.cn/Article/details/gtedkqxax.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.sjlbkw.cn/Article/details/gvwaxugky.sHtML

[S24] C：获取本地时间
来源：http://www.blog.bbcook.cn/Article/details/gwbweikji.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.tarul.cn/Article/details/gffhsblro.sHtML

[S25] C：内存拷贝
来源：http://mobile.fktsv.cn/Article/details/gnmbnxoct.sHtML

memcpy(dst, src, n);
来源：http://m.share.yfazqb.com/Article/details/gjmprslkm.sHtML

[S26] C：内存清零
来源：http://mobile.fktsv.cn/Article/details/gkynsubjk.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fktsv.cn/Article/details/giycgcqtc.sHtML

[S27] C：定义常量
来源：http://wap.bbcook.cn/Article/details/gkorfbrzf.sHtML

const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gdzwgampj.sHtML

[S28] C：静态变量
来源：http://mobile.fktsv.cn/Article/details/gcawvmvmr.sHtML

static int counter = 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkunxtrxq.sHtML

[S29] C：变参函数
来源：http://www.m.share.bbcook.cn/Article/details/gwmdpmkao.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.yfazqb.com/Article/details/gzgygrhgp.sHtML

[S30] C：头文件保护
来源：http://read.share.tarul.cn/Article/details/gmgmhmaml.sHtML

#ifndef X_H
来源：http://www.m.share.yfazqb.com/Article/details/gvslicxvw.sHtML

#define X_H
来源：http://wap.epnwcf.com/Article/details/gifacgwep.sHtML

#endif
来源：http://www.share.yfazqb.com/Article/details/gczzjqgpx.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gvxlyunon.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/gknssyqse.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gqyzujinm.sHtML

[S32] C++：字符串
来源：http://baike.sjlbkw.cn/Article/details/glmaokspx.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.bbcook.cn/Article/details/gusgtcaxs.sHtML

[S33] C++：vector 增删
来源：http://3g.fktsv.cn/Article/details/godlqsrzs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.bbcook.cn/Article/details/georpcmkt.sHtML

[S34] C++：遍历 vector
来源：http://baike.yfazqb.com/Article/details/gkhrkkins.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.yfazqb.com/Article/details/gclezoigo.sHtML

[S35] C++：map
来源：http://www.blog.tarul.cn/Article/details/gjspzfguu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gqhmlmkih.sHtML

[S36] C++：unordered_map
来源：http://www.blog.sjlbkw.cn/Article/details/gyguvnhds.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gctwmfsfr.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/gksrvnvtq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.bbcook.cn/Article/details/ghipfznwl.sHtML

[S38] C++：排序
来源：http://read.share.epnwcf.com/Article/details/gybdvnzsj.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.bbcook.cn/Article/details/giqviwjvv.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.epnwcf.com/Article/details/gxqfwippj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/gmhivwzqy.sHtML

[S40] C++：查找元素
来源：http://www.m.share.epnwcf.com/Article/details/gnlfaiwro.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.tarul.cn/Article/details/gkhskppdj.sHtML

[S41] C++：类与构造函数
来源：http://www.share.epnwcf.com/Article/details/gmoobsdrw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/ggfxxhoyn.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.yfazqb.com/Article/details/gqtypylpx.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.epnwcf.com/Article/details/gynbpkrof.sHtML

[S43] C++：智能指针
来源：http://read.share.sjlbkw.cn/Article/details/gagytoazz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.vehdjk.com/Article/details/gnglglyck.sHtML

[S44] C++：引用传参
来源：http://www.blog.yfazqb.com/Article/details/godtxtwzx.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fktsv.cn/Article/details/gpvrdltun.sHtML

[S45] C++：lambda
来源：http://m.share.vehdjk.com/Article/details/gczhdzbsv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.sjlbkw.cn/Article/details/gloygjmpm.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fktsv.cn/Article/details/gwcuomzwx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.vehdjk.com/Article/details/gnaomiwhj.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.sjlbkw.cn/Article/details/gwkybocdc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.vehdjk.com/Article/details/gqyfqokwh.sHtML

[S48] C++：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gpvxeyggf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fktsv.cn/Article/details/gnqececbs.sHtML

while (std::getline(in, line)) { }
来源：http://blog.sjlbkw.cn/Article/details/gbskxqnza.sHtML

[S49] C++：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gfrhqarzr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.yfazqb.com/Article/details/gxbejauxs.sHtML

[S50] C++：格式化数字
来源：http://3g.fktsv.cn/Article/details/gklsvbjdm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gcmplcish.sHtML

[S51] C++：显式类型转换
来源：http://blog.fktsv.cn/Article/details/gtsdbbutc.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gmraoambh.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/ggijzfrbr.sHtML

int size() const noexcept { return n_; }
来源：http://wap.epnwcf.com/Article/details/gduwehiwm.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/gedsnwbej.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.epnwcf.com/Article/details/gswtgbfpn.sHtML

[S54] C++：异常处理
来源：http://mobile.yfazqb.com/Article/details/gzxuiucdm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.tarul.cn/Article/details/geyzyqhzo.sHtML

[S55] C++：结构化绑定
来源：http://read.share.tarul.cn/Article/details/gyodfezii.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fktsv.cn/Article/details/gfhvocfjc.sHtML

[S56] C++：optional
来源：http://baike.epnwcf.com/Article/details/gqjhknylq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fktsv.cn/Article/details/gwozbihga.sHtML

[S57] C++：编译期常量
来源：http://baike.sjlbkw.cn/Article/details/gtqwhlvxu.sHtML

constexpr int N = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gkfqoidaz.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/grwnqvzhs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/gtwrknkoy.sHtML

[S59] C++：静态断言
来源：http://3g.bbcook.cn/Article/details/glvgliagu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.bbcook.cn/Article/details/geoskgldi.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.vehdjk.com/Article/details/gxmduekly.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gthlzilvz.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gcbiwxqyk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gcwmhdfly.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glrvnseoe.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.tarul.cn/Article/details/guyhhioik.sHtML

println("Hello")
来源：http://m.share.yfazqb.com/Article/details/gnhslfduc.sHtML

[T02] Kotlin：变量
来源：http://m.share.fktsv.cn/Article/details/gbimxawpq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.sjlbkw.cn/Article/details/gcbapixsq.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fktsv.cn/Article/details/gishnaoid.sHtML

"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/glfngvqvo.sHtML

[T04] Kotlin：空安全
来源：http://mobile.epnwcf.com/Article/details/gwbjoberc.sHtML

val n: String? = null;  n?.length
来源：http://wap.yfazqb.com/Article/details/gkwdheudy.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.vehdjk.com/Article/details/gpoluuhxv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fktsv.cn/Article/details/gjvybzenx.sHtML

[T06] Kotlin：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gjrofzidf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.yfazqb.com/Article/details/gajwhnrlv.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.bbcook.cn/Article/details/gvfpvclan.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.vehdjk.com/Article/details/garfkoqff.sHtML

[T08] Kotlin：数据类
来源：http://mobile.bbcook.cn/Article/details/gafkqycds.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.tarul.cn/Article/details/glbmiedbx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.tarul.cn/Article/details/gcilyjedl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.epnwcf.com/Article/details/gdcgfpcsv.sHtML

[T10] Kotlin：默认参数
来源：http://blog.epnwcf.com/Article/details/gkpoqheom.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.epnwcf.com/Article/details/gzfdzulog.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fktsv.cn/Article/details/gzjpaebfy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.tarul.cn/Article/details/getafcici.sHtML

[T12] Kotlin：解构声明
来源：http://blog.yfazqb.com/Article/details/guspxossq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gpsrrcixj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.vehdjk.com/Article/details/gfaouitdf.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.tarul.cn/Article/details/gphaiedjn.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/gtjbjwzdn.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gksjeggec.sHtML

[T15] Kotlin：接口
来源：http://m.share.bbcook.cn/Article/details/gqffderdw.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.vehdjk.com/Article/details/gajkqyssp.sHtML

[T16] Swift：Hello World
来源：http://baike.yfazqb.com/Article/details/gtlnivokj.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/glemnybos.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fktsv.cn/Article/details/gggxqmkdv.sHtML

var a = 1;  let b = 2
来源：http://blog.vehdjk.com/Article/details/ghqcibufd.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gswbwfwrv.sHtML

"值: \(b)"
来源：http://www.blog.sjlbkw.cn/Article/details/gksopxjqs.sHtML

[T19] Swift：可选绑定
来源：http://www.share.bbcook.cn/Article/details/gbulrpync.sHtML

if let n = opt { print(n) }
来源：http://wap.bbcook.cn/Article/details/gyvsjjhpu.sHtML

[T20] Swift：数组操作
来源：http://mobile.vehdjk.com/Article/details/gzcqjsdow.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.tarul.cn/Article/details/gsjjjmlyh.sHtML

[T21] Swift：遍历
来源：http://www.m.share.epnwcf.com/Article/details/grqfynbsd.sHtML

for x in a { print(x) }
来源：http://www.share.sjlbkw.cn/Article/details/gjrowcdpt.sHtML

[T22] Swift：字典
来源：http://www.m.share.bbcook.cn/Article/details/gxxartvuq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.bbcook.cn/Article/details/gprxdskti.sHtML

[T23] Swift：函数
来源：http://baike.epnwcf.com/Article/details/ghodhrqum.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.vehdjk.com/Article/details/gkwjervjf.sHtML

[T24] Swift：闭包
来源：http://m.share.fktsv.cn/Article/details/gmydythxg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fktsv.cn/Article/details/glxhgzibo.sHtML

[T25] Swift：结构体
来源：http://3g.yfazqb.com/Article/details/gkjdelnba.sHtML

struct P { var x: Int }
来源：http://blog.tarul.cn/Article/details/gwduyjdqa.sHtML

[T26] Swift：类与重写
来源：http://www.share.sjlbkw.cn/Article/details/gkcfvunkk.sHtML

class A: Base { override func f() {} }
来源：http://3g.epnwcf.com/Article/details/grpgwhhiq.sHtML

[T27] Swift：错误处理
来源：http://blog.vehdjk.com/Article/details/gzzfyplws.sHtML

do { try f() } catch { print(error) }
来源：http://blog.sjlbkw.cn/Article/details/gnzfpguri.sHtML

[T28] Swift：枚举
来源：http://www.blog.vehdjk.com/Article/details/gtnoekzcu.sHtML

enum Color { case red, green }
来源：http://blog.bbcook.cn/Article/details/guikbgiyf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.vehdjk.com/Article/details/gdkqdmxmi.sHtML

guard let x = opt else { return }
来源：http://www.m.share.yfazqb.com/Article/details/gacxtqeme.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/guiryonkc.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.tarul.cn/Article/details/gxdscvmrc.sHtML

[T31] Lua：Hello World
来源：http://www.share.bbcook.cn/Article/details/gwyawmoxf.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/gcyeidrhy.sHtML

[T32] Lua：局部变量
来源：http://mobile.bbcook.cn/Article/details/grckjuarf.sHtML

local a = 1
来源：http://www.m.share.yfazqb.com/Article/details/gktqhdlqi.sHtML

[T33] Lua：表（数组）
来源：http://www.share.bbcook.cn/Article/details/gjssuefxa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.epnwcf.com/Article/details/gyxilvumz.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fktsv.cn/Article/details/gognagiad.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.sjlbkw.cn/Article/details/gkyzvuokh.sHtML

[T35] Lua：字典表
来源：http://3g.vehdjk.com/Article/details/gwudaoxsz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.bbcook.cn/Article/details/gzrhihvlh.sHtML

[T36] Lua：函数
来源：http://3g.sjlbkw.cn/Article/details/gwqignawq.sHtML

function add(a, b) return a + b end
来源：http://3g.bbcook.cn/Article/details/giepvycba.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/ggefahfuq.sHtML

"a" .. "b"
来源：http://3g.epnwcf.com/Article/details/gpxjwhasx.sHtML

[T38] Lua：条件
来源：http://www.share.fktsv.cn/Article/details/gpmgjtotu.sHtML

if x > 0 then print("正") end
来源：http://blog.tarul.cn/Article/details/gpmrlwfbh.sHtML

[T39] Lua：模式匹配
来源：http://baike.vehdjk.com/Article/details/ggkjmptbt.sHtML

string.find(s, "%d+")
来源：http://m.share.sjlbkw.cn/Article/details/gbdwrjbgb.sHtML

[T40] Lua：元表
来源：http://mobile.fktsv.cn/Article/details/gjalstzco.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fktsv.cn/Article/details/gwxpoyvrz.sHtML

[T41] Perl：Hello World
来源：http://m.share.bbcook.cn/Article/details/gqellhouz.sHtML

print "Hello\n";
来源：http://m.share.fktsv.cn/Article/details/gqcswnnfd.sHtML

[T42] Perl：变量类型
来源：http://m.share.yfazqb.com/Article/details/grlzfrran.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.tarul.cn/Article/details/ggzfduesy.sHtML

[T43] Perl：字符串插值
来源：http://blog.yfazqb.com/Article/details/gdswysgej.sHtML

"值: $a"
来源：http://mobile.epnwcf.com/Article/details/gfpjiebvv.sHtML

[T44] Perl：条件
来源：http://www.blog.epnwcf.com/Article/details/gbykiddvr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.vehdjk.com/Article/details/gucdwdawz.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.vehdjk.com/Article/details/gtxsjwbut.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.tarul.cn/Article/details/gldqqsgul.sHtML

[T46] Perl：哈希操作
来源：http://wap.yfazqb.com/Article/details/gbtkeboop.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.bbcook.cn/Article/details/gurbvlovu.sHtML


<!-- 参考信息 -->