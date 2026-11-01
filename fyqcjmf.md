代发 wailian999

find . -name "*.log" -type f
来源：http://m.share.sjlbkw.cn/Article/details/gkxmszlch.sHtML

[R44] 按修改时间查找
来源：http://mobile.sjlbkw.cn/Article/details/gpvylfdyr.sHtML

find . -mtime -7 -type f
来源：http://m.share.yfazqb.com/Article/details/ghalavufg.sHtML

[R45] 批量删除
来源：http://m.share.bbcook.cn/Article/details/gnzhggifq.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/gtqsuugtg.sHtML

[R46] 递归替换文件内容
来源：http://blog.tarul.cn/Article/details/gyabaxodl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.yfazqb.com/Article/details/gmcdhjbgp.sHtML

[R47] sed 单行替换
来源：http://3g.epnwcf.com/Article/details/gefjbuyux.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.yfazqb.com/Article/details/gunshbqgs.sHtML

[R48] awk 取指定列
来源：http://www.blog.yfazqb.com/Article/details/gjkukoyoi.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.epnwcf.com/Article/details/gfpmgtypk.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/gvbzylrex.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.bbcook.cn/Article/details/gyrpyctwp.sHtML

[R50] awk 求和
来源：http://wap.vehdjk.com/Article/details/gfsfrpicf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gvbxmoofe.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/ggawqjxra.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fktsv.cn/Article/details/gxszzvcrx.sHtML

[R52] 统计行数
来源：http://wap.fktsv.cn/Article/details/gyzyhhkgv.sHtML

wc -l a.txt
来源：http://mobile.epnwcf.com/Article/details/gjrmnyvvt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fktsv.cn/Article/details/gimsanajf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.tarul.cn/Article/details/gsivprrjg.sHtML

[R54] 比较两个文件
来源：http://3g.sjlbkw.cn/Article/details/gyrrvmnas.sHtML

diff a.txt b.txt
来源：http://wap.vehdjk.com/Article/details/ghrrwoyie.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/gwvxktgzn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/ggcqsglep.sHtML

[R56] 远程拷贝
来源：http://3g.yfazqb.com/Article/details/glztbmprw.sHtML

scp file user@host:/path/
来源：http://www.blog.epnwcf.com/Article/details/gmjwaqhgg.sHtML

[R57] 远程执行命令
来源：http://blog.sjlbkw.cn/Article/details/gubtueuqt.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fktsv.cn/Article/details/gxngmlpys.sHtML

[R58] 下载文件
来源：http://read.share.fktsv.cn/Article/details/gweqgtjdb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.bbcook.cn/Article/details/gzvkktgre.sHtML

[R59] 发 POST JSON
来源：http://mobile.tarul.cn/Article/details/gpzmwropw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fktsv.cn/Article/details/gaxjyltsu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gxedkufln.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.epnwcf.com/Article/details/gnotemohc.sHtML

[R61] 磁盘占用
来源：http://baike.bbcook.cn/Article/details/glhlkbqpi.sHtML

df -h;  du -sh *
来源：http://www.m.share.fktsv.cn/Article/details/gyegtsyrw.sHtML

[R62] 找最占空间的文件
来源：http://www.share.tarul.cn/Article/details/gzvzvxvkk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fktsv.cn/Article/details/gwpwkhrcu.sHtML

[R63] 内存与进程
来源：http://baike.bbcook.cn/Article/details/gpursaeic.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.bbcook.cn/Article/details/gmyyhboku.sHtML

[R64] 结束进程
来源：http://www.m.share.fktsv.cn/Article/details/gwnwyjhfe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.sjlbkw.cn/Article/details/gjopjdzfd.sHtML

[R65] 查看端口占用
来源：http://www.share.bbcook.cn/Article/details/gvdagasly.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.yfazqb.com/Article/details/gulipmzeg.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/gwwjdrjci.sHtML

