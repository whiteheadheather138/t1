代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.epnwcf.com/Article/details/gkqscsgkf.sHtML

[R18] 遍历数组
来源：http://mobile.yfazqb.com/Article/details/guecijiem.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.vehdjk.com/Article/details/ggzcybtxo.sHtML

[R19] 数组长度
来源：http://www.m.share.vehdjk.com/Article/details/gibuammtw.sHtML

echo "${#arr[@]}"
来源：http://read.share.tarul.cn/Article/details/ggsjwkfav.sHtML

[R20] 关联数组（字典）
来源：http://www.share.tarul.cn/Article/details/gzekqmfqo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.tarul.cn/Article/details/gnnopbvxw.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/gobecrgsk.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/gpwvufzyy.sHtML

[R22] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gfxzlnyat.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/gakntnolc.sHtML

[R23] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gqusrucpv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.epnwcf.com/Article/details/glimldqfm.sHtML

[R24] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gtrpbfmme.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.vehdjk.com/Article/details/gkduyuohq.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fktsv.cn/Article/details/gkbreebhp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.epnwcf.com/Article/details/greuvfhhv.sHtML

[R26] 命令替换
来源：http://www.share.vehdjk.com/Article/details/gtzclvtta.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.yfazqb.com/Article/details/gjdkqlmux.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gijtddmoo.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.yfazqb.com/Article/details/gkkrjnmci.sHtML

[R28] 浮点运算
来源：http://www.share.epnwcf.com/Article/details/gmzqtbxmx.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/gylnopbeo.sHtML

[R29] 定义函数
来源：http://3g.vehdjk.com/Article/details/gpodrswnd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgotbyhc.sHtML

[R30] 函数返回状态码
来源：http://m.share.vehdjk.com/Article/details/gdbixurji.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.sjlbkw.cn/Article/details/gynkpyezx.sHtML

[R31] 局部变量
来源：http://wap.tarul.cn/Article/details/gvnpufdul.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.bbcook.cn/Article/details/gskvkzxaa.sHtML

[R32] 参数个数校验
来源：http://3g.vehdjk.com/Article/details/gcybnpkim.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/gybsmkllh.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.sjlbkw.cn/Article/details/gdfdbnehw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.tarul.cn/Article/details/gssetbvkr.sHtML

[R34] 退出时清理
来源：http://baike.vehdjk.com/Article/details/gjodtjzga.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gbbtlfpfx.sHtML

[R35] 后台执行并等待
来源：http://baike.fktsv.cn/Article/details/guvjyldgn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.epnwcf.com/Article/details/ghucxlgrc.sHtML

[R36] 并发执行多个任务
来源：http://baike.bbcook.cn/Article/details/gotngfwka.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.sjlbkw.cn/Article/details/gnkcwzhey.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/gwamoxyko.sHtML

files=$(ls -1)
来源：http://read.share.epnwcf.com/Article/details/gjqpfrkrh.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/gxkcikdxa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.yfazqb.com/Article/details/ghkbfkmij.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/gcuzjnkkc.sHtML

cmd > out.log 2>&1
来源：http://wap.vehdjk.com/Article/details/gywmowsbe.sHtML

[R40] 追加写日志
来源：http://3g.tarul.cn/Article/details/grfbubxcs.sHtML

echo "log" >> out.log
来源：http://m.share.fktsv.cn/Article/details/gtkemslpq.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/gxpcyjmru.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fktsv.cn/Article/details/gvcktoxfh.sHtML

[R42] 输入重定向
来源：http://www.share.sjlbkw.cn/Article/details/gaozpzsny.sHtML

wc -l < a.txt
来源：http://www.blog.fktsv.cn/Article/details/gkcxsgsnw.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gilhmfdnn.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.tarul.cn/Article/details/gaajomanu.sHtML

[R44] 按修改时间查找
来源：http://mobile.sjlbkw.cn/Article/details/gssihucul.sHtML

find . -mtime -7 -type f
来源：http://www.blog.bbcook.cn/Article/details/gaulnxvpa.sHtML

[R45] 批量删除
来源：http://blog.epnwcf.com/Article/details/gzdoschsn.sHtML

find . -name "*.tmp" -delete
来源：http://wap.bbcook.cn/Article/details/gdwxfpeye.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.epnwcf.com/Article/details/gvcevqwco.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.tarul.cn/Article/details/gyvdlocyh.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/ggwusowxt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.tarul.cn/Article/details/gmghgbzgk.sHtML

[R48] awk 取指定列
来源：http://baike.epnwcf.com/Article/details/guyenmzht.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gkluuptcb.sHtML

