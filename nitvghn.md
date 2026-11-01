代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gafodnfhp.sHtML

[R14] C 风格 for
来源：http://www.blog.fktsv.cn/Article/details/gkfvcgizy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/grzpqpnil.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/ggxkrwbdn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.bbcook.cn/Article/details/gvwxqrhge.sHtML

[R16] until 等待条件
来源：http://www.share.tarul.cn/Article/details/gwbvsutux.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/gzpnlrcqp.sHtML

[R17] 数组定义与取值
来源：http://www.share.sjlbkw.cn/Article/details/gqszliffu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.yfazqb.com/Article/details/gfjhsknni.sHtML

[R18] 遍历数组
来源：http://www.share.bbcook.cn/Article/details/gskmgfred.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.vehdjk.com/Article/details/gcmosbuvu.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/gkrwmdsyo.sHtML

echo "${#arr[@]}"
来源：http://blog.epnwcf.com/Article/details/ghplqoeav.sHtML

[R20] 关联数组（字典）
来源：http://baike.sjlbkw.cn/Article/details/gbfmozapq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.yfazqb.com/Article/details/gmhuqjrxj.sHtML

[R21] 字符串长度
来源：http://3g.epnwcf.com/Article/details/gdeqkgick.sHtML

echo "${#s}"
来源：http://read.share.sjlbkw.cn/Article/details/ghxpjaghl.sHtML

[R22] 截取子串
来源：http://m.share.vehdjk.com/Article/details/guymlqbfp.sHtML

echo "${s:0:5}"
来源：http://baike.epnwcf.com/Article/details/gzqpipvjy.sHtML

[R23] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gwjpzxguf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.yfazqb.com/Article/details/ggrrxskja.sHtML

[R24] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gxowlxatj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.tarul.cn/Article/details/gjqpjkhcp.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.sjlbkw.cn/Article/details/gtyxuxpqk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.tarul.cn/Article/details/glxmjwcls.sHtML

[R26] 命令替换
来源：http://m.share.tarul.cn/Article/details/gzfeimjlc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.epnwcf.com/Article/details/gaecynend.sHtML

[R27] 算术展开
来源：http://mobile.tarul.cn/Article/details/gkrkdgmer.sHtML

echo $((1 + 2 * 3))
来源：http://baike.vehdjk.com/Article/details/gbxvoefkn.sHtML

[R28] 浮点运算
来源：http://mobile.sjlbkw.cn/Article/details/glunhidqd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.sjlbkw.cn/Article/details/grlbvghpm.sHtML

[R29] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gvhswnapx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.vehdjk.com/Article/details/ggkzvgoll.sHtML

[R30] 函数返回状态码
来源：http://3g.yfazqb.com/Article/details/gwkgseosx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.yfazqb.com/Article/details/gjmformji.sHtML

[R31] 局部变量
来源：http://www.share.tarul.cn/Article/details/gwiuqewdp.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.epnwcf.com/Article/details/gmyeyrogh.sHtML

[R32] 参数个数校验
来源：http://m.share.tarul.cn/Article/details/gaqseahyo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gvdfzmuht.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.vehdjk.com/Article/details/gznvamrxf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.epnwcf.com/Article/details/ggoufdtlo.sHtML

[R34] 退出时清理
来源：http://m.share.sjlbkw.cn/Article/details/ggyfjnqvb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/gqzqcoihm.sHtML

[R35] 后台执行并等待
来源：http://3g.epnwcf.com/Article/details/gvxjyxhxs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.sjlbkw.cn/Article/details/gephennex.sHtML

[R36] 并发执行多个任务
来源：http://m.share.sjlbkw.cn/Article/details/gxufbnwwd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.yfazqb.com/Article/details/geluzxgca.sHtML

[R37] 把输出赋给变量
来源：http://m.share.vehdjk.com/Article/details/gtxmlihfi.sHtML

