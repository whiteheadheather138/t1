代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gilxghxub.sHtML

[R48] awk 取指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gushkhbro.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.tarul.cn/Article/details/gdulyzksl.sHtML

[R49] awk 带条件
来源：http://read.share.bbcook.cn/Article/details/gegrsmtpq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.tarul.cn/Article/details/gzvpvvzea.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/gofshwpdr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gwmcraugm.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/gnhasxipj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fktsv.cn/Article/details/ggxuvqbow.sHtML

[R52] 统计行数
来源：http://mobile.yfazqb.com/Article/details/gspgaculc.sHtML

wc -l a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gtevyuvdo.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.vehdjk.com/Article/details/gntqutxto.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.epnwcf.com/Article/details/gwlzwhegu.sHtML

[R54] 比较两个文件
来源：http://www.share.bbcook.cn/Article/details/gnubxckqs.sHtML

diff a.txt b.txt
来源：http://blog.sjlbkw.cn/Article/details/gpexmgmty.sHtML

[R55] 压缩与解压
来源：http://mobile.fktsv.cn/Article/details/gsgvsayrd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.epnwcf.com/Article/details/ghrlsdaan.sHtML

[R56] 远程拷贝
来源：http://www.share.bbcook.cn/Article/details/gaponvqtp.sHtML

scp file user@host:/path/
来源：http://blog.tarul.cn/Article/details/gtmjmnfam.sHtML

[R57] 远程执行命令
来源：http://3g.fktsv.cn/Article/details/gzrwubbjx.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/gmckixxti.sHtML

[R58] 下载文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gedpbelqe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.tarul.cn/Article/details/gfbjuksay.sHtML

[R59] 发 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gqserdfrc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.epnwcf.com/Article/details/gyukgmjhw.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gzzkeeueg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.tarul.cn/Article/details/gyopuwnum.sHtML

[R61] 磁盘占用
来源：http://baike.sjlbkw.cn/Article/details/ghgnknvtz.sHtML

df -h;  du -sh *
来源：http://www.share.sjlbkw.cn/Article/details/gylvnjefp.sHtML

[R62] 找最占空间的文件
来源：http://wap.epnwcf.com/Article/details/gutevtdvy.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.vehdjk.com/Article/details/gmbixojup.sHtML

[R63] 内存与进程
来源：http://www.share.sjlbkw.cn/Article/details/gjeuyltbe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/giwdreeuw.sHtML

[R64] 结束进程
来源：http://blog.vehdjk.com/Article/details/gxrjausgj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fktsv.cn/Article/details/gfbyspjrf.sHtML

[R65] 查看端口占用
来源：http://m.share.yfazqb.com/Article/details/gvabdcght.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.tarul.cn/Article/details/gbwfsmjje.sHtML

[R66] 定时任务
来源：http://read.share.yfazqb.com/Article/details/gjkwsbttn.sHtML

crontab -e;  crontab -l
来源：http://m.share.yfazqb.com/Article/details/goltugbvc.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.bbcook.cn/Article/details/gvferbjlg.sHtML

openssl rand -hex 16
来源：http://read.share.yfazqb.com/Article/details/gbcwfrxol.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.bbcook.cn/Article/details/gsoxkmsnd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.tarul.cn/Article/details/glolbtgpj.sHtML

[R69] 生成随机密码
来源：http://m.share.vehdjk.com/Article/details/glhcqfwht.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.sjlbkw.cn/Article/details/geixsusbd.sHtML

[R70] 时间戳与互转
来源：http://www.blog.tarul.cn/Article/details/gtgnlyumy.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fktsv.cn/Article/details/geyezqbkz.sHtML

[R71] 日期格式化
来源：http://baike.epnwcf.com/Article/details/gaimvuljo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.tarul.cn/Article/details/grbvhxmmw.sHtML

[R72] 等待端口就绪
来源：http://baike.epnwcf.com/Article/details/gkpnwkuiq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gxfkgwbep.sHtML