[R49] awk 带条件
来源：http://mobile.bbcook.cn/Article/details/gyglhwfro.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.sjlbkw.cn/Article/details/gxcinbvzw.sHtML

[R50] awk 求和
来源：http://mobile.epnwcf.com/Article/details/glcdirieu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gzecnfcbb.sHtML

[R51] 排序去重取前几
来源：http://3g.tarul.cn/Article/details/gieazcpfv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.vehdjk.com/Article/details/gthzwplhj.sHtML

[R52] 统计行数
来源：http://www.share.bbcook.cn/Article/details/gudnrmauz.sHtML

wc -l a.txt
来源：http://baike.epnwcf.com/Article/details/gzwqkxcew.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.epnwcf.com/Article/details/gnjlhwpde.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.tarul.cn/Article/details/gqdnjnufn.sHtML

[R54] 比较两个文件
来源：http://mobile.bbcook.cn/Article/details/gaimemsob.sHtML

diff a.txt b.txt
来源：http://read.share.vehdjk.com/Article/details/gjcrjrdzv.sHtML

[R55] 压缩与解压
来源：http://www.m.share.bbcook.cn/Article/details/gtaxezthb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fktsv.cn/Article/details/ghhldfnhn.sHtML

[R56] 远程拷贝
来源：http://mobile.yfazqb.com/Article/details/glnafelqe.sHtML

scp file user@host:/path/
来源：http://3g.vehdjk.com/Article/details/glrpfvfwn.sHtML

[R57] 远程执行命令
来源：http://mobile.tarul.cn/Article/details/gpkcrsgeb.sHtML

ssh user@host 'uptime'
来源：http://mobile.fktsv.cn/Article/details/gewyftlnk.sHtML

[R58] 下载文件
来源：http://www.blog.fktsv.cn/Article/details/gaoxrzasq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.sjlbkw.cn/Article/details/gzlaolnsa.sHtML

[R59] 发 POST JSON
来源：http://3g.epnwcf.com/Article/details/grhpxfcwy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/goscvgctk.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/ggnvltnrs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.bbcook.cn/Article/details/gblpaqmfs.sHtML

[R61] 磁盘占用
来源：http://www.share.vehdjk.com/Article/details/gxamznpne.sHtML

df -h;  du -sh *
来源：http://www.blog.epnwcf.com/Article/details/ggjiqjfzh.sHtML

[R62] 找最占空间的文件
来源：http://mobile.epnwcf.com/Article/details/gxfquvpbs.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fktsv.cn/Article/details/gmeoshcrs.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gtpogstof.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.epnwcf.com/Article/details/gpzajsfhi.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gacuxubzp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.vehdjk.com/Article/details/gwxbyogrt.sHtML

[R65] 查看端口占用
来源：http://wap.vehdjk.com/Article/details/gggknpiij.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.yfazqb.com/Article/details/ggqmgztts.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/gxzgegjng.sHtML

crontab -e;  crontab -l
来源：http://baike.bbcook.cn/Article/details/ggtfnyumb.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.tarul.cn/Article/details/gcdfbezip.sHtML

openssl rand -hex 16
来源：http://3g.bbcook.cn/Article/details/gwnzhanbg.sHtML

[R68] 计算文件校验值
来源：http://www.blog.vehdjk.com/Article/details/gnutpklac.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.tarul.cn/Article/details/gqoftbean.sHtML

[R69] 生成随机密码
来源：http://3g.vehdjk.com/Article/details/gezppfxev.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fktsv.cn/Article/details/gsvlxydqy.sHtML

[R70] 时间戳与互转
来源：http://3g.sjlbkw.cn/Article/details/gamymphby.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.vehdjk.com/Article/details/gbhakrjei.sHtML

[R71] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gsfisvpyv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.yfazqb.com/Article/details/gnbxilyhb.sHtML

[R72] 等待端口就绪
来源：http://mobile.vehdjk.com/Article/details/govqdfoym.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/glpvtevoy.sHtML

[R73] 分割大日志
来源：http://baike.fktsv.cn/Article/details/gembusffd.sHtML

split -l 1000 big.log part_
来源：http://mobile.sjlbkw.cn/Article/details/gwvkszlpi.sHtML

[R74] 批量重命名
来源：http://www.m.share.bbcook.cn/Article/details/gzpjtthed.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/gzqhcigma.sHtML

[R75] 导出环境变量
来源：http://wap.vehdjk.com/Article/details/gdyxbinlq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.yfazqb.com/Article/details/gbgbmorir.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/gpldmgvzl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gmcqblxfu.sHtML

