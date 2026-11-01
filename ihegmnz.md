代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.bbcook.cn/Article/details/gaoxwserz.sHtML

[R30] 函数返回状态码
来源：http://www.share.fktsv.cn/Article/details/gzuioooab.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.epnwcf.com/Article/details/gzpxhmraz.sHtML

[R31] 局部变量
来源：http://www.share.sjlbkw.cn/Article/details/glmzdhuku.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.epnwcf.com/Article/details/gkuswifrt.sHtML

[R32] 参数个数校验
来源：http://blog.yfazqb.com/Article/details/geiqzxbox.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gkekjmtoj.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.sjlbkw.cn/Article/details/gnwiqyrub.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fktsv.cn/Article/details/gskqomgzm.sHtML

[R34] 退出时清理
来源：http://m.share.tarul.cn/Article/details/gdvrogyxm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gdjdzrpiq.sHtML

[R35] 后台执行并等待
来源：http://wap.bbcook.cn/Article/details/guqbskbzd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fktsv.cn/Article/details/gjyfywfwr.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.tarul.cn/Article/details/gkqmezfkd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fktsv.cn/Article/details/grrtxtqrh.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.tarul.cn/Article/details/grzdjdkwa.sHtML

files=$(ls -1)
来源：http://3g.sjlbkw.cn/Article/details/gjqnyckum.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/gkpsivuwp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.bbcook.cn/Article/details/ggrxmnbqy.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.tarul.cn/Article/details/gfelebcwk.sHtML

cmd > out.log 2>&1
来源：http://www.share.yfazqb.com/Article/details/gswblzutt.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/gqgwbfcre.sHtML

echo "log" >> out.log
来源：http://wap.vehdjk.com/Article/details/gwvazgaiy.sHtML

[R41] 丢弃输出
来源：http://www.m.share.yfazqb.com/Article/details/ghuhrvmje.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.epnwcf.com/Article/details/ggmeewxgd.sHtML

[R42] 输入重定向
来源：http://read.share.fktsv.cn/Article/details/gpkiukfpr.sHtML

wc -l < a.txt
来源：http://www.blog.epnwcf.com/Article/details/gkfshiabe.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fktsv.cn/Article/details/gkkuluoxv.sHtML

find . -name "*.log" -type f
来源：http://blog.bbcook.cn/Article/details/gbfbpfolh.sHtML

[R44] 按修改时间查找
来源：http://wap.tarul.cn/Article/details/glxjjcfup.sHtML

find . -mtime -7 -type f
来源：http://baike.tarul.cn/Article/details/gjamujrmh.sHtML

[R45] 批量删除
来源：http://blog.tarul.cn/Article/details/gugnusuux.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/gwzpfxyxp.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fktsv.cn/Article/details/gzxkbndol.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.epnwcf.com/Article/details/gksdopvpg.sHtML

[R47] sed 单行替换
来源：http://blog.bbcook.cn/Article/details/gnpuwuyff.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.yfazqb.com/Article/details/gomtnmiyt.sHtML

[R48] awk 取指定列
来源：http://www.blog.fktsv.cn/Article/details/gcyevqkas.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.tarul.cn/Article/details/gwdnlwnxh.sHtML

[R49] awk 带条件
来源：http://m.share.yfazqb.com/Article/details/ggkcodiln.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.bbcook.cn/Article/details/gbkqazpfd.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/gpetnmjqy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.yfazqb.com/Article/details/gavvaxzdm.sHtML

[R51] 排序去重取前几
来源：http://www.blog.epnwcf.com/Article/details/gnpjkovdp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.tarul.cn/Article/details/guwffkdve.sHtML

[R52] 统计行数
来源：http://3g.bbcook.cn/Article/details/gljeihvjz.sHtML

wc -l a.txt
来源：http://www.blog.fktsv.cn/Article/details/gxgnqrqki.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.epnwcf.com/Article/details/ghlijucap.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.epnwcf.com/Article/details/guumehoos.sHtML