[R73] 分割大日志
来源：http://3g.yfazqb.com/Article/details/gcxwhfkod.sHtML

split -l 1000 big.log part_
来源：http://wap.sjlbkw.cn/Article/details/gcjeeuefd.sHtML

[R74] 批量重命名
来源：http://www.m.share.sjlbkw.cn/Article/details/gsestkkcs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fktsv.cn/Article/details/gysaqutih.sHtML

[R75] 导出环境变量
来源：http://3g.vehdjk.com/Article/details/givqbwtrv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.yfazqb.com/Article/details/gujfjmfkw.sHtML

[R76] 使用临时文件
来源：http://baike.bbcook.cn/Article/details/ghdivcygt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/glgspvkyr.sHtML

[R77] 读取用户输入
来源：http://read.share.epnwcf.com/Article/details/gmvldvmfk.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/gvzdbppjk.sHtML

[R78] 交互式菜单
来源：http://www.share.epnwcf.com/Article/details/gfehvubpk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/gqlropkmp.sHtML

[R79] 解析命令行选项
来源：http://baike.tarul.cn/Article/details/gmcarsdue.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/ggqiawkem.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.bbcook.cn/Article/details/gbawwgcsl.sHtML

time ./run.sh
来源：http://baike.epnwcf.com/Article/details/gcpxzgohw.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gysbxufql.sHtML

S. C / C++ 专题
来源：http://m.share.bbcook.cn/Article/details/gqzjauwog.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gdadwgylz.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/gfzmxxcrd.sHtML

#include <stdio.h>
来源：http://3g.fktsv.cn/Article/details/ggtwrtghv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.vehdjk.com/Article/details/gmrrnfkzv.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fktsv.cn/Article/details/ggiusgjbl.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.yfazqb.com/Article/details/gexvasbpy.sHtML

[S03] C：读入整数
来源：http://blog.fktsv.cn/Article/details/gqlafucpw.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fktsv.cn/Article/details/glbutzizm.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/gqcfuurhg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gxxvssjzm.sHtML

[S05] C：字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/grskscqqi.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/glwcjqirj.sHtML

[S06] C：字符串比较
来源：http://m.share.bbcook.cn/Article/details/gyrnwcsat.sHtML

strcmp(a, b) == 0
来源：http://blog.epnwcf.com/Article/details/geecyjyna.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.epnwcf.com/Article/details/gfdtgikfd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.vehdjk.com/Article/details/gcuuljbsp.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.vehdjk.com/Article/details/guyecnhsu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.tarul.cn/Article/details/gpffcuhau.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.epnwcf.com/Article/details/gmsabwflj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/gwvucyvaa.sHtML

[S10] C：指针与解引用
来源：http://blog.vehdjk.com/Article/details/gongtaaqr.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fktsv.cn/Article/details/gbxbmtltb.sHtML

[S11] C：逐行读文件
来源：http://blog.tarul.cn/Article/details/gmkgbmlxr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.vehdjk.com/Article/details/gwycifwmj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/gdokgirrt.sHtML

fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gmwtouuda.sHtML

[S12] C：写文件
来源：http://3g.bbcook.cn/Article/details/grlzepnba.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gdafpojhz.sHtML

[S13] C：宏定义
来源：http://read.share.sjlbkw.cn/Article/details/guayhlyuq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.yfazqb.com/Article/details/gvimsdjdo.sHtML

[S14] C：枚举
来源：http://blog.fktsv.cn/Article/details/gequvqpyj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fktsv.cn/Article/details/gpsoaccxo.sHtML

[S15] C：类型转换
来源：http://www.share.yfazqb.com/Article/details/gnesninyn.sHtML

(double) a / b
来源：http://blog.epnwcf.com/Article/details/gnhextscz.sHtML

[S16] C：位操作置位
来源：http://read.share.tarul.cn/Article/details/gblwxuvql.sHtML

