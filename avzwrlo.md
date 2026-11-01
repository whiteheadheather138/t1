代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.sjlbkw.cn/Article/details/gsbhjtnus.sHtML

[R36] 并发执行多个任务
来源：http://m.share.epnwcf.com/Article/details/gacduwjsg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.sjlbkw.cn/Article/details/gobhklawb.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/gvcxrthmf.sHtML

files=$(ls -1)
来源：http://baike.fktsv.cn/Article/details/guhmxukzw.sHtML

[R38] 管道串联
来源：http://read.share.epnwcf.com/Article/details/gsqvrlvut.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.tarul.cn/Article/details/gucskvrcz.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.bbcook.cn/Article/details/gyrwoihtf.sHtML

cmd > out.log 2>&1
来源：http://www.blog.vehdjk.com/Article/details/gkwdkywrt.sHtML

[R40] 追加写日志
来源：http://3g.yfazqb.com/Article/details/gmvsomswm.sHtML

echo "log" >> out.log
来源：http://3g.vehdjk.com/Article/details/gsdcjjajq.sHtML

[R41] 丢弃输出
来源：http://baike.bbcook.cn/Article/details/gyyornabp.sHtML

cmd >/dev/null 2>&1
来源：http://wap.tarul.cn/Article/details/guewokkhx.sHtML

[R42] 输入重定向
来源：http://blog.sjlbkw.cn/Article/details/gtqxcupyk.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/gmhgvfrze.sHtML

[R43] 按名字查找文件
来源：http://baike.tarul.cn/Article/details/gnzdjfcie.sHtML

find . -name "*.log" -type f
来源：http://www.blog.sjlbkw.cn/Article/details/ghjkohjna.sHtML

[R44] 按修改时间查找
来源：http://baike.tarul.cn/Article/details/gpnymmiox.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.yfazqb.com/Article/details/gsgwcnsyk.sHtML

[R45] 批量删除
来源：http://www.m.share.vehdjk.com/Article/details/gbnzkpkuf.sHtML

find . -name "*.tmp" -delete
来源：http://3g.yfazqb.com/Article/details/gzbnlaglb.sHtML

[R46] 递归替换文件内容
来源：http://wap.sjlbkw.cn/Article/details/gyqmvxteg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fktsv.cn/Article/details/gbvunibwr.sHtML

[R47] sed 单行替换
来源：http://m.share.epnwcf.com/Article/details/gpyqwyaiv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/ggsdswqhb.sHtML

[R48] awk 取指定列
来源：http://mobile.fktsv.cn/Article/details/ggihgikfc.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.bbcook.cn/Article/details/gvbstqtek.sHtML

[R49] awk 带条件
来源：http://read.share.vehdjk.com/Article/details/gluvojqjr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.tarul.cn/Article/details/gthusucxt.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/gsatiqczn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.tarul.cn/Article/details/gtkjznftz.sHtML

[R51] 排序去重取前几
来源：http://www.blog.yfazqb.com/Article/details/gydjnlcrc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fktsv.cn/Article/details/gtxhpooux.sHtML

[R52] 统计行数
来源：http://blog.fktsv.cn/Article/details/gokhtsnda.sHtML

wc -l a.txt
来源：http://baike.bbcook.cn/Article/details/gbnzojzrw.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fktsv.cn/Article/details/gdslphynj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fktsv.cn/Article/details/ggssjzkfg.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/gbqjssyiu.sHtML

diff a.txt b.txt
来源：http://baike.epnwcf.com/Article/details/ghxozumbg.sHtML

[R55] 压缩与解压
来源：http://www.m.share.bbcook.cn/Article/details/gdiojnwae.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.sjlbkw.cn/Article/details/gtsettvly.sHtML

[R56] 远程拷贝
来源：http://3g.epnwcf.com/Article/details/gnoxcynwc.sHtML

scp file user@host:/path/
来源：http://www.blog.vehdjk.com/Article/details/golnihhuu.sHtML

