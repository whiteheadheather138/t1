代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gypqrymvd.sHtML

[R42] 输入重定向
来源：http://blog.yfazqb.com/Article/details/grnyqzvcx.sHtML

wc -l < a.txt
来源：http://www.share.vehdjk.com/Article/details/grcoeeeup.sHtML

[R43] 按名字查找文件
来源：http://www.blog.yfazqb.com/Article/details/gecvgqrbb.sHtML

find . -name "*.log" -type f
来源：http://read.share.bbcook.cn/Article/details/gmijluhky.sHtML

[R44] 按修改时间查找
来源：http://read.share.fktsv.cn/Article/details/gbdzrhawj.sHtML

find . -mtime -7 -type f
来源：http://www.share.fktsv.cn/Article/details/gmnuwgxjo.sHtML

[R45] 批量删除
来源：http://www.blog.tarul.cn/Article/details/gbvtpwrny.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.yfazqb.com/Article/details/goryozpok.sHtML

[R46] 递归替换文件内容
来源：http://www.share.bbcook.cn/Article/details/gujfredrm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.tarul.cn/Article/details/gvohzkxwe.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/gyjcmgwcj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.vehdjk.com/Article/details/guetdaxey.sHtML

[R48] awk 取指定列
来源：http://read.share.vehdjk.com/Article/details/ggcefqfte.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.yfazqb.com/Article/details/gvclsvrho.sHtML

[R49] awk 带条件
来源：http://mobile.epnwcf.com/Article/details/glowayyxf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.sjlbkw.cn/Article/details/gypwehnke.sHtML

[R50] awk 求和
来源：http://3g.sjlbkw.cn/Article/details/goruiofqe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fktsv.cn/Article/details/gvdghllgz.sHtML

[R51] 排序去重取前几
来源：http://3g.sjlbkw.cn/Article/details/gomfskxxl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.yfazqb.com/Article/details/gwqwhtymd.sHtML

[R52] 统计行数
来源：http://m.share.fktsv.cn/Article/details/gfofdnxnl.sHtML

wc -l a.txt
来源：http://baike.bbcook.cn/Article/details/gtwjehfsd.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fktsv.cn/Article/details/gftarwwbq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.bbcook.cn/Article/details/gmjbltuty.sHtML

[R54] 比较两个文件
来源：http://www.m.share.vehdjk.com/Article/details/gtuwljlyz.sHtML

diff a.txt b.txt
来源：http://3g.yfazqb.com/Article/details/grzzmqnrd.sHtML

[R55] 压缩与解压
来源：http://www.m.share.yfazqb.com/Article/details/ghixblist.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fktsv.cn/Article/details/gjfdmfifd.sHtML

[R56] 远程拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gzkfraxdn.sHtML

scp file user@host:/path/
来源：http://www.m.share.tarul.cn/Article/details/gtxgyxqlt.sHtML

[R57] 远程执行命令
来源：http://blog.tarul.cn/Article/details/gtrbyjqne.sHtML

ssh user@host 'uptime'
来源：http://mobile.epnwcf.com/Article/details/gxogadhhc.sHtML

[R58] 下载文件
来源：http://www.share.vehdjk.com/Article/details/gpgkuogxm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.vehdjk.com/Article/details/gazdrudfi.sHtML

[R59] 发 POST JSON
来源：http://wap.bbcook.cn/Article/details/gmrozurgf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.epnwcf.com/Article/details/ghqwxgxmx.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gquuqtefu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.sjlbkw.cn/Article/details/ghmqurhwa.sHtML

[R61] 磁盘占用
来源：http://3g.yfazqb.com/Article/details/gdrydqqbu.sHtML

df -h;  du -sh *
来源：http://m.share.yfazqb.com/Article/details/gfeptkbns.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.tarul.cn/Article/details/ggqecwomd.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.yfazqb.com/Article/details/gcywyqsjn.sHtML

[R63] 内存与进程
来源：http://www.share.sjlbkw.cn/Article/details/ghbjjscdr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fktsv.cn/Article/details/gsgykzsle.sHtML

