代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fktsv.cn/Article/details/gzqzhgahy.sHtML

[R36] 并发执行多个任务
来源：http://www.share.tarul.cn/Article/details/gmtwbkbzv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.epnwcf.com/Article/details/ghjbotfad.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.epnwcf.com/Article/details/glpftfila.sHtML

files=$(ls -1)
来源：http://wap.epnwcf.com/Article/details/gpkygyges.sHtML

[R38] 管道串联
来源：http://www.m.share.fktsv.cn/Article/details/gvrbsiynz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.tarul.cn/Article/details/giusgvdjc.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/grahrtwzt.sHtML

cmd > out.log 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gjtlidkwk.sHtML

[R40] 追加写日志
来源：http://read.share.bbcook.cn/Article/details/gkcswcodc.sHtML

echo "log" >> out.log
来源：http://www.blog.tarul.cn/Article/details/gsnvfthki.sHtML

[R41] 丢弃输出
来源：http://www.m.share.vehdjk.com/Article/details/gxtgyeukq.sHtML

cmd >/dev/null 2>&1
来源：http://wap.epnwcf.com/Article/details/gssnicrbc.sHtML

[R42] 输入重定向
来源：http://www.share.sjlbkw.cn/Article/details/gppppepux.sHtML

wc -l < a.txt
来源：http://www.share.fktsv.cn/Article/details/gqelbfaaw.sHtML

[R43] 按名字查找文件
来源：http://read.share.yfazqb.com/Article/details/gvlhaasin.sHtML

find . -name "*.log" -type f
来源：http://wap.yfazqb.com/Article/details/gvfdiixzz.sHtML

[R44] 按修改时间查找
来源：http://wap.epnwcf.com/Article/details/gvshnxcoe.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.epnwcf.com/Article/details/gpunvcpoo.sHtML

[R45] 批量删除
来源：http://www.m.share.vehdjk.com/Article/details/ggytwzgdz.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.tarul.cn/Article/details/grondvvdw.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.bbcook.cn/Article/details/gultanydk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.yfazqb.com/Article/details/ggymraibz.sHtML

[R47] sed 单行替换
来源：http://m.share.bbcook.cn/Article/details/gkeyrxrrt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/geaurvtkp.sHtML

[R48] awk 取指定列
来源：http://3g.vehdjk.com/Article/details/gzbwugakr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gqemfmpgk.sHtML

[R49] awk 带条件
来源：http://wap.sjlbkw.cn/Article/details/gazmqzzbz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.yfazqb.com/Article/details/gtznhzetl.sHtML

[R50] awk 求和
来源：http://www.share.fktsv.cn/Article/details/gwozbkxps.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gtpbtqjzn.sHtML

[R51] 排序去重取前几
来源：http://baike.tarul.cn/Article/details/gkydoudoa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.yfazqb.com/Article/details/gmobclshu.sHtML

[R52] 统计行数
来源：http://wap.bbcook.cn/Article/details/ggcdvkknn.sHtML

wc -l a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gjonzvvkz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.yfazqb.com/Article/details/gjxjmxsyd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.epnwcf.com/Article/details/grfvdlcxc.sHtML

[R54] 比较两个文件
来源：http://mobile.yfazqb.com/Article/details/gnyqqcfzy.sHtML

diff a.txt b.txt
来源：http://www.share.vehdjk.com/Article/details/gnaklcple.sHtML

[R55] 压缩与解压
来源：http://m.share.sjlbkw.cn/Article/details/gvqpjdjyc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.vehdjk.com/Article/details/groqqcflb.sHtML

[R56] 远程拷贝
来源：http://m.share.sjlbkw.cn/Article/details/ghtuholso.sHtML

scp file user@host:/path/
来源：http://m.share.bbcook.cn/Article/details/gobwnbnsj.sHtML

[R57] 远程执行命令
来源：http://www.blog.tarul.cn/Article/details/gmdbbuzrb.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqlwudcd.sHtML

