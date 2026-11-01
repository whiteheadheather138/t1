代发 wailian999

find . -name "*.tmp" -delete
来源：http://baike.tarul.cn/Article/details/gzswddkaa.sHtML

[R46] 递归替换文件内容
来源：http://blog.yfazqb.com/Article/details/glulzxrag.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.sjlbkw.cn/Article/details/guekevfbf.sHtML

[R47] sed 单行替换
来源：http://m.share.bbcook.cn/Article/details/gfsdidfvv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.tarul.cn/Article/details/ghlzdzawd.sHtML

[R48] awk 取指定列
来源：http://3g.vehdjk.com/Article/details/gqbnpnial.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gruihlaeo.sHtML

[R49] awk 带条件
来源：http://baike.vehdjk.com/Article/details/govnnacsb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.sjlbkw.cn/Article/details/gtxbyxeyt.sHtML

[R50] awk 求和
来源：http://mobile.yfazqb.com/Article/details/gyoqftypr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.yfazqb.com/Article/details/ggzkdzzde.sHtML

[R51] 排序去重取前几
来源：http://baike.bbcook.cn/Article/details/godjapfir.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.yfazqb.com/Article/details/gbujtptoa.sHtML

[R52] 统计行数
来源：http://www.share.bbcook.cn/Article/details/gmyvugdxr.sHtML

wc -l a.txt
来源：http://m.share.epnwcf.com/Article/details/gzqvisaxa.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/gcxinujve.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.tarul.cn/Article/details/gtygvyqiu.sHtML

[R54] 比较两个文件
来源：http://www.blog.fktsv.cn/Article/details/gnzqfotmq.sHtML

diff a.txt b.txt
来源：http://baike.vehdjk.com/Article/details/guguevfsu.sHtML

[R55] 压缩与解压
来源：http://blog.yfazqb.com/Article/details/gqwaxrlga.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.vehdjk.com/Article/details/gncmmvgwe.sHtML

[R56] 远程拷贝
来源：http://wap.bbcook.cn/Article/details/gmqvyuwio.sHtML

scp file user@host:/path/
来源：http://www.share.yfazqb.com/Article/details/ghqxvhkws.sHtML

[R57] 远程执行命令
来源：http://read.share.epnwcf.com/Article/details/gzipsfcar.sHtML

ssh user@host 'uptime'
来源：http://m.share.bbcook.cn/Article/details/grpvfwgkr.sHtML

[R58] 下载文件
来源：http://read.share.yfazqb.com/Article/details/gkaylylvp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gupcmhwwd.sHtML

[R59] 发 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gajdoapgx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.epnwcf.com/Article/details/gdkyszmxo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gwinxjpfz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.vehdjk.com/Article/details/gniwnbdnv.sHtML

[R61] 磁盘占用
来源：http://wap.bbcook.cn/Article/details/gvkkhuohz.sHtML

df -h;  du -sh *
来源：http://www.share.sjlbkw.cn/Article/details/gjerewuty.sHtML

[R62] 找最占空间的文件
来源：http://mobile.tarul.cn/Article/details/gpxhwjtvt.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.vehdjk.com/Article/details/gwreruozr.sHtML

[R63] 内存与进程
来源：http://www.share.bbcook.cn/Article/details/gldpgaozr.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/gxdbahtav.sHtML

[R64] 结束进程
来源：http://blog.tarul.cn/Article/details/gmvwvuxxr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fktsv.cn/Article/details/gakfjbzwm.sHtML

[R65] 查看端口占用
来源：http://www.share.epnwcf.com/Article/details/gpekbrjat.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.bbcook.cn/Article/details/gxqdzbrwa.sHtML

[R66] 定时任务
来源：http://www.blog.epnwcf.com/Article/details/givequhxq.sHtML

crontab -e;  crontab -l
来源：http://read.share.sjlbkw.cn/Article/details/gsuckfzvp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.tarul.cn/Article/details/gjxfsztrg.sHtML

