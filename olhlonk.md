代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.sjlbkw.cn/Article/details/gsgdihaxd.sHtML

[R26] 命令替换
来源：http://baike.epnwcf.com/Article/details/gpmdjayqt.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.bbcook.cn/Article/details/gmvjrmqzl.sHtML

[R27] 算术展开
来源：http://www.share.yfazqb.com/Article/details/gjopmgmeb.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fktsv.cn/Article/details/gkcaqytcw.sHtML

[R28] 浮点运算
来源：http://www.share.epnwcf.com/Article/details/giwkgumfa.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fktsv.cn/Article/details/gcdwdblio.sHtML

[R29] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gyjxyjtgq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fktsv.cn/Article/details/gulftannk.sHtML

[R30] 函数返回状态码
来源：http://wap.bbcook.cn/Article/details/gmcsmzrez.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.sjlbkw.cn/Article/details/gnsiheule.sHtML

[R31] 局部变量
来源：http://mobile.tarul.cn/Article/details/ggfesgjwv.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fktsv.cn/Article/details/gdbjkcpnf.sHtML

[R32] 参数个数校验
来源：http://www.blog.bbcook.cn/Article/details/gglhacwoh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gayiepgdd.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.vehdjk.com/Article/details/gjmmqalge.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.tarul.cn/Article/details/ghhxoiydp.sHtML

[R34] 退出时清理
来源：http://read.share.epnwcf.com/Article/details/gsrismddl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/gizenwzel.sHtML

[R35] 后台执行并等待
来源：http://www.share.vehdjk.com/Article/details/goewzaehx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.bbcook.cn/Article/details/gulozyagl.sHtML

[R36] 并发执行多个任务
来源：http://wap.tarul.cn/Article/details/gcotjjqwg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fktsv.cn/Article/details/ghtqfwuiw.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fktsv.cn/Article/details/ginarvhyw.sHtML

files=$(ls -1)
来源：http://read.share.tarul.cn/Article/details/gzdpenbre.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/ghlkzbixb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.tarul.cn/Article/details/gekzwkswg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.bbcook.cn/Article/details/gwajordqo.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fktsv.cn/Article/details/ghylsksha.sHtML

[R40] 追加写日志
来源：http://wap.epnwcf.com/Article/details/gxlcdgqwh.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/gxtsbdufq.sHtML

[R41] 丢弃输出
来源：http://www.m.share.bbcook.cn/Article/details/gijcaxywb.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.epnwcf.com/Article/details/gjaqpmfxy.sHtML

[R42] 输入重定向
来源：http://mobile.tarul.cn/Article/details/gmhzqsycw.sHtML

wc -l < a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gtkzbltad.sHtML

[R43] 按名字查找文件
来源：http://www.blog.epnwcf.com/Article/details/gvffnccma.sHtML

find . -name "*.log" -type f
来源：http://read.share.fktsv.cn/Article/details/gguoskthf.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/gxpdpdunc.sHtML

find . -mtime -7 -type f
来源：http://wap.epnwcf.com/Article/details/gnxnhpznf.sHtML

[R45] 批量删除
来源：http://www.m.share.yfazqb.com/Article/details/genlazjmr.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/gtkhhsfrm.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.vehdjk.com/Article/details/gljqvpwyo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.vehdjk.com/Article/details/gthwqlvlb.sHtML

[R47] sed 单行替换
来源：http://blog.yfazqb.com/Article/details/gjyxqzwcn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.yfazqb.com/Article/details/gtitwpkwd.sHtML

[R48] awk 取指定列
来源：http://www.share.yfazqb.com/Article/details/gmjqrsbis.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gtehnwxln.sHtML

[R49] awk 带条件
来源：http://www.blog.bbcook.cn/Article/details/gfejptymu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.bbcook.cn/Article/details/gdakniqxk.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/ggnsbtohp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gzpaaolos.sHtML

