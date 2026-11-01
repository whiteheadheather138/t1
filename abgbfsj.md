代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.yfazqb.com/Article/details/gcslrmxwi.sHtML

[R10] 正则匹配
来源：http://www.blog.vehdjk.com/Article/details/gdnoeejeq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/gsvamcwlr.sHtML

[R11] case 多分支
来源：http://www.m.share.fktsv.cn/Article/details/gsntvnalx.sHtML

case "$1" in
来源：http://wap.yfazqb.com/Article/details/gmlivedjt.sHtML

start) echo "启动" ;;
来源：http://baike.sjlbkw.cn/Article/details/gzonnsxwv.sHtML

stop)  echo "停止" ;;
来源：http://blog.tarul.cn/Article/details/gzjxtrkxi.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.yfazqb.com/Article/details/gatwxzhkm.sHtML

esac
来源：http://read.share.epnwcf.com/Article/details/gesggweuc.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/gsiihojve.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.bbcook.cn/Article/details/gmbezegye.sHtML

[R13] for 计数循环
来源：http://baike.yfazqb.com/Article/details/gjftdcvfa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/gqgipszpr.sHtML

[R14] C 风格 for
来源：http://www.share.sjlbkw.cn/Article/details/gvlkpbiiv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gmapmgigm.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gdonpijjh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.tarul.cn/Article/details/gcpxvfvhk.sHtML

[R16] until 等待条件
来源：http://www.share.tarul.cn/Article/details/gngpivmkj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/gsllznqyl.sHtML

[R17] 数组定义与取值
来源：http://www.share.tarul.cn/Article/details/ggfhbrtxx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.tarul.cn/Article/details/gscluftbw.sHtML

[R18] 遍历数组
来源：http://mobile.bbcook.cn/Article/details/gukfagjwg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.bbcook.cn/Article/details/govqycdce.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/gqiejzblw.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/gxxotfrsq.sHtML

[R20] 关联数组（字典）
来源：http://m.share.yfazqb.com/Article/details/gwwkqyuur.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fktsv.cn/Article/details/gbrrnpavc.sHtML

[R21] 字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/geemncvos.sHtML

echo "${#s}"
来源：http://www.m.share.epnwcf.com/Article/details/gorlsalti.sHtML

[R22] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gyzbjzicw.sHtML

echo "${s:0:5}"
来源：http://www.share.bbcook.cn/Article/details/ggcuoojas.sHtML

[R23] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gcnjiweow.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.bbcook.cn/Article/details/gmcxesfci.sHtML

[R24] 大小写转换
来源：http://baike.bbcook.cn/Article/details/giqazfslh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.yfazqb.com/Article/details/ggxitevmb.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.epnwcf.com/Article/details/gnhejvpih.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.bbcook.cn/Article/details/gnsopzpzh.sHtML

[R26] 命令替换
来源：http://www.blog.fktsv.cn/Article/details/gnaygvnvo.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.tarul.cn/Article/details/gfmeqwiyt.sHtML

[R27] 算术展开
来源：http://read.share.tarul.cn/Article/details/gpngxrnyk.sHtML

echo $((1 + 2 * 3))
来源：http://3g.epnwcf.com/Article/details/gwepjwgpw.sHtML

[R28] 浮点运算
来源：http://www.share.fktsv.cn/Article/details/gayppfief.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.bbcook.cn/Article/details/gsgbiutnv.sHtML

[R29] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gpzpjymia.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.sjlbkw.cn/Article/details/gsiqxdcog.sHtML

[R30] 函数返回状态码
来源：http://wap.vehdjk.com/Article/details/gxyacuubs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fktsv.cn/Article/details/gaoftidkb.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gsowkxiss.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/gyczrsvyd.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/glrcvgtii.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.tarul.cn/Article/details/gnokbqlug.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.epnwcf.com/Article/details/gwxaxirlc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fktsv.cn/Article/details/gytnmhkgw.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/gpevsbzoe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gtfgljump.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/gwqyazxic.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.vehdjk.com/Article/details/gizgvfwfr.sHtML

[R36] 并发执行多个任务
来源：http://blog.tarul.cn/Article/details/gzlqpzbzm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/gfwgxbtvg.sHtML

[R37] 把输出赋给变量
来源：http://baike.vehdjk.com/Article/details/gupvaaxyw.sHtML

files=$(ls -1)
来源：http://www.share.vehdjk.com/Article/details/gcmmxgncf.sHtML

