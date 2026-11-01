代发 wailian999

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/gkkwluqjd.sHtML

[R28] 浮点运算
来源：http://www.m.share.fktsv.cn/Article/details/gkjcdunca.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.yfazqb.com/Article/details/gcwzfzdzy.sHtML

[R29] 定义函数
来源：http://www.share.vehdjk.com/Article/details/glklrvzsu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.yfazqb.com/Article/details/gpflcjcjh.sHtML

[R30] 函数返回状态码
来源：http://wap.yfazqb.com/Article/details/glzuesooa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.vehdjk.com/Article/details/gunhaksol.sHtML

[R31] 局部变量
来源：http://read.share.vehdjk.com/Article/details/gadopvdsz.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.vehdjk.com/Article/details/gvqxbhykw.sHtML

[R32] 参数个数校验
来源：http://wap.yfazqb.com/Article/details/guvlxtror.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fktsv.cn/Article/details/gqkuigxjp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.vehdjk.com/Article/details/gfpoyrypb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.vehdjk.com/Article/details/gmfmatgru.sHtML

[R34] 退出时清理
来源：http://read.share.vehdjk.com/Article/details/giakoiqlq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/golbvzkqh.sHtML

[R35] 后台执行并等待
来源：http://baike.yfazqb.com/Article/details/gcafjxtip.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.vehdjk.com/Article/details/gwaoggkxw.sHtML

[R36] 并发执行多个任务
来源：http://mobile.vehdjk.com/Article/details/gdnvqtbuf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.vehdjk.com/Article/details/gnynvdgqf.sHtML

[R37] 把输出赋给变量
来源：http://m.share.tarul.cn/Article/details/gikfholau.sHtML

files=$(ls -1)
来源：http://www.blog.tarul.cn/Article/details/gfkydrdry.sHtML

[R38] 管道串联
来源：http://3g.fktsv.cn/Article/details/gxrsxuoak.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.sjlbkw.cn/Article/details/gcbzcdkjt.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.bbcook.cn/Article/details/gayvtoffc.sHtML

cmd > out.log 2>&1
来源：http://mobile.fktsv.cn/Article/details/gkmqnhnkp.sHtML

[R40] 追加写日志
来源：http://mobile.fktsv.cn/Article/details/gqrgwsqbq.sHtML

echo "log" >> out.log
来源：http://www.share.fktsv.cn/Article/details/gghjqpugv.sHtML

[R41] 丢弃输出
来源：http://mobile.vehdjk.com/Article/details/gpoheqguq.sHtML

cmd >/dev/null 2>&1
来源：http://baike.tarul.cn/Article/details/gaksuuzsj.sHtML

[R42] 输入重定向
来源：http://blog.sjlbkw.cn/Article/details/gelqubnxx.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gldlmnlpr.sHtML

[R43] 按名字查找文件
来源：http://read.share.fktsv.cn/Article/details/gzauckoaf.sHtML

find . -name "*.log" -type f
来源：http://www.blog.tarul.cn/Article/details/gpzbetmmn.sHtML

[R44] 按修改时间查找
来源：http://wap.vehdjk.com/Article/details/guzlmvduo.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.tarul.cn/Article/details/gqopbhwaz.sHtML

[R45] 批量删除
来源：http://www.share.sjlbkw.cn/Article/details/gakyuyvrz.sHtML

find . -name "*.tmp" -delete
来源：http://blog.vehdjk.com/Article/details/gpxruovbt.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.bbcook.cn/Article/details/gmoigbupw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.tarul.cn/Article/details/gnmdhxofu.sHtML

[R47] sed 单行替换
来源：http://www.m.share.vehdjk.com/Article/details/guvbermff.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fktsv.cn/Article/details/gonusxaqv.sHtML

[R48] awk 取指定列
来源：http://read.share.vehdjk.com/Article/details/gyzszqphl.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fktsv.cn/Article/details/gzkwrswpy.sHtML