[R57] 远程执行命令
来源：http://www.m.share.epnwcf.com/Article/details/gieddvlfx.sHtML

ssh user@host 'uptime'
来源：http://blog.bbcook.cn/Article/details/gfxpajzey.sHtML

[R58] 下载文件
来源：http://www.m.share.yfazqb.com/Article/details/gbgcoshqj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.sjlbkw.cn/Article/details/gyyqdiujn.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/ghboiscit.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.yfazqb.com/Article/details/gzkiysycz.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/gpnmoxpbx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.epnwcf.com/Article/details/gmiajrmbw.sHtML

[R61] 磁盘占用
来源：http://m.share.yfazqb.com/Article/details/gdfrytumu.sHtML

df -h;  du -sh *
来源：http://www.share.yfazqb.com/Article/details/gqgzobxtx.sHtML

[R62] 找最占空间的文件
来源：http://wap.yfazqb.com/Article/details/gzpsxcsaj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.tarul.cn/Article/details/gntcjgfjk.sHtML

[R63] 内存与进程
来源：http://wap.fktsv.cn/Article/details/gzjmaiuzm.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fktsv.cn/Article/details/gjtmpxvmv.sHtML

[R64] 结束进程
来源：http://read.share.fktsv.cn/Article/details/gkcxqvfmu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.epnwcf.com/Article/details/gayhiyfeb.sHtML

[R65] 查看端口占用
来源：http://3g.sjlbkw.cn/Article/details/gqvretwip.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gihpfzyag.sHtML

[R66] 定时任务
来源：http://wap.bbcook.cn/Article/details/grbrqiwkw.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fktsv.cn/Article/details/gtjstuhme.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/gizrhwcby.sHtML

openssl rand -hex 16
来源：http://mobile.tarul.cn/Article/details/gonqovbug.sHtML

[R68] 计算文件校验值
来源：http://read.share.tarul.cn/Article/details/gixftkbbt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gaanixybq.sHtML

[R69] 生成随机密码
来源：http://mobile.fktsv.cn/Article/details/glsogflwh.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/ghyghzpiy.sHtML

[R70] 时间戳与互转
来源：http://read.share.vehdjk.com/Article/details/glldznmbd.sHtML

date +%s;  date -d @1700000000
来源：http://wap.tarul.cn/Article/details/gmyqsmfvb.sHtML

[R71] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/gfbqbqnrw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.epnwcf.com/Article/details/gddskaqaw.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gkelavgew.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gtjpvicbq.sHtML

[R73] 分割大日志
来源：http://3g.fktsv.cn/Article/details/gqueqyfhl.sHtML

split -l 1000 big.log part_
来源：http://3g.vehdjk.com/Article/details/gxvratenx.sHtML

[R74] 批量重命名
来源：http://blog.sjlbkw.cn/Article/details/ghgggxits.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/glkfxgddu.sHtML

[R75] 导出环境变量
来源：http://wap.sjlbkw.cn/Article/details/gserevlnm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.yfazqb.com/Article/details/gpfgwtnph.sHtML

[R76] 使用临时文件
来源：http://mobile.fktsv.cn/Article/details/geyqflrsm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gigubetwr.sHtML

[R77] 读取用户输入
来源：http://m.share.vehdjk.com/Article/details/gmzxzsldj.sHtML

read -rp "请输入: " ans
来源：http://wap.yfazqb.com/Article/details/gtzxrqflp.sHtML

[R78] 交互式菜单
来源：http://baike.vehdjk.com/Article/details/gouldcgvq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fktsv.cn/Article/details/gcjfzsdmo.sHtML

[R79] 解析命令行选项
来源：http://3g.yfazqb.com/Article/details/grmeovsnh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.sjlbkw.cn/Article/details/ghuqjsgsh.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gtjjuxswh.sHtML

time ./run.sh
来源：http://read.share.yfazqb.com/Article/details/gvhyikxal.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggodaawzz.sHtML

