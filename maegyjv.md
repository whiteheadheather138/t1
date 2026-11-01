代发 wailian999

esac
来源：http://mobile.yfazqb.com/Article/details/gylepxxfe.sHtML

[R12] for 遍历文件
来源：http://blog.tarul.cn/Article/details/gtsapcezq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.bbcook.cn/Article/details/gzoerpnit.sHtML

[R13] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/gadwayvxj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/ghyxqqgos.sHtML

[R14] C 风格 for
来源：http://baike.tarul.cn/Article/details/giqbmlmuv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gpridgcfv.sHtML

[R15] while 逐行读文件
来源：http://m.share.epnwcf.com/Article/details/glfdsmpoj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gindiazvi.sHtML

[R16] until 等待条件
来源：http://www.m.share.yfazqb.com/Article/details/gyahapjum.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/guyavdpoc.sHtML

[R17] 数组定义与取值
来源：http://m.share.bbcook.cn/Article/details/gycqqktnz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.bbcook.cn/Article/details/gsvarlaqu.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/ghapndmmb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.yfazqb.com/Article/details/gfhqrdhng.sHtML

[R19] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/gmfkmbrhd.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/gmdpandyd.sHtML

[R20] 关联数组（字典）
来源：http://m.share.epnwcf.com/Article/details/gclijybhm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.vehdjk.com/Article/details/gvokjjjcn.sHtML

[R21] 字符串长度
来源：http://wap.sjlbkw.cn/Article/details/grfndpotc.sHtML

echo "${#s}"
来源：http://www.m.share.epnwcf.com/Article/details/gcaffdpxx.sHtML

[R22] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/geampkzii.sHtML

echo "${s:0:5}"
来源：http://baike.tarul.cn/Article/details/gdiqijkce.sHtML

[R23] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/ghzopcmna.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.vehdjk.com/Article/details/gfwnybqfr.sHtML

[R24] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gkihaizfz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.sjlbkw.cn/Article/details/gjueiiyxy.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.sjlbkw.cn/Article/details/gscjvlidz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.bbcook.cn/Article/details/gnpbuwqym.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/gicisksin.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gbygdaeow.sHtML

[R27] 算术展开
来源：http://3g.sjlbkw.cn/Article/details/gjuvhzlsj.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.yfazqb.com/Article/details/gjxpkitxl.sHtML

[R28] 浮点运算
来源：http://www.blog.yfazqb.com/Article/details/gbplnfydw.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.bbcook.cn/Article/details/gjgxsnmuh.sHtML

[R29] 定义函数
来源：http://www.share.vehdjk.com/Article/details/gqgwpxbgt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/gwmgezwug.sHtML

[R30] 函数返回状态码
来源：http://3g.bbcook.cn/Article/details/gdjmkjrtj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.yfazqb.com/Article/details/gfdjrzgbi.sHtML

[R31] 局部变量
来源：http://www.blog.yfazqb.com/Article/details/gapedxlwa.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.tarul.cn/Article/details/getrbqzrv.sHtML

[R32] 参数个数校验
来源：http://mobile.sjlbkw.cn/Article/details/gmstwigse.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gglloykcl.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.epnwcf.com/Article/details/gmnqzgplh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.sjlbkw.cn/Article/details/gvfafmqgu.sHtML

[R34] 退出时清理
来源：http://mobile.yfazqb.com/Article/details/gfjwuhzsq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/gljokjiem.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/gxczdhajy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.yfazqb.com/Article/details/gvjgeiwko.sHtML

[R36] 并发执行多个任务
来源：http://wap.epnwcf.com/Article/details/ggzoyhjcg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.epnwcf.com/Article/details/gqtzbaufy.sHtML

[R37] 把输出赋给变量
来源：http://www.share.yfazqb.com/Article/details/gaxlhwnov.sHtML

files=$(ls -1)
来源：http://baike.sjlbkw.cn/Article/details/gwyfwleeo.sHtML

[R38] 管道串联
来源：http://baike.tarul.cn/Article/details/gwqtzkzal.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.tarul.cn/Article/details/gloynpaor.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.vehdjk.com/Article/details/gaptmyjal.sHtML

cmd > out.log 2>&1
来源：http://read.share.fktsv.cn/Article/details/gioiwyhjj.sHtML

[R40] 追加写日志
来源：http://baike.yfazqb.com/Article/details/gkzxzeqjy.sHtML

echo "log" >> out.log
来源：http://baike.yfazqb.com/Article/details/gseatgppb.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/gvpfojqke.sHtML