files=$(ls -1)
来源：http://m.share.yfazqb.com/Article/details/gbzulqfdu.sHtML

[R38] 管道串联
来源：http://3g.yfazqb.com/Article/details/guiyousfu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.yfazqb.com/Article/details/gorwswxdj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fktsv.cn/Article/details/gjujsiill.sHtML

cmd > out.log 2>&1
来源：http://www.share.yfazqb.com/Article/details/gknqqpbtw.sHtML

[R40] 追加写日志
来源：http://read.share.tarul.cn/Article/details/gbvyycyay.sHtML

echo "log" >> out.log
来源：http://m.share.fktsv.cn/Article/details/glxszrxhf.sHtML

[R41] 丢弃输出
来源：http://www.m.share.vehdjk.com/Article/details/glpzmnhuj.sHtML

cmd >/dev/null 2>&1
来源：http://wap.epnwcf.com/Article/details/gifcckcri.sHtML

[R42] 输入重定向
来源：http://www.blog.yfazqb.com/Article/details/gmvrvcood.sHtML

wc -l < a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gzjtjdzrc.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gndafqnoc.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.bbcook.cn/Article/details/gnlcnoytn.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.yfazqb.com/Article/details/gpmwxjxma.sHtML

find . -mtime -7 -type f
来源：http://www.share.yfazqb.com/Article/details/grhqzqtfh.sHtML

[R45] 批量删除
来源：http://www.m.share.yfazqb.com/Article/details/gspzmyrzg.sHtML

find . -name "*.tmp" -delete
来源：http://wap.vehdjk.com/Article/details/grphgjasy.sHtML

[R46] 递归替换文件内容
来源：http://m.share.bbcook.cn/Article/details/gvzulqtig.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/gyzesxwfk.sHtML

[R47] sed 单行替换
来源：http://3g.tarul.cn/Article/details/gcmhjvsdr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fktsv.cn/Article/details/gekrqwoib.sHtML

[R48] awk 取指定列
来源：http://mobile.epnwcf.com/Article/details/gihbzunqb.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.tarul.cn/Article/details/gpcfmgikp.sHtML

[R49] awk 带条件
来源：http://www.m.share.epnwcf.com/Article/details/ghghvsiwq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.bbcook.cn/Article/details/gppjpdyja.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/gyvsnlgag.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gipvhurbv.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjlvexxt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.tarul.cn/Article/details/gvdmsdpmb.sHtML

[R52] 统计行数
来源：http://m.share.vehdjk.com/Article/details/gsyeomxve.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/gxvowcvip.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.tarul.cn/Article/details/gfkraewkr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.epnwcf.com/Article/details/gzpuasuko.sHtML

[R54] 比较两个文件
来源：http://wap.vehdjk.com/Article/details/ghestkbcg.sHtML

diff a.txt b.txt
来源：http://m.share.bbcook.cn/Article/details/gqzyxzixr.sHtML

[R55] 压缩与解压
来源：http://wap.tarul.cn/Article/details/gbufzoojh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gwatdrxzt.sHtML

[R56] 远程拷贝
来源：http://read.share.vehdjk.com/Article/details/ghqktggqd.sHtML

scp file user@host:/path/
来源：http://baike.sjlbkw.cn/Article/details/gslgkbubg.sHtML

[R57] 远程执行命令
来源：http://read.share.bbcook.cn/Article/details/gjivcmxef.sHtML

ssh user@host 'uptime'
来源：http://m.share.tarul.cn/Article/details/gajdotbbc.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/glkuaadxp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fktsv.cn/Article/details/gefsqwzvb.sHtML

[R59] 发 POST JSON
来源：http://www.share.fktsv.cn/Article/details/gvqnjdjho.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.vehdjk.com/Article/details/gcexryutc.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/gjwtkfjva.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.bbcook.cn/Article/details/gsvothzsa.sHtML

[R61] 磁盘占用
来源：http://m.share.epnwcf.com/Article/details/gbcwaggaj.sHtML

