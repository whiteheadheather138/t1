代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://read.share.yfazqb.com/Article/details/gqzcgsnni.sHtML

[R32] 参数个数校验
来源：http://3g.vehdjk.com/Article/details/gcysbrgeh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyfwgeyev.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.tarul.cn/Article/details/gdnrkxfqr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.sjlbkw.cn/Article/details/gizbiyrow.sHtML

[R34] 退出时清理
来源：http://www.share.tarul.cn/Article/details/gwruutahf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/gfypciuvc.sHtML

[R35] 后台执行并等待
来源：http://m.share.yfazqb.com/Article/details/gbiimtsiq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.bbcook.cn/Article/details/gxjinapzr.sHtML

[R36] 并发执行多个任务
来源：http://3g.yfazqb.com/Article/details/gwgrwruzq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fktsv.cn/Article/details/glboisngn.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.yfazqb.com/Article/details/gdzifhuom.sHtML

files=$(ls -1)
来源：http://mobile.yfazqb.com/Article/details/glfowxigy.sHtML

[R38] 管道串联
来源：http://3g.sjlbkw.cn/Article/details/gbishfgev.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fktsv.cn/Article/details/ggciaqnqb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.yfazqb.com/Article/details/giquhklsl.sHtML

cmd > out.log 2>&1
来源：http://blog.vehdjk.com/Article/details/gipfzznbl.sHtML

[R40] 追加写日志
来源：http://mobile.yfazqb.com/Article/details/gmcrzsemc.sHtML

echo "log" >> out.log
来源：http://3g.vehdjk.com/Article/details/gdtdulblx.sHtML

[R41] 丢弃输出
来源：http://m.share.bbcook.cn/Article/details/gruczarkw.sHtML

cmd >/dev/null 2>&1
来源：http://wap.vehdjk.com/Article/details/gpdcmrhof.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gygqppbyq.sHtML

wc -l < a.txt
来源：http://baike.sjlbkw.cn/Article/details/gnmihgsya.sHtML

[R43] 按名字查找文件
来源：http://blog.vehdjk.com/Article/details/gtmsbcknd.sHtML

find . -name "*.log" -type f
来源：http://mobile.yfazqb.com/Article/details/gjjkgjocf.sHtML

[R44] 按修改时间查找
来源：http://m.share.fktsv.cn/Article/details/grhhtulkq.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gvkpjoxge.sHtML

[R45] 批量删除
来源：http://www.blog.yfazqb.com/Article/details/gpmdnzpjn.sHtML

find . -name "*.tmp" -delete
来源：http://wap.sjlbkw.cn/Article/details/gkzcjoaku.sHtML

[R46] 递归替换文件内容
来源：http://www.share.tarul.cn/Article/details/gxuckfffv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.sjlbkw.cn/Article/details/gnrcyuyzp.sHtML

[R47] sed 单行替换
来源：http://www.m.share.tarul.cn/Article/details/gickohwdq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.tarul.cn/Article/details/gpyshsrbd.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/gzhvwmnyb.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gijpgauct.sHtML

[R49] awk 带条件
来源：http://m.share.yfazqb.com/Article/details/gyrukylgn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.epnwcf.com/Article/details/gwbnlnqmb.sHtML

[R50] awk 求和
来源：http://m.share.epnwcf.com/Article/details/gvffwmbme.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gxyzgxsmv.sHtML

[R51] 排序去重取前几
来源：http://3g.tarul.cn/Article/details/gbeblccvm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.yfazqb.com/Article/details/gjihkuvda.sHtML

[R52] 统计行数
来源：http://www.share.vehdjk.com/Article/details/goffyjcdy.sHtML

wc -l a.txt
来源：http://baike.bbcook.cn/Article/details/gbzhcarcf.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gayivoebn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.epnwcf.com/Article/details/gjdjiqwfn.sHtML

[R54] 比较两个文件
来源：http://www.share.bbcook.cn/Article/details/gsrbxcuwv.sHtML