[R64] 结束进程
来源：http://www.blog.yfazqb.com/Article/details/gyztocoho.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fktsv.cn/Article/details/gktvmhxqf.sHtML

[R65] 查看端口占用
来源：http://baike.fktsv.cn/Article/details/gmcwinylq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fktsv.cn/Article/details/gdeutalws.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/grutilesw.sHtML

crontab -e;  crontab -l
来源：http://m.share.bbcook.cn/Article/details/gfwctgqat.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/gpqcczcqi.sHtML

openssl rand -hex 16
来源：http://read.share.vehdjk.com/Article/details/gvhzlzzlv.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/gqtczfytw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.bbcook.cn/Article/details/gkafasxzc.sHtML

[R69] 生成随机密码
来源：http://www.blog.vehdjk.com/Article/details/gupeipdwq.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.vehdjk.com/Article/details/gdepvadse.sHtML

[R70] 时间戳与互转
来源：http://www.blog.tarul.cn/Article/details/glnrxetjl.sHtML

date +%s;  date -d @1700000000
来源：http://3g.vehdjk.com/Article/details/gxtrcujsa.sHtML

[R71] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/guzzglirf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fktsv.cn/Article/details/gcxqgygcn.sHtML

[R72] 等待端口就绪
来源：http://www.blog.vehdjk.com/Article/details/gezejsezq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/ghckijsgh.sHtML

[R73] 分割大日志
来源：http://www.blog.tarul.cn/Article/details/gffkfmaat.sHtML

split -l 1000 big.log part_
来源：http://www.share.tarul.cn/Article/details/gqncsumay.sHtML

[R74] 批量重命名
来源：http://read.share.fktsv.cn/Article/details/gietmhwmo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.bbcook.cn/Article/details/gkcdxfnss.sHtML

[R75] 导出环境变量
来源：http://3g.sjlbkw.cn/Article/details/ggtvqpyde.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.yfazqb.com/Article/details/gaglvknjr.sHtML

[R76] 使用临时文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gugjcbwhk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/gtersryqp.sHtML

[R77] 读取用户输入
来源：http://mobile.tarul.cn/Article/details/geyzxucgm.sHtML

read -rp "请输入: " ans
来源：http://www.share.sjlbkw.cn/Article/details/gqherlngi.sHtML

[R78] 交互式菜单
来源：http://blog.sjlbkw.cn/Article/details/gwmogszde.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.tarul.cn/Article/details/gbxbmldei.sHtML

[R79] 解析命令行选项
来源：http://m.share.sjlbkw.cn/Article/details/gqpcvqfgp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.sjlbkw.cn/Article/details/grxilgsrl.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.sjlbkw.cn/Article/details/geqescthc.sHtML

time ./run.sh
来源：http://mobile.epnwcf.com/Article/details/gvpvkkhol.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gpnlecisd.sHtML

S. C / C++ 专题
来源：http://blog.yfazqb.com/Article/details/giuscpgcp.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gzvyyfiju.sHtML

[S01] C：Hello World
来源：http://mobile.epnwcf.com/Article/details/ggdbcbecj.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/gfklojeau.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.yfazqb.com/Article/details/ghnyckdwj.sHtML

[S02] C：变量与格式化输出
来源：http://3g.epnwcf.com/Article/details/geoceofsv.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.yfazqb.com/Article/details/gwgylwjuy.sHtML

[S03] C：读入整数
来源：http://blog.vehdjk.com/Article/details/gchxatvhi.sHtML

int x; scanf("%d", &x);
来源：http://www.share.tarul.cn/Article/details/gydmogssd.sHtML

[S04] C：字符串复制
来源：http://baike.tarul.cn/Article/details/gtvaubzem.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.tarul.cn/Article/details/ggcsyshtp.sHtML

[S05] C：字符串长度
来源：http://3g.fktsv.cn/Article/details/gozdhpjtv.sHtML

strlen(s)
来源：http://m.share.sjlbkw.cn/Article/details/glidpreah.sHtML

[S06] C：字符串比较
来源：http://3g.sjlbkw.cn/Article/details/grhekvgoi.sHtML

