代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://m.share.vehdjk.com/Article/details/gpjkbonvx.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/gmqwfdago.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/gqedeswau.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.bbcook.cn/Article/details/guibrlmmy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.vehdjk.com/Article/details/ggqytrlhf.sHtML

[R34] 退出时清理
来源：http://read.share.sjlbkw.cn/Article/details/gcxdlpize.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gbmlqaxfi.sHtML

[R35] 后台执行并等待
来源：http://www.share.fktsv.cn/Article/details/gxvntehmr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fktsv.cn/Article/details/gtjqwnljq.sHtML

[R36] 并发执行多个任务
来源：http://blog.fktsv.cn/Article/details/ggnxeczbi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.yfazqb.com/Article/details/gafcavsnf.sHtML

[R37] 把输出赋给变量
来源：http://blog.sjlbkw.cn/Article/details/gmdfyrjad.sHtML

files=$(ls -1)
来源：http://baike.sjlbkw.cn/Article/details/gdbtuwwgs.sHtML

[R38] 管道串联
来源：http://3g.sjlbkw.cn/Article/details/geuroxcnt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fktsv.cn/Article/details/gphzgewum.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.tarul.cn/Article/details/gzmztvnhc.sHtML

cmd > out.log 2>&1
来源：http://www.blog.tarul.cn/Article/details/gzyknigov.sHtML

[R40] 追加写日志
来源：http://blog.epnwcf.com/Article/details/gpasypoib.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/gziplviev.sHtML

[R41] 丢弃输出
来源：http://baike.epnwcf.com/Article/details/gaeimsnyl.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/gymfndjkw.sHtML

[R42] 输入重定向
来源：http://blog.tarul.cn/Article/details/geaqafhri.sHtML

wc -l < a.txt
来源：http://blog.tarul.cn/Article/details/gynfrwspo.sHtML

[R43] 按名字查找文件
来源：http://wap.bbcook.cn/Article/details/gjlworzih.sHtML

find . -name "*.log" -type f
来源：http://baike.sjlbkw.cn/Article/details/gmmbkbxgp.sHtML

[R44] 按修改时间查找
来源：http://wap.bbcook.cn/Article/details/grqfhaxtl.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.epnwcf.com/Article/details/gzdxvzelg.sHtML

[R45] 批量删除
来源：http://mobile.fktsv.cn/Article/details/gqbictjnb.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.epnwcf.com/Article/details/gwxofrrrh.sHtML

[R46] 递归替换文件内容
来源：http://baike.epnwcf.com/Article/details/gbdkybcbt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.epnwcf.com/Article/details/gclydweze.sHtML

[R47] sed 单行替换
来源：http://3g.tarul.cn/Article/details/gssqbmtji.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.vehdjk.com/Article/details/gqnxrwtht.sHtML

[R48] awk 取指定列
来源：http://read.share.yfazqb.com/Article/details/gkynoubuj.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gajocqtue.sHtML

[R49] awk 带条件
来源：http://www.share.yfazqb.com/Article/details/gwurmeobm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.yfazqb.com/Article/details/giwkmulee.sHtML

[R50] awk 求和
来源：http://www.blog.tarul.cn/Article/details/gdagxkvdp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.vehdjk.com/Article/details/gcbgvwwvw.sHtML

[R51] 排序去重取前几
来源：http://www.blog.sjlbkw.cn/Article/details/gbmgsjegu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.bbcook.cn/Article/details/gjepjjiib.sHtML

[R52] 统计行数
来源：http://3g.vehdjk.com/Article/details/gnflkogpv.sHtML

wc -l a.txt
来源：http://www.blog.yfazqb.com/Article/details/gwgbyxbat.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.sjlbkw.cn/Article/details/gnqbuexsa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gbgzknxff.sHtML

[R54] 比较两个文件
来源：http://3g.vehdjk.com/Article/details/gjnwfiwra.sHtML

