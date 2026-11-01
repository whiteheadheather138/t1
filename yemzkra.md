代发 wailian999

case "$1" in
来源：http://read.share.yfazqb.com/Article/details/gogcbczcr.sHtML

start) echo "启动" ;;
来源：http://m.share.bbcook.cn/Article/details/gxbvdsbek.sHtML

stop)  echo "停止" ;;
来源：http://3g.vehdjk.com/Article/details/gdrtetddr.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gezzyydhn.sHtML

esac
来源：http://www.blog.tarul.cn/Article/details/gchqycdxc.sHtML

[R12] for 遍历文件
来源：http://blog.epnwcf.com/Article/details/ghebbdjjq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/ggvmtxfyt.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gqlbbjltc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gcrgqgejp.sHtML

[R14] C 风格 for
来源：http://www.share.yfazqb.com/Article/details/gaaqwlhhe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gzruzdsul.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gxjxasktf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.tarul.cn/Article/details/gakqgwojg.sHtML

[R16] until 等待条件
来源：http://wap.vehdjk.com/Article/details/gdfdmwaje.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gepsxuory.sHtML

[R17] 数组定义与取值
来源：http://blog.tarul.cn/Article/details/giklmramu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.yfazqb.com/Article/details/gnxtigmwl.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/geknvmfxh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.sjlbkw.cn/Article/details/gbpsvzyvi.sHtML

[R19] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gmrnpcmww.sHtML

echo "${#arr[@]}"
来源：http://m.share.vehdjk.com/Article/details/gwwmnrrhq.sHtML

[R20] 关联数组（字典）
来源：http://blog.fktsv.cn/Article/details/gkmmboral.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.tarul.cn/Article/details/grevcuwfe.sHtML

[R21] 字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gagcnsfiq.sHtML

echo "${#s}"
来源：http://read.share.tarul.cn/Article/details/gmpmmwrfg.sHtML

[R22] 截取子串
来源：http://mobile.tarul.cn/Article/details/gyynicxwd.sHtML

echo "${s:0:5}"
来源：http://baike.sjlbkw.cn/Article/details/gsjacpghv.sHtML

[R23] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gqfcexbai.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.vehdjk.com/Article/details/guujvtnhc.sHtML

[R24] 大小写转换
来源：http://read.share.tarul.cn/Article/details/grrzczgms.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.bbcook.cn/Article/details/gxlnpljxz.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.vehdjk.com/Article/details/gtkmvvrqa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.epnwcf.com/Article/details/gejggxguf.sHtML

[R26] 命令替换
来源：http://baike.epnwcf.com/Article/details/gdeeykuna.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.bbcook.cn/Article/details/gdyrjdexk.sHtML

[R27] 算术展开
来源：http://wap.bbcook.cn/Article/details/gszklsltn.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.tarul.cn/Article/details/ggldqguuo.sHtML

[R28] 浮点运算
来源：http://blog.sjlbkw.cn/Article/details/ggomokbvc.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.yfazqb.com/Article/details/gwvpfouwl.sHtML

[R29] 定义函数
来源：http://mobile.bbcook.cn/Article/details/gykfytgtw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.yfazqb.com/Article/details/gjjgdejjo.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fktsv.cn/Article/details/gxudapwfp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fktsv.cn/Article/details/gcejwwinm.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gyabdzilb.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.vehdjk.com/Article/details/gbbzlhaeu.sHtML

[R32] 参数个数校验
来源：http://read.share.bbcook.cn/Article/details/glpcuufjx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/geqaaozum.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/gdwlvtivo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fktsv.cn/Article/details/gnwsggawl.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/gudznfohh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gnvcibsso.sHtML

[R35] 后台执行并等待
来源：http://wap.bbcook.cn/Article/details/gdrnckxxo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.yfazqb.com/Article/details/gghtjoqib.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.bbcook.cn/Article/details/glzakabba.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.bbcook.cn/Article/details/gxkbjbqyf.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/gflsmcssa.sHtML

files=$(ls -1)
来源：http://www.blog.vehdjk.com/Article/details/gpnclvrvd.sHtML

[R38] 管道串联
来源：http://3g.fktsv.cn/Article/details/gsrnsdrnz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fktsv.cn/Article/details/geqlmamnt.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/gxzeifgyr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/gxsomdmjy.sHtML

[R40] 追加写日志
来源：http://m.share.vehdjk.com/Article/details/gvwuqccvh.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/gceffktqc.sHtML

