代发 wailian999

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/ghfknjmoa.sHtML

[R28] 浮点运算
来源：http://www.m.share.fktsv.cn/Article/details/ggxkwllqx.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.bbcook.cn/Article/details/gtnfuokbj.sHtML

[R29] 定义函数
来源：http://3g.fktsv.cn/Article/details/gfvfottwl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/grlcjafir.sHtML

[R30] 函数返回状态码
来源：http://wap.epnwcf.com/Article/details/goijvosic.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.sjlbkw.cn/Article/details/glalbadys.sHtML

[R31] 局部变量
来源：http://read.share.vehdjk.com/Article/details/gudmqwoqh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.tarul.cn/Article/details/glclwbrrh.sHtML

[R32] 参数个数校验
来源：http://read.share.bbcook.cn/Article/details/guxsuiizw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/govplfqpx.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/goteynqxd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.sjlbkw.cn/Article/details/gvudvjalz.sHtML

[R34] 退出时清理
来源：http://www.m.share.yfazqb.com/Article/details/gxcqqwfwb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gyvmnveii.sHtML

[R35] 后台执行并等待
来源：http://m.share.epnwcf.com/Article/details/gajjyvovy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.yfazqb.com/Article/details/gbfimhekf.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.bbcook.cn/Article/details/gxkjwqgdq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.yfazqb.com/Article/details/gohkbowdp.sHtML

[R37] 把输出赋给变量
来源：http://baike.sjlbkw.cn/Article/details/grlxsbvrn.sHtML

files=$(ls -1)
来源：http://wap.fktsv.cn/Article/details/glvcqdqsb.sHtML

[R38] 管道串联
来源：http://m.share.tarul.cn/Article/details/ghcvdbqwl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.tarul.cn/Article/details/gtfgftjcu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.bbcook.cn/Article/details/gbylqzfij.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/gkeyogpmy.sHtML

[R40] 追加写日志
来源：http://3g.vehdjk.com/Article/details/gplxbdxpw.sHtML

echo "log" >> out.log
来源：http://www.share.epnwcf.com/Article/details/gcmtxshlk.sHtML

[R41] 丢弃输出
来源：http://www.blog.epnwcf.com/Article/details/gdiyceevg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.yfazqb.com/Article/details/ghoulouhu.sHtML

[R42] 输入重定向
来源：http://baike.yfazqb.com/Article/details/guqdqdcdw.sHtML

wc -l < a.txt
来源：http://3g.fktsv.cn/Article/details/gxswylifi.sHtML

[R43] 按名字查找文件
来源：http://baike.fktsv.cn/Article/details/geezersdt.sHtML

find . -name "*.log" -type f
来源：http://baike.tarul.cn/Article/details/ghebyxedp.sHtML

[R44] 按修改时间查找
来源：http://wap.yfazqb.com/Article/details/gnxwnboox.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/gurorzelj.sHtML

[R45] 批量删除
来源：http://blog.yfazqb.com/Article/details/guxnsmdkn.sHtML

find . -name "*.tmp" -delete
来源：http://baike.tarul.cn/Article/details/ghgdnsazg.sHtML

[R46] 递归替换文件内容
来源：http://mobile.yfazqb.com/Article/details/ggxtcentt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fktsv.cn/Article/details/gpxvsalkf.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gwjfxxmtw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.epnwcf.com/Article/details/gfefdusef.sHtML

[R48] awk 取指定列
来源：http://mobile.yfazqb.com/Article/details/grcikvhhr.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.tarul.cn/Article/details/ghrkcedda.sHtML

[R49] awk 带条件
来源：http://baike.sjlbkw.cn/Article/details/gjtrzxugr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.bbcook.cn/Article/details/gnqdhdsfl.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/gjvytgouw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmtxwwkw.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.vehdjk.com/Article/details/gbhcoetai.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.bbcook.cn/Article/details/gqphmqngz.sHtML

[R52] 统计行数
来源：http://blog.tarul.cn/Article/details/gmsiujkax.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/garcgawab.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gphtmafzn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.yfazqb.com/Article/details/geruusapx.sHtML

[R54] 比较两个文件
来源：http://www.blog.epnwcf.com/Article/details/gmatlqubx.sHtML

diff a.txt b.txt
来源：http://mobile.sjlbkw.cn/Article/details/gojlphwyj.sHtML

[R55] 压缩与解压
来源：http://www.share.bbcook.cn/Article/details/gpwkkncuw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.yfazqb.com/Article/details/gfhkqokqi.sHtML

