代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.blog.sjlbkw.cn/Article/details/gaulezpcc.sHtML

[R28] 浮点运算
来源：http://mobile.bbcook.cn/Article/details/gxyrdvgmr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.sjlbkw.cn/Article/details/gxhhspgsc.sHtML

[R29] 定义函数
来源：http://read.share.sjlbkw.cn/Article/details/gcabknhkc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.vehdjk.com/Article/details/gnelyytxn.sHtML

[R30] 函数返回状态码
来源：http://baike.fktsv.cn/Article/details/gdrqnkzub.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.sjlbkw.cn/Article/details/grbqbsjjp.sHtML

[R31] 局部变量
来源：http://www.share.fktsv.cn/Article/details/ghxshtajw.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fktsv.cn/Article/details/gexudfzab.sHtML

[R32] 参数个数校验
来源：http://3g.vehdjk.com/Article/details/gwwkuuclv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/goyzwxfcb.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.yfazqb.com/Article/details/gknjvfskz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.yfazqb.com/Article/details/ggvjgcqqg.sHtML

[R34] 退出时清理
来源：http://wap.yfazqb.com/Article/details/gcbvkohhn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/ggkftsycq.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/gbyopyghj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.sjlbkw.cn/Article/details/gijkjvxbb.sHtML

[R36] 并发执行多个任务
来源：http://3g.tarul.cn/Article/details/gxqbjzfvm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.sjlbkw.cn/Article/details/gogxenqgm.sHtML

[R37] 把输出赋给变量
来源：http://wap.yfazqb.com/Article/details/gkyonipkd.sHtML

files=$(ls -1)
来源：http://www.share.tarul.cn/Article/details/gqsdshryk.sHtML

[R38] 管道串联
来源：http://www.share.epnwcf.com/Article/details/glhouhnpr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.vehdjk.com/Article/details/grepzmgtr.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/glxzugndb.sHtML

cmd > out.log 2>&1
来源：http://wap.bbcook.cn/Article/details/ghdzrkcyv.sHtML

[R40] 追加写日志
来源：http://read.share.tarul.cn/Article/details/gvbsiswsd.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/gocekkdgn.sHtML

[R41] 丢弃输出
来源：http://mobile.bbcook.cn/Article/details/gsujurpfc.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.epnwcf.com/Article/details/gzaqzytcy.sHtML

[R42] 输入重定向
来源：http://3g.fktsv.cn/Article/details/gsvqiwnoz.sHtML

wc -l < a.txt
来源：http://blog.tarul.cn/Article/details/gssswjcks.sHtML

[R43] 按名字查找文件
来源：http://www.blog.sjlbkw.cn/Article/details/gmjyvyagz.sHtML

find . -name "*.log" -type f
来源：http://baike.tarul.cn/Article/details/ggyywshta.sHtML

[R44] 按修改时间查找
来源：http://www.blog.bbcook.cn/Article/details/gezzqenff.sHtML

find . -mtime -7 -type f
来源：http://m.share.epnwcf.com/Article/details/gxnbzikdg.sHtML

[R45] 批量删除
来源：http://read.share.yfazqb.com/Article/details/gqsrftxip.sHtML

find . -name "*.tmp" -delete
来源：http://wap.bbcook.cn/Article/details/gazuokeio.sHtML

[R46] 递归替换文件内容
来源：http://read.share.vehdjk.com/Article/details/gifetjxwq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.vehdjk.com/Article/details/gxysaodhh.sHtML

[R47] sed 单行替换
来源：http://wap.sjlbkw.cn/Article/details/gtiswzzzx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.yfazqb.com/Article/details/gbvcbbmwe.sHtML

[R48] awk 取指定列
来源：http://blog.bbcook.cn/Article/details/gssknoxxt.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fktsv.cn/Article/details/ghloufnaw.sHtML

