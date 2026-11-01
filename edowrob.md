代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/gvweobcvh.sHtML

[R14] C 风格 for
来源：http://www.blog.sjlbkw.cn/Article/details/gmskpugrx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gchucruxn.sHtML

[R15] while 逐行读文件
来源：http://blog.tarul.cn/Article/details/grurezdqv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.tarul.cn/Article/details/gciuvxnkk.sHtML

[R16] until 等待条件
来源：http://3g.bbcook.cn/Article/details/gypfxnrfh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gkyeidrrp.sHtML

[R17] 数组定义与取值
来源：http://read.share.epnwcf.com/Article/details/gkcqhfqqx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/grfpoqacu.sHtML

[R18] 遍历数组
来源：http://m.share.bbcook.cn/Article/details/gzqacxlay.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/gwdrtaxbj.sHtML

[R19] 数组长度
来源：http://www.m.share.vehdjk.com/Article/details/gpwwwzkoq.sHtML

echo "${#arr[@]}"
来源：http://mobile.sjlbkw.cn/Article/details/gwqcbseoa.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjywvpfls.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fktsv.cn/Article/details/gvvmxfmke.sHtML

[R21] 字符串长度
来源：http://blog.yfazqb.com/Article/details/gnnauzisk.sHtML

echo "${#s}"
来源：http://www.m.share.bbcook.cn/Article/details/gavbfohvo.sHtML

[R22] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gddafcdzv.sHtML

echo "${s:0:5}"
来源：http://3g.fktsv.cn/Article/details/gadothgqs.sHtML

[R23] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gzbweurfm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gypuxnvuq.sHtML

[R24] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gshmicsfk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fktsv.cn/Article/details/gzglynfdp.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.epnwcf.com/Article/details/gszlujpij.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.bbcook.cn/Article/details/gfrqlbiin.sHtML

[R26] 命令替换
来源：http://wap.bbcook.cn/Article/details/gbzsfucso.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.epnwcf.com/Article/details/gmqewjtwh.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gtebysqzp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.vehdjk.com/Article/details/gxpmmzzpr.sHtML

[R28] 浮点运算
来源：http://www.share.epnwcf.com/Article/details/glbvalnxu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.sjlbkw.cn/Article/details/gfhwebjao.sHtML

[R29] 定义函数
来源：http://www.share.vehdjk.com/Article/details/gqrvklsmj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/giqzuqyuf.sHtML

[R30] 函数返回状态码
来源：http://www.share.epnwcf.com/Article/details/gutpngorq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.bbcook.cn/Article/details/gnhzrmzjr.sHtML

[R31] 局部变量
来源：http://www.share.vehdjk.com/Article/details/ghqwzqjna.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.vehdjk.com/Article/details/gkzntdwlb.sHtML

[R32] 参数个数校验
来源：http://wap.tarul.cn/Article/details/grilvhjtn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/ggkzaxiry.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.tarul.cn/Article/details/gokvcmhcx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fktsv.cn/Article/details/gxzdkuhxu.sHtML

[R34] 退出时清理
来源：http://3g.epnwcf.com/Article/details/gyrbgskpe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/guqhyibwb.sHtML

[R35] 后台执行并等待
来源：http://www.share.epnwcf.com/Article/details/guftjazdx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.sjlbkw.cn/Article/details/gplkgdnxg.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.vehdjk.com/Article/details/gavntcajh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.vehdjk.com/Article/details/gfsptqkvt.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.epnwcf.com/Article/details/gvjxgnedw.sHtML

files=$(ls -1)
来源：http://www.m.share.vehdjk.com/Article/details/gfacqjfdc.sHtML

[R38] 管道串联
来源：http://3g.vehdjk.com/Article/details/gdhuflcse.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.sjlbkw.cn/Article/details/gcryiedjl.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/gsrntotfp.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gwohcrnjc.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/gttkbbtay.sHtML

echo "log" >> out.log
来源：http://m.share.vehdjk.com/Article/details/gbkxcltsa.sHtML

[R41] 丢弃输出
来源：http://wap.fktsv.cn/Article/details/gzfwgvmjy.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.yfazqb.com/Article/details/gvwpsivji.sHtML

[R42] 输入重定向
来源：http://3g.tarul.cn/Article/details/goijhknug.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/gqlikbqjc.sHtML

[R43] 按名字查找文件
来源：http://www.blog.epnwcf.com/Article/details/gvhdwuzrn.sHtML

find . -name "*.log" -type f
来源：http://m.share.vehdjk.com/Article/details/gytrqrldc.sHtML