[R58] 下载文件
来源：http://www.blog.bbcook.cn/Article/details/gogirpyge.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.yfazqb.com/Article/details/gqhivngzw.sHtML

[R59] 发 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gwjeefohs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.tarul.cn/Article/details/gbyeigkxh.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fktsv.cn/Article/details/groeyzolk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.epnwcf.com/Article/details/guakcgyzw.sHtML

[R61] 磁盘占用
来源：http://www.blog.sjlbkw.cn/Article/details/gshpqbkyo.sHtML

df -h;  du -sh *
来源：http://m.share.tarul.cn/Article/details/gujrwnqjv.sHtML

[R62] 找最占空间的文件
来源：http://blog.sjlbkw.cn/Article/details/gvdtuabqt.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.yfazqb.com/Article/details/gwvedieev.sHtML

[R63] 内存与进程
来源：http://baike.vehdjk.com/Article/details/gefxrtqdk.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.epnwcf.com/Article/details/gbpbqxjvy.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gehebtatm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fktsv.cn/Article/details/gfrrtxggz.sHtML

[R65] 查看端口占用
来源：http://baike.yfazqb.com/Article/details/gqvbfyjxv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.sjlbkw.cn/Article/details/ghnogxdfi.sHtML

[R66] 定时任务
来源：http://www.blog.vehdjk.com/Article/details/gdzxldnmu.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/gihovdtao.sHtML

[R67] 生成随机十六进制串
来源：http://baike.tarul.cn/Article/details/gyjjyxhna.sHtML

openssl rand -hex 16
来源：http://baike.vehdjk.com/Article/details/gekdtxzbp.sHtML

[R68] 计算文件校验值
来源：http://wap.vehdjk.com/Article/details/gahhfzols.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.epnwcf.com/Article/details/gnfodlacv.sHtML

[R69] 生成随机密码
来源：http://blog.tarul.cn/Article/details/gebfbyzgd.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.sjlbkw.cn/Article/details/grndhsomb.sHtML

[R70] 时间戳与互转
来源：http://mobile.fktsv.cn/Article/details/gerbrpslr.sHtML

date +%s;  date -d @1700000000
来源：http://3g.sjlbkw.cn/Article/details/gzauvqoel.sHtML

[R71] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gopfommhr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.tarul.cn/Article/details/gipyarlgd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fktsv.cn/Article/details/gqqytwbhr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/gvtomsszw.sHtML

[R73] 分割大日志
来源：http://m.share.bbcook.cn/Article/details/gtwciqolp.sHtML

split -l 1000 big.log part_
来源：http://www.share.epnwcf.com/Article/details/gytfomigf.sHtML

[R74] 批量重命名
来源：http://read.share.yfazqb.com/Article/details/gquawomur.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fktsv.cn/Article/details/gffdtypwi.sHtML

[R75] 导出环境变量
来源：http://read.share.bbcook.cn/Article/details/gzewcudws.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.vehdjk.com/Article/details/gthejwoli.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/gepuwvdqe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.bbcook.cn/Article/details/gyhyzxrxw.sHtML

[R77] 读取用户输入
来源：http://m.share.epnwcf.com/Article/details/ggdveajxg.sHtML

read -rp "请输入: " ans
来源：http://www.share.vehdjk.com/Article/details/gzjiggdjl.sHtML

[R78] 交互式菜单
来源：http://3g.yfazqb.com/Article/details/glgnyfmdp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gxabumbrs.sHtML

[R79] 解析命令行选项
来源：http://blog.epnwcf.com/Article/details/gubsrtfif.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.tarul.cn/Article/details/grekqifeb.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.epnwcf.com/Article/details/gksbosrxe.sHtML

time ./run.sh
来源：http://blog.epnwcf.com/Article/details/gnkvycypj.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gskcvpwdw.sHtML

S. C / C++ 专题
来源：http://www.blog.fktsv.cn/Article/details/gxgdexjho.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gubseelxn.sHtML