strcmp(a, b) == 0
来源：http://baike.vehdjk.com/Article/details/gbhgsruui.sHtML

[S07] C：数组遍历求和
来源：http://baike.sjlbkw.cn/Article/details/gtjnbmcfr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fktsv.cn/Article/details/gnabvnilj.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.yfazqb.com/Article/details/gdolovlmo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fktsv.cn/Article/details/gdppancia.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/grkpgkyqw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.epnwcf.com/Article/details/gogbtiqdz.sHtML

[S10] C：指针与解引用
来源：http://mobile.epnwcf.com/Article/details/gfcngsgcu.sHtML

int *p = &a;  *p = 5;
来源：http://wap.yfazqb.com/Article/details/gznnbtesf.sHtML

[S11] C：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/giqmundvz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.vehdjk.com/Article/details/gmzdjrygv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.yfazqb.com/Article/details/gopqucvtg.sHtML

fclose(f);
来源：http://m.share.epnwcf.com/Article/details/gkwrvojmw.sHtML

[S12] C：写文件
来源：http://wap.sjlbkw.cn/Article/details/gpmqntgwk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gnkuglckw.sHtML

[S13] C：宏定义
来源：http://3g.fktsv.cn/Article/details/gbvjyxcnp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.yfazqb.com/Article/details/gvacxvavn.sHtML

[S14] C：枚举
来源：http://wap.tarul.cn/Article/details/gveseuidb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/ggwolpfrm.sHtML

[S15] C：类型转换
来源：http://m.share.epnwcf.com/Article/details/giroctjrp.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gcupgxmzv.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fktsv.cn/Article/details/gpnhrarez.sHtML

x |= (1 << 3);
来源：http://3g.vehdjk.com/Article/details/gzijrzqoc.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/geasbugtv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/gckopwskg.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/gabhcdhkk.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/gylwoaora.sHtML

[S19] C：快速排序
来源：http://www.blog.epnwcf.com/Article/details/gpblagruo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/gobwvprrh.sHtML

[S20] C：二分查找
来源：http://read.share.fktsv.cn/Article/details/gvbdbobub.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/gymccqpis.sHtML

[S21] C：字符类别判断
来源：http://m.share.tarul.cn/Article/details/gmczjmchd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.epnwcf.com/Article/details/gptvkffee.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/gxaifcqcc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.bbcook.cn/Article/details/grfhcqhwd.sHtML

[S23] C：随机数
来源：http://3g.epnwcf.com/Article/details/gtpakdkyh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.epnwcf.com/Article/details/gpmlouqrr.sHtML

[S24] C：获取本地时间
来源：http://www.blog.bbcook.cn/Article/details/goeonauge.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.vehdjk.com/Article/details/gjcvopyux.sHtML

[S25] C：内存拷贝
来源：http://3g.yfazqb.com/Article/details/giujbrtxj.sHtML

memcpy(dst, src, n);
来源：http://blog.fktsv.cn/Article/details/gwyemixfb.sHtML

[S26] C：内存清零
来源：http://mobile.sjlbkw.cn/Article/details/gxatunfef.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.epnwcf.com/Article/details/gcaxqyapd.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/glxzpfdzm.sHtML

const double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gjnajfohr.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/gybkaxldy.sHtML

static int counter = 0;
来源：http://www.m.share.fktsv.cn/Article/details/ghaxyedvc.sHtML

[S29] C：变参函数
来源：http://www.share.fktsv.cn/Article/details/gcyemsner.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.yfazqb.com/Article/details/gzhrjdsti.sHtML

[S30] C：头文件保护
来源：http://www.share.yfazqb.com/Article/details/gpaplnmct.sHtML

#ifndef X_H
来源：http://m.share.fktsv.cn/Article/details/gwvhsviav.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/gsylaherd.sHtML

#endif
来源：http://blog.bbcook.cn/Article/details/gumpbhsny.sHtML

[S31] C++：Hello World
来源：http://wap.tarul.cn/Article/details/gcvyfqige.sHtML

#include <iostream>
来源：http://baike.yfazqb.com/Article/details/gxmlfrasv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.tarul.cn/Article/details/gmnvbedhq.sHtML

