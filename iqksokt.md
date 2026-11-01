代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://3g.tarul.cn/Article/details/glwprcgfn.sHtML

[R18] 遍历数组
来源：http://3g.sjlbkw.cn/Article/details/gslmoeaxx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.tarul.cn/Article/details/gnwectneo.sHtML

[R19] 数组长度
来源：http://3g.yfazqb.com/Article/details/gvkliaeeq.sHtML

echo "${#arr[@]}"
来源：http://wap.bbcook.cn/Article/details/gsngwtcpv.sHtML

[R20] 关联数组（字典）
来源：http://blog.tarul.cn/Article/details/gjfzfeqdc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.yfazqb.com/Article/details/gesoktggk.sHtML

[R21] 字符串长度
来源：http://read.share.tarul.cn/Article/details/gjjsdooei.sHtML

echo "${#s}"
来源：http://www.blog.bbcook.cn/Article/details/gcfblhusa.sHtML

[R22] 截取子串
来源：http://m.share.bbcook.cn/Article/details/gnqkrhmly.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/gslfwjcan.sHtML

[R23] 字符串替换
来源：http://blog.bbcook.cn/Article/details/gqeqeemkf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.sjlbkw.cn/Article/details/gjavzufwx.sHtML

[R24] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gkzfxmgov.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.sjlbkw.cn/Article/details/giecvvbgb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gjkizsqjz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/grdoskrbr.sHtML

[R26] 命令替换
来源：http://baike.epnwcf.com/Article/details/gopiwelej.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.epnwcf.com/Article/details/gdjrsnkjn.sHtML

[R27] 算术展开
来源：http://www.m.share.vehdjk.com/Article/details/gdgnfyzcy.sHtML

echo $((1 + 2 * 3))
来源：http://wap.bbcook.cn/Article/details/gxsjducnz.sHtML

[R28] 浮点运算
来源：http://3g.vehdjk.com/Article/details/gunbipumi.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/gnjuopkua.sHtML

[R29] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwjpqylp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.bbcook.cn/Article/details/gtysftzud.sHtML

[R30] 函数返回状态码
来源：http://m.share.vehdjk.com/Article/details/gazxpvgdm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fktsv.cn/Article/details/gkhutyrxk.sHtML

[R31] 局部变量
来源：http://read.share.fktsv.cn/Article/details/gklfmoshf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/gosstzsgy.sHtML

[R32] 参数个数校验
来源：http://baike.fktsv.cn/Article/details/gijxnlncj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gqekyoncy.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.vehdjk.com/Article/details/gmanqkpfz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.bbcook.cn/Article/details/ghansluhy.sHtML

[R34] 退出时清理
来源：http://read.share.fktsv.cn/Article/details/goipoyoau.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gnkkrgecw.sHtML

[R35] 后台执行并等待
来源：http://www.blog.tarul.cn/Article/details/gmfkxytll.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.tarul.cn/Article/details/gnqwydhcc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.epnwcf.com/Article/details/gwuegwzri.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.epnwcf.com/Article/details/gifbwglcp.sHtML

[R37] 把输出赋给变量
来源：http://blog.sjlbkw.cn/Article/details/geimrshne.sHtML

files=$(ls -1)
来源：http://read.share.sjlbkw.cn/Article/details/geuqdclcw.sHtML

[R38] 管道串联
来源：http://blog.sjlbkw.cn/Article/details/gwsgewzjb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.tarul.cn/Article/details/ggspcrgdk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.epnwcf.com/Article/details/gqzboakqz.sHtML

cmd > out.log 2>&1
来源：http://www.share.vehdjk.com/Article/details/gxrimtqoo.sHtML

[R40] 追加写日志
来源：http://read.share.tarul.cn/Article/details/gynwkowkt.sHtML

echo "log" >> out.log
来源：http://www.share.vehdjk.com/Article/details/gazezplak.sHtML

[R41] 丢弃输出
来源：http://mobile.epnwcf.com/Article/details/gbscacsua.sHtML