[R56] 远程拷贝
来源：http://mobile.bbcook.cn/Article/details/gjnxitehq.sHtML

scp file user@host:/path/
来源：http://wap.vehdjk.com/Article/details/gaabnlbzo.sHtML

[R57] 远程执行命令
来源：http://read.share.sjlbkw.cn/Article/details/gwjnnmczk.sHtML

ssh user@host 'uptime'
来源：http://baike.epnwcf.com/Article/details/gvuonibwb.sHtML

[R58] 下载文件
来源：http://read.share.bbcook.cn/Article/details/grtfdugiy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fktsv.cn/Article/details/gvfkommfu.sHtML

[R59] 发 POST JSON
来源：http://baike.vehdjk.com/Article/details/gwfjzomjk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.yfazqb.com/Article/details/gfzhwlbyy.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gwnfbacqq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.sjlbkw.cn/Article/details/geeyenvry.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/gphzyiyjw.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/gajjzpjmw.sHtML

[R62] 找最占空间的文件
来源：http://baike.epnwcf.com/Article/details/gjoqlbqym.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.epnwcf.com/Article/details/gushvtjxx.sHtML

[R63] 内存与进程
来源：http://baike.bbcook.cn/Article/details/glndsyuqe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fktsv.cn/Article/details/gigoxqbtr.sHtML

[R64] 结束进程
来源：http://www.blog.tarul.cn/Article/details/gutuxhlpe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.vehdjk.com/Article/details/gqbekmoim.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/gimruywhm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.sjlbkw.cn/Article/details/gjrdpuudh.sHtML

[R66] 定时任务
来源：http://3g.bbcook.cn/Article/details/ghkyspmhs.sHtML

crontab -e;  crontab -l
来源：http://blog.vehdjk.com/Article/details/gghlwkvpu.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/gxvcmrspm.sHtML

openssl rand -hex 16
来源：http://wap.epnwcf.com/Article/details/gpcrutobi.sHtML

[R68] 计算文件校验值
来源：http://www.share.sjlbkw.cn/Article/details/gryjmumdb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.bbcook.cn/Article/details/griwshkcx.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/gavvityjd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fktsv.cn/Article/details/gedugucqb.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gvusmxkkx.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/gcgrexbct.sHtML

[R71] 日期格式化
来源：http://blog.bbcook.cn/Article/details/ghsasbmju.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.sjlbkw.cn/Article/details/gfbkjgoab.sHtML

[R72] 等待端口就绪
来源：http://read.share.fktsv.cn/Article/details/gwnfsgwyf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gfigzzokv.sHtML

[R73] 分割大日志
来源：http://www.share.epnwcf.com/Article/details/ghywvbdcz.sHtML

split -l 1000 big.log part_
来源：http://www.blog.vehdjk.com/Article/details/grslleveg.sHtML

[R74] 批量重命名
来源：http://mobile.sjlbkw.cn/Article/details/genkigums.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.vehdjk.com/Article/details/gnbiewhmt.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/gihclqmel.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.bbcook.cn/Article/details/glbkrffmz.sHtML

[R76] 使用临时文件
来源：http://mobile.yfazqb.com/Article/details/gdtcletaa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gsgaaqier.sHtML

[R77] 读取用户输入
来源：http://m.share.vehdjk.com/Article/details/gsbtordmr.sHtML

read -rp "请输入: " ans
来源：http://mobile.epnwcf.com/Article/details/glqxnyimc.sHtML

[R78] 交互式菜单
来源：http://www.m.share.sjlbkw.cn/Article/details/goblbznwn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.vehdjk.com/Article/details/gqkncscnn.sHtML

[R79] 解析命令行选项
来源：http://www.share.yfazqb.com/Article/details/gophozuky.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.yfazqb.com/Article/details/gxdoaxnnd.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.epnwcf.com/Article/details/ghcqtyszt.sHtML

time ./run.sh
来源：http://www.m.share.tarul.cn/Article/details/gtrgromcw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjfrucncb.sHtML

S. C / C++ 专题
来源：http://www.blog.bbcook.cn/Article/details/gifvxkojx.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzdcbmmmx.sHtML

[S01] C：Hello World
来源：http://blog.epnwcf.com/Article/details/gskcjdgbd.sHtML

#include <stdio.h>
来源：http://read.share.tarul.cn/Article/details/gbbivykon.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fktsv.cn/Article/details/gqyfeleat.sHtML

[S02] C：变量与格式化输出
来源：http://blog.tarul.cn/Article/details/gdfekogol.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.sjlbkw.cn/Article/details/gllbtwswi.sHtML