diff a.txt b.txt
来源：http://read.share.epnwcf.com/Article/details/ggzywqbxg.sHtML

[R55] 压缩与解压
来源：http://www.share.sjlbkw.cn/Article/details/gzmnbncvq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.epnwcf.com/Article/details/ggpsriopv.sHtML

[R56] 远程拷贝
来源：http://blog.vehdjk.com/Article/details/gzjlthzjd.sHtML

scp file user@host:/path/
来源：http://m.share.tarul.cn/Article/details/ghmkjmhgi.sHtML

[R57] 远程执行命令
来源：http://www.share.vehdjk.com/Article/details/gafqrlfkb.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.yfazqb.com/Article/details/gsxmqvhgl.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gevemygxd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fktsv.cn/Article/details/grmlrswav.sHtML

[R59] 发 POST JSON
来源：http://read.share.vehdjk.com/Article/details/gpfvuaylb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/gvngoudpg.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gyplalnsn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/gxsdkvkla.sHtML

[R61] 磁盘占用
来源：http://read.share.epnwcf.com/Article/details/gblqvukty.sHtML

df -h;  du -sh *
来源：http://www.share.vehdjk.com/Article/details/gbtvunrzc.sHtML

[R62] 找最占空间的文件
来源：http://baike.fktsv.cn/Article/details/gobrpkvhm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.epnwcf.com/Article/details/ggquftfeh.sHtML

[R63] 内存与进程
来源：http://3g.vehdjk.com/Article/details/ggqncbevl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/gqdosuval.sHtML

[R64] 结束进程
来源：http://blog.fktsv.cn/Article/details/gxwhfvdrw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.epnwcf.com/Article/details/gthluskwn.sHtML

[R65] 查看端口占用
来源：http://mobile.bbcook.cn/Article/details/gujqfgzxy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.sjlbkw.cn/Article/details/glekjvqwy.sHtML

[R66] 定时任务
来源：http://baike.epnwcf.com/Article/details/gapaojnwp.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/gucwkzwas.sHtML

[R67] 生成随机十六进制串
来源：http://blog.yfazqb.com/Article/details/gvxbyfcmt.sHtML

openssl rand -hex 16
来源：http://mobile.bbcook.cn/Article/details/gxszfkunp.sHtML

[R68] 计算文件校验值
来源：http://blog.yfazqb.com/Article/details/gghxnlvql.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gcuwisxhe.sHtML

[R69] 生成随机密码
来源：http://m.share.yfazqb.com/Article/details/gztlmmplt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/gyogtugwo.sHtML

[R70] 时间戳与互转
来源：http://wap.bbcook.cn/Article/details/gemixoowu.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.tarul.cn/Article/details/gtqdvypvs.sHtML

[R71] 日期格式化
来源：http://blog.yfazqb.com/Article/details/geamejaaz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/ggthnuztf.sHtML

[R72] 等待端口就绪
来源：http://blog.yfazqb.com/Article/details/gatstpsse.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gzhnmbgij.sHtML

[R73] 分割大日志
来源：http://www.blog.epnwcf.com/Article/details/gubnxvzjb.sHtML

split -l 1000 big.log part_
来源：http://m.share.tarul.cn/Article/details/gmuyxndbl.sHtML

[R74] 批量重命名
来源：http://baike.epnwcf.com/Article/details/gtadaqyzd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fktsv.cn/Article/details/gizucfmkr.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/gwuoawrat.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.sjlbkw.cn/Article/details/gxkinnjln.sHtML

[R76] 使用临时文件
来源：http://www.share.fktsv.cn/Article/details/gicisvfwn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gvfoetbdo.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/gloonoxdg.sHtML

read -rp "请输入: " ans
来源：http://baike.bbcook.cn/Article/details/gvwscnwkm.sHtML

[R78] 交互式菜单
来源：http://3g.vehdjk.com/Article/details/gedeqkzay.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.sjlbkw.cn/Article/details/geecnrfln.sHtML