[R44] 按修改时间查找
来源：http://3g.fktsv.cn/Article/details/gqnfohwoi.sHtML

find . -mtime -7 -type f
来源：http://mobile.vehdjk.com/Article/details/gpqqabxdk.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/gdhqensio.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.yfazqb.com/Article/details/gwluoyebg.sHtML

[R46] 递归替换文件内容
来源：http://3g.epnwcf.com/Article/details/ghzncbfsf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.tarul.cn/Article/details/gywfojjhy.sHtML

[R47] sed 单行替换
来源：http://blog.vehdjk.com/Article/details/goysjouoy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gevqpxlve.sHtML

[R48] awk 取指定列
来源：http://read.share.epnwcf.com/Article/details/gzysmxqlb.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.tarul.cn/Article/details/gozmeushz.sHtML

[R49] awk 带条件
来源：http://baike.yfazqb.com/Article/details/gghgaobfz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.bbcook.cn/Article/details/grpmjrgyf.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/gvglssrga.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gstmoglsk.sHtML

[R51] 排序去重取前几
来源：http://wap.tarul.cn/Article/details/glfbyhqsz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.vehdjk.com/Article/details/ghxypwtpw.sHtML

[R52] 统计行数
来源：http://3g.sjlbkw.cn/Article/details/gcmzxjxvq.sHtML

wc -l a.txt
来源：http://mobile.yfazqb.com/Article/details/gweoyacyr.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.bbcook.cn/Article/details/gfmmmwdpv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.yfazqb.com/Article/details/ghykgugdu.sHtML

[R54] 比较两个文件
来源：http://read.share.sjlbkw.cn/Article/details/gkgnbsyzf.sHtML

diff a.txt b.txt
来源：http://baike.epnwcf.com/Article/details/ggzdtiqnf.sHtML

[R55] 压缩与解压
来源：http://baike.bbcook.cn/Article/details/gqibematt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.yfazqb.com/Article/details/gedcxqhmr.sHtML

[R56] 远程拷贝
来源：http://www.share.bbcook.cn/Article/details/gcogzybsm.sHtML

scp file user@host:/path/
来源：http://www.share.bbcook.cn/Article/details/gqphnhyqq.sHtML

[R57] 远程执行命令
来源：http://baike.epnwcf.com/Article/details/ghicwxoss.sHtML

ssh user@host 'uptime'
来源：http://m.share.epnwcf.com/Article/details/gbgyhitsb.sHtML

[R58] 下载文件
来源：http://www.blog.tarul.cn/Article/details/gypngsbro.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.epnwcf.com/Article/details/guoamubsq.sHtML

[R59] 发 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/gxeyagkqa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/gwsdkzlcj.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gxauomngl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/gmmtsglue.sHtML

[R61] 磁盘占用
来源：http://baike.yfazqb.com/Article/details/gnfoqkfzf.sHtML

df -h;  du -sh *
来源：http://www.m.share.epnwcf.com/Article/details/gqygudxec.sHtML

[R62] 找最占空间的文件
来源：http://3g.epnwcf.com/Article/details/gxjiwogxe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.epnwcf.com/Article/details/gycvbubij.sHtML

[R63] 内存与进程
来源：http://read.share.sjlbkw.cn/Article/details/gbvyuxjwb.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.epnwcf.com/Article/details/gjtmppxwo.sHtML

[R64] 结束进程
来源：http://www.m.share.epnwcf.com/Article/details/glvdeybzl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/gtrqzeqtt.sHtML

[R65] 查看端口占用
来源：http://read.share.vehdjk.com/Article/details/ginktdyfd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.epnwcf.com/Article/details/gxubtgzvo.sHtML

[R66] 定时任务
来源：http://3g.sjlbkw.cn/Article/details/gtqlcjnvs.sHtML

crontab -e;  crontab -l
来源：http://3g.fktsv.cn/Article/details/gihdoextw.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/gprkymbtq.sHtML

openssl rand -hex 16
来源：http://www.blog.epnwcf.com/Article/details/gkjszdeyp.sHtML

[R68] 计算文件校验值
来源：http://wap.epnwcf.com/Article/details/gkycoowgl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.yfazqb.com/Article/details/gjqwbwhum.sHtML

[R69] 生成随机密码
来源：http://m.share.bbcook.cn/Article/details/gwrammluw.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.sjlbkw.cn/Article/details/gslcjfrab.sHtML

[R70] 时间戳与互转
来源：http://www.share.vehdjk.com/Article/details/gqbgmqguq.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.vehdjk.com/Article/details/gycpbifqz.sHtML