[S03] C：读入整数
来源：http://m.share.yfazqb.com/Article/details/gcjgczcgp.sHtML

int x; scanf("%d", &x);
来源：http://read.share.tarul.cn/Article/details/gbmgmiowc.sHtML

[S04] C：字符串复制
来源：http://www.share.fktsv.cn/Article/details/gukfircxk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gutyiknta.sHtML

[S05] C：字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gzcpjyjei.sHtML

strlen(s)
来源：http://mobile.bbcook.cn/Article/details/gvbeuabpl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gxbsbpcye.sHtML

strcmp(a, b) == 0
来源：http://blog.fktsv.cn/Article/details/gbpmsblrm.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gpxoqxtyi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.vehdjk.com/Article/details/gngophyxh.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.epnwcf.com/Article/details/gricanusc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fktsv.cn/Article/details/gxgepwezb.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.yfazqb.com/Article/details/gjjlkaugb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.epnwcf.com/Article/details/gytesjfuk.sHtML

[S10] C：指针与解引用
来源：http://3g.bbcook.cn/Article/details/gpayzknlv.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fktsv.cn/Article/details/gnclpcfej.sHtML

[S11] C：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gujslskwu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.yfazqb.com/Article/details/gsnqbkxjh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.yfazqb.com/Article/details/gckwtvmdp.sHtML

fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/gmqjxnmaw.sHtML

[S12] C：写文件
来源：http://read.share.epnwcf.com/Article/details/ghpchnuoo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/gpqczzbvy.sHtML

[S13] C：宏定义
来源：http://blog.fktsv.cn/Article/details/gayhyqizx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.sjlbkw.cn/Article/details/ggyvjjapr.sHtML

[S14] C：枚举
来源：http://wap.sjlbkw.cn/Article/details/gzmudshmp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.sjlbkw.cn/Article/details/gvgveiqtw.sHtML

[S15] C：类型转换
来源：http://www.m.share.bbcook.cn/Article/details/ghopgjgyd.sHtML

(double) a / b
来源：http://wap.fktsv.cn/Article/details/gzhdofwsd.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/gkpsbcuzh.sHtML

x |= (1 << 3);
来源：http://m.share.bbcook.cn/Article/details/gvgaowznp.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gndsttmbf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.yfazqb.com/Article/details/gndpyvmrz.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/gwfiyuszd.sHtML

int main(int argc, char **argv)
来源：http://blog.tarul.cn/Article/details/gxmyiaqqb.sHtML

[S19] C：快速排序
来源：http://3g.fktsv.cn/Article/details/gjijvbmme.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gqvfeyfsv.sHtML

[S20] C：二分查找
来源：http://3g.tarul.cn/Article/details/gwnmqmphd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/ghnzdfnje.sHtML

[S21] C：字符类别判断
来源：http://wap.fktsv.cn/Article/details/gvqugukgu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/grumdlogv.sHtML

[S22] C：字符串转数字
来源：http://baike.vehdjk.com/Article/details/gvuuuewmx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.vehdjk.com/Article/details/gxdmwvtbt.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gocxdngau.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.vehdjk.com/Article/details/ggcqibbmt.sHtML

[S24] C：获取本地时间
来源：http://www.share.epnwcf.com/Article/details/gjfqezxkg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/giqpzvvlu.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gyeifdcvf.sHtML

memcpy(dst, src, n);
来源：http://mobile.tarul.cn/Article/details/gnisxairc.sHtML

[S26] C：内存清零
来源：http://www.share.tarul.cn/Article/details/gffuwdexc.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.tarul.cn/Article/details/gggyrrtbp.sHtML

[S27] C：定义常量
来源：http://mobile.bbcook.cn/Article/details/gqyyxufop.sHtML

const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gpfnavowl.sHtML

[S28] C：静态变量
来源：http://blog.epnwcf.com/Article/details/gosxlnnvr.sHtML

static int counter = 0;
来源：http://3g.sjlbkw.cn/Article/details/gatmbfmhd.sHtML

[S29] C：变参函数
来源：http://baike.epnwcf.com/Article/details/geovrfmoh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fktsv.cn/Article/details/gwyasykjz.sHtML

[S30] C：头文件保护
来源：http://mobile.fktsv.cn/Article/details/gislftqwj.sHtML

#ifndef X_H
来源：http://read.share.tarul.cn/Article/details/gavisfbsq.sHtML

#define X_H
来源：http://m.share.tarul.cn/Article/details/gkiveggzq.sHtML