[R77] 读取用户输入
来源：http://baike.yfazqb.com/Article/details/gsnlrjxzy.sHtML

read -rp "请输入: " ans
来源：http://m.share.fktsv.cn/Article/details/gukdmfcjs.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/gowhqrvrc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.sjlbkw.cn/Article/details/gwqaaknkw.sHtML

[R79] 解析命令行选项
来源：http://baike.bbcook.cn/Article/details/gluuhzlya.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fktsv.cn/Article/details/gwqypeagx.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.tarul.cn/Article/details/gbpwxsnpc.sHtML

time ./run.sh
来源：http://blog.sjlbkw.cn/Article/details/gstlzwdjp.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gbdhjzvrs.sHtML

S. C / C++ 专题
来源：http://blog.yfazqb.com/Article/details/gsgywrshp.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gyajypsmr.sHtML

[S01] C：Hello World
来源：http://3g.fktsv.cn/Article/details/gzexfvucj.sHtML

#include <stdio.h>
来源：http://www.blog.sjlbkw.cn/Article/details/gpxgojhxl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.yfazqb.com/Article/details/gvzwiredx.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.yfazqb.com/Article/details/ghwveiqfk.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.sjlbkw.cn/Article/details/gecpgdvyi.sHtML

[S03] C：读入整数
来源：http://3g.epnwcf.com/Article/details/gpdadaokr.sHtML

int x; scanf("%d", &x);
来源：http://blog.bbcook.cn/Article/details/gblvrtxvh.sHtML

[S04] C：字符串复制
来源：http://read.share.tarul.cn/Article/details/glafljvao.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/gebpiuquy.sHtML

[S05] C：字符串长度
来源：http://mobile.fktsv.cn/Article/details/grvotlfek.sHtML

strlen(s)
来源：http://blog.bbcook.cn/Article/details/giucjchpt.sHtML

[S06] C：字符串比较
来源：http://wap.vehdjk.com/Article/details/gjhvnwszs.sHtML

strcmp(a, b) == 0
来源：http://wap.bbcook.cn/Article/details/gxlpowtnv.sHtML

[S07] C：数组遍历求和
来源：http://blog.yfazqb.com/Article/details/gqxcwmjnl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.epnwcf.com/Article/details/gmjzcxtnh.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.epnwcf.com/Article/details/gqqvjxjnf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/gnxxqcfnz.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.tarul.cn/Article/details/gdmbyprxa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.yfazqb.com/Article/details/gtvrvnsok.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.tarul.cn/Article/details/gvznazgvv.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.tarul.cn/Article/details/gejrlulvv.sHtML

[S11] C：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gstgvzrvh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.bbcook.cn/Article/details/gjadvkmla.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fktsv.cn/Article/details/gqtgfrnkh.sHtML

fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gwphyocaw.sHtML

[S12] C：写文件
来源：http://m.share.epnwcf.com/Article/details/gliofdqyb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gjeusxxhb.sHtML

[S13] C：宏定义
来源：http://www.m.share.epnwcf.com/Article/details/ggckenerz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/gaymshbcf.sHtML

[S14] C：枚举
来源：http://mobile.epnwcf.com/Article/details/gihnhbxle.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fktsv.cn/Article/details/gapaepdie.sHtML

[S15] C：类型转换
来源：http://read.share.epnwcf.com/Article/details/glrkacevi.sHtML

(double) a / b
来源：http://mobile.tarul.cn/Article/details/gxcdabyvp.sHtML

[S16] C：位操作置位
来源：http://www.m.share.sjlbkw.cn/Article/details/gsulihebl.sHtML

x |= (1 << 3);
来源：http://www.blog.yfazqb.com/Article/details/gywagxmuh.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gcsflokek.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fktsv.cn/Article/details/gaxzqaxur.sHtML

[S18] C：命令行参数
来源：http://mobile.vehdjk.com/Article/details/gchstoffv.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/gjqmlixzr.sHtML

[S19] C：快速排序
来源：http://3g.bbcook.cn/Article/details/gjxwyazld.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/gukvrajal.sHtML

[S20] C：二分查找
来源：http://m.share.bbcook.cn/Article/details/gdwfmdksy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/ghexzfxbn.sHtML

[S21] C：字符类别判断
来源：http://baike.tarul.cn/Article/details/grizxqvxi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.tarul.cn/Article/details/ggfrhuzjb.sHtML

[S22] C：字符串转数字
来源：http://blog.bbcook.cn/Article/details/girhoxosq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/gklioucqa.sHtML