[R51] 排序去重取前几
来源：http://read.share.vehdjk.com/Article/details/gimrzirhm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fktsv.cn/Article/details/gkarhctgc.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/grreapmgl.sHtML

wc -l a.txt
来源：http://read.share.epnwcf.com/Article/details/gtcoplcht.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.tarul.cn/Article/details/gnutayqls.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.vehdjk.com/Article/details/gqoxnggmx.sHtML

[R54] 比较两个文件
来源：http://www.share.yfazqb.com/Article/details/gronxcezt.sHtML

diff a.txt b.txt
来源：http://blog.sjlbkw.cn/Article/details/gshvuqvaf.sHtML

[R55] 压缩与解压
来源：http://mobile.vehdjk.com/Article/details/gddytzohn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.epnwcf.com/Article/details/ghyzptmiz.sHtML

[R56] 远程拷贝
来源：http://www.share.vehdjk.com/Article/details/gmgwkwsuk.sHtML

scp file user@host:/path/
来源：http://read.share.fktsv.cn/Article/details/guyktzxkv.sHtML

[R57] 远程执行命令
来源：http://blog.epnwcf.com/Article/details/gfwzkqimv.sHtML

ssh user@host 'uptime'
来源：http://baike.fktsv.cn/Article/details/gfllvbpjt.sHtML

[R58] 下载文件
来源：http://m.share.yfazqb.com/Article/details/gvkhjlych.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.bbcook.cn/Article/details/gzvoyytlc.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/gqfjltwtj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.epnwcf.com/Article/details/gbvnphjgs.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gokkjfgkh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.vehdjk.com/Article/details/glrgbuhja.sHtML

[R61] 磁盘占用
来源：http://mobile.yfazqb.com/Article/details/gjjkzufjn.sHtML

df -h;  du -sh *
来源：http://read.share.tarul.cn/Article/details/ggchsrvrq.sHtML

[R62] 找最占空间的文件
来源：http://mobile.bbcook.cn/Article/details/gsnbhwbxi.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fktsv.cn/Article/details/gufvxeskj.sHtML

[R63] 内存与进程
来源：http://read.share.sjlbkw.cn/Article/details/gqxbaiksn.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.vehdjk.com/Article/details/gwaziweim.sHtML

[R64] 结束进程
来源：http://3g.fktsv.cn/Article/details/gtyfmvjhr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.sjlbkw.cn/Article/details/gefwcqdvn.sHtML

[R65] 查看端口占用
来源：http://read.share.sjlbkw.cn/Article/details/gqugzzcjk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fktsv.cn/Article/details/gnhcpeumh.sHtML

[R66] 定时任务
来源：http://m.share.yfazqb.com/Article/details/gtljffgpg.sHtML

crontab -e;  crontab -l
来源：http://wap.bbcook.cn/Article/details/gfmiulsqy.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fktsv.cn/Article/details/gszuiqfed.sHtML

openssl rand -hex 16
来源：http://read.share.epnwcf.com/Article/details/gtgrtebet.sHtML

[R68] 计算文件校验值
来源：http://blog.vehdjk.com/Article/details/ggxwvubsf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.epnwcf.com/Article/details/gpsqgbzjw.sHtML

[R69] 生成随机密码
来源：http://blog.fktsv.cn/Article/details/ghgpzifth.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.vehdjk.com/Article/details/gdouhqopy.sHtML

[R70] 时间戳与互转
来源：http://baike.yfazqb.com/Article/details/grsfrtagu.sHtML

date +%s;  date -d @1700000000
来源：http://3g.sjlbkw.cn/Article/details/gowfsmoro.sHtML

[R71] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gpqcwmbhn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.tarul.cn/Article/details/gmdjwpzzz.sHtML

[R72] 等待端口就绪
来源：http://3g.fktsv.cn/Article/details/gvpudxqmh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gxwznrxob.sHtML

