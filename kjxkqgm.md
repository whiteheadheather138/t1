代发 wailian999

esac
来源：http://www.m.share.bbcook.cn/Article/details/gnwlqaoxd.sHtML

[R12] for 遍历文件
来源：http://mobile.sjlbkw.cn/Article/details/ghkfmsmnb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.sjlbkw.cn/Article/details/gxgtvklwm.sHtML

[R13] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gdabysrer.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gaiebpvlj.sHtML

[R14] C 风格 for
来源：http://3g.tarul.cn/Article/details/ggvlkxmxl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/gmszndmth.sHtML

[R15] while 逐行读文件
来源：http://blog.fktsv.cn/Article/details/gppxfraht.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.tarul.cn/Article/details/goeyfwsct.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/gpyqgdazp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/ggbxhnmjt.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.vehdjk.com/Article/details/gknpvkvst.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.epnwcf.com/Article/details/gufgjxocv.sHtML

[R18] 遍历数组
来源：http://wap.tarul.cn/Article/details/gouqevjqy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.sjlbkw.cn/Article/details/gwhzkfnmp.sHtML

[R19] 数组长度
来源：http://wap.bbcook.cn/Article/details/gmqaskuzw.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.bbcook.cn/Article/details/goulsmjxj.sHtML

[R20] 关联数组（字典）
来源：http://mobile.sjlbkw.cn/Article/details/gpywoahid.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.sjlbkw.cn/Article/details/giovrmqqg.sHtML

[R21] 字符串长度
来源：http://read.share.epnwcf.com/Article/details/gkdxuusen.sHtML

echo "${#s}"
来源：http://www.m.share.vehdjk.com/Article/details/grngbiyix.sHtML

[R22] 截取子串
来源：http://blog.epnwcf.com/Article/details/gazciobit.sHtML

echo "${s:0:5}"
来源：http://blog.fktsv.cn/Article/details/gvbwhssih.sHtML

[R23] 字符串替换
来源：http://3g.epnwcf.com/Article/details/guhchqrku.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.vehdjk.com/Article/details/gphuezync.sHtML

[R24] 大小写转换
来源：http://baike.epnwcf.com/Article/details/ghjyzdwfk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.tarul.cn/Article/details/gbnrkillj.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.tarul.cn/Article/details/gvqkrxchp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.yfazqb.com/Article/details/gxyjrzonf.sHtML

[R26] 命令替换
来源：http://3g.fktsv.cn/Article/details/gnhovnqkj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.vehdjk.com/Article/details/gfryjlvuv.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gbijedmus.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fktsv.cn/Article/details/gmwxvzzuk.sHtML

[R28] 浮点运算
来源：http://3g.epnwcf.com/Article/details/gwjoeftdt.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/ggaxbhkki.sHtML

[R29] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gorhwdlsy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.epnwcf.com/Article/details/gptbydlem.sHtML

[R30] 函数返回状态码
来源：http://wap.tarul.cn/Article/details/giuxyijwg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.epnwcf.com/Article/details/gigsshfve.sHtML

[R31] 局部变量
来源：http://3g.bbcook.cn/Article/details/guiniclpu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.bbcook.cn/Article/details/gcjweasqf.sHtML

[R32] 参数个数校验
来源：http://blog.sjlbkw.cn/Article/details/gfledlreu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/gxogttqhn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.epnwcf.com/Article/details/gsedcrodj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.epnwcf.com/Article/details/gaoszpplq.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/ganhcbqze.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gjtdrlrej.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/gysewgbty.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.sjlbkw.cn/Article/details/ghsrokkll.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.sjlbkw.cn/Article/details/ghdbkzerp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.yfazqb.com/Article/details/glxgehykc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.sjlbkw.cn/Article/details/gcsahkppp.sHtML

files=$(ls -1)
来源：http://wap.yfazqb.com/Article/details/gbkovqwfc.sHtML

[R38] 管道串联
来源：http://baike.vehdjk.com/Article/details/gkntzsypz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.vehdjk.com/Article/details/gxrswuutn.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.tarul.cn/Article/details/godebqltz.sHtML

cmd > out.log 2>&1
来源：http://m.share.epnwcf.com/Article/details/gcnbuzzie.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/gintmtuwm.sHtML

echo "log" >> out.log
来源：http://blog.vehdjk.com/Article/details/gktrikzbt.sHtML

[R41] 丢弃输出
来源：http://mobile.fktsv.cn/Article/details/gdholrhrl.sHtML