#endif
来源：http://www.blog.sjlbkw.cn/Article/details/gcswlvrcw.sHtML

[S31] C++：Hello World
来源：http://read.share.tarul.cn/Article/details/gdgufnbrm.sHtML

#include <iostream>
来源：http://www.share.yfazqb.com/Article/details/gllkemztr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.epnwcf.com/Article/details/gjrspwjrm.sHtML

[S32] C++：字符串
来源：http://www.m.share.vehdjk.com/Article/details/gnsuvrdng.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.yfazqb.com/Article/details/gninlrvtq.sHtML

[S33] C++：vector 增删
来源：http://3g.tarul.cn/Article/details/gzsgxpcok.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.epnwcf.com/Article/details/glajqznnt.sHtML

[S34] C++：遍历 vector
来源：http://wap.vehdjk.com/Article/details/gevaxlvek.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.sjlbkw.cn/Article/details/glrhdnixd.sHtML

[S35] C++：map
来源：http://wap.bbcook.cn/Article/details/gohhpoknj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gssufshmz.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gkiiyhfwl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gyksxhwbj.sHtML

[S37] C++：set
来源：http://mobile.vehdjk.com/Article/details/gratxrdfl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/gjmjhvhad.sHtML

[S38] C++：排序
来源：http://m.share.tarul.cn/Article/details/gsbrblypg.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.bbcook.cn/Article/details/gbutquhhn.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fktsv.cn/Article/details/gcmqyqwin.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.epnwcf.com/Article/details/gboogjmgb.sHtML

[S40] C++：查找元素
来源：http://wap.yfazqb.com/Article/details/gwexnrjnw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.vehdjk.com/Article/details/gstgrlscq.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gldhuxepc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.tarul.cn/Article/details/gdllkggtc.sHtML

[S42] C++：继承与虚函数
来源：http://baike.epnwcf.com/Article/details/guabngkkt.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.yfazqb.com/Article/details/giboyilqa.sHtML

[S43] C++：智能指针
来源：http://www.blog.epnwcf.com/Article/details/gbqgagkit.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.vehdjk.com/Article/details/ginneghqw.sHtML

[S44] C++：引用传参
来源：http://m.share.bbcook.cn/Article/details/ghgbohjmq.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.yfazqb.com/Article/details/gwlpnvnal.sHtML

[S45] C++：lambda
来源：http://www.blog.tarul.cn/Article/details/gbdpjuaxt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.tarul.cn/Article/details/gbffxsqfv.sHtML

[S46] C++：函数模板
来源：http://baike.tarul.cn/Article/details/gkvtvuatd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fktsv.cn/Article/details/gupbgpczh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fktsv.cn/Article/details/gsbteewdh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fktsv.cn/Article/details/gohdsisbd.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/ghcodqwwc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.epnwcf.com/Article/details/goizvfqpl.sHtML

while (std::getline(in, line)) { }
来源：http://3g.yfazqb.com/Article/details/gwjvcgfzf.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/grmiwesmr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.yfazqb.com/Article/details/gytottwvj.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.epnwcf.com/Article/details/gmmyjkhyo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/grsgrqvji.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/ggtldjutt.sHtML

static_cast<double>(a) / b
来源：http://blog.bbcook.cn/Article/details/gfmrqjjeh.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.yfazqb.com/Article/details/gxtgkanpx.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.bbcook.cn/Article/details/ghiqtxanh.sHtML

[S53] C++：移动语义
来源：http://www.blog.fktsv.cn/Article/details/gwagqvfyg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.vehdjk.com/Article/details/gcjedrlpb.sHtML

[S54] C++：异常处理
来源：http://baike.fktsv.cn/Article/details/gnjsusobl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.bbcook.cn/Article/details/gshcybxsl.sHtML

[S55] C++：结构化绑定
来源：http://blog.bbcook.cn/Article/details/glxvnuqmx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.epnwcf.com/Article/details/gookgsprx.sHtML

[S56] C++：optional
来源：http://www.blog.yfazqb.com/Article/details/geutmlpnv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/gvdjzwuep.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.vehdjk.com/Article/details/gqobhafii.sHtML

constexpr int N = 10;
来源：http://blog.vehdjk.com/Article/details/gcykuujzo.sHtML

[S58] C++：命名空间
来源：http://blog.yfazqb.com/Article/details/grosdocoz.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.tarul.cn/Article/details/ggtedjhcn.sHtML