cmd >/dev/null 2>&1
来源：http://wap.yfazqb.com/Article/details/ghyinfzrw.sHtML

[R42] 输入重定向
来源：http://www.m.share.sjlbkw.cn/Article/details/gghhofaiu.sHtML

wc -l < a.txt
来源：http://read.share.sjlbkw.cn/Article/details/ghjdleqau.sHtML

[R43] 按名字查找文件
来源：http://mobile.fktsv.cn/Article/details/gtcdyjpmh.sHtML

find . -name "*.log" -type f
来源：http://m.share.bbcook.cn/Article/details/ghyflhceh.sHtML

[R44] 按修改时间查找
来源：http://read.share.yfazqb.com/Article/details/gnqdcdvue.sHtML

find . -mtime -7 -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gwgujlbvp.sHtML

[R45] 批量删除
来源：http://3g.yfazqb.com/Article/details/gamfquejr.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.vehdjk.com/Article/details/gdnoqkdqh.sHtML

[R46] 递归替换文件内容
来源：http://baike.epnwcf.com/Article/details/gpgvqkxnz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.bbcook.cn/Article/details/gcihyavea.sHtML

[R47] sed 单行替换
来源：http://wap.epnwcf.com/Article/details/gbxwveinl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fktsv.cn/Article/details/gvkltenus.sHtML

[R48] awk 取指定列
来源：http://3g.fktsv.cn/Article/details/gydohicxr.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.tarul.cn/Article/details/gfoutitsu.sHtML

[R49] awk 带条件
来源：http://read.share.fktsv.cn/Article/details/gmfklavss.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.yfazqb.com/Article/details/gqfwcipmp.sHtML

[R50] awk 求和
来源：http://wap.tarul.cn/Article/details/gjpfugdxw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gtmjmextx.sHtML

[R51] 排序去重取前几
来源：http://baike.epnwcf.com/Article/details/gpqewihsa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.vehdjk.com/Article/details/gqowcecmd.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/gtgounjzp.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gnixfllcg.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.tarul.cn/Article/details/gphimymru.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.yfazqb.com/Article/details/gvzozrqlr.sHtML

[R54] 比较两个文件
来源：http://baike.bbcook.cn/Article/details/gbotktrpb.sHtML

diff a.txt b.txt
来源：http://read.share.tarul.cn/Article/details/gqezncbvc.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/grsenbyzs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.bbcook.cn/Article/details/gdnscujel.sHtML

[R56] 远程拷贝
来源：http://mobile.tarul.cn/Article/details/gcdypkiac.sHtML

scp file user@host:/path/
来源：http://baike.yfazqb.com/Article/details/ggrpmmawc.sHtML

[R57] 远程执行命令
来源：http://baike.bbcook.cn/Article/details/gnpvgfinc.sHtML

ssh user@host 'uptime'
来源：http://wap.fktsv.cn/Article/details/gesekkcqz.sHtML

[R58] 下载文件
来源：http://baike.bbcook.cn/Article/details/gzwkkxclg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.yfazqb.com/Article/details/gmuxhlezi.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gcglfruua.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.vehdjk.com/Article/details/gsshajmvf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/ggcjriite.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.vehdjk.com/Article/details/gkdhdscoh.sHtML

[R61] 磁盘占用
来源：http://mobile.sjlbkw.cn/Article/details/gyotdomvc.sHtML

df -h;  du -sh *
来源：http://www.share.tarul.cn/Article/details/glritnojb.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/gxcrwymof.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.yfazqb.com/Article/details/gpkyrosvg.sHtML

[R63] 内存与进程
来源：http://m.share.vehdjk.com/Article/details/gznlzezsy.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.sjlbkw.cn/Article/details/gqbwkvypv.sHtML

[R64] 结束进程
来源：http://read.share.tarul.cn/Article/details/gllllliuf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.yfazqb.com/Article/details/gphrjhktb.sHtML

[R65] 查看端口占用
来源：http://m.share.epnwcf.com/Article/details/gihlnkzdg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.sjlbkw.cn/Article/details/gxguaithq.sHtML

[R66] 定时任务
来源：http://www.m.share.yfazqb.com/Article/details/gcqcsqfem.sHtML

crontab -e;  crontab -l
来源：http://3g.fktsv.cn/Article/details/gkbfvjupj.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.vehdjk.com/Article/details/govozottw.sHtML

openssl rand -hex 16
来源：http://3g.epnwcf.com/Article/details/gmifarnni.sHtML

