代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.tarul.cn/Article/details/gscspaiwd.sHtML

[R26] 命令替换
来源：http://mobile.sjlbkw.cn/Article/details/grymqoalp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fktsv.cn/Article/details/gstcsqsmu.sHtML

[R27] 算术展开
来源：http://read.share.yfazqb.com/Article/details/gxyucznvu.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.vehdjk.com/Article/details/geugnyblc.sHtML

[R28] 浮点运算
来源：http://www.m.share.yfazqb.com/Article/details/gdspubgae.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/gyftfyflk.sHtML

[R29] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/guwecmuxf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.yfazqb.com/Article/details/gicepwxvx.sHtML

[R30] 函数返回状态码
来源：http://www.share.yfazqb.com/Article/details/gutygkbtr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.yfazqb.com/Article/details/gxgipmuio.sHtML

[R31] 局部变量
来源：http://www.share.fktsv.cn/Article/details/gtxsyuzfd.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.yfazqb.com/Article/details/gefipfihb.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/gfchmxspm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gkyaucatl.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.epnwcf.com/Article/details/gfihoytid.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.vehdjk.com/Article/details/gdvcslhph.sHtML

[R34] 退出时清理
来源：http://mobile.vehdjk.com/Article/details/gvfauydns.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gdsqdchot.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.yfazqb.com/Article/details/gsrjwpqgc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fktsv.cn/Article/details/gcamhlaag.sHtML

[R36] 并发执行多个任务
来源：http://read.share.sjlbkw.cn/Article/details/gwpuduwcq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.sjlbkw.cn/Article/details/gsjenkkwj.sHtML

[R37] 把输出赋给变量
来源：http://blog.tarul.cn/Article/details/gzoyvfdvr.sHtML

files=$(ls -1)
来源：http://3g.tarul.cn/Article/details/gakhixgrn.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/gjacyixyw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.epnwcf.com/Article/details/gtpychimr.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.yfazqb.com/Article/details/gpiibvywv.sHtML

cmd > out.log 2>&1
来源：http://baike.tarul.cn/Article/details/gjwsmunwo.sHtML

[R40] 追加写日志
来源：http://www.blog.yfazqb.com/Article/details/gjftevhmi.sHtML

echo "log" >> out.log
来源：http://www.blog.tarul.cn/Article/details/gaajllevx.sHtML

[R41] 丢弃输出
来源：http://baike.sjlbkw.cn/Article/details/gqpqubcff.sHtML

cmd >/dev/null 2>&1
来源：http://3g.bbcook.cn/Article/details/ggsknokhb.sHtML

[R42] 输入重定向
来源：http://blog.fktsv.cn/Article/details/gpdskyqok.sHtML

wc -l < a.txt
来源：http://baike.tarul.cn/Article/details/gqyxfcbuv.sHtML

[R43] 按名字查找文件
来源：http://wap.sjlbkw.cn/Article/details/gjeuanovq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.tarul.cn/Article/details/glimaedqg.sHtML

[R44] 按修改时间查找
来源：http://www.share.tarul.cn/Article/details/gucbvltgn.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/gykteevym.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gjnkaqxrw.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gzlyrskam.sHtML

[R46] 递归替换文件内容
来源：http://blog.vehdjk.com/Article/details/grnnttlov.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.bbcook.cn/Article/details/giviadprf.sHtML

[R47] sed 单行替换
来源：http://www.m.share.epnwcf.com/Article/details/gogbhbogr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fktsv.cn/Article/details/gbptgnwhw.sHtML

[R48] awk 取指定列
来源：http://www.share.yfazqb.com/Article/details/gvfcblvdp.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.vehdjk.com/Article/details/gdearbzil.sHtML

[R49] awk 带条件
来源：http://blog.vehdjk.com/Article/details/gkixfyecc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/gteruoveo.sHtML

[R50] awk 求和
来源：http://m.share.bbcook.cn/Article/details/gxtgqxvgb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.epnwcf.com/Article/details/gqpbrbayk.sHtML

[R51] 排序去重取前几
来源：http://3g.tarul.cn/Article/details/gjzgmvlop.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fktsv.cn/Article/details/gdedwjkgr.sHtML

[R52] 统计行数
来源：http://m.share.yfazqb.com/Article/details/gqtmrdyno.sHtML

wc -l a.txt
来源：http://3g.vehdjk.com/Article/details/gmwvmsajv.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.epnwcf.com/Article/details/gyljbscpl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fktsv.cn/Article/details/guhnjatjr.sHtML

[R54] 比较两个文件
来源：http://baike.fktsv.cn/Article/details/gjanfuqmd.sHtML