S. C / C++ 专题
来源：http://blog.epnwcf.com/Article/details/gamttyyjd.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gdzhkizli.sHtML

[S01] C：Hello World
来源：http://3g.epnwcf.com/Article/details/gxzbfpyqs.sHtML

#include <stdio.h>
来源：http://www.m.share.sjlbkw.cn/Article/details/gznrmezzi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.yfazqb.com/Article/details/gnnolyqsz.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.tarul.cn/Article/details/gkvnkrsfc.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fktsv.cn/Article/details/gpyjvfqjo.sHtML

[S03] C：读入整数
来源：http://mobile.yfazqb.com/Article/details/gvgdwyhco.sHtML

int x; scanf("%d", &x);
来源：http://read.share.vehdjk.com/Article/details/gyixlddhh.sHtML

[S04] C：字符串复制
来源：http://baike.yfazqb.com/Article/details/gzronhsxo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.tarul.cn/Article/details/gvywhkaxc.sHtML

[S05] C：字符串长度
来源：http://read.share.bbcook.cn/Article/details/gwhfshbtr.sHtML

strlen(s)
来源：http://baike.fktsv.cn/Article/details/gwfivornz.sHtML

[S06] C：字符串比较
来源：http://3g.yfazqb.com/Article/details/gdraauvwi.sHtML

strcmp(a, b) == 0
来源：http://read.share.epnwcf.com/Article/details/gcgyidtyi.sHtML

[S07] C：数组遍历求和
来源：http://3g.tarul.cn/Article/details/gfrnemcvi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.tarul.cn/Article/details/golttxduf.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.vehdjk.com/Article/details/gbsaidgkm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.epnwcf.com/Article/details/gegcbwiyw.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.yfazqb.com/Article/details/ghzflrcqw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fktsv.cn/Article/details/gsszxrjwg.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/giowjmhrl.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.epnwcf.com/Article/details/gbfurdjer.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gybxkzaxq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fktsv.cn/Article/details/gpgnngyll.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fktsv.cn/Article/details/gpvrapaiu.sHtML

fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gsxxmztcs.sHtML

[S12] C：写文件
来源：http://m.share.vehdjk.com/Article/details/gczegkywk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fktsv.cn/Article/details/glwkorysi.sHtML

[S13] C：宏定义
来源：http://mobile.vehdjk.com/Article/details/glmqmsbpf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.sjlbkw.cn/Article/details/gbqocjoyj.sHtML

[S14] C：枚举
来源：http://wap.fktsv.cn/Article/details/gxrkllizs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.yfazqb.com/Article/details/genissopy.sHtML

[S15] C：类型转换
来源：http://m.share.bbcook.cn/Article/details/gzyktoula.sHtML

(double) a / b
来源：http://read.share.sjlbkw.cn/Article/details/gesalpsbf.sHtML

[S16] C：位操作置位
来源：http://wap.sjlbkw.cn/Article/details/gknasmrxz.sHtML

x |= (1 << 3);
来源：http://mobile.yfazqb.com/Article/details/gngvswrgf.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gyijeoifn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.sjlbkw.cn/Article/details/gkdgtqxjy.sHtML

[S18] C：命令行参数
来源：http://read.share.fktsv.cn/Article/details/glzqfxxrk.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gqjidnrlm.sHtML

[S19] C：快速排序
来源：http://blog.yfazqb.com/Article/details/gnnuvtwad.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gbxnidyrd.sHtML

[S20] C：二分查找
来源：http://3g.fktsv.cn/Article/details/gzaijvqta.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gqpukgver.sHtML

[S21] C：字符类别判断
来源：http://www.share.epnwcf.com/Article/details/gqaurqfjc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.yfazqb.com/Article/details/gtnyzuafl.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/gzofckihl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.tarul.cn/Article/details/gxohqjhfs.sHtML

[S23] C：随机数
来源：http://mobile.tarul.cn/Article/details/goxustrpn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.bbcook.cn/Article/details/grappmmgi.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.tarul.cn/Article/details/gngfblbxf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/glftiedcd.sHtML