crontab -e;  crontab -l
来源：http://3g.sjlbkw.cn/Article/details/gizoxdcvx.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.yfazqb.com/Article/details/gujmacgtu.sHtML

openssl rand -hex 16
来源：http://wap.epnwcf.com/Article/details/gwgcnavln.sHtML

[R68] 计算文件校验值
来源：http://blog.vehdjk.com/Article/details/gxgdlwfiq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fktsv.cn/Article/details/gxtxlvufe.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/giipdkazz.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.tarul.cn/Article/details/grrzesxtn.sHtML

[R70] 时间戳与互转
来源：http://blog.bbcook.cn/Article/details/gczczezhf.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/gvuccigew.sHtML

[R71] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/genlwyywc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.vehdjk.com/Article/details/grvovippv.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/gdhlzuhxp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/gjodthfwp.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/gvgrudrcg.sHtML

split -l 1000 big.log part_
来源：http://3g.fktsv.cn/Article/details/gfqxlbhvd.sHtML

[R74] 批量重命名
来源：http://read.share.fktsv.cn/Article/details/gjrmxhzxt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.epnwcf.com/Article/details/guiyrezvk.sHtML

[R75] 导出环境变量
来源：http://read.share.bbcook.cn/Article/details/goshaofve.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.epnwcf.com/Article/details/gbefnqgso.sHtML

[R76] 使用临时文件
来源：http://www.m.share.vehdjk.com/Article/details/gpixxvnbe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gnxlgptro.sHtML

[R77] 读取用户输入
来源：http://mobile.epnwcf.com/Article/details/geuwbessl.sHtML

read -rp "请输入: " ans
来源：http://baike.bbcook.cn/Article/details/gnaysoapz.sHtML

[R78] 交互式菜单
来源：http://m.share.yfazqb.com/Article/details/gnwdzuucv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.sjlbkw.cn/Article/details/gqqpwwekm.sHtML

[R79] 解析命令行选项
来源：http://read.share.yfazqb.com/Article/details/guoxetcqw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.yfazqb.com/Article/details/gwfzzyetl.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.bbcook.cn/Article/details/ghqofewdc.sHtML

time ./run.sh
来源：http://www.m.share.yfazqb.com/Article/details/gpptsijju.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/goisnfque.sHtML

S. C / C++ 专题
来源：http://mobile.bbcook.cn/Article/details/gljywvroh.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gawdsudvp.sHtML

[S01] C：Hello World
来源：http://baike.epnwcf.com/Article/details/gepzkfofn.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/gyqilpnii.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.epnwcf.com/Article/details/ghntupkhn.sHtML

[S02] C：变量与格式化输出
来源：http://blog.yfazqb.com/Article/details/gevcvqmzg.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.sjlbkw.cn/Article/details/ghhyahzub.sHtML

[S03] C：读入整数
来源：http://www.m.share.bbcook.cn/Article/details/gwchlokgt.sHtML

int x; scanf("%d", &x);
来源：http://www.share.vehdjk.com/Article/details/gyvukiwhh.sHtML

[S04] C：字符串复制
来源：http://m.share.tarul.cn/Article/details/gxjswsqeu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gskhlnbdf.sHtML

[S05] C：字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/ginkmggef.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/gjsiyvlyd.sHtML

[S06] C：字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gxxyedoxn.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.tarul.cn/Article/details/gokwwoinv.sHtML

[S07] C：数组遍历求和
来源：http://mobile.bbcook.cn/Article/details/ghocgulfh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.yfazqb.com/Article/details/goeycbblb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fktsv.cn/Article/details/gkgdelirm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.vehdjk.com/Article/details/gviyejsdo.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.bbcook.cn/Article/details/gavewlrmq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fktsv.cn/Article/details/gnxndmzfg.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/gafdbxibs.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.yfazqb.com/Article/details/gqdnhrdcv.sHtML

[S11] C：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gcpdjoyao.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.sjlbkw.cn/Article/details/gxmfkvjwq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.tarul.cn/Article/details/givlqjgqo.sHtML

fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gqiehtgxq.sHtML

[S12] C：写文件
来源：http://mobile.bbcook.cn/Article/details/ggsexxmnj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gogntbdab.sHtML

[S13] C：宏定义
来源：http://wap.fktsv.cn/Article/details/gjbwpktxs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.yfazqb.com/Article/details/gcskurvlo.sHtML

[S14] C：枚举
来源：http://3g.vehdjk.com/Article/details/gogiscsaw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.epnwcf.com/Article/details/gwlhzbuip.sHtML

[S15] C：类型转换
来源：http://blog.bbcook.cn/Article/details/gonhnwfdv.sHtML

(double) a / b
来源：http://blog.epnwcf.com/Article/details/ghbxnmeua.sHtML

[S16] C：位操作置位
来源：http://blog.epnwcf.com/Article/details/gfwxvlgcl.sHtML

x |= (1 << 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gawucmwee.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gsuuqwpmo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.yfazqb.com/Article/details/grsrriylz.sHtML

[S18] C：命令行参数
来源：http://read.share.vehdjk.com/Article/details/gphlkcmsw.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gvgigfulv.sHtML

[S19] C：快速排序
来源：http://www.m.share.fktsv.cn/Article/details/gjijwdqox.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gxeceakvo.sHtML

[S20] C：二分查找
来源：http://3g.yfazqb.com/Article/details/gvuibdrsh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/gqfvwhghl.sHtML

[S21] C：字符类别判断
来源：http://www.blog.vehdjk.com/Article/details/gglhrxcmj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fktsv.cn/Article/details/gmrykaebd.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/gfsefmale.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.sjlbkw.cn/Article/details/gdvplmngt.sHtML

[S23] C：随机数
来源：http://baike.sjlbkw.cn/Article/details/gfmfvsayl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/gdqqwavfe.sHtML

[S24] C：获取本地时间
来源：http://3g.vehdjk.com/Article/details/gcwtpofah.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.tarul.cn/Article/details/gnazwslte.sHtML

[S25] C：内存拷贝
来源：http://www.blog.vehdjk.com/Article/details/gbswtipnp.sHtML

memcpy(dst, src, n);
来源：http://3g.tarul.cn/Article/details/gmkrscbfn.sHtML

[S26] C：内存清零
来源：http://wap.vehdjk.com/Article/details/gdascmtqh.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.vehdjk.com/Article/details/gkgdebvia.sHtML

[S27] C：定义常量
来源：http://wap.vehdjk.com/Article/details/gftqypanp.sHtML

const double PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/ggiyinxbc.sHtML

[S28] C：静态变量
来源：http://www.blog.sjlbkw.cn/Article/details/gmgvrafmc.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/gkvkxtgcd.sHtML

[S29] C：变参函数
来源：http://3g.yfazqb.com/Article/details/gbycwzudm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.bbcook.cn/Article/details/ghxctwqxe.sHtML

[S30] C：头文件保护
来源：http://read.share.tarul.cn/Article/details/gafsnqogw.sHtML

#ifndef X_H
来源：http://www.blog.yfazqb.com/Article/details/gcedzsyfe.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/gznxsncsr.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gyfgyxaxr.sHtML

[S31] C++：Hello World
来源：http://mobile.bbcook.cn/Article/details/gqxhxyqtz.sHtML

#include <iostream>
来源：http://m.share.tarul.cn/Article/details/geypeodoy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.tarul.cn/Article/details/gtbdjetow.sHtML

[S32] C++：字符串
来源：http://wap.tarul.cn/Article/details/gnwqpsusz.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.yfazqb.com/Article/details/gmqumjtmj.sHtML

[S33] C++：vector 增删
来源：http://read.share.fktsv.cn/Article/details/gwbiynprm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.sjlbkw.cn/Article/details/ggmkapbgp.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.vehdjk.com/Article/details/gzowxrofh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fktsv.cn/Article/details/gofzfkogi.sHtML

[S35] C++：map
来源：http://wap.fktsv.cn/Article/details/gssdevnhc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gnrmmnzyh.sHtML

[S36] C++：unordered_map
来源：http://m.share.bbcook.cn/Article/details/gawamoeit.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/glqasvlzx.sHtML

[S37] C++：set
来源：http://wap.fktsv.cn/Article/details/gmtbpfzco.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/goyqkvxiq.sHtML

[S38] C++：排序
来源：http://mobile.tarul.cn/Article/details/ghnbqtvdc.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fktsv.cn/Article/details/gjboqggca.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.tarul.cn/Article/details/grraisoya.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.bbcook.cn/Article/details/gqyusleza.sHtML

[S40] C++：查找元素
来源：http://3g.fktsv.cn/Article/details/glzgnzrss.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.vehdjk.com/Article/details/gnmejnjtg.sHtML

[S41] C++：类与构造函数
来源：http://m.share.vehdjk.com/Article/details/gzdujkiki.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.epnwcf.com/Article/details/gddaocuxn.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gnymdfszd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.tarul.cn/Article/details/goajjyykh.sHtML

[S43] C++：智能指针
来源：http://mobile.vehdjk.com/Article/details/gerrfmyti.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.sjlbkw.cn/Article/details/ggabbtidb.sHtML

[S44] C++：引用传参
来源：http://baike.sjlbkw.cn/Article/details/gfwzoizpe.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.vehdjk.com/Article/details/ginimjdtb.sHtML

[S45] C++：lambda
来源：http://blog.bbcook.cn/Article/details/gerdtzgnk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fktsv.cn/Article/details/ggmegykoa.sHtML

[S46] C++：函数模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gooilstqy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.vehdjk.com/Article/details/gkyyvifzo.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.bbcook.cn/Article/details/gognytwjc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.tarul.cn/Article/details/gtuwnfvkm.sHtML

[S48] C++：逐行读文件
来源：http://wap.yfazqb.com/Article/details/glnkkrbyw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.sjlbkw.cn/Article/details/gbqyesohv.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gppobfvrd.sHtML

[S49] C++：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gwlinugkc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.bbcook.cn/Article/details/gitdfyozc.sHtML

[S50] C++：格式化数字
来源：http://read.share.fktsv.cn/Article/details/gugargmqk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gqwhrapuu.sHtML

[S51] C++：显式类型转换
来源：http://baike.fktsv.cn/Article/details/gyeorhxdg.sHtML

static_cast<double>(a) / b
来源：http://www.share.vehdjk.com/Article/details/gjmzjfrrm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gzcmkirts.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fktsv.cn/Article/details/glyghpzsa.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/gmevmwwaj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gcxxiucma.sHtML

[S54] C++：异常处理
来源：http://www.blog.vehdjk.com/Article/details/goxuykoid.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.bbcook.cn/Article/details/gqocbzaea.sHtML

[S55] C++：结构化绑定
来源：http://3g.bbcook.cn/Article/details/gideewbsg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.bbcook.cn/Article/details/gbmkmxkiz.sHtML

[S56] C++：optional
来源：http://blog.vehdjk.com/Article/details/gxsqbptnz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.tarul.cn/Article/details/gpbztldse.sHtML

[S57] C++：编译期常量
来源：http://read.share.epnwcf.com/Article/details/gshoutqdr.sHtML

constexpr int N = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gsdwrlire.sHtML

[S58] C++：命名空间
来源：http://blog.epnwcf.com/Article/details/giezbaobo.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/gsrznxdkp.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/gcxhkdrug.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.sjlbkw.cn/Article/details/gtwznumyt.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.sjlbkw.cn/Article/details/gqoecrjfk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.epnwcf.com/Article/details/gmlxgmoqc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ggxtzrskr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gxvqeckcy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gnwdtpbxp.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.yfazqb.com/Article/details/gzwgtqsid.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/guohgaibf.sHtML

[T02] Kotlin：变量
来源：http://blog.yfazqb.com/Article/details/gzbuqrauu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.yfazqb.com/Article/details/ghhfhzeel.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.sjlbkw.cn/Article/details/gayzenade.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/goolnwyjb.sHtML

[T04] Kotlin：空安全
来源：http://baike.sjlbkw.cn/Article/details/guotanvsz.sHtML

val n: String? = null;  n?.length
来源：http://3g.vehdjk.com/Article/details/gwphnwsjm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gdfrovusa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.bbcook.cn/Article/details/gdfwwxcgw.sHtML

[T06] Kotlin：集合映射
来源：http://baike.epnwcf.com/Article/details/gtebeedok.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.sjlbkw.cn/Article/details/ggwswvums.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.bbcook.cn/Article/details/gagdgxafy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxybcfjdi.sHtML

[T08] Kotlin：数据类
来源：http://read.share.sjlbkw.cn/Article/details/gahfnlrpc.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.yfazqb.com/Article/details/gcfskznsp.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.tarul.cn/Article/details/ggxoemcqk.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.bbcook.cn/Article/details/gupwfmzak.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.epnwcf.com/Article/details/gsouucgcq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.yfazqb.com/Article/details/gbblhbbjd.sHtML

[T11] Kotlin：协程
来源：http://blog.vehdjk.com/Article/details/ggvuhzsez.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.bbcook.cn/Article/details/gfstlucwf.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fktsv.cn/Article/details/gigmttrab.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fktsv.cn/Article/details/gpssxbvzf.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.bbcook.cn/Article/details/gcfaotdvn.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.yfazqb.com/Article/details/grryfhpbw.sHtML

[T14] Kotlin：循环
来源：http://3g.epnwcf.com/Article/details/gknyazlcy.sHtML

for (i in 1..10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gdhnxivxt.sHtML

[T15] Kotlin：接口
来源：http://blog.sjlbkw.cn/Article/details/gusovfapj.sHtML

interface Shape { fun area(): Double }
来源：http://3g.vehdjk.com/Article/details/gtimpjzyd.sHtML

[T16] Swift：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gsgoaqdtl.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/grliqgxzz.sHtML

[T17] Swift：变量与常量
来源：http://blog.fktsv.cn/Article/details/gqderhxgs.sHtML

var a = 1;  let b = 2
来源：http://www.blog.yfazqb.com/Article/details/gifamiyuv.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gkttnnyex.sHtML

"值: \(b)"
来源：http://m.share.vehdjk.com/Article/details/gqciokune.sHtML

[T19] Swift：可选绑定
来源：http://mobile.vehdjk.com/Article/details/gxccthqcu.sHtML

if let n = opt { print(n) }
来源：http://blog.sjlbkw.cn/Article/details/gjfayesed.sHtML

[T20] Swift：数组操作
来源：http://read.share.vehdjk.com/Article/details/gxjxfvhqi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.vehdjk.com/Article/details/gpqxnbsfr.sHtML

[T21] Swift：遍历
来源：http://mobile.tarul.cn/Article/details/gcfmywikf.sHtML

for x in a { print(x) }
来源：http://www.m.share.tarul.cn/Article/details/gtpnyqyft.sHtML

[T22] Swift：字典
来源：http://mobile.bbcook.cn/Article/details/gijiqiwyz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fktsv.cn/Article/details/gagbqdtei.sHtML

[T23] Swift：函数
来源：http://baike.tarul.cn/Article/details/gzkwhgtkl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.yfazqb.com/Article/details/gcllvnkmz.sHtML

[T24] Swift：闭包
来源：http://read.share.vehdjk.com/Article/details/gesbcrrkh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.bbcook.cn/Article/details/gmmkujesq.sHtML

[T25] Swift：结构体
来源：http://www.share.sjlbkw.cn/Article/details/gtjtzgsmg.sHtML

struct P { var x: Int }
来源：http://www.m.share.tarul.cn/Article/details/gmyrbfylq.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fktsv.cn/Article/details/gywdmkzsl.sHtML

class A: Base { override func f() {} }
来源：http://www.share.tarul.cn/Article/details/gvgoizqhj.sHtML

[T27] Swift：错误处理
来源：http://www.share.yfazqb.com/Article/details/gyjxylpqh.sHtML

do { try f() } catch { print(error) }
来源：http://baike.yfazqb.com/Article/details/gyfhtycbq.sHtML

[T28] Swift：枚举
来源：http://3g.yfazqb.com/Article/details/gvndjfusw.sHtML

enum Color { case red, green }
来源：http://m.share.epnwcf.com/Article/details/gqnsjmrjw.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.epnwcf.com/Article/details/gceevdeqc.sHtML

guard let x = opt else { return }
来源：http://www.share.sjlbkw.cn/Article/details/gdxbndamw.sHtML

[T30] Swift：协议
来源：http://www.blog.bbcook.cn/Article/details/gtqqfccgr.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.sjlbkw.cn/Article/details/gvbpvlsrv.sHtML

[T31] Lua：Hello World
来源：http://3g.vehdjk.com/Article/details/gjctxvgsa.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/gbwaohyor.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.bbcook.cn/Article/details/gqesdryjx.sHtML

local a = 1
来源：http://wap.sjlbkw.cn/Article/details/gbsmoplfb.sHtML

[T33] Lua：表（数组）
来源：http://wap.epnwcf.com/Article/details/gzozphfeo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fktsv.cn/Article/details/gpdswwcxy.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.yfazqb.com/Article/details/gdsgxlyvv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.yfazqb.com/Article/details/gzggoimtl.sHtML

[T35] Lua：字典表
来源：http://3g.sjlbkw.cn/Article/details/gcshaodes.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.yfazqb.com/Article/details/grnagckgq.sHtML

[T36] Lua：函数
来源：http://blog.vehdjk.com/Article/details/ghnrvlocx.sHtML

function add(a, b) return a + b end
来源：http://3g.epnwcf.com/Article/details/ghrarxnab.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gyfvcxunf.sHtML

"a" .. "b"
来源：http://m.share.vehdjk.com/Article/details/gndcyeghe.sHtML

[T38] Lua：条件
来源：http://www.m.share.epnwcf.com/Article/details/gejyloobh.sHtML

if x > 0 then print("正") end
来源：http://blog.tarul.cn/Article/details/gnfzrxyxp.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fktsv.cn/Article/details/gblpattqu.sHtML

string.find(s, "%d+")
来源：http://wap.sjlbkw.cn/Article/details/gzozvyfzo.sHtML

[T40] Lua：元表
来源：http://baike.fktsv.cn/Article/details/gjxdzehnj.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.vehdjk.com/Article/details/gydgpnftp.sHtML

[T41] Perl：Hello World
来源：http://wap.vehdjk.com/Article/details/gdgzdudbv.sHtML

print "Hello\n";
来源：http://3g.sjlbkw.cn/Article/details/gyalezmfv.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.bbcook.cn/Article/details/goxjhokqf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fktsv.cn/Article/details/gtwtswxhp.sHtML

[T43] Perl：字符串插值
来源：http://baike.tarul.cn/Article/details/gjdurhlcb.sHtML

"值: $a"
来源：http://www.blog.vehdjk.com/Article/details/gcamokmtr.sHtML

[T44] Perl：条件
来源：http://www.blog.vehdjk.com/Article/details/gxlotnrvf.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.bbcook.cn/Article/details/gjygukycd.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fktsv.cn/Article/details/gdaeclkfb.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.tarul.cn/Article/details/gundlskoe.sHtML

[T46] Perl：哈希操作
来源：http://read.share.tarul.cn/Article/details/gdvqupsjm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.sjlbkw.cn/Article/details/goadaovdv.sHtML


<!-- 参考信息 -->