[S59] C++：静态断言
来源：http://wap.epnwcf.com/Article/details/gzoxditkp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/gqnsszdrt.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.bbcook.cn/Article/details/gbosvhtic.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.epnwcf.com/Article/details/gztarfign.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gfcwoygeu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/ghwnaezph.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gmqhcvjqt.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.bbcook.cn/Article/details/gvuiaxdfu.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/ghnkyalla.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.vehdjk.com/Article/details/gtzfbeprn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.sjlbkw.cn/Article/details/gtzlkmcre.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.tarul.cn/Article/details/gmfgexsgy.sHtML

"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gnuloabgs.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gzsfetrpq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.bbcook.cn/Article/details/gijipvwsv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/guohmdxtv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/gbopxpoyw.sHtML

[T06] Kotlin：集合映射
来源：http://3g.bbcook.cn/Article/details/gfsldkdby.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.epnwcf.com/Article/details/gncdlzlmt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.yfazqb.com/Article/details/gtsrufuhn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.epnwcf.com/Article/details/ggjowjict.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/gyqgmwrcq.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.sjlbkw.cn/Article/details/grgwkxeaj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/gpbryblwy.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.bbcook.cn/Article/details/guwerfbya.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.epnwcf.com/Article/details/gqrdtsdhi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.epnwcf.com/Article/details/gnrlixtwk.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/gqhmnmpwu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.sjlbkw.cn/Article/details/gfivnoqvi.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/gcolhuill.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.epnwcf.com/Article/details/gmjuvycra.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.epnwcf.com/Article/details/glefmwfuw.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fktsv.cn/Article/details/gsjewrmrj.sHtML

[T14] Kotlin：循环
来源：http://mobile.bbcook.cn/Article/details/gyhzspnaa.sHtML

for (i in 1..10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gbnysxces.sHtML

[T15] Kotlin：接口
来源：http://read.share.yfazqb.com/Article/details/gockrhall.sHtML

interface Shape { fun area(): Double }
来源：http://wap.sjlbkw.cn/Article/details/gsprkibvl.sHtML

[T16] Swift：Hello World
来源：http://wap.vehdjk.com/Article/details/geqwrefux.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gqxjeoupr.sHtML

[T17] Swift：变量与常量
来源：http://3g.tarul.cn/Article/details/gksysobjv.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/gknpvtrdd.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gfdqzdjpb.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/gmizzwlnp.sHtML

[T19] Swift：可选绑定
来源：http://baike.bbcook.cn/Article/details/geucmqwfp.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.yfazqb.com/Article/details/gpkjokldt.sHtML

[T20] Swift：数组操作
来源：http://mobile.yfazqb.com/Article/details/ghxmrvsoy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.bbcook.cn/Article/details/garlkyhrg.sHtML

[T21] Swift：遍历
来源：http://m.share.bbcook.cn/Article/details/gtoqbpbuz.sHtML

for x in a { print(x) }
来源：http://www.blog.vehdjk.com/Article/details/gdrskmact.sHtML

[T22] Swift：字典
来源：http://www.share.fktsv.cn/Article/details/guzwsptpq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.sjlbkw.cn/Article/details/gguryvgbr.sHtML

[T23] Swift：函数
来源：http://blog.tarul.cn/Article/details/gzpcddeoj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.vehdjk.com/Article/details/gvgrnsukw.sHtML

[T24] Swift：闭包
来源：http://baike.tarul.cn/Article/details/gaeyvkpqp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.epnwcf.com/Article/details/gyttokirg.sHtML

[T25] Swift：结构体
来源：http://mobile.yfazqb.com/Article/details/gifpzomlr.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/guscvpauy.sHtML

[T26] Swift：类与重写
来源：http://3g.vehdjk.com/Article/details/gatpsxrxz.sHtML

class A: Base { override func f() {} }
来源：http://blog.bbcook.cn/Article/details/gkzwmyxeu.sHtML

[T27] Swift：错误处理
来源：http://m.share.sjlbkw.cn/Article/details/grlwgcyqr.sHtML

do { try f() } catch { print(error) }
来源：http://baike.yfazqb.com/Article/details/gxkaclgcp.sHtML

[T28] Swift：枚举
来源：http://m.share.tarul.cn/Article/details/ggleamani.sHtML

enum Color { case red, green }
来源：http://www.blog.bbcook.cn/Article/details/gccgeqzie.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.sjlbkw.cn/Article/details/gecptldhv.sHtML

guard let x = opt else { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gyjdveghh.sHtML

[T30] Swift：协议
来源：http://wap.vehdjk.com/Article/details/grxpcguxi.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fktsv.cn/Article/details/gkiapvqoo.sHtML


<!-- 参考信息 -->