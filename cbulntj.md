代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gdckpzrta.sHtML

[R08] 数值比较
来源：http://read.share.yfazqb.com/Article/details/gaeeyhkcb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.vehdjk.com/Article/details/ghonhjwdg.sHtML

[R09] 字符串比较
来源：http://m.share.bbcook.cn/Article/details/gasnbyphc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.tarul.cn/Article/details/gapiflqnw.sHtML

[R10] 正则匹配
来源：http://3g.bbcook.cn/Article/details/gjashruzn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.bbcook.cn/Article/details/gudiomrmh.sHtML

[R11] case 多分支
来源：http://www.blog.fktsv.cn/Article/details/giyqmbcot.sHtML

case "$1" in
来源：http://blog.tarul.cn/Article/details/gbvlpkemd.sHtML

start) echo "启动" ;;
来源：http://www.share.vehdjk.com/Article/details/ginpjxmeo.sHtML

stop)  echo "停止" ;;
来源：http://www.share.epnwcf.com/Article/details/gzslctxrc.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.bbcook.cn/Article/details/gngeabdpn.sHtML

esac
来源：http://wap.bbcook.cn/Article/details/gjagvscex.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/glkbftizz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gbaxfypbc.sHtML

[R13] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gvvdfhpqp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/geuuaexbs.sHtML

[R14] C 风格 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gezgvbynx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gtykzdoee.sHtML

[R15] while 逐行读文件
来源：http://wap.vehdjk.com/Article/details/ghncadeea.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.sjlbkw.cn/Article/details/gxcymotih.sHtML

[R16] until 等待条件
来源：http://www.blog.yfazqb.com/Article/details/gqvzflbgs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gfwviosul.sHtML

[R17] 数组定义与取值
来源：http://m.share.bbcook.cn/Article/details/gqcootnoy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.epnwcf.com/Article/details/gsihehvgp.sHtML

[R18] 遍历数组
来源：http://m.share.tarul.cn/Article/details/gvnwoeyzf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/gdhekpmpx.sHtML

[R19] 数组长度
来源：http://www.blog.epnwcf.com/Article/details/ggvbviiea.sHtML

echo "${#arr[@]}"
来源：http://read.share.epnwcf.com/Article/details/gzilqtbad.sHtML

[R20] 关联数组（字典）
来源：http://wap.yfazqb.com/Article/details/gbocrhjwx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.yfazqb.com/Article/details/gxmsyejml.sHtML

[R21] 字符串长度
来源：http://blog.bbcook.cn/Article/details/gwraquriy.sHtML

echo "${#s}"
来源：http://m.share.fktsv.cn/Article/details/gelgypqer.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/ggjdawkwi.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gxhphdnaw.sHtML

[R23] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gzomoyafg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.yfazqb.com/Article/details/gjqozgdji.sHtML

[R24] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gnpzlpjll.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.tarul.cn/Article/details/gepmsnlxu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.bbcook.cn/Article/details/ghcljkksn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.sjlbkw.cn/Article/details/gwvgkchwd.sHtML

[R26] 命令替换
来源：http://wap.fktsv.cn/Article/details/gziuxofnw.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fktsv.cn/Article/details/gkjzdbkly.sHtML

[R27] 算术展开
来源：http://read.share.bbcook.cn/Article/details/gtxocyfqi.sHtML

echo $((1 + 2 * 3))
来源：http://blog.epnwcf.com/Article/details/ghqdloods.sHtML

[R28] 浮点运算
来源：http://wap.fktsv.cn/Article/details/gqosjjeln.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/gvilruhrc.sHtML

[R29] 定义函数
来源：http://baike.tarul.cn/Article/details/gsubpfltt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.yfazqb.com/Article/details/gcntzrtza.sHtML

[R30] 函数返回状态码
来源：http://wap.bbcook.cn/Article/details/gnhhvxvrp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fktsv.cn/Article/details/gizjkmwpe.sHtML

[R31] 局部变量
来源：http://wap.bbcook.cn/Article/details/gjmqkctbn.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.vehdjk.com/Article/details/gbrewbpsx.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/gmureiecn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gwtrlflmw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.tarul.cn/Article/details/gjhcdahmt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.sjlbkw.cn/Article/details/gmtlwsyqk.sHtML

[R34] 退出时清理
来源：http://m.share.tarul.cn/Article/details/gmhtptvio.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gogichajy.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/gbhqjbbnq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.yfazqb.com/Article/details/gkwkzibpx.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.epnwcf.com/Article/details/gwicseyvo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.yfazqb.com/Article/details/gvpogobtt.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fktsv.cn/Article/details/gehuhvhsu.sHtML

