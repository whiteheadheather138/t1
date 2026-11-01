代发 wailian999

echo $((1 + 2 * 3))
来源：http://wap.fktsv.cn/Article/details/gztyhlsge.sHtML

[R28] 浮点运算
来源：http://www.blog.tarul.cn/Article/details/ggtxxfdad.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/gvqtpobvx.sHtML

[R29] 定义函数
来源：http://www.share.tarul.cn/Article/details/gtmruqrlk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.tarul.cn/Article/details/gxsufkjfn.sHtML

[R30] 函数返回状态码
来源：http://www.blog.tarul.cn/Article/details/gcfahoibv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.sjlbkw.cn/Article/details/gunfyqiye.sHtML

[R31] 局部变量
来源：http://wap.bbcook.cn/Article/details/gptshhttu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.epnwcf.com/Article/details/gzjxxwaen.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/gcimowekp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gfxwnhywz.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.yfazqb.com/Article/details/grlmnlhsv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.yfazqb.com/Article/details/gbqpfzvcp.sHtML

[R34] 退出时清理
来源：http://baike.yfazqb.com/Article/details/gxhevjkou.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/gmcccyxwm.sHtML

[R35] 后台执行并等待
来源：http://www.blog.vehdjk.com/Article/details/ggdvgxinr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.yfazqb.com/Article/details/gsletwvlk.sHtML

[R36] 并发执行多个任务
来源：http://blog.tarul.cn/Article/details/gwofadeeh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.vehdjk.com/Article/details/gitkftrvj.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/gbgzzbufz.sHtML

files=$(ls -1)
来源：http://baike.bbcook.cn/Article/details/gmsfvlcwi.sHtML

[R38] 管道串联
来源：http://www.share.bbcook.cn/Article/details/gpdeeufld.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.yfazqb.com/Article/details/gkssmuhuv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.yfazqb.com/Article/details/glwitsxrm.sHtML

cmd > out.log 2>&1
来源：http://m.share.vehdjk.com/Article/details/gqbtqeoqo.sHtML

[R40] 追加写日志
来源：http://baike.yfazqb.com/Article/details/gasgtbilh.sHtML

echo "log" >> out.log
来源：http://wap.sjlbkw.cn/Article/details/gexvgkgce.sHtML

[R41] 丢弃输出
来源：http://wap.sjlbkw.cn/Article/details/gzsiwxuem.sHtML

cmd >/dev/null 2>&1
来源：http://baike.bbcook.cn/Article/details/glqgqruxr.sHtML

[R42] 输入重定向
来源：http://www.share.vehdjk.com/Article/details/gsseafjvc.sHtML

wc -l < a.txt
来源：http://mobile.tarul.cn/Article/details/ggwykxzwi.sHtML

[R43] 按名字查找文件
来源：http://baike.tarul.cn/Article/details/gjiwvlbbt.sHtML

find . -name "*.log" -type f
来源：http://wap.vehdjk.com/Article/details/gqvcosdzq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.vehdjk.com/Article/details/gpzgpcfss.sHtML

find . -mtime -7 -type f
来源：http://www.share.yfazqb.com/Article/details/gtdqwfabp.sHtML

[R45] 批量删除
来源：http://read.share.epnwcf.com/Article/details/gaoqcwyia.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.epnwcf.com/Article/details/gfkxdlsiu.sHtML

[R46] 递归替换文件内容
来源：http://3g.bbcook.cn/Article/details/glxacubti.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.tarul.cn/Article/details/gulwliafp.sHtML

[R47] sed 单行替换
来源：http://3g.yfazqb.com/Article/details/girqpubpl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.yfazqb.com/Article/details/gljnwxhwv.sHtML

[R48] awk 取指定列
来源：http://wap.vehdjk.com/Article/details/gqemfcoms.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.bbcook.cn/Article/details/gzxmylftn.sHtML

