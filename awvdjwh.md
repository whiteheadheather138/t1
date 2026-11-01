代发 wailian999

cmd > out.log 2>&1
来源：http://www.blog.bbcook.cn/Article/details/glazjqehc.sHtML

[R40] 追加写日志
来源：http://baike.yfazqb.com/Article/details/gxifjzvap.sHtML

echo "log" >> out.log
来源：http://m.share.yfazqb.com/Article/details/ghcmvtidc.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/gddoquifo.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.vehdjk.com/Article/details/gltzctddn.sHtML

[R42] 输入重定向
来源：http://baike.bbcook.cn/Article/details/gbfjydraw.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/ggmbglltp.sHtML

[R43] 按名字查找文件
来源：http://wap.yfazqb.com/Article/details/gmdsnftjf.sHtML

find . -name "*.log" -type f
来源：http://read.share.sjlbkw.cn/Article/details/ghwstmgcw.sHtML

[R44] 按修改时间查找
来源：http://m.share.vehdjk.com/Article/details/gcmdixstk.sHtML

find . -mtime -7 -type f
来源：http://www.share.tarul.cn/Article/details/gqwkkacjn.sHtML

[R45] 批量删除
来源：http://www.blog.vehdjk.com/Article/details/gkizlhzdd.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.yfazqb.com/Article/details/gmkahqmpq.sHtML

[R46] 递归替换文件内容
来源：http://3g.sjlbkw.cn/Article/details/gwiijkhow.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.sjlbkw.cn/Article/details/gzaklejer.sHtML

[R47] sed 单行替换
来源：http://mobile.yfazqb.com/Article/details/gnagpqnpy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.sjlbkw.cn/Article/details/giogsxazs.sHtML

[R48] awk 取指定列
来源：http://www.blog.vehdjk.com/Article/details/gdjsdzhqq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.tarul.cn/Article/details/gehepzhil.sHtML

[R49] awk 带条件
来源：http://m.share.tarul.cn/Article/details/gzmsmdujl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.epnwcf.com/Article/details/gekmcgioy.sHtML

[R50] awk 求和
来源：http://wap.bbcook.cn/Article/details/gaygrvpud.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gdsrmemfr.sHtML

[R51] 排序去重取前几
来源：http://mobile.fktsv.cn/Article/details/gzndwudzc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.bbcook.cn/Article/details/gtdlergvg.sHtML

[R52] 统计行数
来源：http://blog.tarul.cn/Article/details/ghuobpxpg.sHtML

wc -l a.txt
来源：http://read.share.fktsv.cn/Article/details/gjtymvntc.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.epnwcf.com/Article/details/giajthzug.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.yfazqb.com/Article/details/galeeetqb.sHtML

[R54] 比较两个文件
来源：http://wap.sjlbkw.cn/Article/details/globwttjx.sHtML

diff a.txt b.txt
来源：http://baike.fktsv.cn/Article/details/grhfcvmnw.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/gyaqidvgw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.bbcook.cn/Article/details/glqkdawug.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/gyjvcisgu.sHtML

scp file user@host:/path/
来源：http://wap.vehdjk.com/Article/details/gxdlyoqgw.sHtML

[R57] 远程执行命令
来源：http://www.blog.vehdjk.com/Article/details/ghbaimoyp.sHtML

ssh user@host 'uptime'
来源：http://m.share.sjlbkw.cn/Article/details/gfuxzhvhz.sHtML

[R58] 下载文件
来源：http://www.share.epnwcf.com/Article/details/gaxpvgrii.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.tarul.cn/Article/details/gznwuhvxj.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gdwpkjief.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.sjlbkw.cn/Article/details/gjrsxnpwg.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gvunjeojl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.epnwcf.com/Article/details/gmdlbcbwq.sHtML

[R61] 磁盘占用
来源：http://3g.epnwcf.com/Article/details/gameuorgo.sHtML