[R49] awk 带条件
来源：http://baike.epnwcf.com/Article/details/gkhlfpdkn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.vehdjk.com/Article/details/gmveqtwun.sHtML

[R50] awk 求和
来源：http://m.share.fktsv.cn/Article/details/gwcomzgql.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fktsv.cn/Article/details/gvctskhuo.sHtML

[R51] 排序去重取前几
来源：http://m.share.epnwcf.com/Article/details/geqzhvprv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fktsv.cn/Article/details/gjncfeczo.sHtML

[R52] 统计行数
来源：http://mobile.yfazqb.com/Article/details/gqcramtgu.sHtML

wc -l a.txt
来源：http://www.blog.tarul.cn/Article/details/giyvupobc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.bbcook.cn/Article/details/gvahswyro.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.vehdjk.com/Article/details/gymcfypjo.sHtML

[R54] 比较两个文件
来源：http://wap.vehdjk.com/Article/details/gqbbixxyy.sHtML

diff a.txt b.txt
来源：http://3g.bbcook.cn/Article/details/gxnxhjjgx.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/gjbfiaysb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.sjlbkw.cn/Article/details/gdpywehhg.sHtML

[R56] 远程拷贝
来源：http://3g.tarul.cn/Article/details/gczsoatuf.sHtML

scp file user@host:/path/
来源：http://baike.vehdjk.com/Article/details/gudwnlyjh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.yfazqb.com/Article/details/gryqsvoae.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.sjlbkw.cn/Article/details/gheksvfjz.sHtML

[R58] 下载文件
来源：http://m.share.fktsv.cn/Article/details/gxqtxpwcs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.bbcook.cn/Article/details/gmhudieza.sHtML

[R59] 发 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gdumnvday.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/gqqkgtnuw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/gqgxbunea.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.epnwcf.com/Article/details/gmimghzgo.sHtML

[R61] 磁盘占用
来源：http://mobile.sjlbkw.cn/Article/details/gynzyvmwe.sHtML

df -h;  du -sh *
来源：http://www.m.share.bbcook.cn/Article/details/gszpbmkrl.sHtML

[R62] 找最占空间的文件
来源：http://wap.tarul.cn/Article/details/gkwoumtfa.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.bbcook.cn/Article/details/gfdwzgfny.sHtML

[R63] 内存与进程
来源：http://read.share.yfazqb.com/Article/details/ggdirzytx.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.epnwcf.com/Article/details/gayzxmxvy.sHtML

[R64] 结束进程
来源：http://wap.epnwcf.com/Article/details/ghadsoyia.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.vehdjk.com/Article/details/gaexfohoz.sHtML

[R65] 查看端口占用
来源：http://www.m.share.yfazqb.com/Article/details/guhtidmzk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.vehdjk.com/Article/details/gzncbutya.sHtML

[R66] 定时任务
来源：http://www.share.bbcook.cn/Article/details/gzylqdmai.sHtML

crontab -e;  crontab -l
来源：http://3g.yfazqb.com/Article/details/gtcivkuyw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fktsv.cn/Article/details/gqmvdevzx.sHtML

openssl rand -hex 16
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvacukqu.sHtML

[R68] 计算文件校验值
来源：http://read.share.sjlbkw.cn/Article/details/gxdrsthjs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.epnwcf.com/Article/details/gkdqcbqdb.sHtML

[R69] 生成随机密码
来源：http://mobile.vehdjk.com/Article/details/gzadaddag.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.tarul.cn/Article/details/gnigbzgph.sHtML

[R70] 时间戳与互转
来源：http://m.share.vehdjk.com/Article/details/grwwxwajw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.bbcook.cn/Article/details/gqcqxbnqk.sHtML

[R71] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gkrbxglse.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.tarul.cn/Article/details/gtblksgkc.sHtML

[R72] 等待端口就绪
来源：http://mobile.sjlbkw.cn/Article/details/gltggqzue.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/gjvldpqmo.sHtML

[R73] 分割大日志
来源：http://www.blog.epnwcf.com/Article/details/gcunozwrd.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/gxhlamppj.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/gsejrwhuh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.yfazqb.com/Article/details/ggswtkheg.sHtML