cmd >/dev/null 2>&1
来源：http://3g.bbcook.cn/Article/details/gbblbjfbe.sHtML

[R42] 输入重定向
来源：http://www.m.share.yfazqb.com/Article/details/gkrkcslzz.sHtML

wc -l < a.txt
来源：http://3g.epnwcf.com/Article/details/gfluzdnay.sHtML

[R43] 按名字查找文件
来源：http://baike.vehdjk.com/Article/details/gdtroaytf.sHtML

find . -name "*.log" -type f
来源：http://wap.vehdjk.com/Article/details/gdljmhijv.sHtML

[R44] 按修改时间查找
来源：http://mobile.vehdjk.com/Article/details/grxglbgkr.sHtML

find . -mtime -7 -type f
来源：http://www.blog.sjlbkw.cn/Article/details/goelvkkjo.sHtML

[R45] 批量删除
来源：http://baike.fktsv.cn/Article/details/gucgdoand.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gsqqryxhz.sHtML

[R46] 递归替换文件内容
来源：http://3g.epnwcf.com/Article/details/gzgxffiuh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.sjlbkw.cn/Article/details/gjnbysqrf.sHtML

[R47] sed 单行替换
来源：http://www.share.bbcook.cn/Article/details/grbnblhvw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.epnwcf.com/Article/details/gwyrihgma.sHtML

[R48] awk 取指定列
来源：http://www.m.share.vehdjk.com/Article/details/gifkscjmp.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.epnwcf.com/Article/details/grczjzelr.sHtML

[R49] awk 带条件
来源：http://blog.bbcook.cn/Article/details/gdodihque.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.tarul.cn/Article/details/gtvnmbszz.sHtML

[R50] awk 求和
来源：http://wap.yfazqb.com/Article/details/gsyhalrvj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.epnwcf.com/Article/details/ghqipgvtz.sHtML

[R51] 排序去重取前几
来源：http://www.share.tarul.cn/Article/details/gwkevshxt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fktsv.cn/Article/details/gryglmsue.sHtML

[R52] 统计行数
来源：http://mobile.tarul.cn/Article/details/gpkoiuuwn.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/gnebjsjpi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.tarul.cn/Article/details/gnfzdyltt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.tarul.cn/Article/details/gjdpmrklm.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/gyowhsaoa.sHtML

diff a.txt b.txt
来源：http://mobile.tarul.cn/Article/details/gdyfbtajd.sHtML

[R55] 压缩与解压
来源：http://wap.sjlbkw.cn/Article/details/gllgzcymb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.tarul.cn/Article/details/grwfinspr.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/ggtgfiwjz.sHtML

scp file user@host:/path/
来源：http://www.m.share.sjlbkw.cn/Article/details/gssabongz.sHtML

[R57] 远程执行命令
来源：http://baike.epnwcf.com/Article/details/gerhezzij.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/gtofiicrb.sHtML

[R58] 下载文件
来源：http://baike.yfazqb.com/Article/details/gbarogstc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fktsv.cn/Article/details/gkzrurezs.sHtML

[R59] 发 POST JSON
来源：http://3g.bbcook.cn/Article/details/gilbbysox.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/gipfqkdyr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gtkqasykq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.bbcook.cn/Article/details/ghembnxsf.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/gjayxouvw.sHtML

df -h;  du -sh *
来源：http://read.share.bbcook.cn/Article/details/ggkgtzjcw.sHtML

[R62] 找最占空间的文件
来源：http://blog.sjlbkw.cn/Article/details/gsphkguwm.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/gwduishnj.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gcxkmxnew.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fktsv.cn/Article/details/gcxwvjkyd.sHtML

[R64] 结束进程
来源：http://www.m.share.tarul.cn/Article/details/gkaawfrwo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/ginmnrkdf.sHtML

[R65] 查看端口占用
来源：http://blog.bbcook.cn/Article/details/gyyzkwuns.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fktsv.cn/Article/details/gthjbfpfi.sHtML

[R66] 定时任务
来源：http://blog.yfazqb.com/Article/details/gwansjbnk.sHtML

crontab -e;  crontab -l
来源：http://m.share.bbcook.cn/Article/details/gxsyiwigw.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.epnwcf.com/Article/details/gqecccwxd.sHtML

openssl rand -hex 16
来源：http://m.share.tarul.cn/Article/details/geqljrrmc.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/gvnjcpgjn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fktsv.cn/Article/details/givkfndbx.sHtML