[S23] C：随机数
来源：http://read.share.yfazqb.com/Article/details/gzsrpkyhf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.tarul.cn/Article/details/gadzykouk.sHtML

[S24] C：获取本地时间
来源：http://wap.yfazqb.com/Article/details/gxgrlblvp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/gehunrune.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/gfdbqnrot.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.yfazqb.com/Article/details/gshwnlsjz.sHtML

[S26] C：内存清零
来源：http://read.share.fktsv.cn/Article/details/gluabhqrz.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fktsv.cn/Article/details/gfwbnrhnl.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/gcvxbfroz.sHtML

const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/grhlzpzpp.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/gtogubzmk.sHtML

static int counter = 0;
来源：http://mobile.sjlbkw.cn/Article/details/glrmzqllv.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/gehrqplxo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.sjlbkw.cn/Article/details/geoywgxrv.sHtML

[S30] C：头文件保护
来源：http://wap.vehdjk.com/Article/details/gzjihsfsm.sHtML

#ifndef X_H
来源：http://mobile.yfazqb.com/Article/details/gxcyfsnhj.sHtML

#define X_H
来源：http://www.m.share.tarul.cn/Article/details/gvmaqrstb.sHtML

#endif
来源：http://www.blog.tarul.cn/Article/details/giliesfwy.sHtML

[S31] C++：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/goqhcmxkq.sHtML

#include <iostream>
来源：http://www.m.share.epnwcf.com/Article/details/gosdcbqhy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.yfazqb.com/Article/details/gsjktmvma.sHtML

[S32] C++：字符串
来源：http://3g.epnwcf.com/Article/details/guiercjqf.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.vehdjk.com/Article/details/gkpnvlvhs.sHtML

[S33] C++：vector 增删
来源：http://baike.epnwcf.com/Article/details/gzozbupzp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.vehdjk.com/Article/details/gvkhqesij.sHtML

[S34] C++：遍历 vector
来源：http://baike.fktsv.cn/Article/details/gsvusnvjx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.tarul.cn/Article/details/giwtpwksq.sHtML

[S35] C++：map
来源：http://wap.bbcook.cn/Article/details/goiyiahqe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gxbxzqwbw.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gmohixklx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gvvyusptz.sHtML

[S37] C++：set
来源：http://www.m.share.sjlbkw.cn/Article/details/goadxtpac.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.vehdjk.com/Article/details/gnricfsix.sHtML

[S38] C++：排序
来源：http://blog.epnwcf.com/Article/details/gwmdotlpy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gagaidfec.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.tarul.cn/Article/details/gxoyatjit.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.epnwcf.com/Article/details/gwxyfovko.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/gxxuaqkcy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.sjlbkw.cn/Article/details/gafkqbhtn.sHtML

[S41] C++：类与构造函数
来源：http://wap.epnwcf.com/Article/details/gpodfokww.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.tarul.cn/Article/details/grbuttazh.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.vehdjk.com/Article/details/gigwpqttj.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.tarul.cn/Article/details/grlwwwyck.sHtML

[S43] C++：智能指针
来源：http://www.blog.epnwcf.com/Article/details/gztzspvzz.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.sjlbkw.cn/Article/details/gzecmhfyo.sHtML

[S44] C++：引用传参
来源：http://baike.vehdjk.com/Article/details/gqfqyltcz.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fktsv.cn/Article/details/gbrlvgcfk.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/gctvuuoch.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/grlrjrrkh.sHtML

[S46] C++：函数模板
来源：http://3g.epnwcf.com/Article/details/gxshqhgvp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/gsgwseuot.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.vehdjk.com/Article/details/gxtrcvtbg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.vehdjk.com/Article/details/gomlfjdtg.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gtbrgvzwk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fktsv.cn/Article/details/govmodfqo.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/gsjlejsom.sHtML

[S49] C++：写文件
来源：http://read.share.epnwcf.com/Article/details/gzixkfylm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.bbcook.cn/Article/details/gvpaptgii.sHtML

[S50] C++：格式化数字
来源：http://www.blog.epnwcf.com/Article/details/gmjcfwbxv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/ggxpodklw.sHtML

[S51] C++：显式类型转换
来源：http://baike.yfazqb.com/Article/details/gvjiagjoz.sHtML

static_cast<double>(a) / b
来源：http://www.share.vehdjk.com/Article/details/gmfqvqyqd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.vehdjk.com/Article/details/gpeugulko.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.tarul.cn/Article/details/gphcrgrpu.sHtML