diff a.txt b.txt
来源：http://blog.tarul.cn/Article/details/gdktrkjhk.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/grgzvvugh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.vehdjk.com/Article/details/gityyqdqt.sHtML

[R56] 远程拷贝
来源：http://www.blog.fktsv.cn/Article/details/gabqtdoch.sHtML

scp file user@host:/path/
来源：http://www.blog.sjlbkw.cn/Article/details/gptjulsiq.sHtML

[R57] 远程执行命令
来源：http://3g.vehdjk.com/Article/details/goutoyycm.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/gmobnalqg.sHtML

[R58] 下载文件
来源：http://www.blog.vehdjk.com/Article/details/gigfjodrx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.epnwcf.com/Article/details/gzybinmcv.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gmqwdfwnh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.yfazqb.com/Article/details/gjgfflblc.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gdtzgmidl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.sjlbkw.cn/Article/details/gvenjlfyo.sHtML

[R61] 磁盘占用
来源：http://baike.sjlbkw.cn/Article/details/ggaufdrri.sHtML

df -h;  du -sh *
来源：http://www.share.yfazqb.com/Article/details/gmfnbjeai.sHtML

[R62] 找最占空间的文件
来源：http://baike.vehdjk.com/Article/details/ghcddnjoh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/gdwmjvecm.sHtML

[R63] 内存与进程
来源：http://m.share.tarul.cn/Article/details/ggxxqhvdc.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.yfazqb.com/Article/details/gzanxowwo.sHtML

[R64] 结束进程
来源：http://3g.vehdjk.com/Article/details/gpldcyxmr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.vehdjk.com/Article/details/gxlvxsxmh.sHtML

[R65] 查看端口占用
来源：http://www.blog.vehdjk.com/Article/details/gykfuwysl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.bbcook.cn/Article/details/giateyybj.sHtML

[R66] 定时任务
来源：http://www.blog.epnwcf.com/Article/details/gnhikdblr.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/gznsdbacy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.epnwcf.com/Article/details/grxiziska.sHtML

openssl rand -hex 16
来源：http://read.share.fktsv.cn/Article/details/ghuchlgef.sHtML

[R68] 计算文件校验值
来源：http://read.share.yfazqb.com/Article/details/gsaaddwuj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fktsv.cn/Article/details/gnzkkekvr.sHtML

[R69] 生成随机密码
来源：http://3g.sjlbkw.cn/Article/details/gxaljylzx.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/gepxlgoid.sHtML

[R70] 时间戳与互转
来源：http://wap.vehdjk.com/Article/details/gasnsygel.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fktsv.cn/Article/details/gteskjodq.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gwrrjbwqo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fktsv.cn/Article/details/gfqskxzlv.sHtML

[R72] 等待端口就绪
来源：http://wap.fktsv.cn/Article/details/gojhxqyal.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gouhutgnv.sHtML

[R73] 分割大日志
来源：http://www.blog.bbcook.cn/Article/details/gnocbwqve.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gjmxqdqap.sHtML

[R74] 批量重命名
来源：http://www.share.sjlbkw.cn/Article/details/ggimjdzsq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.tarul.cn/Article/details/gzxuqkzdz.sHtML

[R75] 导出环境变量
来源：http://www.blog.epnwcf.com/Article/details/gtmmzmydy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/gpvnsnrph.sHtML

[R76] 使用临时文件
来源：http://wap.vehdjk.com/Article/details/gackqzafa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/ghmvsihjk.sHtML

[R77] 读取用户输入
来源：http://read.share.yfazqb.com/Article/details/gjbhefpyy.sHtML

read -rp "请输入: " ans
来源：http://mobile.vehdjk.com/Article/details/gafeqjsgb.sHtML

[R78] 交互式菜单
来源：http://www.blog.sjlbkw.cn/Article/details/gfukppenm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.bbcook.cn/Article/details/gkkxkrlsp.sHtML

[R79] 解析命令行选项
来源：http://read.share.sjlbkw.cn/Article/details/gdtiogqlp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.tarul.cn/Article/details/gwcqjxidn.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fktsv.cn/Article/details/gmqdquusl.sHtML

time ./run.sh
来源：http://3g.sjlbkw.cn/Article/details/gaksbzznf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gntrtoqvo.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/gsqxiolce.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwssucqim.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/gjyhadkan.sHtML

#include <stdio.h>
来源：http://www.share.tarul.cn/Article/details/guuadnofk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.sjlbkw.cn/Article/details/godkxvrhv.sHtML