[R38] 管道串联
来源：http://wap.bbcook.cn/Article/details/gorthsngu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.epnwcf.com/Article/details/gxuuvgvfc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.sjlbkw.cn/Article/details/geqpmtbqo.sHtML

cmd > out.log 2>&1
来源：http://m.share.bbcook.cn/Article/details/gcrsqiehq.sHtML

[R40] 追加写日志
来源：http://blog.vehdjk.com/Article/details/gblzuitze.sHtML

echo "log" >> out.log
来源：http://wap.sjlbkw.cn/Article/details/gtvbnrgzz.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/gvkezvlxr.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fktsv.cn/Article/details/glthzwisd.sHtML

[R42] 输入重定向
来源：http://www.m.share.bbcook.cn/Article/details/gqrqlattt.sHtML

wc -l < a.txt
来源：http://wap.sjlbkw.cn/Article/details/gqaasinwz.sHtML

[R43] 按名字查找文件
来源：http://www.blog.vehdjk.com/Article/details/gyemmjzje.sHtML

find . -name "*.log" -type f
来源：http://www.share.vehdjk.com/Article/details/gqtweqhav.sHtML

[R44] 按修改时间查找
来源：http://3g.sjlbkw.cn/Article/details/gyyqxwqmj.sHtML

find . -mtime -7 -type f
来源：http://baike.vehdjk.com/Article/details/gfgscnzva.sHtML

[R45] 批量删除
来源：http://blog.epnwcf.com/Article/details/gmgnvesic.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.bbcook.cn/Article/details/guujvknez.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fktsv.cn/Article/details/gofqfvpoq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fktsv.cn/Article/details/gwgdiceqh.sHtML

[R47] sed 单行替换
来源：http://blog.bbcook.cn/Article/details/gikdmyoaf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gitbjjqfh.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/gznjduqxe.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gjowefhrl.sHtML

[R49] awk 带条件
来源：http://www.share.vehdjk.com/Article/details/gzdntflbc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.bbcook.cn/Article/details/gpatqdftu.sHtML

[R50] awk 求和
来源：http://mobile.bbcook.cn/Article/details/ghhqnnhsx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.vehdjk.com/Article/details/gcuxixcca.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/godbkiyrx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.yfazqb.com/Article/details/gfdvrvysp.sHtML

[R52] 统计行数
来源：http://wap.vehdjk.com/Article/details/gjffehqkm.sHtML

wc -l a.txt
来源：http://baike.fktsv.cn/Article/details/gzhgjwjqa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.bbcook.cn/Article/details/gizdzphfe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.yfazqb.com/Article/details/glzlpchka.sHtML

[R54] 比较两个文件
来源：http://mobile.sjlbkw.cn/Article/details/gxjtlrxge.sHtML

diff a.txt b.txt
来源：http://m.share.vehdjk.com/Article/details/gpzxkpneo.sHtML

[R55] 压缩与解压
来源：http://www.share.vehdjk.com/Article/details/ghyheudjb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/gepyzethq.sHtML

[R56] 远程拷贝
来源：http://read.share.epnwcf.com/Article/details/glvywgzww.sHtML

scp file user@host:/path/
来源：http://baike.vehdjk.com/Article/details/gejzsrbsf.sHtML

[R57] 远程执行命令
来源：http://blog.tarul.cn/Article/details/gqbqdpkwp.sHtML

ssh user@host 'uptime'
来源：http://www.blog.yfazqb.com/Article/details/gpfyrscnh.sHtML

[R58] 下载文件
来源：http://www.m.share.tarul.cn/Article/details/gxmqbvjub.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.vehdjk.com/Article/details/gsdiujzkm.sHtML

[R59] 发 POST JSON
来源：http://blog.sjlbkw.cn/Article/details/gypiinpim.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.vehdjk.com/Article/details/gpggjnlzy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gmcpsyaqt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gdedorpzn.sHtML

[R61] 磁盘占用
来源：http://mobile.epnwcf.com/Article/details/gesvosfbf.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/gtlonbxxu.sHtML

[R62] 找最占空间的文件
来源：http://blog.epnwcf.com/Article/details/ghlbvepme.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.sjlbkw.cn/Article/details/gyfsycfwh.sHtML

[R63] 内存与进程
来源：http://wap.vehdjk.com/Article/details/glznfwbao.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.sjlbkw.cn/Article/details/gsmswntzl.sHtML

[R64] 结束进程
来源：http://m.share.yfazqb.com/Article/details/gfrpygclc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gtldtppcu.sHtML

