代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.vehdjk.com/Article/details/gjirgqasj.sHtML

[R36] 并发执行多个任务
来源：http://mobile.yfazqb.com/Article/details/gbseecjws.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.vehdjk.com/Article/details/ghtbxyoox.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/gykkvsjhk.sHtML

files=$(ls -1)
来源：http://www.blog.fktsv.cn/Article/details/glhtlcivk.sHtML

[R38] 管道串联
来源：http://3g.tarul.cn/Article/details/goonyvbjc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fktsv.cn/Article/details/gfvpfoanx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.epnwcf.com/Article/details/geetpmsxe.sHtML

cmd > out.log 2>&1
来源：http://3g.bbcook.cn/Article/details/gcdzelljs.sHtML

[R40] 追加写日志
来源：http://baike.fktsv.cn/Article/details/glmwruzxm.sHtML

echo "log" >> out.log
来源：http://www.m.share.bbcook.cn/Article/details/gpllblhcn.sHtML

[R41] 丢弃输出
来源：http://mobile.tarul.cn/Article/details/gzouuhica.sHtML

cmd >/dev/null 2>&1
来源：http://baike.bbcook.cn/Article/details/gjwojrayf.sHtML

[R42] 输入重定向
来源：http://m.share.bbcook.cn/Article/details/gascdkcmn.sHtML

wc -l < a.txt
来源：http://www.blog.epnwcf.com/Article/details/gylycjlmi.sHtML

[R43] 按名字查找文件
来源：http://read.share.bbcook.cn/Article/details/gmeiwpwrr.sHtML

find . -name "*.log" -type f
来源：http://3g.yfazqb.com/Article/details/gettanvvp.sHtML

[R44] 按修改时间查找
来源：http://wap.yfazqb.com/Article/details/gazsmgege.sHtML

find . -mtime -7 -type f
来源：http://baike.sjlbkw.cn/Article/details/gfltujwfp.sHtML

[R45] 批量删除
来源：http://m.share.epnwcf.com/Article/details/ghuixoiay.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/gqkqfezio.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/ghizvopzp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.bbcook.cn/Article/details/gkejeught.sHtML

[R47] sed 单行替换
来源：http://www.blog.fktsv.cn/Article/details/ghqzaoeat.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.yfazqb.com/Article/details/grgprfnza.sHtML

[R48] awk 取指定列
来源：http://baike.tarul.cn/Article/details/gczopqsdp.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.bbcook.cn/Article/details/gupghodya.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/goknbrkek.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/gslhrxvld.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/gnummvnlz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gopkhypbn.sHtML

[R51] 排序去重取前几
来源：http://read.share.vehdjk.com/Article/details/gurqyscek.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.yfazqb.com/Article/details/gcbozptjc.sHtML

[R52] 统计行数
来源：http://www.blog.yfazqb.com/Article/details/givjoolzn.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gfyuitozz.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.yfazqb.com/Article/details/gcsdmytrx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.epnwcf.com/Article/details/ghshukzwz.sHtML

[R54] 比较两个文件
来源：http://www.blog.bbcook.cn/Article/details/gyjgwwsak.sHtML

diff a.txt b.txt
来源：http://baike.sjlbkw.cn/Article/details/ggkqhckab.sHtML

[R55] 压缩与解压
来源：http://mobile.sjlbkw.cn/Article/details/gypmnvzjk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/gxfzrbnnx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gvnyxnrqx.sHtML

scp file user@host:/path/
来源：http://m.share.epnwcf.com/Article/details/gsqqmizeg.sHtML

[R57] 远程执行命令
来源：http://3g.tarul.cn/Article/details/gvuvgpskq.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.vehdjk.com/Article/details/gzlijomou.sHtML

[R58] 下载文件
来源：http://www.share.bbcook.cn/Article/details/grliqlthk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.vehdjk.com/Article/details/gvqhjfhhk.sHtML

[R59] 发 POST JSON
来源：http://read.share.tarul.cn/Article/details/goemswrvc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.sjlbkw.cn/Article/details/gomvkeyge.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/gqeqmfgsn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fktsv.cn/Article/details/grbwkxqoe.sHtML