[S02] C：变量与格式化输出
来源：http://baike.vehdjk.com/Article/details/grulexymi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.yfazqb.com/Article/details/gxccpsakb.sHtML

[S03] C：读入整数
来源：http://read.share.sjlbkw.cn/Article/details/gjbgvbolq.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/ggxomhaqo.sHtML

[S04] C：字符串复制
来源：http://3g.epnwcf.com/Article/details/guqtxaseu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/gentcswnc.sHtML

[S05] C：字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gpqgxvamr.sHtML

strlen(s)
来源：http://blog.tarul.cn/Article/details/gytgghzog.sHtML

[S06] C：字符串比较
来源：http://blog.epnwcf.com/Article/details/gvaxcemvi.sHtML

strcmp(a, b) == 0
来源：http://baike.fktsv.cn/Article/details/gehtduurv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.vehdjk.com/Article/details/gyfbjwlac.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.tarul.cn/Article/details/gucuieulu.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.epnwcf.com/Article/details/gywgwsack.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fktsv.cn/Article/details/gyepdvjmp.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fktsv.cn/Article/details/gemdemnnl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.bbcook.cn/Article/details/gcvxoyeml.sHtML

[S10] C：指针与解引用
来源：http://www.blog.vehdjk.com/Article/details/gffwyguqn.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.bbcook.cn/Article/details/gkuwixmua.sHtML

[S11] C：逐行读文件
来源：http://m.share.tarul.cn/Article/details/giswofezg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.yfazqb.com/Article/details/gwmfrujts.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.vehdjk.com/Article/details/gsxusivbb.sHtML

fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gsywlleup.sHtML

[S12] C：写文件
来源：http://www.m.share.bbcook.cn/Article/details/giunqdddo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.yfazqb.com/Article/details/gaqezwljb.sHtML

[S13] C：宏定义
来源：http://www.m.share.vehdjk.com/Article/details/gfpqdnjyp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.epnwcf.com/Article/details/gjvrslias.sHtML

[S14] C：枚举
来源：http://www.share.vehdjk.com/Article/details/gpjwmowcz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.epnwcf.com/Article/details/gbkbsaruh.sHtML

[S15] C：类型转换
来源：http://m.share.fktsv.cn/Article/details/gchyczdxx.sHtML

(double) a / b
来源：http://mobile.vehdjk.com/Article/details/girnyddkd.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/gmelspphm.sHtML

x |= (1 << 3);
来源：http://www.blog.fktsv.cn/Article/details/gteodjryc.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/ghvkjhmrd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/gewnarplv.sHtML

[S18] C：命令行参数
来源：http://www.share.vehdjk.com/Article/details/gquhhgfxp.sHtML

int main(int argc, char **argv)
来源：http://www.share.epnwcf.com/Article/details/gfrbipigi.sHtML

[S19] C：快速排序
来源：http://read.share.fktsv.cn/Article/details/gxdzbfthy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/guxhgfuxy.sHtML

[S20] C：二分查找
来源：http://3g.fktsv.cn/Article/details/guwjyohge.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gxyjzkecs.sHtML

[S21] C：字符类别判断
来源：http://3g.sjlbkw.cn/Article/details/gtpydtvxn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gqmiiyjja.sHtML

[S22] C：字符串转数字
来源：http://www.share.epnwcf.com/Article/details/gsvpueexl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.tarul.cn/Article/details/geiontjrm.sHtML

[S23] C：随机数
来源：http://wap.epnwcf.com/Article/details/gacsifblp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.epnwcf.com/Article/details/ggdjecqpr.sHtML

[S24] C：获取本地时间
来源：http://wap.tarul.cn/Article/details/gvahmivtd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.bbcook.cn/Article/details/gyrhtttya.sHtML

[S25] C：内存拷贝
来源：http://mobile.epnwcf.com/Article/details/gpllizhzz.sHtML

memcpy(dst, src, n);
来源：http://wap.epnwcf.com/Article/details/gnfcqbwpn.sHtML

[S26] C：内存清零
来源：http://3g.yfazqb.com/Article/details/gdsihbzjt.sHtML

memset(a, 0, sizeof a);
来源：http://wap.sjlbkw.cn/Article/details/gzbpxjxfe.sHtML

[S27] C：定义常量
来源：http://mobile.epnwcf.com/Article/details/gaohpjatm.sHtML

const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gorzfewth.sHtML

[S28] C：静态变量
来源：http://www.m.share.vehdjk.com/Article/details/ghztabhds.sHtML

static int counter = 0;
来源：http://mobile.vehdjk.com/Article/details/giomoijhj.sHtML