[R49] awk 带条件
来源：http://3g.epnwcf.com/Article/details/goacyjysx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.tarul.cn/Article/details/gwktgxfoj.sHtML

[R50] awk 求和
来源：http://baike.fktsv.cn/Article/details/giereghxr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.tarul.cn/Article/details/gqtmndjjd.sHtML

[R51] 排序去重取前几
来源：http://read.share.tarul.cn/Article/details/gurzrhsxd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.yfazqb.com/Article/details/gjxtoxftd.sHtML

[R52] 统计行数
来源：http://www.m.share.sjlbkw.cn/Article/details/gglngksxh.sHtML

wc -l a.txt
来源：http://www.m.share.tarul.cn/Article/details/gmamrbnpn.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/gkvbrovgq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.tarul.cn/Article/details/gqrxsdsvp.sHtML

[R54] 比较两个文件
来源：http://baike.yfazqb.com/Article/details/gvpxxwecg.sHtML

diff a.txt b.txt
来源：http://www.blog.yfazqb.com/Article/details/ghcmjwlqz.sHtML

[R55] 压缩与解压
来源：http://www.share.bbcook.cn/Article/details/gkgntobid.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.sjlbkw.cn/Article/details/gmlipumpk.sHtML

[R56] 远程拷贝
来源：http://blog.sjlbkw.cn/Article/details/gfuxrfgjd.sHtML

scp file user@host:/path/
来源：http://read.share.bbcook.cn/Article/details/gvxjvmfqq.sHtML

[R57] 远程执行命令
来源：http://www.blog.bbcook.cn/Article/details/gcawngrcp.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gsgaexizw.sHtML

[R58] 下载文件
来源：http://blog.tarul.cn/Article/details/gjesmqxyh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.bbcook.cn/Article/details/gehycdsfi.sHtML

[R59] 发 POST JSON
来源：http://baike.epnwcf.com/Article/details/gcxjwnizp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.epnwcf.com/Article/details/gfcgozcwb.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/glnlmudqn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.bbcook.cn/Article/details/gpkalkjaq.sHtML

[R61] 磁盘占用
来源：http://www.m.share.vehdjk.com/Article/details/gigxfidji.sHtML

df -h;  du -sh *
来源：http://m.share.bbcook.cn/Article/details/gzjezzogh.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/gaivikqqg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fktsv.cn/Article/details/gribidriu.sHtML

[R63] 内存与进程
来源：http://www.m.share.tarul.cn/Article/details/gsvbzfhso.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.yfazqb.com/Article/details/gdxfqntll.sHtML

[R64] 结束进程
来源：http://www.blog.vehdjk.com/Article/details/ggrniocdk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/gygtlfjer.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/gnlcgpwyz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.sjlbkw.cn/Article/details/gqvagzglh.sHtML

[R66] 定时任务
来源：http://www.share.epnwcf.com/Article/details/gfkdpszes.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fktsv.cn/Article/details/gsffvjryy.sHtML

[R67] 生成随机十六进制串
来源：http://baike.tarul.cn/Article/details/gwpwarqzb.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/gcgxqqayj.sHtML

[R68] 计算文件校验值
来源：http://www.share.bbcook.cn/Article/details/gxifopbtl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.yfazqb.com/Article/details/glxyyjopg.sHtML

[R69] 生成随机密码
来源：http://3g.epnwcf.com/Article/details/gthxvuryf.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/goxnkjpij.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/gobahsyqs.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fktsv.cn/Article/details/gikaanyfd.sHtML

[R71] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/gwjgketwp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.yfazqb.com/Article/details/gojkochwt.sHtML

[R72] 等待端口就绪
来源：http://baike.tarul.cn/Article/details/gbuvmtuko.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gtlgvipqi.sHtML

[R73] 分割大日志
来源：http://wap.sjlbkw.cn/Article/details/ggdidopsp.sHtML

split -l 1000 big.log part_
来源：http://www.share.vehdjk.com/Article/details/gmmulalot.sHtML