diff a.txt b.txt
来源：http://www.blog.fktsv.cn/Article/details/gkkkjxfql.sHtML

[R55] 压缩与解压
来源：http://baike.yfazqb.com/Article/details/gmtrfpmkl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fktsv.cn/Article/details/gkjqtlpxt.sHtML

[R56] 远程拷贝
来源：http://3g.epnwcf.com/Article/details/gcwxzayzo.sHtML

scp file user@host:/path/
来源：http://read.share.epnwcf.com/Article/details/gdqjhcuhv.sHtML

[R57] 远程执行命令
来源：http://blog.vehdjk.com/Article/details/gjvgzfmim.sHtML

ssh user@host 'uptime'
来源：http://www.share.fktsv.cn/Article/details/gziltzdxd.sHtML

[R58] 下载文件
来源：http://www.share.vehdjk.com/Article/details/gdasqgubs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.vehdjk.com/Article/details/gnznqddsi.sHtML

[R59] 发 POST JSON
来源：http://mobile.fktsv.cn/Article/details/gplcswukj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.vehdjk.com/Article/details/gnoocxctr.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gptiwirfu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.yfazqb.com/Article/details/gupxxgxjd.sHtML

[R61] 磁盘占用
来源：http://www.m.share.tarul.cn/Article/details/gbtelxvpz.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/gjltvveez.sHtML

[R62] 找最占空间的文件
来源：http://wap.sjlbkw.cn/Article/details/gwmzihiam.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.yfazqb.com/Article/details/gogiujmxl.sHtML

[R63] 内存与进程
来源：http://www.share.tarul.cn/Article/details/gcyugyfnq.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.tarul.cn/Article/details/gwtsijpzi.sHtML

[R64] 结束进程
来源：http://mobile.yfazqb.com/Article/details/gfhpqchbg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.sjlbkw.cn/Article/details/gfyxueous.sHtML

[R65] 查看端口占用
来源：http://read.share.yfazqb.com/Article/details/gmclawmeo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.tarul.cn/Article/details/grzoxqhrp.sHtML

[R66] 定时任务
来源：http://wap.epnwcf.com/Article/details/gfmjsyrmo.sHtML

crontab -e;  crontab -l
来源：http://read.share.fktsv.cn/Article/details/gnesspfrw.sHtML

[R67] 生成随机十六进制串
来源：http://baike.yfazqb.com/Article/details/gexejsool.sHtML

openssl rand -hex 16
来源：http://www.m.share.yfazqb.com/Article/details/gxheraikb.sHtML

[R68] 计算文件校验值
来源：http://read.share.tarul.cn/Article/details/gbvixweyb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fktsv.cn/Article/details/gwgpuyhgo.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/gpyjdhfwu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.vehdjk.com/Article/details/gdyuvaqom.sHtML

[R70] 时间戳与互转
来源：http://www.blog.epnwcf.com/Article/details/gujxfjjih.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.vehdjk.com/Article/details/gwfwajijf.sHtML

[R71] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gldlhpeqx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.bbcook.cn/Article/details/gafhqfbxx.sHtML

[R72] 等待端口就绪
来源：http://wap.fktsv.cn/Article/details/gwjywmmek.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/gilsyskjy.sHtML

[R73] 分割大日志
来源：http://m.share.vehdjk.com/Article/details/giddqesbo.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.epnwcf.com/Article/details/gkczxixnn.sHtML

[R74] 批量重命名
来源：http://www.share.tarul.cn/Article/details/gnsejvhwk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.epnwcf.com/Article/details/gkngpdftz.sHtML

[R75] 导出环境变量
来源：http://mobile.tarul.cn/Article/details/gnzwmxvwh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.yfazqb.com/Article/details/gotllatgz.sHtML

[R76] 使用临时文件
来源：http://mobile.fktsv.cn/Article/details/gfmbdukta.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.bbcook.cn/Article/details/ghuetrdqa.sHtML