df -h;  du -sh *
来源：http://wap.sjlbkw.cn/Article/details/guesqyiwu.sHtML

[R62] 找最占空间的文件
来源：http://read.share.sjlbkw.cn/Article/details/gtoiqltjz.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.sjlbkw.cn/Article/details/gobmlhhkv.sHtML

[R63] 内存与进程
来源：http://www.share.epnwcf.com/Article/details/gglsnyqyo.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.vehdjk.com/Article/details/gjtacdjji.sHtML

[R64] 结束进程
来源：http://blog.yfazqb.com/Article/details/grepnlflm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.vehdjk.com/Article/details/gqsoosbtm.sHtML

[R65] 查看端口占用
来源：http://mobile.sjlbkw.cn/Article/details/gtjfkainx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.epnwcf.com/Article/details/gkushkzbq.sHtML

[R66] 定时任务
来源：http://wap.sjlbkw.cn/Article/details/gumlycryn.sHtML

crontab -e;  crontab -l
来源：http://www.share.bbcook.cn/Article/details/gnxcwapih.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.yfazqb.com/Article/details/goctigdrd.sHtML

openssl rand -hex 16
来源：http://wap.yfazqb.com/Article/details/gmjksqcxh.sHtML

[R68] 计算文件校验值
来源：http://m.share.fktsv.cn/Article/details/guwkhjuyw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.tarul.cn/Article/details/gvkgpdefh.sHtML

[R69] 生成随机密码
来源：http://www.blog.epnwcf.com/Article/details/gowfqndvc.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.yfazqb.com/Article/details/gerxsvgjb.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/giapndcny.sHtML

date +%s;  date -d @1700000000
来源：http://3g.yfazqb.com/Article/details/gshewtobw.sHtML

[R71] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqbncdla.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.sjlbkw.cn/Article/details/gbhneiasf.sHtML

[R72] 等待端口就绪
来源：http://baike.vehdjk.com/Article/details/geselopfi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gtupbjswf.sHtML

[R73] 分割大日志
来源：http://baike.sjlbkw.cn/Article/details/gkipvfqke.sHtML

split -l 1000 big.log part_
来源：http://blog.epnwcf.com/Article/details/gwikqswnu.sHtML

[R74] 批量重命名
来源：http://m.share.yfazqb.com/Article/details/gbbypidtp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.vehdjk.com/Article/details/gcezgzmhw.sHtML

[R75] 导出环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gzcovqqed.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.bbcook.cn/Article/details/glclcatrg.sHtML

[R76] 使用临时文件
来源：http://m.share.vehdjk.com/Article/details/gqlrcoquq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/guysilojk.sHtML

[R77] 读取用户输入
来源：http://www.m.share.yfazqb.com/Article/details/gqjxfvyvl.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.yfazqb.com/Article/details/gtcytzoiw.sHtML

[R78] 交互式菜单
来源：http://blog.yfazqb.com/Article/details/ghqxaqsrx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.vehdjk.com/Article/details/gehwshmvf.sHtML

[R79] 解析命令行选项
来源：http://www.share.vehdjk.com/Article/details/gtidotbdn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.bbcook.cn/Article/details/gagfvjxxc.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.yfazqb.com/Article/details/ggijzgxcy.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gaysvcrei.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxsnurxrg.sHtML

S. C / C++ 专题
来源：http://www.blog.vehdjk.com/Article/details/gvnnrytup.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gpsognioz.sHtML

[S01] C：Hello World
来源：http://baike.sjlbkw.cn/Article/details/glolcnfsv.sHtML

#include <stdio.h>
来源：http://m.share.vehdjk.com/Article/details/gsoryughm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.epnwcf.com/Article/details/gbkazzmkl.sHtML

[S02] C：变量与格式化输出
来源：http://blog.bbcook.cn/Article/details/gdndtwzbw.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.epnwcf.com/Article/details/glpadhybu.sHtML