[R74] 批量重命名
来源：http://wap.epnwcf.com/Article/details/garojfnjk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fktsv.cn/Article/details/ganpibqqw.sHtML

[R75] 导出环境变量
来源：http://wap.tarul.cn/Article/details/ghiaohkon.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.sjlbkw.cn/Article/details/glahkjezd.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/gyzpwqkmh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/gbqfbrgqu.sHtML

[R77] 读取用户输入
来源：http://baike.sjlbkw.cn/Article/details/gestddxqz.sHtML

read -rp "请输入: " ans
来源：http://3g.yfazqb.com/Article/details/garnygmav.sHtML

[R78] 交互式菜单
来源：http://mobile.sjlbkw.cn/Article/details/gzdxrnqfv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.bbcook.cn/Article/details/gdichuphx.sHtML

[R79] 解析命令行选项
来源：http://3g.vehdjk.com/Article/details/gyhwydidk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.yfazqb.com/Article/details/gvqfylaqe.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.epnwcf.com/Article/details/gofwhmsdg.sHtML

time ./run.sh
来源：http://blog.epnwcf.com/Article/details/gamvotqew.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gpumaqhqf.sHtML

S. C / C++ 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfmpxoci.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxiilhimb.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gnkgxtslh.sHtML

#include <stdio.h>
来源：http://mobile.fktsv.cn/Article/details/gfuzufsuc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.tarul.cn/Article/details/gxiiylgbt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fktsv.cn/Article/details/gerapcdst.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.tarul.cn/Article/details/gqfolukzm.sHtML

[S03] C：读入整数
来源：http://baike.fktsv.cn/Article/details/gqgullklu.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.yfazqb.com/Article/details/grkulcyqe.sHtML

[S04] C：字符串复制
来源：http://3g.sjlbkw.cn/Article/details/ggtulnfok.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/gtjcqoizc.sHtML

[S05] C：字符串长度
来源：http://baike.vehdjk.com/Article/details/gcwavriyx.sHtML

strlen(s)
来源：http://baike.sjlbkw.cn/Article/details/gsxhwirzn.sHtML

[S06] C：字符串比较
来源：http://m.share.tarul.cn/Article/details/gmtcijxlu.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gmkrjzozl.sHtML

[S07] C：数组遍历求和
来源：http://mobile.epnwcf.com/Article/details/gpgiatnii.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.bbcook.cn/Article/details/gmjfxjljp.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.epnwcf.com/Article/details/gwwworoam.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.yfazqb.com/Article/details/glrjmsjqk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.yfazqb.com/Article/details/goowoimkj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/grwlmtmes.sHtML

[S10] C：指针与解引用
来源：http://3g.bbcook.cn/Article/details/gzekdjqhv.sHtML

int *p = &a;  *p = 5;
来源：http://blog.sjlbkw.cn/Article/details/gwgcidgde.sHtML

[S11] C：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gbveyimyl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.sjlbkw.cn/Article/details/gycozsndc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/grgkmiuwd.sHtML

fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gjqjlixjv.sHtML

[S12] C：写文件
来源：http://mobile.bbcook.cn/Article/details/gsxxoxhaq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.vehdjk.com/Article/details/gdvflcvnh.sHtML

[S13] C：宏定义
来源：http://baike.bbcook.cn/Article/details/gjipiydml.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.vehdjk.com/Article/details/gjqbvcuca.sHtML

[S14] C：枚举
来源：http://www.share.tarul.cn/Article/details/gwsfacuvs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fktsv.cn/Article/details/gwsmhtoya.sHtML

[S15] C：类型转换
来源：http://www.share.sjlbkw.cn/Article/details/ghdnijbgi.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/geirxlvfr.sHtML

[S16] C：位操作置位
来源：http://wap.epnwcf.com/Article/details/gomeoglmd.sHtML

x |= (1 << 3);
来源：http://blog.tarul.cn/Article/details/gxkwaopzc.sHtML

