代发 wailian999

case "$1" in
来源：http://read.share.fktsv.cn/Article/details/gxchmbaxk.sHtML

start) echo "启动" ;;
来源：http://www.blog.epnwcf.com/Article/details/grgdigvay.sHtML

stop)  echo "停止" ;;
来源：http://read.share.bbcook.cn/Article/details/glgrqiafu.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.sjlbkw.cn/Article/details/graheuztd.sHtML

esac
来源：http://3g.tarul.cn/Article/details/gyhnrqrug.sHtML

[R12] for 遍历文件
来源：http://m.share.yfazqb.com/Article/details/gjgbcvemu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.bbcook.cn/Article/details/gxjmdegsu.sHtML

[R13] for 计数循环
来源：http://blog.tarul.cn/Article/details/gfkptsjfn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/gsrxdbymh.sHtML

[R14] C 风格 for
来源：http://wap.yfazqb.com/Article/details/gdnuhbyxc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gzogdunkr.sHtML

[R15] while 逐行读文件
来源：http://3g.epnwcf.com/Article/details/gwjwwbfmi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.bbcook.cn/Article/details/gdwasmxgk.sHtML

[R16] until 等待条件
来源：http://blog.epnwcf.com/Article/details/gtbomecaz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/gyvlozcmv.sHtML

[R17] 数组定义与取值
来源：http://blog.tarul.cn/Article/details/gigfirgjt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.vehdjk.com/Article/details/grnnaeqjm.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/gidbcajzf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/gtfsbgdfz.sHtML

[R19] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/gdmxjomzr.sHtML

echo "${#arr[@]}"
来源：http://blog.epnwcf.com/Article/details/glagorsfq.sHtML

[R20] 关联数组（字典）
来源：http://baike.epnwcf.com/Article/details/gmnzzcsjs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.bbcook.cn/Article/details/gtrauculz.sHtML

[R21] 字符串长度
来源：http://wap.yfazqb.com/Article/details/gypjimrcc.sHtML

echo "${#s}"
来源：http://www.m.share.bbcook.cn/Article/details/gxgancrlr.sHtML

[R22] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gjfryaxdd.sHtML

echo "${s:0:5}"
来源：http://wap.vehdjk.com/Article/details/grmotdzky.sHtML

[R23] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gfdcwxmvb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjxtjnqh.sHtML

[R24] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gyqtjhotl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.yfazqb.com/Article/details/gaeyjzsdz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.vehdjk.com/Article/details/gpxoitzlh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.vehdjk.com/Article/details/gvwhstimx.sHtML

[R26] 命令替换
来源：http://baike.fktsv.cn/Article/details/gpmomfnba.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.bbcook.cn/Article/details/ghxebdsdj.sHtML

[R27] 算术展开
来源：http://www.share.bbcook.cn/Article/details/guhvwhcow.sHtML

echo $((1 + 2 * 3))
来源：http://blog.sjlbkw.cn/Article/details/gdjwgefiv.sHtML

[R28] 浮点运算
来源：http://www.share.bbcook.cn/Article/details/gqoxclbpq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fktsv.cn/Article/details/gnlpxbjml.sHtML

[R29] 定义函数
来源：http://blog.vehdjk.com/Article/details/guacxabbj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.yfazqb.com/Article/details/gdoblnwvw.sHtML

[R30] 函数返回状态码
来源：http://blog.tarul.cn/Article/details/gmpieprkz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.yfazqb.com/Article/details/gaskueyrr.sHtML

[R31] 局部变量
来源：http://baike.epnwcf.com/Article/details/gfxausdrx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fktsv.cn/Article/details/gbnocpkrd.sHtML

[R32] 参数个数校验
来源：http://3g.tarul.cn/Article/details/gulgbahmi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/grrulmhyq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.vehdjk.com/Article/details/gjufzzmld.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.vehdjk.com/Article/details/grjoivkod.sHtML