[R41] 丢弃输出
来源：http://wap.tarul.cn/Article/details/gigvbbfcb.sHtML

cmd >/dev/null 2>&1
来源：http://baike.tarul.cn/Article/details/ghbiaqokr.sHtML

[R42] 输入重定向
来源：http://mobile.tarul.cn/Article/details/gmsniadqt.sHtML

wc -l < a.txt
来源：http://m.share.fktsv.cn/Article/details/gfptvlnmz.sHtML

[R43] 按名字查找文件
来源：http://3g.sjlbkw.cn/Article/details/gnvybgqml.sHtML

find . -name "*.log" -type f
来源：http://www.blog.epnwcf.com/Article/details/gtwokqwng.sHtML

[R44] 按修改时间查找
来源：http://www.blog.vehdjk.com/Article/details/gndqofxxq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.yfazqb.com/Article/details/glrsxjngw.sHtML

[R45] 批量删除
来源：http://3g.tarul.cn/Article/details/gnjvjiivw.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fktsv.cn/Article/details/gzczsmlhb.sHtML

[R46] 递归替换文件内容
来源：http://www.share.bbcook.cn/Article/details/gxsulhxvl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.tarul.cn/Article/details/ghdjkuhwc.sHtML

[R47] sed 单行替换
来源：http://3g.vehdjk.com/Article/details/grzelfxfz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.vehdjk.com/Article/details/gxrcigicp.sHtML

[R48] awk 取指定列
来源：http://baike.fktsv.cn/Article/details/grpcbrrdo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gqdwzqjte.sHtML

[R49] awk 带条件
来源：http://3g.sjlbkw.cn/Article/details/gohbjonca.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/gfyhzpjcv.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/gkevirmov.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.tarul.cn/Article/details/giixhkpzy.sHtML

[R51] 排序去重取前几
来源：http://mobile.fktsv.cn/Article/details/gasczlftq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.sjlbkw.cn/Article/details/grqikhame.sHtML

[R52] 统计行数
来源：http://www.share.yfazqb.com/Article/details/gsvocieum.sHtML

wc -l a.txt
来源：http://www.share.fktsv.cn/Article/details/ggsroiqtc.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.tarul.cn/Article/details/gxqvjrook.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.tarul.cn/Article/details/gylbvlydl.sHtML

[R54] 比较两个文件
来源：http://blog.fktsv.cn/Article/details/gjnilxapi.sHtML

diff a.txt b.txt
来源：http://www.blog.epnwcf.com/Article/details/gqufcwbyu.sHtML

[R55] 压缩与解压
来源：http://wap.fktsv.cn/Article/details/gxtohjoiy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.bbcook.cn/Article/details/gshuoxkhn.sHtML

[R56] 远程拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gmgsewgoa.sHtML

scp file user@host:/path/
来源：http://baike.fktsv.cn/Article/details/gooimlpzl.sHtML

[R57] 远程执行命令
来源：http://3g.fktsv.cn/Article/details/gxerggimm.sHtML

ssh user@host 'uptime'
来源：http://wap.epnwcf.com/Article/details/gvwvhlytb.sHtML

[R58] 下载文件
来源：http://www.blog.tarul.cn/Article/details/gpgafqsdz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fktsv.cn/Article/details/gtiytstfh.sHtML

[R59] 发 POST JSON
来源：http://blog.tarul.cn/Article/details/gvfguyklh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.sjlbkw.cn/Article/details/grtaquuof.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/ggkdknbpw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.yfazqb.com/Article/details/gxasaeqec.sHtML

[R61] 磁盘占用
来源：http://wap.bbcook.cn/Article/details/gcckznacy.sHtML

df -h;  du -sh *
来源：http://3g.yfazqb.com/Article/details/gnlkconwe.sHtML

[R62] 找最占空间的文件
来源：http://3g.yfazqb.com/Article/details/gkjtbxvyk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.tarul.cn/Article/details/gazkhpkmp.sHtML

[R63] 内存与进程
来源：http://3g.epnwcf.com/Article/details/gzwtzrgab.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.sjlbkw.cn/Article/details/gqtnftbzh.sHtML

[R64] 结束进程
来源：http://blog.yfazqb.com/Article/details/giyuixyty.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.bbcook.cn/Article/details/gxhirfhla.sHtML

[R65] 查看端口占用
来源：http://m.share.sjlbkw.cn/Article/details/gjmeemiej.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.bbcook.cn/Article/details/gupgikxus.sHtML

[R66] 定时任务
来源：http://www.share.yfazqb.com/Article/details/gelhidhas.sHtML