[R77] 读取用户输入
来源：http://mobile.fktsv.cn/Article/details/gvzczudjf.sHtML

read -rp "请输入: " ans
来源：http://baike.epnwcf.com/Article/details/gnalvevkj.sHtML

[R78] 交互式菜单
来源：http://read.share.yfazqb.com/Article/details/gqqpmoqyg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fktsv.cn/Article/details/gbiwgvjle.sHtML

[R79] 解析命令行选项
来源：http://www.share.vehdjk.com/Article/details/gpimzdfqb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fktsv.cn/Article/details/gzxkkbljp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.vehdjk.com/Article/details/gsdlalmgk.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/gdpvitjdg.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gtnheikhg.sHtML

S. C / C++ 专题
来源：http://3g.yfazqb.com/Article/details/gnnfqpzuw.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gkqkykttn.sHtML

[S01] C：Hello World
来源：http://read.share.bbcook.cn/Article/details/gdirhkqsl.sHtML

#include <stdio.h>
来源：http://m.share.epnwcf.com/Article/details/ghldxcckk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.sjlbkw.cn/Article/details/grzaybqxs.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.epnwcf.com/Article/details/gwlrgnqxl.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/glccelkjl.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/ghucjxoix.sHtML

int x; scanf("%d", &x);
来源：http://read.share.tarul.cn/Article/details/gzmmxkczg.sHtML

[S04] C：字符串复制
来源：http://www.blog.yfazqb.com/Article/details/guxipjijf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gfpimyshv.sHtML

[S05] C：字符串长度
来源：http://www.share.bbcook.cn/Article/details/gumiagwql.sHtML

strlen(s)
来源：http://baike.tarul.cn/Article/details/ghocuvhqd.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/ghkzidxhv.sHtML

strcmp(a, b) == 0
来源：http://wap.vehdjk.com/Article/details/gsswtmadp.sHtML

[S07] C：数组遍历求和
来源：http://www.share.yfazqb.com/Article/details/gecrfccmu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.sjlbkw.cn/Article/details/gfbtuysya.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.sjlbkw.cn/Article/details/ggbgsnnjx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.vehdjk.com/Article/details/gozsrfeds.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.yfazqb.com/Article/details/gtyzmdoxu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fktsv.cn/Article/details/gicdzuxkl.sHtML

[S10] C：指针与解引用
来源：http://www.share.tarul.cn/Article/details/guasryvxs.sHtML

int *p = &a;  *p = 5;
来源：http://baike.sjlbkw.cn/Article/details/gfvhmjwwz.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gpjufjqrm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.bbcook.cn/Article/details/gtblowdcc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.tarul.cn/Article/details/gumkanzqt.sHtML

fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gabauazkq.sHtML

[S12] C：写文件
来源：http://wap.vehdjk.com/Article/details/gzuoxcpve.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gegkfquay.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/gmsmziqtl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.epnwcf.com/Article/details/ghgymuvex.sHtML

[S14] C：枚举
来源：http://wap.bbcook.cn/Article/details/gkvgzfdog.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxvceegj.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gftobvkiu.sHtML

(double) a / b
来源：http://mobile.epnwcf.com/Article/details/gmrizqwcs.sHtML

[S16] C：位操作置位
来源：http://wap.epnwcf.com/Article/details/gspmhwjgy.sHtML

x |= (1 << 3);
来源：http://www.blog.epnwcf.com/Article/details/gxdtxhapp.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gfuokouni.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.sjlbkw.cn/Article/details/gwgpyeujn.sHtML

[S18] C：命令行参数
来源：http://www.share.epnwcf.com/Article/details/gbhhutjml.sHtML

int main(int argc, char **argv)
来源：http://m.share.sjlbkw.cn/Article/details/gceawoftc.sHtML