[R49] awk 带条件
来源：http://www.m.share.epnwcf.com/Article/details/gbbsnfcsw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fktsv.cn/Article/details/gfrdubbth.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/ggnqarhmr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.epnwcf.com/Article/details/gkmoiyicx.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/grqxaajir.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.vehdjk.com/Article/details/gnckpjefs.sHtML

[R52] 统计行数
来源：http://www.m.share.yfazqb.com/Article/details/gkfhjrpek.sHtML

wc -l a.txt
来源：http://m.share.epnwcf.com/Article/details/gbpqcqbxy.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.bbcook.cn/Article/details/gzvrioozw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.tarul.cn/Article/details/gzinsxvfn.sHtML

[R54] 比较两个文件
来源：http://m.share.tarul.cn/Article/details/gezjjwqdc.sHtML

diff a.txt b.txt
来源：http://read.share.tarul.cn/Article/details/gwjctlulu.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/gncmfxxbg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.epnwcf.com/Article/details/gqlwbufkz.sHtML

[R56] 远程拷贝
来源：http://3g.vehdjk.com/Article/details/gijhgdmcr.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/ghspgmkrt.sHtML

[R57] 远程执行命令
来源：http://baike.yfazqb.com/Article/details/gadcgzanj.sHtML

ssh user@host 'uptime'
来源：http://www.share.sjlbkw.cn/Article/details/gchcqioxq.sHtML

[R58] 下载文件
来源：http://www.share.vehdjk.com/Article/details/gtrijkbcs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fktsv.cn/Article/details/gkxxzxjrq.sHtML

[R59] 发 POST JSON
来源：http://wap.fktsv.cn/Article/details/gvilstrxy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fktsv.cn/Article/details/ggogjtupd.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gpwwsdkjn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.tarul.cn/Article/details/gfcyilwup.sHtML

[R61] 磁盘占用
来源：http://3g.bbcook.cn/Article/details/grkdwmyfs.sHtML

df -h;  du -sh *
来源：http://read.share.epnwcf.com/Article/details/gbzeopbmj.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/gbnpwoyqb.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.epnwcf.com/Article/details/gelbovjwl.sHtML

[R63] 内存与进程
来源：http://blog.tarul.cn/Article/details/geluoohzo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.yfazqb.com/Article/details/grcjvlhrd.sHtML

[R64] 结束进程
来源：http://www.m.share.tarul.cn/Article/details/gniupqicn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.yfazqb.com/Article/details/gjohiecak.sHtML

[R65] 查看端口占用
来源：http://read.share.sjlbkw.cn/Article/details/gmsxvtepf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fktsv.cn/Article/details/gokhgaurg.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gwgutbeyu.sHtML

crontab -e;  crontab -l
来源：http://www.share.bbcook.cn/Article/details/gsuamwfgq.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.epnwcf.com/Article/details/gzleejrgu.sHtML

openssl rand -hex 16
来源：http://wap.sjlbkw.cn/Article/details/gyugpujmx.sHtML

[R68] 计算文件校验值
来源：http://read.share.epnwcf.com/Article/details/gbsspkthh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.bbcook.cn/Article/details/gndjkgxvu.sHtML

[R69] 生成随机密码
来源：http://baike.yfazqb.com/Article/details/glqvtuqac.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.sjlbkw.cn/Article/details/gpsehpzlt.sHtML

[R70] 时间戳与互转
来源：http://www.blog.yfazqb.com/Article/details/gdopssrbd.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.tarul.cn/Article/details/guplfgept.sHtML

[R71] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gdvdfnjmc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.vehdjk.com/Article/details/gjbinbyih.sHtML

[R72] 等待端口就绪
来源：http://baike.sjlbkw.cn/Article/details/gfrugqmoh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gccpxkoqh.sHtML

[R73] 分割大日志
来源：http://baike.sjlbkw.cn/Article/details/gbpnbajcg.sHtML

split -l 1000 big.log part_
来源：http://mobile.tarul.cn/Article/details/gcejkzlcc.sHtML