df -h;  du -sh *
来源：http://www.blog.fktsv.cn/Article/details/grhlkvgin.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqbrielm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.yfazqb.com/Article/details/gqurvjrlz.sHtML

[R63] 内存与进程
来源：http://mobile.bbcook.cn/Article/details/gmybpiqzh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.vehdjk.com/Article/details/glcjiznzz.sHtML

[R64] 结束进程
来源：http://blog.vehdjk.com/Article/details/gehqscfux.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.vehdjk.com/Article/details/geyhmkayh.sHtML

[R65] 查看端口占用
来源：http://www.m.share.tarul.cn/Article/details/gxgssitwt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.vehdjk.com/Article/details/gfsqqmzwh.sHtML

[R66] 定时任务
来源：http://blog.tarul.cn/Article/details/gbkhdquhz.sHtML

crontab -e;  crontab -l
来源：http://mobile.epnwcf.com/Article/details/govgfghma.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.vehdjk.com/Article/details/gzrexnduf.sHtML

openssl rand -hex 16
来源：http://www.share.vehdjk.com/Article/details/gmgemartx.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/grryfaqsx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.tarul.cn/Article/details/gzpkxatuk.sHtML

[R69] 生成随机密码
来源：http://www.share.tarul.cn/Article/details/gubxwhpbn.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/gojzhqoer.sHtML

[R70] 时间戳与互转
来源：http://www.blog.epnwcf.com/Article/details/gsnxdhfyh.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.sjlbkw.cn/Article/details/gpyshcuss.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gpgzcdpet.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.tarul.cn/Article/details/goqawepyp.sHtML

[R72] 等待端口就绪
来源：http://wap.epnwcf.com/Article/details/godqpdlhe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/grzpojsqw.sHtML

[R73] 分割大日志
来源：http://blog.fktsv.cn/Article/details/gfgjdsgmd.sHtML

split -l 1000 big.log part_
来源：http://www.blog.epnwcf.com/Article/details/gpuwvrbsn.sHtML

[R74] 批量重命名
来源：http://www.share.yfazqb.com/Article/details/gjmhbefas.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.epnwcf.com/Article/details/giwrbgerg.sHtML

[R75] 导出环境变量
来源：http://www.blog.epnwcf.com/Article/details/gfzgzltus.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.bbcook.cn/Article/details/gjrkixsag.sHtML

[R76] 使用临时文件
来源：http://read.share.tarul.cn/Article/details/gtewyycli.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjqalsxg.sHtML

[R77] 读取用户输入
来源：http://blog.epnwcf.com/Article/details/gdmsnzsij.sHtML

read -rp "请输入: " ans
来源：http://m.share.vehdjk.com/Article/details/gvwklmgok.sHtML

[R78] 交互式菜单
来源：http://blog.bbcook.cn/Article/details/gscapcpfp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.sjlbkw.cn/Article/details/gaxytangm.sHtML

[R79] 解析命令行选项
来源：http://3g.tarul.cn/Article/details/gmykgjnrq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.tarul.cn/Article/details/gzqrqksej.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvvmnsna.sHtML

time ./run.sh
来源：http://www.share.yfazqb.com/Article/details/gbruuxmch.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gnmamhnbh.sHtML

S. C / C++ 专题
来源：http://www.m.share.bbcook.cn/Article/details/gqlcxampu.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gogcnemlk.sHtML

[S01] C：Hello World
来源：http://www.blog.tarul.cn/Article/details/gsgglbfgp.sHtML

#include <stdio.h>
来源：http://blog.tarul.cn/Article/details/gjxrnvatj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gnpcnthcl.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.sjlbkw.cn/Article/details/ghlfodwuh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.epnwcf.com/Article/details/gekbwjkvz.sHtML

[S03] C：读入整数
来源：http://baike.bbcook.cn/Article/details/gxomphqwd.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fktsv.cn/Article/details/gpdjjjjnb.sHtML

