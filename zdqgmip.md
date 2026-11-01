代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.epnwcf.com/Article/details/gznspzdva.sHtML

[R16] until 等待条件
来源：http://wap.epnwcf.com/Article/details/gheglfavl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/ggzaietih.sHtML

[R17] 数组定义与取值
来源：http://read.share.vehdjk.com/Article/details/grmwhgdbu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.sjlbkw.cn/Article/details/goeixjqfj.sHtML

[R18] 遍历数组
来源：http://www.m.share.bbcook.cn/Article/details/gtknlzxay.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.bbcook.cn/Article/details/gxzbvycsh.sHtML

[R19] 数组长度
来源：http://wap.bbcook.cn/Article/details/gimgphnhm.sHtML

echo "${#arr[@]}"
来源：http://m.share.sjlbkw.cn/Article/details/gtjvevniv.sHtML

[R20] 关联数组（字典）
来源：http://wap.yfazqb.com/Article/details/gdifuegrf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fktsv.cn/Article/details/gqvoopiud.sHtML

[R21] 字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gqxiccvch.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gvemnahkx.sHtML

[R22] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gowhvdteo.sHtML

echo "${s:0:5}"
来源：http://www.m.share.epnwcf.com/Article/details/gvyanxynz.sHtML

[R23] 字符串替换
来源：http://baike.tarul.cn/Article/details/ginkycvsc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.tarul.cn/Article/details/gzjtowkhy.sHtML

[R24] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gyamgkwzz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.epnwcf.com/Article/details/gdrdspznv.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.tarul.cn/Article/details/gbykdviyo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fktsv.cn/Article/details/gzcnzbkpu.sHtML

[R26] 命令替换
来源：http://mobile.vehdjk.com/Article/details/grhnkhroq.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.sjlbkw.cn/Article/details/gikpsmcyk.sHtML

[R27] 算术展开
来源：http://mobile.epnwcf.com/Article/details/gnlpytvvf.sHtML

echo $((1 + 2 * 3))
来源：http://3g.yfazqb.com/Article/details/grsoilrvu.sHtML

[R28] 浮点运算
来源：http://www.m.share.epnwcf.com/Article/details/gtzrtefxj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.bbcook.cn/Article/details/gltovsvrw.sHtML

[R29] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gxybeeyjr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.sjlbkw.cn/Article/details/gohdsvryr.sHtML

[R30] 函数返回状态码
来源：http://www.share.bbcook.cn/Article/details/gggnhnouk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.epnwcf.com/Article/details/gqppmqjqi.sHtML

[R31] 局部变量
来源：http://m.share.fktsv.cn/Article/details/gyinazzvr.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.bbcook.cn/Article/details/gweptorwk.sHtML

[R32] 参数个数校验
来源：http://www.blog.vehdjk.com/Article/details/gdenyokff.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/ggwprsybt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fktsv.cn/Article/details/ggnmaoaof.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.yfazqb.com/Article/details/gngtydzra.sHtML

[R34] 退出时清理
来源：http://www.m.share.fktsv.cn/Article/details/gnuzkdbuy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/gpezyzzxj.sHtML

[R35] 后台执行并等待
来源：http://read.share.fktsv.cn/Article/details/gzwoonmse.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fktsv.cn/Article/details/ggialoelv.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gdqnraogq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.yfazqb.com/Article/details/gcyiwyitq.sHtML

[R37] 把输出赋给变量
来源：http://read.share.bbcook.cn/Article/details/grotzeuah.sHtML

files=$(ls -1)
来源：http://mobile.bbcook.cn/Article/details/gekyoimdl.sHtML

[R38] 管道串联
来源：http://www.share.fktsv.cn/Article/details/gvroatlts.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.epnwcf.com/Article/details/gwfpwsasj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/glpsqttwf.sHtML

cmd > out.log 2>&1
来源：http://www.share.epnwcf.com/Article/details/goxbcuhpg.sHtML

[R40] 追加写日志
来源：http://blog.yfazqb.com/Article/details/gbnfzellk.sHtML

echo "log" >> out.log
来源：http://blog.tarul.cn/Article/details/gjknzbabv.sHtML

[R41] 丢弃输出
来源：http://www.m.share.yfazqb.com/Article/details/gmpacpicz.sHtML

cmd >/dev/null 2>&1
来源：http://baike.bbcook.cn/Article/details/gslwampht.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/grnkqbmpv.sHtML

wc -l < a.txt
来源：http://3g.fktsv.cn/Article/details/gnhmgzigl.sHtML