[R61] 磁盘占用
来源：http://wap.epnwcf.com/Article/details/gdrottkad.sHtML

df -h;  du -sh *
来源：http://read.share.epnwcf.com/Article/details/gxmlprsgi.sHtML

[R62] 找最占空间的文件
来源：http://read.share.tarul.cn/Article/details/gswylytdf.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.yfazqb.com/Article/details/gfuvbjgpx.sHtML

[R63] 内存与进程
来源：http://www.share.tarul.cn/Article/details/gjnilxogb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fktsv.cn/Article/details/grinwggyp.sHtML

[R64] 结束进程
来源：http://m.share.epnwcf.com/Article/details/gdktgarxm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.yfazqb.com/Article/details/giusmdzkq.sHtML

[R65] 查看端口占用
来源：http://www.m.share.bbcook.cn/Article/details/giyzdqaku.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.bbcook.cn/Article/details/gbbwhzfit.sHtML

[R66] 定时任务
来源：http://m.share.vehdjk.com/Article/details/gwmlvjhbl.sHtML

crontab -e;  crontab -l
来源：http://m.share.sjlbkw.cn/Article/details/gdgfgmdob.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fktsv.cn/Article/details/gedbmsocp.sHtML

openssl rand -hex 16
来源：http://www.blog.yfazqb.com/Article/details/gelomctfc.sHtML

[R68] 计算文件校验值
来源：http://read.share.epnwcf.com/Article/details/ggjmsfkib.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.tarul.cn/Article/details/gpdvyjfqy.sHtML

[R69] 生成随机密码
来源：http://www.share.fktsv.cn/Article/details/glgnugzbx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.vehdjk.com/Article/details/gwfeqqcme.sHtML

[R70] 时间戳与互转
来源：http://www.share.sjlbkw.cn/Article/details/gtbmfupjg.sHtML

date +%s;  date -d @1700000000
来源：http://wap.tarul.cn/Article/details/glxfucbdk.sHtML

[R71] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gbkldhfzz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.vehdjk.com/Article/details/gzjulizfr.sHtML

[R72] 等待端口就绪
来源：http://blog.yfazqb.com/Article/details/gdqvxsbmo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gzsapipoy.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/gvktwpkgz.sHtML

split -l 1000 big.log part_
来源：http://mobile.tarul.cn/Article/details/gbeokouqc.sHtML

[R74] 批量重命名
来源：http://www.m.share.fktsv.cn/Article/details/gapdamhxv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.vehdjk.com/Article/details/gboojjnit.sHtML

[R75] 导出环境变量
来源：http://www.m.share.epnwcf.com/Article/details/grutbdgxc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fktsv.cn/Article/details/guaumwcki.sHtML

[R76] 使用临时文件
来源：http://3g.epnwcf.com/Article/details/gsfefvnty.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/ggzebcnfy.sHtML

[R77] 读取用户输入
来源：http://wap.fktsv.cn/Article/details/gufymmjer.sHtML

read -rp "请输入: " ans
来源：http://wap.yfazqb.com/Article/details/ghwmusgyy.sHtML

[R78] 交互式菜单
来源：http://read.share.tarul.cn/Article/details/gwgtqvjdh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.vehdjk.com/Article/details/gwiadctab.sHtML

[R79] 解析命令行选项
来源：http://www.share.vehdjk.com/Article/details/gltfaljha.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gdbppbiks.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/gasjxxuyl.sHtML

time ./run.sh
来源：http://www.share.yfazqb.com/Article/details/gqrhnoghy.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gbuqrmrra.sHtML

S. C / C++ 专题
来源：http://www.blog.fktsv.cn/Article/details/gqqdqrclx.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grfeywwgn.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gilspvovq.sHtML

#include <stdio.h>
来源：http://mobile.fktsv.cn/Article/details/gnrrtqylq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.vehdjk.com/Article/details/gotgzzmha.sHtML

[S02] C：变量与格式化输出
来源：http://baike.tarul.cn/Article/details/gzzndqexy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.vehdjk.com/Article/details/gxrxpjska.sHtML