[R65] 查看端口占用
来源：http://baike.yfazqb.com/Article/details/gkkmsmeve.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.epnwcf.com/Article/details/giczeyqrz.sHtML

[R66] 定时任务
来源：http://3g.vehdjk.com/Article/details/gskvfmdpv.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/gmwilykir.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.sjlbkw.cn/Article/details/gdimhzcdn.sHtML

openssl rand -hex 16
来源：http://blog.sjlbkw.cn/Article/details/gplgfwloo.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/gcwnpqhan.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.bbcook.cn/Article/details/gmpqkcftm.sHtML

[R69] 生成随机密码
来源：http://read.share.vehdjk.com/Article/details/gdatzmjsv.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.sjlbkw.cn/Article/details/gbbxzokry.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/gsozgjabt.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.vehdjk.com/Article/details/gvqkzygjf.sHtML

[R71] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gczhijdxz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.tarul.cn/Article/details/ghsbgjlml.sHtML

[R72] 等待端口就绪
来源：http://baike.bbcook.cn/Article/details/glitwdhgs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/gznhfpdpg.sHtML

[R73] 分割大日志
来源：http://mobile.tarul.cn/Article/details/gaztfioso.sHtML

split -l 1000 big.log part_
来源：http://www.share.fktsv.cn/Article/details/gpshujien.sHtML

[R74] 批量重命名
来源：http://www.blog.vehdjk.com/Article/details/gddlgtqek.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.epnwcf.com/Article/details/gygpwfztj.sHtML

[R75] 导出环境变量
来源：http://3g.fktsv.cn/Article/details/gzdvdsehr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.yfazqb.com/Article/details/gpqhitqyc.sHtML

[R76] 使用临时文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gscwlkcbv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gkqktxbxe.sHtML

[R77] 读取用户输入
来源：http://m.share.yfazqb.com/Article/details/gurcqopgl.sHtML

read -rp "请输入: " ans
来源：http://baike.fktsv.cn/Article/details/gzdzzsini.sHtML

[R78] 交互式菜单
来源：http://www.blog.sjlbkw.cn/Article/details/gxdpgbaqu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.tarul.cn/Article/details/gpluogwoy.sHtML

[R79] 解析命令行选项
来源：http://wap.tarul.cn/Article/details/gjksrcscn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.yfazqb.com/Article/details/gbdgbsxox.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.epnwcf.com/Article/details/gzyzrweob.sHtML

time ./run.sh
来源：http://mobile.sjlbkw.cn/Article/details/gtziusyfc.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqadvroeh.sHtML

S. C / C++ 专题
来源：http://mobile.fktsv.cn/Article/details/gnrsfjmfe.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdhfnyyhw.sHtML

[S01] C：Hello World
来源：http://read.share.tarul.cn/Article/details/gmufnasht.sHtML

#include <stdio.h>
来源：http://wap.tarul.cn/Article/details/gnxkuidtt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.bbcook.cn/Article/details/gbcesauck.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fktsv.cn/Article/details/gcgqrmdpe.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.tarul.cn/Article/details/gkztvrggd.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/gekvfhynv.sHtML

int x; scanf("%d", &x);
来源：http://m.share.yfazqb.com/Article/details/gdlhegiip.sHtML

[S04] C：字符串复制
来源：http://www.m.share.tarul.cn/Article/details/gexdmumve.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.yfazqb.com/Article/details/gchbaqnxo.sHtML

[S05] C：字符串长度
来源：http://blog.tarul.cn/Article/details/gznymnphg.sHtML

strlen(s)
来源：http://baike.tarul.cn/Article/details/gwugzjwxx.sHtML

[S06] C：字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gbhxrbbvl.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fktsv.cn/Article/details/gqksyhliw.sHtML

[S07] C：数组遍历求和
来源：http://baike.bbcook.cn/Article/details/gbfmbsvgh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.yfazqb.com/Article/details/gztyoaufq.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.tarul.cn/Article/details/gvnbpprik.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/gszdwdfwe.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.vehdjk.com/Article/details/gnxidbvjq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fktsv.cn/Article/details/gfvjdyvhg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.epnwcf.com/Article/details/ggrmmjwry.sHtML

int *p = &a;  *p = 5;
来源：http://wap.vehdjk.com/Article/details/gporxdfuv.sHtML

[S11] C：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gkjbxfqkx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.vehdjk.com/Article/details/gdkvfjygp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.epnwcf.com/Article/details/gesxfsssl.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gulzafwin.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/gkubpqynd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.epnwcf.com/Article/details/gthpmzaqa.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/gkcwyrqvv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.sjlbkw.cn/Article/details/gnvptsyax.sHtML

