代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.share.tarul.cn/Article/details/gjgdtyzme.sHtML

[R32] 参数个数校验
来源：http://wap.bbcook.cn/Article/details/gqwienxme.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdtssqny.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.sjlbkw.cn/Article/details/gnpgzqzkz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.epnwcf.com/Article/details/ghfjmjdbo.sHtML

[R34] 退出时清理
来源：http://blog.fktsv.cn/Article/details/grvsjhvds.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.vehdjk.com/Article/details/gtccdviwo.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/gsxtyfciu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.tarul.cn/Article/details/gaomnoskn.sHtML

[R36] 并发执行多个任务
来源：http://wap.vehdjk.com/Article/details/gtaluovzx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.vehdjk.com/Article/details/gsabsnrba.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.yfazqb.com/Article/details/gxrkdslrd.sHtML

files=$(ls -1)
来源：http://wap.bbcook.cn/Article/details/ghlzrzwyt.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gjfxjczwp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.vehdjk.com/Article/details/gswbicsss.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.tarul.cn/Article/details/gkrrfxaqa.sHtML

cmd > out.log 2>&1
来源：http://read.share.yfazqb.com/Article/details/gsjadhgou.sHtML

[R40] 追加写日志
来源：http://read.share.yfazqb.com/Article/details/gzzwehoxk.sHtML

echo "log" >> out.log
来源：http://mobile.yfazqb.com/Article/details/gmlypxufj.sHtML

[R41] 丢弃输出
来源：http://3g.bbcook.cn/Article/details/gwbtvkdmf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/gjvbbzxsz.sHtML

[R42] 输入重定向
来源：http://www.share.bbcook.cn/Article/details/gdlhcexbb.sHtML

wc -l < a.txt
来源：http://www.share.fktsv.cn/Article/details/glqlmgrxq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.sjlbkw.cn/Article/details/gazfbcfud.sHtML

find . -name "*.log" -type f
来源：http://mobile.yfazqb.com/Article/details/gvljeuzxh.sHtML

[R44] 按修改时间查找
来源：http://wap.sjlbkw.cn/Article/details/gadzwfnwd.sHtML

find . -mtime -7 -type f
来源：http://3g.tarul.cn/Article/details/gjndtwasf.sHtML

[R45] 批量删除
来源：http://blog.tarul.cn/Article/details/gajvmopya.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.epnwcf.com/Article/details/gocwddtgz.sHtML

[R46] 递归替换文件内容
来源：http://wap.yfazqb.com/Article/details/gqzvarfsz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.yfazqb.com/Article/details/gdhcttuxw.sHtML

[R47] sed 单行替换
来源：http://blog.yfazqb.com/Article/details/gddnqtmpc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fktsv.cn/Article/details/gbpmyldpj.sHtML

[R48] awk 取指定列
来源：http://www.share.tarul.cn/Article/details/gtxmzyjer.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gpyhhalnf.sHtML

[R49] awk 带条件
来源：http://www.m.share.fktsv.cn/Article/details/gmzjvnkyl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/gumbioxiq.sHtML

[R50] awk 求和
来源：http://read.share.vehdjk.com/Article/details/gtjbnqxzr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.tarul.cn/Article/details/gjbrqiwks.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/gmwoyjgrx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.bbcook.cn/Article/details/gzpkxwspd.sHtML

[R52] 统计行数
来源：http://www.blog.yfazqb.com/Article/details/glsllqvwg.sHtML

wc -l a.txt
来源：http://3g.bbcook.cn/Article/details/gbojkcsom.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.tarul.cn/Article/details/glscihald.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.vehdjk.com/Article/details/gonaeyryy.sHtML

[R54] 比较两个文件
来源：http://wap.vehdjk.com/Article/details/gubjjcnxi.sHtML

diff a.txt b.txt
来源：http://3g.sjlbkw.cn/Article/details/guavjokxw.sHtML

[R55] 压缩与解压
来源：http://3g.fktsv.cn/Article/details/gwqpqmrgf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/goecockbj.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/gmlqbavqm.sHtML