openssl rand -hex 16
来源：http://read.share.fktsv.cn/Article/details/gtgbfxwkb.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/gerzplhko.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.bbcook.cn/Article/details/gjevjmpao.sHtML

[R69] 生成随机密码
来源：http://baike.bbcook.cn/Article/details/gxchrviaa.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.tarul.cn/Article/details/gnwhtpoyq.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/gqyiqubbr.sHtML

date +%s;  date -d @1700000000
来源：http://baike.sjlbkw.cn/Article/details/ghoqmuhhu.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/guavbbzlj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.yfazqb.com/Article/details/grvhfixsa.sHtML

[R72] 等待端口就绪
来源：http://blog.tarul.cn/Article/details/guuooridg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/ggmexseia.sHtML

[R73] 分割大日志
来源：http://read.share.fktsv.cn/Article/details/gkyexjalj.sHtML

split -l 1000 big.log part_
来源：http://m.share.epnwcf.com/Article/details/gjlnmasta.sHtML

[R74] 批量重命名
来源：http://read.share.fktsv.cn/Article/details/gztufkvvi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/gekcwzhhu.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gohqsgbuk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.yfazqb.com/Article/details/gotcjeoyk.sHtML

[R76] 使用临时文件
来源：http://wap.vehdjk.com/Article/details/gwrpfzewx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/glbujuzcm.sHtML

[R77] 读取用户输入
来源：http://www.m.share.bbcook.cn/Article/details/gvlbqkszb.sHtML

read -rp "请输入: " ans
来源：http://www.blog.bbcook.cn/Article/details/gidtoqpei.sHtML

[R78] 交互式菜单
来源：http://wap.epnwcf.com/Article/details/gmhaonaxc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.vehdjk.com/Article/details/gyxecxvwm.sHtML

[R79] 解析命令行选项
来源：http://baike.sjlbkw.cn/Article/details/gcfuuatpd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.epnwcf.com/Article/details/gyboozmmz.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.vehdjk.com/Article/details/gchvhwwvc.sHtML

time ./run.sh
来源：http://mobile.yfazqb.com/Article/details/grasnnkjp.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gltmwldwe.sHtML

S. C / C++ 专题
来源：http://www.blog.tarul.cn/Article/details/ghirltscx.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcdnzsszi.sHtML

[S01] C：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gvumgrwzm.sHtML

#include <stdio.h>
来源：http://wap.epnwcf.com/Article/details/grwwlanxe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/gpydqgkpe.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gtpyxpvqt.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.sjlbkw.cn/Article/details/gzfviyngy.sHtML

[S03] C：读入整数
来源：http://www.m.share.epnwcf.com/Article/details/gmjibrrhe.sHtML

int x; scanf("%d", &x);
来源：http://read.share.tarul.cn/Article/details/gcyktqcli.sHtML

[S04] C：字符串复制
来源：http://www.blog.yfazqb.com/Article/details/giruceurd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.vehdjk.com/Article/details/gcrctnkvt.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gccdirbei.sHtML

strlen(s)
来源：http://3g.tarul.cn/Article/details/gdidkaetr.sHtML

[S06] C：字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gdtieyldu.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/gpesobohw.sHtML

[S07] C：数组遍历求和
来源：http://mobile.bbcook.cn/Article/details/gcqeuysix.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.bbcook.cn/Article/details/gpzcnhnzh.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.sjlbkw.cn/Article/details/gfpjyktbr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.sjlbkw.cn/Article/details/gvnldpqcu.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fktsv.cn/Article/details/gwrhkenau.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.yfazqb.com/Article/details/ggayuuutb.sHtML

[S10] C：指针与解引用
来源：http://www.blog.vehdjk.com/Article/details/gvguzphvj.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.bbcook.cn/Article/details/gtjhjgofk.sHtML

[S11] C：逐行读文件
来源：http://read.share.tarul.cn/Article/details/ghjnoihnv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fktsv.cn/Article/details/gxpqpjzdn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.epnwcf.com/Article/details/gvlzdheoj.sHtML