[R68] 计算文件校验值
来源：http://mobile.vehdjk.com/Article/details/getrfhhfu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.bbcook.cn/Article/details/gbomiujhf.sHtML

[R69] 生成随机密码
来源：http://mobile.epnwcf.com/Article/details/gnotrtsoy.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.tarul.cn/Article/details/gradlsanv.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gtwisgbmz.sHtML

date +%s;  date -d @1700000000
来源：http://blog.bbcook.cn/Article/details/gmzvvklvn.sHtML

[R71] 日期格式化
来源：http://blog.vehdjk.com/Article/details/ggifrxaqt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.tarul.cn/Article/details/gctfybjhf.sHtML

[R72] 等待端口就绪
来源：http://baike.bbcook.cn/Article/details/gjczwblpa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/guuzvoage.sHtML

[R73] 分割大日志
来源：http://read.share.sjlbkw.cn/Article/details/gaciickfu.sHtML

split -l 1000 big.log part_
来源：http://www.blog.sjlbkw.cn/Article/details/ghjudtdxa.sHtML

[R74] 批量重命名
来源：http://wap.bbcook.cn/Article/details/gtnnatokv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.vehdjk.com/Article/details/gjrodblmd.sHtML

[R75] 导出环境变量
来源：http://www.blog.yfazqb.com/Article/details/gtkjunagw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.vehdjk.com/Article/details/getmsydwi.sHtML

[R76] 使用临时文件
来源：http://baike.vehdjk.com/Article/details/gmhwtaybb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/guclktrae.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gplsopmtr.sHtML

read -rp "请输入: " ans
来源：http://3g.sjlbkw.cn/Article/details/gggrxpktq.sHtML

[R78] 交互式菜单
来源：http://www.m.share.yfazqb.com/Article/details/gczniqxmo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.tarul.cn/Article/details/gvxxatbfw.sHtML

[R79] 解析命令行选项
来源：http://read.share.tarul.cn/Article/details/gtjupovys.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.bbcook.cn/Article/details/gyevmwtpg.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fktsv.cn/Article/details/gerkrinvd.sHtML

time ./run.sh
来源：http://baike.tarul.cn/Article/details/gfszmmupb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnrheafdf.sHtML

S. C / C++ 专题
来源：http://www.blog.yfazqb.com/Article/details/grlzlvrrx.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzhnnnpvn.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/geklnqvip.sHtML

#include <stdio.h>
来源：http://www.blog.fktsv.cn/Article/details/gcteurmug.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.vehdjk.com/Article/details/gztmphdto.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fktsv.cn/Article/details/gdfvdrlva.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.vehdjk.com/Article/details/ghxabicjk.sHtML

[S03] C：读入整数
来源：http://read.share.tarul.cn/Article/details/gqyxpkirs.sHtML

int x; scanf("%d", &x);
来源：http://mobile.sjlbkw.cn/Article/details/gjnffprno.sHtML

[S04] C：字符串复制
来源：http://blog.tarul.cn/Article/details/gnxkuwrxw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fktsv.cn/Article/details/gaixznzrc.sHtML

[S05] C：字符串长度
来源：http://3g.bbcook.cn/Article/details/gesrsoaio.sHtML

strlen(s)
来源：http://mobile.yfazqb.com/Article/details/gfivfpotl.sHtML

[S06] C：字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gsteccsyn.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fktsv.cn/Article/details/gooovoicu.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.bbcook.cn/Article/details/gdjyqirom.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.sjlbkw.cn/Article/details/gheodueay.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.yfazqb.com/Article/details/gejvcmfvc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.epnwcf.com/Article/details/guqhxmxnm.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.epnwcf.com/Article/details/gqqmkutpi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fktsv.cn/Article/details/ghekwddwd.sHtML

[S10] C：指针与解引用
来源：http://mobile.epnwcf.com/Article/details/ghppicwdm.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.sjlbkw.cn/Article/details/gpkhpssdr.sHtML

[S11] C：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/goeuonnnl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.tarul.cn/Article/details/gonnleqoi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.yfazqb.com/Article/details/ggtjihkvd.sHtML

fclose(f);
来源：http://3g.yfazqb.com/Article/details/gbukarmwu.sHtML

[S12] C：写文件
来源：http://baike.fktsv.cn/Article/details/gjmpklnir.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.tarul.cn/Article/details/gefllgsnl.sHtML

[S13] C：宏定义
来源：http://www.blog.yfazqb.com/Article/details/gmmnlhxrl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/gworxvegc.sHtML