x |= (1 << 3);
来源：http://www.m.share.epnwcf.com/Article/details/giwvxemkw.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gzxiabrlb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fktsv.cn/Article/details/gixobdvvn.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gonnlaqts.sHtML

int main(int argc, char **argv)
来源：http://www.share.fktsv.cn/Article/details/gyuegyqwc.sHtML

[S19] C：快速排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxkcjpja.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/ggrxnmbck.sHtML

[S20] C：二分查找
来源：http://wap.yfazqb.com/Article/details/gvgzcnbnn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/gfdenpxse.sHtML

[S21] C：字符类别判断
来源：http://3g.fktsv.cn/Article/details/ggzqhzvks.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.sjlbkw.cn/Article/details/gjavwuqhi.sHtML

[S22] C：字符串转数字
来源：http://m.share.tarul.cn/Article/details/gmoxwbhft.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.vehdjk.com/Article/details/ghbatoowb.sHtML

[S23] C：随机数
来源：http://wap.sjlbkw.cn/Article/details/gzqcrspds.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.yfazqb.com/Article/details/gtixpyeat.sHtML

[S24] C：获取本地时间
来源：http://3g.epnwcf.com/Article/details/gpdnponrs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.yfazqb.com/Article/details/gsiembkci.sHtML

[S25] C：内存拷贝
来源：http://3g.tarul.cn/Article/details/gokgsqntk.sHtML

memcpy(dst, src, n);
来源：http://wap.fktsv.cn/Article/details/gevjkrird.sHtML

[S26] C：内存清零
来源：http://blog.epnwcf.com/Article/details/gihjnxeje.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fktsv.cn/Article/details/gwzdnjxmn.sHtML

[S27] C：定义常量
来源：http://wap.epnwcf.com/Article/details/gerjnramg.sHtML

const double PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gfkujwzwh.sHtML

[S28] C：静态变量
来源：http://read.share.yfazqb.com/Article/details/gwtsteqfh.sHtML

static int counter = 0;
来源：http://baike.fktsv.cn/Article/details/gbhtcnnvd.sHtML

[S29] C：变参函数
来源：http://baike.vehdjk.com/Article/details/giybvzcbs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.tarul.cn/Article/details/gqxtyqlua.sHtML

[S30] C：头文件保护
来源：http://www.m.share.epnwcf.com/Article/details/glyayrtaj.sHtML

#ifndef X_H
来源：http://baike.epnwcf.com/Article/details/gjmuwnjcd.sHtML

#define X_H
来源：http://baike.yfazqb.com/Article/details/gojepxjda.sHtML

#endif
来源：http://www.share.vehdjk.com/Article/details/gwikgkipk.sHtML

[S31] C++：Hello World
来源：http://read.share.fktsv.cn/Article/details/gxubdixwr.sHtML

#include <iostream>
来源：http://3g.tarul.cn/Article/details/gdwlqolts.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.epnwcf.com/Article/details/gzcvysplp.sHtML

[S32] C++：字符串
来源：http://mobile.vehdjk.com/Article/details/gmniskhgl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fktsv.cn/Article/details/gyxfnvlfb.sHtML

[S33] C++：vector 增删
来源：http://m.share.epnwcf.com/Article/details/gjdbwwauc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.yfazqb.com/Article/details/gkvpzzrww.sHtML

[S34] C++：遍历 vector
来源：http://wap.sjlbkw.cn/Article/details/grcmwccqo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.vehdjk.com/Article/details/gaqhmrvvr.sHtML

[S35] C++：map
来源：http://www.blog.vehdjk.com/Article/details/goxkxikbu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/glsnguxzz.sHtML

[S36] C++：unordered_map
来源：http://blog.yfazqb.com/Article/details/gmxhlerlr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gkhzmnekh.sHtML