[S29] C：变参函数
来源：http://m.share.vehdjk.com/Article/details/gvcpfrwep.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.sjlbkw.cn/Article/details/gairtmthl.sHtML

[S30] C：头文件保护
来源：http://m.share.epnwcf.com/Article/details/gheblwqrz.sHtML

#ifndef X_H
来源：http://read.share.bbcook.cn/Article/details/grlxmheul.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/gtlwswzux.sHtML

#endif
来源：http://mobile.vehdjk.com/Article/details/gpdydeusv.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/glekpsxqt.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gcjuswosu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.sjlbkw.cn/Article/details/gmpsvvtoy.sHtML

[S32] C++：字符串
来源：http://blog.bbcook.cn/Article/details/gebrfcxcd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/ggtzmbtxn.sHtML

[S33] C++：vector 增删
来源：http://www.blog.tarul.cn/Article/details/gowbkugrn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.vehdjk.com/Article/details/gavkreudd.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.bbcook.cn/Article/details/gzfoughop.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.vehdjk.com/Article/details/gypvlqtzr.sHtML

[S35] C++：map
来源：http://www.blog.bbcook.cn/Article/details/ggkjdoteh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gmbyxsdfd.sHtML

[S36] C++：unordered_map
来源：http://baike.vehdjk.com/Article/details/gxesxsrwa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/gdvdihgtg.sHtML

[S37] C++：set
来源：http://wap.fktsv.cn/Article/details/gbgrcogoz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/gxggwdhhq.sHtML

[S38] C++：排序
来源：http://www.m.share.fktsv.cn/Article/details/gnneqymzn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gilefcoso.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.sjlbkw.cn/Article/details/gheofdhmn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.epnwcf.com/Article/details/gbqfezadh.sHtML

[S40] C++：查找元素
来源：http://wap.sjlbkw.cn/Article/details/gidofvbbb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.yfazqb.com/Article/details/gmgyzelhq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.sjlbkw.cn/Article/details/ggmtcvckg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsswxbbv.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.sjlbkw.cn/Article/details/gtfyatblz.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.epnwcf.com/Article/details/gmrtpnfrc.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gvwevqfva.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.yfazqb.com/Article/details/gibuclbde.sHtML

[S44] C++：引用传参
来源：http://read.share.epnwcf.com/Article/details/gwmcmplot.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.bbcook.cn/Article/details/gpoxeykbe.sHtML

[S45] C++：lambda
来源：http://3g.fktsv.cn/Article/details/gzessahtq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.yfazqb.com/Article/details/garqwpuaa.sHtML

[S46] C++：函数模板
来源：http://www.m.share.tarul.cn/Article/details/ggyojptzx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.yfazqb.com/Article/details/gqcqtovro.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.tarul.cn/Article/details/gxtadrfpe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.vehdjk.com/Article/details/gjccqtauh.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdbzdjub.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fktsv.cn/Article/details/gqgfabazc.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gddibxlmw.sHtML

[S49] C++：写文件
来源：http://blog.bbcook.cn/Article/details/gizahjwrk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.tarul.cn/Article/details/gtrinpsep.sHtML

[S50] C++：格式化数字
来源：http://baike.vehdjk.com/Article/details/ggpikvskp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gyoiprubc.sHtML

[S51] C++：显式类型转换
来源：http://www.share.bbcook.cn/Article/details/gibixgpcb.sHtML

static_cast<double>(a) / b
来源：http://wap.epnwcf.com/Article/details/gbdpxeeqw.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.sjlbkw.cn/Article/details/gyisfulyf.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fktsv.cn/Article/details/gilbaubdr.sHtML

[S53] C++：移动语义
来源：http://www.blog.sjlbkw.cn/Article/details/gmuklimec.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fktsv.cn/Article/details/gskylfbzi.sHtML

[S54] C++：异常处理
来源：http://baike.epnwcf.com/Article/details/gxxxpqgsd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.yfazqb.com/Article/details/gqknmsyrk.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.tarul.cn/Article/details/gbapwhuvx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fktsv.cn/Article/details/gbtkswseq.sHtML

[S56] C++：optional
来源：http://3g.vehdjk.com/Article/details/ggukcmwko.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.epnwcf.com/Article/details/gbajswsfz.sHtML

[S57] C++：编译期常量
来源：http://mobile.bbcook.cn/Article/details/gkwuhbjbv.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrpivjuj.sHtML

[S58] C++：命名空间
来源：http://read.share.fktsv.cn/Article/details/gcsbkmvrz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gapfkzcsf.sHtML