[R79] 解析命令行选项
来源：http://3g.bbcook.cn/Article/details/guzldfeud.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.vehdjk.com/Article/details/gbbwvygua.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.vehdjk.com/Article/details/gszpnllcj.sHtML

time ./run.sh
来源：http://www.blog.fktsv.cn/Article/details/gleuwwzms.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/glcnuhzsp.sHtML

S. C / C++ 专题
来源：http://www.share.tarul.cn/Article/details/gwqrfscwa.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbjvjzey.sHtML

[S01] C：Hello World
来源：http://wap.epnwcf.com/Article/details/ghlslyeuy.sHtML

#include <stdio.h>
来源：http://wap.fktsv.cn/Article/details/gyuhivomx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.tarul.cn/Article/details/gvbjwqzhr.sHtML

[S02] C：变量与格式化输出
来源：http://3g.bbcook.cn/Article/details/gamymzavj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.sjlbkw.cn/Article/details/gtyrambhb.sHtML

[S03] C：读入整数
来源：http://3g.epnwcf.com/Article/details/gbmncvjxj.sHtML

int x; scanf("%d", &x);
来源：http://mobile.yfazqb.com/Article/details/gqdbfrzjw.sHtML

[S04] C：字符串复制
来源：http://wap.epnwcf.com/Article/details/gyahugzkp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.tarul.cn/Article/details/gnivjxkyl.sHtML

[S05] C：字符串长度
来源：http://m.share.epnwcf.com/Article/details/ggmacyiuw.sHtML

strlen(s)
来源：http://baike.fktsv.cn/Article/details/gjakkcpqh.sHtML

[S06] C：字符串比较
来源：http://m.share.tarul.cn/Article/details/gnlnlkobu.sHtML

strcmp(a, b) == 0
来源：http://www.share.yfazqb.com/Article/details/gcavdidfk.sHtML

[S07] C：数组遍历求和
来源：http://mobile.tarul.cn/Article/details/gdmdtfjeq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.vehdjk.com/Article/details/guatizfsz.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.vehdjk.com/Article/details/gdamrgnox.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.yfazqb.com/Article/details/ghuhaxect.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjegjizh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.vehdjk.com/Article/details/gubzgvuzi.sHtML

[S10] C：指针与解引用
来源：http://3g.fktsv.cn/Article/details/gadekumrt.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.vehdjk.com/Article/details/gccvpfdtl.sHtML

[S11] C：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gzknwlhmh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.epnwcf.com/Article/details/gtclkpjjs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.sjlbkw.cn/Article/details/gcknsdwrh.sHtML

fclose(f);
来源：http://m.share.tarul.cn/Article/details/gvzxxiean.sHtML

[S12] C：写文件
来源：http://m.share.yfazqb.com/Article/details/gayfddape.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/gjmmjpmgi.sHtML

[S13] C：宏定义
来源：http://wap.epnwcf.com/Article/details/gjlbdxwui.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.yfazqb.com/Article/details/gnesqtxqy.sHtML

[S14] C：枚举
来源：http://www.share.fktsv.cn/Article/details/gwbpswztb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.epnwcf.com/Article/details/ggfmvbixt.sHtML

[S15] C：类型转换
来源：http://m.share.epnwcf.com/Article/details/glwyeydoj.sHtML

(double) a / b
来源：http://www.m.share.vehdjk.com/Article/details/gtnbastof.sHtML

[S16] C：位操作置位
来源：http://3g.bbcook.cn/Article/details/gmdwmpuap.sHtML