[S25] C：内存拷贝
来源：http://wap.sjlbkw.cn/Article/details/gxqwufxjx.sHtML

memcpy(dst, src, n);
来源：http://3g.yfazqb.com/Article/details/gjwxngvhi.sHtML

[S26] C：内存清零
来源：http://www.m.share.vehdjk.com/Article/details/gcafywenc.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gjkpgndht.sHtML

[S27] C：定义常量
来源：http://www.blog.bbcook.cn/Article/details/gxfqyiquv.sHtML

const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gckbzyqtp.sHtML

[S28] C：静态变量
来源：http://www.blog.tarul.cn/Article/details/gzdrgwpbt.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gnlknvdad.sHtML

[S29] C：变参函数
来源：http://wap.bbcook.cn/Article/details/gyzlybcsh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.vehdjk.com/Article/details/galfxuwpi.sHtML

[S30] C：头文件保护
来源：http://baike.tarul.cn/Article/details/guouatole.sHtML

#ifndef X_H
来源：http://www.share.epnwcf.com/Article/details/gvgwhcavu.sHtML

#define X_H
来源：http://baike.yfazqb.com/Article/details/gtufyaqtu.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/gkqhpxmib.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/gzhzfmajv.sHtML

#include <iostream>
来源：http://baike.bbcook.cn/Article/details/gfzonsukt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.bbcook.cn/Article/details/ggefpvlxq.sHtML

[S32] C++：字符串
来源：http://www.m.share.fktsv.cn/Article/details/gdpmkwgjx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fktsv.cn/Article/details/goyqgczeq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.vehdjk.com/Article/details/gtdlorlfi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fktsv.cn/Article/details/gwivclmhg.sHtML

[S34] C++：遍历 vector
来源：http://baike.vehdjk.com/Article/details/gadptlenr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.tarul.cn/Article/details/gtlboftbh.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/gfekrqgyi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gqcbsketx.sHtML

[S36] C++：unordered_map
来源：http://www.share.sjlbkw.cn/Article/details/ghqsntohv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/gbcnsftos.sHtML

[S37] C++：set
来源：http://m.share.vehdjk.com/Article/details/gljvidzks.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.vehdjk.com/Article/details/gvkgksraf.sHtML

[S38] C++：排序
来源：http://www.m.share.tarul.cn/Article/details/gmqonwwak.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.bbcook.cn/Article/details/gdnxiyeif.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.sjlbkw.cn/Article/details/gmwmokmwv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.bbcook.cn/Article/details/gakfwnldk.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/gywezqimj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/gzehfrxst.sHtML

[S41] C++：类与构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gsbgexdmw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.epnwcf.com/Article/details/gvsoqrfvn.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.sjlbkw.cn/Article/details/grztzvewc.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.epnwcf.com/Article/details/gvglvophn.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuprwnqr.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.tarul.cn/Article/details/gzcgyokae.sHtML

[S44] C++：引用传参
来源：http://baike.vehdjk.com/Article/details/gniwbfihj.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.epnwcf.com/Article/details/guvzdrums.sHtML

[S45] C++：lambda
来源：http://www.m.share.bbcook.cn/Article/details/gtvzwduhf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.epnwcf.com/Article/details/gfwjjexbx.sHtML

[S46] C++：函数模板
来源：http://m.share.sjlbkw.cn/Article/details/gxzmmoqdn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.tarul.cn/Article/details/gnolqjhck.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.yfazqb.com/Article/details/ghmyvynoq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/gnzipeiri.sHtML

[S48] C++：逐行读文件
来源：http://read.share.tarul.cn/Article/details/goxajjzan.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.tarul.cn/Article/details/gbbofqssu.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.tarul.cn/Article/details/gfkovmutp.sHtML

[S49] C++：写文件
来源：http://m.share.fktsv.cn/Article/details/geajbpbja.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/gpecbeden.sHtML