[S14] C：枚举
来源：http://3g.tarul.cn/Article/details/gztpgtjqy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.epnwcf.com/Article/details/ggvayiqck.sHtML

[S15] C：类型转换
来源：http://www.m.share.vehdjk.com/Article/details/grouxgycu.sHtML

(double) a / b
来源：http://3g.tarul.cn/Article/details/gfmqraifl.sHtML

[S16] C：位操作置位
来源：http://baike.fktsv.cn/Article/details/gonrurrcx.sHtML

x |= (1 << 3);
来源：http://www.m.share.fktsv.cn/Article/details/gljucqpmi.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/gfhxvgfnx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.yfazqb.com/Article/details/gyirhddha.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzaqqmer.sHtML

int main(int argc, char **argv)
来源：http://baike.yfazqb.com/Article/details/gwtrtilzr.sHtML

[S19] C：快速排序
来源：http://www.share.vehdjk.com/Article/details/gwmybdigw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/goohllpku.sHtML

[S20] C：二分查找
来源：http://wap.vehdjk.com/Article/details/gnerrtviv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gbhbqeafr.sHtML

[S21] C：字符类别判断
来源：http://read.share.yfazqb.com/Article/details/gnuadsjqx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.vehdjk.com/Article/details/gexrnpavn.sHtML

[S22] C：字符串转数字
来源：http://wap.tarul.cn/Article/details/ggkmxvtda.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.yfazqb.com/Article/details/gujhthojd.sHtML

[S23] C：随机数
来源：http://wap.tarul.cn/Article/details/gqrbuyolz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.vehdjk.com/Article/details/gztvcacdb.sHtML

[S24] C：获取本地时间
来源：http://read.share.fktsv.cn/Article/details/gkeywbuqg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/gkeqxnqeq.sHtML

[S25] C：内存拷贝
来源：http://m.share.fktsv.cn/Article/details/gdpmypiak.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/gifnfntje.sHtML

[S26] C：内存清零
来源：http://baike.epnwcf.com/Article/details/gxbxngeku.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.epnwcf.com/Article/details/ghvauqskr.sHtML

[S27] C：定义常量
来源：http://www.m.share.yfazqb.com/Article/details/gmvverowz.sHtML

const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gmmwjnewp.sHtML

[S28] C：静态变量
来源：http://blog.bbcook.cn/Article/details/gxeknltkp.sHtML

static int counter = 0;
来源：http://www.blog.yfazqb.com/Article/details/gnllqggvp.sHtML

[S29] C：变参函数
来源：http://3g.epnwcf.com/Article/details/gvtffyucz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fktsv.cn/Article/details/guqipujpd.sHtML

[S30] C：头文件保护
来源：http://m.share.epnwcf.com/Article/details/gvrsmmodp.sHtML

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/gfbkwnley.sHtML

#define X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gfylvhehn.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/gqadzpakg.sHtML

[S31] C++：Hello World
来源：http://3g.sjlbkw.cn/Article/details/ghmrgnfrb.sHtML

#include <iostream>
来源：http://wap.tarul.cn/Article/details/glxytoomy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.tarul.cn/Article/details/gaalnmlnj.sHtML

[S32] C++：字符串
来源：http://baike.yfazqb.com/Article/details/glwstlzky.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fktsv.cn/Article/details/gpmolkmlq.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/gbrlodsrz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.sjlbkw.cn/Article/details/gvvlbvish.sHtML

[S34] C++：遍历 vector
来源：http://blog.fktsv.cn/Article/details/girysmtdx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.bbcook.cn/Article/details/gddpmljhs.sHtML

[S35] C++：map
来源：http://wap.vehdjk.com/Article/details/ghqjeqeev.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gwymfllsj.sHtML

[S36] C++：unordered_map
来源：http://blog.fktsv.cn/Article/details/gasehndtv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/grsitdmzw.sHtML

[S37] C++：set
来源：http://baike.epnwcf.com/Article/details/grgqjgcie.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.tarul.cn/Article/details/gaqpzaeyt.sHtML

[S38] C++：排序
来源：http://baike.epnwcf.com/Article/details/gfukaamrh.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.yfazqb.com/Article/details/gcokkqrom.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fktsv.cn/Article/details/grrqqaats.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/gfesdbnme.sHtML

[S40] C++：查找元素
来源：http://3g.fktsv.cn/Article/details/gptcbdepd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.bbcook.cn/Article/details/gvysarzgu.sHtML

[S41] C++：类与构造函数
来源：http://m.share.vehdjk.com/Article/details/gbpyxcrif.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.epnwcf.com/Article/details/glkkbprwl.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgiaplsg.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.epnwcf.com/Article/details/gxnlusacs.sHtML