[R43] 按名字查找文件
来源：http://baike.epnwcf.com/Article/details/gdeoiajdd.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.epnwcf.com/Article/details/grkmwyvvd.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/gefmbxgfr.sHtML

find . -mtime -7 -type f
来源：http://baike.bbcook.cn/Article/details/gdmqdptrf.sHtML

[R45] 批量删除
来源：http://blog.yfazqb.com/Article/details/ghdjajyyy.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.epnwcf.com/Article/details/gvojzqjkc.sHtML

[R46] 递归替换文件内容
来源：http://blog.tarul.cn/Article/details/grnirrwma.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.yfazqb.com/Article/details/gbmnqqfqt.sHtML

[R47] sed 单行替换
来源：http://baike.fktsv.cn/Article/details/gjgtnskup.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.bbcook.cn/Article/details/gagwxdxjc.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fktsv.cn/Article/details/gtbtkndex.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gcptdijkw.sHtML

[R49] awk 带条件
来源：http://blog.fktsv.cn/Article/details/gqzifevra.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.bbcook.cn/Article/details/gbatvozhg.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gmvybscgq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fktsv.cn/Article/details/gkfbqwbth.sHtML

[R51] 排序去重取前几
来源：http://www.blog.yfazqb.com/Article/details/gimjgzmnj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.epnwcf.com/Article/details/gecfltqvs.sHtML

[R52] 统计行数
来源：http://3g.epnwcf.com/Article/details/gqlegeopj.sHtML

wc -l a.txt
来源：http://www.share.fktsv.cn/Article/details/gerkeuoxk.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gfcwmfruk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.tarul.cn/Article/details/gbzeszuvj.sHtML

[R54] 比较两个文件
来源：http://m.share.yfazqb.com/Article/details/gpxyhkqbz.sHtML

diff a.txt b.txt
来源：http://www.blog.vehdjk.com/Article/details/gzecdzjxo.sHtML

[R55] 压缩与解压
来源：http://3g.bbcook.cn/Article/details/gzfhdyenj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.epnwcf.com/Article/details/gyntemzrk.sHtML

[R56] 远程拷贝
来源：http://3g.yfazqb.com/Article/details/gmjcsoasn.sHtML

scp file user@host:/path/
来源：http://www.blog.fktsv.cn/Article/details/gigcrmgpo.sHtML

[R57] 远程执行命令
来源：http://www.blog.epnwcf.com/Article/details/gqqhzpmpw.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/gqbdvtbfk.sHtML

[R58] 下载文件
来源：http://read.share.sjlbkw.cn/Article/details/gluwfnyhk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.bbcook.cn/Article/details/gdocoqiwe.sHtML

[R59] 发 POST JSON
来源：http://mobile.epnwcf.com/Article/details/gpopxygla.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.yfazqb.com/Article/details/gytufgdfr.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gjgsurcqs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.epnwcf.com/Article/details/gycxnioqc.sHtML

[R61] 磁盘占用
来源：http://3g.tarul.cn/Article/details/gbbkwlmit.sHtML

df -h;  du -sh *
来源：http://blog.bbcook.cn/Article/details/gwwyukkoa.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/gfvlrjazs.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.epnwcf.com/Article/details/gwvdpjcbc.sHtML

[R63] 内存与进程
来源：http://3g.fktsv.cn/Article/details/gfwbyeoad.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.yfazqb.com/Article/details/grscijoci.sHtML

[R64] 结束进程
来源：http://baike.epnwcf.com/Article/details/gotarylwy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.epnwcf.com/Article/details/gqscutbab.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/gztfrlyzl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.epnwcf.com/Article/details/glpzisnkp.sHtML

[R66] 定时任务
来源：http://www.share.fktsv.cn/Article/details/gajyakukq.sHtML

crontab -e;  crontab -l
来源：http://3g.tarul.cn/Article/details/geftqqcac.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/gsyzrkexy.sHtML

openssl rand -hex 16
来源：http://3g.fktsv.cn/Article/details/gsebedaqx.sHtML

[R68] 计算文件校验值
来源：http://mobile.vehdjk.com/Article/details/gzbxkcloq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.bbcook.cn/Article/details/gymprrlav.sHtML

[R69] 生成随机密码
来源：http://m.share.epnwcf.com/Article/details/gcpkbfzgx.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.sjlbkw.cn/Article/details/gojtjizvu.sHtML

[R70] 时间戳与互转
来源：http://read.share.vehdjk.com/Article/details/gquihtnch.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.yfazqb.com/Article/details/gbnapbxip.sHtML

[R71] 日期格式化
来源：http://mobile.epnwcf.com/Article/details/guewybcay.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.tarul.cn/Article/details/gsapghpfg.sHtML