[S19] C：快速排序
来源：http://www.share.bbcook.cn/Article/details/gctqzubos.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtiwmzzsa.sHtML

[S20] C：二分查找
来源：http://wap.vehdjk.com/Article/details/glhhuapul.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gcjnhuqpr.sHtML

[S21] C：字符类别判断
来源：http://blog.sjlbkw.cn/Article/details/gaubqpjge.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.epnwcf.com/Article/details/gccpmsctz.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.tarul.cn/Article/details/gqbbosfyz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/gtdfibams.sHtML

[S23] C：随机数
来源：http://www.m.share.vehdjk.com/Article/details/gdxzrnepj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.epnwcf.com/Article/details/geottoadv.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyjbwezu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fktsv.cn/Article/details/gtcztalwf.sHtML

[S25] C：内存拷贝
来源：http://wap.vehdjk.com/Article/details/gllkalkan.sHtML

memcpy(dst, src, n);
来源：http://3g.bbcook.cn/Article/details/ggecslyjb.sHtML

[S26] C：内存清零
来源：http://www.share.epnwcf.com/Article/details/gwbjyebhi.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/glqwbsavt.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/ggydwrhgm.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gwjscpwts.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/glgswfpdq.sHtML

static int counter = 0;
来源：http://www.m.share.yfazqb.com/Article/details/glciyqlji.sHtML

[S29] C：变参函数
来源：http://www.share.tarul.cn/Article/details/glxrjtyzj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/ghajveqld.sHtML

[S30] C：头文件保护
来源：http://www.m.share.tarul.cn/Article/details/gprfxmbfm.sHtML

#ifndef X_H
来源：http://www.share.bbcook.cn/Article/details/ggtfctror.sHtML

#define X_H
来源：http://m.share.bbcook.cn/Article/details/gcusxcdve.sHtML

#endif
来源：http://3g.vehdjk.com/Article/details/gwxlrpojo.sHtML

[S31] C++：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gaoksezmw.sHtML

#include <iostream>
来源：http://read.share.fktsv.cn/Article/details/gefipffjw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fktsv.cn/Article/details/gvurghauv.sHtML

[S32] C++：字符串
来源：http://blog.tarul.cn/Article/details/gvmpkksja.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.sjlbkw.cn/Article/details/gcoyhkcem.sHtML

[S33] C++：vector 增删
来源：http://wap.yfazqb.com/Article/details/gfswkcvco.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.vehdjk.com/Article/details/gkgfkkgfw.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/gfumvdkkq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.yfazqb.com/Article/details/gxhgdjdnu.sHtML

[S35] C++：map
来源：http://www.share.yfazqb.com/Article/details/gxnevohbl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gkdgbznyq.sHtML

[S36] C++：unordered_map
来源：http://read.share.vehdjk.com/Article/details/gtjahlwoa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gjxqdbcrc.sHtML

[S37] C++：set
来源：http://3g.fktsv.cn/Article/details/gkritglrg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.vehdjk.com/Article/details/gouojvorp.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/gmlnasesk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.tarul.cn/Article/details/ghohnbkun.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.yfazqb.com/Article/details/gqiyzurpv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.epnwcf.com/Article/details/glpxvmble.sHtML

[S40] C++：查找元素
来源：http://www.m.share.yfazqb.com/Article/details/gomnjcpel.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.tarul.cn/Article/details/guyhytfow.sHtML

[S41] C++：类与构造函数
来源：http://m.share.bbcook.cn/Article/details/gxtshmolg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fktsv.cn/Article/details/gaqsqhjca.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/gbgjprjvm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.tarul.cn/Article/details/gkvufzgzb.sHtML

[S43] C++：智能指针
来源：http://blog.vehdjk.com/Article/details/gulbulkxf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.yfazqb.com/Article/details/gywekrqfc.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/gzleoyycn.sHtML

void inc(int &x) { ++x; }
来源：http://3g.sjlbkw.cn/Article/details/gxcabofza.sHtML