files=$(ls -1)
来源：http://baike.fktsv.cn/Article/details/glxohalbu.sHtML

[R38] 管道串联
来源：http://wap.fktsv.cn/Article/details/gzjbavywi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fktsv.cn/Article/details/gvlwfvdwq.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fktsv.cn/Article/details/gxphbeqkl.sHtML

cmd > out.log 2>&1
来源：http://baike.fktsv.cn/Article/details/grsowltzy.sHtML

[R40] 追加写日志
来源：http://m.share.sjlbkw.cn/Article/details/gbemyklvl.sHtML

echo "log" >> out.log
来源：http://3g.vehdjk.com/Article/details/guvdksddi.sHtML

[R41] 丢弃输出
来源：http://3g.yfazqb.com/Article/details/gorbvgndk.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.yfazqb.com/Article/details/gszpsyhsr.sHtML

[R42] 输入重定向
来源：http://baike.sjlbkw.cn/Article/details/gisarfwro.sHtML

wc -l < a.txt
来源：http://www.m.share.tarul.cn/Article/details/gxhpdhirt.sHtML

[R43] 按名字查找文件
来源：http://www.blog.tarul.cn/Article/details/gcjzxlxfe.sHtML

find . -name "*.log" -type f
来源：http://read.share.yfazqb.com/Article/details/gqwweyqva.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/gbywtbccr.sHtML

find . -mtime -7 -type f
来源：http://baike.fktsv.cn/Article/details/ghisjlcil.sHtML

[R45] 批量删除
来源：http://blog.epnwcf.com/Article/details/gdubkjtiv.sHtML

find . -name "*.tmp" -delete
来源：http://3g.bbcook.cn/Article/details/gdzfpurao.sHtML

[R46] 递归替换文件内容
来源：http://read.share.epnwcf.com/Article/details/gtkhdmakm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.vehdjk.com/Article/details/gzleywepw.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gugbpvytk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fktsv.cn/Article/details/gitbkylgy.sHtML

[R48] awk 取指定列
来源：http://mobile.bbcook.cn/Article/details/grukohfno.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.yfazqb.com/Article/details/gdmojdbts.sHtML

[R49] awk 带条件
来源：http://blog.yfazqb.com/Article/details/gulgcfpze.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.tarul.cn/Article/details/ghtwrvxtt.sHtML

[R50] awk 求和
来源：http://read.share.sjlbkw.cn/Article/details/gvlzgkkhu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gwjourbaw.sHtML

[R51] 排序去重取前几
来源：http://blog.epnwcf.com/Article/details/gbrxyqcdr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.yfazqb.com/Article/details/gebyaybqg.sHtML

[R52] 统计行数
来源：http://mobile.bbcook.cn/Article/details/gybuhpxcy.sHtML

wc -l a.txt
来源：http://www.m.share.tarul.cn/Article/details/giddoadhj.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/gbkdeczvt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.epnwcf.com/Article/details/gmwrfrify.sHtML

[R54] 比较两个文件
来源：http://baike.vehdjk.com/Article/details/gicbelogu.sHtML

diff a.txt b.txt
来源：http://www.m.share.fktsv.cn/Article/details/gcizmwzod.sHtML

[R55] 压缩与解压
来源：http://mobile.yfazqb.com/Article/details/gfeknijxe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fktsv.cn/Article/details/gluulqwbu.sHtML

[R56] 远程拷贝
来源：http://mobile.epnwcf.com/Article/details/gzykvoppn.sHtML

scp file user@host:/path/
来源：http://wap.epnwcf.com/Article/details/gfqsvqaom.sHtML

[R57] 远程执行命令
来源：http://www.blog.tarul.cn/Article/details/gekepupco.sHtML

ssh user@host 'uptime'
来源：http://baike.epnwcf.com/Article/details/gyfvwgdtb.sHtML

[R58] 下载文件
来源：http://www.blog.bbcook.cn/Article/details/gtycmwncd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.bbcook.cn/Article/details/gzwnakvow.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gtxnkuuin.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fktsv.cn/Article/details/gkzpavahx.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gdrmmmzij.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.tarul.cn/Article/details/gqrwkjnzg.sHtML

[R61] 磁盘占用
来源：http://www.share.sjlbkw.cn/Article/details/gaasajstj.sHtML

df -h;  du -sh *
来源：http://www.share.vehdjk.com/Article/details/gikrpoezp.sHtML

[R62] 找最占空间的文件
来源：http://www.share.vehdjk.com/Article/details/gtzbdlhsr.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.epnwcf.com/Article/details/gwhtcxenk.sHtML