[R54] 比较两个文件
来源：http://www.blog.fktsv.cn/Article/details/gddsqaigv.sHtML

diff a.txt b.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/guqyksane.sHtML

[R55] 压缩与解压
来源：http://m.share.bbcook.cn/Article/details/gcelvuhkp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.epnwcf.com/Article/details/ghkvstmag.sHtML

[R56] 远程拷贝
来源：http://read.share.fktsv.cn/Article/details/gfzoyqixd.sHtML

scp file user@host:/path/
来源：http://wap.yfazqb.com/Article/details/gjjxyqbzr.sHtML

[R57] 远程执行命令
来源：http://wap.bbcook.cn/Article/details/ghrijxhxx.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gmjepnkct.sHtML

[R58] 下载文件
来源：http://m.share.yfazqb.com/Article/details/gnemrosrx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/goykinulr.sHtML

[R59] 发 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/gqiytcszj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.vehdjk.com/Article/details/gjvtvsbqi.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gwjcnmphs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.epnwcf.com/Article/details/gzlzyxctn.sHtML

[R61] 磁盘占用
来源：http://www.blog.fktsv.cn/Article/details/gyrkgsplg.sHtML

df -h;  du -sh *
来源：http://3g.vehdjk.com/Article/details/glzzshtde.sHtML

[R62] 找最占空间的文件
来源：http://blog.sjlbkw.cn/Article/details/gqkbjisrf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.yfazqb.com/Article/details/gtwjzrqkn.sHtML

[R63] 内存与进程
来源：http://www.share.sjlbkw.cn/Article/details/gvybcbeec.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fktsv.cn/Article/details/gtgfqkcgg.sHtML

[R64] 结束进程
来源：http://baike.yfazqb.com/Article/details/ggqaouhlk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.tarul.cn/Article/details/guitcqblb.sHtML

[R65] 查看端口占用
来源：http://wap.bbcook.cn/Article/details/gkzsedqkl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/ghsxvvqqn.sHtML

[R66] 定时任务
来源：http://mobile.vehdjk.com/Article/details/geqwkqoaj.sHtML

crontab -e;  crontab -l
来源：http://m.share.vehdjk.com/Article/details/gfirlpnpj.sHtML

[R67] 生成随机十六进制串
来源：http://blog.tarul.cn/Article/details/geggfikss.sHtML

openssl rand -hex 16
来源：http://mobile.sjlbkw.cn/Article/details/gsdnsuyef.sHtML

[R68] 计算文件校验值
来源：http://baike.bbcook.cn/Article/details/gblfwjbfq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.tarul.cn/Article/details/gnpdugkcs.sHtML

[R69] 生成随机密码
来源：http://baike.sjlbkw.cn/Article/details/gomrqdybb.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gdppxcnfu.sHtML

[R70] 时间戳与互转
来源：http://blog.epnwcf.com/Article/details/glbwiodnp.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.epnwcf.com/Article/details/gcukupptp.sHtML

[R71] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/giumlnmac.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.vehdjk.com/Article/details/gvtopabyn.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/grmaybhwm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gyiotrjcv.sHtML

[R73] 分割大日志
来源：http://read.share.yfazqb.com/Article/details/gxlvtdots.sHtML

split -l 1000 big.log part_
来源：http://baike.sjlbkw.cn/Article/details/gehneyass.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/gglkrozod.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.sjlbkw.cn/Article/details/gefnkxuwd.sHtML

[R75] 导出环境变量
来源：http://wap.tarul.cn/Article/details/gooxepcez.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.bbcook.cn/Article/details/gtypjsfgu.sHtML

[R76] 使用临时文件
来源：http://3g.vehdjk.com/Article/details/gbcmocwsn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gdtovqrln.sHtML

[R77] 读取用户输入
来源：http://3g.epnwcf.com/Article/details/grkogcufc.sHtML

read -rp "请输入: " ans
来源：http://www.blog.vehdjk.com/Article/details/gotlcnqju.sHtML