[S14] C：枚举
来源：http://m.share.bbcook.cn/Article/details/gjuzkgxxz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.vehdjk.com/Article/details/gkvxrekyw.sHtML

[S15] C：类型转换
来源：http://wap.bbcook.cn/Article/details/gzquypzfx.sHtML

(double) a / b
来源：http://www.m.share.epnwcf.com/Article/details/ggtzziwnp.sHtML

[S16] C：位操作置位
来源：http://mobile.epnwcf.com/Article/details/gkrpmlmur.sHtML

x |= (1 << 3);
来源：http://3g.yfazqb.com/Article/details/goduyzxdt.sHtML

[S17] C：安全拼接字符串
来源：http://blog.bbcook.cn/Article/details/gqhkiolfh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.bbcook.cn/Article/details/gypyfbfhz.sHtML

[S18] C：命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/ggnphajrp.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/ghucxhnqe.sHtML

[S19] C：快速排序
来源：http://www.blog.epnwcf.com/Article/details/gqikkprii.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/gqukvyxkb.sHtML

[S20] C：二分查找
来源：http://wap.vehdjk.com/Article/details/ghotkpqgq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gyedmmjex.sHtML

[S21] C：字符类别判断
来源：http://m.share.epnwcf.com/Article/details/glzdludcq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.epnwcf.com/Article/details/gjvcwdqnf.sHtML

[S22] C：字符串转数字
来源：http://read.share.epnwcf.com/Article/details/gjxbuuxmd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/gohqmvpyh.sHtML

[S23] C：随机数
来源：http://mobile.tarul.cn/Article/details/gfsaulvch.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.yfazqb.com/Article/details/gmsxudpzm.sHtML

[S24] C：获取本地时间
来源：http://read.share.sjlbkw.cn/Article/details/grxzqvgnu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.vehdjk.com/Article/details/gjloofmnm.sHtML

[S25] C：内存拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gbwgjzqqo.sHtML

memcpy(dst, src, n);
来源：http://baike.fktsv.cn/Article/details/gkrrwgptw.sHtML

[S26] C：内存清零
来源：http://read.share.tarul.cn/Article/details/gwycdwxil.sHtML

memset(a, 0, sizeof a);
来源：http://wap.yfazqb.com/Article/details/gbuynalhm.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/ggeephrwb.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gtviqqdzg.sHtML

[S28] C：静态变量
来源：http://www.share.tarul.cn/Article/details/gccmrqioh.sHtML

static int counter = 0;
来源：http://www.share.yfazqb.com/Article/details/gamdjmode.sHtML

[S29] C：变参函数
来源：http://blog.sjlbkw.cn/Article/details/gspqhnnom.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.sjlbkw.cn/Article/details/gcafxptcp.sHtML

[S30] C：头文件保护
来源：http://wap.tarul.cn/Article/details/gycohqine.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/gxbevnnwk.sHtML

#define X_H
来源：http://www.share.sjlbkw.cn/Article/details/ghlblfdtc.sHtML

#endif
来源：http://mobile.bbcook.cn/Article/details/gtzzeuogd.sHtML

[S31] C++：Hello World
来源：http://baike.vehdjk.com/Article/details/gtfhhiekm.sHtML

#include <iostream>
来源：http://mobile.fktsv.cn/Article/details/gtmewtplu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fktsv.cn/Article/details/ggopmlhfg.sHtML

[S32] C++：字符串
来源：http://www.blog.bbcook.cn/Article/details/gtvnfwmjk.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fktsv.cn/Article/details/gxkcjogzm.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.tarul.cn/Article/details/ghqyvavza.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.tarul.cn/Article/details/gyyubyhdq.sHtML

[S34] C++：遍历 vector
来源：http://wap.epnwcf.com/Article/details/ghjmkzxec.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.bbcook.cn/Article/details/gqhnaifxd.sHtML

[S35] C++：map
来源：http://m.share.vehdjk.com/Article/details/gnutpllfl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gowodrvur.sHtML

[S36] C++：unordered_map
来源：http://m.share.sjlbkw.cn/Article/details/gaieenyqu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/grgzzbkqd.sHtML

[S37] C++：set
来源：http://www.m.share.sjlbkw.cn/Article/details/glfgfmwds.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.vehdjk.com/Article/details/gdlxgicnm.sHtML

[S38] C++：排序
来源：http://wap.epnwcf.com/Article/details/glojdcetj.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.epnwcf.com/Article/details/gyiwklufo.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.yfazqb.com/Article/details/gisijeqei.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.vehdjk.com/Article/details/gtifcumzf.sHtML