[S03] C：读入整数
来源：http://read.share.sjlbkw.cn/Article/details/gexsyaros.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fktsv.cn/Article/details/gcvcxghus.sHtML

[S04] C：字符串复制
来源：http://3g.tarul.cn/Article/details/gboctnsqh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/gcntbkfyo.sHtML

[S05] C：字符串长度
来源：http://m.share.epnwcf.com/Article/details/gdawfidsi.sHtML

strlen(s)
来源：http://mobile.sjlbkw.cn/Article/details/gesbawtnv.sHtML

[S06] C：字符串比较
来源：http://www.share.tarul.cn/Article/details/grnppsrgo.sHtML

strcmp(a, b) == 0
来源：http://3g.fktsv.cn/Article/details/gbebjpbkc.sHtML

[S07] C：数组遍历求和
来源：http://www.share.bbcook.cn/Article/details/gdpvfjwel.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.yfazqb.com/Article/details/gkumuybjz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.sjlbkw.cn/Article/details/gmqkwodxz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.tarul.cn/Article/details/gcmhvkxkt.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.epnwcf.com/Article/details/gnnrvsnsd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fktsv.cn/Article/details/gxjloohmt.sHtML

[S10] C：指针与解引用
来源：http://wap.bbcook.cn/Article/details/gafbregpu.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.epnwcf.com/Article/details/gdorakzlg.sHtML

[S11] C：逐行读文件
来源：http://wap.tarul.cn/Article/details/ggikygfrw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fktsv.cn/Article/details/gpkidlvnc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.vehdjk.com/Article/details/gjbztbhip.sHtML

fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gqxqzfark.sHtML

[S12] C：写文件
来源：http://wap.bbcook.cn/Article/details/gxvmnklkk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gnaldxjhm.sHtML

[S13] C：宏定义
来源：http://www.m.share.vehdjk.com/Article/details/gmpctgmmi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.bbcook.cn/Article/details/grprukdzb.sHtML

[S14] C：枚举
来源：http://m.share.fktsv.cn/Article/details/glzsjprnx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.yfazqb.com/Article/details/gyozyvvnl.sHtML

[S15] C：类型转换
来源：http://blog.sjlbkw.cn/Article/details/gjwlzktls.sHtML

(double) a / b
来源：http://www.share.yfazqb.com/Article/details/gcpushtom.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/gphsaibyy.sHtML

x |= (1 << 3);
来源：http://mobile.tarul.cn/Article/details/gpkkvoawi.sHtML

[S17] C：安全拼接字符串
来源：http://wap.bbcook.cn/Article/details/gfogzlbbp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.tarul.cn/Article/details/gmovfybsd.sHtML

[S18] C：命令行参数
来源：http://blog.fktsv.cn/Article/details/glwaacdrh.sHtML

int main(int argc, char **argv)
来源：http://m.share.bbcook.cn/Article/details/guoabscfc.sHtML

[S19] C：快速排序
来源：http://m.share.fktsv.cn/Article/details/gtyddaljz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/gjphduvxz.sHtML

[S20] C：二分查找
来源：http://mobile.tarul.cn/Article/details/gouajjbcf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gbsxmssev.sHtML

[S21] C：字符类别判断
来源：http://www.blog.sjlbkw.cn/Article/details/guofnmwom.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.bbcook.cn/Article/details/gmektcaxv.sHtML

[S22] C：字符串转数字
来源：http://3g.bbcook.cn/Article/details/greakghte.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.vehdjk.com/Article/details/gjoxfdycy.sHtML

[S23] C：随机数
来源：http://m.share.vehdjk.com/Article/details/gbbcsjnoz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/gtelwytju.sHtML

[S24] C：获取本地时间
来源：http://blog.yfazqb.com/Article/details/gigjpzkcp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.vehdjk.com/Article/details/gzmwedcyg.sHtML

[S25] C：内存拷贝
来源：http://mobile.tarul.cn/Article/details/gvckygaqh.sHtML

memcpy(dst, src, n);
来源：http://blog.fktsv.cn/Article/details/ghqgjldjn.sHtML