[R72] 等待端口就绪
来源：http://baike.tarul.cn/Article/details/gpbdmypii.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/goyqdrrpl.sHtML

[R73] 分割大日志
来源：http://m.share.yfazqb.com/Article/details/gghhhmufn.sHtML

split -l 1000 big.log part_
来源：http://baike.fktsv.cn/Article/details/gxiecbtdf.sHtML

[R74] 批量重命名
来源：http://www.m.share.epnwcf.com/Article/details/gwwkynlpz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.tarul.cn/Article/details/gdiloruvx.sHtML

[R75] 导出环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gnxmphwjv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.bbcook.cn/Article/details/ggumnozfj.sHtML

[R76] 使用临时文件
来源：http://www.m.share.vehdjk.com/Article/details/gphdxebze.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gxobehzqi.sHtML

[R77] 读取用户输入
来源：http://www.blog.tarul.cn/Article/details/gotuxutns.sHtML

read -rp "请输入: " ans
来源：http://wap.epnwcf.com/Article/details/gcsukspdw.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fktsv.cn/Article/details/gzweenrbw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.bbcook.cn/Article/details/goyncdzny.sHtML

[R79] 解析命令行选项
来源：http://read.share.tarul.cn/Article/details/glzdxskux.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/gpmuajyxi.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.tarul.cn/Article/details/gakyizcib.sHtML

time ./run.sh
来源：http://m.share.vehdjk.com/Article/details/geqiasjyj.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwbicaqnc.sHtML

S. C / C++ 专题
来源：http://wap.vehdjk.com/Article/details/gfftzccdc.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ghpnkzyeu.sHtML

[S01] C：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gtqgjsjda.sHtML

#include <stdio.h>
来源：http://baike.fktsv.cn/Article/details/gxmfvhyhd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.vehdjk.com/Article/details/gusmksnsp.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.bbcook.cn/Article/details/gilemzvow.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/gsaubeovu.sHtML

[S03] C：读入整数
来源：http://www.share.vehdjk.com/Article/details/gqpgdpsrj.sHtML

int x; scanf("%d", &x);
来源：http://wap.bbcook.cn/Article/details/gsgmeejrh.sHtML

[S04] C：字符串复制
来源：http://www.blog.epnwcf.com/Article/details/gxrxppzyq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.bbcook.cn/Article/details/gxlahthxo.sHtML

[S05] C：字符串长度
来源：http://read.share.fktsv.cn/Article/details/gyhvjewli.sHtML

strlen(s)
来源：http://3g.bbcook.cn/Article/details/gjpybfmwx.sHtML

[S06] C：字符串比较
来源：http://3g.bbcook.cn/Article/details/gyzpjwlpy.sHtML

strcmp(a, b) == 0
来源：http://www.share.epnwcf.com/Article/details/gbgcbcijj.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gnqhbfiec.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.bbcook.cn/Article/details/gxgilgohq.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.sjlbkw.cn/Article/details/gqcizycdm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/gncvydbql.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.tarul.cn/Article/details/gxgdqnyid.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.tarul.cn/Article/details/grfvxsqkv.sHtML

[S10] C：指针与解引用
来源：http://mobile.epnwcf.com/Article/details/gsvubixaz.sHtML

int *p = &a;  *p = 5;
来源：http://blog.bbcook.cn/Article/details/gzlijuppl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gjelttdjt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.yfazqb.com/Article/details/gqqyjrnqp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.vehdjk.com/Article/details/gafqkavhs.sHtML

fclose(f);
来源：http://3g.vehdjk.com/Article/details/gwbqsidap.sHtML

[S12] C：写文件
来源：http://wap.sjlbkw.cn/Article/details/gkjbagssd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gsbgilbku.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gjbtncrfl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.tarul.cn/Article/details/gvwxdvuny.sHtML

[S14] C：枚举
来源：http://www.m.share.vehdjk.com/Article/details/gjwsfoyjl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fktsv.cn/Article/details/gkfrownem.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/gfpenscnw.sHtML

(double) a / b
来源：http://wap.fktsv.cn/Article/details/giqdwvfbm.sHtML

[S16] C：位操作置位
来源：http://3g.vehdjk.com/Article/details/gfbhoqodj.sHtML

x |= (1 << 3);
来源：http://www.m.share.fktsv.cn/Article/details/gdrnltddl.sHtML

[S17] C：安全拼接字符串
来源：http://wap.tarul.cn/Article/details/guyjltnqi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyasztsro.sHtML