[S32] C++：字符串
来源：http://blog.tarul.cn/Article/details/gwwgbfbxs.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.yfazqb.com/Article/details/gvkphtszk.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/gwhtqtoyc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.yfazqb.com/Article/details/guqvdfmdp.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/gwyvbcnwd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.yfazqb.com/Article/details/gmkvbvxxu.sHtML

[S35] C++：map
来源：http://www.share.sjlbkw.cn/Article/details/gwpgpyzig.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gzwyqjtbn.sHtML

[S36] C++：unordered_map
来源：http://www.share.bbcook.cn/Article/details/gqlziqcaq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gbxixlrcu.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/gimeknkzf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.bbcook.cn/Article/details/gfzghqqsz.sHtML

[S38] C++：排序
来源：http://www.share.tarul.cn/Article/details/gtrtfbllp.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.epnwcf.com/Article/details/gznxjyevj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.epnwcf.com/Article/details/grijpkblg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.epnwcf.com/Article/details/gsgrzdplv.sHtML

[S40] C++：查找元素
来源：http://mobile.yfazqb.com/Article/details/gtrcibjfg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.vehdjk.com/Article/details/gzzjukekx.sHtML

[S41] C++：类与构造函数
来源：http://read.share.tarul.cn/Article/details/gqwqgtqet.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.sjlbkw.cn/Article/details/gjjuipygk.sHtML

[S42] C++：继承与虚函数
来源：http://blog.vehdjk.com/Article/details/gvtuhgoxx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gcviyhjqf.sHtML

[S43] C++：智能指针
来源：http://wap.yfazqb.com/Article/details/gxmvpwscg.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.vehdjk.com/Article/details/gykthcqpd.sHtML

[S44] C++：引用传参
来源：http://baike.fktsv.cn/Article/details/gdtbeszyi.sHtML

void inc(int &x) { ++x; }
来源：http://blog.sjlbkw.cn/Article/details/gxuiswepn.sHtML

[S45] C++：lambda
来源：http://read.share.vehdjk.com/Article/details/gpihvxdia.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.vehdjk.com/Article/details/gabhhbuin.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/gyfrfbuff.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.vehdjk.com/Article/details/gdxhfjvsv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.epnwcf.com/Article/details/guguzueht.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grfhcxwls.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gfxusptmi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.vehdjk.com/Article/details/gojpzorqr.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.vehdjk.com/Article/details/glvmascjd.sHtML

[S49] C++：写文件
来源：http://www.share.fktsv.cn/Article/details/gavuyjaqb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.vehdjk.com/Article/details/gpclrrigp.sHtML

[S50] C++：格式化数字
来源：http://m.share.yfazqb.com/Article/details/gtvbkkhml.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gliorzdeh.sHtML

[S51] C++：显式类型转换
来源：http://mobile.yfazqb.com/Article/details/gnvmnvyud.sHtML

static_cast<double>(a) / b
来源：http://3g.vehdjk.com/Article/details/gktymlfuu.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.vehdjk.com/Article/details/glgprkxof.sHtML

int size() const noexcept { return n_; }
来源：http://blog.bbcook.cn/Article/details/gnfmfuosg.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/gmbuwgxwi.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fktsv.cn/Article/details/geuznrjfa.sHtML

[S54] C++：异常处理
来源：http://www.blog.sjlbkw.cn/Article/details/gpcqpiaid.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpafgnhd.sHtML

[S55] C++：结构化绑定
来源：http://m.share.sjlbkw.cn/Article/details/gombclglv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.epnwcf.com/Article/details/ghciytygy.sHtML

[S56] C++：optional
来源：http://3g.sjlbkw.cn/Article/details/gorfzhnbb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fktsv.cn/Article/details/gldinrmes.sHtML

[S57] C++：编译期常量
来源：http://m.share.sjlbkw.cn/Article/details/gmstkhhjt.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggibkulgt.sHtML

[S58] C++：命名空间
来源：http://mobile.vehdjk.com/Article/details/guhxscpzb.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.tarul.cn/Article/details/grcgrdqqa.sHtML