[R73] 分割大日志
来源：http://mobile.vehdjk.com/Article/details/gxevfhasm.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.tarul.cn/Article/details/glsepjbbe.sHtML

[R74] 批量重命名
来源：http://mobile.tarul.cn/Article/details/gcxrlewsv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.yfazqb.com/Article/details/gbhgzjhyi.sHtML

[R75] 导出环境变量
来源：http://m.share.fktsv.cn/Article/details/gddpiijcm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fktsv.cn/Article/details/glevpurom.sHtML

[R76] 使用临时文件
来源：http://wap.vehdjk.com/Article/details/giimncnax.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gxsenxusf.sHtML

[R77] 读取用户输入
来源：http://read.share.sjlbkw.cn/Article/details/gwdxfgwit.sHtML

read -rp "请输入: " ans
来源：http://www.share.yfazqb.com/Article/details/gjrqkikyd.sHtML

[R78] 交互式菜单
来源：http://blog.vehdjk.com/Article/details/gerointnh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.sjlbkw.cn/Article/details/gxcljkvmc.sHtML

[R79] 解析命令行选项
来源：http://blog.epnwcf.com/Article/details/gmozemmsk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.yfazqb.com/Article/details/glmfwgjhn.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fktsv.cn/Article/details/gexqxiuvq.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gnjzrdjpj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gitaeneeq.sHtML

S. C / C++ 专题
来源：http://www.m.share.epnwcf.com/Article/details/grdqlrgjj.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gioocijew.sHtML

[S01] C：Hello World
来源：http://read.share.tarul.cn/Article/details/gnhezdjvm.sHtML

#include <stdio.h>
来源：http://3g.epnwcf.com/Article/details/ggzpkndum.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.yfazqb.com/Article/details/gxnhihcvt.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.yfazqb.com/Article/details/guzgmxgss.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fktsv.cn/Article/details/grfedvqiu.sHtML

[S03] C：读入整数
来源：http://www.m.share.vehdjk.com/Article/details/gzksytpch.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.epnwcf.com/Article/details/gtrqqahfm.sHtML

[S04] C：字符串复制
来源：http://m.share.vehdjk.com/Article/details/gsenjgshw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.yfazqb.com/Article/details/gyckaglnt.sHtML

[S05] C：字符串长度
来源：http://3g.fktsv.cn/Article/details/gpguvcezu.sHtML

strlen(s)
来源：http://blog.epnwcf.com/Article/details/gsevqlwfc.sHtML

[S06] C：字符串比较
来源：http://mobile.vehdjk.com/Article/details/gotplpuzl.sHtML

strcmp(a, b) == 0
来源：http://read.share.epnwcf.com/Article/details/gcsfrbktn.sHtML

[S07] C：数组遍历求和
来源：http://wap.epnwcf.com/Article/details/gcdpsdmmd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.tarul.cn/Article/details/ghtugtpdv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.epnwcf.com/Article/details/gmfxtumhu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.bbcook.cn/Article/details/gakqxjeqq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.bbcook.cn/Article/details/gculnaage.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.yfazqb.com/Article/details/ggpwzawzc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.vehdjk.com/Article/details/gtnjotrmw.sHtML

int *p = &a;  *p = 5;
来源：http://3g.sjlbkw.cn/Article/details/gjtjnvwno.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/goinlrnet.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.vehdjk.com/Article/details/gntqrwkmm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.bbcook.cn/Article/details/glilxnbrz.sHtML

fclose(f);
来源：http://wap.tarul.cn/Article/details/gxsjukouz.sHtML

[S12] C：写文件
来源：http://baike.fktsv.cn/Article/details/gylckrbae.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gzeoofzdt.sHtML

[S13] C：宏定义
来源：http://www.share.tarul.cn/Article/details/gwcbxfuoj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.bbcook.cn/Article/details/gphfwacvb.sHtML