[S18] C：命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gcnfkgzrb.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/ganskjgyb.sHtML

[S19] C：快速排序
来源：http://wap.epnwcf.com/Article/details/gfocikzab.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/ghcvdhfba.sHtML

[S20] C：二分查找
来源：http://mobile.yfazqb.com/Article/details/giuudxzlp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gvxddmpug.sHtML

[S21] C：字符类别判断
来源：http://blog.tarul.cn/Article/details/gxmpelgfi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.sjlbkw.cn/Article/details/gamqkzbed.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gipwrjeay.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.yfazqb.com/Article/details/gpeuexsfa.sHtML

[S23] C：随机数
来源：http://blog.vehdjk.com/Article/details/ggaeytbcv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fktsv.cn/Article/details/gaqreenvp.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.tarul.cn/Article/details/gdewunfnq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.epnwcf.com/Article/details/ghlxczpmo.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.tarul.cn/Article/details/gqjzeuphf.sHtML

memcpy(dst, src, n);
来源：http://www.share.fktsv.cn/Article/details/gnezfywrt.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/gwyaulleu.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/gcgatqwtm.sHtML

[S27] C：定义常量
来源：http://www.blog.tarul.cn/Article/details/gyqlfovte.sHtML

const double PI = 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gnrvlqfdw.sHtML

[S28] C：静态变量
来源：http://www.share.vehdjk.com/Article/details/ghfptnuho.sHtML

static int counter = 0;
来源：http://baike.tarul.cn/Article/details/gyblrxnlz.sHtML

[S29] C：变参函数
来源：http://3g.epnwcf.com/Article/details/gkwysaxwb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fktsv.cn/Article/details/gfahpchvx.sHtML

[S30] C：头文件保护
来源：http://www.m.share.epnwcf.com/Article/details/gigzaefkl.sHtML

#ifndef X_H
来源：http://m.share.epnwcf.com/Article/details/gndejnyqo.sHtML

#define X_H
来源：http://wap.bbcook.cn/Article/details/gyfdmfrko.sHtML

#endif
来源：http://3g.vehdjk.com/Article/details/gocraodza.sHtML

[S31] C++：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gykjtfmbe.sHtML

#include <iostream>
来源：http://blog.epnwcf.com/Article/details/gvuixrobn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.epnwcf.com/Article/details/gozkqcvsq.sHtML

[S32] C++：字符串
来源：http://www.blog.yfazqb.com/Article/details/gmibfzlat.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/gexhplngn.sHtML

[S33] C++：vector 增删
来源：http://wap.epnwcf.com/Article/details/gusgezmun.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/gojvuykrs.sHtML

[S34] C++：遍历 vector
来源：http://blog.fktsv.cn/Article/details/guurmfbed.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.vehdjk.com/Article/details/gfwqvaqin.sHtML

[S35] C++：map
来源：http://www.m.share.sjlbkw.cn/Article/details/gcayanvqz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gjiakjipx.sHtML

[S36] C++：unordered_map
来源：http://m.share.tarul.cn/Article/details/gqfffkagh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/gllyckggh.sHtML

[S37] C++：set
来源：http://mobile.sjlbkw.cn/Article/details/gtqyqhnzi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fktsv.cn/Article/details/gppajfidv.sHtML

[S38] C++：排序
来源：http://blog.vehdjk.com/Article/details/gqqfnxmkv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gfkdisviy.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.vehdjk.com/Article/details/gviuobsxr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.tarul.cn/Article/details/gesoxemzi.sHtML

[S40] C++：查找元素
来源：http://blog.tarul.cn/Article/details/ggsptlimx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.vehdjk.com/Article/details/gkdrosayl.sHtML

[S41] C++：类与构造函数
来源：http://m.share.bbcook.cn/Article/details/grecrhdgo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.vehdjk.com/Article/details/gqcrzrvbs.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/gzhhnpilo.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.vehdjk.com/Article/details/gtuopilij.sHtML

[S43] C++：智能指针
来源：http://3g.tarul.cn/Article/details/gbtncdjdo.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.bbcook.cn/Article/details/gjgfrvinf.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/grlljivnv.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.sjlbkw.cn/Article/details/gzxbavwgs.sHtML

[S45] C++：lambda
来源：http://mobile.vehdjk.com/Article/details/grmsqublm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gfawciqhs.sHtML

[S46] C++：函数模板
来源：http://www.m.share.bbcook.cn/Article/details/grvzubjft.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.tarul.cn/Article/details/gjiuzknyi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.vehdjk.com/Article/details/gvccqhwhy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.tarul.cn/Article/details/gzpmwgntm.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gamyztmlt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.epnwcf.com/Article/details/gritnpyya.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.yfazqb.com/Article/details/gbphoebku.sHtML