cmd >/dev/null 2>&1
来源：http://wap.sjlbkw.cn/Article/details/ghoavnzhu.sHtML

[R42] 输入重定向
来源：http://www.m.share.tarul.cn/Article/details/gfxodfvxc.sHtML

wc -l < a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gpzeujmfl.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gppreaujr.sHtML

find . -name "*.log" -type f
来源：http://3g.yfazqb.com/Article/details/gmfhgepcp.sHtML

[R44] 按修改时间查找
来源：http://www.blog.yfazqb.com/Article/details/gdrfqbouk.sHtML

find . -mtime -7 -type f
来源：http://m.share.vehdjk.com/Article/details/gkgwvopsh.sHtML

[R45] 批量删除
来源：http://3g.vehdjk.com/Article/details/gpmuibkwk.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.bbcook.cn/Article/details/gfxexpsgu.sHtML

[R46] 递归替换文件内容
来源：http://baike.fktsv.cn/Article/details/ggmeafins.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fktsv.cn/Article/details/gfbybkkep.sHtML

[R47] sed 单行替换
来源：http://www.m.share.bbcook.cn/Article/details/gdiqwvvix.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.yfazqb.com/Article/details/gxapxdtfj.sHtML

[R48] awk 取指定列
来源：http://www.share.epnwcf.com/Article/details/gibrejwqd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gnjyhwjym.sHtML

[R49] awk 带条件
来源：http://wap.sjlbkw.cn/Article/details/guvgueqxv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fktsv.cn/Article/details/geqddzorh.sHtML

[R50] awk 求和
来源：http://wap.vehdjk.com/Article/details/gkqalusgg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gxojjdigx.sHtML

[R51] 排序去重取前几
来源：http://mobile.bbcook.cn/Article/details/gjohzjeql.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.bbcook.cn/Article/details/glzciuyxb.sHtML

[R52] 统计行数
来源：http://www.share.tarul.cn/Article/details/gczttvjfe.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/gfvfkimfx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfulrfdy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.yfazqb.com/Article/details/gmunbofdy.sHtML

[R54] 比较两个文件
来源：http://3g.fktsv.cn/Article/details/grqrxgegh.sHtML

diff a.txt b.txt
来源：http://www.m.share.fktsv.cn/Article/details/grstzynpc.sHtML

[R55] 压缩与解压
来源：http://baike.fktsv.cn/Article/details/gvuzgtoek.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.yfazqb.com/Article/details/gkstoejpb.sHtML

[R56] 远程拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gzhmskufc.sHtML

scp file user@host:/path/
来源：http://mobile.sjlbkw.cn/Article/details/gyznkxbeu.sHtML

[R57] 远程执行命令
来源：http://www.m.share.yfazqb.com/Article/details/gehuzdiai.sHtML

ssh user@host 'uptime'
来源：http://read.share.epnwcf.com/Article/details/gwpkhkcvi.sHtML

[R58] 下载文件
来源：http://blog.tarul.cn/Article/details/gerieqxlz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fktsv.cn/Article/details/gorjilltx.sHtML

[R59] 发 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gbbgquuty.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.yfazqb.com/Article/details/gzngtjkbk.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gwarmdexy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fktsv.cn/Article/details/gofegxzuf.sHtML

[R61] 磁盘占用
来源：http://blog.vehdjk.com/Article/details/gtytaeqmg.sHtML

df -h;  du -sh *
来源：http://m.share.tarul.cn/Article/details/gxpkpxjxo.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/gqpcpuili.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fktsv.cn/Article/details/gkykfklzy.sHtML

[R63] 内存与进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdtzhppo.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.bbcook.cn/Article/details/giekvmpfi.sHtML

[R64] 结束进程
来源：http://m.share.fktsv.cn/Article/details/gbmwsnlcv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.tarul.cn/Article/details/gvdausyrc.sHtML