[R78] 交互式菜单
来源：http://read.share.yfazqb.com/Article/details/ggntwhkpg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/ghhtigwis.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/goesdkbxb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.vehdjk.com/Article/details/grdcxiegi.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.yfazqb.com/Article/details/gjaaqwruz.sHtML

time ./run.sh
来源：http://read.share.epnwcf.com/Article/details/ginkdqvgp.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gqwndfqnb.sHtML

S. C / C++ 专题
来源：http://baike.tarul.cn/Article/details/gjynkmifk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkpjcounr.sHtML

[S01] C：Hello World
来源：http://3g.tarul.cn/Article/details/gkwwggixp.sHtML

#include <stdio.h>
来源：http://m.share.epnwcf.com/Article/details/gizowskkn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.tarul.cn/Article/details/ghamttrco.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.tarul.cn/Article/details/gtwvdnjez.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fktsv.cn/Article/details/gbvwqqnxp.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gvivhyjpc.sHtML

int x; scanf("%d", &x);
来源：http://blog.fktsv.cn/Article/details/gbwmuuine.sHtML

[S04] C：字符串复制
来源：http://blog.bbcook.cn/Article/details/gpziulmju.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.vehdjk.com/Article/details/gwgnzqwnm.sHtML

[S05] C：字符串长度
来源：http://blog.yfazqb.com/Article/details/glsptacci.sHtML

strlen(s)
来源：http://3g.fktsv.cn/Article/details/ggtrodkgj.sHtML

[S06] C：字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gguuxhftq.sHtML

strcmp(a, b) == 0
来源：http://www.blog.yfazqb.com/Article/details/gufwhpsyq.sHtML

[S07] C：数组遍历求和
来源：http://wap.bbcook.cn/Article/details/gwbavpzai.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fktsv.cn/Article/details/gazzgfocd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.vehdjk.com/Article/details/gwlywniwr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.yfazqb.com/Article/details/guzetesjg.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/gcoboygnv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.yfazqb.com/Article/details/gmyjavntg.sHtML

[S10] C：指针与解引用
来源：http://www.share.yfazqb.com/Article/details/gbpynyfne.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.yfazqb.com/Article/details/gqgsglvxm.sHtML

[S11] C：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/grpdqplxf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.tarul.cn/Article/details/gdjtedfxh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.tarul.cn/Article/details/goevnvrsi.sHtML

fclose(f);
来源：http://blog.vehdjk.com/Article/details/gnlyclgfc.sHtML

[S12] C：写文件
来源：http://blog.bbcook.cn/Article/details/gwwgxohuf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.bbcook.cn/Article/details/gtbumwdgh.sHtML

[S13] C：宏定义
来源：http://mobile.vehdjk.com/Article/details/gbmzkjnrl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.sjlbkw.cn/Article/details/gdgznvjcy.sHtML

[S14] C：枚举
来源：http://m.share.sjlbkw.cn/Article/details/gpdaiceyz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.vehdjk.com/Article/details/gsttrqehp.sHtML

[S15] C：类型转换
来源：http://www.share.tarul.cn/Article/details/gfmmzcymh.sHtML

(double) a / b
来源：http://read.share.epnwcf.com/Article/details/gdqnkcocp.sHtML

[S16] C：位操作置位
来源：http://www.share.epnwcf.com/Article/details/grchjevqo.sHtML

