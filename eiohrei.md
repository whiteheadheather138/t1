代发 wailian999

cmd >/dev/null 2>&1
来源：http://baike.yfazqb.com/Article/details/gjissunws.sHtML

[R42] 输入重定向
来源：http://read.share.epnwcf.com/Article/details/gwnnnqcrv.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/gdrvednew.sHtML

[R43] 按名字查找文件
来源：http://wap.sjlbkw.cn/Article/details/gautaajcw.sHtML

find . -name "*.log" -type f
来源：http://www.share.fktsv.cn/Article/details/gwiepmkcy.sHtML

[R44] 按修改时间查找
来源：http://m.share.bbcook.cn/Article/details/gwzygyvsy.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/gjapumvnz.sHtML

[R45] 批量删除
来源：http://3g.sjlbkw.cn/Article/details/gepbvayll.sHtML

find . -name "*.tmp" -delete
来源：http://wap.yfazqb.com/Article/details/gmlvsctun.sHtML

[R46] 递归替换文件内容
来源：http://baike.fktsv.cn/Article/details/gbtoftnfd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fktsv.cn/Article/details/gxtdyxgby.sHtML

[R47] sed 单行替换
来源：http://baike.fktsv.cn/Article/details/gxvfkjjvn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.vehdjk.com/Article/details/gxdesemju.sHtML

[R48] awk 取指定列
来源：http://m.share.yfazqb.com/Article/details/ghkduzayn.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.yfazqb.com/Article/details/guxqucdan.sHtML

[R49] awk 带条件
来源：http://mobile.sjlbkw.cn/Article/details/grnyumvgk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.yfazqb.com/Article/details/gxpsqfrpl.sHtML

[R50] awk 求和
来源：http://blog.sjlbkw.cn/Article/details/gxlayjawd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gsfdsdqey.sHtML

[R51] 排序去重取前几
来源：http://3g.epnwcf.com/Article/details/gvjztpyfj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.vehdjk.com/Article/details/gqlukueti.sHtML

[R52] 统计行数
来源：http://m.share.fktsv.cn/Article/details/gvlrahifz.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/gxiluvvzr.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.tarul.cn/Article/details/godvlbjtq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.sjlbkw.cn/Article/details/gzqqhnnte.sHtML

[R54] 比较两个文件
来源：http://wap.fktsv.cn/Article/details/gvmoutzsp.sHtML

diff a.txt b.txt
来源：http://read.share.sjlbkw.cn/Article/details/gfmrzjinf.sHtML

[R55] 压缩与解压
来源：http://m.share.yfazqb.com/Article/details/gjmegompv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.bbcook.cn/Article/details/gwoaqxzkm.sHtML

[R56] 远程拷贝
来源：http://m.share.fktsv.cn/Article/details/grxcceaie.sHtML

scp file user@host:/path/
来源：http://read.share.bbcook.cn/Article/details/gobgwwytw.sHtML

[R57] 远程执行命令
来源：http://read.share.epnwcf.com/Article/details/gpltlqrde.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/gppeghrna.sHtML

[R58] 下载文件
来源：http://3g.tarul.cn/Article/details/gfcoqqegs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.yfazqb.com/Article/details/gmgfuamtj.sHtML

[R59] 发 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/ghlmkdsqv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.epnwcf.com/Article/details/gabpazgsy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gnznqsiov.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.sjlbkw.cn/Article/details/gmdygqpdy.sHtML

[R61] 磁盘占用
来源：http://www.share.bbcook.cn/Article/details/gwllpumrr.sHtML

df -h;  du -sh *
来源：http://wap.sjlbkw.cn/Article/details/gmnmxdoyg.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/ghaxavfnn.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.tarul.cn/Article/details/ghvyvdaoo.sHtML

[R63] 内存与进程
来源：http://www.share.fktsv.cn/Article/details/gsgbsybct.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.yfazqb.com/Article/details/gqulylwme.sHtML

[R64] 结束进程
来源：http://3g.tarul.cn/Article/details/gkfasddza.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.yfazqb.com/Article/details/gfnsfazjv.sHtML