[R71] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gcrmelmqc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fktsv.cn/Article/details/gvigbqjpz.sHtML

[R72] 等待端口就绪
来源：http://www.blog.bbcook.cn/Article/details/gpfkfvhjv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/giqeuzdir.sHtML

[R73] 分割大日志
来源：http://www.blog.sjlbkw.cn/Article/details/gnilstpev.sHtML

split -l 1000 big.log part_
来源：http://www.share.vehdjk.com/Article/details/gnsbaxewb.sHtML

[R74] 批量重命名
来源：http://3g.fktsv.cn/Article/details/glqmcvrjt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/gcnzbupeu.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/grlynjpkn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.tarul.cn/Article/details/gmeyizdzv.sHtML

[R76] 使用临时文件
来源：http://m.share.sjlbkw.cn/Article/details/gzbyzlcub.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gjtlmxghh.sHtML

[R77] 读取用户输入
来源：http://3g.fktsv.cn/Article/details/ghgzrpeqb.sHtML

read -rp "请输入: " ans
来源：http://mobile.epnwcf.com/Article/details/gjiggtedu.sHtML

[R78] 交互式菜单
来源：http://mobile.fktsv.cn/Article/details/gigxvwscn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.yfazqb.com/Article/details/gqtkbxfja.sHtML

[R79] 解析命令行选项
来源：http://baike.fktsv.cn/Article/details/ggsedrrrf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/gskcuzcyd.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.tarul.cn/Article/details/gmeronawi.sHtML

time ./run.sh
来源：http://mobile.epnwcf.com/Article/details/gdjwmdbwg.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/geslswwcn.sHtML

S. C / C++ 专题
来源：http://wap.bbcook.cn/Article/details/gyhhnzkbx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gmswupsbk.sHtML

[S01] C：Hello World
来源：http://read.share.epnwcf.com/Article/details/gexxcfohj.sHtML

#include <stdio.h>
来源：http://mobile.epnwcf.com/Article/details/gahovajcr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.bbcook.cn/Article/details/geqmehxyb.sHtML

[S02] C：变量与格式化输出
来源：http://blog.bbcook.cn/Article/details/gckqlzmgw.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.vehdjk.com/Article/details/gvlkxgwji.sHtML

[S03] C：读入整数
来源：http://read.share.fktsv.cn/Article/details/gtajxrbfe.sHtML

int x; scanf("%d", &x);
来源：http://3g.bbcook.cn/Article/details/gzpotzilg.sHtML

[S04] C：字符串复制
来源：http://www.m.share.epnwcf.com/Article/details/gkbqsyjgg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gazcmcsyr.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/ggknmocir.sHtML

strlen(s)
来源：http://3g.fktsv.cn/Article/details/gtopmzfsp.sHtML

[S06] C：字符串比较
来源：http://m.share.tarul.cn/Article/details/gjkvcbwbc.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/gzehbruwa.sHtML

[S07] C：数组遍历求和
来源：http://baike.tarul.cn/Article/details/gfrszcvdm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.sjlbkw.cn/Article/details/gizdkgtlg.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.bbcook.cn/Article/details/ggzyoclua.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.epnwcf.com/Article/details/gjueuxiqe.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.epnwcf.com/Article/details/gccgnsjbs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.bbcook.cn/Article/details/gmgrlamnb.sHtML

[S10] C：指针与解引用
来源：http://3g.vehdjk.com/Article/details/gccizmexy.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fktsv.cn/Article/details/gzstzvisa.sHtML

[S11] C：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/ghtaqkncs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fktsv.cn/Article/details/ghsgokkgz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.tarul.cn/Article/details/gqylyjvtj.sHtML

fclose(f);
来源：http://baike.yfazqb.com/Article/details/gvuusdmaq.sHtML

[S12] C：写文件
来源：http://read.share.tarul.cn/Article/details/gpldgpexa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.yfazqb.com/Article/details/gmyxgxmtm.sHtML

[S13] C：宏定义
来源：http://www.m.share.sjlbkw.cn/Article/details/grkzcvdrt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.sjlbkw.cn/Article/details/gyaospgbj.sHtML

[S14] C：枚举
来源：http://www.m.share.vehdjk.com/Article/details/gumpreqbu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fktsv.cn/Article/details/gyboocjdu.sHtML

[S15] C：类型转换
来源：http://baike.sjlbkw.cn/Article/details/gmyvpjblf.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/gnqecplff.sHtML

[S16] C：位操作置位
来源：http://m.share.fktsv.cn/Article/details/gzwuwpkac.sHtML