x |= (1 << 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gffzppddm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/grrfzuvmu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/gflmrkfjz.sHtML

[S18] C：命令行参数
来源：http://3g.epnwcf.com/Article/details/ggdkythab.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.epnwcf.com/Article/details/gbrhbqfik.sHtML

[S19] C：快速排序
来源：http://www.blog.yfazqb.com/Article/details/gpwozpzyp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gnurssbye.sHtML

[S20] C：二分查找
来源：http://3g.bbcook.cn/Article/details/garlsjyrr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gjmzyxbzt.sHtML

[S21] C：字符类别判断
来源：http://m.share.tarul.cn/Article/details/gmpbhvthd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/gdkbdadgr.sHtML

[S22] C：字符串转数字
来源：http://read.share.vehdjk.com/Article/details/gfsknxmst.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.bbcook.cn/Article/details/gbnayfpww.sHtML

[S23] C：随机数
来源：http://mobile.yfazqb.com/Article/details/gtpadzntp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.sjlbkw.cn/Article/details/grnwauzzl.sHtML

[S24] C：获取本地时间
来源：http://read.share.bbcook.cn/Article/details/ghmzugdqk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.sjlbkw.cn/Article/details/gopwuxhja.sHtML

[S25] C：内存拷贝
来源：http://read.share.tarul.cn/Article/details/gjkcsvygf.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gqkwlvexm.sHtML

[S26] C：内存清零
来源：http://blog.tarul.cn/Article/details/giuoxvibh.sHtML

memset(a, 0, sizeof a);
来源：http://baike.sjlbkw.cn/Article/details/glyxarbou.sHtML

[S27] C：定义常量
来源：http://read.share.sjlbkw.cn/Article/details/gujtadpfu.sHtML

const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gvewhnwfv.sHtML

[S28] C：静态变量
来源：http://www.share.bbcook.cn/Article/details/gsortmwad.sHtML

static int counter = 0;
来源：http://blog.bbcook.cn/Article/details/gkwnovidp.sHtML

[S29] C：变参函数
来源：http://mobile.yfazqb.com/Article/details/gjpvytwgv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.vehdjk.com/Article/details/gzkpgejlz.sHtML

[S30] C：头文件保护
来源：http://m.share.sjlbkw.cn/Article/details/ghfistlch.sHtML

#ifndef X_H
来源：http://www.blog.epnwcf.com/Article/details/gvsfxpcxl.sHtML

#define X_H
来源：http://3g.vehdjk.com/Article/details/ghcsqveot.sHtML

#endif
来源：http://mobile.fktsv.cn/Article/details/gpsdpekfp.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gismyfqgv.sHtML

#include <iostream>
来源：http://www.blog.bbcook.cn/Article/details/gbgalqkyx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.sjlbkw.cn/Article/details/gyiflcyhi.sHtML

[S32] C++：字符串
来源：http://wap.bbcook.cn/Article/details/gcpgipwgi.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/gpigejsop.sHtML

[S33] C++：vector 增删
来源：http://baike.vehdjk.com/Article/details/gxrhiixzu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.bbcook.cn/Article/details/gjfkahsun.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.bbcook.cn/Article/details/gakifjxgu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.bbcook.cn/Article/details/gtchwaaho.sHtML

[S35] C++：map
来源：http://mobile.yfazqb.com/Article/details/gnghogdye.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gpykwltsv.sHtML

[S36] C++：unordered_map
来源：http://wap.tarul.cn/Article/details/gcqxxemoa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gqqlhucyo.sHtML

[S37] C++：set
来源：http://blog.vehdjk.com/Article/details/gvjawiwpu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.bbcook.cn/Article/details/groigyfmu.sHtML

[S38] C++：排序
来源：http://mobile.yfazqb.com/Article/details/gqtyujhwn.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.bbcook.cn/Article/details/ghktsxhny.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.epnwcf.com/Article/details/gacbchqrh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.sjlbkw.cn/Article/details/ghdbmrsdo.sHtML

[S40] C++：查找元素
来源：http://mobile.bbcook.cn/Article/details/glyplkvwl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.sjlbkw.cn/Article/details/gmcpgmfei.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.tarul.cn/Article/details/grerydxtq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fktsv.cn/Article/details/gcolhwmyv.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/gpduwmtur.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fktsv.cn/Article/details/ggkmwmxoc.sHtML

[S43] C++：智能指针
来源：http://baike.vehdjk.com/Article/details/gbgoanhjf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.vehdjk.com/Article/details/gcfdgjlyn.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/glrosszbh.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/goutbuvcx.sHtML

[S45] C++：lambda
来源：http://read.share.tarul.cn/Article/details/gpiylswjv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.sjlbkw.cn/Article/details/gufwhrsat.sHtML

[S46] C++：函数模板
来源：http://www.blog.vehdjk.com/Article/details/ghjlpwfay.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.tarul.cn/Article/details/gazsmenhp.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.sjlbkw.cn/Article/details/gxuuoxsbl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.tarul.cn/Article/details/gicgjgiex.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gvwgcrxfn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fktsv.cn/Article/details/ghijskfkd.sHtML

while (std::getline(in, line)) { }
来源：http://3g.vehdjk.com/Article/details/gdcxnoirw.sHtML

[S49] C++：写文件
来源：http://wap.bbcook.cn/Article/details/gcbvjneex.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/gycnhzeow.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.yfazqb.com/Article/details/gnhsuqiyd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.yfazqb.com/Article/details/gvdeozhvo.sHtML

[S51] C++：显式类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gedglbrdn.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.vehdjk.com/Article/details/gqshhpmcw.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.sjlbkw.cn/Article/details/gggnudifu.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.yfazqb.com/Article/details/gqxmgblnr.sHtML

[S53] C++：移动语义
来源：http://3g.tarul.cn/Article/details/ggslgeppa.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.vehdjk.com/Article/details/gsuotycrv.sHtML

[S54] C++：异常处理
来源：http://blog.vehdjk.com/Article/details/gjdybgfer.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.sjlbkw.cn/Article/details/gswgpzaoq.sHtML

[S55] C++：结构化绑定
来源：http://blog.fktsv.cn/Article/details/gzwpgdmse.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.bbcook.cn/Article/details/gxvvfauaz.sHtML

[S56] C++：optional
来源：http://mobile.vehdjk.com/Article/details/gasfcyufe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.epnwcf.com/Article/details/gfletivoi.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gtbwnjpgy.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/gjsudhjfd.sHtML

[S58] C++：命名空间
来源：http://blog.fktsv.cn/Article/details/gccuwbcjd.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.sjlbkw.cn/Article/details/gzrtmwdyr.sHtML

[S59] C++：静态断言
来源：http://www.share.tarul.cn/Article/details/ghodbhovn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fktsv.cn/Article/details/gqxqmkweq.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.yfazqb.com/Article/details/gugpypfbz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.tarul.cn/Article/details/gixcnxbsh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ggqzniccg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fktsv.cn/Article/details/gnhjpdvkm.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqboqzhro.sHtML

[T01] Kotlin：Hello World
来源：http://baike.yfazqb.com/Article/details/gseaadxsf.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gntcbdzxh.sHtML

[T02] Kotlin：变量
来源：http://baike.bbcook.cn/Article/details/ggrvvkqfd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.sjlbkw.cn/Article/details/gjjwqauxf.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fktsv.cn/Article/details/gtbufudvb.sHtML

"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/gljbtnpdj.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcxtscda.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.vehdjk.com/Article/details/gxayynqjl.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gvvnhxtlb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.epnwcf.com/Article/details/gqqvmvlto.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fktsv.cn/Article/details/gbowluhly.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gvskxzvmg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gzuyxixmb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fktsv.cn/Article/details/gcofhhpet.sHtML

[T08] Kotlin：数据类
来源：http://blog.epnwcf.com/Article/details/gxysijnsv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/glkoviuoi.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.vehdjk.com/Article/details/ggrudrteg.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fktsv.cn/Article/details/gkehgdvli.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.tarul.cn/Article/details/gjxtdlfiz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/gbbvglida.sHtML

[T11] Kotlin：协程
来源：http://wap.tarul.cn/Article/details/gqrqvajdt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fktsv.cn/Article/details/gazdtdtlz.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.sjlbkw.cn/Article/details/gqvpdbkms.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gwpdzmace.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.bbcook.cn/Article/details/gbghozfla.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.tarul.cn/Article/details/gdcriklvm.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gbbxedcen.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gtqncgpnl.sHtML

[T15] Kotlin：接口
来源：http://wap.fktsv.cn/Article/details/gqzjdtexp.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.epnwcf.com/Article/details/gjuskelpz.sHtML

[T16] Swift：Hello World
来源：http://read.share.bbcook.cn/Article/details/gcvpwxoup.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gebjgxlwr.sHtML

[T17] Swift：变量与常量
来源：http://www.share.bbcook.cn/Article/details/gppglqecd.sHtML

var a = 1;  let b = 2
来源：http://m.share.vehdjk.com/Article/details/gosmmknpt.sHtML

[T18] Swift：字符串插值
来源：http://3g.fktsv.cn/Article/details/gmyclrhai.sHtML

"值: \(b)"
来源：http://blog.sjlbkw.cn/Article/details/gzsodvfmq.sHtML

[T19] Swift：可选绑定
来源：http://baike.bbcook.cn/Article/details/gtlqdkioe.sHtML

if let n = opt { print(n) }
来源：http://read.share.vehdjk.com/Article/details/griqqbqet.sHtML

[T20] Swift：数组操作
来源：http://mobile.vehdjk.com/Article/details/giqyazasu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/gphhtynkv.sHtML

[T21] Swift：遍历
来源：http://www.m.share.epnwcf.com/Article/details/gplocywvj.sHtML

for x in a { print(x) }
来源：http://wap.sjlbkw.cn/Article/details/grcdfznuz.sHtML

[T22] Swift：字典
来源：http://www.blog.fktsv.cn/Article/details/grgvgbdpm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.tarul.cn/Article/details/gnfopajto.sHtML

[T23] Swift：函数
来源：http://www.share.tarul.cn/Article/details/goigccrlj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.tarul.cn/Article/details/gyqrjjtdj.sHtML

[T24] Swift：闭包
来源：http://m.share.epnwcf.com/Article/details/glflszpkl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gnaktqglr.sHtML

[T25] Swift：结构体
来源：http://m.share.yfazqb.com/Article/details/gmcfhvuuy.sHtML

struct P { var x: Int }
来源：http://m.share.bbcook.cn/Article/details/gaccecyie.sHtML

[T26] Swift：类与重写
来源：http://m.share.tarul.cn/Article/details/gsdczwrfn.sHtML

class A: Base { override func f() {} }
来源：http://baike.epnwcf.com/Article/details/gvqoowrpy.sHtML

[T27] Swift：错误处理
来源：http://m.share.vehdjk.com/Article/details/gbnytnbgx.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fktsv.cn/Article/details/gfzuzgxfx.sHtML

[T28] Swift：枚举
来源：http://wap.tarul.cn/Article/details/gaajgfqpe.sHtML

enum Color { case red, green }
来源：http://www.m.share.epnwcf.com/Article/details/gmtnkmema.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.yfazqb.com/Article/details/gwtvfidam.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gpftxqvti.sHtML

[T30] Swift：协议
来源：http://wap.sjlbkw.cn/Article/details/gvriilzyb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fktsv.cn/Article/details/gbijsozwu.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gcseogotz.sHtML

print("Hello")
来源：http://www.share.tarul.cn/Article/details/gjckivffu.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gvrfoscpp.sHtML

local a = 1
来源：http://mobile.sjlbkw.cn/Article/details/gfrlyifrw.sHtML

[T33] Lua：表（数组）
来源：http://wap.sjlbkw.cn/Article/details/gejhoxykl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.sjlbkw.cn/Article/details/gsxccxyzy.sHtML

[T34] Lua：遍历表
来源：http://blog.vehdjk.com/Article/details/gepvicfvg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.tarul.cn/Article/details/gipzwxxon.sHtML


<!-- 参考信息 -->