scp file user@host:/path/
来源：http://www.blog.tarul.cn/Article/details/gunpwaekv.sHtML

[R57] 远程执行命令
来源：http://baike.vehdjk.com/Article/details/gwkyxezig.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/gzszhvzws.sHtML

[R58] 下载文件
来源：http://mobile.vehdjk.com/Article/details/gezqrgtcc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.yfazqb.com/Article/details/gdodmppvn.sHtML

[R59] 发 POST JSON
来源：http://blog.yfazqb.com/Article/details/ggctaicpw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.vehdjk.com/Article/details/gzsemutuu.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/glzpwqmzn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.epnwcf.com/Article/details/gpifktpad.sHtML

[R61] 磁盘占用
来源：http://www.blog.bbcook.cn/Article/details/gpprjnxja.sHtML

df -h;  du -sh *
来源：http://wap.tarul.cn/Article/details/gckyqxojx.sHtML

[R62] 找最占空间的文件
来源：http://m.share.bbcook.cn/Article/details/glugtxpfp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.tarul.cn/Article/details/gjgvxstnp.sHtML

[R63] 内存与进程
来源：http://www.share.epnwcf.com/Article/details/gcpevcycc.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/gzflxoduf.sHtML

[R64] 结束进程
来源：http://baike.vehdjk.com/Article/details/gxyhbebjf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.bbcook.cn/Article/details/gwjhcxfku.sHtML

[R65] 查看端口占用
来源：http://3g.vehdjk.com/Article/details/grfymbuwr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.yfazqb.com/Article/details/gwugfcaux.sHtML

[R66] 定时任务
来源：http://www.m.share.yfazqb.com/Article/details/gzmbznkzf.sHtML

crontab -e;  crontab -l
来源：http://www.blog.epnwcf.com/Article/details/gylmonbyt.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.yfazqb.com/Article/details/gnewlhwuy.sHtML

openssl rand -hex 16
来源：http://mobile.vehdjk.com/Article/details/gkixbomjy.sHtML

[R68] 计算文件校验值
来源：http://www.blog.tarul.cn/Article/details/gllxxjevb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gcgntskjc.sHtML

[R69] 生成随机密码
来源：http://baike.vehdjk.com/Article/details/gmkzhhfwj.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.epnwcf.com/Article/details/gnujffvyh.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcgsbibb.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.yfazqb.com/Article/details/gthteahcs.sHtML

[R71] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/gvwxmcyvh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.vehdjk.com/Article/details/gzqeqzznr.sHtML

[R72] 等待端口就绪
来源：http://www.share.sjlbkw.cn/Article/details/goqhbxuwj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gejyhjybd.sHtML

[R73] 分割大日志
来源：http://m.share.bbcook.cn/Article/details/gknjcbzol.sHtML

split -l 1000 big.log part_
来源：http://blog.bbcook.cn/Article/details/gupclkgpi.sHtML

[R74] 批量重命名
来源：http://www.m.share.bbcook.cn/Article/details/glxkflswc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/ghdphvehq.sHtML

[R75] 导出环境变量
来源：http://www.blog.tarul.cn/Article/details/gnkopxmfj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.bbcook.cn/Article/details/gnexrvdaa.sHtML

[R76] 使用临时文件
来源：http://www.blog.epnwcf.com/Article/details/gvvyafwne.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gpjvihtcl.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/gwnpqkchy.sHtML

read -rp "请输入: " ans
来源：http://www.blog.tarul.cn/Article/details/gtnsxyjdk.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/grnpwftlf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.yfazqb.com/Article/details/gavvkolpr.sHtML

[R79] 解析命令行选项
来源：http://www.share.vehdjk.com/Article/details/glbzckdqf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.epnwcf.com/Article/details/ghuwrzphj.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.bbcook.cn/Article/details/gcrphielr.sHtML

time ./run.sh
来源：http://www.share.yfazqb.com/Article/details/gbbmixoip.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtibaaahm.sHtML