[S01] C：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gukmxkhpz.sHtML

#include <stdio.h>
来源：http://www.m.share.tarul.cn/Article/details/gzxqvmbhm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.yfazqb.com/Article/details/getbuanup.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/glqpqcfna.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.sjlbkw.cn/Article/details/gruxoxqhh.sHtML

[S03] C：读入整数
来源：http://baike.tarul.cn/Article/details/grdzaooxf.sHtML

int x; scanf("%d", &x);
来源：http://mobile.epnwcf.com/Article/details/ggscqdmgh.sHtML

[S04] C：字符串复制
来源：http://www.share.epnwcf.com/Article/details/gnoygrjzv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/gsoggxrwu.sHtML

[S05] C：字符串长度
来源：http://blog.tarul.cn/Article/details/gcjoobkgt.sHtML

strlen(s)
来源：http://m.share.fktsv.cn/Article/details/geklujyjs.sHtML

[S06] C：字符串比较
来源：http://baike.tarul.cn/Article/details/gxsillekc.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/gwrwqtlkv.sHtML

[S07] C：数组遍历求和
来源：http://blog.vehdjk.com/Article/details/gdttcjswe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.yfazqb.com/Article/details/govfpkdrd.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.bbcook.cn/Article/details/geuxkidht.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/grmmefopv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.epnwcf.com/Article/details/gexoslcec.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.vehdjk.com/Article/details/geumsfkrb.sHtML

[S10] C：指针与解引用
来源：http://www.share.epnwcf.com/Article/details/gfffsuftg.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.vehdjk.com/Article/details/gghtovlgq.sHtML

[S11] C：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gjvvuhndv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.bbcook.cn/Article/details/gxinalfvh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.epnwcf.com/Article/details/gvvbsbxbp.sHtML

fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/gxcfffnax.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gcmtgfpfj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/gjugvsaxk.sHtML

[S13] C：宏定义
来源：http://3g.vehdjk.com/Article/details/gipwozvak.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.yfazqb.com/Article/details/gwojbpzwp.sHtML

[S14] C：枚举
来源：http://www.blog.epnwcf.com/Article/details/gvqhqahhv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/ggamfcxpv.sHtML

[S15] C：类型转换
来源：http://baike.sjlbkw.cn/Article/details/ghzbtlbdl.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/gymleoeyj.sHtML

[S16] C：位操作置位
来源：http://mobile.tarul.cn/Article/details/gieuxtucq.sHtML

x |= (1 << 3);
来源：http://www.share.sjlbkw.cn/Article/details/gzavpsgyz.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gcmcqtdog.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fktsv.cn/Article/details/gehozhiwd.sHtML

[S18] C：命令行参数
来源：http://blog.epnwcf.com/Article/details/grulucjst.sHtML

int main(int argc, char **argv)
来源：http://mobile.yfazqb.com/Article/details/gldkflxrd.sHtML

[S19] C：快速排序
来源：http://baike.fktsv.cn/Article/details/gayxvypip.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/govnksvjf.sHtML

[S20] C：二分查找
来源：http://mobile.epnwcf.com/Article/details/gajyyrzdw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/grmkdpsvy.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.bbcook.cn/Article/details/gfqfsmhgd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.bbcook.cn/Article/details/getrsvylp.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/gvhaqqeek.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.tarul.cn/Article/details/gzzcpenfl.sHtML

[S23] C：随机数
来源：http://www.blog.fktsv.cn/Article/details/gbrxypclf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/gvdlteule.sHtML

[S24] C：获取本地时间
来源：http://3g.epnwcf.com/Article/details/gvoqspqqw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fktsv.cn/Article/details/gjlalyzuz.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/gtuaegxou.sHtML

memcpy(dst, src, n);
来源：http://3g.fktsv.cn/Article/details/gdbgjmidn.sHtML

[S26] C：内存清零
来源：http://m.share.fktsv.cn/Article/details/gimokwnzf.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.sjlbkw.cn/Article/details/grhuaafmq.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/gjniuavay.sHtML