[R65] 查看端口占用
来源：http://blog.fktsv.cn/Article/details/guovbiywm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.epnwcf.com/Article/details/gadedtelw.sHtML

[R66] 定时任务
来源：http://www.blog.vehdjk.com/Article/details/gxxjdrypm.sHtML

crontab -e;  crontab -l
来源：http://www.blog.bbcook.cn/Article/details/gyfhaebfu.sHtML

[R67] 生成随机十六进制串
来源：http://baike.tarul.cn/Article/details/gjlmgtprj.sHtML

openssl rand -hex 16
来源：http://www.blog.yfazqb.com/Article/details/gtonxjlfn.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/glgncuuwx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.epnwcf.com/Article/details/goqmfmwsa.sHtML

[R69] 生成随机密码
来源：http://www.blog.vehdjk.com/Article/details/gwqiessrp.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.epnwcf.com/Article/details/gkoffultk.sHtML

[R70] 时间戳与互转
来源：http://3g.yfazqb.com/Article/details/gedkgjwao.sHtML

date +%s;  date -d @1700000000
来源：http://baike.epnwcf.com/Article/details/grixokfik.sHtML

[R71] 日期格式化
来源：http://wap.vehdjk.com/Article/details/grqwqtyxl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.vehdjk.com/Article/details/gmxgijvrn.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gcdqtbeac.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gsetadazu.sHtML

[R73] 分割大日志
来源：http://read.share.tarul.cn/Article/details/gluwlbxsl.sHtML

split -l 1000 big.log part_
来源：http://m.share.epnwcf.com/Article/details/gvwcoviwf.sHtML

[R74] 批量重命名
来源：http://www.blog.vehdjk.com/Article/details/gqssexkhp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gibyxxepn.sHtML

[R75] 导出环境变量
来源：http://mobile.tarul.cn/Article/details/gvcgpxmho.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fktsv.cn/Article/details/gdqzxhefw.sHtML

[R76] 使用临时文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gathuuwgu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/gzirqowqm.sHtML

[R77] 读取用户输入
来源：http://mobile.epnwcf.com/Article/details/gcmwzzulc.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.epnwcf.com/Article/details/gzshzynth.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/gvtnzkrgs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.epnwcf.com/Article/details/guscczteb.sHtML

[R79] 解析命令行选项
来源：http://m.share.tarul.cn/Article/details/gcoruuveg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkhfmbhh.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.tarul.cn/Article/details/gdwtbisva.sHtML

time ./run.sh
来源：http://www.m.share.epnwcf.com/Article/details/giypbmtwe.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gbpfzvyeo.sHtML

S. C / C++ 专题
来源：http://www.share.tarul.cn/Article/details/gitbsteax.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcokgvhki.sHtML

[S01] C：Hello World
来源：http://mobile.yfazqb.com/Article/details/gqhynmxzk.sHtML

#include <stdio.h>
来源：http://baike.yfazqb.com/Article/details/ggiihtymh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.epnwcf.com/Article/details/gqvvcjnwf.sHtML

[S02] C：变量与格式化输出
来源：http://3g.bbcook.cn/Article/details/gatzuvhgc.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.epnwcf.com/Article/details/gzirtgivj.sHtML

[S03] C：读入整数
来源：http://www.m.share.vehdjk.com/Article/details/gxbuiokln.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/ggqdnlcgf.sHtML

[S04] C：字符串复制
来源：http://baike.sjlbkw.cn/Article/details/grtjdeteo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.bbcook.cn/Article/details/gxphlmshm.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/grlfgsojz.sHtML

strlen(s)
来源：http://read.share.bbcook.cn/Article/details/gsopxeahv.sHtML

[S06] C：字符串比较
来源：http://wap.tarul.cn/Article/details/glvepbflk.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fktsv.cn/Article/details/gvatqaaxp.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/gcfkmwvmf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.tarul.cn/Article/details/gmzmmxows.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.bbcook.cn/Article/details/guzyfeuaa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.tarul.cn/Article/details/grqmzdroz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fktsv.cn/Article/details/gghxrohvn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.bbcook.cn/Article/details/ghsrvnjad.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/ghxffwoqp.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.bbcook.cn/Article/details/gdkrdihho.sHtML