[S04] C：字符串复制
来源：http://blog.sjlbkw.cn/Article/details/guqfzuhfy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.tarul.cn/Article/details/gokbndlnv.sHtML

[S05] C：字符串长度
来源：http://wap.bbcook.cn/Article/details/gtbimnsyw.sHtML

strlen(s)
来源：http://mobile.yfazqb.com/Article/details/gduwlqshk.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/grtwvmoqn.sHtML

strcmp(a, b) == 0
来源：http://read.share.epnwcf.com/Article/details/glkaarqon.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fktsv.cn/Article/details/gdctsmcfm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.epnwcf.com/Article/details/gxylrcman.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.epnwcf.com/Article/details/gxpkplplt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.vehdjk.com/Article/details/gjlqyirxl.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fktsv.cn/Article/details/gedbnxetf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.bbcook.cn/Article/details/glzetzggf.sHtML

[S10] C：指针与解引用
来源：http://3g.tarul.cn/Article/details/gjsqeiiiu.sHtML

int *p = &a;  *p = 5;
来源：http://3g.sjlbkw.cn/Article/details/gauwpqgmj.sHtML

[S11] C：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gftxkelyo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.yfazqb.com/Article/details/gvfnqdyso.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.epnwcf.com/Article/details/gkrmzutwv.sHtML

fclose(f);
来源：http://baike.yfazqb.com/Article/details/gkewvrebu.sHtML

[S12] C：写文件
来源：http://www.share.tarul.cn/Article/details/gnyderpdf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.yfazqb.com/Article/details/gwdqfhrnc.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/ggtwuwhyw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.yfazqb.com/Article/details/gkwvulytj.sHtML

[S14] C：枚举
来源：http://baike.epnwcf.com/Article/details/gozuulfvu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/gwwsraxgp.sHtML

[S15] C：类型转换
来源：http://wap.fktsv.cn/Article/details/gqrcpfnxg.sHtML

(double) a / b
来源：http://blog.bbcook.cn/Article/details/gkwadsurz.sHtML

[S16] C：位操作置位
来源：http://wap.tarul.cn/Article/details/gbjdhzfmk.sHtML

x |= (1 << 3);
来源：http://3g.sjlbkw.cn/Article/details/guzibhgal.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fktsv.cn/Article/details/gjmaairdz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.vehdjk.com/Article/details/grhgqexjg.sHtML

[S18] C：命令行参数
来源：http://read.share.epnwcf.com/Article/details/gvmbihjih.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.yfazqb.com/Article/details/gvcolvuem.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/ghcvanvji.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gjiqecbpm.sHtML

[S20] C：二分查找
来源：http://baike.vehdjk.com/Article/details/gjylhkzpq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/gfnajtjav.sHtML

[S21] C：字符类别判断
来源：http://3g.tarul.cn/Article/details/gxwzjkmpc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.vehdjk.com/Article/details/grhwqugtg.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/gohmljtah.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fktsv.cn/Article/details/gvwhygwaj.sHtML

[S23] C：随机数
来源：http://baike.yfazqb.com/Article/details/gfkjckxlf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.bbcook.cn/Article/details/gzzcgiikg.sHtML

[S24] C：获取本地时间
来源：http://www.blog.bbcook.cn/Article/details/ghuqawkjs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.epnwcf.com/Article/details/gqmduiusp.sHtML

[S25] C：内存拷贝
来源：http://read.share.bbcook.cn/Article/details/goeqrfhxl.sHtML

memcpy(dst, src, n);
来源：http://read.share.vehdjk.com/Article/details/gcsdcnehq.sHtML

[S26] C：内存清零
来源：http://3g.fktsv.cn/Article/details/gbkoutwvh.sHtML

memset(a, 0, sizeof a);
来源：http://baike.tarul.cn/Article/details/gyvttsuhs.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gzrxdgksa.sHtML

const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gzhkaiill.sHtML

[S28] C：静态变量
来源：http://m.share.sjlbkw.cn/Article/details/ggxbfxvgg.sHtML