[S03] C：读入整数
来源：http://www.share.yfazqb.com/Article/details/gcwrxvovf.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/ghjtlkmrs.sHtML

[S04] C：字符串复制
来源：http://read.share.epnwcf.com/Article/details/gnvewyatk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.epnwcf.com/Article/details/geolsdnad.sHtML

[S05] C：字符串长度
来源：http://3g.sjlbkw.cn/Article/details/ghmwcpjhh.sHtML

strlen(s)
来源：http://3g.yfazqb.com/Article/details/gpvtmxoah.sHtML

[S06] C：字符串比较
来源：http://mobile.bbcook.cn/Article/details/gqfjpdlmb.sHtML

strcmp(a, b) == 0
来源：http://read.share.yfazqb.com/Article/details/gnaogmiac.sHtML

[S07] C：数组遍历求和
来源：http://baike.sjlbkw.cn/Article/details/glzpnadwj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.yfazqb.com/Article/details/gendgnzwf.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fktsv.cn/Article/details/gqgbbzlht.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fktsv.cn/Article/details/griwiudfi.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/gpvlqsxgp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.bbcook.cn/Article/details/gedwsmdxv.sHtML

[S10] C：指针与解引用
来源：http://read.share.yfazqb.com/Article/details/gutanccel.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/gpkickwnb.sHtML

[S11] C：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gberfnqcc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.tarul.cn/Article/details/gkydmdwyp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.bbcook.cn/Article/details/gkerjrlbg.sHtML

fclose(f);
来源：http://blog.vehdjk.com/Article/details/gulbkurrd.sHtML

[S12] C：写文件
来源：http://3g.fktsv.cn/Article/details/gfrkbbind.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/ghutyjfvd.sHtML

[S13] C：宏定义
来源：http://baike.yfazqb.com/Article/details/gbmqjuaxk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.bbcook.cn/Article/details/gtjighyky.sHtML

[S14] C：枚举
来源：http://wap.vehdjk.com/Article/details/gtvnginui.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.yfazqb.com/Article/details/gspgtwlpc.sHtML

[S15] C：类型转换
来源：http://www.share.vehdjk.com/Article/details/giewnqcir.sHtML

(double) a / b
来源：http://mobile.vehdjk.com/Article/details/ggidfugjq.sHtML

[S16] C：位操作置位
来源：http://www.share.yfazqb.com/Article/details/gizxpmuip.sHtML

x |= (1 << 3);
来源：http://mobile.yfazqb.com/Article/details/gkufydpuz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gqpybwkjb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fktsv.cn/Article/details/gbukwyzql.sHtML

[S18] C：命令行参数
来源：http://blog.yfazqb.com/Article/details/gtzepztom.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.epnwcf.com/Article/details/gtuwqwlsl.sHtML

[S19] C：快速排序
来源：http://www.share.yfazqb.com/Article/details/gxjstdkhw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gwjvmbymj.sHtML

[S20] C：二分查找
来源：http://3g.vehdjk.com/Article/details/guyfohybp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/gokokltgz.sHtML

[S21] C：字符类别判断
来源：http://wap.sjlbkw.cn/Article/details/gwjxktldw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.epnwcf.com/Article/details/gdilsbccb.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/gudmgadbz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.yfazqb.com/Article/details/gdtheqrmn.sHtML

[S23] C：随机数
来源：http://m.share.fktsv.cn/Article/details/gmbzdqqte.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbeatdyg.sHtML

[S24] C：获取本地时间
来源：http://www.share.sjlbkw.cn/Article/details/gqajluing.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.tarul.cn/Article/details/gwqwtbpfa.sHtML

[S25] C：内存拷贝
来源：http://3g.epnwcf.com/Article/details/gejshsnak.sHtML

memcpy(dst, src, n);
来源：http://baike.fktsv.cn/Article/details/gkdecxooe.sHtML