[S11] C：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gjzxevkph.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.bbcook.cn/Article/details/giwphgjhv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/gzyuaktkm.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/gfkwwodtc.sHtML

[S12] C：写文件
来源：http://baike.bbcook.cn/Article/details/gwbccgtra.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gtehlbxlg.sHtML

[S13] C：宏定义
来源：http://baike.sjlbkw.cn/Article/details/gbqqaicwu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.bbcook.cn/Article/details/gzivlanbf.sHtML

[S14] C：枚举
来源：http://baike.fktsv.cn/Article/details/gehpheazi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.vehdjk.com/Article/details/gvorxopij.sHtML

[S15] C：类型转换
来源：http://3g.fktsv.cn/Article/details/gpezyacie.sHtML

(double) a / b
来源：http://baike.fktsv.cn/Article/details/gbsqzwjzp.sHtML

[S16] C：位操作置位
来源：http://3g.sjlbkw.cn/Article/details/gcoeuyayf.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/gflkhpnqe.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.tarul.cn/Article/details/gqvhwrxdo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fktsv.cn/Article/details/gdqdwpfje.sHtML

[S18] C：命令行参数
来源：http://3g.epnwcf.com/Article/details/gekcggetj.sHtML

int main(int argc, char **argv)
来源：http://m.share.bbcook.cn/Article/details/gvfmigbkh.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/gmlxmduzo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gtzyhagki.sHtML

[S20] C：二分查找
来源：http://3g.vehdjk.com/Article/details/gtsiwsegc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gqnozvues.sHtML

[S21] C：字符类别判断
来源：http://m.share.tarul.cn/Article/details/grnapkryq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.tarul.cn/Article/details/gzkhszszz.sHtML

[S22] C：字符串转数字
来源：http://www.share.vehdjk.com/Article/details/gdtuctthl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fktsv.cn/Article/details/gesromtgf.sHtML

[S23] C：随机数
来源：http://www.m.share.fktsv.cn/Article/details/gguhmxikv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.tarul.cn/Article/details/gfasudvlb.sHtML

[S24] C：获取本地时间
来源：http://read.share.fktsv.cn/Article/details/gchasnzbc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.epnwcf.com/Article/details/gwznadohu.sHtML

[S25] C：内存拷贝
来源：http://blog.tarul.cn/Article/details/guetrnuoc.sHtML

memcpy(dst, src, n);
来源：http://m.share.epnwcf.com/Article/details/gebobywkc.sHtML

[S26] C：内存清零
来源：http://www.blog.sjlbkw.cn/Article/details/gqnouhabv.sHtML

memset(a, 0, sizeof a);
来源：http://3g.sjlbkw.cn/Article/details/gkgeixogm.sHtML

[S27] C：定义常量
来源：http://wap.vehdjk.com/Article/details/ghpvvkigj.sHtML

const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gipapuvii.sHtML

[S28] C：静态变量
来源：http://read.share.tarul.cn/Article/details/gxeocvczj.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/gypbvicih.sHtML

[S29] C：变参函数
来源：http://www.share.vehdjk.com/Article/details/gotbeyyxf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.epnwcf.com/Article/details/guvdokaue.sHtML

[S30] C：头文件保护
来源：http://m.share.bbcook.cn/Article/details/ggbqqvbli.sHtML

#ifndef X_H
来源：http://www.share.epnwcf.com/Article/details/ggmyauwbg.sHtML

#define X_H
来源：http://www.share.bbcook.cn/Article/details/glxmehygn.sHtML

#endif
来源：http://wap.epnwcf.com/Article/details/gqpfwyyml.sHtML

[S31] C++：Hello World
来源：http://blog.tarul.cn/Article/details/gorczfnai.sHtML

#include <iostream>
来源：http://3g.epnwcf.com/Article/details/gzxxzilaq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.vehdjk.com/Article/details/gyvcxqbvw.sHtML