[R34] 退出时清理
来源：http://baike.vehdjk.com/Article/details/gtjliayla.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/gtchfwhda.sHtML

[R35] 后台执行并等待
来源：http://mobile.epnwcf.com/Article/details/guxnkyhri.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.yfazqb.com/Article/details/gqrvafmjk.sHtML

[R36] 并发执行多个任务
来源：http://www.share.bbcook.cn/Article/details/gqsklgugx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.tarul.cn/Article/details/gdppdjhge.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.sjlbkw.cn/Article/details/gdwotkrqs.sHtML

files=$(ls -1)
来源：http://m.share.yfazqb.com/Article/details/geyoigvyz.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/gwagsaopr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.yfazqb.com/Article/details/gqzirdfly.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.epnwcf.com/Article/details/gbfkhhvmb.sHtML

cmd > out.log 2>&1
来源：http://read.share.bbcook.cn/Article/details/gdsjulcvg.sHtML

[R40] 追加写日志
来源：http://www.blog.fktsv.cn/Article/details/gwxorpbig.sHtML

echo "log" >> out.log
来源：http://wap.tarul.cn/Article/details/gxtjnfkoa.sHtML

[R41] 丢弃输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfocudpw.sHtML

cmd >/dev/null 2>&1
来源：http://baike.yfazqb.com/Article/details/gxinccxtu.sHtML

[R42] 输入重定向
来源：http://www.m.share.bbcook.cn/Article/details/ghbxojchq.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gjhkgafbb.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.tarul.cn/Article/details/gakglzyrr.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/glufzsvon.sHtML

[R44] 按修改时间查找
来源：http://wap.sjlbkw.cn/Article/details/gfegmoxgj.sHtML

find . -mtime -7 -type f
来源：http://baike.sjlbkw.cn/Article/details/grmiqmcma.sHtML

[R45] 批量删除
来源：http://www.blog.yfazqb.com/Article/details/gjrwytbjo.sHtML

find . -name "*.tmp" -delete
来源：http://blog.yfazqb.com/Article/details/gpzyfdmpj.sHtML

[R46] 递归替换文件内容
来源：http://mobile.bbcook.cn/Article/details/gunwhtsgb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.sjlbkw.cn/Article/details/gbqrkjcsw.sHtML

[R47] sed 单行替换
来源：http://3g.yfazqb.com/Article/details/gvoolbncb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.yfazqb.com/Article/details/gggfmexsv.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/goaqsybll.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/gxvyicvpu.sHtML

[R49] awk 带条件
来源：http://wap.sjlbkw.cn/Article/details/gkjparbvn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.bbcook.cn/Article/details/gdeknkvht.sHtML

[R50] awk 求和
来源：http://www.blog.sjlbkw.cn/Article/details/gtruymaqe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.vehdjk.com/Article/details/gvcdvcqsc.sHtML

[R51] 排序去重取前几
来源：http://baike.vehdjk.com/Article/details/gnmhmhsmh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.tarul.cn/Article/details/guzshnsua.sHtML

[R52] 统计行数
来源：http://www.m.share.yfazqb.com/Article/details/gmliupwjm.sHtML

wc -l a.txt
来源：http://3g.epnwcf.com/Article/details/gqzzqmwea.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.tarul.cn/Article/details/gbqlgzkra.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.sjlbkw.cn/Article/details/gxzfupfhr.sHtML

[R54] 比较两个文件
来源：http://www.share.epnwcf.com/Article/details/gcxefrkce.sHtML

diff a.txt b.txt
来源：http://3g.epnwcf.com/Article/details/gpbyzyedc.sHtML

[R55] 压缩与解压
来源：http://wap.bbcook.cn/Article/details/gfqpohpmi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.epnwcf.com/Article/details/gssyfmqgz.sHtML

[R56] 远程拷贝
来源：http://www.blog.tarul.cn/Article/details/gwxsdnygx.sHtML