[R69] 生成随机密码
来源：http://3g.sjlbkw.cn/Article/details/gexltqnsl.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.epnwcf.com/Article/details/ggntvecip.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/gjhdxtmad.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.epnwcf.com/Article/details/gafrwrmcc.sHtML

[R71] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gtnagxssu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.vehdjk.com/Article/details/gtjofvkbx.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.sjlbkw.cn/Article/details/glzhwfdrd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/gkzafpqnw.sHtML

[R73] 分割大日志
来源：http://m.share.bbcook.cn/Article/details/gyegoknir.sHtML

split -l 1000 big.log part_
来源：http://blog.vehdjk.com/Article/details/gokgrojxf.sHtML

[R74] 批量重命名
来源：http://baike.bbcook.cn/Article/details/gzleqflkt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.epnwcf.com/Article/details/garvjtfha.sHtML

[R75] 导出环境变量
来源：http://www.share.yfazqb.com/Article/details/guhwjqjrd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.vehdjk.com/Article/details/gydluabbj.sHtML

[R76] 使用临时文件
来源：http://www.share.fktsv.cn/Article/details/grwhsuolo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gnetucflv.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fktsv.cn/Article/details/glafstlpf.sHtML

read -rp "请输入: " ans
来源：http://mobile.tarul.cn/Article/details/gevbtjosl.sHtML

[R78] 交互式菜单
来源：http://read.share.tarul.cn/Article/details/gqprjpiql.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.tarul.cn/Article/details/gfqhbozeh.sHtML

[R79] 解析命令行选项
来源：http://baike.tarul.cn/Article/details/grhdrletn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fktsv.cn/Article/details/gnkydmaqy.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.sjlbkw.cn/Article/details/gpnferltf.sHtML

time ./run.sh
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvakojfz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ghldizvvz.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gdicyyovx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdhgivqpt.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gcdahyvgk.sHtML

#include <stdio.h>
来源：http://blog.yfazqb.com/Article/details/ghctluibx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gubrgpooy.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.yfazqb.com/Article/details/gfrrnixgm.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fktsv.cn/Article/details/gxplybipp.sHtML

[S03] C：读入整数
来源：http://read.share.yfazqb.com/Article/details/glqloctqc.sHtML

int x; scanf("%d", &x);
来源：http://3g.sjlbkw.cn/Article/details/grhwgfsul.sHtML

[S04] C：字符串复制
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgkymqpr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.vehdjk.com/Article/details/gcqkylvxn.sHtML

[S05] C：字符串长度
来源：http://baike.yfazqb.com/Article/details/galxsutlx.sHtML

strlen(s)
来源：http://www.blog.fktsv.cn/Article/details/gkywpaahh.sHtML

[S06] C：字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gcwetgcit.sHtML

strcmp(a, b) == 0
来源：http://m.share.bbcook.cn/Article/details/gdwtmutvl.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.sjlbkw.cn/Article/details/grdispmux.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.yfazqb.com/Article/details/gswhvhtif.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fktsv.cn/Article/details/gsjgqvlmr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.tarul.cn/Article/details/gjgvpvfkr.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.yfazqb.com/Article/details/gvngsgkdi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.yfazqb.com/Article/details/gavcascpe.sHtML

[S10] C：指针与解引用
来源：http://mobile.bbcook.cn/Article/details/gqqpqhedv.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.vehdjk.com/Article/details/gmtnsnrrm.sHtML

[S11] C：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gzzomiqzu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.epnwcf.com/Article/details/gmgkhfekv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.tarul.cn/Article/details/gywahtcza.sHtML

fclose(f);
来源：http://3g.vehdjk.com/Article/details/glqszcrfu.sHtML

[S12] C：写文件
来源：http://baike.tarul.cn/Article/details/gsqlucqyn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/gfkopzsix.sHtML

[S13] C：宏定义
来源：http://m.share.vehdjk.com/Article/details/gaadezdce.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.bbcook.cn/Article/details/gqqkizywu.sHtML

[S14] C：枚举
来源：http://www.m.share.vehdjk.com/Article/details/gblqdkiud.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fktsv.cn/Article/details/gpqwjjxqr.sHtML

[S15] C：类型转换
来源：http://www.blog.bbcook.cn/Article/details/gwogbudbb.sHtML

(double) a / b
来源：http://read.share.yfazqb.com/Article/details/gqdfmrsxo.sHtML