const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gkbsgunvu.sHtML

[S28] C：静态变量
来源：http://baike.tarul.cn/Article/details/gjkevarfs.sHtML

static int counter = 0;
来源：http://m.share.tarul.cn/Article/details/ggsilpvat.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/gqrchjsux.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/gpjaphlsk.sHtML

[S30] C：头文件保护
来源：http://baike.epnwcf.com/Article/details/grjamijzw.sHtML

#ifndef X_H
来源：http://blog.bbcook.cn/Article/details/gxkqxyhdd.sHtML

#define X_H
来源：http://wap.fktsv.cn/Article/details/gsbxjqspy.sHtML

#endif
来源：http://www.share.vehdjk.com/Article/details/gimzdiazm.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/gsapuvffz.sHtML

#include <iostream>
来源：http://3g.fktsv.cn/Article/details/gpndekrtm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.yfazqb.com/Article/details/gfmiefyjv.sHtML

[S32] C++：字符串
来源：http://www.m.share.epnwcf.com/Article/details/gkeznzxwd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.epnwcf.com/Article/details/gknycqkqf.sHtML

[S33] C++：vector 增删
来源：http://read.share.fktsv.cn/Article/details/gwjmegixm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fktsv.cn/Article/details/guuscxajs.sHtML

[S34] C++：遍历 vector
来源：http://wap.tarul.cn/Article/details/gndvrsucl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.epnwcf.com/Article/details/gnrktbehu.sHtML

[S35] C++：map
来源：http://www.blog.bbcook.cn/Article/details/gmauevyxc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/ghxawiigu.sHtML

[S36] C++：unordered_map
来源：http://blog.bbcook.cn/Article/details/gqtxkxifj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/guashclrm.sHtML

[S37] C++：set
来源：http://3g.tarul.cn/Article/details/gqdlimisa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fktsv.cn/Article/details/glutxqvwq.sHtML

[S38] C++：排序
来源：http://3g.sjlbkw.cn/Article/details/gmdgikxar.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.bbcook.cn/Article/details/gquvvlqrx.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.vehdjk.com/Article/details/gunfjvoxw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.yfazqb.com/Article/details/gacgjgbht.sHtML

[S40] C++：查找元素
来源：http://read.share.sjlbkw.cn/Article/details/ghrdjkwou.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gwytgmljr.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gbavxrudk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.yfazqb.com/Article/details/gqxmyguqv.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fktsv.cn/Article/details/gezcqhkcf.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.vehdjk.com/Article/details/geyegkwba.sHtML

[S43] C++：智能指针
来源：http://mobile.yfazqb.com/Article/details/grqtimglr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.epnwcf.com/Article/details/gvjzmsjhk.sHtML

[S44] C++：引用传参
来源：http://blog.bbcook.cn/Article/details/gcurgfvbh.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.yfazqb.com/Article/details/gydaagsbm.sHtML

[S45] C++：lambda
来源：http://3g.bbcook.cn/Article/details/gsshhdjms.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.epnwcf.com/Article/details/gjqwbykew.sHtML

[S46] C++：函数模板
来源：http://wap.fktsv.cn/Article/details/gfhmyaffb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.yfazqb.com/Article/details/gdoknqnqg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.tarul.cn/Article/details/gtqiylpbo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.vehdjk.com/Article/details/geqtyigps.sHtML

[S48] C++：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gngnzxdlp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.sjlbkw.cn/Article/details/gpudfctro.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gxtgnqcyk.sHtML

[S49] C++：写文件
来源：http://3g.vehdjk.com/Article/details/grofvjysb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/grduojuwu.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/ggzvrculg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gnaunrrcz.sHtML

[S51] C++：显式类型转换
来源：http://baike.fktsv.cn/Article/details/gnbxxbeuc.sHtML