[S26] C：内存清零
来源：http://read.share.vehdjk.com/Article/details/gqvbveigi.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.tarul.cn/Article/details/gtnjqrbvm.sHtML

[S27] C：定义常量
来源：http://www.m.share.fktsv.cn/Article/details/grwmefurw.sHtML

const double PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gpwbiopwb.sHtML

[S28] C：静态变量
来源：http://m.share.bbcook.cn/Article/details/glufavnrd.sHtML

static int counter = 0;
来源：http://blog.bbcook.cn/Article/details/gjaupshkm.sHtML

[S29] C：变参函数
来源：http://wap.tarul.cn/Article/details/gsqxnlsot.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.epnwcf.com/Article/details/gjzrdjpts.sHtML

[S30] C：头文件保护
来源：http://wap.yfazqb.com/Article/details/ggjmwuqqu.sHtML

#ifndef X_H
来源：http://www.blog.fktsv.cn/Article/details/goxhtmhaj.sHtML

#define X_H
来源：http://www.blog.yfazqb.com/Article/details/gjixzyvfv.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/glagzsuye.sHtML

[S31] C++：Hello World
来源：http://mobile.fktsv.cn/Article/details/grbqsesut.sHtML

#include <iostream>
来源：http://baike.bbcook.cn/Article/details/gfeujaltv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/goeookcrr.sHtML

[S32] C++：字符串
来源：http://mobile.bbcook.cn/Article/details/gygdvsclf.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/gkhyqacvc.sHtML

[S33] C++：vector 增删
来源：http://read.share.epnwcf.com/Article/details/ghhgyqnbz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.sjlbkw.cn/Article/details/gbxdybrec.sHtML

[S34] C++：遍历 vector
来源：http://read.share.epnwcf.com/Article/details/gmmdwtesj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.yfazqb.com/Article/details/glnocfsus.sHtML

[S35] C++：map
来源：http://3g.epnwcf.com/Article/details/ggsifikhf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gufkjtjvg.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.yfazqb.com/Article/details/gzeejjzkk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gfupafzwp.sHtML

[S37] C++：set
来源：http://m.share.bbcook.cn/Article/details/goeswimlb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.tarul.cn/Article/details/gfvxdvpiw.sHtML

[S38] C++：排序
来源：http://blog.epnwcf.com/Article/details/ghsavckno.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.epnwcf.com/Article/details/gmsmgwfei.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.epnwcf.com/Article/details/gxcqvemec.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.vehdjk.com/Article/details/gtudjvuvb.sHtML

[S40] C++：查找元素
来源：http://www.m.share.sjlbkw.cn/Article/details/ghshmkvit.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.yfazqb.com/Article/details/ggtzucztj.sHtML

[S41] C++：类与构造函数
来源：http://3g.tarul.cn/Article/details/gqkirlewx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.tarul.cn/Article/details/gxyvzsgng.sHtML

[S42] C++：继承与虚函数
来源：http://wap.vehdjk.com/Article/details/gaodclssb.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.epnwcf.com/Article/details/galofthdq.sHtML

[S43] C++：智能指针
来源：http://3g.fktsv.cn/Article/details/gkvjwdylj.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.tarul.cn/Article/details/ghslumagm.sHtML

[S44] C++：引用传参
来源：http://blog.epnwcf.com/Article/details/gxpeevttj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/gesvkrstv.sHtML

[S45] C++：lambda
来源：http://www.blog.yfazqb.com/Article/details/gtkmpcrxo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.epnwcf.com/Article/details/gevzcubqo.sHtML

[S46] C++：函数模板
来源：http://3g.vehdjk.com/Article/details/gfjyarifc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.bbcook.cn/Article/details/gvaqaouja.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.epnwcf.com/Article/details/gtxzztgwo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.epnwcf.com/Article/details/gbnkkmczl.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gsukqcqcb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.epnwcf.com/Article/details/glrwmolhx.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.yfazqb.com/Article/details/gvkbiddeu.sHtML

[S49] C++：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gghuxrtsf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fktsv.cn/Article/details/gqqycrbdl.sHtML