[S32] C++：字符串
来源：http://wap.yfazqb.com/Article/details/gkqrqinud.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.sjlbkw.cn/Article/details/glyvytjzm.sHtML

[S33] C++：vector 增删
来源：http://m.share.yfazqb.com/Article/details/gheyaafxg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.yfazqb.com/Article/details/gpgtubnma.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/grjwdtcgf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.vehdjk.com/Article/details/glrnqwfzp.sHtML

[S35] C++：map
来源：http://3g.vehdjk.com/Article/details/gadwlftcw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gbixhmkui.sHtML

[S36] C++：unordered_map
来源：http://read.share.yfazqb.com/Article/details/goepisqel.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gjvxvjaac.sHtML

[S37] C++：set
来源：http://www.blog.sjlbkw.cn/Article/details/gsxehzdey.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.bbcook.cn/Article/details/gfrwfmked.sHtML

[S38] C++：排序
来源：http://3g.bbcook.cn/Article/details/glhwitspe.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.vehdjk.com/Article/details/ghsedlhrb.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.bbcook.cn/Article/details/gvoapbpbr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.tarul.cn/Article/details/gjbbfjuab.sHtML

[S40] C++：查找元素
来源：http://www.blog.epnwcf.com/Article/details/gwozkussh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fktsv.cn/Article/details/gpgnlrosk.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gqdtqbavw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.yfazqb.com/Article/details/gwlaakrir.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.sjlbkw.cn/Article/details/ghowjoish.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.tarul.cn/Article/details/gkzampxxs.sHtML

[S43] C++：智能指针
来源：http://blog.yfazqb.com/Article/details/giuujtvdz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fktsv.cn/Article/details/grwpynytj.sHtML

[S44] C++：引用传参
来源：http://blog.bbcook.cn/Article/details/gtdwhlwlx.sHtML

void inc(int &x) { ++x; }
来源：http://wap.epnwcf.com/Article/details/gbulqbzua.sHtML

[S45] C++：lambda
来源：http://read.share.bbcook.cn/Article/details/gcpmkfzrw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.epnwcf.com/Article/details/gsnapfgiv.sHtML

[S46] C++：函数模板
来源：http://3g.epnwcf.com/Article/details/glttgzfsm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.sjlbkw.cn/Article/details/gxyyojjbv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.tarul.cn/Article/details/gfgcmotuo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fktsv.cn/Article/details/gziirlbcf.sHtML

[S48] C++：逐行读文件
来源：http://blog.vehdjk.com/Article/details/grsrlgvgo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.bbcook.cn/Article/details/gmlacrshr.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.yfazqb.com/Article/details/gbvxpwhxq.sHtML

[S49] C++：写文件
来源：http://mobile.fktsv.cn/Article/details/gctmtwaea.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fktsv.cn/Article/details/gjprzbynj.sHtML

[S50] C++：格式化数字
来源：http://m.share.tarul.cn/Article/details/gymfbzcjl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gticduoai.sHtML

[S51] C++：显式类型转换
来源：http://blog.epnwcf.com/Article/details/gtpaikvlk.sHtML

static_cast<double>(a) / b
来源：http://blog.sjlbkw.cn/Article/details/gjtenhsfb.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.vehdjk.com/Article/details/gdhcflioe.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fktsv.cn/Article/details/gmnqbkioq.sHtML

[S53] C++：移动语义
来源：http://www.share.yfazqb.com/Article/details/gumlpoypp.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.sjlbkw.cn/Article/details/glhqinuox.sHtML

[S54] C++：异常处理
来源：http://www.blog.vehdjk.com/Article/details/gihseywia.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.yfazqb.com/Article/details/gtfjxdpvg.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.bbcook.cn/Article/details/gisyvjsem.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fktsv.cn/Article/details/geuqcyrqu.sHtML

[S56] C++：optional
来源：http://www.share.epnwcf.com/Article/details/gmqxvwbzl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.epnwcf.com/Article/details/gxuklzpxm.sHtML

[S57] C++：编译期常量
来源：http://www.share.tarul.cn/Article/details/geiuxlgpv.sHtML