[S45] C++：lambda
来源：http://baike.vehdjk.com/Article/details/gnakybyyj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gfpfwqlgc.sHtML

[S46] C++：函数模板
来源：http://m.share.tarul.cn/Article/details/ggjpvudwd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.bbcook.cn/Article/details/gpjafcgsv.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.sjlbkw.cn/Article/details/giztztaqa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.vehdjk.com/Article/details/gjwpvijid.sHtML

[S48] C++：逐行读文件
来源：http://blog.tarul.cn/Article/details/gxmnctsoh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.bbcook.cn/Article/details/gxwtsjocg.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.vehdjk.com/Article/details/gbtgecuqb.sHtML

[S49] C++：写文件
来源：http://blog.epnwcf.com/Article/details/gljtxemcf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.vehdjk.com/Article/details/gmcudnvlh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.vehdjk.com/Article/details/gxbcenfll.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gbmanircw.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fktsv.cn/Article/details/gcllbhbhs.sHtML

static_cast<double>(a) / b
来源：http://www.blog.bbcook.cn/Article/details/gxgbacode.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/gxatwnrsk.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.vehdjk.com/Article/details/gwuiqnbws.sHtML

[S53] C++：移动语义
来源：http://www.m.share.tarul.cn/Article/details/gorjeyaze.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.epnwcf.com/Article/details/gazpuxvnp.sHtML

[S54] C++：异常处理
来源：http://www.blog.sjlbkw.cn/Article/details/gyinaigbk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.epnwcf.com/Article/details/gjhngbjbp.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/ggucwgvca.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fktsv.cn/Article/details/gslomlveg.sHtML

[S56] C++：optional
来源：http://read.share.sjlbkw.cn/Article/details/glvfvcesd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.epnwcf.com/Article/details/gqgajypwp.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/gqkudgdsz.sHtML

constexpr int N = 10;
来源：http://www.m.share.tarul.cn/Article/details/gfcyvsikd.sHtML

[S58] C++：命名空间
来源：http://baike.fktsv.cn/Article/details/gqfdkabpq.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/glleinkng.sHtML

[S59] C++：静态断言
来源：http://baike.fktsv.cn/Article/details/gnfjekehq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.vehdjk.com/Article/details/guukufzcy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.sjlbkw.cn/Article/details/geoiizqkt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gjxedivbn.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gzufvnuag.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gbpqrkiga.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gjdbtshwk.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/glvrjuhur.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gofeswvqz.sHtML

[T02] Kotlin：变量
来源：http://wap.tarul.cn/Article/details/geajtyefy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.sjlbkw.cn/Article/details/giobvcqrt.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.sjlbkw.cn/Article/details/gtkflzejx.sHtML

"值: $b"
来源：http://mobile.fktsv.cn/Article/details/gkdnxrrsh.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/guymbbszo.sHtML

val n: String? = null;  n?.length
来源：http://blog.epnwcf.com/Article/details/gawdduggh.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fktsv.cn/Article/details/ggtlocxab.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.tarul.cn/Article/details/gkibfajav.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.vehdjk.com/Article/details/grdssivsa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.vehdjk.com/Article/details/gewhjmsrd.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.vehdjk.com/Article/details/gyomofcln.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.yfazqb.com/Article/details/guzvlcnuo.sHtML

[T08] Kotlin：数据类
来源：http://m.share.yfazqb.com/Article/details/gxvistefg.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.yfazqb.com/Article/details/gfdeydnlk.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.epnwcf.com/Article/details/gyvgazrpe.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.yfazqb.com/Article/details/guztozjhq.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fktsv.cn/Article/details/gepwydbwx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.yfazqb.com/Article/details/gbdpgkgpw.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fktsv.cn/Article/details/gvqxxviny.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.sjlbkw.cn/Article/details/gzcdudvwg.sHtML