[S14] C：枚举
来源：http://3g.yfazqb.com/Article/details/gzihwagxj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fktsv.cn/Article/details/gjrvqasol.sHtML

[S15] C：类型转换
来源：http://baike.sjlbkw.cn/Article/details/gwpdybtpq.sHtML

(double) a / b
来源：http://mobile.epnwcf.com/Article/details/grpsquhye.sHtML

[S16] C：位操作置位
来源：http://www.blog.fktsv.cn/Article/details/gdzdytijp.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/gorlkaeak.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.epnwcf.com/Article/details/ggdcmjcvi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.yfazqb.com/Article/details/gejgsesdy.sHtML

[S18] C：命令行参数
来源：http://www.blog.vehdjk.com/Article/details/guakkxbwa.sHtML

int main(int argc, char **argv)
来源：http://baike.vehdjk.com/Article/details/gpdkpvovg.sHtML

[S19] C：快速排序
来源：http://wap.tarul.cn/Article/details/gczduacar.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gvukvbejz.sHtML

[S20] C：二分查找
来源：http://read.share.epnwcf.com/Article/details/gpuusyhec.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/glhxnehaj.sHtML

[S21] C：字符类别判断
来源：http://www.share.epnwcf.com/Article/details/gfuhvtxfx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.tarul.cn/Article/details/gdkzzunur.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/gacsefqkq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.yfazqb.com/Article/details/gypjomcjo.sHtML

[S23] C：随机数
来源：http://wap.epnwcf.com/Article/details/gstabrgom.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.tarul.cn/Article/details/gtqoncdbi.sHtML

[S24] C：获取本地时间
来源：http://read.share.fktsv.cn/Article/details/guduicxnp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.epnwcf.com/Article/details/gwxsucoht.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/gznxqtnxj.sHtML

memcpy(dst, src, n);
来源：http://blog.vehdjk.com/Article/details/gnjxpwhww.sHtML

[S26] C：内存清零
来源：http://mobile.bbcook.cn/Article/details/gsjuyuqyg.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gzwiokqjh.sHtML

[S27] C：定义常量
来源：http://www.share.tarul.cn/Article/details/gckbmuojr.sHtML

const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gcwweklge.sHtML

[S28] C：静态变量
来源：http://3g.sjlbkw.cn/Article/details/gjiyelrvj.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/ggobyrcmr.sHtML

[S29] C：变参函数
来源：http://read.share.sjlbkw.cn/Article/details/gimoyeppu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.tarul.cn/Article/details/gwaxpuoin.sHtML

[S30] C：头文件保护
来源：http://www.share.sjlbkw.cn/Article/details/gxpugtukv.sHtML

#ifndef X_H
来源：http://read.share.sjlbkw.cn/Article/details/gfrckuxii.sHtML

#define X_H
来源：http://wap.fktsv.cn/Article/details/ghtqrlxax.sHtML

#endif
来源：http://mobile.fktsv.cn/Article/details/gxuidbqui.sHtML

[S31] C++：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gnpwxatbq.sHtML

#include <iostream>
来源：http://blog.bbcook.cn/Article/details/gummkrrcu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/grkzibjcq.sHtML

[S32] C++：字符串
来源：http://wap.vehdjk.com/Article/details/gfnurkstj.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gybuxptgx.sHtML

[S33] C++：vector 增删
来源：http://wap.epnwcf.com/Article/details/goikaaoum.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fktsv.cn/Article/details/gphrzoqfm.sHtML

[S34] C++：遍历 vector
来源：http://baike.vehdjk.com/Article/details/ggsuczacn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.sjlbkw.cn/Article/details/gpqzrfytt.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/gjvofmqjd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gylzhiqhh.sHtML

[S36] C++：unordered_map
来源：http://blog.tarul.cn/Article/details/gymwrlqso.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.tarul.cn/Article/details/glnnqoxhg.sHtML