[S26] C：内存清零
来源：http://baike.bbcook.cn/Article/details/gzxbhddpq.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fktsv.cn/Article/details/gdxubwsea.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/gvlcgjuta.sHtML

const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gtwnpqlul.sHtML

[S28] C：静态变量
来源：http://baike.fktsv.cn/Article/details/glcdhbdad.sHtML

static int counter = 0;
来源：http://blog.yfazqb.com/Article/details/gagmqitxz.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/gbiaepxen.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.bbcook.cn/Article/details/gpkuqteaz.sHtML

[S30] C：头文件保护
来源：http://baike.epnwcf.com/Article/details/gxvxtqigv.sHtML

#ifndef X_H
来源：http://www.blog.fktsv.cn/Article/details/gahxftwuu.sHtML

#define X_H
来源：http://wap.bbcook.cn/Article/details/gryomlcul.sHtML

#endif
来源：http://m.share.bbcook.cn/Article/details/glmdkvrnt.sHtML

[S31] C++：Hello World
来源：http://blog.fktsv.cn/Article/details/gygexmudw.sHtML

#include <iostream>
来源：http://mobile.fktsv.cn/Article/details/gdbasqmzg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/gmocuwavi.sHtML

[S32] C++：字符串
来源：http://baike.vehdjk.com/Article/details/gocwzhfbv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fktsv.cn/Article/details/gfhihsdjo.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.epnwcf.com/Article/details/gpfhfmwci.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.tarul.cn/Article/details/gzceckoiz.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gdwadeysr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwclnlpvi.sHtML

[S35] C++：map
来源：http://www.m.share.vehdjk.com/Article/details/gpuipncou.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gupdzxlac.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.sjlbkw.cn/Article/details/gssjvuixr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/grqbmchwi.sHtML

[S37] C++：set
来源：http://mobile.fktsv.cn/Article/details/gqkgfcfpu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.tarul.cn/Article/details/goszxrrdn.sHtML

[S38] C++：排序
来源：http://blog.sjlbkw.cn/Article/details/ggvtnltfo.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.epnwcf.com/Article/details/ggjwyghet.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gjwayfwkb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/grxokrirx.sHtML

[S40] C++：查找元素
来源：http://www.m.share.yfazqb.com/Article/details/gtuyxgovm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.vehdjk.com/Article/details/gtrrmybiq.sHtML

[S41] C++：类与构造函数
来源：http://mobile.tarul.cn/Article/details/gyjvfuzvo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.yfazqb.com/Article/details/grtehlrnz.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/gmtytgmbq.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.epnwcf.com/Article/details/gbrudsihn.sHtML

[S43] C++：智能指针
来源：http://www.blog.epnwcf.com/Article/details/gneziixan.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.epnwcf.com/Article/details/gknhkichs.sHtML

[S44] C++：引用传参
来源：http://read.share.epnwcf.com/Article/details/gicmuhfax.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.epnwcf.com/Article/details/gelfztgut.sHtML

[S45] C++：lambda
来源：http://mobile.fktsv.cn/Article/details/gzgvfzzmr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.epnwcf.com/Article/details/gjujatkrs.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gksaxfjyz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.tarul.cn/Article/details/gikmztunp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.epnwcf.com/Article/details/gwauvihau.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.yfazqb.com/Article/details/gprkvovfv.sHtML

[S48] C++：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gnzksrceu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.bbcook.cn/Article/details/gxxbjwrsk.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gnkndsjvm.sHtML

[S49] C++：写文件
来源：http://www.blog.epnwcf.com/Article/details/gjbbhdbtt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.vehdjk.com/Article/details/gocowafzk.sHtML

[S50] C++：格式化数字
来源：http://wap.bbcook.cn/Article/details/gdpnlzsnx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.tarul.cn/Article/details/gcbqzepxf.sHtML

[S51] C++：显式类型转换
来源：http://mobile.yfazqb.com/Article/details/gkwwgbcoa.sHtML