[S50] C++：格式化数字
来源：http://blog.bbcook.cn/Article/details/gfnzlsqix.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gpbakxarq.sHtML

[S51] C++：显式类型转换
来源：http://m.share.epnwcf.com/Article/details/gakxjdiri.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/gkvkdupfe.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fktsv.cn/Article/details/gspdhwche.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.sjlbkw.cn/Article/details/gzfndshzg.sHtML

[S53] C++：移动语义
来源：http://www.share.tarul.cn/Article/details/gozjgmkje.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.epnwcf.com/Article/details/gwjjrmtzn.sHtML

[S54] C++：异常处理
来源：http://blog.vehdjk.com/Article/details/gooxvaqra.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.bbcook.cn/Article/details/gpkttdzqw.sHtML

[S55] C++：结构化绑定
来源：http://wap.epnwcf.com/Article/details/gubdubcpz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.vehdjk.com/Article/details/gympkrjjj.sHtML

[S56] C++：optional
来源：http://3g.sjlbkw.cn/Article/details/gjectfxqp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.epnwcf.com/Article/details/gjenjzqdi.sHtML

[S57] C++：编译期常量
来源：http://3g.vehdjk.com/Article/details/gdsusnyqi.sHtML

constexpr int N = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gdcqcceqq.sHtML

[S58] C++：命名空间
来源：http://www.blog.yfazqb.com/Article/details/gorvsrpop.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.sjlbkw.cn/Article/details/gaupyhotk.sHtML

[S59] C++：静态断言
来源：http://3g.sjlbkw.cn/Article/details/gymhosuzj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.tarul.cn/Article/details/gbiqjzsht.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.bbcook.cn/Article/details/gsltdauio.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.bbcook.cn/Article/details/gpjelptjq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ggbdifnfy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.bbcook.cn/Article/details/gepblcros.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/govtprhzq.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/glgaxccqa.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gjxktswrt.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/gjfcgtufl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.vehdjk.com/Article/details/glqywtgvm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.epnwcf.com/Article/details/ganeiwdsl.sHtML

"值: $b"
来源：http://read.share.epnwcf.com/Article/details/gdijobvpv.sHtML

[T04] Kotlin：空安全
来源：http://baike.sjlbkw.cn/Article/details/grvzfdrzl.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.tarul.cn/Article/details/gqqgastxx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.bbcook.cn/Article/details/gebsllecy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.sjlbkw.cn/Article/details/gxokdslem.sHtML

[T06] Kotlin：集合映射
来源：http://blog.vehdjk.com/Article/details/ghagydvkh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.tarul.cn/Article/details/gclgwfbye.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fktsv.cn/Article/details/gcuwwyyxk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fktsv.cn/Article/details/gdlllxbjp.sHtML

[T08] Kotlin：数据类
来源：http://3g.sjlbkw.cn/Article/details/guevwoprb.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.epnwcf.com/Article/details/gzlepfwfm.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.yfazqb.com/Article/details/gvjscqrrf.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.bbcook.cn/Article/details/gyjqccvil.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.epnwcf.com/Article/details/ghomzbxwl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/gbxlsbqms.sHtML

[T11] Kotlin：协程
来源：http://wap.tarul.cn/Article/details/gyaqzgkrk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.epnwcf.com/Article/details/ghhvhglgh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.epnwcf.com/Article/details/gflngztmz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.tarul.cn/Article/details/gufdqpeyp.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.yfazqb.com/Article/details/gawjvjauk.sHtML

val m = mapOf("a" to 1)
来源：http://wap.tarul.cn/Article/details/glwxewekg.sHtML

[T14] Kotlin：循环
来源：http://3g.sjlbkw.cn/Article/details/gedvayvek.sHtML