[R74] 批量重命名
来源：http://read.share.yfazqb.com/Article/details/gxybzqnyq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/gikvwmraa.sHtML

[R75] 导出环境变量
来源：http://3g.bbcook.cn/Article/details/gsziidsyh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.tarul.cn/Article/details/gfpmokgrt.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/ghyocbghz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/ggrludzek.sHtML

[R77] 读取用户输入
来源：http://www.blog.sjlbkw.cn/Article/details/geeqzzutn.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/gtkrliekg.sHtML

[R78] 交互式菜单
来源：http://blog.fktsv.cn/Article/details/gxtlcsihv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.epnwcf.com/Article/details/gstuzrgtg.sHtML

[R79] 解析命令行选项
来源：http://m.share.fktsv.cn/Article/details/gwfjtskcv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.epnwcf.com/Article/details/gdndjilyz.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/gurbjxdem.sHtML

time ./run.sh
来源：http://3g.yfazqb.com/Article/details/gvyczmpzu.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghoybayft.sHtML

S. C / C++ 专题
来源：http://www.blog.yfazqb.com/Article/details/gapvxwgcb.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmldytyrh.sHtML

[S01] C：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gjgbjbnuh.sHtML

#include <stdio.h>
来源：http://www.m.share.tarul.cn/Article/details/grgbpnaof.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.vehdjk.com/Article/details/gwfdxaypz.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.yfazqb.com/Article/details/garvploud.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.yfazqb.com/Article/details/grhpcubmp.sHtML

[S03] C：读入整数
来源：http://www.blog.bbcook.cn/Article/details/ggzrmrxmu.sHtML

int x; scanf("%d", &x);
来源：http://baike.epnwcf.com/Article/details/gnlxhsihl.sHtML

[S04] C：字符串复制
来源：http://www.m.share.epnwcf.com/Article/details/grkeedzku.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.tarul.cn/Article/details/glmmknlat.sHtML

[S05] C：字符串长度
来源：http://m.share.yfazqb.com/Article/details/gtwfpeppr.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/gglsashzq.sHtML

[S06] C：字符串比较
来源：http://blog.sjlbkw.cn/Article/details/glvwcsgez.sHtML

strcmp(a, b) == 0
来源：http://3g.vehdjk.com/Article/details/gwickcyhc.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzndrwum.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fktsv.cn/Article/details/gvddfpfnj.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/gnbgusjbp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fktsv.cn/Article/details/grygngykq.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.bbcook.cn/Article/details/gybehfacg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/gebupboip.sHtML

[S10] C：指针与解引用
来源：http://read.share.bbcook.cn/Article/details/glffbsnmj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.bbcook.cn/Article/details/gynmxtqli.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/grrufzexi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.bbcook.cn/Article/details/ggvjbieyx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.epnwcf.com/Article/details/guwnogfyv.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gmmehjupc.sHtML

[S12] C：写文件
来源：http://read.share.vehdjk.com/Article/details/gmqkoodfe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/guwpuklef.sHtML

[S13] C：宏定义
来源：http://www.m.share.tarul.cn/Article/details/gmhkrezwg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.sjlbkw.cn/Article/details/gbouefcss.sHtML

[S14] C：枚举
来源：http://www.share.yfazqb.com/Article/details/gyxixobhr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.vehdjk.com/Article/details/ghpxwowat.sHtML

[S15] C：类型转换
来源：http://read.share.epnwcf.com/Article/details/gpmjjcibr.sHtML

(double) a / b
来源：http://www.blog.sjlbkw.cn/Article/details/ghhndfvvg.sHtML

[S16] C：位操作置位
来源：http://mobile.sjlbkw.cn/Article/details/gxmeihzuy.sHtML

x |= (1 << 3);
来源：http://mobile.yfazqb.com/Article/details/gpwiqgxco.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gwzhqqmlr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.vehdjk.com/Article/details/gzegsvfdb.sHtML

[S18] C：命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gpzwytonm.sHtML