[S37] C++：set
来源：http://wap.tarul.cn/Article/details/gwosnegfh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.sjlbkw.cn/Article/details/grbqnymsa.sHtML

[S38] C++：排序
来源：http://read.share.vehdjk.com/Article/details/gjylbbpyb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.yfazqb.com/Article/details/ghsosjgkb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.bbcook.cn/Article/details/ggcjrwnli.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.sjlbkw.cn/Article/details/gtcqslsnx.sHtML

[S40] C++：查找元素
来源：http://wap.yfazqb.com/Article/details/gpimqxtdb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fktsv.cn/Article/details/geqjyrzit.sHtML

[S41] C++：类与构造函数
来源：http://read.share.yfazqb.com/Article/details/gdbssoxbj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.sjlbkw.cn/Article/details/gobhvxuvr.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.sjlbkw.cn/Article/details/gqvxfqmfo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.bbcook.cn/Article/details/gvwgsvuxy.sHtML

[S43] C++：智能指针
来源：http://www.share.bbcook.cn/Article/details/gysjklyzk.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.epnwcf.com/Article/details/gjjrngkwu.sHtML

[S44] C++：引用传参
来源：http://blog.yfazqb.com/Article/details/gunootedh.sHtML

void inc(int &x) { ++x; }
来源：http://3g.yfazqb.com/Article/details/gzuarrakj.sHtML

[S45] C++：lambda
来源：http://wap.tarul.cn/Article/details/gztzzhslf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.yfazqb.com/Article/details/guzinwbhb.sHtML

[S46] C++：函数模板
来源：http://www.share.tarul.cn/Article/details/gclgnvdgg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.epnwcf.com/Article/details/gtcsydiot.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.tarul.cn/Article/details/gavgvjdcu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.epnwcf.com/Article/details/gtcufbqti.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gcinqcesr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.epnwcf.com/Article/details/gojtbcyhb.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/gadlkqgnv.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/gjjqmwnxn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.sjlbkw.cn/Article/details/giicyuria.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.bbcook.cn/Article/details/gasovxlvw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gjwinofxo.sHtML

[S51] C++：显式类型转换
来源：http://m.share.tarul.cn/Article/details/gysldyxao.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.epnwcf.com/Article/details/gpkpowozf.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.sjlbkw.cn/Article/details/ghmelvqic.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.yfazqb.com/Article/details/gruzldmtz.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/govdiqxbx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.tarul.cn/Article/details/gydxcncpc.sHtML

[S54] C++：异常处理
来源：http://blog.vehdjk.com/Article/details/gvgajirjz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.vehdjk.com/Article/details/gbnmxfuab.sHtML

[S55] C++：结构化绑定
来源：http://read.share.bbcook.cn/Article/details/gkqwuxudr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.vehdjk.com/Article/details/gwvizxodo.sHtML

[S56] C++：optional
来源：http://3g.vehdjk.com/Article/details/ggeezlhjz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/gpqdturlx.sHtML

[S57] C++：编译期常量
来源：http://wap.bbcook.cn/Article/details/gculphjkz.sHtML

constexpr int N = 10;
来源：http://www.share.yfazqb.com/Article/details/gghzmoynu.sHtML

[S58] C++：命名空间
来源：http://www.share.bbcook.cn/Article/details/ggozzrzhl.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.yfazqb.com/Article/details/gsoavoqsi.sHtML

[S59] C++：静态断言
来源：http://read.share.epnwcf.com/Article/details/gvockkicc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.sjlbkw.cn/Article/details/giusxrbws.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.yfazqb.com/Article/details/ghgvwpyke.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gjihsvvyr.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gnajjobjm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gezzikepk.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/giifavruj.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gqhqdmynh.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/ghljxukkd.sHtML

[T02] Kotlin：变量
来源：http://www.blog.tarul.cn/Article/details/gxqtydvcv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.yfazqb.com/Article/details/gzngudhbv.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.vehdjk.com/Article/details/gdlhimmzd.sHtML