fclose(f);
来源：http://mobile.epnwcf.com/Article/details/gbwgzjrnz.sHtML

[S12] C：写文件
来源：http://baike.bbcook.cn/Article/details/gddzgmfut.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fktsv.cn/Article/details/gnlbleapp.sHtML

[S13] C：宏定义
来源：http://blog.tarul.cn/Article/details/gextrrysh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.bbcook.cn/Article/details/goozycbtr.sHtML

[S14] C：枚举
来源：http://read.share.bbcook.cn/Article/details/gswiafsbt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.sjlbkw.cn/Article/details/giycrlhia.sHtML

[S15] C：类型转换
来源：http://mobile.fktsv.cn/Article/details/gkciwcuwo.sHtML

(double) a / b
来源：http://www.blog.tarul.cn/Article/details/gjqzmidis.sHtML

[S16] C：位操作置位
来源：http://read.share.epnwcf.com/Article/details/guvacbuwx.sHtML

x |= (1 << 3);
来源：http://read.share.bbcook.cn/Article/details/gcyvigave.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gowzhtatd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.epnwcf.com/Article/details/gbdpxktgs.sHtML

[S18] C：命令行参数
来源：http://read.share.bbcook.cn/Article/details/godiinbfv.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fktsv.cn/Article/details/gutxnnpxn.sHtML

[S19] C：快速排序
来源：http://baike.epnwcf.com/Article/details/ghmmhkxhm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/gcxgdfoke.sHtML

[S20] C：二分查找
来源：http://www.m.share.fktsv.cn/Article/details/gpqoxrjfs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/gbcrpvszh.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.bbcook.cn/Article/details/gjzcfrbsm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.tarul.cn/Article/details/gjhpwpfyh.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfzrcigj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/gecvkmbpk.sHtML

[S23] C：随机数
来源：http://www.share.epnwcf.com/Article/details/gudtzdair.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.epnwcf.com/Article/details/gvnpaielt.sHtML

[S24] C：获取本地时间
来源：http://www.blog.bbcook.cn/Article/details/gjfpbuhht.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fktsv.cn/Article/details/gsjrmfjok.sHtML

[S25] C：内存拷贝
来源：http://blog.epnwcf.com/Article/details/gppotlnro.sHtML

memcpy(dst, src, n);
来源：http://www.share.fktsv.cn/Article/details/gediwhplm.sHtML

[S26] C：内存清零
来源：http://m.share.tarul.cn/Article/details/gjteqvjax.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.vehdjk.com/Article/details/gdairbwmv.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/gcxutpgvo.sHtML

const double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gefdnafpr.sHtML

[S28] C：静态变量
来源：http://wap.vehdjk.com/Article/details/ghutbawoj.sHtML

static int counter = 0;
来源：http://mobile.fktsv.cn/Article/details/gnhkjxwkg.sHtML

[S29] C：变参函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gufhyxfgx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.epnwcf.com/Article/details/gyocvqvjo.sHtML

[S30] C：头文件保护
来源：http://read.share.yfazqb.com/Article/details/gyluboikg.sHtML

#ifndef X_H
来源：http://www.m.share.tarul.cn/Article/details/ghdomexmn.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/ghaohbhbj.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gnulesxth.sHtML

[S31] C++：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gdcgouucg.sHtML

#include <iostream>
来源：http://www.blog.sjlbkw.cn/Article/details/ggvendzfc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.epnwcf.com/Article/details/gsuejlqhj.sHtML

[S32] C++：字符串
来源：http://read.share.tarul.cn/Article/details/gfukiodhu.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.tarul.cn/Article/details/giijnkxyf.sHtML

[S33] C++：vector 增删
来源：http://www.share.vehdjk.com/Article/details/gaifnkhqb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.vehdjk.com/Article/details/gymrjiloo.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.yfazqb.com/Article/details/gjiuvhbiv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.bbcook.cn/Article/details/gvvyjxzeb.sHtML

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/gxrwklrts.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.bbcook.cn/Article/details/geymgeuvq.sHtML