[S40] C++：查找元素
来源：http://baike.vehdjk.com/Article/details/gulnmungi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/gjpzgmwto.sHtML

[S41] C++：类与构造函数
来源：http://3g.yfazqb.com/Article/details/ggsispxqo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.epnwcf.com/Article/details/gefdjpxpr.sHtML

[S42] C++：继承与虚函数
来源：http://blog.yfazqb.com/Article/details/gguxfwlaf.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fktsv.cn/Article/details/gddztzqbq.sHtML

[S43] C++：智能指针
来源：http://baike.fktsv.cn/Article/details/gxqlpnsip.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.yfazqb.com/Article/details/gtpnfadrw.sHtML

[S44] C++：引用传参
来源：http://baike.vehdjk.com/Article/details/glfaqxmur.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.tarul.cn/Article/details/gbvmhccup.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/gczvwldfs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/gwsdrbxll.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/gwsephcrz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.tarul.cn/Article/details/gajohecmi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.bbcook.cn/Article/details/gcsqztpvd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.epnwcf.com/Article/details/gfuwpzotq.sHtML

[S48] C++：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gitfbshsl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gmrpfntkj.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.bbcook.cn/Article/details/gicdmlwyt.sHtML

[S49] C++：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gntspywkf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.tarul.cn/Article/details/gzecqkbln.sHtML

[S50] C++：格式化数字
来源：http://baike.sjlbkw.cn/Article/details/gmhunphix.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gwotocgzm.sHtML

[S51] C++：显式类型转换
来源：http://www.share.vehdjk.com/Article/details/gmcowrhzo.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/govsnamqs.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fktsv.cn/Article/details/gwkbhiiql.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.vehdjk.com/Article/details/gnuvzvaiu.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/gpneoxiij.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gbxvosrwf.sHtML

[S54] C++：异常处理
来源：http://m.share.tarul.cn/Article/details/gmcqoldpt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.yfazqb.com/Article/details/gtikfwbjw.sHtML

[S55] C++：结构化绑定
来源：http://baike.vehdjk.com/Article/details/gxhzwdkun.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.epnwcf.com/Article/details/gjophuxft.sHtML

[S56] C++：optional
来源：http://wap.vehdjk.com/Article/details/gthzaglop.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpffpbbck.sHtML

[S57] C++：编译期常量
来源：http://blog.tarul.cn/Article/details/gpxlyexdb.sHtML

constexpr int N = 10;
来源：http://read.share.tarul.cn/Article/details/gwmagykox.sHtML

[S58] C++：命名空间
来源：http://m.share.epnwcf.com/Article/details/gfuejiikh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.bbcook.cn/Article/details/gkcmczqou.sHtML

[S59] C++：静态断言
来源：http://wap.epnwcf.com/Article/details/goqvwigtk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.tarul.cn/Article/details/gxqjwpcna.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fktsv.cn/Article/details/gzktzqjwl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.yfazqb.com/Article/details/gtcpzosxs.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvxshekpx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.sjlbkw.cn/Article/details/gefwrystt.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmonbvmye.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.yfazqb.com/Article/details/gxhtprebx.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gzwogvwxu.sHtML

[T02] Kotlin：变量
来源：http://wap.epnwcf.com/Article/details/gpmwroodb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/gupeegore.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.yfazqb.com/Article/details/gnxofijsk.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/gbxsajmjh.sHtML

[T04] Kotlin：空安全
来源：http://mobile.tarul.cn/Article/details/gcacmwpam.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fktsv.cn/Article/details/gdqxsztwg.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.epnwcf.com/Article/details/glooaffry.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.tarul.cn/Article/details/ggzqnmxnw.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.tarul.cn/Article/details/gptvngtsh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fktsv.cn/Article/details/gthpcdnvh.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.bbcook.cn/Article/details/gqyvvtrxv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.bbcook.cn/Article/details/gwqxhmhqs.sHtML

[T08] Kotlin：数据类
来源：http://wap.epnwcf.com/Article/details/ggcrdmuhv.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.epnwcf.com/Article/details/gsoliyfda.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fktsv.cn/Article/details/graffmwwa.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.bbcook.cn/Article/details/gvldbatkr.sHtML

[T10] Kotlin：默认参数
来源：http://baike.yfazqb.com/Article/details/guzazmifi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.yfazqb.com/Article/details/gfvtazdpo.sHtML


<!-- 参考信息 -->