"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gumuzasgy.sHtML

[T04] Kotlin：空安全
来源：http://baike.tarul.cn/Article/details/garajmtod.sHtML

val n: String? = null;  n?.length
来源：http://mobile.yfazqb.com/Article/details/gxakbjrgu.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fktsv.cn/Article/details/gtrhlkfzq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.tarul.cn/Article/details/ggzmoxflc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.bbcook.cn/Article/details/gtpdfldor.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.epnwcf.com/Article/details/gzifnuqbq.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gdaomqjvr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/gwntjdwpz.sHtML

[T08] Kotlin：数据类
来源：http://wap.tarul.cn/Article/details/ghkbesjip.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gfvcfzlam.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fktsv.cn/Article/details/gaawrwisa.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.sjlbkw.cn/Article/details/grskzmznm.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fktsv.cn/Article/details/gxevpxwra.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.vehdjk.com/Article/details/gklnhrbem.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/gdvsrjllm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.yfazqb.com/Article/details/gmmauanbc.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.tarul.cn/Article/details/gohvxffdi.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gmnrxoswl.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.vehdjk.com/Article/details/gmzuvfsal.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.vehdjk.com/Article/details/ghgjmwjfg.sHtML

[T14] Kotlin：循环
来源：http://wap.tarul.cn/Article/details/grekkirsj.sHtML

for (i in 1..10) println(i)
来源：http://www.share.tarul.cn/Article/details/gidbhvjfz.sHtML

[T15] Kotlin：接口
来源：http://read.share.sjlbkw.cn/Article/details/gnxtdfdxz.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.epnwcf.com/Article/details/gmasmbmye.sHtML

[T16] Swift：Hello World
来源：http://mobile.fktsv.cn/Article/details/grccykxiq.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gqcmknmmg.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.yfazqb.com/Article/details/gqyhzwwjk.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gcjtxlyst.sHtML

[T18] Swift：字符串插值
来源：http://3g.epnwcf.com/Article/details/ghynbgsvh.sHtML

"值: \(b)"
来源：http://3g.yfazqb.com/Article/details/gcxoicxpd.sHtML

[T19] Swift：可选绑定
来源：http://www.share.yfazqb.com/Article/details/gvltvizkc.sHtML

if let n = opt { print(n) }
来源：http://www.share.fktsv.cn/Article/details/gokddtgub.sHtML

[T20] Swift：数组操作
来源：http://read.share.bbcook.cn/Article/details/grzofktkq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.yfazqb.com/Article/details/gnfbpbzmf.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/gmhkdmyiq.sHtML

for x in a { print(x) }
来源：http://www.blog.sjlbkw.cn/Article/details/gkbqqqzlr.sHtML

[T22] Swift：字典
来源：http://blog.yfazqb.com/Article/details/gywthmlbc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.sjlbkw.cn/Article/details/gqvyqwgms.sHtML

[T23] Swift：函数
来源：http://read.share.fktsv.cn/Article/details/gcndfpdtd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.vehdjk.com/Article/details/gpfcfrxhd.sHtML

[T24] Swift：闭包
来源：http://baike.bbcook.cn/Article/details/gliibcvik.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gufwqfndn.sHtML

[T25] Swift：结构体
来源：http://www.m.share.epnwcf.com/Article/details/gzmleknvy.sHtML

struct P { var x: Int }
来源：http://m.share.sjlbkw.cn/Article/details/gufbspvxt.sHtML

[T26] Swift：类与重写
来源：http://blog.tarul.cn/Article/details/guewrrqgx.sHtML

class A: Base { override func f() {} }
来源：http://m.share.vehdjk.com/Article/details/gyklzutem.sHtML

[T27] Swift：错误处理
来源：http://3g.tarul.cn/Article/details/gsbyumwqu.sHtML

do { try f() } catch { print(error) }
来源：http://3g.yfazqb.com/Article/details/gehpoxnly.sHtML