crontab -e;  crontab -l
来源：http://wap.tarul.cn/Article/details/gbvsfgfcs.sHtML

[R67] 生成随机十六进制串
来源：http://3g.vehdjk.com/Article/details/gymmpsbcz.sHtML

openssl rand -hex 16
来源：http://3g.bbcook.cn/Article/details/gfpvrryna.sHtML

[R68] 计算文件校验值
来源：http://mobile.vehdjk.com/Article/details/gsndizyea.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.bbcook.cn/Article/details/geuhwytkh.sHtML

[R69] 生成随机密码
来源：http://baike.tarul.cn/Article/details/glliduudb.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fktsv.cn/Article/details/gkqijodup.sHtML

[R70] 时间戳与互转
来源：http://m.share.vehdjk.com/Article/details/grkvauzdz.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fktsv.cn/Article/details/giwybamcs.sHtML

[R71] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gihcztpfr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.bbcook.cn/Article/details/gvfhhtgfs.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnlrrhnx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gvwkserlj.sHtML

[R73] 分割大日志
来源：http://mobile.tarul.cn/Article/details/gnqguupot.sHtML

split -l 1000 big.log part_
来源：http://m.share.sjlbkw.cn/Article/details/gmebomzrj.sHtML

[R74] 批量重命名
来源：http://blog.yfazqb.com/Article/details/gwdqfqern.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.sjlbkw.cn/Article/details/gqnunwpjv.sHtML

[R75] 导出环境变量
来源：http://baike.tarul.cn/Article/details/grkgajmgn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.sjlbkw.cn/Article/details/gyvgqhkgu.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/gdnsbnxag.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gboglqgmp.sHtML

[R77] 读取用户输入
来源：http://www.share.tarul.cn/Article/details/gsmktyilk.sHtML

read -rp "请输入: " ans
来源：http://www.share.tarul.cn/Article/details/gqhclqazf.sHtML

[R78] 交互式菜单
来源：http://read.share.tarul.cn/Article/details/gceyidpsa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.epnwcf.com/Article/details/gajbltxyq.sHtML

[R79] 解析命令行选项
来源：http://3g.vehdjk.com/Article/details/glybswddq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.bbcook.cn/Article/details/gkxndwlzg.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fktsv.cn/Article/details/gjpagermp.sHtML

time ./run.sh
来源：http://www.blog.vehdjk.com/Article/details/gyiooptbp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gdukcveem.sHtML

S. C / C++ 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gybaugfxj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/giepnndxq.sHtML

[S01] C：Hello World
来源：http://baike.tarul.cn/Article/details/ggogweizk.sHtML

#include <stdio.h>
来源：http://read.share.tarul.cn/Article/details/gzqdtorie.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.tarul.cn/Article/details/geycuslgi.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.tarul.cn/Article/details/gmzvfgkky.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fktsv.cn/Article/details/gacltqhjg.sHtML

[S03] C：读入整数
来源：http://wap.epnwcf.com/Article/details/gmbdtzbgu.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.vehdjk.com/Article/details/gdubwenks.sHtML

[S04] C：字符串复制
来源：http://www.blog.epnwcf.com/Article/details/gtwmzuyon.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.vehdjk.com/Article/details/gghaahvdi.sHtML

[S05] C：字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gltlddqvl.sHtML

strlen(s)
来源：http://www.blog.epnwcf.com/Article/details/gyxkzqxhx.sHtML

[S06] C：字符串比较
来源：http://baike.vehdjk.com/Article/details/gupyqjxqk.sHtML

strcmp(a, b) == 0
来源：http://www.share.tarul.cn/Article/details/giikzikxg.sHtML

[S07] C：数组遍历求和
来源：http://www.share.yfazqb.com/Article/details/gckvhpzbo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.epnwcf.com/Article/details/gehinsadj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.vehdjk.com/Article/details/gettdrfor.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.tarul.cn/Article/details/gomjvrmse.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.yfazqb.com/Article/details/ghxbsgnvp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.tarul.cn/Article/details/gfsvxjuop.sHtML

[S10] C：指针与解引用
来源：http://mobile.epnwcf.com/Article/details/gmefgwtpp.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.sjlbkw.cn/Article/details/gvrvfjffn.sHtML

[S11] C：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gbinmhmak.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/gnihvygtg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.tarul.cn/Article/details/gsbnvsocd.sHtML

fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gcvokpnju.sHtML