x |= (1 << 3);
来源：http://mobile.yfazqb.com/Article/details/gwsewyjqx.sHtML

[S17] C：安全拼接字符串
来源：http://blog.tarul.cn/Article/details/gixkgrmhb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.epnwcf.com/Article/details/ggupdhjkc.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gvmzbeqca.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gnvlwnnev.sHtML

[S19] C：快速排序
来源：http://baike.vehdjk.com/Article/details/gihjxrybu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/gnaelemlz.sHtML

[S20] C：二分查找
来源：http://m.share.fktsv.cn/Article/details/glcxcwxkt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gmtxlgmol.sHtML

[S21] C：字符类别判断
来源：http://www.share.fktsv.cn/Article/details/gjefeqmtd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/gfsnurwlg.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/gglejrpsj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.bbcook.cn/Article/details/gyacxxjzt.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/gfmifgztn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.sjlbkw.cn/Article/details/gwkchcjxw.sHtML

[S24] C：获取本地时间
来源：http://wap.epnwcf.com/Article/details/gqfstywqo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.epnwcf.com/Article/details/gtzvlzgzc.sHtML

[S25] C：内存拷贝
来源：http://read.share.fktsv.cn/Article/details/godipidyc.sHtML

memcpy(dst, src, n);
来源：http://3g.fktsv.cn/Article/details/gowzdrhsa.sHtML

[S26] C：内存清零
来源：http://www.m.share.epnwcf.com/Article/details/grbuxonfu.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.bbcook.cn/Article/details/grnuccojh.sHtML

[S27] C：定义常量
来源：http://www.m.share.vehdjk.com/Article/details/gtgtdwghs.sHtML

const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gwarqquim.sHtML

[S28] C：静态变量
来源：http://m.share.fktsv.cn/Article/details/ghafgqrsf.sHtML

static int counter = 0;
来源：http://3g.fktsv.cn/Article/details/gdvxqogpw.sHtML

[S29] C：变参函数
来源：http://3g.epnwcf.com/Article/details/gqsjpfqrt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.tarul.cn/Article/details/gswmgkgoc.sHtML

[S30] C：头文件保护
来源：http://www.blog.vehdjk.com/Article/details/gytjckahc.sHtML

#ifndef X_H
来源：http://www.blog.vehdjk.com/Article/details/goasxpyjj.sHtML

#define X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gurkpvnoe.sHtML

#endif
来源：http://wap.bbcook.cn/Article/details/gtzsyqypq.sHtML

[S31] C++：Hello World
来源：http://read.share.vehdjk.com/Article/details/glvfwnsnz.sHtML

#include <iostream>
来源：http://www.blog.bbcook.cn/Article/details/gliogetqp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpazkzogc.sHtML

[S32] C++：字符串
来源：http://m.share.bbcook.cn/Article/details/gmvimqcel.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fktsv.cn/Article/details/gbrmsqcso.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvgqvtdr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.epnwcf.com/Article/details/guisxlbfw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.vehdjk.com/Article/details/gspntadzv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.vehdjk.com/Article/details/gwtdanpxw.sHtML

[S35] C++：map
来源：http://3g.tarul.cn/Article/details/gcwevfbsi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gqbxckrmy.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.epnwcf.com/Article/details/gtxmwixmw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gyvibxwiz.sHtML

[S37] C++：set
来源：http://baike.bbcook.cn/Article/details/gcjjsyrag.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.sjlbkw.cn/Article/details/gbnssdevd.sHtML

[S38] C++：排序
来源：http://wap.fktsv.cn/Article/details/gozmoqsad.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.yfazqb.com/Article/details/gezglnrkf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.yfazqb.com/Article/details/giaorecjh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.vehdjk.com/Article/details/ghbesimgq.sHtML

[S40] C++：查找元素
来源：http://www.m.share.yfazqb.com/Article/details/gqtpttzmi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.sjlbkw.cn/Article/details/ghuaaoeqa.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gmzqppaeh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.yfazqb.com/Article/details/gxikegecy.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/gijizjgcy.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.vehdjk.com/Article/details/ghvdoytyc.sHtML

[S43] C++：智能指针
来源：http://m.share.yfazqb.com/Article/details/ginnypkwa.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gtqksvspu.sHtML

[S44] C++：引用传参
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpebqrhm.sHtML

void inc(int &x) { ++x; }
来源：http://wap.bbcook.cn/Article/details/gndxviumt.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/gtbyscazg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/gmkftbazy.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gopvshaef.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.tarul.cn/Article/details/gukghupfk.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/grluqenvx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gfhrshpny.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gopdvpmeu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.epnwcf.com/Article/details/gwsekcbkn.sHtML