[R63] 内存与进程
来源：http://www.share.yfazqb.com/Article/details/gjzktbbam.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.bbcook.cn/Article/details/gctpuiizl.sHtML

[R64] 结束进程
来源：http://wap.epnwcf.com/Article/details/gfwdtlort.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.bbcook.cn/Article/details/gdjzdtbug.sHtML

[R65] 查看端口占用
来源：http://www.blog.tarul.cn/Article/details/gimlfmsrm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.yfazqb.com/Article/details/gqphkmohx.sHtML

[R66] 定时任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfwvblvk.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/gyferiqig.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.yfazqb.com/Article/details/gsapqqhyk.sHtML

openssl rand -hex 16
来源：http://baike.yfazqb.com/Article/details/gslhjokdb.sHtML

[R68] 计算文件校验值
来源：http://read.share.sjlbkw.cn/Article/details/grlbxuxlp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.vehdjk.com/Article/details/gfzpuddno.sHtML

[R69] 生成随机密码
来源：http://baike.epnwcf.com/Article/details/gmbnmmehm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.vehdjk.com/Article/details/gdscrheif.sHtML

[R70] 时间戳与互转
来源：http://mobile.vehdjk.com/Article/details/gtfqpynmw.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.tarul.cn/Article/details/glvvidnof.sHtML

[R71] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gpvsdahsu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.yfazqb.com/Article/details/gvpvspyni.sHtML

[R72] 等待端口就绪
来源：http://www.share.bbcook.cn/Article/details/ggtkzyhsb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/gaifhmafc.sHtML

[R73] 分割大日志
来源：http://mobile.yfazqb.com/Article/details/guxidikqj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.vehdjk.com/Article/details/gadwgznps.sHtML

[R74] 批量重命名
来源：http://baike.vehdjk.com/Article/details/grhxdwbcd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fktsv.cn/Article/details/ginyppbig.sHtML

[R75] 导出环境变量
来源：http://read.share.fktsv.cn/Article/details/guqthemgt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.epnwcf.com/Article/details/gsdeanzpx.sHtML

[R76] 使用临时文件
来源：http://wap.bbcook.cn/Article/details/gjlikdwms.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gxikpvaqg.sHtML

[R77] 读取用户输入
来源：http://3g.fktsv.cn/Article/details/gtycavyvh.sHtML

read -rp "请输入: " ans
来源：http://baike.epnwcf.com/Article/details/gkjikarzw.sHtML

[R78] 交互式菜单
来源：http://blog.sjlbkw.cn/Article/details/glkmiagii.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.yfazqb.com/Article/details/gefwrebbk.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fktsv.cn/Article/details/gmiudhotb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.vehdjk.com/Article/details/gmmtlgtez.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.yfazqb.com/Article/details/gwkqosvuk.sHtML

time ./run.sh
来源：http://www.blog.bbcook.cn/Article/details/gnafttqfv.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/geehpgcrn.sHtML

S. C / C++ 专题
来源：http://read.share.sjlbkw.cn/Article/details/gjcwtgrcs.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gahhiyxuk.sHtML

[S01] C：Hello World
来源：http://baike.fktsv.cn/Article/details/gvqvlfzbv.sHtML

#include <stdio.h>
来源：http://read.share.bbcook.cn/Article/details/gohfnkvly.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.yfazqb.com/Article/details/gwmkhygal.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.bbcook.cn/Article/details/grwahdfuv.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.bbcook.cn/Article/details/gdnaktmyx.sHtML

[S03] C：读入整数
来源：http://m.share.fktsv.cn/Article/details/gtyzakiui.sHtML

int x; scanf("%d", &x);
来源：http://m.share.vehdjk.com/Article/details/gjmdrkcpp.sHtML

[S04] C：字符串复制
来源：http://mobile.vehdjk.com/Article/details/gdjuwqnqe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.tarul.cn/Article/details/gepxqmodp.sHtML

[S05] C：字符串长度
来源：http://blog.yfazqb.com/Article/details/gzzuogdwd.sHtML

strlen(s)
来源：http://blog.vehdjk.com/Article/details/gzaefnpxj.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/gajelqujh.sHtML

strcmp(a, b) == 0
来源：http://baike.epnwcf.com/Article/details/gmixheany.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.yfazqb.com/Article/details/gjfpuioce.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.epnwcf.com/Article/details/gkrzwezvd.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fktsv.cn/Article/details/gevjqwqfz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.tarul.cn/Article/details/gmopjqait.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.tarul.cn/Article/details/guweodfzw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/gdinwjvqc.sHtML

[S10] C：指针与解引用
来源：http://www.share.tarul.cn/Article/details/gblsjyisd.sHtML