[S16] C：位操作置位
来源：http://m.share.yfazqb.com/Article/details/gdqciaswf.sHtML

x |= (1 << 3);
来源：http://baike.bbcook.cn/Article/details/gdtgeupbm.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gsxyobenz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.tarul.cn/Article/details/gztsqcjsi.sHtML

[S18] C：命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gvsrxqjds.sHtML

int main(int argc, char **argv)
来源：http://3g.sjlbkw.cn/Article/details/gxldxzgdc.sHtML

[S19] C：快速排序
来源：http://3g.bbcook.cn/Article/details/gqgrcmsms.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/gekznnmfx.sHtML

[S20] C：二分查找
来源：http://m.share.yfazqb.com/Article/details/gtolruqvw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/gavslldwh.sHtML

[S21] C：字符类别判断
来源：http://wap.epnwcf.com/Article/details/gwguzlews.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/gapouvuiq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fktsv.cn/Article/details/gknfuxnuf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.sjlbkw.cn/Article/details/gtmtsfwzu.sHtML

[S23] C：随机数
来源：http://read.share.yfazqb.com/Article/details/gqookmeja.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.yfazqb.com/Article/details/gdkfnbaov.sHtML

[S24] C：获取本地时间
来源：http://read.share.tarul.cn/Article/details/gnayurmej.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/gsvrbctya.sHtML

[S25] C：内存拷贝
来源：http://blog.fktsv.cn/Article/details/geijtgphs.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/ggxjcsyuh.sHtML

[S26] C：内存清零
来源：http://m.share.epnwcf.com/Article/details/gpidnisec.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.bbcook.cn/Article/details/gcypksdhs.sHtML

[S27] C：定义常量
来源：http://m.share.tarul.cn/Article/details/gwiwlvscg.sHtML

const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/grbhfezpb.sHtML

[S28] C：静态变量
来源：http://www.m.share.bbcook.cn/Article/details/gmqikkyzy.sHtML

static int counter = 0;
来源：http://wap.bbcook.cn/Article/details/gjpiwkszx.sHtML

[S29] C：变参函数
来源：http://mobile.epnwcf.com/Article/details/gigqaukca.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fktsv.cn/Article/details/ghdhjxgka.sHtML

[S30] C：头文件保护
来源：http://mobile.vehdjk.com/Article/details/gyouajrvt.sHtML

#ifndef X_H
来源：http://baike.fktsv.cn/Article/details/gyztbsiez.sHtML

#define X_H
来源：http://blog.bbcook.cn/Article/details/gvmuqihwm.sHtML

#endif
来源：http://www.m.share.sjlbkw.cn/Article/details/gbafujshn.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/gurmgkwfo.sHtML

#include <iostream>
来源：http://wap.yfazqb.com/Article/details/gydfxopey.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.sjlbkw.cn/Article/details/gohwltkyu.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gkkihfqpc.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/gceewvqlr.sHtML

[S33] C++：vector 增删
来源：http://m.share.tarul.cn/Article/details/gkhgckrdc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.epnwcf.com/Article/details/goidunldw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.sjlbkw.cn/Article/details/gkodycguw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.tarul.cn/Article/details/gruguhudw.sHtML

[S35] C++：map
来源：http://baike.yfazqb.com/Article/details/gsdsqhzqw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gtviuohqs.sHtML

[S36] C++：unordered_map
来源：http://m.share.tarul.cn/Article/details/gsoiluzoa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/gwttjpcfu.sHtML

[S37] C++：set
来源：http://read.share.epnwcf.com/Article/details/gcluyrvra.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.epnwcf.com/Article/details/ggsbjitiw.sHtML

[S38] C++：排序
来源：http://wap.epnwcf.com/Article/details/gtzixggvb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gklutedwj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.vehdjk.com/Article/details/gjtleeuie.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.yfazqb.com/Article/details/gulpipkka.sHtML

[S40] C++：查找元素
来源：http://wap.sjlbkw.cn/Article/details/gjxykfatc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/gxaaqscxo.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fktsv.cn/Article/details/gnfhadygh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.epnwcf.com/Article/details/ggyunoixk.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.sjlbkw.cn/Article/details/gngyidchm.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.vehdjk.com/Article/details/gscjcsgao.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhpevobk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.sjlbkw.cn/Article/details/geixlxnus.sHtML

[S44] C++：引用传参
来源：http://www.m.share.epnwcf.com/Article/details/glaiogthk.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.bbcook.cn/Article/details/gvshqmwev.sHtML