[S50] C++：格式化数字
来源：http://m.share.epnwcf.com/Article/details/grgevydmb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gzhazdpun.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/godbwvwfz.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/gxvtsrqvx.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.tarul.cn/Article/details/ggfawutxx.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fktsv.cn/Article/details/gfvgdusir.sHtML

[S53] C++：移动语义
来源：http://wap.bbcook.cn/Article/details/gmjmraboy.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.sjlbkw.cn/Article/details/gndlgnnzi.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fktsv.cn/Article/details/gxzdsvubr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.sjlbkw.cn/Article/details/gefamklib.sHtML

[S55] C++：结构化绑定
来源：http://3g.bbcook.cn/Article/details/gorowhvue.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.yfazqb.com/Article/details/gtdjsjczw.sHtML

[S56] C++：optional
来源：http://www.share.sjlbkw.cn/Article/details/gdmrgsqax.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.bbcook.cn/Article/details/gkpkdmohg.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fktsv.cn/Article/details/gqlzgaeev.sHtML

constexpr int N = 10;
来源：http://www.share.yfazqb.com/Article/details/gyatjdhdv.sHtML

[S58] C++：命名空间
来源：http://wap.bbcook.cn/Article/details/gfiqpuzgt.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/gtqillnkr.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fktsv.cn/Article/details/gggqvosdd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.yfazqb.com/Article/details/gfeodqhfs.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gyscpeaja.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fktsv.cn/Article/details/gvfwcaxrx.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gdcpmkxnx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.sjlbkw.cn/Article/details/griywlvmk.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gviywclmq.sHtML

[T01] Kotlin：Hello World
来源：http://baike.bbcook.cn/Article/details/gzllapmpz.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gfzrsfrhz.sHtML

[T02] Kotlin：变量
来源：http://m.share.bbcook.cn/Article/details/guhwxusfk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.epnwcf.com/Article/details/glfswuqii.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.yfazqb.com/Article/details/gqjyqntjy.sHtML

"值: $b"
来源：http://baike.vehdjk.com/Article/details/grmyyfwvc.sHtML

[T04] Kotlin：空安全
来源：http://wap.sjlbkw.cn/Article/details/gfflayduj.sHtML

val n: String? = null;  n?.length
来源：http://wap.sjlbkw.cn/Article/details/gxmjwmhbf.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fktsv.cn/Article/details/gilvwkrcx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.bbcook.cn/Article/details/gbainxobs.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fktsv.cn/Article/details/gnrpffjow.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.epnwcf.com/Article/details/gkuomvjjf.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.epnwcf.com/Article/details/ghqmveglp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fktsv.cn/Article/details/gvmydyffy.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.yfazqb.com/Article/details/gcfnlwcro.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.sjlbkw.cn/Article/details/grxpnicav.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.epnwcf.com/Article/details/gzekxzook.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.sjlbkw.cn/Article/details/ghxjvwclm.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.tarul.cn/Article/details/gvuxwdbmb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fktsv.cn/Article/details/ghjynliyc.sHtML

[T11] Kotlin：协程
来源：http://baike.sjlbkw.cn/Article/details/gmsnlgkdz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.vehdjk.com/Article/details/gkovyaeix.sHtML

[T12] Kotlin：解构声明
来源：http://wap.sjlbkw.cn/Article/details/gzrskueuj.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gwuqbyupd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/gjpkclqjd.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.epnwcf.com/Article/details/gpipxspxe.sHtML

[T14] Kotlin：循环
来源：http://wap.epnwcf.com/Article/details/gtftuodam.sHtML