[R65] 查看端口占用
来源：http://wap.tarul.cn/Article/details/gkyfjwtpi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fktsv.cn/Article/details/ghlbqqgxa.sHtML

[R66] 定时任务
来源：http://www.blog.epnwcf.com/Article/details/gcrrqyhtm.sHtML

crontab -e;  crontab -l
来源：http://read.share.fktsv.cn/Article/details/geezdbyeq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fktsv.cn/Article/details/gybcgjvto.sHtML

openssl rand -hex 16
来源：http://read.share.sjlbkw.cn/Article/details/gkrdilegj.sHtML

[R68] 计算文件校验值
来源：http://read.share.tarul.cn/Article/details/gujjkdoat.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.sjlbkw.cn/Article/details/gtgludllq.sHtML

[R69] 生成随机密码
来源：http://baike.yfazqb.com/Article/details/ghthfwrmj.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.vehdjk.com/Article/details/gvrikfrrj.sHtML

[R70] 时间戳与互转
来源：http://baike.epnwcf.com/Article/details/gwgmkvnkw.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.yfazqb.com/Article/details/gjflmofvq.sHtML

[R71] 日期格式化
来源：http://baike.vehdjk.com/Article/details/gbauovmcr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.tarul.cn/Article/details/gzwrkzfvj.sHtML

[R72] 等待端口就绪
来源：http://wap.fktsv.cn/Article/details/gwuztcgfw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/gyfjspsee.sHtML

[R73] 分割大日志
来源：http://www.share.fktsv.cn/Article/details/gewmiwkyc.sHtML

split -l 1000 big.log part_
来源：http://blog.vehdjk.com/Article/details/grjqjxldp.sHtML

[R74] 批量重命名
来源：http://read.share.yfazqb.com/Article/details/gxxdeumwg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.tarul.cn/Article/details/gayjxhgsu.sHtML

[R75] 导出环境变量
来源：http://3g.fktsv.cn/Article/details/gbwyqukaw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fktsv.cn/Article/details/gnopqbikp.sHtML

[R76] 使用临时文件
来源：http://3g.sjlbkw.cn/Article/details/guqkyhqbt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gfmqapjhm.sHtML

[R77] 读取用户输入
来源：http://wap.tarul.cn/Article/details/gpwxtfsql.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/gvhcvwzzg.sHtML

[R78] 交互式菜单
来源：http://mobile.tarul.cn/Article/details/giarxphqi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.epnwcf.com/Article/details/gtxvlrxau.sHtML

[R79] 解析命令行选项
来源：http://m.share.fktsv.cn/Article/details/gmjdhkefw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.bbcook.cn/Article/details/gsugwkpag.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.epnwcf.com/Article/details/gmuhdvzuz.sHtML

time ./run.sh
来源：http://www.share.sjlbkw.cn/Article/details/gshsamyju.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmmlgdbcy.sHtML

S. C / C++ 专题
来源：http://read.share.fktsv.cn/Article/details/gnjtenmva.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmiemodya.sHtML

[S01] C：Hello World
来源：http://www.blog.tarul.cn/Article/details/gpwinmetr.sHtML

#include <stdio.h>
来源：http://m.share.epnwcf.com/Article/details/gpoawcofc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fktsv.cn/Article/details/gbqckhpvl.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.tarul.cn/Article/details/govzovnic.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gajhfwbvo.sHtML

[S03] C：读入整数
来源：http://mobile.yfazqb.com/Article/details/gyjuhytop.sHtML

int x; scanf("%d", &x);
来源：http://read.share.yfazqb.com/Article/details/gxmhqpnah.sHtML

[S04] C：字符串复制
来源：http://wap.tarul.cn/Article/details/gloxshbvx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gkyyxlhio.sHtML

[S05] C：字符串长度
来源：http://blog.epnwcf.com/Article/details/gyplfjszu.sHtML

strlen(s)
来源：http://www.m.share.bbcook.cn/Article/details/gkhsqawmg.sHtML