[S59] C++：静态断言
来源：http://www.m.share.yfazqb.com/Article/details/gpdyismwm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.vehdjk.com/Article/details/gftuobaeo.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.yfazqb.com/Article/details/gfphyhobc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.epnwcf.com/Article/details/gunhnxcqq.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gndstirhy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.bbcook.cn/Article/details/gwhqwmicu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gpylptquc.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fktsv.cn/Article/details/gymisirwq.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gvcdvcdjx.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.vehdjk.com/Article/details/gqoewwoaw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.bbcook.cn/Article/details/gyxyvweuo.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.tarul.cn/Article/details/gvgfiqtge.sHtML

"值: $b"
来源：http://blog.vehdjk.com/Article/details/gioszcjlp.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.epnwcf.com/Article/details/gvmjyiqej.sHtML

val n: String? = null;  n?.length
来源：http://www.share.yfazqb.com/Article/details/glglbfras.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.epnwcf.com/Article/details/gqndtmghs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.bbcook.cn/Article/details/gonjvkfgu.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.tarul.cn/Article/details/gjtvcvgqu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.epnwcf.com/Article/details/gsauyvtjm.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gwxnwfrwt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fktsv.cn/Article/details/guwsqbfeb.sHtML

[T08] Kotlin：数据类
来源：http://www.share.bbcook.cn/Article/details/glmgkojou.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.vehdjk.com/Article/details/gznssjxkh.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.sjlbkw.cn/Article/details/gtfkhrhel.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.vehdjk.com/Article/details/gelyyatea.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.vehdjk.com/Article/details/gvfadzrtg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.tarul.cn/Article/details/ghhmvumzt.sHtML

[T11] Kotlin：协程
来源：http://www.share.tarul.cn/Article/details/gxpitaadm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.vehdjk.com/Article/details/geawllkhe.sHtML

[T12] Kotlin：解构声明
来源：http://blog.tarul.cn/Article/details/gmomvbzfo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gpcrpuvxb.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.sjlbkw.cn/Article/details/gownpuxod.sHtML

val m = mapOf("a" to 1)
来源：http://baike.vehdjk.com/Article/details/gcgczdtnb.sHtML

[T14] Kotlin：循环
来源：http://www.share.sjlbkw.cn/Article/details/gdkshomuq.sHtML

for (i in 1..10) println(i)
来源：http://blog.bbcook.cn/Article/details/gbpyajjpx.sHtML

[T15] Kotlin：接口
来源：http://www.blog.epnwcf.com/Article/details/gtrkofjwk.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.yfazqb.com/Article/details/gggasqlxn.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/gvgdvkvys.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gguesnicu.sHtML

[T17] Swift：变量与常量
来源：http://3g.sjlbkw.cn/Article/details/gjlacxekx.sHtML

var a = 1;  let b = 2
来源：http://www.share.tarul.cn/Article/details/gxosjtffu.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gzkjfvwaf.sHtML

"值: \(b)"
来源：http://wap.vehdjk.com/Article/details/glejepmef.sHtML

[T19] Swift：可选绑定
来源：http://baike.sjlbkw.cn/Article/details/gzrnktzhz.sHtML

if let n = opt { print(n) }
来源：http://read.share.tarul.cn/Article/details/ghowcxhyl.sHtML

[T20] Swift：数组操作
来源：http://3g.sjlbkw.cn/Article/details/gnudluwbp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fktsv.cn/Article/details/gzqkftomw.sHtML

[T21] Swift：遍历
来源：http://blog.bbcook.cn/Article/details/gawzfxqql.sHtML

for x in a { print(x) }
来源：http://read.share.bbcook.cn/Article/details/giksjsail.sHtML

[T22] Swift：字典
来源：http://3g.vehdjk.com/Article/details/gsrubhiqs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.vehdjk.com/Article/details/glrjqzgtl.sHtML

[T23] Swift：函数
来源：http://read.share.fktsv.cn/Article/details/gojdwhuie.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fktsv.cn/Article/details/gimzismla.sHtML