[S43] C++：智能指针
来源：http://baike.fktsv.cn/Article/details/gcbcmlcav.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.epnwcf.com/Article/details/gmcypqusl.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/gmyhplgni.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.tarul.cn/Article/details/gpsfofdpr.sHtML

[S45] C++：lambda
来源：http://www.share.tarul.cn/Article/details/gqxuxidme.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.yfazqb.com/Article/details/gmfsoigxy.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/grjrwclay.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.epnwcf.com/Article/details/gegbnkwfd.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.bbcook.cn/Article/details/gvwmpmbdu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.epnwcf.com/Article/details/gecsjgyoh.sHtML

[S48] C++：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gsciepcmv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.bbcook.cn/Article/details/gsysiluou.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gixzvnorn.sHtML

[S49] C++：写文件
来源：http://mobile.epnwcf.com/Article/details/ggsnziyxk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.vehdjk.com/Article/details/gbnqaosox.sHtML

[S50] C++：格式化数字
来源：http://m.share.tarul.cn/Article/details/gbxhopqtr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gritjdwtp.sHtML

[S51] C++：显式类型转换
来源：http://blog.bbcook.cn/Article/details/gdejwajio.sHtML

static_cast<double>(a) / b
来源：http://3g.vehdjk.com/Article/details/ggcjlgcoj.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.tarul.cn/Article/details/gfozvhmud.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.yfazqb.com/Article/details/gegwyscpq.sHtML

[S53] C++：移动语义
来源：http://baike.fktsv.cn/Article/details/gkmzqoftk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.bbcook.cn/Article/details/gbvyvmqcd.sHtML

[S54] C++：异常处理
来源：http://blog.tarul.cn/Article/details/gnmelersr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.epnwcf.com/Article/details/gajfsxoao.sHtML

[S55] C++：结构化绑定
来源：http://www.share.sjlbkw.cn/Article/details/gccsprbbk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.vehdjk.com/Article/details/gmliuncht.sHtML

[S56] C++：optional
来源：http://3g.epnwcf.com/Article/details/gpkhgpina.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.epnwcf.com/Article/details/glivecgyr.sHtML

[S57] C++：编译期常量
来源：http://blog.bbcook.cn/Article/details/gpugdupqg.sHtML

constexpr int N = 10;
来源：http://mobile.vehdjk.com/Article/details/gxjmnosaq.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/gfnyekjdb.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.bbcook.cn/Article/details/gztsbtabs.sHtML

[S59] C++：静态断言
来源：http://3g.bbcook.cn/Article/details/gpzpfrnbj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.epnwcf.com/Article/details/gsoaxzlgd.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/gwcimsnpc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gpbrpgpyy.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gksfmdnun.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/gvwcmtslw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gddeeatpg.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gikhidfos.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gtqtdtjik.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gvbnpbzad.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.epnwcf.com/Article/details/ghrxjuoff.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.tarul.cn/Article/details/gifwulpze.sHtML

"值: $b"
来源：http://baike.vehdjk.com/Article/details/grlipdrwu.sHtML

[T04] Kotlin：空安全
来源：http://read.share.tarul.cn/Article/details/gnuoleicj.sHtML

val n: String? = null;  n?.length
来源：http://3g.epnwcf.com/Article/details/govkbbrck.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/gdvszfebk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/gynweoxje.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.vehdjk.com/Article/details/gjxpaedas.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gjchedqeh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gbopskgem.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.yfazqb.com/Article/details/gswzlkiqq.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/gxephtudn.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fktsv.cn/Article/details/giknjqhdw.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.vehdjk.com/Article/details/gnblgaklt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.vehdjk.com/Article/details/gzoslsexg.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gxelluiwr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.epnwcf.com/Article/details/gkbhpeafc.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fktsv.cn/Article/details/gbsfcpnts.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.tarul.cn/Article/details/gigrukekp.sHtML

[T12] Kotlin：解构声明
来源：http://wap.tarul.cn/Article/details/gxubpyyxg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gznuifwbx.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.sjlbkw.cn/Article/details/gtnkgyznp.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.yfazqb.com/Article/details/gxvdoruix.sHtML

[T14] Kotlin：循环
来源：http://read.share.sjlbkw.cn/Article/details/gammyfkjt.sHtML

for (i in 1..10) println(i)
来源：http://blog.bbcook.cn/Article/details/gaxxqotbe.sHtML


<!-- 参考信息 -->