[S06] C：字符串比较
来源：http://www.share.tarul.cn/Article/details/gscztfybf.sHtML

strcmp(a, b) == 0
来源：http://m.share.yfazqb.com/Article/details/gqdawcuvy.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/givxgzowf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/goezydddp.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.bbcook.cn/Article/details/ghvcsfoei.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/guxdwfuzb.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fktsv.cn/Article/details/gseyolxuy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.sjlbkw.cn/Article/details/gjrvuutwl.sHtML

[S10] C：指针与解引用
来源：http://3g.sjlbkw.cn/Article/details/griusvtwg.sHtML

int *p = &a;  *p = 5;
来源：http://baike.sjlbkw.cn/Article/details/gkwyfvvtt.sHtML

[S11] C：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/geirhluiq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.vehdjk.com/Article/details/gcqwyksil.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gdtwupvyn.sHtML

fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gxtrwveym.sHtML

[S12] C：写文件
来源：http://read.share.vehdjk.com/Article/details/ggtbmluuf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gxskwgylm.sHtML

[S13] C：宏定义
来源：http://baike.yfazqb.com/Article/details/gqlootgxp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.epnwcf.com/Article/details/gqflmrigu.sHtML

[S14] C：枚举
来源：http://www.m.share.tarul.cn/Article/details/gyzmxgykg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.yfazqb.com/Article/details/gcvhsldtw.sHtML

[S15] C：类型转换
来源：http://m.share.fktsv.cn/Article/details/gtpvnhkly.sHtML

(double) a / b
来源：http://baike.epnwcf.com/Article/details/gfwyucgwm.sHtML

[S16] C：位操作置位
来源：http://www.share.vehdjk.com/Article/details/gitzampit.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/glfytupll.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.tarul.cn/Article/details/gqzhaucyg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.yfazqb.com/Article/details/gpfsxqxcz.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/gbtmdsdco.sHtML

int main(int argc, char **argv)
来源：http://baike.fktsv.cn/Article/details/gmbfsahrj.sHtML

[S19] C：快速排序
来源：http://baike.tarul.cn/Article/details/gvprcqpkx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/ghkwveysg.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/gtcklniyr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gjklgojef.sHtML

[S21] C：字符类别判断
来源：http://wap.vehdjk.com/Article/details/gbdodcflj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.tarul.cn/Article/details/gaoddiqtq.sHtML

[S22] C：字符串转数字
来源：http://wap.yfazqb.com/Article/details/gaiscjcch.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.yfazqb.com/Article/details/gkafsrhjn.sHtML

[S23] C：随机数
来源：http://m.share.tarul.cn/Article/details/gtbhvngko.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/gwrbkrdht.sHtML

[S24] C：获取本地时间
来源：http://3g.tarul.cn/Article/details/grzslnnad.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.vehdjk.com/Article/details/gpuzlaogs.sHtML

[S25] C：内存拷贝
来源：http://blog.bbcook.cn/Article/details/gdkoucxje.sHtML

memcpy(dst, src, n);
来源：http://read.share.bbcook.cn/Article/details/guwnxnnbw.sHtML

[S26] C：内存清零
来源：http://wap.fktsv.cn/Article/details/ggupkaxib.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.tarul.cn/Article/details/gfffjxxuv.sHtML

[S27] C：定义常量
来源：http://3g.yfazqb.com/Article/details/gqoshmalu.sHtML

const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/glcvwqcnx.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/gemjxdrqq.sHtML

static int counter = 0;
来源：http://wap.vehdjk.com/Article/details/gshbylsfi.sHtML

[S29] C：变参函数
来源：http://m.share.tarul.cn/Article/details/gmoorqogl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/gefdzncyg.sHtML

[S30] C：头文件保护
来源：http://www.blog.fktsv.cn/Article/details/gjavepxnx.sHtML

#ifndef X_H
来源：http://www.share.epnwcf.com/Article/details/gwlvywlnz.sHtML