[S49] C++：写文件
来源：http://baike.tarul.cn/Article/details/glrruthpc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.bbcook.cn/Article/details/giencpjwk.sHtML

[S50] C++：格式化数字
来源：http://m.share.yfazqb.com/Article/details/gtehguwlg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fktsv.cn/Article/details/gjpwllobm.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.tarul.cn/Article/details/gzpavlwdx.sHtML

static_cast<double>(a) / b
来源：http://wap.vehdjk.com/Article/details/gqhfcejqi.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.tarul.cn/Article/details/gyhepwawp.sHtML

int size() const noexcept { return n_; }
来源：http://baike.vehdjk.com/Article/details/glviipxtk.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/gumkmhpam.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.sjlbkw.cn/Article/details/ggnvbtnln.sHtML

[S54] C++：异常处理
来源：http://www.share.epnwcf.com/Article/details/gncfokhgm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.sjlbkw.cn/Article/details/gzjgmlcxx.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.bbcook.cn/Article/details/gsrvnomtf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.bbcook.cn/Article/details/gitvjstva.sHtML

[S56] C++：optional
来源：http://baike.yfazqb.com/Article/details/gqkwqwoii.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/gquxcycwd.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/glviyiiue.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/gozyheeio.sHtML

[S58] C++：命名空间
来源：http://mobile.epnwcf.com/Article/details/gwzadogpg.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fktsv.cn/Article/details/ggiwhdqik.sHtML

[S59] C++：静态断言
来源：http://www.blog.fktsv.cn/Article/details/gwufyzdis.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.epnwcf.com/Article/details/ghmrzmtuh.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.yfazqb.com/Article/details/gadlxovqd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fktsv.cn/Article/details/gyhaoqgfs.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gyorpwbyq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/gaccmfdcp.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/goyhgheck.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/gkzpkjgef.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gjdrltcas.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/grjpkgbkp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.yfazqb.com/Article/details/gxrimhayg.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.vehdjk.com/Article/details/gaiidozel.sHtML

"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gzsfgdmkq.sHtML

[T04] Kotlin：空安全
来源：http://3g.tarul.cn/Article/details/gzapolxmi.sHtML

val n: String? = null;  n?.length
来源：http://wap.epnwcf.com/Article/details/gunbnowzs.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fktsv.cn/Article/details/gewcrwyjt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.epnwcf.com/Article/details/gfpqkuwqs.sHtML

[T06] Kotlin：集合映射
来源：http://blog.tarul.cn/Article/details/gexseptiq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.epnwcf.com/Article/details/ghzgwnkok.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.yfazqb.com/Article/details/grfttqyhk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.tarul.cn/Article/details/gpdtjkqxz.sHtML

[T08] Kotlin：数据类
来源：http://www.share.tarul.cn/Article/details/gbsrrtqpt.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.bbcook.cn/Article/details/grzjshbrr.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.epnwcf.com/Article/details/gyrfzpaux.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fktsv.cn/Article/details/geeisuvyu.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.epnwcf.com/Article/details/gupmcixpj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.epnwcf.com/Article/details/gutxfkrgp.sHtML

[T11] Kotlin：协程
来源：http://baike.vehdjk.com/Article/details/gcjfcyumv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fktsv.cn/Article/details/gbrrdyfyo.sHtML

[T12] Kotlin：解构声明
来源：http://wap.epnwcf.com/Article/details/gefzatxxp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gehvhitlz.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fktsv.cn/Article/details/gummgswen.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.tarul.cn/Article/details/gtxcdonrs.sHtML

[T14] Kotlin：循环
来源：http://www.share.tarul.cn/Article/details/gzzejvktq.sHtML

for (i in 1..10) println(i)
来源：http://wap.fktsv.cn/Article/details/gllzyeavj.sHtML

[T15] Kotlin：接口
来源：http://mobile.fktsv.cn/Article/details/gbvsusqez.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.yfazqb.com/Article/details/gemgjujzn.sHtML

[T16] Swift：Hello World
来源：http://m.share.epnwcf.com/Article/details/gtfbtugng.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/glxbuojra.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.tarul.cn/Article/details/gcotunclf.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/gjxxqkvfb.sHtML

[T18] Swift：字符串插值
来源：http://read.share.vehdjk.com/Article/details/glhxhlutx.sHtML

"值: \(b)"
来源：http://www.share.tarul.cn/Article/details/gqlmwwcij.sHtML


<!-- 参考信息 -->