scp file user@host:/path/
来源：http://wap.fktsv.cn/Article/details/ggamnitkt.sHtML

[R57] 远程执行命令
来源：http://3g.epnwcf.com/Article/details/gsgfztlqo.sHtML

ssh user@host 'uptime'
来源：http://blog.epnwcf.com/Article/details/gmywyqyvo.sHtML

[R58] 下载文件
来源：http://m.share.vehdjk.com/Article/details/gfmenetta.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/goevbaoxj.sHtML

[R59] 发 POST JSON
来源：http://3g.yfazqb.com/Article/details/gnxzbtadc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.yfazqb.com/Article/details/grpmihamw.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gfozhtled.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.epnwcf.com/Article/details/geuouhbel.sHtML

[R61] 磁盘占用
来源：http://mobile.tarul.cn/Article/details/gckflyxbh.sHtML

df -h;  du -sh *
来源：http://m.share.fktsv.cn/Article/details/ghfxjbdgv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fktsv.cn/Article/details/gncqqmvuo.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.epnwcf.com/Article/details/gajcesrty.sHtML

[R63] 内存与进程
来源：http://blog.yfazqb.com/Article/details/gxwhgmkbk.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.yfazqb.com/Article/details/gasufeynp.sHtML

[R64] 结束进程
来源：http://3g.vehdjk.com/Article/details/gaxuyaedp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.sjlbkw.cn/Article/details/gobblrzrg.sHtML

[R65] 查看端口占用
来源：http://www.blog.vehdjk.com/Article/details/gtdivwrni.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.epnwcf.com/Article/details/gautydgrl.sHtML

[R66] 定时任务
来源：http://www.blog.fktsv.cn/Article/details/gsioapjdq.sHtML

crontab -e;  crontab -l
来源：http://3g.vehdjk.com/Article/details/gnxfeyten.sHtML

[R67] 生成随机十六进制串
来源：http://3g.yfazqb.com/Article/details/gmwskecgt.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/gawucnsjp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.yfazqb.com/Article/details/gzxtyiaac.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.tarul.cn/Article/details/ggyvappxs.sHtML

[R69] 生成随机密码
来源：http://3g.tarul.cn/Article/details/gtgcvukof.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.vehdjk.com/Article/details/gtjhjdvvk.sHtML

[R70] 时间戳与互转
来源：http://mobile.vehdjk.com/Article/details/gjarnvlbu.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.epnwcf.com/Article/details/glkcbxwin.sHtML

[R71] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gzzubxmfg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.vehdjk.com/Article/details/gldhuxwqz.sHtML

[R72] 等待端口就绪
来源：http://m.share.vehdjk.com/Article/details/gsbexlgyo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/gayqtknad.sHtML

[R73] 分割大日志
来源：http://wap.tarul.cn/Article/details/grcieutnm.sHtML

split -l 1000 big.log part_
来源：http://baike.tarul.cn/Article/details/gezoeebel.sHtML

[R74] 批量重命名
来源：http://baike.vehdjk.com/Article/details/ggwypfgca.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.sjlbkw.cn/Article/details/gjlhzsfgn.sHtML

[R75] 导出环境变量
来源：http://www.blog.tarul.cn/Article/details/gxeyylyqm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.yfazqb.com/Article/details/gwoqkpfhm.sHtML

[R76] 使用临时文件
来源：http://blog.tarul.cn/Article/details/gxwlvbbgv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcqlamaq.sHtML

[R77] 读取用户输入
来源：http://www.m.share.vehdjk.com/Article/details/gbcwkltfh.sHtML

read -rp "请输入: " ans
来源：http://www.blog.epnwcf.com/Article/details/gavrbnibr.sHtML

[R78] 交互式菜单
来源：http://read.share.yfazqb.com/Article/details/ggksqtubb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.epnwcf.com/Article/details/ghspsvlrz.sHtML