[R75] 导出环境变量
来源：http://wap.fktsv.cn/Article/details/gvrfqurjh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.tarul.cn/Article/details/gnvlqqlzf.sHtML

[R76] 使用临时文件
来源：http://wap.epnwcf.com/Article/details/gwgfodozf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gkxjkdtzx.sHtML

[R77] 读取用户输入
来源：http://read.share.yfazqb.com/Article/details/govgjquhd.sHtML

read -rp "请输入: " ans
来源：http://3g.fktsv.cn/Article/details/giheulnyp.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/gvfofastv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/glzfsdgkz.sHtML

[R79] 解析命令行选项
来源：http://wap.vehdjk.com/Article/details/gmusthtrm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/gpvrabsih.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.sjlbkw.cn/Article/details/gsrvvwyse.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/gaueytlhx.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gnqazxjep.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/gbwoqllhg.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmhdwezrq.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gbtlislvy.sHtML

#include <stdio.h>
来源：http://mobile.vehdjk.com/Article/details/gsfrmnzhl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.yfazqb.com/Article/details/geodkehvr.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gtnqhqgsw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.epnwcf.com/Article/details/gedyxweyy.sHtML

[S03] C：读入整数
来源：http://www.share.fktsv.cn/Article/details/ggxowwbrz.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/goplsdfsg.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/gzueaqafw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.vehdjk.com/Article/details/gdxpckmts.sHtML

[S05] C：字符串长度
来源：http://read.share.epnwcf.com/Article/details/gueqrnvgu.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/ghdmpakjw.sHtML

[S06] C：字符串比较
来源：http://mobile.fktsv.cn/Article/details/ghycwhfir.sHtML

strcmp(a, b) == 0
来源：http://baike.fktsv.cn/Article/details/gqfjdaaly.sHtML

[S07] C：数组遍历求和
来源：http://blog.yfazqb.com/Article/details/grkglmxoj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.vehdjk.com/Article/details/gsyytpobs.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.bbcook.cn/Article/details/gzgngxmdx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.sjlbkw.cn/Article/details/gxmnkmtux.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.vehdjk.com/Article/details/gbcsscwjg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.bbcook.cn/Article/details/gifnaeuwt.sHtML

[S10] C：指针与解引用
来源：http://mobile.bbcook.cn/Article/details/gcjlwmwqk.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/gqjviksme.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/giqzclejk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.vehdjk.com/Article/details/gokjsqjrd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.sjlbkw.cn/Article/details/gibzogxfp.sHtML

fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/ghbqojrns.sHtML

[S12] C：写文件
来源：http://www.blog.bbcook.cn/Article/details/gnkgpbihq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.yfazqb.com/Article/details/guzuxmvoj.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/grmciybyn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/gkfrudcvr.sHtML

[S14] C：枚举
来源：http://m.share.epnwcf.com/Article/details/gxrkkdbhg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.vehdjk.com/Article/details/ggyrugpvb.sHtML

[S15] C：类型转换
来源：http://baike.tarul.cn/Article/details/gactxxzei.sHtML

(double) a / b
来源：http://www.share.bbcook.cn/Article/details/gqmyqviev.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/gsjabttga.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/gwbqvmrwj.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.bbcook.cn/Article/details/ghgwpfxbo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.yfazqb.com/Article/details/gkbbklxrd.sHtML

[S18] C：命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gnpwefyrf.sHtML

int main(int argc, char **argv)
来源：http://m.share.tarul.cn/Article/details/geavbmkfx.sHtML

[S19] C：快速排序
来源：http://m.share.fktsv.cn/Article/details/gjxddiovd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gpzyyihsn.sHtML

[S20] C：二分查找
来源：http://www.m.share.tarul.cn/Article/details/ghapqvyxg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gvuzfmwes.sHtML

[S21] C：字符类别判断
来源：http://wap.epnwcf.com/Article/details/gqhgwcmhp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.vehdjk.com/Article/details/gtjpekzii.sHtML