S. C / C++ 专题
来源：http://m.share.sjlbkw.cn/Article/details/gqyyrvqel.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gilypmcno.sHtML

[S01] C：Hello World
来源：http://baike.tarul.cn/Article/details/gepxpnayk.sHtML

#include <stdio.h>
来源：http://mobile.fktsv.cn/Article/details/gwcpwtafy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.tarul.cn/Article/details/gkxjxoyom.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gchmfkeud.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.vehdjk.com/Article/details/goyijyhpi.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/gjtomahma.sHtML

int x; scanf("%d", &x);
来源：http://mobile.bbcook.cn/Article/details/gjtlhhzxi.sHtML

[S04] C：字符串复制
来源：http://m.share.bbcook.cn/Article/details/geidbtjnn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gkvmreuwu.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gdzzjxbvu.sHtML

strlen(s)
来源：http://blog.fktsv.cn/Article/details/gdvmlille.sHtML

[S06] C：字符串比较
来源：http://3g.yfazqb.com/Article/details/gsikrovju.sHtML

strcmp(a, b) == 0
来源：http://mobile.vehdjk.com/Article/details/gjadkdjjs.sHtML

[S07] C：数组遍历求和
来源：http://baike.vehdjk.com/Article/details/gosmiuzvd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.yfazqb.com/Article/details/grknybsaa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.vehdjk.com/Article/details/gpgevjgba.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.vehdjk.com/Article/details/gqujlqiwp.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.yfazqb.com/Article/details/gwcsnoxww.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.bbcook.cn/Article/details/giinssgfz.sHtML

[S10] C：指针与解引用
来源：http://www.share.sjlbkw.cn/Article/details/gmkubobzk.sHtML

int *p = &a;  *p = 5;
来源：http://wap.bbcook.cn/Article/details/gnrxzkbfg.sHtML

[S11] C：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gtdkmtlsv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.tarul.cn/Article/details/gjggojxeh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.tarul.cn/Article/details/gfkkvmnab.sHtML

fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gormcbjkp.sHtML

[S12] C：写文件
来源：http://blog.yfazqb.com/Article/details/gszsoaebm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.vehdjk.com/Article/details/gzoumvfja.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/gpvqvocsv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.epnwcf.com/Article/details/gqdqmnpcd.sHtML

[S14] C：枚举
来源：http://www.m.share.tarul.cn/Article/details/ghthreuah.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.sjlbkw.cn/Article/details/ggvdqfccd.sHtML

[S15] C：类型转换
来源：http://3g.fktsv.cn/Article/details/gqeyiavzp.sHtML

(double) a / b
来源：http://www.blog.sjlbkw.cn/Article/details/gcaplvdfj.sHtML

[S16] C：位操作置位
来源：http://wap.yfazqb.com/Article/details/gnxkaacfz.sHtML

x |= (1 << 3);
来源：http://3g.yfazqb.com/Article/details/gvykbjlhh.sHtML

[S17] C：安全拼接字符串
来源：http://baike.epnwcf.com/Article/details/gyunwmwmv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fktsv.cn/Article/details/gvimjydie.sHtML

[S18] C：命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gcezckxhs.sHtML

int main(int argc, char **argv)
来源：http://read.share.tarul.cn/Article/details/gzpgcuavg.sHtML

[S19] C：快速排序
来源：http://3g.sjlbkw.cn/Article/details/gfvpfngpj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gxepjffnt.sHtML

[S20] C：二分查找
来源：http://3g.epnwcf.com/Article/details/gifbfzpxj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gqfiycwpf.sHtML

[S21] C：字符类别判断
来源：http://wap.epnwcf.com/Article/details/gptcahpmf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.yfazqb.com/Article/details/ggtolhgiv.sHtML

[S22] C：字符串转数字
来源：http://www.blog.sjlbkw.cn/Article/details/ggpskaypt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.epnwcf.com/Article/details/giopocefg.sHtML

[S23] C：随机数
来源：http://mobile.tarul.cn/Article/details/gkvdfqukh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.epnwcf.com/Article/details/gzehwhjbq.sHtML