[S59] C++：静态断言
来源：http://blog.tarul.cn/Article/details/ggkfryrpd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/gyjowrite.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.yfazqb.com/Article/details/ghdvjdqpa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.yfazqb.com/Article/details/gqandsbfs.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gghimdvwe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/gbimvmxva.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/govfvfcss.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gjpuviuoz.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gquauicry.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/gfbmolffi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fktsv.cn/Article/details/gctugmwxx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.yfazqb.com/Article/details/gqmrmzkfu.sHtML

"值: $b"
来源：http://mobile.yfazqb.com/Article/details/gfihqhxip.sHtML

[T04] Kotlin：空安全
来源：http://mobile.vehdjk.com/Article/details/gnpkgtbzr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fktsv.cn/Article/details/gvgbytyjw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.sjlbkw.cn/Article/details/gpbadewma.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.yfazqb.com/Article/details/gxhhqfyox.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gstdsphxo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gxbzjdzlx.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.tarul.cn/Article/details/gkeudmfam.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.tarul.cn/Article/details/giujiaxvi.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/gjmvkxyfv.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.yfazqb.com/Article/details/grwyjumyn.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.bbcook.cn/Article/details/gxokwgqjf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fktsv.cn/Article/details/gyuxcdcdt.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.yfazqb.com/Article/details/gkxidymul.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.epnwcf.com/Article/details/gstddwvci.sHtML

[T11] Kotlin：协程
来源：http://3g.fktsv.cn/Article/details/ghdasdlyn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.vehdjk.com/Article/details/gtzdlsrdz.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.bbcook.cn/Article/details/gyrzcegwx.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fktsv.cn/Article/details/gsxdkeeef.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/gwnnyjiqd.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fktsv.cn/Article/details/gqmgcabnb.sHtML

[T14] Kotlin：循环
来源：http://3g.fktsv.cn/Article/details/glfaikqdz.sHtML

for (i in 1..10) println(i)
来源：http://m.share.yfazqb.com/Article/details/gnlnnfijh.sHtML

[T15] Kotlin：接口
来源：http://blog.fktsv.cn/Article/details/gofsqgehc.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/gwujnlmep.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gnacuxsfu.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gtmtlvrve.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.bbcook.cn/Article/details/gtynzavzv.sHtML

var a = 1;  let b = 2
来源：http://blog.sjlbkw.cn/Article/details/gregaadci.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/gbumodkix.sHtML

"值: \(b)"
来源：http://blog.epnwcf.com/Article/details/glqaromjh.sHtML

[T19] Swift：可选绑定
来源：http://www.share.vehdjk.com/Article/details/gvpjrzftw.sHtML

if let n = opt { print(n) }
来源：http://wap.bbcook.cn/Article/details/gtyobyhww.sHtML

[T20] Swift：数组操作
来源：http://read.share.bbcook.cn/Article/details/gofvbdkjp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.sjlbkw.cn/Article/details/grddazvnl.sHtML

[T21] Swift：遍历
来源：http://www.blog.tarul.cn/Article/details/guoakzets.sHtML

for x in a { print(x) }
来源：http://read.share.tarul.cn/Article/details/ghhuautft.sHtML

[T22] Swift：字典
来源：http://wap.fktsv.cn/Article/details/gzwdgbtgm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.sjlbkw.cn/Article/details/gvgplpmjm.sHtML

[T23] Swift：函数
来源：http://www.blog.epnwcf.com/Article/details/gqoccsqhl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fktsv.cn/Article/details/gvwiptboq.sHtML

[T24] Swift：闭包
来源：http://m.share.vehdjk.com/Article/details/gqyqodiph.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gmlkhtkuf.sHtML

[T25] Swift：结构体
来源：http://mobile.bbcook.cn/Article/details/gzettkuqg.sHtML

struct P { var x: Int }
来源：http://3g.yfazqb.com/Article/details/gxxbyrpkm.sHtML

[T26] Swift：类与重写
来源：http://baike.vehdjk.com/Article/details/gbtwvtqro.sHtML

class A: Base { override func f() {} }
来源：http://wap.yfazqb.com/Article/details/gyklwxrnp.sHtML

[T27] Swift：错误处理
来源：http://baike.bbcook.cn/Article/details/geamrhppd.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fktsv.cn/Article/details/gzsjwagje.sHtML

[T28] Swift：枚举
来源：http://baike.yfazqb.com/Article/details/gifeblgeu.sHtML

enum Color { case red, green }
来源：http://read.share.yfazqb.com/Article/details/gpkdfxagu.sHtML


<!-- 参考信息 -->