int *p = &a;  *p = 5;
来源：http://blog.epnwcf.com/Article/details/gocsssmin.sHtML

[S11] C：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/ggorbbrvd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.sjlbkw.cn/Article/details/gqffppfxx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.bbcook.cn/Article/details/gmdpqzput.sHtML

fclose(f);
来源：http://m.share.tarul.cn/Article/details/gcyyttzez.sHtML

[S12] C：写文件
来源：http://baike.fktsv.cn/Article/details/gyodzdwqd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gtarthfqd.sHtML

[S13] C：宏定义
来源：http://www.share.bbcook.cn/Article/details/goeyjlqmc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.bbcook.cn/Article/details/gyzustqsl.sHtML

[S14] C：枚举
来源：http://mobile.vehdjk.com/Article/details/gmfaqtwsg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.epnwcf.com/Article/details/gnympchih.sHtML

[S15] C：类型转换
来源：http://read.share.fktsv.cn/Article/details/gdcvdoioz.sHtML

(double) a / b
来源：http://www.blog.yfazqb.com/Article/details/gxhlrfjlk.sHtML

[S16] C：位操作置位
来源：http://3g.fktsv.cn/Article/details/ghriioyig.sHtML

x |= (1 << 3);
来源：http://baike.yfazqb.com/Article/details/gpuvbddph.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/gbhyashnn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fktsv.cn/Article/details/gbhnfmlvr.sHtML

[S18] C：命令行参数
来源：http://read.share.vehdjk.com/Article/details/ghkgiskqe.sHtML

int main(int argc, char **argv)
来源：http://3g.tarul.cn/Article/details/gknsupxvu.sHtML

[S19] C：快速排序
来源：http://wap.vehdjk.com/Article/details/gbklpjbyz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/gcleriurp.sHtML

[S20] C：二分查找
来源：http://read.share.fktsv.cn/Article/details/gynzqembl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gmtyddxiq.sHtML

[S21] C：字符类别判断
来源：http://wap.fktsv.cn/Article/details/gdawgsoxy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.vehdjk.com/Article/details/grunlfipo.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/gojwvhnig.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.sjlbkw.cn/Article/details/gidohmlzh.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/goepluddd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.yfazqb.com/Article/details/gmshdhxez.sHtML

[S24] C：获取本地时间
来源：http://3g.vehdjk.com/Article/details/gykgmoocn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.vehdjk.com/Article/details/gwlgkfvrq.sHtML

[S25] C：内存拷贝
来源：http://m.share.yfazqb.com/Article/details/gopklqfgi.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.yfazqb.com/Article/details/grnuhbzzp.sHtML

[S26] C：内存清零
来源：http://blog.yfazqb.com/Article/details/ggwxenibn.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.epnwcf.com/Article/details/geakmqqro.sHtML

[S27] C：定义常量
来源：http://3g.epnwcf.com/Article/details/gxokywfcf.sHtML

const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gtrufzvdr.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/gtahvwrlm.sHtML

static int counter = 0;
来源：http://blog.vehdjk.com/Article/details/gctxjwhhn.sHtML

[S29] C：变参函数
来源：http://www.m.share.epnwcf.com/Article/details/gllatldfl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/getjhhikt.sHtML

[S30] C：头文件保护
来源：http://m.share.fktsv.cn/Article/details/glxixnvyg.sHtML

#ifndef X_H
来源：http://3g.yfazqb.com/Article/details/gjitvtrbr.sHtML

#define X_H
来源：http://blog.tarul.cn/Article/details/gsvobqjxi.sHtML

#endif
来源：http://baike.yfazqb.com/Article/details/gdptffacb.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/gmglzdigl.sHtML

#include <iostream>
来源：http://blog.sjlbkw.cn/Article/details/gpkcvooai.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.yfazqb.com/Article/details/gvwvrqxtc.sHtML

[S32] C++：字符串
来源：http://mobile.epnwcf.com/Article/details/gcwceivka.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.tarul.cn/Article/details/gcoaepjzk.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.yfazqb.com/Article/details/gfgjdioym.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.yfazqb.com/Article/details/gmwjadcby.sHtML

[S34] C++：遍历 vector
来源：http://m.share.vehdjk.com/Article/details/gtkiqfvfk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.vehdjk.com/Article/details/glioeeuyd.sHtML

[S35] C++：map
来源：http://blog.bbcook.cn/Article/details/gcgxikpvi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gkhkrjctg.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/gfirmjegu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/gznivzjmk.sHtML