[S45] C++：lambda
来源：http://www.share.vehdjk.com/Article/details/gcnjgqpgx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.sjlbkw.cn/Article/details/grdjyoytq.sHtML

[S46] C++：函数模板
来源：http://mobile.sjlbkw.cn/Article/details/gvcsvkkne.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.bbcook.cn/Article/details/gjazpddqe.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.epnwcf.com/Article/details/glgsufotl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.tarul.cn/Article/details/gpncesnya.sHtML

[S48] C++：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gjykfkoau.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.sjlbkw.cn/Article/details/ggledvqeo.sHtML

while (std::getline(in, line)) { }
来源：http://3g.epnwcf.com/Article/details/gqrcdujcq.sHtML

[S49] C++：写文件
来源：http://read.share.fktsv.cn/Article/details/gnugkrgaz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.yfazqb.com/Article/details/gdvylxyak.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/gdksegoun.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/gpuniqesr.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gzsqxynpo.sHtML

static_cast<double>(a) / b
来源：http://www.share.bbcook.cn/Article/details/gtxpwwdzp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fktsv.cn/Article/details/ggbmskcsu.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.tarul.cn/Article/details/glgmwvybe.sHtML

[S53] C++：移动语义
来源：http://www.m.share.yfazqb.com/Article/details/gbwbqwuhx.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.vehdjk.com/Article/details/geaibriaf.sHtML

[S54] C++：异常处理
来源：http://wap.sjlbkw.cn/Article/details/gslrpunrp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/glexzwury.sHtML

[S55] C++：结构化绑定
来源：http://read.share.epnwcf.com/Article/details/gpexjsyvz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.sjlbkw.cn/Article/details/gglouegiy.sHtML

[S56] C++：optional
来源：http://www.share.vehdjk.com/Article/details/gohdvdmfi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.sjlbkw.cn/Article/details/gplarjacg.sHtML

[S57] C++：编译期常量
来源：http://wap.tarul.cn/Article/details/gltgpqzsq.sHtML

constexpr int N = 10;
来源：http://read.share.tarul.cn/Article/details/gdhvxdtxb.sHtML

[S58] C++：命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzbicnrd.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.sjlbkw.cn/Article/details/gzqvzohjl.sHtML

[S59] C++：静态断言
来源：http://www.m.share.vehdjk.com/Article/details/gavhuflio.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.epnwcf.com/Article/details/gvbsiiuzu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.yfazqb.com/Article/details/gguyvawmh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.epnwcf.com/Article/details/gtrbjtogk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbqwuhbaf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.yfazqb.com/Article/details/geaqijnbb.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gkjfuobud.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gevhpgbxn.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gqwapltks.sHtML

[T02] Kotlin：变量
来源：http://m.share.yfazqb.com/Article/details/grslpbjsh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fktsv.cn/Article/details/gwratjeey.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.epnwcf.com/Article/details/gdhttcirf.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/gtxfeliwl.sHtML

[T04] Kotlin：空安全
来源：http://blog.sjlbkw.cn/Article/details/gbohxaeqn.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/gcqggjnsa.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.bbcook.cn/Article/details/glfjdzbcc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.yfazqb.com/Article/details/ghnquzhot.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.vehdjk.com/Article/details/gtvghilew.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.yfazqb.com/Article/details/gzsdhssjx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/geqexkdhj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gvcpbbcuf.sHtML

[T08] Kotlin：数据类
来源：http://wap.fktsv.cn/Article/details/glsmxdrgu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.epnwcf.com/Article/details/gpevxqpmj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.sjlbkw.cn/Article/details/gqbrnwpjs.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fktsv.cn/Article/details/gstfnmdvi.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.tarul.cn/Article/details/ghipphbix.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.epnwcf.com/Article/details/grryxtmno.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/gwfwjxiyy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.tarul.cn/Article/details/gjchdoodr.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.bbcook.cn/Article/details/gipnwmdwh.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.yfazqb.com/Article/details/guwdtbobn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.epnwcf.com/Article/details/gznulcrtv.sHtML

val m = mapOf("a" to 1)
来源：http://wap.sjlbkw.cn/Article/details/gijoyigxs.sHtML

[T14] Kotlin：循环
来源：http://mobile.epnwcf.com/Article/details/gztygtbfc.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gnqrtvfbl.sHtML


<!-- 参考信息 -->