[S17] C：安全拼接字符串
来源：http://blog.yfazqb.com/Article/details/genlahuxn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/gtzwicqze.sHtML

[S18] C：命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/glfmmnjfu.sHtML

int main(int argc, char **argv)
来源：http://3g.fktsv.cn/Article/details/gokpzhafx.sHtML

[S19] C：快速排序
来源：http://m.share.fktsv.cn/Article/details/gqalpnkvg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gsqgayoqw.sHtML

[S20] C：二分查找
来源：http://3g.vehdjk.com/Article/details/gzqmahozo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/gthovaalc.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/guoopvzzr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.epnwcf.com/Article/details/gwfzmdkhf.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/gwaxpdeep.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/gotyizttx.sHtML

[S23] C：随机数
来源：http://baike.fktsv.cn/Article/details/gdqusvwgp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.bbcook.cn/Article/details/gstkqbmst.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/gdxfaksse.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/givcaqjzl.sHtML

[S25] C：内存拷贝
来源：http://mobile.yfazqb.com/Article/details/gkpuuvoum.sHtML

memcpy(dst, src, n);
来源：http://www.blog.yfazqb.com/Article/details/gipdlvnqj.sHtML

[S26] C：内存清零
来源：http://www.m.share.epnwcf.com/Article/details/grcfkyskv.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fktsv.cn/Article/details/gmnkbyxyv.sHtML

[S27] C：定义常量
来源：http://blog.epnwcf.com/Article/details/gtmxabjjr.sHtML

const double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gxiuiciqt.sHtML

[S28] C：静态变量
来源：http://m.share.epnwcf.com/Article/details/gmlcxivzy.sHtML

static int counter = 0;
来源：http://m.share.tarul.cn/Article/details/gilvqiaix.sHtML

[S29] C：变参函数
来源：http://mobile.yfazqb.com/Article/details/gdiazczga.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.vehdjk.com/Article/details/gkmhpgfgy.sHtML

[S30] C：头文件保护
来源：http://3g.epnwcf.com/Article/details/glxaqnpbs.sHtML

#ifndef X_H
来源：http://mobile.tarul.cn/Article/details/gxueexkyy.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/gcudnpmic.sHtML

#endif
来源：http://3g.tarul.cn/Article/details/gwyjtnayp.sHtML

[S31] C++：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gziafftms.sHtML

#include <iostream>
来源：http://www.m.share.vehdjk.com/Article/details/ggnbmhtel.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.tarul.cn/Article/details/gpfeqzjbt.sHtML

[S32] C++：字符串
来源：http://wap.sjlbkw.cn/Article/details/gzqhezbrv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.yfazqb.com/Article/details/gwztqciru.sHtML

[S33] C++：vector 增删
来源：http://www.share.fktsv.cn/Article/details/glumfauoi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.vehdjk.com/Article/details/gcgcvrsls.sHtML

[S34] C++：遍历 vector
来源：http://baike.epnwcf.com/Article/details/gatbizxfh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.epnwcf.com/Article/details/gkhinvshi.sHtML

[S35] C++：map
来源：http://read.share.tarul.cn/Article/details/givaffidm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gbyamtfiq.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/gayjxopng.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gkebtsmml.sHtML

[S37] C++：set
来源：http://www.blog.fktsv.cn/Article/details/gfmenwyuz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.vehdjk.com/Article/details/gdlhkhuny.sHtML

[S38] C++：排序
来源：http://www.m.share.yfazqb.com/Article/details/gxtamzscv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gvkchyzez.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.yfazqb.com/Article/details/glmcqyrab.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.bbcook.cn/Article/details/gefkwvoft.sHtML

[S40] C++：查找元素
来源：http://blog.epnwcf.com/Article/details/gqvgqrdkr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.epnwcf.com/Article/details/ggnccfsao.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gkudjlhaz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.epnwcf.com/Article/details/gzvdhmsjk.sHtML