[T28] Swift：枚举
来源：http://blog.bbcook.cn/Article/details/gvatwsjls.sHtML

enum Color { case red, green }
来源：http://baike.tarul.cn/Article/details/gsqxeyjmp.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.tarul.cn/Article/details/gjzfdtvar.sHtML

guard let x = opt else { return }
来源：http://read.share.sjlbkw.cn/Article/details/gteabvwbf.sHtML

[T30] Swift：协议
来源：http://www.blog.epnwcf.com/Article/details/gqcmhlmfy.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.yfazqb.com/Article/details/gsstnyenh.sHtML

[T31] Lua：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gltrrsqdx.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/genmqwtht.sHtML

[T32] Lua：局部变量
来源：http://www.share.fktsv.cn/Article/details/ghsuufkqf.sHtML

local a = 1
来源：http://www.blog.fktsv.cn/Article/details/gdxkcifax.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.epnwcf.com/Article/details/gidlgrtpk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.yfazqb.com/Article/details/goiyrsbne.sHtML

[T34] Lua：遍历表
来源：http://baike.tarul.cn/Article/details/gyhkdmmzb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.bbcook.cn/Article/details/gjypdqkan.sHtML

[T35] Lua：字典表
来源：http://3g.epnwcf.com/Article/details/gbvdrplkg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fktsv.cn/Article/details/gsuywnxzn.sHtML

[T36] Lua：函数
来源：http://mobile.sjlbkw.cn/Article/details/gxdioynxf.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/gfjjwlzla.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gpjkshccb.sHtML

"a" .. "b"
来源：http://mobile.vehdjk.com/Article/details/gedociwxm.sHtML

[T38] Lua：条件
来源：http://read.share.tarul.cn/Article/details/gysygcvtt.sHtML

if x > 0 then print("正") end
来源：http://m.share.epnwcf.com/Article/details/gtqmglrde.sHtML

[T39] Lua：模式匹配
来源：http://baike.bbcook.cn/Article/details/gcukitweh.sHtML

string.find(s, "%d+")
来源：http://m.share.vehdjk.com/Article/details/ggbyeakwd.sHtML

[T40] Lua：元表
来源：http://mobile.bbcook.cn/Article/details/gxbghwqgj.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fktsv.cn/Article/details/gncdrdpcw.sHtML

[T41] Perl：Hello World
来源：http://wap.bbcook.cn/Article/details/giuiyykis.sHtML

print "Hello\n";
来源：http://wap.epnwcf.com/Article/details/gzmqcclsa.sHtML

[T42] Perl：变量类型
来源：http://www.share.yfazqb.com/Article/details/gblwsubpm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.epnwcf.com/Article/details/gdhsdhwgy.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/gpqpipymb.sHtML

"值: $a"
来源：http://m.share.epnwcf.com/Article/details/gtaxsrpdm.sHtML

[T44] Perl：条件
来源：http://www.share.sjlbkw.cn/Article/details/gegtfisch.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.bbcook.cn/Article/details/gawymimrd.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.tarul.cn/Article/details/gruxmysan.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.yfazqb.com/Article/details/gulmgpjjs.sHtML

[T46] Perl：哈希操作
来源：http://blog.bbcook.cn/Article/details/govemmhhw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.vehdjk.com/Article/details/gayrsfeux.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.yfazqb.com/Article/details/gzsakfwiv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.sjlbkw.cn/Article/details/gnwbrfcdy.sHtML

[T48] Perl：正则替换
来源：http://read.share.tarul.cn/Article/details/gpeisugvd.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.bbcook.cn/Article/details/gpwmqnimf.sHtML

[T49] Perl：函数
来源：http://mobile.bbcook.cn/Article/details/gyzjxzavu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/ggqaeglxy.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gbpobyaiw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.sjlbkw.cn/Article/details/gybonoegk.sHtML


<!-- 参考信息 -->