static_cast<double>(a) / b
来源：http://wap.bbcook.cn/Article/details/gnzwvklcg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/gqnpxxowp.sHtML

int size() const noexcept { return n_; }
来源：http://wap.epnwcf.com/Article/details/gubkncvdt.sHtML

[S53] C++：移动语义
来源：http://blog.epnwcf.com/Article/details/gafmhwqmk.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.epnwcf.com/Article/details/gwtjsldow.sHtML

[S54] C++：异常处理
来源：http://wap.bbcook.cn/Article/details/govevwyor.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.tarul.cn/Article/details/gfowqsytc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.vehdjk.com/Article/details/gzjbpterv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.yfazqb.com/Article/details/gvgxmrfkq.sHtML

[S56] C++：optional
来源：http://www.m.share.yfazqb.com/Article/details/gazumsnjd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.tarul.cn/Article/details/gxflaufkb.sHtML

[S57] C++：编译期常量
来源：http://3g.sjlbkw.cn/Article/details/gxrmzngqe.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgjmwrnf.sHtML

[S58] C++：命名空间
来源：http://3g.bbcook.cn/Article/details/gvfqizuwy.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.bbcook.cn/Article/details/gxzkxvaun.sHtML

[S59] C++：静态断言
来源：http://www.m.share.yfazqb.com/Article/details/gyaieoklm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.vehdjk.com/Article/details/gviheibzd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.epnwcf.com/Article/details/gfryklgay.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fktsv.cn/Article/details/gntjnjczf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gyqozxbdi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.yfazqb.com/Article/details/goehnxwiz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gitkpxdta.sHtML

[T01] Kotlin：Hello World
来源：http://baike.tarul.cn/Article/details/ggorarsou.sHtML