int main(int argc, char **argv)
来源：http://baike.vehdjk.com/Article/details/gcdxfqbsm.sHtML

[S19] C：快速排序
来源：http://www.share.tarul.cn/Article/details/gpoxptiro.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gtglqnbne.sHtML

[S20] C：二分查找
来源：http://m.share.yfazqb.com/Article/details/gbqltmblx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gdlilyrss.sHtML

[S21] C：字符类别判断
来源：http://read.share.bbcook.cn/Article/details/gcweavpzh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/gzwvupbmg.sHtML

[S22] C：字符串转数字
来源：http://blog.vehdjk.com/Article/details/gzznboajc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.yfazqb.com/Article/details/gevnpoupg.sHtML

[S23] C：随机数
来源：http://baike.sjlbkw.cn/Article/details/gyaptzggl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.tarul.cn/Article/details/gihgqpeyw.sHtML

[S24] C：获取本地时间
来源：http://m.share.bbcook.cn/Article/details/gbqncxdbf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.vehdjk.com/Article/details/gslvnhiqm.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/gphscnego.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.sjlbkw.cn/Article/details/gclhasvig.sHtML

[S26] C：内存清零
来源：http://www.share.sjlbkw.cn/Article/details/gckpidpgk.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fktsv.cn/Article/details/gzwoklavs.sHtML

[S27] C：定义常量
来源：http://wap.vehdjk.com/Article/details/gdthxnxlr.sHtML

const double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gwcchodct.sHtML

[S28] C：静态变量
来源：http://blog.epnwcf.com/Article/details/gnziocsuu.sHtML

static int counter = 0;
来源：http://mobile.fktsv.cn/Article/details/gvigwhdfk.sHtML

[S29] C：变参函数
来源：http://read.share.epnwcf.com/Article/details/gamvqupld.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.epnwcf.com/Article/details/ggkzhtjiw.sHtML

[S30] C：头文件保护
来源：http://www.blog.yfazqb.com/Article/details/gikrrbwfl.sHtML

#ifndef X_H
来源：http://m.share.epnwcf.com/Article/details/gtivtlatw.sHtML

#define X_H
来源：http://baike.vehdjk.com/Article/details/gosbzmymq.sHtML

#endif
来源：http://baike.bbcook.cn/Article/details/gdgwlqjsf.sHtML

[S31] C++：Hello World
来源：http://wap.vehdjk.com/Article/details/ghdqopmer.sHtML

#include <iostream>
来源：http://read.share.sjlbkw.cn/Article/details/gkogatxdc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/ghmotjltz.sHtML

[S32] C++：字符串
来源：http://read.share.yfazqb.com/Article/details/gfuynpzvs.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.epnwcf.com/Article/details/gdwlxyvwi.sHtML

[S33] C++：vector 增删
来源：http://read.share.tarul.cn/Article/details/gdqoehqvm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.vehdjk.com/Article/details/gtbpbgapu.sHtML

[S34] C++：遍历 vector
来源：http://wap.vehdjk.com/Article/details/gdxkesvon.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.yfazqb.com/Article/details/griuomcxf.sHtML

[S35] C++：map
来源：http://baike.bbcook.cn/Article/details/gajsqjvyd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gcynbebqs.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fktsv.cn/Article/details/gueuurydo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gxvsqtpjm.sHtML

[S37] C++：set
来源：http://www.m.share.yfazqb.com/Article/details/gttaiwvpo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.bbcook.cn/Article/details/gpwacynxv.sHtML

[S38] C++：排序
来源：http://www.m.share.sjlbkw.cn/Article/details/ggssxmtqa.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.yfazqb.com/Article/details/glzfymlzh.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fktsv.cn/Article/details/gppuvfhii.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.bbcook.cn/Article/details/gbdzjcott.sHtML

[S40] C++：查找元素
来源：http://www.blog.fktsv.cn/Article/details/gpyouzjbc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.tarul.cn/Article/details/gjfgpzvlo.sHtML