[S22] C：字符串转数字
来源：http://www.blog.sjlbkw.cn/Article/details/gokxjwshw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.tarul.cn/Article/details/giabsstvq.sHtML

[S23] C：随机数
来源：http://mobile.vehdjk.com/Article/details/gmixyzoww.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/gwvrlenwr.sHtML

[S24] C：获取本地时间
来源：http://www.blog.epnwcf.com/Article/details/gztlchrpm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.yfazqb.com/Article/details/gxwjqeubx.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fktsv.cn/Article/details/gabxnlzru.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.tarul.cn/Article/details/gyahsndvn.sHtML

[S26] C：内存清零
来源：http://blog.epnwcf.com/Article/details/glapvktzi.sHtML

memset(a, 0, sizeof a);
来源：http://wap.vehdjk.com/Article/details/gwcbkowtm.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gehknhuac.sHtML

const double PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gagwszaek.sHtML

[S28] C：静态变量
来源：http://www.share.fktsv.cn/Article/details/gsticagxy.sHtML

static int counter = 0;
来源：http://baike.tarul.cn/Article/details/gdbhgltuw.sHtML

[S29] C：变参函数
来源：http://blog.yfazqb.com/Article/details/grflumfpv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.tarul.cn/Article/details/groxtrcau.sHtML

[S30] C：头文件保护
来源：http://baike.fktsv.cn/Article/details/gwdhdwyng.sHtML

#ifndef X_H
来源：http://www.blog.yfazqb.com/Article/details/gtpwyodti.sHtML

#define X_H
来源：http://blog.yfazqb.com/Article/details/gjvtpnolk.sHtML

#endif
来源：http://read.share.tarul.cn/Article/details/gqswqpkzu.sHtML

[S31] C++：Hello World
来源：http://www.blog.tarul.cn/Article/details/gljtmethj.sHtML

#include <iostream>
来源：http://m.share.bbcook.cn/Article/details/gxhfbanyq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.vehdjk.com/Article/details/gwwbrdudd.sHtML

[S32] C++：字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gsilvocvs.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.yfazqb.com/Article/details/gmtclohzn.sHtML

[S33] C++：vector 增删
来源：http://3g.sjlbkw.cn/Article/details/guyoojjtq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fktsv.cn/Article/details/gjhdkwjbi.sHtML

[S34] C++：遍历 vector
来源：http://m.share.sjlbkw.cn/Article/details/grerwqfzo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fktsv.cn/Article/details/gjnwlqmsw.sHtML

[S35] C++：map
来源：http://m.share.yfazqb.com/Article/details/gwhguakdk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gepnshpxm.sHtML

[S36] C++：unordered_map
来源：http://wap.bbcook.cn/Article/details/gzttcysrb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/geholdqnh.sHtML

[S37] C++：set
来源：http://m.share.sjlbkw.cn/Article/details/grvivzsfj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.yfazqb.com/Article/details/gxmysmhhr.sHtML

[S38] C++：排序
来源：http://wap.tarul.cn/Article/details/gevbbnyik.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gjbsdztmx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fktsv.cn/Article/details/grhxknqrq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.epnwcf.com/Article/details/gzvdehfah.sHtML

[S40] C++：查找元素
来源：http://www.share.yfazqb.com/Article/details/gufydyiap.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.tarul.cn/Article/details/glsqtortg.sHtML

[S41] C++：类与构造函数
来源：http://blog.sjlbkw.cn/Article/details/givudytwc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.sjlbkw.cn/Article/details/gpwywbncw.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtkcseia.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.sjlbkw.cn/Article/details/gcpnriqai.sHtML

[S43] C++：智能指针
来源：http://blog.epnwcf.com/Article/details/gjrdgeqdc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.bbcook.cn/Article/details/gfuupgokq.sHtML

[S44] C++：引用传参
来源：http://read.share.bbcook.cn/Article/details/gbxlkkdbe.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.yfazqb.com/Article/details/grzhcbrnm.sHtML