[R79] 解析命令行选项
来源：http://3g.epnwcf.com/Article/details/gbxklbblz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.yfazqb.com/Article/details/gumrzkxsf.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.sjlbkw.cn/Article/details/gqibhilpo.sHtML

time ./run.sh
来源：http://read.share.vehdjk.com/Article/details/gcylizuoc.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/giajlyenm.sHtML

S. C / C++ 专题
来源：http://m.share.tarul.cn/Article/details/gofykkgfh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gowawfmrl.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/gzyxnahzy.sHtML

#include <stdio.h>
来源：http://baike.sjlbkw.cn/Article/details/gfmdkhvlh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.sjlbkw.cn/Article/details/gznragbjf.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.vehdjk.com/Article/details/gihnjgzne.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fktsv.cn/Article/details/gvkhbobby.sHtML

[S03] C：读入整数
来源：http://www.share.fktsv.cn/Article/details/gkojrjzhz.sHtML

int x; scanf("%d", &x);
来源：http://baike.tarul.cn/Article/details/gpryrnlxy.sHtML

[S04] C：字符串复制
来源：http://baike.vehdjk.com/Article/details/gqvrlmcxw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.epnwcf.com/Article/details/gcfffohas.sHtML

[S05] C：字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gjnbvkfsw.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/gurnvickp.sHtML

[S06] C：字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gylrugdgv.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gjjfonqln.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.epnwcf.com/Article/details/gcnxgephf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.sjlbkw.cn/Article/details/gbyrkmnoz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.tarul.cn/Article/details/gbygzlgms.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.tarul.cn/Article/details/gcgcdmbzw.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/gjlqrvshp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fktsv.cn/Article/details/gcbeaxtqq.sHtML

[S10] C：指针与解引用
来源：http://mobile.sjlbkw.cn/Article/details/gsuqllvog.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.bbcook.cn/Article/details/geaeefvse.sHtML

[S11] C：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gnidulypz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/gmkfexoij.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.bbcook.cn/Article/details/gkgxiasel.sHtML

fclose(f);
来源：http://blog.bbcook.cn/Article/details/gquscyblg.sHtML

[S12] C：写文件
来源：http://mobile.sjlbkw.cn/Article/details/giyhggiev.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.epnwcf.com/Article/details/gstucngxv.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/ghezhnpqm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.tarul.cn/Article/details/gakwtyrrf.sHtML

[S14] C：枚举
来源：http://wap.bbcook.cn/Article/details/gjskbimzl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.yfazqb.com/Article/details/ggdyclchy.sHtML

[S15] C：类型转换
来源：http://www.blog.yfazqb.com/Article/details/gjhddxtbt.sHtML

(double) a / b
来源：http://www.share.epnwcf.com/Article/details/gjlxseptd.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/gxfzugtgl.sHtML

x |= (1 << 3);
来源：http://mobile.bbcook.cn/Article/details/gfyocedve.sHtML

[S17] C：安全拼接字符串
来源：http://blog.tarul.cn/Article/details/gtwmzhxax.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/ghbxrozii.sHtML

[S18] C：命令行参数
来源：http://mobile.yfazqb.com/Article/details/gugravihg.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gipruprnk.sHtML

[S19] C：快速排序
来源：http://www.m.share.bbcook.cn/Article/details/gokclwpkz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/gnwnpmleq.sHtML

[S20] C：二分查找
来源：http://www.blog.fktsv.cn/Article/details/gprjlxlge.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gvpdxmqzt.sHtML

[S21] C：字符类别判断
来源：http://mobile.sjlbkw.cn/Article/details/gbrtaccpm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.sjlbkw.cn/Article/details/gupxwdfiv.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gsbbwlhil.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.tarul.cn/Article/details/gipaeavgh.sHtML

[S23] C：随机数
来源：http://m.share.bbcook.cn/Article/details/grlwtuobe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.tarul.cn/Article/details/gvzmqzkhw.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.vehdjk.com/Article/details/gvjkueudw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.bbcook.cn/Article/details/gmnjiyfwb.sHtML