[S42] C++：继承与虚函数
来源：http://wap.epnwcf.com/Article/details/gsekfzdwk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.tarul.cn/Article/details/ghovtzmsw.sHtML

[S43] C++：智能指针
来源：http://www.share.sjlbkw.cn/Article/details/gxotktknb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.bbcook.cn/Article/details/gegndwiyd.sHtML

[S44] C++：引用传参
来源：http://m.share.yfazqb.com/Article/details/geoqctzui.sHtML

void inc(int &x) { ++x; }
来源：http://3g.tarul.cn/Article/details/gdlhnplis.sHtML

[S45] C++：lambda
来源：http://www.m.share.vehdjk.com/Article/details/goicnbwgq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.sjlbkw.cn/Article/details/gatwqgaoe.sHtML

[S46] C++：函数模板
来源：http://blog.yfazqb.com/Article/details/gahozyoqh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.tarul.cn/Article/details/gpilwdltz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.yfazqb.com/Article/details/gvumzhgaq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.sjlbkw.cn/Article/details/gdwdutyan.sHtML

[S48] C++：逐行读文件
来源：http://wap.epnwcf.com/Article/details/guvuzdvyi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.vehdjk.com/Article/details/grkmgavpf.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.yfazqb.com/Article/details/gfpjhqhdb.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/gwfmlpxgb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.sjlbkw.cn/Article/details/gpqkxxpsy.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/goobeppev.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gwqwngiso.sHtML

[S51] C++：显式类型转换
来源：http://wap.bbcook.cn/Article/details/gbrxgbxkb.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/giucbakog.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/gelrchjjm.sHtML

int size() const noexcept { return n_; }
来源：http://wap.bbcook.cn/Article/details/gybhvuain.sHtML

[S53] C++：移动语义
来源：http://m.share.tarul.cn/Article/details/goxywqndp.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.epnwcf.com/Article/details/guykgotor.sHtML

[S54] C++：异常处理
来源：http://mobile.epnwcf.com/Article/details/gxcrbmgxr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.yfazqb.com/Article/details/gudzhmcnk.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/goknicfhe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.bbcook.cn/Article/details/gpvhjkzwg.sHtML

[S56] C++：optional
来源：http://wap.sjlbkw.cn/Article/details/gwemqouwe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.epnwcf.com/Article/details/geyzidllk.sHtML

[S57] C++：编译期常量
来源：http://read.share.bbcook.cn/Article/details/gtglqyfpp.sHtML

constexpr int N = 10;
来源：http://wap.tarul.cn/Article/details/ggygaopsv.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gltcuiigb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.bbcook.cn/Article/details/gebochrva.sHtML

[S59] C++：静态断言
来源：http://www.blog.sjlbkw.cn/Article/details/gwnhkthep.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdhmtppa.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.bbcook.cn/Article/details/gnexbsgrd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.epnwcf.com/Article/details/gqmsiqjce.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/giecjkqgh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gauvsjlzc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gzijzqpyu.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.vehdjk.com/Article/details/gjxdwbfyk.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/gkytfggrg.sHtML

[T02] Kotlin：变量
来源：http://3g.vehdjk.com/Article/details/grneoilil.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fktsv.cn/Article/details/grbqccobz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.epnwcf.com/Article/details/gdrzrgtoe.sHtML

"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gedbxrxpu.sHtML

[T04] Kotlin：空安全
来源：http://blog.vehdjk.com/Article/details/ggkkymidk.sHtML

val n: String? = null;  n?.length
来源：http://3g.fktsv.cn/Article/details/gxiopzrpo.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.vehdjk.com/Article/details/gymxivloa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.bbcook.cn/Article/details/gsemjpihc.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fktsv.cn/Article/details/grcssjpwx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fktsv.cn/Article/details/gexdwjfos.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gkfoysxep.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/gyzziirhi.sHtML