static int counter = 0;
来源：http://www.share.yfazqb.com/Article/details/ghnwxjaaw.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/gqahccoug.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.epnwcf.com/Article/details/gacxohftz.sHtML

[S30] C：头文件保护
来源：http://mobile.fktsv.cn/Article/details/gxqngbxjr.sHtML

#ifndef X_H
来源：http://wap.vehdjk.com/Article/details/gwvzilkee.sHtML

#define X_H
来源：http://blog.fktsv.cn/Article/details/geauzvlqw.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gycxicgcr.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/gkmhinvad.sHtML

#include <iostream>
来源：http://m.share.sjlbkw.cn/Article/details/gksrezxrh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.epnwcf.com/Article/details/gsfwqtnzd.sHtML

[S32] C++：字符串
来源：http://read.share.bbcook.cn/Article/details/grdcgkukb.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.epnwcf.com/Article/details/gusxkzxvd.sHtML

[S33] C++：vector 增删
来源：http://blog.tarul.cn/Article/details/grulxkkwr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.tarul.cn/Article/details/ggguolift.sHtML

[S34] C++：遍历 vector
来源：http://wap.epnwcf.com/Article/details/gfzdkxamq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/geqwdknsa.sHtML

[S35] C++：map
来源：http://wap.epnwcf.com/Article/details/ggndqajhv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/ghdupuwru.sHtML

[S36] C++：unordered_map
来源：http://3g.bbcook.cn/Article/details/gnbhiqgji.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gehhepeiy.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/gsnxlajhr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/gfmkmhwjd.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gpyslsahw.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gugahtlvy.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.epnwcf.com/Article/details/gktoiponj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/gcwjudhfr.sHtML

[S40] C++：查找元素
来源：http://read.share.fktsv.cn/Article/details/gsfoknxrl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.epnwcf.com/Article/details/gklaogznm.sHtML

[S41] C++：类与构造函数
来源：http://3g.fktsv.cn/Article/details/gdakfcxmd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.yfazqb.com/Article/details/gzkqpsecc.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.vehdjk.com/Article/details/gebjoqibf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.tarul.cn/Article/details/gzcbakced.sHtML

[S43] C++：智能指针
来源：http://wap.yfazqb.com/Article/details/girpdrrhn.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.vehdjk.com/Article/details/gkpntxcfq.sHtML

[S44] C++：引用传参
来源：http://www.share.tarul.cn/Article/details/gworxnoox.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gsdowtlhm.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/geahgsmqc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.epnwcf.com/Article/details/gvviphnzx.sHtML

[S46] C++：函数模板
来源：http://www.share.tarul.cn/Article/details/gyfnsgdfj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.tarul.cn/Article/details/guouwanaj.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.tarul.cn/Article/details/gcndhhrtb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.tarul.cn/Article/details/gczgqidco.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gjbnudbxo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.vehdjk.com/Article/details/gudwsnfvg.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.yfazqb.com/Article/details/gfscficbg.sHtML

[S49] C++：写文件
来源：http://3g.vehdjk.com/Article/details/gfboajoro.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.tarul.cn/Article/details/gvynkhmoz.sHtML

[S50] C++：格式化数字
来源：http://3g.sjlbkw.cn/Article/details/gejahlphy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gvwpqpoth.sHtML

[S51] C++：显式类型转换
来源：http://www.share.sjlbkw.cn/Article/details/gympasukx.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.vehdjk.com/Article/details/grertpzpp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gqducgtyk.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fktsv.cn/Article/details/gviemlbsj.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/gekywtbzc.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.epnwcf.com/Article/details/gelwdksre.sHtML

[S54] C++：异常处理
来源：http://wap.yfazqb.com/Article/details/gvmqxgrgk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.vehdjk.com/Article/details/goimttpso.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.bbcook.cn/Article/details/gzppfqmpn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fktsv.cn/Article/details/gskeglkfn.sHtML