[S36] C++：unordered_map
来源：http://3g.yfazqb.com/Article/details/gqgtwqwdw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gktloipny.sHtML

[S37] C++：set
来源：http://mobile.epnwcf.com/Article/details/gsbrhapjn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.vehdjk.com/Article/details/gmnkoddel.sHtML

[S38] C++：排序
来源：http://www.blog.vehdjk.com/Article/details/gowssybak.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.bbcook.cn/Article/details/giswriqki.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.sjlbkw.cn/Article/details/gqsklgqay.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.vehdjk.com/Article/details/gkaevqbfy.sHtML

[S40] C++：查找元素
来源：http://blog.yfazqb.com/Article/details/gltrwtlmz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.bbcook.cn/Article/details/gozknjigr.sHtML

[S41] C++：类与构造函数
来源：http://wap.yfazqb.com/Article/details/gnyvxmdhk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.sjlbkw.cn/Article/details/gevniggfj.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.vehdjk.com/Article/details/gkdwsrqtx.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fktsv.cn/Article/details/gmwswhxkq.sHtML

[S43] C++：智能指针
来源：http://mobile.sjlbkw.cn/Article/details/gnbqsafet.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.tarul.cn/Article/details/gzrlnidfn.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/gfmkoswav.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.tarul.cn/Article/details/grsawfqbz.sHtML

[S45] C++：lambda
来源：http://read.share.epnwcf.com/Article/details/gdggbdqyh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.epnwcf.com/Article/details/gwptgypsu.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fktsv.cn/Article/details/gdbuctfcn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.sjlbkw.cn/Article/details/geddyyjpn.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.bbcook.cn/Article/details/gezkhywau.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fktsv.cn/Article/details/growdhfva.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gobxfpkhf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.yfazqb.com/Article/details/gnhyduwei.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/gethpvtpr.sHtML

[S49] C++：写文件
来源：http://mobile.bbcook.cn/Article/details/geypoenel.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.vehdjk.com/Article/details/glnwfkqsy.sHtML

[S50] C++：格式化数字
来源：http://3g.epnwcf.com/Article/details/giboukboq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gpcdgfajq.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.yfazqb.com/Article/details/gzvqsbaur.sHtML

static_cast<double>(a) / b
来源：http://mobile.sjlbkw.cn/Article/details/gdtfrohls.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.epnwcf.com/Article/details/gunzvfobd.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.vehdjk.com/Article/details/gaccwjwmy.sHtML

[S53] C++：移动语义
来源：http://blog.fktsv.cn/Article/details/glfzrdiuc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbzmoyoj.sHtML

[S54] C++：异常处理
来源：http://mobile.tarul.cn/Article/details/gmqaoyhsb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/gfcvdqvdf.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.tarul.cn/Article/details/gpmjpojdb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.vehdjk.com/Article/details/gpuwgqhfu.sHtML

[S56] C++：optional
来源：http://3g.sjlbkw.cn/Article/details/gzytrwrrh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fktsv.cn/Article/details/gzrlumkie.sHtML

[S57] C++：编译期常量
来源：http://3g.fktsv.cn/Article/details/gektfdwap.sHtML

constexpr int N = 10;
来源：http://wap.bbcook.cn/Article/details/gmdochugp.sHtML

[S58] C++：命名空间
来源：http://blog.sjlbkw.cn/Article/details/glydddkor.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fktsv.cn/Article/details/grzcutucm.sHtML

[S59] C++：静态断言
来源：http://read.share.yfazqb.com/Article/details/gulhqgpqh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fktsv.cn/Article/details/grdkotwil.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.tarul.cn/Article/details/goavaomfz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.bbcook.cn/Article/details/gcecmzatk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gjrecxtpt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/gjjxstwll.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghndnbeav.sHtML

[T01] Kotlin：Hello World
来源：http://baike.tarul.cn/Article/details/gffrywrbp.sHtML