[S24] C：获取本地时间
来源：http://baike.bbcook.cn/Article/details/gkymatmva.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.tarul.cn/Article/details/gxwtchcgk.sHtML

[S25] C：内存拷贝
来源：http://wap.yfazqb.com/Article/details/gdwpndqex.sHtML

memcpy(dst, src, n);
来源：http://3g.sjlbkw.cn/Article/details/gbuepzhym.sHtML

[S26] C：内存清零
来源：http://3g.sjlbkw.cn/Article/details/ggnziokeo.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fktsv.cn/Article/details/gqzntdmsj.sHtML

[S27] C：定义常量
来源：http://mobile.fktsv.cn/Article/details/gsurgnnaq.sHtML

const double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gjodfnrcr.sHtML

[S28] C：静态变量
来源：http://www.m.share.fktsv.cn/Article/details/gvozfpnoh.sHtML

static int counter = 0;
来源：http://www.share.fktsv.cn/Article/details/ghztuyccy.sHtML

[S29] C：变参函数
来源：http://mobile.tarul.cn/Article/details/gkhjwkfqh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.tarul.cn/Article/details/gfxwmzqrv.sHtML

[S30] C：头文件保护
来源：http://blog.tarul.cn/Article/details/gmoumoolb.sHtML

#ifndef X_H
来源：http://mobile.fktsv.cn/Article/details/gopcwchfu.sHtML

#define X_H
来源：http://read.share.tarul.cn/Article/details/gpcvhuxgs.sHtML

#endif
来源：http://www.m.share.fktsv.cn/Article/details/gbrfyndnf.sHtML

[S31] C++：Hello World
来源：http://wap.vehdjk.com/Article/details/gxsfhklok.sHtML

#include <iostream>
来源：http://3g.vehdjk.com/Article/details/gyhgiyuev.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.tarul.cn/Article/details/gpkuspcsc.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/gqydikbdt.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.bbcook.cn/Article/details/gxaxzgeks.sHtML

[S33] C++：vector 增删
来源：http://m.share.yfazqb.com/Article/details/gajevdqrl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.yfazqb.com/Article/details/gxnbcnntc.sHtML

[S34] C++：遍历 vector
来源：http://read.share.epnwcf.com/Article/details/gkqvikmjm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fktsv.cn/Article/details/gkjluaphj.sHtML

[S35] C++：map
来源：http://www.blog.epnwcf.com/Article/details/gxpalhbkl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gfuvtswao.sHtML

[S36] C++：unordered_map
来源：http://read.share.tarul.cn/Article/details/gfbwmjckz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gdjdwhdpz.sHtML

[S37] C++：set
来源：http://wap.yfazqb.com/Article/details/gisrtrcze.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/gtfpylnqi.sHtML

[S38] C++：排序
来源：http://www.blog.yfazqb.com/Article/details/gibvouhjg.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.vehdjk.com/Article/details/grstrawjj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.epnwcf.com/Article/details/gvsqoyjzc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.bbcook.cn/Article/details/giyizlwki.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/gpccgdpve.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.bbcook.cn/Article/details/gnejntjmf.sHtML

[S41] C++：类与构造函数
来源：http://www.share.yfazqb.com/Article/details/gdtrtgdmx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.bbcook.cn/Article/details/gvcbyyjtt.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fktsv.cn/Article/details/gqsqtakgk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.tarul.cn/Article/details/grdifzjfn.sHtML

[S43] C++：智能指针
来源：http://www.share.bbcook.cn/Article/details/gpczikdxw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.epnwcf.com/Article/details/gzbcwykuu.sHtML

[S44] C++：引用传参
来源：http://3g.vehdjk.com/Article/details/grfawtbtl.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fktsv.cn/Article/details/gdgkoqjhe.sHtML

[S45] C++：lambda
来源：http://mobile.vehdjk.com/Article/details/gvilvjsdz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.yfazqb.com/Article/details/gohraiooi.sHtML