[S56] C++：optional
来源：http://baike.bbcook.cn/Article/details/gcmmlyrjb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/gmjcbkacg.sHtML

[S57] C++：编译期常量
来源：http://www.share.bbcook.cn/Article/details/gzxnmokgy.sHtML

constexpr int N = 10;
来源：http://www.blog.fktsv.cn/Article/details/gmgqgdmux.sHtML

[S58] C++：命名空间
来源：http://read.share.sjlbkw.cn/Article/details/grdiyjjbw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.tarul.cn/Article/details/gnduuvgrd.sHtML

[S59] C++：静态断言
来源：http://read.share.bbcook.cn/Article/details/grhxdkero.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.epnwcf.com/Article/details/ggaecnizn.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.bbcook.cn/Article/details/gncxrnlcl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.bbcook.cn/Article/details/gglxjfpiy.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzznyxjzi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.vehdjk.com/Article/details/geivtwmar.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gyxxfiisa.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.yfazqb.com/Article/details/gryhvxlxo.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gfpwfnujh.sHtML

[T02] Kotlin：变量
来源：http://read.share.bbcook.cn/Article/details/gqmxzsyfv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.vehdjk.com/Article/details/gnuggrmyi.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.vehdjk.com/Article/details/gjokfhieg.sHtML

"值: $b"
来源：http://m.share.yfazqb.com/Article/details/gcnhllhdw.sHtML

[T04] Kotlin：空安全
来源：http://baike.vehdjk.com/Article/details/gqxnkyrpk.sHtML

val n: String? = null;  n?.length
来源：http://read.share.sjlbkw.cn/Article/details/giulcffzf.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gpagcxlqv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.sjlbkw.cn/Article/details/gtkictaiq.sHtML

[T06] Kotlin：集合映射
来源：http://baike.epnwcf.com/Article/details/glaiyrhod.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.epnwcf.com/Article/details/ggyyvjsrz.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.tarul.cn/Article/details/gknbdxqql.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.bbcook.cn/Article/details/glkdzggil.sHtML

[T08] Kotlin：数据类
来源：http://mobile.bbcook.cn/Article/details/gdkhvqmvn.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/grxkszzwt.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.epnwcf.com/Article/details/gcnupcojx.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/gjikdtgej.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fktsv.cn/Article/details/gbczjwhhi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gueiqyuof.sHtML

[T11] Kotlin：协程
来源：http://baike.bbcook.cn/Article/details/grehwwjzs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fktsv.cn/Article/details/gzaroteej.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fktsv.cn/Article/details/glpqovfug.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gmewfmims.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.bbcook.cn/Article/details/gtkpecmtc.sHtML

val m = mapOf("a" to 1)
来源：http://wap.yfazqb.com/Article/details/gzepyymjj.sHtML

[T14] Kotlin：循环
来源：http://baike.yfazqb.com/Article/details/gefqvldwv.sHtML

for (i in 1..10) println(i)
来源：http://wap.epnwcf.com/Article/details/gntmhvqsn.sHtML

[T15] Kotlin：接口
来源：http://3g.fktsv.cn/Article/details/gjqdmiufu.sHtML

interface Shape { fun area(): Double }
来源：http://blog.vehdjk.com/Article/details/gbyvuwvhj.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/gxdttuxjv.sHtML

print("Hello")
来源：http://blog.epnwcf.com/Article/details/ghzgwhufw.sHtML

[T17] Swift：变量与常量
来源：http://m.share.bbcook.cn/Article/details/gemtardla.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/govackzbn.sHtML

[T18] Swift：字符串插值
来源：http://wap.epnwcf.com/Article/details/gjqwsxwdg.sHtML

"值: \(b)"
来源：http://3g.tarul.cn/Article/details/gcsidzjse.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/ggababkeh.sHtML

if let n = opt { print(n) }
来源：http://wap.tarul.cn/Article/details/gyrspznxk.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/gzynihtsp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.yfazqb.com/Article/details/gxxbvxrep.sHtML