while (std::getline(in, line)) { }
来源：http://wap.vehdjk.com/Article/details/gaydcvhfk.sHtML

[S49] C++：写文件
来源：http://www.share.vehdjk.com/Article/details/gtuwvxepq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fktsv.cn/Article/details/gqqwibdid.sHtML

[S50] C++：格式化数字
来源：http://3g.vehdjk.com/Article/details/golcxczyr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/goktmvzqr.sHtML

[S51] C++：显式类型转换
来源：http://blog.epnwcf.com/Article/details/glaqmipzp.sHtML

static_cast<double>(a) / b
来源：http://www.blog.bbcook.cn/Article/details/gposlqzds.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/girkfjrxj.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.epnwcf.com/Article/details/gfsfpaxrp.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/glgfpjhya.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/gbmxwpeed.sHtML

[S54] C++：异常处理
来源：http://3g.sjlbkw.cn/Article/details/giyefpoib.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.bbcook.cn/Article/details/gydibfavu.sHtML

[S55] C++：结构化绑定
来源：http://mobile.tarul.cn/Article/details/gjvjcdfqa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/gbymbljmm.sHtML

[S56] C++：optional
来源：http://blog.fktsv.cn/Article/details/givvvugnb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.tarul.cn/Article/details/gfhqfoxlp.sHtML

[S57] C++：编译期常量
来源：http://www.share.bbcook.cn/Article/details/gclftvoxt.sHtML

constexpr int N = 10;
来源：http://baike.bbcook.cn/Article/details/gvgpuxinv.sHtML

[S58] C++：命名空间
来源：http://www.blog.bbcook.cn/Article/details/gmixxaumg.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.tarul.cn/Article/details/gwirknotw.sHtML

[S59] C++：静态断言
来源：http://www.share.epnwcf.com/Article/details/gtfrghplf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.tarul.cn/Article/details/gnnwrpfcp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fktsv.cn/Article/details/gmapjtcqp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fktsv.cn/Article/details/gvpssozvk.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gigkdlqhy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gixmzsafy.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gotqocgjx.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fktsv.cn/Article/details/gwinyohpc.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gjcdmgxpe.sHtML

[T02] Kotlin：变量
来源：http://mobile.yfazqb.com/Article/details/gukcwgyyt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/goqquqelc.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.sjlbkw.cn/Article/details/gvgivukra.sHtML

"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gvwwrdzet.sHtML

[T04] Kotlin：空安全
来源：http://www.share.yfazqb.com/Article/details/gbygafqjc.sHtML

val n: String? = null;  n?.length
来源：http://mobile.bbcook.cn/Article/details/gyqxhqcps.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gatxxnpvy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.tarul.cn/Article/details/gkkegfyun.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fktsv.cn/Article/details/gsggauzvh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.tarul.cn/Article/details/gqiezxaqd.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/gytiwivpb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.bbcook.cn/Article/details/gxdbtncso.sHtML

[T08] Kotlin：数据类
来源：http://wap.vehdjk.com/Article/details/gucxudhwz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fktsv.cn/Article/details/gptuvkpbu.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.bbcook.cn/Article/details/gwncmpjcv.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.epnwcf.com/Article/details/gjwwsohom.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.tarul.cn/Article/details/ggecpfdsq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fktsv.cn/Article/details/gjsqjboul.sHtML

[T11] Kotlin：协程
来源：http://www.blog.epnwcf.com/Article/details/gdjcdmrro.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.tarul.cn/Article/details/ghxfoqplv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.epnwcf.com/Article/details/gxhhoktmg.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gxatnghce.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.bbcook.cn/Article/details/gxqgnnthm.sHtML

val m = mapOf("a" to 1)
来源：http://blog.sjlbkw.cn/Article/details/gwhxdbbel.sHtML

[T14] Kotlin：循环
来源：http://3g.sjlbkw.cn/Article/details/gmnateqqs.sHtML

for (i in 1..10) println(i)
来源：http://3g.epnwcf.com/Article/details/gsewhetli.sHtML

[T15] Kotlin：接口
来源：http://wap.sjlbkw.cn/Article/details/gzteduaav.sHtML

interface Shape { fun area(): Double }
来源：http://wap.tarul.cn/Article/details/gzwdbofqx.sHtML

[T16] Swift：Hello World
来源：http://blog.yfazqb.com/Article/details/gkolgcldz.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gkhowjhvo.sHtML


<!-- 参考信息 -->