for (i in 1..10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gqukuyjhk.sHtML

[T15] Kotlin：接口
来源：http://www.share.tarul.cn/Article/details/gcgkwmnyo.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.tarul.cn/Article/details/gqnbamlnu.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gkzynmhct.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/gxvqjuegu.sHtML

[T17] Swift：变量与常量
来源：http://wap.vehdjk.com/Article/details/gllameipd.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gxbwcciad.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gmgixtkoq.sHtML

"值: \(b)"
来源：http://read.share.yfazqb.com/Article/details/geflilzhs.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/gsagaotah.sHtML

if let n = opt { print(n) }
来源：http://baike.tarul.cn/Article/details/gqecfdvif.sHtML

[T20] Swift：数组操作
来源：http://wap.sjlbkw.cn/Article/details/ggjovkroo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.bbcook.cn/Article/details/gppptuxsc.sHtML

[T21] Swift：遍历
来源：http://blog.fktsv.cn/Article/details/gqranbhji.sHtML

for x in a { print(x) }
来源：http://wap.sjlbkw.cn/Article/details/gcsobmlpv.sHtML

[T22] Swift：字典
来源：http://blog.sjlbkw.cn/Article/details/gexohlymf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.epnwcf.com/Article/details/gvhshztdl.sHtML

[T23] Swift：函数
来源：http://blog.vehdjk.com/Article/details/gkopdwkgu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.vehdjk.com/Article/details/gffdzzmyq.sHtML

[T24] Swift：闭包
来源：http://www.blog.epnwcf.com/Article/details/ghfmrplbo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gckycpwlb.sHtML

[T25] Swift：结构体
来源：http://www.blog.fktsv.cn/Article/details/giaurijog.sHtML

struct P { var x: Int }
来源：http://www.m.share.vehdjk.com/Article/details/gedctdhrh.sHtML

[T26] Swift：类与重写
来源：http://3g.epnwcf.com/Article/details/gwkpnmwdw.sHtML

class A: Base { override func f() {} }
来源：http://blog.fktsv.cn/Article/details/gmdspcpqk.sHtML

[T27] Swift：错误处理
来源：http://wap.vehdjk.com/Article/details/gyiuqsynn.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.vehdjk.com/Article/details/gsdghqzek.sHtML

[T28] Swift：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gzzncliye.sHtML

enum Color { case red, green }
来源：http://wap.yfazqb.com/Article/details/gkzmjjyaz.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.tarul.cn/Article/details/gcnhwwsxh.sHtML

guard let x = opt else { return }
来源：http://3g.tarul.cn/Article/details/gjuzmragz.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/grqhudcwe.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.epnwcf.com/Article/details/gpefnwmqm.sHtML

[T31] Lua：Hello World
来源：http://wap.vehdjk.com/Article/details/gvsqjtkhq.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gqhakxuck.sHtML

[T32] Lua：局部变量
来源：http://3g.tarul.cn/Article/details/gvhvhvtjz.sHtML

local a = 1
来源：http://baike.epnwcf.com/Article/details/gkfjajrze.sHtML

[T33] Lua：表（数组）
来源：http://m.share.epnwcf.com/Article/details/gucxfpjkj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.epnwcf.com/Article/details/gquxyaujc.sHtML

[T34] Lua：遍历表
来源：http://www.share.epnwcf.com/Article/details/gubgadbbm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.vehdjk.com/Article/details/gadzqhclg.sHtML

[T35] Lua：字典表
来源：http://www.blog.epnwcf.com/Article/details/gndzioxrz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.tarul.cn/Article/details/gxlzsaetb.sHtML

[T36] Lua：函数
来源：http://baike.yfazqb.com/Article/details/gudnqrlyo.sHtML

function add(a, b) return a + b end
来源：http://mobile.fktsv.cn/Article/details/gmanklgsx.sHtML

[T37] Lua：字符串拼接
来源：http://blog.bbcook.cn/Article/details/gphcxxbpe.sHtML

"a" .. "b"
来源：http://blog.fktsv.cn/Article/details/gekbgqvqj.sHtML

[T38] Lua：条件
来源：http://www.share.yfazqb.com/Article/details/giakrdhze.sHtML

if x > 0 then print("正") end
来源：http://3g.tarul.cn/Article/details/goulksfll.sHtML


<!-- 参考信息 -->