[S12] C：写文件
来源：http://mobile.epnwcf.com/Article/details/ggkahsvve.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.vehdjk.com/Article/details/ghqzbdmeo.sHtML

[S13] C：宏定义
来源：http://www.m.share.fktsv.cn/Article/details/gfxafkblc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fktsv.cn/Article/details/glwmdiqpz.sHtML

[S14] C：枚举
来源：http://m.share.vehdjk.com/Article/details/gctdufwuk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.epnwcf.com/Article/details/gjobeocxm.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/grfxyaukj.sHtML

(double) a / b
来源：http://3g.tarul.cn/Article/details/gruwrabrf.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/gjcgmllop.sHtML

x |= (1 << 3);
来源：http://read.share.tarul.cn/Article/details/gfnlruxze.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gezffnlau.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.bbcook.cn/Article/details/gykvsnxav.sHtML

[S18] C：命令行参数
来源：http://www.share.yfazqb.com/Article/details/gchccirlj.sHtML

int main(int argc, char **argv)
来源：http://mobile.bbcook.cn/Article/details/gqepsltaq.sHtML

[S19] C：快速排序
来源：http://mobile.epnwcf.com/Article/details/gwpwfpmkz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gvcdgupqc.sHtML

[S20] C：二分查找
来源：http://www.m.share.vehdjk.com/Article/details/ghtdcfaho.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/gauvhxqgu.sHtML

[S21] C：字符类别判断
来源：http://mobile.vehdjk.com/Article/details/grnqdblzj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/gwvtqsvpm.sHtML

[S22] C：字符串转数字
来源：http://read.share.sjlbkw.cn/Article/details/gsceqauyy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.epnwcf.com/Article/details/gzljqyayk.sHtML

[S23] C：随机数
来源：http://mobile.sjlbkw.cn/Article/details/gfrupmdee.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.bbcook.cn/Article/details/genqjlprn.sHtML

[S24] C：获取本地时间
来源：http://blog.fktsv.cn/Article/details/gnqqxnova.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.yfazqb.com/Article/details/gycilxwfl.sHtML

[S25] C：内存拷贝
来源：http://wap.sjlbkw.cn/Article/details/gxekbamdt.sHtML

memcpy(dst, src, n);
来源：http://www.blog.yfazqb.com/Article/details/gbxnofemi.sHtML

[S26] C：内存清零
来源：http://wap.vehdjk.com/Article/details/ghjynpnat.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/girlyyflk.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/gnfpnhupa.sHtML

const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gyuuncgei.sHtML

[S28] C：静态变量
来源：http://www.share.epnwcf.com/Article/details/gzxxpflmo.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/geqpybubv.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/glguxvefs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.yfazqb.com/Article/details/gqboklgbu.sHtML

[S30] C：头文件保护
来源：http://www.share.epnwcf.com/Article/details/glrjnhoml.sHtML

#ifndef X_H
来源：http://blog.sjlbkw.cn/Article/details/gqeslfyal.sHtML

#define X_H
来源：http://www.m.share.epnwcf.com/Article/details/gtqwrezvh.sHtML

#endif
来源：http://3g.tarul.cn/Article/details/gvahugjmm.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gzygjnamk.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/gdsgytnnx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.yfazqb.com/Article/details/ginbjwobz.sHtML

[S32] C++：字符串
来源：http://3g.vehdjk.com/Article/details/glchehgfu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.bbcook.cn/Article/details/gtcxrbfsi.sHtML

[S33] C++：vector 增删
来源：http://read.share.tarul.cn/Article/details/gzgizhrlm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fktsv.cn/Article/details/gusodumae.sHtML

[S34] C++：遍历 vector
来源：http://www.share.bbcook.cn/Article/details/gouabqtdu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fktsv.cn/Article/details/gvkedfgwo.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/glskfjhng.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gsfxjqgra.sHtML

[S36] C++：unordered_map
来源：http://3g.tarul.cn/Article/details/gzzhuzwfe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gjfqyitry.sHtML

[S37] C++：set
来源：http://wap.fktsv.cn/Article/details/guqvznxaf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.bbcook.cn/Article/details/gujsusmfb.sHtML

[S38] C++：排序
来源：http://m.share.sjlbkw.cn/Article/details/gviprfpbv.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.vehdjk.com/Article/details/grgpxvmtt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.tarul.cn/Article/details/gidfoautb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/gcebubjxk.sHtML

[S40] C++：查找元素
来源：http://m.share.bbcook.cn/Article/details/ghvpqzmfi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.yfazqb.com/Article/details/gpxnssoac.sHtML