[S53] C++：移动语义
来源：http://mobile.epnwcf.com/Article/details/gvscmrdnl.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.yfazqb.com/Article/details/gntzjphib.sHtML

[S54] C++：异常处理
来源：http://m.share.yfazqb.com/Article/details/gwducyqts.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.epnwcf.com/Article/details/gspssovum.sHtML

[S55] C++：结构化绑定
来源：http://read.share.vehdjk.com/Article/details/gzecycgky.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fktsv.cn/Article/details/gicjgyanu.sHtML

[S56] C++：optional
来源：http://www.blog.tarul.cn/Article/details/grlwzrqsv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.yfazqb.com/Article/details/grwovosrg.sHtML

[S57] C++：编译期常量
来源：http://blog.yfazqb.com/Article/details/geelngmoz.sHtML

constexpr int N = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gnazkdsva.sHtML

[S58] C++：命名空间
来源：http://read.share.fktsv.cn/Article/details/gstffdxfm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.epnwcf.com/Article/details/gqcjwdeoj.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/gonwygfpi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.bbcook.cn/Article/details/gvmwdioki.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.yfazqb.com/Article/details/gmrlabake.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fktsv.cn/Article/details/gvfwqhksb.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmojsbalw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.tarul.cn/Article/details/gcpbczjri.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gchedkmof.sHtML

[T01] Kotlin：Hello World
来源：http://baike.epnwcf.com/Article/details/gwlbplwdo.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gyqsknjde.sHtML

[T02] Kotlin：变量
来源：http://blog.vehdjk.com/Article/details/gazewkurf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.yfazqb.com/Article/details/gdffnaxsy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fktsv.cn/Article/details/gbrixmhxs.sHtML

"值: $b"
来源：http://wap.sjlbkw.cn/Article/details/gqxpxtqdu.sHtML

[T04] Kotlin：空安全
来源：http://baike.tarul.cn/Article/details/gpwwubyzo.sHtML

val n: String? = null;  n?.length
来源：http://m.share.yfazqb.com/Article/details/gknkkmehp.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.bbcook.cn/Article/details/gzhwxwttt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.epnwcf.com/Article/details/gbsrdjwgp.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.tarul.cn/Article/details/gyjobajbx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gwyornwgc.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gyknzxpkd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.yfazqb.com/Article/details/gepznqifh.sHtML

[T08] Kotlin：数据类
来源：http://wap.yfazqb.com/Article/details/gcpbdamjp.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fktsv.cn/Article/details/gsyrstjvu.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.yfazqb.com/Article/details/gpszatujm.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.bbcook.cn/Article/details/gehgqmznh.sHtML

[T10] Kotlin：默认参数
来源：http://3g.tarul.cn/Article/details/gdymcvevt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.yfazqb.com/Article/details/gfhggsvan.sHtML

[T11] Kotlin：协程
来源：http://mobile.tarul.cn/Article/details/gkmllrwau.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.epnwcf.com/Article/details/gvoffshyj.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.yfazqb.com/Article/details/gdfdvgxnv.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gyhzfitom.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.bbcook.cn/Article/details/gtnjvpzgt.sHtML

val m = mapOf("a" to 1)
来源：http://3g.vehdjk.com/Article/details/gbnmlbyao.sHtML

[T14] Kotlin：循环
来源：http://3g.sjlbkw.cn/Article/details/gunkawqpq.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gaoynkbta.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/gcjxhbfqs.sHtML

interface Shape { fun area(): Double }
来源：http://3g.epnwcf.com/Article/details/grpffwpzf.sHtML

[T16] Swift：Hello World
来源：http://read.share.tarul.cn/Article/details/gnlvqdpjl.sHtML

print("Hello")
来源：http://read.share.tarul.cn/Article/details/gekuegcia.sHtML

[T17] Swift：变量与常量
来源：http://m.share.sjlbkw.cn/Article/details/ggftcnhcp.sHtML

var a = 1;  let b = 2
来源：http://blog.bbcook.cn/Article/details/gducclhlz.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gzygdfmda.sHtML

"值: \(b)"
来源：http://m.share.sjlbkw.cn/Article/details/gxmoxgwqd.sHtML

[T19] Swift：可选绑定
来源：http://read.share.vehdjk.com/Article/details/gysygtxct.sHtML

if let n = opt { print(n) }
来源：http://3g.sjlbkw.cn/Article/details/guaqxlrzr.sHtML

[T20] Swift：数组操作
来源：http://m.share.bbcook.cn/Article/details/gfybwfgas.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.bbcook.cn/Article/details/gdnacqomh.sHtML


<!-- 参考信息 -->