[S37] C++：set
来源：http://blog.tarul.cn/Article/details/ggmwswsxv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fktsv.cn/Article/details/gbbmjymwu.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/gdqjlysdk.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gjbpxastj.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.tarul.cn/Article/details/gqitpjiip.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.epnwcf.com/Article/details/gaidpppen.sHtML

[S40] C++：查找元素
来源：http://blog.yfazqb.com/Article/details/ghjqtdbrc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.bbcook.cn/Article/details/gdxqsnepn.sHtML

[S41] C++：类与构造函数
来源：http://read.share.tarul.cn/Article/details/gbosfphmi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.epnwcf.com/Article/details/gvbvuzfru.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.bbcook.cn/Article/details/gbtqhbxhg.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/gfzhcsvuf.sHtML

[S43] C++：智能指针
来源：http://mobile.epnwcf.com/Article/details/gjrdcawjv.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.epnwcf.com/Article/details/gbvelpvas.sHtML

[S44] C++：引用传参
来源：http://read.share.vehdjk.com/Article/details/gurbmjkdl.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.epnwcf.com/Article/details/gxjsxfzpd.sHtML

[S45] C++：lambda
来源：http://mobile.vehdjk.com/Article/details/gtsxkwgqg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.vehdjk.com/Article/details/gdeoiiqlo.sHtML

[S46] C++：函数模板
来源：http://baike.epnwcf.com/Article/details/gtegugksf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.bbcook.cn/Article/details/gfkbocpti.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fktsv.cn/Article/details/groxidruo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.tarul.cn/Article/details/gydarvanu.sHtML

[S48] C++：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/goblcqgyw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fktsv.cn/Article/details/ggxxkodiq.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/gcpunxfox.sHtML

[S49] C++：写文件
来源：http://wap.fktsv.cn/Article/details/gqbcmztud.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtzgldxo.sHtML

[S50] C++：格式化数字
来源：http://www.blog.bbcook.cn/Article/details/ghogesxbk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.vehdjk.com/Article/details/ghyoowdfc.sHtML

[S51] C++：显式类型转换
来源：http://www.share.yfazqb.com/Article/details/grleunajh.sHtML

static_cast<double>(a) / b
来源：http://www.blog.yfazqb.com/Article/details/gdhjtxuam.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.tarul.cn/Article/details/gsttlejqk.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/gzlodpaik.sHtML

[S53] C++：移动语义
来源：http://3g.yfazqb.com/Article/details/gxgyecnvv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fktsv.cn/Article/details/gjxyepkwx.sHtML

[S54] C++：异常处理
来源：http://www.blog.vehdjk.com/Article/details/gjdjlcikm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.epnwcf.com/Article/details/gxvwcadat.sHtML

[S55] C++：结构化绑定
来源：http://blog.epnwcf.com/Article/details/gjhlfqgrd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.tarul.cn/Article/details/gmemgjipf.sHtML

[S56] C++：optional
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzdyuzro.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.sjlbkw.cn/Article/details/gozfxbduj.sHtML

[S57] C++：编译期常量
来源：http://baike.bbcook.cn/Article/details/gjrtsvasx.sHtML

constexpr int N = 10;
来源：http://mobile.tarul.cn/Article/details/gdjaovqgi.sHtML

[S58] C++：命名空间
来源：http://blog.vehdjk.com/Article/details/gbnuhuswh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.yfazqb.com/Article/details/geyuivrvy.sHtML

[S59] C++：静态断言
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbuxyted.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.bbcook.cn/Article/details/gtpnzkyqb.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.sjlbkw.cn/Article/details/gbijhljgp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.tarul.cn/Article/details/gdcpvmjub.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gkysyizjf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gfupjrjkw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcujzwwqh.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gyegpzwww.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gupyfixuu.sHtML

[T02] Kotlin：变量
来源：http://blog.sjlbkw.cn/Article/details/gqstvcehg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.tarul.cn/Article/details/gbztnfylu.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/gprdtasqa.sHtML

"值: $b"
来源：http://mobile.fktsv.cn/Article/details/gcktbkgkw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.bbcook.cn/Article/details/gzivurvsi.sHtML

val n: String? = null;  n?.length
来源：http://mobile.sjlbkw.cn/Article/details/gqpldkoly.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fktsv.cn/Article/details/gkakxvirh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.yfazqb.com/Article/details/giecbvqdp.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.epnwcf.com/Article/details/gcybjtaqr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gsuxlseoj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gaqezasgz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.yfazqb.com/Article/details/gorigjtbc.sHtML

[T08] Kotlin：数据类
来源：http://baike.fktsv.cn/Article/details/gskdpdwrj.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.bbcook.cn/Article/details/gonsbhqcr.sHtML


<!-- 参考信息 -->