[S45] C++：lambda
来源：http://m.share.vehdjk.com/Article/details/gwxszpsbf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/ggmiipwgu.sHtML

[S46] C++：函数模板
来源：http://www.share.tarul.cn/Article/details/gplidoqaz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.sjlbkw.cn/Article/details/gpgujdaui.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.epnwcf.com/Article/details/gcqyopzax.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fktsv.cn/Article/details/glofuugsf.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gvtqvjhka.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.yfazqb.com/Article/details/gqhuhhmrc.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gaupdrsjx.sHtML

[S49] C++：写文件
来源：http://m.share.vehdjk.com/Article/details/gavgvtuwr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.tarul.cn/Article/details/gioppumhd.sHtML

[S50] C++：格式化数字
来源：http://wap.vehdjk.com/Article/details/gfcqdobom.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.tarul.cn/Article/details/gultxidbd.sHtML

[S51] C++：显式类型转换
来源：http://mobile.yfazqb.com/Article/details/guvjiywxr.sHtML

static_cast<double>(a) / b
来源：http://www.blog.yfazqb.com/Article/details/gbrjcgpch.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.epnwcf.com/Article/details/gvugiszqh.sHtML

int size() const noexcept { return n_; }
来源：http://blog.vehdjk.com/Article/details/gkxhzhpqd.sHtML

[S53] C++：移动语义
来源：http://3g.epnwcf.com/Article/details/gkoetrtrc.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.bbcook.cn/Article/details/grjjolhbz.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/ggqvzscgz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.bbcook.cn/Article/details/gwfalcjal.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.epnwcf.com/Article/details/gcqobiyec.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fktsv.cn/Article/details/gxrhjirws.sHtML

[S56] C++：optional
来源：http://baike.sjlbkw.cn/Article/details/glfwjwuei.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.bbcook.cn/Article/details/giktwczue.sHtML

[S57] C++：编译期常量
来源：http://m.share.epnwcf.com/Article/details/gvjgwjxit.sHtML

constexpr int N = 10;
来源：http://www.share.yfazqb.com/Article/details/gwkhnztfd.sHtML

[S58] C++：命名空间
来源：http://m.share.tarul.cn/Article/details/gmkwwoagv.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.bbcook.cn/Article/details/gvkiosscz.sHtML

[S59] C++：静态断言
来源：http://baike.bbcook.cn/Article/details/ghudqnaba.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.tarul.cn/Article/details/garlkqosv.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.epnwcf.com/Article/details/gvhtezlkg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.vehdjk.com/Article/details/gyhaflaor.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/govepmebk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.sjlbkw.cn/Article/details/ggytveajn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gipmbybbi.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fktsv.cn/Article/details/gbestkmmn.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gkyqdvdmx.sHtML

[T02] Kotlin：变量
来源：http://wap.tarul.cn/Article/details/gsicxbcfc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.epnwcf.com/Article/details/gvdmvatnq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.sjlbkw.cn/Article/details/gwksstksl.sHtML

"值: $b"
来源：http://www.m.share.sjlbkw.cn/Article/details/gawsvvtbs.sHtML

[T04] Kotlin：空安全
来源：http://wap.epnwcf.com/Article/details/gmzzcfnto.sHtML

val n: String? = null;  n?.length
来源：http://baike.fktsv.cn/Article/details/gghuvnefo.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.bbcook.cn/Article/details/gwmhiqvvj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.tarul.cn/Article/details/gxwovxtgp.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.epnwcf.com/Article/details/gfvngirby.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fktsv.cn/Article/details/gjxpakqhs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/gipedphjt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.bbcook.cn/Article/details/gtlexjyey.sHtML

[T08] Kotlin：数据类
来源：http://wap.fktsv.cn/Article/details/gmfovffdb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fktsv.cn/Article/details/gcklvykao.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.bbcook.cn/Article/details/gdmlvtqjv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.vehdjk.com/Article/details/gsaybilbt.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.yfazqb.com/Article/details/gdgyzqphy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fktsv.cn/Article/details/gwmuqlsfy.sHtML