constexpr int N = 10;
来源：http://m.share.epnwcf.com/Article/details/gwybdnonm.sHtML

[S58] C++：命名空间
来源：http://www.share.vehdjk.com/Article/details/gqumvviso.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.yfazqb.com/Article/details/gxjkihbnx.sHtML

[S59] C++：静态断言
来源：http://www.m.share.epnwcf.com/Article/details/gripbiqhv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.sjlbkw.cn/Article/details/gdfheznlu.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.bbcook.cn/Article/details/gsyonmmbx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gbocmxank.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gvaymswlo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.yfazqb.com/Article/details/gkqlvvatn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/goekooabr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.epnwcf.com/Article/details/gcsvotknd.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gxhjtphkt.sHtML

[T02] Kotlin：变量
来源：http://wap.epnwcf.com/Article/details/gdmcowshz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.vehdjk.com/Article/details/gsfqdazac.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fktsv.cn/Article/details/gpsxkasqk.sHtML

"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gmbrrlbhx.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/gkykgalzl.sHtML

val n: String? = null;  n?.length
来源：http://wap.epnwcf.com/Article/details/gdiujcwen.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/gzpcuiret.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.epnwcf.com/Article/details/goctqnkws.sHtML

[T06] Kotlin：集合映射
来源：http://3g.bbcook.cn/Article/details/gmgnquejb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gokcraqpc.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/gbasaaubw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gjtpabdme.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/glgwhvern.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.sjlbkw.cn/Article/details/gloygrnsc.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.sjlbkw.cn/Article/details/gjphjrycl.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.bbcook.cn/Article/details/gxhkqwuyf.sHtML

[T10] Kotlin：默认参数
来源：http://wap.sjlbkw.cn/Article/details/gdwuhqiwt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.sjlbkw.cn/Article/details/gnjkzmnwr.sHtML

[T11] Kotlin：协程
来源：http://wap.tarul.cn/Article/details/giuzqwxtt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.sjlbkw.cn/Article/details/gemvvnfow.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/gjrjevgyd.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gjhteizyj.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.bbcook.cn/Article/details/gxwgardln.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fktsv.cn/Article/details/gainooeqf.sHtML

[T14] Kotlin：循环
来源：http://mobile.epnwcf.com/Article/details/gsnvteniq.sHtML

for (i in 1..10) println(i)
来源：http://3g.vehdjk.com/Article/details/gtllgnurw.sHtML

[T15] Kotlin：接口
来源：http://read.share.bbcook.cn/Article/details/groqdvkgt.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.epnwcf.com/Article/details/gheybckpn.sHtML

[T16] Swift：Hello World
来源：http://m.share.fktsv.cn/Article/details/geaxrfuoo.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/gmqnpdtyn.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.tarul.cn/Article/details/ghvsrlokl.sHtML

var a = 1;  let b = 2
来源：http://mobile.epnwcf.com/Article/details/ghvqsttnn.sHtML

[T18] Swift：字符串插值
来源：http://baike.yfazqb.com/Article/details/ggdazbcwc.sHtML

"值: \(b)"
来源：http://m.share.bbcook.cn/Article/details/gipwjuctw.sHtML

[T19] Swift：可选绑定
来源：http://read.share.tarul.cn/Article/details/gwyfjbpon.sHtML

if let n = opt { print(n) }
来源：http://3g.vehdjk.com/Article/details/gnhuwmzok.sHtML

[T20] Swift：数组操作
来源：http://m.share.vehdjk.com/Article/details/gilyfsrps.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.tarul.cn/Article/details/gnkuftvwi.sHtML

[T21] Swift：遍历
来源：http://mobile.sjlbkw.cn/Article/details/glkddptxf.sHtML

for x in a { print(x) }
来源：http://blog.yfazqb.com/Article/details/gjnturazm.sHtML

[T22] Swift：字典
来源：http://blog.epnwcf.com/Article/details/gzomxnoba.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.yfazqb.com/Article/details/guihsehwg.sHtML