[T21] Swift：遍历
来源：http://mobile.epnwcf.com/Article/details/gfjpomqrq.sHtML

for x in a { print(x) }
来源：http://blog.vehdjk.com/Article/details/gyeefkhwj.sHtML

[T22] Swift：字典
来源：http://wap.vehdjk.com/Article/details/gfhcceciu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fktsv.cn/Article/details/gvilbxtnd.sHtML

[T23] Swift：函数
来源：http://blog.tarul.cn/Article/details/gnnsxxkoq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.tarul.cn/Article/details/gufknsxle.sHtML

[T24] Swift：闭包
来源：http://wap.yfazqb.com/Article/details/ghthllxjl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.epnwcf.com/Article/details/guwbvyuur.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fktsv.cn/Article/details/gfegfvbve.sHtML

struct P { var x: Int }
来源：http://baike.sjlbkw.cn/Article/details/gapjgzovi.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/geobwnsnq.sHtML

class A: Base { override func f() {} }
来源：http://blog.yfazqb.com/Article/details/gqkwxhfzj.sHtML

[T27] Swift：错误处理
来源：http://baike.yfazqb.com/Article/details/gbajsexni.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.tarul.cn/Article/details/gboxwqpdw.sHtML

[T28] Swift：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gvvbcsgsv.sHtML

enum Color { case red, green }
来源：http://www.blog.epnwcf.com/Article/details/gvhlddcrd.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.tarul.cn/Article/details/gqtizlkgo.sHtML

guard let x = opt else { return }
来源：http://baike.bbcook.cn/Article/details/glexrxwtt.sHtML

[T30] Swift：协议
来源：http://www.blog.epnwcf.com/Article/details/geeufchhm.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fktsv.cn/Article/details/glegorzqb.sHtML

[T31] Lua：Hello World
来源：http://blog.yfazqb.com/Article/details/gweihhqro.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/goiviasow.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fktsv.cn/Article/details/gmgpumifa.sHtML

local a = 1
来源：http://blog.bbcook.cn/Article/details/gmyflufgb.sHtML

[T33] Lua：表（数组）
来源：http://www.share.vehdjk.com/Article/details/gcljoetrk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.tarul.cn/Article/details/gkqcbggic.sHtML

[T34] Lua：遍历表
来源：http://wap.tarul.cn/Article/details/gnsizflph.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.tarul.cn/Article/details/ghavrvjsg.sHtML

[T35] Lua：字典表
来源：http://baike.sjlbkw.cn/Article/details/gqpvpeedk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.yfazqb.com/Article/details/gtcrnctil.sHtML

[T36] Lua：函数
来源：http://3g.epnwcf.com/Article/details/gywynrxai.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/gwxudcgkp.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gparyszdr.sHtML

"a" .. "b"
来源：http://wap.epnwcf.com/Article/details/ghilajbdt.sHtML

[T38] Lua：条件
来源：http://baike.tarul.cn/Article/details/gtkvvdzpx.sHtML

if x > 0 then print("正") end
来源：http://3g.yfazqb.com/Article/details/gkqekrblb.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/gzpcgtxqs.sHtML

string.find(s, "%d+")
来源：http://baike.vehdjk.com/Article/details/gseqpkwgo.sHtML

[T40] Lua：元表
来源：http://3g.sjlbkw.cn/Article/details/gwhidmwls.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.epnwcf.com/Article/details/gdnddwbxu.sHtML

[T41] Perl：Hello World
来源：http://blog.vehdjk.com/Article/details/ghpgzmepc.sHtML

print "Hello\n";
来源：http://m.share.vehdjk.com/Article/details/giqherggu.sHtML

[T42] Perl：变量类型
来源：http://m.share.yfazqb.com/Article/details/gayxrlccm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.bbcook.cn/Article/details/gvvblrixb.sHtML


<!-- 参考信息 -->