[T24] Swift：闭包
来源：http://3g.sjlbkw.cn/Article/details/grcvbwccv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.vehdjk.com/Article/details/gojcpfyyp.sHtML

[T25] Swift：结构体
来源：http://m.share.yfazqb.com/Article/details/glcjtmsrr.sHtML

struct P { var x: Int }
来源：http://blog.sjlbkw.cn/Article/details/gzfuhdomv.sHtML

[T26] Swift：类与重写
来源：http://www.blog.epnwcf.com/Article/details/gvbkkqprb.sHtML

class A: Base { override func f() {} }
来源：http://mobile.epnwcf.com/Article/details/glhrprmqg.sHtML

[T27] Swift：错误处理
来源：http://www.blog.bbcook.cn/Article/details/gpwzuqcss.sHtML

do { try f() } catch { print(error) }
来源：http://3g.vehdjk.com/Article/details/gobjedrjg.sHtML

[T28] Swift：枚举
来源：http://read.share.epnwcf.com/Article/details/gjjfsstzj.sHtML

enum Color { case red, green }
来源：http://www.share.yfazqb.com/Article/details/grvmjdtpj.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.sjlbkw.cn/Article/details/gxqufjhsl.sHtML

guard let x = opt else { return }
来源：http://www.m.share.tarul.cn/Article/details/gcgzojvls.sHtML

[T30] Swift：协议
来源：http://wap.vehdjk.com/Article/details/glvwgwofm.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.bbcook.cn/Article/details/gxpcwyuax.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gfhrrrjgm.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/goikuqdvs.sHtML

[T32] Lua：局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gdxbvapdt.sHtML

local a = 1
来源：http://read.share.vehdjk.com/Article/details/gdmhbvoes.sHtML

[T33] Lua：表（数组）
来源：http://blog.yfazqb.com/Article/details/gnufzcnwf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.epnwcf.com/Article/details/gfhuzmoia.sHtML

[T34] Lua：遍历表
来源：http://baike.epnwcf.com/Article/details/gshnqurqu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.sjlbkw.cn/Article/details/gbqnsuqtm.sHtML

[T35] Lua：字典表
来源：http://www.blog.tarul.cn/Article/details/gvcgqkfcf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gclqerkhk.sHtML

[T36] Lua：函数
来源：http://wap.bbcook.cn/Article/details/gvvtfovys.sHtML

function add(a, b) return a + b end
来源：http://wap.epnwcf.com/Article/details/guzsjgwyp.sHtML

[T37] Lua：字符串拼接
来源：http://baike.vehdjk.com/Article/details/gciviipva.sHtML

"a" .. "b"
来源：http://3g.tarul.cn/Article/details/gilojdgrz.sHtML

[T38] Lua：条件
来源：http://mobile.sjlbkw.cn/Article/details/gsxxfteyi.sHtML

if x > 0 then print("正") end
来源：http://www.share.tarul.cn/Article/details/gvjjwwdwx.sHtML

[T39] Lua：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gntakbpfv.sHtML

string.find(s, "%d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvepehtb.sHtML

[T40] Lua：元表
来源：http://mobile.fktsv.cn/Article/details/gjaghgzqy.sHtML

setmetatable({}, { __index = base })
来源：http://3g.tarul.cn/Article/details/goyfptyno.sHtML

[T41] Perl：Hello World
来源：http://www.share.fktsv.cn/Article/details/gmgvgnmee.sHtML

print "Hello\n";
来源：http://read.share.epnwcf.com/Article/details/gnorpbdgy.sHtML

[T42] Perl：变量类型
来源：http://3g.tarul.cn/Article/details/gqsguvipv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fktsv.cn/Article/details/grykpnjkn.sHtML

[T43] Perl：字符串插值
来源：http://m.share.tarul.cn/Article/details/grgwwdrrt.sHtML

"值: $a"
来源：http://www.share.yfazqb.com/Article/details/gdhdakwqv.sHtML

[T44] Perl：条件
来源：http://blog.sjlbkw.cn/Article/details/gydnysomn.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.vehdjk.com/Article/details/gbpxcocgy.sHtML


<!-- 参考信息 -->