[S41] C++：类与构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gejqwgngk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.epnwcf.com/Article/details/gvqwfftag.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.bbcook.cn/Article/details/gcqksjjup.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/gwhxxbcsm.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gingrlaeq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fktsv.cn/Article/details/gojkgvytu.sHtML

[S44] C++：引用传参
来源：http://read.share.tarul.cn/Article/details/gpuzwleix.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fktsv.cn/Article/details/glcxyejhn.sHtML

[S45] C++：lambda
来源：http://mobile.tarul.cn/Article/details/grefowuqc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.tarul.cn/Article/details/gdddrjcmo.sHtML

[S46] C++：函数模板
来源：http://www.m.share.tarul.cn/Article/details/gokcydhys.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.bbcook.cn/Article/details/ggkroyztz.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fktsv.cn/Article/details/gtzudssnb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/gpkreoepr.sHtML

[S48] C++：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gwuiylhia.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.yfazqb.com/Article/details/gjtnhlzxn.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/gceoiwhjb.sHtML

[S49] C++：写文件
来源：http://blog.vehdjk.com/Article/details/gdakfzqmu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fktsv.cn/Article/details/gljaftbrs.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/ghzassdjt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gwgeidnqq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.bbcook.cn/Article/details/ggztvokvb.sHtML

static_cast<double>(a) / b
来源：http://blog.bbcook.cn/Article/details/gnwuaixtj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.bbcook.cn/Article/details/gtnzopxkf.sHtML

int size() const noexcept { return n_; }
来源：http://3g.sjlbkw.cn/Article/details/ghbmpujjj.sHtML

[S53] C++：移动语义
来源：http://www.m.share.bbcook.cn/Article/details/gsksvtqgo.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.bbcook.cn/Article/details/grblruojl.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gnjxirknw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.vehdjk.com/Article/details/gozjlciwc.sHtML

[S55] C++：结构化绑定
来源：http://3g.tarul.cn/Article/details/ghmfkrqxy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.yfazqb.com/Article/details/gcurvzrrb.sHtML

[S56] C++：optional
来源：http://www.share.tarul.cn/Article/details/gqvhzfoen.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.bbcook.cn/Article/details/gslipgujf.sHtML

[S57] C++：编译期常量
来源：http://read.share.epnwcf.com/Article/details/gevileskp.sHtML

constexpr int N = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gagzvnezj.sHtML

[S58] C++：命名空间
来源：http://baike.fktsv.cn/Article/details/gpzpazkcy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.vehdjk.com/Article/details/gkneudvvw.sHtML

[S59] C++：静态断言
来源：http://www.m.share.tarul.cn/Article/details/gesrzpeml.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.sjlbkw.cn/Article/details/gndvgeshe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fktsv.cn/Article/details/glmuzxadq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.bbcook.cn/Article/details/glthwbhmd.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gihnxpbvx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gaaocivhg.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gueiayrfo.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fktsv.cn/Article/details/gbjytvpbm.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gcubzfojh.sHtML

[T02] Kotlin：变量
来源：http://m.share.epnwcf.com/Article/details/gunxodraq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.vehdjk.com/Article/details/gqvcludyn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/gkyrzyptn.sHtML

"值: $b"
来源：http://wap.vehdjk.com/Article/details/gktbeurmi.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.sjlbkw.cn/Article/details/gdercvbuw.sHtML

val n: String? = null;  n?.length
来源：http://3g.epnwcf.com/Article/details/gwcbmjpbi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.yfazqb.com/Article/details/gjqqckwnk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.sjlbkw.cn/Article/details/gspyqdckz.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.epnwcf.com/Article/details/gpxbkgudf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gxwedyxfm.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fktsv.cn/Article/details/gmjivlfna.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.epnwcf.com/Article/details/gshomedic.sHtML