for (i in 1..10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gvfrgzfdb.sHtML

[T15] Kotlin：接口
来源：http://read.share.yfazqb.com/Article/details/gswrhahba.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.bbcook.cn/Article/details/gruntyjyz.sHtML

[T16] Swift：Hello World
来源：http://3g.tarul.cn/Article/details/gutijwgiq.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/gfxmlgeoy.sHtML

[T17] Swift：变量与常量
来源：http://m.share.tarul.cn/Article/details/gliwwcgad.sHtML

var a = 1;  let b = 2
来源：http://wap.bbcook.cn/Article/details/grppcksnr.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gautjzicu.sHtML

"值: \(b)"
来源：http://mobile.epnwcf.com/Article/details/grbptcacj.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.vehdjk.com/Article/details/gzorgoepk.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.bbcook.cn/Article/details/gvglsoamm.sHtML

[T20] Swift：数组操作
来源：http://blog.sjlbkw.cn/Article/details/gxhwsekon.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.vehdjk.com/Article/details/gekxhcyjz.sHtML

[T21] Swift：遍历
来源：http://www.share.bbcook.cn/Article/details/gzxpzplns.sHtML

for x in a { print(x) }
来源：http://m.share.tarul.cn/Article/details/gehzfpdif.sHtML

[T22] Swift：字典
来源：http://baike.vehdjk.com/Article/details/gsemttqui.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.epnwcf.com/Article/details/gafgkynhm.sHtML

[T23] Swift：函数
来源：http://mobile.bbcook.cn/Article/details/gohfgeqzq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.yfazqb.com/Article/details/goagwdkif.sHtML

[T24] Swift：闭包
来源：http://www.share.yfazqb.com/Article/details/gwfuwqpof.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.yfazqb.com/Article/details/ghtukbrxc.sHtML

[T25] Swift：结构体
来源：http://wap.vehdjk.com/Article/details/gnvahxjke.sHtML

struct P { var x: Int }
来源：http://wap.fktsv.cn/Article/details/gnzuryipd.sHtML

[T26] Swift：类与重写
来源：http://3g.epnwcf.com/Article/details/grqmrvmva.sHtML

class A: Base { override func f() {} }
来源：http://m.share.tarul.cn/Article/details/gwttazbwn.sHtML

[T27] Swift：错误处理
来源：http://wap.epnwcf.com/Article/details/ggzqwbehn.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.sjlbkw.cn/Article/details/gjfrtvxpm.sHtML

[T28] Swift：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/grpdwzkwp.sHtML

enum Color { case red, green }
来源：http://baike.yfazqb.com/Article/details/gnoisjlae.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.epnwcf.com/Article/details/gildwzrxd.sHtML

guard let x = opt else { return }
来源：http://blog.epnwcf.com/Article/details/gkuttkhpz.sHtML

[T30] Swift：协议
来源：http://www.blog.bbcook.cn/Article/details/gkqrtfrcu.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fktsv.cn/Article/details/gekturxiq.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/gycxtxzfi.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/gskzotikt.sHtML

[T32] Lua：局部变量
来源：http://www.share.epnwcf.com/Article/details/gltetohmt.sHtML

local a = 1
来源：http://read.share.epnwcf.com/Article/details/gjmuxyztw.sHtML

[T33] Lua：表（数组）
来源：http://baike.sjlbkw.cn/Article/details/gaxhjompa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fktsv.cn/Article/details/gafzfpalj.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gbkrgbipc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.tarul.cn/Article/details/gryhrrgfi.sHtML

[T35] Lua：字典表
来源：http://blog.bbcook.cn/Article/details/gmtcynevt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fktsv.cn/Article/details/gnnyesfup.sHtML

[T36] Lua：函数
来源：http://wap.vehdjk.com/Article/details/gewyxhqdt.sHtML

function add(a, b) return a + b end
来源：http://3g.fktsv.cn/Article/details/ghcbdcihj.sHtML

[T37] Lua：字符串拼接
来源：http://blog.yfazqb.com/Article/details/gsfrjkscz.sHtML

"a" .. "b"
来源：http://www.m.share.tarul.cn/Article/details/gxjzusbuq.sHtML

[T38] Lua：条件
来源：http://blog.sjlbkw.cn/Article/details/gzguqkxht.sHtML

if x > 0 then print("正") end
来源：http://wap.vehdjk.com/Article/details/gwwkbyxps.sHtML


<!-- 参考信息 -->