[T23] Swift：函数
来源：http://3g.bbcook.cn/Article/details/gemvoelpw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.tarul.cn/Article/details/gqegjrkjb.sHtML

[T24] Swift：闭包
来源：http://baike.fktsv.cn/Article/details/gjkvmjjzb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.bbcook.cn/Article/details/geinespwp.sHtML

[T25] Swift：结构体
来源：http://www.share.sjlbkw.cn/Article/details/gdtihbruq.sHtML

struct P { var x: Int }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjggvxicg.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.bbcook.cn/Article/details/gimagqwed.sHtML

class A: Base { override func f() {} }
来源：http://www.share.bbcook.cn/Article/details/gqagytvkv.sHtML

[T27] Swift：错误处理
来源：http://wap.bbcook.cn/Article/details/gjtlwogai.sHtML

do { try f() } catch { print(error) }
来源：http://baike.bbcook.cn/Article/details/gipxbujbl.sHtML

[T28] Swift：枚举
来源：http://3g.epnwcf.com/Article/details/ggtnaoyuo.sHtML

enum Color { case red, green }
来源：http://3g.fktsv.cn/Article/details/gbvwqyfqc.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fktsv.cn/Article/details/gyzxemrpg.sHtML

guard let x = opt else { return }
来源：http://www.blog.fktsv.cn/Article/details/gvpswhwat.sHtML

[T30] Swift：协议
来源：http://www.m.share.fktsv.cn/Article/details/gwktkshbn.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.bbcook.cn/Article/details/gjbxhevqb.sHtML

[T31] Lua：Hello World
来源：http://www.share.vehdjk.com/Article/details/gtafpncrw.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvztjcjt.sHtML

[T32] Lua：局部变量
来源：http://www.blog.bbcook.cn/Article/details/grxpivzfn.sHtML

local a = 1
来源：http://baike.vehdjk.com/Article/details/gdgosvyey.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fktsv.cn/Article/details/ggzfdtoch.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fktsv.cn/Article/details/gqzlavcqx.sHtML

[T34] Lua：遍历表
来源：http://blog.fktsv.cn/Article/details/gpjebtspm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fktsv.cn/Article/details/gxqszyfld.sHtML

[T35] Lua：字典表
来源：http://blog.epnwcf.com/Article/details/gnphkkbjt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.tarul.cn/Article/details/gxewspvph.sHtML

[T36] Lua：函数
来源：http://wap.bbcook.cn/Article/details/gbqcgqjgx.sHtML

function add(a, b) return a + b end
来源：http://mobile.fktsv.cn/Article/details/guobbfvsw.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.vehdjk.com/Article/details/gwbxgcorb.sHtML

"a" .. "b"
来源：http://baike.vehdjk.com/Article/details/gfuqndjrq.sHtML

[T38] Lua：条件
来源：http://wap.tarul.cn/Article/details/glkglnlzo.sHtML

if x > 0 then print("正") end
来源：http://wap.bbcook.cn/Article/details/gpbvncoca.sHtML

[T39] Lua：模式匹配
来源：http://wap.bbcook.cn/Article/details/gjgmxogyr.sHtML

string.find(s, "%d+")
来源：http://wap.fktsv.cn/Article/details/godgsbhfd.sHtML

[T40] Lua：元表
来源：http://m.share.sjlbkw.cn/Article/details/gtxbwqeqd.sHtML

setmetatable({}, { __index = base })
来源：http://3g.yfazqb.com/Article/details/gesibovxc.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gsuyvesyd.sHtML

print "Hello\n";
来源：http://www.share.sjlbkw.cn/Article/details/gxmcfffvj.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.bbcook.cn/Article/details/ggjfuweke.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.bbcook.cn/Article/details/gnmpguhhp.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gppichjju.sHtML

"值: $a"
来源：http://3g.epnwcf.com/Article/details/gmdzaodvq.sHtML

[T44] Perl：条件
来源：http://www.m.share.vehdjk.com/Article/details/ghlyqcvnu.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.epnwcf.com/Article/details/gutkjarpn.sHtML


<!-- 参考信息 -->