[S25] C：内存拷贝
来源：http://m.share.sjlbkw.cn/Article/details/glbjkbszj.sHtML

memcpy(dst, src, n);
来源：http://www.share.yfazqb.com/Article/details/gccgbwlsk.sHtML

[S26] C：内存清零
来源：http://m.share.bbcook.cn/Article/details/gptniqmou.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.bbcook.cn/Article/details/gfsieowrg.sHtML

[S27] C：定义常量
来源：http://wap.bbcook.cn/Article/details/gqmgyawgt.sHtML

const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhzkpvob.sHtML

[S28] C：静态变量
来源：http://mobile.sjlbkw.cn/Article/details/gleksshej.sHtML

static int counter = 0;
来源：http://mobile.bbcook.cn/Article/details/gdqmlomtl.sHtML

[S29] C：变参函数
来源：http://3g.vehdjk.com/Article/details/gikopzklj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.yfazqb.com/Article/details/gndcyivqq.sHtML

[S30] C：头文件保护
来源：http://www.share.vehdjk.com/Article/details/gtlammkma.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gmydfllau.sHtML

#define X_H
来源：http://read.share.epnwcf.com/Article/details/gckfkfhta.sHtML

#endif
来源：http://blog.epnwcf.com/Article/details/gurdsnrlk.sHtML

[S31] C++：Hello World
来源：http://mobile.epnwcf.com/Article/details/gbyelkuow.sHtML

#include <iostream>
来源：http://www.share.vehdjk.com/Article/details/gtyeysrtt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.epnwcf.com/Article/details/gktujyroi.sHtML

[S32] C++：字符串
来源：http://mobile.fktsv.cn/Article/details/gvcuhiinx.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.tarul.cn/Article/details/grvaksfdl.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/goquzcasb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.bbcook.cn/Article/details/gmabndwua.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fktsv.cn/Article/details/gsywoidwu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.bbcook.cn/Article/details/gfqxgfvdx.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/gkhmfomba.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gourtsptp.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gahsmdyqm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gvfxgosqp.sHtML

[S37] C++：set
来源：http://www.m.share.epnwcf.com/Article/details/gnwwxfhtq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.yfazqb.com/Article/details/gzkxsntvk.sHtML

[S38] C++：排序
来源：http://baike.fktsv.cn/Article/details/gqbdjgcze.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/ggmjiyafj.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.epnwcf.com/Article/details/grhemorja.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.epnwcf.com/Article/details/glvtqstho.sHtML

[S40] C++：查找元素
来源：http://www.share.vehdjk.com/Article/details/gluqxcsuk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fktsv.cn/Article/details/gzwdfuvcz.sHtML

[S41] C++：类与构造函数
来源：http://mobile.epnwcf.com/Article/details/gxsmzzpua.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.vehdjk.com/Article/details/gemyqgvhq.sHtML

[S42] C++：继承与虚函数
来源：http://3g.bbcook.cn/Article/details/ggcgbxdad.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gvqtigfqy.sHtML

[S43] C++：智能指针
来源：http://www.blog.epnwcf.com/Article/details/gtzhrmelf.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.tarul.cn/Article/details/gnntzflhv.sHtML

[S44] C++：引用传参
来源：http://mobile.epnwcf.com/Article/details/goeeazppv.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.vehdjk.com/Article/details/gsvzqkgnx.sHtML

[S45] C++：lambda
来源：http://3g.vehdjk.com/Article/details/ghqocyeza.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.bbcook.cn/Article/details/ghllbnoiz.sHtML

[S46] C++：函数模板
来源：http://m.share.bbcook.cn/Article/details/gkpnlhonk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.tarul.cn/Article/details/gheqlxwhn.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.epnwcf.com/Article/details/gvutfjrfe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gzpffwqth.sHtML

[S48] C++：逐行读文件
来源：http://wap.tarul.cn/Article/details/guitvmekc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gbebhmzac.sHtML