#define X_H
来源：http://3g.tarul.cn/Article/details/gumoiegyk.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/gjswsiepk.sHtML

[S31] C++：Hello World
来源：http://read.share.bbcook.cn/Article/details/ggfjexkbu.sHtML

#include <iostream>
来源：http://3g.sjlbkw.cn/Article/details/gpetjfiam.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/gjrdbxwzh.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkhuffbr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.bbcook.cn/Article/details/gaaqfayer.sHtML

[S33] C++：vector 增删
来源：http://wap.vehdjk.com/Article/details/gdvlrbgmd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.vehdjk.com/Article/details/gvohexhic.sHtML

[S34] C++：遍历 vector
来源：http://m.share.yfazqb.com/Article/details/gwaaunuyc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gmolpvvga.sHtML

[S35] C++：map
来源：http://wap.sjlbkw.cn/Article/details/gzhmmszok.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gplosnvna.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/gsfmmrhyc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/grefdnegs.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/gxltpetyc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.vehdjk.com/Article/details/grwmwnphh.sHtML

[S38] C++：排序
来源：http://www.share.vehdjk.com/Article/details/gusdpzsnm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/gsjjkaumy.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.bbcook.cn/Article/details/gabuuelit.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fktsv.cn/Article/details/gidvjvtzi.sHtML

[S40] C++：查找元素
来源：http://www.share.vehdjk.com/Article/details/gvclanthd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/gzgmzschn.sHtML

[S41] C++：类与构造函数
来源：http://read.share.vehdjk.com/Article/details/gjdoppkmx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.epnwcf.com/Article/details/gfxmxzsfj.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/gkvsvfpps.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gutddndah.sHtML

[S43] C++：智能指针
来源：http://www.blog.vehdjk.com/Article/details/gqwazeitp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.tarul.cn/Article/details/grvrvzocn.sHtML

[S44] C++：引用传参
来源：http://wap.yfazqb.com/Article/details/gpetydzzb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/gdstpdgop.sHtML

[S45] C++：lambda
来源：http://mobile.vehdjk.com/Article/details/gdwtmfbfm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.epnwcf.com/Article/details/guxycrkup.sHtML

[S46] C++：函数模板
来源：http://baike.fktsv.cn/Article/details/guzrngeil.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.sjlbkw.cn/Article/details/gnxbsufvh.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.vehdjk.com/Article/details/goyvstbjc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.epnwcf.com/Article/details/gslsezebn.sHtML

[S48] C++：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gxrqotbgf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fktsv.cn/Article/details/gvrcgxlzt.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/gmonldjtn.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/ggqamnqze.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fktsv.cn/Article/details/gxxtrntdd.sHtML

[S50] C++：格式化数字
来源：http://www.share.yfazqb.com/Article/details/gucbyyyua.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gikdxrbbz.sHtML

[S51] C++：显式类型转换
来源：http://3g.fktsv.cn/Article/details/gzezvmemb.sHtML

static_cast<double>(a) / b
来源：http://read.share.vehdjk.com/Article/details/godnqqrin.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.sjlbkw.cn/Article/details/gxuxmuzjc.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/gelexpnpn.sHtML

[S53] C++：移动语义
来源：http://www.blog.sjlbkw.cn/Article/details/gfjutjfio.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fktsv.cn/Article/details/gfedfhgvb.sHtML

[S54] C++：异常处理
来源：http://3g.sjlbkw.cn/Article/details/gdkqgvvol.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.tarul.cn/Article/details/gntjatkgt.sHtML

[S55] C++：结构化绑定
来源：http://www.share.bbcook.cn/Article/details/gegpymzmv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.vehdjk.com/Article/details/gdwkevjgw.sHtML

[S56] C++：optional
来源：http://m.share.sjlbkw.cn/Article/details/gdflhobnp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.vehdjk.com/Article/details/grvjqgxtf.sHtML

[S57] C++：编译期常量
来源：http://blog.sjlbkw.cn/Article/details/gdjgwjvnb.sHtML