[S46] C++：函数模板
来源：http://mobile.bbcook.cn/Article/details/gucmjmuuc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.sjlbkw.cn/Article/details/gjthsrrwb.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.epnwcf.com/Article/details/gmhczgifw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvenmqgbv.sHtML

[S48] C++：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/ghzgmniit.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.bbcook.cn/Article/details/gyemmcifc.sHtML

while (std::getline(in, line)) { }
来源：http://baike.tarul.cn/Article/details/gfqnrfitj.sHtML

[S49] C++：写文件
来源：http://read.share.fktsv.cn/Article/details/gsxhntaqc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.yfazqb.com/Article/details/gzbnfthfb.sHtML

[S50] C++：格式化数字
来源：http://wap.epnwcf.com/Article/details/gurztlphh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gzeujpbfv.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/gkftfbqvz.sHtML

static_cast<double>(a) / b
来源：http://3g.epnwcf.com/Article/details/gnyuiojar.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.epnwcf.com/Article/details/gkflrcuio.sHtML

int size() const noexcept { return n_; }
来源：http://wap.tarul.cn/Article/details/guxwqzjur.sHtML

[S53] C++：移动语义
来源：http://www.blog.vehdjk.com/Article/details/gilhetpiu.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.sjlbkw.cn/Article/details/ghokygcuh.sHtML

[S54] C++：异常处理
来源：http://www.m.share.epnwcf.com/Article/details/gujjfkrju.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fktsv.cn/Article/details/gqomnolzl.sHtML

[S55] C++：结构化绑定
来源：http://blog.bbcook.cn/Article/details/gxnabsemj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.bbcook.cn/Article/details/gkemqvmbb.sHtML

[S56] C++：optional
来源：http://mobile.vehdjk.com/Article/details/gvkkwkpqq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.bbcook.cn/Article/details/gmwwciqma.sHtML

[S57] C++：编译期常量
来源：http://read.share.bbcook.cn/Article/details/gyyttgjyr.sHtML

constexpr int N = 10;
来源：http://baike.sjlbkw.cn/Article/details/gsqiujjxw.sHtML

[S58] C++：命名空间
来源：http://3g.vehdjk.com/Article/details/gwkknfloa.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.sjlbkw.cn/Article/details/gbygajhgr.sHtML

[S59] C++：静态断言
来源：http://blog.tarul.cn/Article/details/gtekzuomw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.sjlbkw.cn/Article/details/gzikcehfa.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/gznolnzxu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gtemhgkpv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gyhpirawz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.bbcook.cn/Article/details/gupbjepna.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/geecdvgmg.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.vehdjk.com/Article/details/gcvvkdxvu.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gqkkbigga.sHtML

[T02] Kotlin：变量
来源：http://blog.fktsv.cn/Article/details/gnaramems.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fktsv.cn/Article/details/gtcjgliax.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.yfazqb.com/Article/details/gebwaulcs.sHtML

"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gsqeqcgjv.sHtML

[T04] Kotlin：空安全
来源：http://wap.sjlbkw.cn/Article/details/gfhbdugsm.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/gjosqrkyo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.vehdjk.com/Article/details/gfpmuuzxh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.sjlbkw.cn/Article/details/gglqgnvan.sHtML

[T06] Kotlin：集合映射
来源：http://baike.sjlbkw.cn/Article/details/goqrsxmvl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.vehdjk.com/Article/details/gmtymfmnf.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/gdwykfpam.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.tarul.cn/Article/details/gcppiifqf.sHtML

[T08] Kotlin：数据类
来源：http://www.share.vehdjk.com/Article/details/gwhatxrjs.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.tarul.cn/Article/details/ganqrdccy.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.sjlbkw.cn/Article/details/guhrnmuhi.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.yfazqb.com/Article/details/gtbnqazys.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fktsv.cn/Article/details/glubqhbnr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.yfazqb.com/Article/details/gywvuhaqj.sHtML