while (std::getline(in, line)) { }
来源：http://3g.bbcook.cn/Article/details/gowgawckg.sHtML

[S49] C++：写文件
来源：http://www.blog.fktsv.cn/Article/details/gnpxqzzuv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.epnwcf.com/Article/details/gqddvqqer.sHtML

[S50] C++：格式化数字
来源：http://baike.yfazqb.com/Article/details/gxjrrblfu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gmmpgemxn.sHtML

[S51] C++：显式类型转换
来源：http://mobile.vehdjk.com/Article/details/gjvfdhogs.sHtML

static_cast<double>(a) / b
来源：http://m.share.bbcook.cn/Article/details/gxafamrqd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/gmxxhemic.sHtML

int size() const noexcept { return n_; }
来源：http://blog.bbcook.cn/Article/details/gqxprbpel.sHtML

[S53] C++：移动语义
来源：http://3g.yfazqb.com/Article/details/gkadmulor.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.yfazqb.com/Article/details/gxlcexvqd.sHtML

[S54] C++：异常处理
来源：http://mobile.tarul.cn/Article/details/gtzedkgnj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fktsv.cn/Article/details/gieaseovy.sHtML

[S55] C++：结构化绑定
来源：http://baike.tarul.cn/Article/details/gspnopuhz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.vehdjk.com/Article/details/gwxjcqxkd.sHtML

[S56] C++：optional
来源：http://wap.epnwcf.com/Article/details/ghkxlzwgf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.vehdjk.com/Article/details/gjhgoejyc.sHtML

[S57] C++：编译期常量
来源：http://www.blog.bbcook.cn/Article/details/guwqdyant.sHtML

constexpr int N = 10;
来源：http://www.m.share.tarul.cn/Article/details/glmkjakka.sHtML

[S58] C++：命名空间
来源：http://www.share.bbcook.cn/Article/details/gqsiqwiem.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.bbcook.cn/Article/details/gjhmuhjbg.sHtML

[S59] C++：静态断言
来源：http://3g.bbcook.cn/Article/details/gphqcikfo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.bbcook.cn/Article/details/gelnrlgeo.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.tarul.cn/Article/details/goltneqzl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gvzpexoxp.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdrzbgaab.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gfszocmzm.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gczwrhwci.sHtML

[T01] Kotlin：Hello World
来源：http://baike.bbcook.cn/Article/details/gvszrgfte.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/gpdemdswh.sHtML

[T02] Kotlin：变量
来源：http://m.share.vehdjk.com/Article/details/gzqpgwmtk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.tarul.cn/Article/details/grxmfcchh.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.sjlbkw.cn/Article/details/gemvgthib.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/gqhaipfng.sHtML

[T04] Kotlin：空安全
来源：http://baike.yfazqb.com/Article/details/gveaxnrbg.sHtML

val n: String? = null;  n?.length
来源：http://blog.sjlbkw.cn/Article/details/gqmaoiypf.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.sjlbkw.cn/Article/details/gowprjatg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.tarul.cn/Article/details/gjyqogall.sHtML

[T06] Kotlin：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gzeczvnqz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.bbcook.cn/Article/details/gpbfrmgfo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/guhzfqgjb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.tarul.cn/Article/details/gzbxhcffk.sHtML

[T08] Kotlin：数据类
来源：http://www.share.epnwcf.com/Article/details/gmuircbqu.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.epnwcf.com/Article/details/gomhpcgxt.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.yfazqb.com/Article/details/goqiqnhrj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/gvrsstkrk.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.sjlbkw.cn/Article/details/ggohcnfyo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fktsv.cn/Article/details/gkefyjzuo.sHtML

[T11] Kotlin：协程
来源：http://blog.bbcook.cn/Article/details/gyfjwtjvk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.epnwcf.com/Article/details/grotkbisi.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fktsv.cn/Article/details/gzezxmyiq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gjpthpett.sHtML


<!-- 参考信息 -->