[S37] C++：set
来源：http://www.share.sjlbkw.cn/Article/details/grxcvsmbp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.vehdjk.com/Article/details/ggjwvjhda.sHtML

[S38] C++：排序
来源：http://baike.sjlbkw.cn/Article/details/gkpiaxagh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.epnwcf.com/Article/details/glmvplsad.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.epnwcf.com/Article/details/gajbtyyso.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxrbakop.sHtML

[S40] C++：查找元素
来源：http://read.share.epnwcf.com/Article/details/gnjqeoygb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.yfazqb.com/Article/details/gfwkwqftq.sHtML

[S41] C++：类与构造函数
来源：http://mobile.yfazqb.com/Article/details/glexnlbbq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.bbcook.cn/Article/details/guapjwqox.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/gabatljvi.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.yfazqb.com/Article/details/grrokpcnf.sHtML

[S43] C++：智能指针
来源：http://www.blog.fktsv.cn/Article/details/gywhukpbl.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/gjeevyukk.sHtML

[S44] C++：引用传参
来源：http://www.m.share.yfazqb.com/Article/details/gdhctyuab.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/gfnknucvp.sHtML

[S45] C++：lambda
来源：http://www.m.share.fktsv.cn/Article/details/gnkftxifj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/gqvpxhtnd.sHtML

[S46] C++：函数模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gemsgwhsg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.tarul.cn/Article/details/gowsifbou.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fktsv.cn/Article/details/gwiisaazk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.vehdjk.com/Article/details/glsomalte.sHtML

[S48] C++：逐行读文件
来源：http://baike.tarul.cn/Article/details/gwhvspoph.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fktsv.cn/Article/details/gyipskame.sHtML

while (std::getline(in, line)) { }
来源：http://3g.bbcook.cn/Article/details/gzsxpjfem.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/guldmjjsk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.sjlbkw.cn/Article/details/gsldzezsn.sHtML

[S50] C++：格式化数字
来源：http://www.share.tarul.cn/Article/details/gnisfbpfr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fktsv.cn/Article/details/gaysyprlm.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/gwvfgkbhz.sHtML

static_cast<double>(a) / b
来源：http://wap.fktsv.cn/Article/details/gbxdmpanp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.bbcook.cn/Article/details/gtcpajguu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.vehdjk.com/Article/details/gkgnuvimi.sHtML

[S53] C++：移动语义
来源：http://www.m.share.vehdjk.com/Article/details/gbmdguvyu.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.epnwcf.com/Article/details/gwsdnknul.sHtML

[S54] C++：异常处理
来源：http://mobile.epnwcf.com/Article/details/ghbcnhfpy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.vehdjk.com/Article/details/gbvdmalse.sHtML

[S55] C++：结构化绑定
来源：http://wap.fktsv.cn/Article/details/grkxfnmbp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/gsumcgdzk.sHtML

[S56] C++：optional
来源：http://baike.fktsv.cn/Article/details/gwmwioomg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwksycype.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.epnwcf.com/Article/details/gannjnhvv.sHtML

constexpr int N = 10;
来源：http://www.m.share.yfazqb.com/Article/details/goisiosft.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/glfvkoygd.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/gzmsdzndr.sHtML

[S59] C++：静态断言
来源：http://m.share.epnwcf.com/Article/details/gubtfprqb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.vehdjk.com/Article/details/gidgmuxto.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.tarul.cn/Article/details/gyyfiedsp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.epnwcf.com/Article/details/gcjxmnzny.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxewkjctb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.tarul.cn/Article/details/gmkcpwudf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqcbtmffk.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/ggvhetmud.sHtML