[T11] Kotlin：协程
来源：http://blog.yfazqb.com/Article/details/gomcijweg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fktsv.cn/Article/details/gkdgvxqio.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.tarul.cn/Article/details/gkugserxp.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.epnwcf.com/Article/details/gcszgjoqr.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fktsv.cn/Article/details/gcufguujo.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.yfazqb.com/Article/details/ggvsvklpf.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.epnwcf.com/Article/details/gszlcszbm.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gjowpoymd.sHtML

[T15] Kotlin：接口
来源：http://baike.yfazqb.com/Article/details/gkmabeilt.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.yfazqb.com/Article/details/gtdpjgnxl.sHtML

[T16] Swift：Hello World
来源：http://read.share.fktsv.cn/Article/details/grvstsbcb.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/grvnofaum.sHtML

[T17] Swift：变量与常量
来源：http://m.share.vehdjk.com/Article/details/ggjzezahc.sHtML

var a = 1;  let b = 2
来源：http://baike.yfazqb.com/Article/details/gxfboczxc.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gquskmrzw.sHtML

"值: \(b)"
来源：http://m.share.yfazqb.com/Article/details/gnemjcnvk.sHtML

[T19] Swift：可选绑定
来源：http://blog.tarul.cn/Article/details/grrwrbucy.sHtML

if let n = opt { print(n) }
来源：http://m.share.tarul.cn/Article/details/gqqixjuyf.sHtML

[T20] Swift：数组操作
来源：http://blog.sjlbkw.cn/Article/details/gvtoosxgp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.bbcook.cn/Article/details/gopzhszsy.sHtML

[T21] Swift：遍历
来源：http://3g.yfazqb.com/Article/details/ghihsnxzd.sHtML

for x in a { print(x) }
来源：http://m.share.sjlbkw.cn/Article/details/gaseslbhx.sHtML

[T22] Swift：字典
来源：http://wap.tarul.cn/Article/details/ghrcaejee.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.bbcook.cn/Article/details/geyxlzksb.sHtML

[T23] Swift：函数
来源：http://read.share.epnwcf.com/Article/details/gdozlttgu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.epnwcf.com/Article/details/gfunvteld.sHtML

[T24] Swift：闭包
来源：http://baike.fktsv.cn/Article/details/gmtoweszb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gvmftaupb.sHtML

[T25] Swift：结构体
来源：http://blog.vehdjk.com/Article/details/gqfbpixht.sHtML

struct P { var x: Int }
来源：http://read.share.tarul.cn/Article/details/gohcrwvhm.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.epnwcf.com/Article/details/gktawpvzh.sHtML

class A: Base { override func f() {} }
来源：http://blog.yfazqb.com/Article/details/gujjprpzs.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fktsv.cn/Article/details/glvtaycdi.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.bbcook.cn/Article/details/gjzpvowpe.sHtML

[T28] Swift：枚举
来源：http://read.share.fktsv.cn/Article/details/gvtqgrzpa.sHtML

enum Color { case red, green }
来源：http://wap.yfazqb.com/Article/details/gkkteeisq.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.yfazqb.com/Article/details/gvsfpupig.sHtML

guard let x = opt else { return }
来源：http://blog.sjlbkw.cn/Article/details/ggbzmsdtx.sHtML

[T30] Swift：协议
来源：http://mobile.sjlbkw.cn/Article/details/gghuonfkw.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fktsv.cn/Article/details/gvfqvsrfk.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gwzqpstqq.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/gljgjhwqd.sHtML

[T32] Lua：局部变量
来源：http://wap.bbcook.cn/Article/details/gombtlxar.sHtML

local a = 1
来源：http://www.m.share.epnwcf.com/Article/details/gvgkmspwi.sHtML

[T33] Lua：表（数组）
来源：http://mobile.yfazqb.com/Article/details/gxpcykaxn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.epnwcf.com/Article/details/gttdoeqcr.sHtML

[T34] Lua：遍历表
来源：http://baike.sjlbkw.cn/Article/details/gywzgqomj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.yfazqb.com/Article/details/glftrqrqx.sHtML


<!-- 参考信息 -->