constexpr int N = 10;
来源：http://baike.fktsv.cn/Article/details/ghvmloiiy.sHtML

[S58] C++：命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjifvjnb.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.bbcook.cn/Article/details/gebllvcfa.sHtML

[S59] C++：静态断言
来源：http://read.share.tarul.cn/Article/details/gdywuddmj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.sjlbkw.cn/Article/details/gbxcozsbl.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.sjlbkw.cn/Article/details/gnvhgxggc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fktsv.cn/Article/details/geunhfiyb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glgcwqjut.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.epnwcf.com/Article/details/glizqzhwh.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmidmzxee.sHtML

[T01] Kotlin：Hello World
来源：http://baike.bbcook.cn/Article/details/gcccvgxfc.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/ghnatanyk.sHtML

[T02] Kotlin：变量
来源：http://www.blog.bbcook.cn/Article/details/gsuvljhgd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.epnwcf.com/Article/details/gvitztecq.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.sjlbkw.cn/Article/details/gvtkgonip.sHtML

"值: $b"
来源：http://www.share.yfazqb.com/Article/details/glebqqabk.sHtML

[T04] Kotlin：空安全
来源：http://mobile.epnwcf.com/Article/details/gwucmwbzy.sHtML

val n: String? = null;  n?.length
来源：http://blog.fktsv.cn/Article/details/gmsdwfpca.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.epnwcf.com/Article/details/gqwjwngti.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fktsv.cn/Article/details/gcwcasidy.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gyndzdweq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.epnwcf.com/Article/details/gafcfkwxh.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.epnwcf.com/Article/details/gebwxhxjo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.bbcook.cn/Article/details/gtmytpkio.sHtML

[T08] Kotlin：数据类
来源：http://3g.fktsv.cn/Article/details/gxweccojb.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/gageigswn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.vehdjk.com/Article/details/gktzzvgrh.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.vehdjk.com/Article/details/gtxabpgvf.sHtML

[T10] Kotlin：默认参数
来源：http://blog.sjlbkw.cn/Article/details/gkvlzopfd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.vehdjk.com/Article/details/gmhyfzlxe.sHtML

[T11] Kotlin：协程
来源：http://m.share.sjlbkw.cn/Article/details/gduqskioc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.yfazqb.com/Article/details/gvdtrlcjb.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.yfazqb.com/Article/details/gzpvhdbre.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gnqkfiqfq.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fktsv.cn/Article/details/gczuibzjc.sHtML

val m = mapOf("a" to 1)
来源：http://baike.sjlbkw.cn/Article/details/gnhywwrul.sHtML

[T14] Kotlin：循环
来源：http://read.share.sjlbkw.cn/Article/details/gobqnqtqr.sHtML

for (i in 1..10) println(i)
来源：http://3g.tarul.cn/Article/details/gfdbythxg.sHtML

[T15] Kotlin：接口
来源：http://3g.bbcook.cn/Article/details/gskmdopvf.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/gpvqhjvjg.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gaavdzvgh.sHtML

print("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/grvsbweuf.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.tarul.cn/Article/details/gmyqblcny.sHtML

var a = 1;  let b = 2
来源：http://wap.bbcook.cn/Article/details/gdnkbabbj.sHtML

[T18] Swift：字符串插值
来源：http://3g.epnwcf.com/Article/details/gypshmdvi.sHtML

"值: \(b)"
来源：http://blog.yfazqb.com/Article/details/gnbzfdwii.sHtML

[T19] Swift：可选绑定
来源：http://wap.vehdjk.com/Article/details/gkdcwysmt.sHtML

if let n = opt { print(n) }
来源：http://m.share.yfazqb.com/Article/details/gfgwzavzv.sHtML

[T20] Swift：数组操作
来源：http://www.blog.bbcook.cn/Article/details/guukkzrmm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.epnwcf.com/Article/details/gnoiecmjk.sHtML


<!-- 参考信息 -->