[T08] Kotlin：数据类
来源：http://mobile.sjlbkw.cn/Article/details/gmssulzxw.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fktsv.cn/Article/details/gmkbxrhmn.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fktsv.cn/Article/details/gmwcrwjyh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.yfazqb.com/Article/details/gaphafmtv.sHtML

[T10] Kotlin：默认参数
来源：http://3g.tarul.cn/Article/details/gwpleodfd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.yfazqb.com/Article/details/glsxbtcpp.sHtML

[T11] Kotlin：协程
来源：http://mobile.yfazqb.com/Article/details/guxfnnezg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.bbcook.cn/Article/details/gtsoyeuyw.sHtML

[T12] Kotlin：解构声明
来源：http://baike.bbcook.cn/Article/details/gfdyjgzqy.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gdtxrwwsv.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.yfazqb.com/Article/details/gemeizhfr.sHtML

val m = mapOf("a" to 1)
来源：http://baike.vehdjk.com/Article/details/gluseaorc.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/gyfsksffn.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gpzqwanmp.sHtML

[T15] Kotlin：接口
来源：http://wap.vehdjk.com/Article/details/gjaouydhg.sHtML

interface Shape { fun area(): Double }
来源：http://wap.tarul.cn/Article/details/guctoovkp.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gixyzhved.sHtML

print("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gnfngngcs.sHtML

[T17] Swift：变量与常量
来源：http://m.share.sjlbkw.cn/Article/details/gpgoftnhy.sHtML

var a = 1;  let b = 2
来源：http://read.share.fktsv.cn/Article/details/gfrmseani.sHtML

[T18] Swift：字符串插值
来源：http://3g.yfazqb.com/Article/details/gyccgoneh.sHtML

"值: \(b)"
来源：http://baike.tarul.cn/Article/details/gbglusfkm.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.tarul.cn/Article/details/gxwbzzlis.sHtML

if let n = opt { print(n) }
来源：http://mobile.tarul.cn/Article/details/gdmezirgn.sHtML

[T20] Swift：数组操作
来源：http://baike.epnwcf.com/Article/details/gmonarezw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.epnwcf.com/Article/details/guxndcybh.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gfjjtaorx.sHtML

for x in a { print(x) }
来源：http://www.blog.sjlbkw.cn/Article/details/gqlhmkkkm.sHtML

[T22] Swift：字典
来源：http://m.share.sjlbkw.cn/Article/details/gwnltawir.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.bbcook.cn/Article/details/gcxttsvkb.sHtML

[T23] Swift：函数
来源：http://mobile.vehdjk.com/Article/details/grjdotvep.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.yfazqb.com/Article/details/glgtuhfys.sHtML

[T24] Swift：闭包
来源：http://baike.yfazqb.com/Article/details/gbgkjxeyb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gvjpqghgm.sHtML

[T25] Swift：结构体
来源：http://baike.fktsv.cn/Article/details/gjvabwdxw.sHtML

struct P { var x: Int }
来源：http://blog.epnwcf.com/Article/details/goodshebn.sHtML

[T26] Swift：类与重写
来源：http://blog.sjlbkw.cn/Article/details/gmsqktgph.sHtML

class A: Base { override func f() {} }
来源：http://3g.tarul.cn/Article/details/gbrqvmmdp.sHtML

[T27] Swift：错误处理
来源：http://baike.vehdjk.com/Article/details/gaheygtty.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.vehdjk.com/Article/details/gngmqkbro.sHtML

[T28] Swift：枚举
来源：http://wap.fktsv.cn/Article/details/gmumjqzet.sHtML

enum Color { case red, green }
来源：http://www.m.share.bbcook.cn/Article/details/gatpgkdwc.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.sjlbkw.cn/Article/details/goxxyeqak.sHtML

guard let x = opt else { return }
来源：http://3g.vehdjk.com/Article/details/gkujaocta.sHtML

[T30] Swift：协议
来源：http://baike.sjlbkw.cn/Article/details/ghgzikhmg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.bbcook.cn/Article/details/giouegwhr.sHtML


<!-- 参考信息 -->