x |= (1 << 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvewecvuy.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gnclpvlrv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fktsv.cn/Article/details/gfbwfhsic.sHtML

[S18] C：命令行参数
来源：http://m.share.vehdjk.com/Article/details/ggttgsbbf.sHtML

int main(int argc, char **argv)
来源：http://wap.vehdjk.com/Article/details/gmqhomdla.sHtML

[S19] C：快速排序
来源：http://read.share.tarul.cn/Article/details/gjbzjwurk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gkefayfgp.sHtML

[S20] C：二分查找
来源：http://baike.epnwcf.com/Article/details/gldeernhb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gczmwitfn.sHtML

[S21] C：字符类别判断
来源：http://3g.bbcook.cn/Article/details/gjddmqnag.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fktsv.cn/Article/details/gqzpcsymt.sHtML

[S22] C：字符串转数字
来源：http://3g.epnwcf.com/Article/details/gmkpcxlpm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.sjlbkw.cn/Article/details/gqkbllvdq.sHtML

[S23] C：随机数
来源：http://www.m.share.vehdjk.com/Article/details/gjxmagyzw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.epnwcf.com/Article/details/gvpclwopl.sHtML

[S24] C：获取本地时间
来源：http://baike.yfazqb.com/Article/details/gvvcyvouj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.bbcook.cn/Article/details/gxguqcxnx.sHtML

[S25] C：内存拷贝
来源：http://www.blog.tarul.cn/Article/details/gnqdbslpq.sHtML

memcpy(dst, src, n);
来源：http://baike.tarul.cn/Article/details/gmtybauns.sHtML

[S26] C：内存清零
来源：http://baike.fktsv.cn/Article/details/gjumzgxrc.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.tarul.cn/Article/details/glnqidzkp.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gjldwqaxp.sHtML

const double PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gatcptfzs.sHtML

[S28] C：静态变量
来源：http://3g.sjlbkw.cn/Article/details/gcxcybyqf.sHtML

static int counter = 0;
来源：http://mobile.epnwcf.com/Article/details/gbstfkiej.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/gcvkukmme.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.tarul.cn/Article/details/gqjsseklb.sHtML

[S30] C：头文件保护
来源：http://baike.tarul.cn/Article/details/gygtbdwlv.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/gieyuhggk.sHtML

#define X_H
来源：http://m.share.sjlbkw.cn/Article/details/grkfacshi.sHtML

#endif
来源：http://m.share.fktsv.cn/Article/details/gcsicpghq.sHtML

[S31] C++：Hello World
来源：http://blog.bbcook.cn/Article/details/gcgupbbvu.sHtML

#include <iostream>
来源：http://m.share.fktsv.cn/Article/details/giehklyke.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fktsv.cn/Article/details/gfpuneueu.sHtML

[S32] C++：字符串
来源：http://www.share.yfazqb.com/Article/details/gyqbcdwfc.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/gqopvmuzk.sHtML

[S33] C++：vector 增删
来源：http://m.share.yfazqb.com/Article/details/gnchfjarb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.epnwcf.com/Article/details/gbahqlnlm.sHtML

[S34] C++：遍历 vector
来源：http://blog.epnwcf.com/Article/details/gvveffpza.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.tarul.cn/Article/details/gpfvmlzve.sHtML

[S35] C++：map
来源：http://baike.sjlbkw.cn/Article/details/gnxkvdmna.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gbvdidjzh.sHtML

[S36] C++：unordered_map
来源：http://read.share.tarul.cn/Article/details/gejattuqa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gercvyxnb.sHtML

[S37] C++：set
来源：http://www.share.bbcook.cn/Article/details/gombqesew.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.vehdjk.com/Article/details/gqpfwqwnf.sHtML

[S38] C++：排序
来源：http://www.m.share.vehdjk.com/Article/details/gplffdplh.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.tarul.cn/Article/details/gtmtakggi.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/grgfgbidw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/glumjiqzw.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/gvpvvqqjj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.vehdjk.com/Article/details/gkoexzjzv.sHtML

[S41] C++：类与构造函数
来源：http://wap.sjlbkw.cn/Article/details/gpqvfifnd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.bbcook.cn/Article/details/gytowkgvz.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.sjlbkw.cn/Article/details/ggdacnylf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gznsdlgsn.sHtML

[S43] C++：智能指针
来源：http://baike.vehdjk.com/Article/details/gkcbphlzo.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.yfazqb.com/Article/details/gdjyphqbb.sHtML

[S44] C++：引用传参
来源：http://read.share.bbcook.cn/Article/details/gpfeyzmaf.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmndyosh.sHtML

[S45] C++：lambda
来源：http://read.share.bbcook.cn/Article/details/gmmkzgsda.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.vehdjk.com/Article/details/glzfioecl.sHtML

[S46] C++：函数模板
来源：http://m.share.epnwcf.com/Article/details/gbfcvkoxs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.vehdjk.com/Article/details/gguafkkwk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.bbcook.cn/Article/details/gummlajks.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.bbcook.cn/Article/details/gineitfhl.sHtML

[S48] C++：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gxzhkwnhi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.sjlbkw.cn/Article/details/gnidcccpb.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/gokpkadzp.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/gidqkassq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.epnwcf.com/Article/details/gbhdgquez.sHtML

[S50] C++：格式化数字
来源：http://baike.vehdjk.com/Article/details/ghxjuhreq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fktsv.cn/Article/details/gyruetltd.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gwhpbrwvx.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fktsv.cn/Article/details/gochvnbju.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.yfazqb.com/Article/details/gcsudroup.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.epnwcf.com/Article/details/gshwpehpt.sHtML

[S53] C++：移动语义
来源：http://blog.epnwcf.com/Article/details/gqgfmozwz.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gegyjrauq.sHtML

[S54] C++：异常处理
来源：http://read.share.epnwcf.com/Article/details/giitsiegs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.tarul.cn/Article/details/gnytxebqf.sHtML

[S55] C++：结构化绑定
来源：http://wap.vehdjk.com/Article/details/gcgcrevxj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/ggvsexpnj.sHtML

[S56] C++：optional
来源：http://mobile.fktsv.cn/Article/details/gjbzwfjar.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fktsv.cn/Article/details/gyuoncegx.sHtML

[S57] C++：编译期常量
来源：http://www.share.sjlbkw.cn/Article/details/gduexpltq.sHtML

constexpr int N = 10;
来源：http://www.blog.tarul.cn/Article/details/gbixgnvoc.sHtML

[S58] C++：命名空间
来源：http://blog.vehdjk.com/Article/details/gzejcarce.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fktsv.cn/Article/details/gykygcskd.sHtML

[S59] C++：静态断言
来源：http://read.share.sjlbkw.cn/Article/details/gnnxbzfxz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.yfazqb.com/Article/details/geakgrloa.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.sjlbkw.cn/Article/details/gyoyzuoby.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fktsv.cn/Article/details/gohkgbqvb.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gtiwkmcoo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.yfazqb.com/Article/details/gmhulssgl.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gbrbvdhxd.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gtrmlztth.sHtML

println("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/ghwaonohc.sHtML

[T02] Kotlin：变量
来源：http://wap.vehdjk.com/Article/details/gnlpdiqik.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.yfazqb.com/Article/details/getvworrn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.epnwcf.com/Article/details/gyphwpxra.sHtML

"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/glvxemtsf.sHtML

[T04] Kotlin：空安全
来源：http://m.share.vehdjk.com/Article/details/gltiloxmd.sHtML

val n: String? = null;  n?.length
来源：http://baike.epnwcf.com/Article/details/gitqqtver.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/ggwbafadw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fktsv.cn/Article/details/glikmmjya.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.yfazqb.com/Article/details/gjnkfzgmt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.bbcook.cn/Article/details/gyrfzsxbf.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.vehdjk.com/Article/details/gqvnhnzqd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.tarul.cn/Article/details/gsavfcljc.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.bbcook.cn/Article/details/gvplnlwxv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fktsv.cn/Article/details/gemwszvgi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.epnwcf.com/Article/details/gaaxvnbqi.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.sjlbkw.cn/Article/details/gnrabtaci.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.bbcook.cn/Article/details/gsjkecvku.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gypztyasx.sHtML

[T11] Kotlin：协程
来源：http://read.share.epnwcf.com/Article/details/gyhziwkhb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.sjlbkw.cn/Article/details/gjolsjfar.sHtML

[T12] Kotlin：解构声明
来源：http://3g.bbcook.cn/Article/details/gdmxwbgfg.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gxmtybnim.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.bbcook.cn/Article/details/gidmmlaox.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.tarul.cn/Article/details/ggyuhmzfz.sHtML

[T14] Kotlin：循环
来源：http://wap.tarul.cn/Article/details/gxlhehayt.sHtML

for (i in 1..10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/gydsfcyyi.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.bbcook.cn/Article/details/gbueliczv.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fktsv.cn/Article/details/gxeldrehg.sHtML

[T16] Swift：Hello World
来源：http://wap.vehdjk.com/Article/details/gdnzqpmze.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gmrfwqdpy.sHtML

[T17] Swift：变量与常量
来源：http://www.share.vehdjk.com/Article/details/gaxuwwjiw.sHtML

var a = 1;  let b = 2
来源：http://read.share.yfazqb.com/Article/details/gwqkwnbdg.sHtML

[T18] Swift：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gojminzwr.sHtML

"值: \(b)"
来源：http://mobile.epnwcf.com/Article/details/gtyddzhwe.sHtML

[T19] Swift：可选绑定
来源：http://baike.tarul.cn/Article/details/ggmzlvkqa.sHtML

if let n = opt { print(n) }
来源：http://www.blog.vehdjk.com/Article/details/gsflgugsy.sHtML

[T20] Swift：数组操作
来源：http://m.share.epnwcf.com/Article/details/gnacppkgw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.sjlbkw.cn/Article/details/gaetfgplw.sHtML

[T21] Swift：遍历
来源：http://read.share.yfazqb.com/Article/details/gkbegisdj.sHtML

for x in a { print(x) }
来源：http://www.blog.fktsv.cn/Article/details/gslkvrtls.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/gcsykadxo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fktsv.cn/Article/details/gbtkclbvi.sHtML

[T23] Swift：函数
来源：http://3g.epnwcf.com/Article/details/gxhgtgzcl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.epnwcf.com/Article/details/ggeyqrecm.sHtML

[T24] Swift：闭包
来源：http://baike.tarul.cn/Article/details/gpvsllrqs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.yfazqb.com/Article/details/gonurfhkw.sHtML

[T25] Swift：结构体
来源：http://www.share.vehdjk.com/Article/details/gqyoogatc.sHtML

struct P { var x: Int }
来源：http://mobile.bbcook.cn/Article/details/gaklcyfmz.sHtML

[T26] Swift：类与重写
来源：http://www.share.fktsv.cn/Article/details/gkymkfwsg.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.yfazqb.com/Article/details/gmvmtrmwk.sHtML

[T27] Swift：错误处理
来源：http://baike.yfazqb.com/Article/details/ghekaolgp.sHtML

do { try f() } catch { print(error) }
来源：http://baike.epnwcf.com/Article/details/gaqenwtfw.sHtML

[T28] Swift：枚举
来源：http://mobile.vehdjk.com/Article/details/goydjbozn.sHtML

enum Color { case red, green }
来源：http://3g.fktsv.cn/Article/details/gdbzjrneb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.vehdjk.com/Article/details/gnkwuszhj.sHtML

guard let x = opt else { return }
来源：http://m.share.epnwcf.com/Article/details/gtatvmkkk.sHtML

[T30] Swift：协议
来源：http://baike.vehdjk.com/Article/details/gzrdejwuj.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.tarul.cn/Article/details/gdhuszpfr.sHtML

[T31] Lua：Hello World
来源：http://mobile.yfazqb.com/Article/details/gugkzmuux.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/ghgqzhsjw.sHtML

[T32] Lua：局部变量
来源：http://wap.vehdjk.com/Article/details/gijijwfjh.sHtML

local a = 1
来源：http://blog.epnwcf.com/Article/details/gecjmcdvp.sHtML


<!-- 参考信息 -->