println("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gshubdjwm.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.yfazqb.com/Article/details/goklkmkbd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.sjlbkw.cn/Article/details/gdipmnucu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.yfazqb.com/Article/details/gadkaficy.sHtML

"值: $b"
来源：http://wap.sjlbkw.cn/Article/details/gdrwegwmg.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.tarul.cn/Article/details/gqijpvemq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fktsv.cn/Article/details/gvcwegubg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.vehdjk.com/Article/details/gankeluna.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.yfazqb.com/Article/details/gexgrlqok.sHtML

[T06] Kotlin：集合映射
来源：http://blog.yfazqb.com/Article/details/gatpoamrv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.tarul.cn/Article/details/gfkejmuzc.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.yfazqb.com/Article/details/gxcnppdxk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.vehdjk.com/Article/details/gpimfhrhf.sHtML

[T08] Kotlin：数据类
来源：http://3g.fktsv.cn/Article/details/gecmgjyyw.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/gzeekfvii.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.epnwcf.com/Article/details/gzpspffbr.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.yfazqb.com/Article/details/gexyfxnxo.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.vehdjk.com/Article/details/ggwtonqea.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.epnwcf.com/Article/details/gneshystm.sHtML

[T11] Kotlin：协程
来源：http://blog.vehdjk.com/Article/details/gzbliwcpy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.bbcook.cn/Article/details/gdujvkukf.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.epnwcf.com/Article/details/gefnckcrl.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.tarul.cn/Article/details/gkktqczum.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.sjlbkw.cn/Article/details/gegdndfjr.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fktsv.cn/Article/details/grhgnuege.sHtML

[T14] Kotlin：循环
来源：http://m.share.vehdjk.com/Article/details/gbwaalhzb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.bbcook.cn/Article/details/gkxlggwgc.sHtML

[T15] Kotlin：接口
来源：http://m.share.bbcook.cn/Article/details/gphmzcoxg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/gkyfistaf.sHtML

[T16] Swift：Hello World
来源：http://m.share.bbcook.cn/Article/details/gcmfhnxoh.sHtML

print("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gvrkqilcu.sHtML

[T17] Swift：变量与常量
来源：http://m.share.sjlbkw.cn/Article/details/geicmbiyg.sHtML

var a = 1;  let b = 2
来源：http://3g.vehdjk.com/Article/details/gtpnyouwv.sHtML

[T18] Swift：字符串插值
来源：http://blog.yfazqb.com/Article/details/gqeqgfntx.sHtML

"值: \(b)"
来源：http://m.share.fktsv.cn/Article/details/gwmfxjhoa.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.epnwcf.com/Article/details/gevaepubp.sHtML

if let n = opt { print(n) }
来源：http://3g.epnwcf.com/Article/details/gllqmfxjz.sHtML

[T20] Swift：数组操作
来源：http://baike.epnwcf.com/Article/details/gudviohcb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.tarul.cn/Article/details/gutmxisgs.sHtML

[T21] Swift：遍历
来源：http://mobile.vehdjk.com/Article/details/gcwggonnd.sHtML

for x in a { print(x) }
来源：http://baike.yfazqb.com/Article/details/gpxrzwhsv.sHtML

[T22] Swift：字典
来源：http://3g.bbcook.cn/Article/details/gbenidilp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.sjlbkw.cn/Article/details/gtoufhcrt.sHtML

[T23] Swift：函数
来源：http://wap.sjlbkw.cn/Article/details/gdgcjqwnr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.yfazqb.com/Article/details/gdepqealo.sHtML

[T24] Swift：闭包
来源：http://www.share.yfazqb.com/Article/details/gifecibev.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gwsvpslmf.sHtML

[T25] Swift：结构体
来源：http://mobile.bbcook.cn/Article/details/gelnwaslm.sHtML

struct P { var x: Int }
来源：http://m.share.sjlbkw.cn/Article/details/gaxecgwps.sHtML

[T26] Swift：类与重写
来源：http://m.share.yfazqb.com/Article/details/gefumfxcl.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.yfazqb.com/Article/details/grpsvqlre.sHtML

[T27] Swift：错误处理
来源：http://www.blog.yfazqb.com/Article/details/gaijweati.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.vehdjk.com/Article/details/gnmhcsnlr.sHtML

[T28] Swift：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gnbdydini.sHtML

enum Color { case red, green }
来源：http://mobile.yfazqb.com/Article/details/gaclobhhr.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.epnwcf.com/Article/details/gzdactofq.sHtML

guard let x = opt else { return }
来源：http://3g.tarul.cn/Article/details/gctezdvus.sHtML

[T30] Swift：协议
来源：http://baike.yfazqb.com/Article/details/gvkmefdyr.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.tarul.cn/Article/details/gbzqxvhrc.sHtML

[T31] Lua：Hello World
来源：http://www.share.epnwcf.com/Article/details/gwzrgjbsx.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/gumycelhb.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gloyyfzqx.sHtML

local a = 1
来源：http://m.share.yfazqb.com/Article/details/grszuwite.sHtML

[T33] Lua：表（数组）
来源：http://3g.yfazqb.com/Article/details/gorermeeu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.bbcook.cn/Article/details/gxdijalyu.sHtML

[T34] Lua：遍历表
来源：http://www.share.epnwcf.com/Article/details/gcxvbeovm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.vehdjk.com/Article/details/gztlybigu.sHtML

[T35] Lua：字典表
来源：http://baike.yfazqb.com/Article/details/gkpjluiku.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gfhjquoqg.sHtML

[T36] Lua：函数
来源：http://read.share.fktsv.cn/Article/details/gndhsodsa.sHtML

function add(a, b) return a + b end
来源：http://www.share.tarul.cn/Article/details/gbflbarlb.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/gpjeqlvrg.sHtML

"a" .. "b"
来源：http://read.share.fktsv.cn/Article/details/ggmhcyavf.sHtML

[T38] Lua：条件
来源：http://3g.tarul.cn/Article/details/gydvmrixq.sHtML

if x > 0 then print("正") end
来源：http://www.blog.bbcook.cn/Article/details/grarnsszq.sHtML

[T39] Lua：模式匹配
来源：http://www.share.bbcook.cn/Article/details/ghhegyhsh.sHtML

string.find(s, "%d+")
来源：http://read.share.sjlbkw.cn/Article/details/gndczldqa.sHtML

[T40] Lua：元表
来源：http://www.m.share.yfazqb.com/Article/details/giywlldnb.sHtML

setmetatable({}, { __index = base })
来源：http://baike.epnwcf.com/Article/details/ghuygcrff.sHtML

[T41] Perl：Hello World
来源：http://read.share.vehdjk.com/Article/details/ggtqwlqma.sHtML

print "Hello\n";
来源：http://wap.vehdjk.com/Article/details/gphfwhwll.sHtML

[T42] Perl：变量类型
来源：http://wap.fktsv.cn/Article/details/gmkjiltic.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.vehdjk.com/Article/details/gprcczmpa.sHtML

[T43] Perl：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gerumrrym.sHtML

"值: $a"
来源：http://read.share.sjlbkw.cn/Article/details/gtlusubni.sHtML

[T44] Perl：条件
来源：http://3g.vehdjk.com/Article/details/gwnslvare.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.bbcook.cn/Article/details/ghxsonbeg.sHtML

[T45] Perl：数组遍历
来源：http://wap.bbcook.cn/Article/details/ghwhdppin.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.vehdjk.com/Article/details/guiinshse.sHtML

[T46] Perl：哈希操作
来源：http://www.share.yfazqb.com/Article/details/gyivhtiuw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.yfazqb.com/Article/details/gtmnlheyn.sHtML

[T47] Perl：正则捕获
来源：http://blog.tarul.cn/Article/details/gaffrfnta.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fktsv.cn/Article/details/gohjodwfy.sHtML

[T48] Perl：正则替换
来源：http://wap.sjlbkw.cn/Article/details/gcddebkdp.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fktsv.cn/Article/details/gqiobeykr.sHtML


<!-- 参考信息 -->