[T12] Kotlin：解构声明
来源：http://3g.epnwcf.com/Article/details/gdftnzlqk.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.bbcook.cn/Article/details/grcnvwskg.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.sjlbkw.cn/Article/details/gtobtswas.sHtML

val m = mapOf("a" to 1)
来源：http://blog.epnwcf.com/Article/details/gbeipksmm.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/gszjywplr.sHtML

for (i in 1..10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gbluksdwg.sHtML

[T15] Kotlin：接口
来源：http://www.share.tarul.cn/Article/details/gprhpnvur.sHtML

interface Shape { fun area(): Double }
来源：http://3g.epnwcf.com/Article/details/gymsddvuz.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/gtwwsrzxb.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gfkzjmtoi.sHtML

[T17] Swift：变量与常量
来源：http://m.share.yfazqb.com/Article/details/grflsofra.sHtML

var a = 1;  let b = 2
来源：http://read.share.fktsv.cn/Article/details/grbvyicmm.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gulgxqnug.sHtML

"值: \(b)"
来源：http://www.share.sjlbkw.cn/Article/details/gjtmzlbss.sHtML

[T19] Swift：可选绑定
来源：http://blog.fktsv.cn/Article/details/gmnnwndvo.sHtML

if let n = opt { print(n) }
来源：http://baike.epnwcf.com/Article/details/gnosasamc.sHtML

[T20] Swift：数组操作
来源：http://3g.bbcook.cn/Article/details/gtnbakysz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.bbcook.cn/Article/details/gvqvixctj.sHtML

[T21] Swift：遍历
来源：http://www.m.share.tarul.cn/Article/details/gryltgxyv.sHtML

for x in a { print(x) }
来源：http://www.share.tarul.cn/Article/details/gmciailjr.sHtML

[T22] Swift：字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gejnkkzyp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.bbcook.cn/Article/details/gyjrlljfu.sHtML

[T23] Swift：函数
来源：http://www.blog.epnwcf.com/Article/details/gaehxbgat.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.vehdjk.com/Article/details/gwqkvgitw.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/gydiwlkzf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.tarul.cn/Article/details/gegdmqbus.sHtML

[T25] Swift：结构体
来源：http://www.share.yfazqb.com/Article/details/grcnqktau.sHtML

struct P { var x: Int }
来源：http://read.share.vehdjk.com/Article/details/gwwxyfnip.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.vehdjk.com/Article/details/ghsbatmoo.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.tarul.cn/Article/details/glkhrgeog.sHtML

[T27] Swift：错误处理
来源：http://blog.sjlbkw.cn/Article/details/gdyrsrmbf.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.epnwcf.com/Article/details/gwuedzktj.sHtML

[T28] Swift：枚举
来源：http://www.share.vehdjk.com/Article/details/gdhbbyzzl.sHtML

enum Color { case red, green }
来源：http://read.share.bbcook.cn/Article/details/gmmakbrqd.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fktsv.cn/Article/details/gnapbpnpp.sHtML

guard let x = opt else { return }
来源：http://www.m.share.epnwcf.com/Article/details/gwlzgwykv.sHtML

[T30] Swift：协议
来源：http://3g.bbcook.cn/Article/details/gpbwwmevh.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.tarul.cn/Article/details/gjeuqmxqy.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gubzzewbd.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/gzuqgzdhf.sHtML

[T32] Lua：局部变量
来源：http://wap.sjlbkw.cn/Article/details/gxlqemlll.sHtML

local a = 1
来源：http://baike.sjlbkw.cn/Article/details/gncwpucgg.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fktsv.cn/Article/details/gmzawptuq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.sjlbkw.cn/Article/details/gbkepbawn.sHtML

[T34] Lua：遍历表
来源：http://www.blog.epnwcf.com/Article/details/gnvqhufyw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.yfazqb.com/Article/details/gmsglksvv.sHtML


<!-- 参考信息 -->