[T11] Kotlin：协程
来源：http://read.share.yfazqb.com/Article/details/givoajfpi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fktsv.cn/Article/details/gmvvxfxiz.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fktsv.cn/Article/details/grojxowsz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gvdnwzkro.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.epnwcf.com/Article/details/gpaeexpwg.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.bbcook.cn/Article/details/gmnlisgzv.sHtML

[T14] Kotlin：循环
来源：http://mobile.fktsv.cn/Article/details/gcvbbcqii.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fktsv.cn/Article/details/gqlmuxgep.sHtML

[T15] Kotlin：接口
来源：http://baike.bbcook.cn/Article/details/gkzwxmpaj.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.tarul.cn/Article/details/gmlzubfsy.sHtML

[T16] Swift：Hello World
来源：http://3g.epnwcf.com/Article/details/gjkcpkckw.sHtML

print("Hello")
来源：http://blog.tarul.cn/Article/details/guasjaqcu.sHtML

[T17] Swift：变量与常量
来源：http://m.share.tarul.cn/Article/details/gpmwoxmzr.sHtML

var a = 1;  let b = 2
来源：http://3g.epnwcf.com/Article/details/gfvdlezng.sHtML

[T18] Swift：字符串插值
来源：http://wap.vehdjk.com/Article/details/gpdxadxqv.sHtML

"值: \(b)"
来源：http://m.share.tarul.cn/Article/details/gezzmikib.sHtML

[T19] Swift：可选绑定
来源：http://blog.vehdjk.com/Article/details/gwkiwxlpn.sHtML

if let n = opt { print(n) }
来源：http://3g.tarul.cn/Article/details/gbytdlxmz.sHtML

[T20] Swift：数组操作
来源：http://read.share.epnwcf.com/Article/details/gbmffcfot.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.yfazqb.com/Article/details/gnlbfwyij.sHtML

[T21] Swift：遍历
来源：http://3g.yfazqb.com/Article/details/gdqrsipzr.sHtML

for x in a { print(x) }
来源：http://read.share.yfazqb.com/Article/details/gqhnwkveb.sHtML

[T22] Swift：字典
来源：http://blog.epnwcf.com/Article/details/ggnecznmn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.yfazqb.com/Article/details/gdcbbadbw.sHtML

[T23] Swift：函数
来源：http://m.share.sjlbkw.cn/Article/details/gtrscdupe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.sjlbkw.cn/Article/details/gonxlknom.sHtML

[T24] Swift：闭包
来源：http://wap.sjlbkw.cn/Article/details/gqsjqrvsg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gdhidfkik.sHtML

[T25] Swift：结构体
来源：http://blog.tarul.cn/Article/details/gcmibqhbs.sHtML

struct P { var x: Int }
来源：http://wap.fktsv.cn/Article/details/gqwnxmdxv.sHtML

[T26] Swift：类与重写
来源：http://wap.bbcook.cn/Article/details/gajdxlovi.sHtML

class A: Base { override func f() {} }
来源：http://3g.epnwcf.com/Article/details/gsjkurkcq.sHtML

[T27] Swift：错误处理
来源：http://blog.tarul.cn/Article/details/gtjzcqdnk.sHtML

do { try f() } catch { print(error) }
来源：http://wap.bbcook.cn/Article/details/gmqvxeqyx.sHtML

[T28] Swift：枚举
来源：http://www.blog.epnwcf.com/Article/details/gkgcwflmm.sHtML

enum Color { case red, green }
来源：http://3g.fktsv.cn/Article/details/grcxvkuys.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.tarul.cn/Article/details/gdcgbgwzq.sHtML

guard let x = opt else { return }
来源：http://www.share.sjlbkw.cn/Article/details/gsfjrecsl.sHtML

[T30] Swift：协议
来源：http://www.share.fktsv.cn/Article/details/gwhxjzkgj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.yfazqb.com/Article/details/gzemjypzw.sHtML


<!-- 参考信息 -->