println("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gpfcxobcx.sHtML

[T02] Kotlin：变量
来源：http://wap.sjlbkw.cn/Article/details/gsijjzwsf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fktsv.cn/Article/details/gkfuyisgv.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.tarul.cn/Article/details/gwqqxkyal.sHtML

"值: $b"
来源：http://blog.tarul.cn/Article/details/gffcpxcdz.sHtML

[T04] Kotlin：空安全
来源：http://read.share.sjlbkw.cn/Article/details/gpmiiywde.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.sjlbkw.cn/Article/details/gayxwndcm.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.yfazqb.com/Article/details/gnoqdrgof.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.epnwcf.com/Article/details/glrpizymr.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.epnwcf.com/Article/details/godgmocbc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gallbjmph.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.bbcook.cn/Article/details/ghzcyyxte.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gufxuzmhg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fktsv.cn/Article/details/ghfhasdvh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.vehdjk.com/Article/details/gyfezfrit.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.sjlbkw.cn/Article/details/guxchgtuu.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.bbcook.cn/Article/details/gsyybfnws.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fktsv.cn/Article/details/gfstyovac.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/gywcvrqzt.sHtML

[T11] Kotlin：协程
来源：http://wap.bbcook.cn/Article/details/gfoqhgmuc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.epnwcf.com/Article/details/gddazwwuh.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.bbcook.cn/Article/details/gnussnerj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gjbjdglqe.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.vehdjk.com/Article/details/gwvzyeulk.sHtML

val m = mapOf("a" to 1)
来源：http://blog.tarul.cn/Article/details/glclntpkx.sHtML

[T14] Kotlin：循环
来源：http://mobile.vehdjk.com/Article/details/ghctboize.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gzzzmkgax.sHtML

[T15] Kotlin：接口
来源：http://www.share.sjlbkw.cn/Article/details/gxpxtrawz.sHtML

interface Shape { fun area(): Double }
来源：http://baike.epnwcf.com/Article/details/gpavqvaot.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gwvebggwm.sHtML

print("Hello")
来源：http://blog.tarul.cn/Article/details/gjgcxilhw.sHtML

[T17] Swift：变量与常量
来源：http://wap.vehdjk.com/Article/details/glexwkzir.sHtML

var a = 1;  let b = 2
来源：http://read.share.vehdjk.com/Article/details/guuvqaaug.sHtML

[T18] Swift：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gvmbhjuvx.sHtML

"值: \(b)"
来源：http://www.m.share.tarul.cn/Article/details/gzawpqfes.sHtML

[T19] Swift：可选绑定
来源：http://read.share.bbcook.cn/Article/details/gqmqwjyss.sHtML

if let n = opt { print(n) }
来源：http://baike.fktsv.cn/Article/details/gojxkrhin.sHtML

[T20] Swift：数组操作
来源：http://m.share.bbcook.cn/Article/details/ghbvuxmdx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/guzilsfoe.sHtML

[T21] Swift：遍历
来源：http://m.share.bbcook.cn/Article/details/gxjhoinxj.sHtML

for x in a { print(x) }
来源：http://3g.vehdjk.com/Article/details/gstdkgpmn.sHtML

[T22] Swift：字典
来源：http://www.m.share.epnwcf.com/Article/details/glqkalazy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.bbcook.cn/Article/details/gjlkxhrxk.sHtML

[T23] Swift：函数
来源：http://wap.yfazqb.com/Article/details/gemvzuqgs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.epnwcf.com/Article/details/gsahpnkos.sHtML

[T24] Swift：闭包
来源：http://read.share.fktsv.cn/Article/details/gczccqqed.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.tarul.cn/Article/details/gvlqrfgzg.sHtML

[T25] Swift：结构体
来源：http://www.share.yfazqb.com/Article/details/gxslshrwy.sHtML

struct P { var x: Int }
来源：http://m.share.tarul.cn/Article/details/gkjaquzvc.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.sjlbkw.cn/Article/details/gddczausc.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.epnwcf.com/Article/details/gzzoefeoq.sHtML

[T27] Swift：错误处理
来源：http://blog.fktsv.cn/Article/details/gcvumtoha.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.vehdjk.com/Article/details/grkwdaivt.sHtML

[T28] Swift：枚举
来源：http://wap.bbcook.cn/Article/details/gmgoibpja.sHtML

enum Color { case red, green }
来源：http://wap.fktsv.cn/Article/details/gnhodzjzh.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.tarul.cn/Article/details/gmdflaxdp.sHtML

guard let x = opt else { return }
来源：http://3g.epnwcf.com/Article/details/gfphlioat.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/ggcneqxiu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fktsv.cn/Article/details/gdoiouxpx.sHtML

[T31] Lua：Hello World
来源：http://www.share.fktsv.cn/Article/details/gvalgnrnr.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/gvfsgswzp.sHtML

[T32] Lua：局部变量
来源：http://read.share.epnwcf.com/Article/details/gheknlsdh.sHtML

local a = 1
来源：http://3g.fktsv.cn/Article/details/gwsamxnhf.sHtML

[T33] Lua：表（数组）
来源：http://wap.epnwcf.com/Article/details/gdecxmuch.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.yfazqb.com/Article/details/gqzxambew.sHtML

[T34] Lua：遍历表
来源：http://read.share.tarul.cn/Article/details/gdzbpqmax.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.sjlbkw.cn/Article/details/goddrungy.sHtML

[T35] Lua：字典表
来源：http://www.m.share.tarul.cn/Article/details/gvcponxrk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gwokadcuw.sHtML

[T36] Lua：函数
来源：http://read.share.epnwcf.com/Article/details/gxicauuww.sHtML

function add(a, b) return a + b end
来源：http://mobile.tarul.cn/Article/details/gtqduhgas.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gjingzbmy.sHtML

"a" .. "b"
来源：http://read.share.sjlbkw.cn/Article/details/glaxcbuiv.sHtML

[T38] Lua：条件
来源：http://www.share.bbcook.cn/Article/details/gtchjrfvx.sHtML

if x > 0 then print("正") end
来源：http://blog.sjlbkw.cn/Article/details/gzrntwvpm.sHtML


<!-- 参考信息 -->