[S41] C++：类与构造函数
来源：http://mobile.epnwcf.com/Article/details/gexrsdguu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.yfazqb.com/Article/details/gjdkyxvzh.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/gknhsvqev.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.sjlbkw.cn/Article/details/gapdbdrfz.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/ghpmxruwa.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gwjheleok.sHtML

[S44] C++：引用传参
来源：http://baike.sjlbkw.cn/Article/details/gplqprqsc.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.yfazqb.com/Article/details/gdthdnskm.sHtML

[S45] C++：lambda
来源：http://www.share.fktsv.cn/Article/details/ghlkptfcc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.bbcook.cn/Article/details/gorgexbdq.sHtML

[S46] C++：函数模板
来源：http://www.blog.vehdjk.com/Article/details/guywydcnu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.epnwcf.com/Article/details/gbrieacpo.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fktsv.cn/Article/details/gattbhnxl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.sjlbkw.cn/Article/details/gguxpvkkf.sHtML

[S48] C++：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gwvcqccro.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.vehdjk.com/Article/details/gysgnptsi.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.sjlbkw.cn/Article/details/giacwdiov.sHtML

[S49] C++：写文件
来源：http://www.blog.fktsv.cn/Article/details/gsezbdeyw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.yfazqb.com/Article/details/gkobeblcw.sHtML

[S50] C++：格式化数字
来源：http://mobile.yfazqb.com/Article/details/ggorxrart.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/gfqbcluwi.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gtnojgcmn.sHtML

static_cast<double>(a) / b
来源：http://m.share.sjlbkw.cn/Article/details/gqkijqjdg.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.tarul.cn/Article/details/gpdyaoicf.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.sjlbkw.cn/Article/details/gtbiosnej.sHtML

[S53] C++：移动语义
来源：http://www.share.yfazqb.com/Article/details/gbqypvrdy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.yfazqb.com/Article/details/gtsqtwvbf.sHtML

[S54] C++：异常处理
来源：http://wap.sjlbkw.cn/Article/details/gqasrxxlq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.epnwcf.com/Article/details/grmirhrjw.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/gzvshtlxa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.bbcook.cn/Article/details/gxfwdquhn.sHtML

[S56] C++：optional
来源：http://wap.vehdjk.com/Article/details/gvyuwevbr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.bbcook.cn/Article/details/gcdadmoiz.sHtML

[S57] C++：编译期常量
来源：http://www.blog.bbcook.cn/Article/details/gyapgnhbk.sHtML

constexpr int N = 10;
来源：http://blog.vehdjk.com/Article/details/gigrwapiy.sHtML

[S58] C++：命名空间
来源：http://wap.yfazqb.com/Article/details/gdoinmhgc.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.yfazqb.com/Article/details/gxnqqdrsk.sHtML

[S59] C++：静态断言
来源：http://www.m.share.tarul.cn/Article/details/gsxdzaimx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.yfazqb.com/Article/details/gmhghzglv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fktsv.cn/Article/details/gwcavuivo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.yfazqb.com/Article/details/glyexpvpa.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gapmcgukv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.epnwcf.com/Article/details/ghqhxginu.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gfruhfrdl.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gbkplvtky.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gtfnhcsnp.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gahjokxnu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.sjlbkw.cn/Article/details/gdakzofkm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.bbcook.cn/Article/details/gheinlqje.sHtML

"值: $b"
来源：http://3g.fktsv.cn/Article/details/gnfcuxerq.sHtML

[T04] Kotlin：空安全
来源：http://m.share.epnwcf.com/Article/details/gofgxdnxx.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.bbcook.cn/Article/details/gxxbkicoc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fktsv.cn/Article/details/gkmbugryb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.bbcook.cn/Article/details/gxcjzckor.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/guedybdxd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gojthgdkq.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.bbcook.cn/Article/details/gpdqhutcu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.vehdjk.com/Article/details/gwjdaslht.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fktsv.cn/Article/details/glpbajled.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.vehdjk.com/Article/details/gubwuiyro.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.vehdjk.com/Article/details/grzptjqml.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/gyihvqdpg.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gmlkbkgoi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.vehdjk.com/Article/details/gaipkvjtd.sHtML

[T11] Kotlin：协程
来源：http://3g.tarul.cn/Article/details/goosrinjh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.sjlbkw.cn/Article/details/grsrlzien.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.sjlbkw.cn/Article/details/gdqixjfil.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.yfazqb.com/Article/details/gnieeutht.sHtML


<!-- 参考信息 -->