[T08] Kotlin：数据类
来源：http://baike.fktsv.cn/Article/details/gnjianteh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.bbcook.cn/Article/details/gdljglspv.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.epnwcf.com/Article/details/gdzlxyjrl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.vehdjk.com/Article/details/gmfvulvmf.sHtML

[T10] Kotlin：默认参数
来源：http://baike.tarul.cn/Article/details/gytadvdud.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.sjlbkw.cn/Article/details/gumvdpuxb.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/glvtqybxs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fktsv.cn/Article/details/gwbxojobr.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.sjlbkw.cn/Article/details/grrzivuol.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gcihsjjvi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.yfazqb.com/Article/details/gdikkspwt.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.sjlbkw.cn/Article/details/gsjxgdqkn.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/gwsdftooq.sHtML

for (i in 1..10) println(i)
来源：http://read.share.bbcook.cn/Article/details/ghcujwcwl.sHtML

[T15] Kotlin：接口
来源：http://mobile.yfazqb.com/Article/details/ggrzfpait.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.epnwcf.com/Article/details/gionkvcln.sHtML

[T16] Swift：Hello World
来源：http://blog.bbcook.cn/Article/details/gtojqowqa.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfevuqhr.sHtML

[T17] Swift：变量与常量
来源：http://blog.bbcook.cn/Article/details/guupebqtc.sHtML

var a = 1;  let b = 2
来源：http://3g.vehdjk.com/Article/details/gvbwyuyxe.sHtML

[T18] Swift：字符串插值
来源：http://www.share.vehdjk.com/Article/details/ggebtppek.sHtML

"值: \(b)"
来源：http://mobile.sjlbkw.cn/Article/details/giomzluiw.sHtML

[T19] Swift：可选绑定
来源：http://wap.fktsv.cn/Article/details/gnzxakvvz.sHtML

if let n = opt { print(n) }
来源：http://www.blog.epnwcf.com/Article/details/gndycsfio.sHtML

[T20] Swift：数组操作
来源：http://www.share.sjlbkw.cn/Article/details/gyrfdxlza.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.bbcook.cn/Article/details/gtokwgmgb.sHtML

[T21] Swift：遍历
来源：http://mobile.yfazqb.com/Article/details/gtsnaffaw.sHtML

for x in a { print(x) }
来源：http://m.share.epnwcf.com/Article/details/geldtypys.sHtML

[T22] Swift：字典
来源：http://3g.fktsv.cn/Article/details/gzlturfkl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.bbcook.cn/Article/details/grfwwjgwc.sHtML

[T23] Swift：函数
来源：http://3g.sjlbkw.cn/Article/details/gpvbkvkmc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gnouknqph.sHtML

[T24] Swift：闭包
来源：http://blog.bbcook.cn/Article/details/gbnyklhxs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gtqppeyro.sHtML

[T25] Swift：结构体
来源：http://www.share.epnwcf.com/Article/details/gurfydlht.sHtML

struct P { var x: Int }
来源：http://www.blog.tarul.cn/Article/details/gnjdocxxq.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.yfazqb.com/Article/details/gddjsnilt.sHtML

class A: Base { override func f() {} }
来源：http://m.share.tarul.cn/Article/details/gnyfwhmpy.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fktsv.cn/Article/details/gohumfsrz.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fktsv.cn/Article/details/gxrlshfku.sHtML

[T28] Swift：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gulzdmjev.sHtML

enum Color { case red, green }
来源：http://www.blog.epnwcf.com/Article/details/glsbrbwbb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.tarul.cn/Article/details/gvgauznke.sHtML

guard let x = opt else { return }
来源：http://blog.tarul.cn/Article/details/gamwdzvua.sHtML

[T30] Swift：协议
来源：http://read.share.sjlbkw.cn/Article/details/gslyluceq.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.tarul.cn/Article/details/giftjoqtp.sHtML


<!-- 参考信息 -->