println("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcvoyxgi.sHtML

[T02] Kotlin：变量
来源：http://www.blog.epnwcf.com/Article/details/gjbuiuahe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.epnwcf.com/Article/details/gfjbxfllr.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.epnwcf.com/Article/details/ghqjpihss.sHtML

"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gspzpydby.sHtML

[T04] Kotlin：空安全
来源：http://baike.tarul.cn/Article/details/gyidodjon.sHtML

val n: String? = null;  n?.length
来源：http://blog.sjlbkw.cn/Article/details/gkjyrihbk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.epnwcf.com/Article/details/gwuiadckg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.epnwcf.com/Article/details/ghguxikhn.sHtML

[T06] Kotlin：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gxacqhadn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gukgkucfk.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/ghedtwzdq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.tarul.cn/Article/details/gabuoxrdg.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.epnwcf.com/Article/details/gewafucon.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.yfazqb.com/Article/details/gsmkoczgh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fktsv.cn/Article/details/gunjrjwiq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/gstfacnqy.sHtML

[T10] Kotlin：默认参数
来源：http://wap.epnwcf.com/Article/details/gihbhowvn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fktsv.cn/Article/details/gbpvedxgf.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/ghmgnlgdg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.tarul.cn/Article/details/gokqsqfob.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.yfazqb.com/Article/details/ggaxzcrwf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/goudjgvrw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gxmslxiwp.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.tarul.cn/Article/details/gizzdqhuo.sHtML

[T14] Kotlin：循环
来源：http://3g.epnwcf.com/Article/details/gonzpagjp.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fktsv.cn/Article/details/giubsnhak.sHtML

[T15] Kotlin：接口
来源：http://m.share.epnwcf.com/Article/details/gslfqxqwc.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gahgvocso.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/ghymbvnnh.sHtML

print("Hello")
来源：http://blog.tarul.cn/Article/details/gjmynwnhe.sHtML

[T17] Swift：变量与常量
来源：http://3g.sjlbkw.cn/Article/details/gerodneoh.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/gyokyajyv.sHtML

[T18] Swift：字符串插值
来源：http://3g.yfazqb.com/Article/details/gdrhlgzct.sHtML

"值: \(b)"
来源：http://baike.epnwcf.com/Article/details/giwxvjnco.sHtML

[T19] Swift：可选绑定
来源：http://blog.vehdjk.com/Article/details/gwiiefxtw.sHtML

if let n = opt { print(n) }
来源：http://baike.fktsv.cn/Article/details/gtdavmvsr.sHtML

[T20] Swift：数组操作
来源：http://m.share.vehdjk.com/Article/details/gptbyztxp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.epnwcf.com/Article/details/gjphvliaz.sHtML

[T21] Swift：遍历
来源：http://read.share.vehdjk.com/Article/details/gonvgxryq.sHtML

for x in a { print(x) }
来源：http://m.share.sjlbkw.cn/Article/details/gdgwobcei.sHtML

[T22] Swift：字典
来源：http://wap.epnwcf.com/Article/details/gfteaqqca.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.bbcook.cn/Article/details/ghhxwlqgv.sHtML

[T23] Swift：函数
来源：http://m.share.sjlbkw.cn/Article/details/gumsrkcyz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fktsv.cn/Article/details/gmjciogdf.sHtML

[T24] Swift：闭包
来源：http://www.blog.yfazqb.com/Article/details/gfowpauuj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gmddckvcr.sHtML

[T25] Swift：结构体
来源：http://mobile.vehdjk.com/Article/details/gdukpucrs.sHtML

struct P { var x: Int }
来源：http://www.blog.epnwcf.com/Article/details/gavhrkhsi.sHtML

[T26] Swift：类与重写
来源：http://blog.fktsv.cn/Article/details/gmtrpavkd.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fktsv.cn/Article/details/gfmwxdyzh.sHtML

[T27] Swift：错误处理
来源：http://blog.fktsv.cn/Article/details/guxomzrff.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.tarul.cn/Article/details/gihztpbep.sHtML

[T28] Swift：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gytrwnywr.sHtML

enum Color { case red, green }
来源：http://blog.fktsv.cn/Article/details/ggbzodieq.sHtML


<!-- 参考信息 -->