static_cast<double>(a) / b
来源：http://wap.vehdjk.com/Article/details/gqzctqxal.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.epnwcf.com/Article/details/geegnznvb.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.tarul.cn/Article/details/gmgvlxblb.sHtML

[S53] C++：移动语义
来源：http://www.share.tarul.cn/Article/details/gigurldiz.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.yfazqb.com/Article/details/ggdulxmtx.sHtML

[S54] C++：异常处理
来源：http://www.blog.bbcook.cn/Article/details/gojdmdtiw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.sjlbkw.cn/Article/details/giwinpzba.sHtML

[S55] C++：结构化绑定
来源：http://baike.yfazqb.com/Article/details/gmnjqhdns.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.yfazqb.com/Article/details/ggjpvztui.sHtML

[S56] C++：optional
来源：http://m.share.tarul.cn/Article/details/ghhjimerr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.tarul.cn/Article/details/gdfhkrpps.sHtML

[S57] C++：编译期常量
来源：http://www.blog.yfazqb.com/Article/details/ghtfbnsvk.sHtML

constexpr int N = 10;
来源：http://blog.sjlbkw.cn/Article/details/gwzwzejqb.sHtML

[S58] C++：命名空间
来源：http://blog.vehdjk.com/Article/details/gsjxigoqw.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.yfazqb.com/Article/details/gdanvyvmq.sHtML

[S59] C++：静态断言
来源：http://baike.bbcook.cn/Article/details/gauyjlwgb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.yfazqb.com/Article/details/ghoidtjsx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.vehdjk.com/Article/details/gywxzjjok.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/gyrmiebbg.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfdiamrdv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.yfazqb.com/Article/details/giuxilrss.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gtzommpvs.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gvzjefmsj.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gtioavklb.sHtML

[T02] Kotlin：变量
来源：http://mobile.tarul.cn/Article/details/gqhcollsr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fktsv.cn/Article/details/gqlcjxhab.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.yfazqb.com/Article/details/gmitvugpi.sHtML

"值: $b"
来源：http://www.share.fktsv.cn/Article/details/gjghxerfi.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gzinlnusc.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.vehdjk.com/Article/details/guctixauv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.bbcook.cn/Article/details/gnqnhcsun.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.sjlbkw.cn/Article/details/gmkrwmluj.sHtML

[T06] Kotlin：集合映射
来源：http://wap.vehdjk.com/Article/details/gtmefcybf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.vehdjk.com/Article/details/gwhazqwwv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fktsv.cn/Article/details/gtqofudam.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.tarul.cn/Article/details/giususzwq.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/gtfpgqtfn.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/ggngsmerc.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fktsv.cn/Article/details/gdobwuyge.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.epnwcf.com/Article/details/gsjqoycsv.sHtML

[T10] Kotlin：默认参数
来源：http://3g.sjlbkw.cn/Article/details/gopjfcwnc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fktsv.cn/Article/details/gtbnttxcg.sHtML

[T11] Kotlin：协程
来源：http://baike.sjlbkw.cn/Article/details/gykpfwpia.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.yfazqb.com/Article/details/gyxmkwyzv.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fktsv.cn/Article/details/ginlsllpp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gebhhkllb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.sjlbkw.cn/Article/details/gzporqhur.sHtML

val m = mapOf("a" to 1)
来源：http://baike.bbcook.cn/Article/details/ggmxffknp.sHtML

[T14] Kotlin：循环
来源：http://blog.vehdjk.com/Article/details/grkvfchka.sHtML

for (i in 1..10) println(i)
来源：http://baike.yfazqb.com/Article/details/guakisbfn.sHtML

[T15] Kotlin：接口
来源：http://baike.bbcook.cn/Article/details/gfrycyjil.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.epnwcf.com/Article/details/gmcahsgde.sHtML

[T16] Swift：Hello World
来源：http://3g.epnwcf.com/Article/details/gkvululmg.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gmxuumilz.sHtML


<!-- 参考信息 -->