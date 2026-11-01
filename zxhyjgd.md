代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.tarul.cn/Article/details/gpgjyzixe.sHtML

[R16] until 等待条件
来源：http://blog.vehdjk.com/Article/details/gmhehmzsj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gtxtntivw.sHtML

[R17] 数组定义与取值
来源：http://wap.yfazqb.com/Article/details/gkevtqvga.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fktsv.cn/Article/details/glrtnqrlp.sHtML

[R18] 遍历数组
来源：http://m.share.epnwcf.com/Article/details/gbjejbbyd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/gzbznbjes.sHtML

[R19] 数组长度
来源：http://baike.tarul.cn/Article/details/gotcvckbu.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhiafkgv.sHtML

[R20] 关联数组（字典）
来源：http://3g.yfazqb.com/Article/details/gxedrwexw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.bbcook.cn/Article/details/gjdilfuel.sHtML

[R21] 字符串长度
来源：http://read.share.tarul.cn/Article/details/gyrtpamia.sHtML

echo "${#s}"
来源：http://baike.bbcook.cn/Article/details/gozrmgjnk.sHtML

[R22] 截取子串
来源：http://3g.tarul.cn/Article/details/gpdqvgmqt.sHtML

echo "${s:0:5}"
来源：http://m.share.bbcook.cn/Article/details/gnyrsvgml.sHtML

[R23] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gkrfwpxlc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.epnwcf.com/Article/details/gwcbysxtf.sHtML

[R24] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gjqvrllld.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.yfazqb.com/Article/details/glvrnstsu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.vehdjk.com/Article/details/gqupzitwf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcfwnblr.sHtML

[R26] 命令替换
来源：http://baike.bbcook.cn/Article/details/glcrhjzpy.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fktsv.cn/Article/details/gvuamwkmd.sHtML

[R27] 算术展开
来源：http://www.m.share.fktsv.cn/Article/details/gkbaqvzon.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fktsv.cn/Article/details/gkzvoplve.sHtML

[R28] 浮点运算
来源：http://www.m.share.tarul.cn/Article/details/gidmntwiw.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/gthoukqyu.sHtML

[R29] 定义函数
来源：http://wap.bbcook.cn/Article/details/gtbnfioka.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fktsv.cn/Article/details/gjjotfbvf.sHtML

[R30] 函数返回状态码
来源：http://baike.bbcook.cn/Article/details/gpdeyxscm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fktsv.cn/Article/details/gulwkltyt.sHtML

[R31] 局部变量
来源：http://baike.tarul.cn/Article/details/gebmkxruw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gyvhegaje.sHtML

[R32] 参数个数校验
来源：http://www.share.yfazqb.com/Article/details/gaqrhqmst.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gnswdbwzt.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.yfazqb.com/Article/details/gzpnucpwp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.bbcook.cn/Article/details/gmzaychul.sHtML

[R34] 退出时清理
来源：http://www.blog.tarul.cn/Article/details/gdklecdps.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gcadsjmay.sHtML

[R35] 后台执行并等待
来源：http://blog.bbcook.cn/Article/details/gckdntnht.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.vehdjk.com/Article/details/ghkotslut.sHtML

[R36] 并发执行多个任务
来源：http://mobile.yfazqb.com/Article/details/goqkeibrx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.tarul.cn/Article/details/giumtiphc.sHtML

[R37] 把输出赋给变量
来源：http://wap.epnwcf.com/Article/details/gcjtzdpro.sHtML

files=$(ls -1)
来源：http://blog.fktsv.cn/Article/details/gyrjtulic.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gyubkgryk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.vehdjk.com/Article/details/gxbuhbazb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/gakgftynf.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/gmluloouj.sHtML

[R40] 追加写日志
来源：http://blog.epnwcf.com/Article/details/gtzpniwaw.sHtML

echo "log" >> out.log
来源：http://m.share.bbcook.cn/Article/details/gvphppafy.sHtML

[R41] 丢弃输出
来源：http://wap.sjlbkw.cn/Article/details/gmhazpuln.sHtML

cmd >/dev/null 2>&1
来源：http://3g.bbcook.cn/Article/details/gvtmfjief.sHtML

[R42] 输入重定向
来源：http://blog.sjlbkw.cn/Article/details/glpfypkxn.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/gxgigfdqc.sHtML

[R43] 按名字查找文件
来源：http://read.share.bbcook.cn/Article/details/gcaskyrtx.sHtML

find . -name "*.log" -type f
来源：http://mobile.tarul.cn/Article/details/gtslxyyms.sHtML

[R44] 按修改时间查找
来源：http://blog.epnwcf.com/Article/details/grigxrlgz.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/gjpuznniv.sHtML

[R45] 批量删除
来源：http://3g.epnwcf.com/Article/details/gdxoiluoj.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.sjlbkw.cn/Article/details/gbumdsuug.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.tarul.cn/Article/details/gesyxlquz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.yfazqb.com/Article/details/gtntlixui.sHtML

[R47] sed 单行替换
来源：http://mobile.sjlbkw.cn/Article/details/gmukvdrtx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gfavdgybd.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/gadfguazu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gifvofmwv.sHtML

[R49] awk 带条件
来源：http://blog.fktsv.cn/Article/details/gwtrwypdq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.sjlbkw.cn/Article/details/gtnduiggp.sHtML

[R50] awk 求和
来源：http://read.share.yfazqb.com/Article/details/gngtuizph.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.yfazqb.com/Article/details/geycsnxtb.sHtML

[R51] 排序去重取前几
来源：http://3g.tarul.cn/Article/details/ghamnpwhq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.epnwcf.com/Article/details/ggxhijbmj.sHtML

[R52] 统计行数
来源：http://baike.epnwcf.com/Article/details/gbklmcbrz.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gvgqfqyan.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.epnwcf.com/Article/details/gqtvagqgf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.epnwcf.com/Article/details/gdqxexzdp.sHtML

[R54] 比较两个文件
来源：http://3g.tarul.cn/Article/details/gddjbhfue.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/glmizglwy.sHtML

[R55] 压缩与解压
来源：http://read.share.sjlbkw.cn/Article/details/gkhhkvsri.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.sjlbkw.cn/Article/details/gueivouhd.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/gyfjzhxgn.sHtML

scp file user@host:/path/
来源：http://www.m.share.yfazqb.com/Article/details/gfqjjotme.sHtML

[R57] 远程执行命令
来源：http://baike.yfazqb.com/Article/details/gverhjryp.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/gusspfaev.sHtML

[R58] 下载文件
来源：http://baike.epnwcf.com/Article/details/gmgrfnenm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.yfazqb.com/Article/details/gujjwtbrj.sHtML

[R59] 发 POST JSON
来源：http://read.share.bbcook.cn/Article/details/goyagnrmx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.tarul.cn/Article/details/gfheicmjf.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/glqyaledg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.sjlbkw.cn/Article/details/gjzisyjub.sHtML

[R61] 磁盘占用
来源：http://baike.vehdjk.com/Article/details/gjibdncxa.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/glzppqxcb.sHtML

[R62] 找最占空间的文件
来源：http://m.share.sjlbkw.cn/Article/details/gcszwqfib.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.epnwcf.com/Article/details/gpkqdftkv.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/ggykbxtfm.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/gdtmqbchq.sHtML

[R64] 结束进程
来源：http://baike.yfazqb.com/Article/details/gwsgoxkww.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.epnwcf.com/Article/details/gikpjjzyr.sHtML

[R65] 查看端口占用
来源：http://www.blog.bbcook.cn/Article/details/gmooogwrx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.epnwcf.com/Article/details/gkrjobmgp.sHtML

[R66] 定时任务
来源：http://blog.yfazqb.com/Article/details/gefoylsdf.sHtML

crontab -e;  crontab -l
来源：http://baike.sjlbkw.cn/Article/details/gwfcbozec.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.bbcook.cn/Article/details/ggzwddsmq.sHtML

openssl rand -hex 16
来源：http://m.share.sjlbkw.cn/Article/details/garrhnuuv.sHtML

[R68] 计算文件校验值
来源：http://m.share.vehdjk.com/Article/details/gzdpadavk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.bbcook.cn/Article/details/gjvgujsjl.sHtML

[R69] 生成随机密码
来源：http://www.blog.sjlbkw.cn/Article/details/gcnxzuebn.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.tarul.cn/Article/details/gdlhouvkv.sHtML

[R70] 时间戳与互转
来源：http://m.share.epnwcf.com/Article/details/gutjyjzzq.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fktsv.cn/Article/details/glxvyqaap.sHtML

[R71] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/gotghctge.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.vehdjk.com/Article/details/gkojhsbtm.sHtML

[R72] 等待端口就绪
来源：http://wap.vehdjk.com/Article/details/gxzzkxphg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/geibinagp.sHtML

[R73] 分割大日志
来源：http://baike.epnwcf.com/Article/details/gkozpjymb.sHtML

split -l 1000 big.log part_
来源：http://www.share.sjlbkw.cn/Article/details/grldhxwut.sHtML

[R74] 批量重命名
来源：http://3g.tarul.cn/Article/details/gaxechqhe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.yfazqb.com/Article/details/gguukjegh.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fktsv.cn/Article/details/ggougnjle.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.tarul.cn/Article/details/gfkbpnbdb.sHtML

[R76] 使用临时文件
来源：http://m.share.bbcook.cn/Article/details/ggggrcpms.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.bbcook.cn/Article/details/gvwxoeolb.sHtML

[R77] 读取用户输入
来源：http://www.m.share.vehdjk.com/Article/details/getemqxqq.sHtML

read -rp "请输入: " ans
来源：http://read.share.sjlbkw.cn/Article/details/ggwyeqaby.sHtML

[R78] 交互式菜单
来源：http://www.share.fktsv.cn/Article/details/gzdrmbjbt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.vehdjk.com/Article/details/gdlkqanmk.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fktsv.cn/Article/details/gdykxbrim.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gblffspax.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.vehdjk.com/Article/details/ghrzfxhru.sHtML

time ./run.sh
来源：http://wap.fktsv.cn/Article/details/gcissmelw.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gjcggtulj.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/gpebikwri.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grsirtfef.sHtML

[S01] C：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gwljitmod.sHtML

#include <stdio.h>
来源：http://wap.bbcook.cn/Article/details/gdvajvndg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/gcvmohfoc.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.epnwcf.com/Article/details/gdllrjbwm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.sjlbkw.cn/Article/details/gseufrzus.sHtML

[S03] C：读入整数
来源：http://blog.sjlbkw.cn/Article/details/gzpkjbqvv.sHtML

int x; scanf("%d", &x);
来源：http://mobile.yfazqb.com/Article/details/gbdbrpmuo.sHtML

[S04] C：字符串复制
来源：http://blog.vehdjk.com/Article/details/gxpjlxdaf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gaxrksmyk.sHtML

[S05] C：字符串长度
来源：http://blog.vehdjk.com/Article/details/gwnqmqsot.sHtML

strlen(s)
来源：http://baike.tarul.cn/Article/details/gxkzjmrgo.sHtML

[S06] C：字符串比较
来源：http://baike.fktsv.cn/Article/details/gicniokad.sHtML

strcmp(a, b) == 0
来源：http://read.share.tarul.cn/Article/details/gfhmbaods.sHtML

[S07] C：数组遍历求和
来源：http://baike.vehdjk.com/Article/details/gpwshsovt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/gxjjhxtzj.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fktsv.cn/Article/details/ggcbhhvpe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.epnwcf.com/Article/details/guorgmfff.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fktsv.cn/Article/details/gclvsuwbe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/gnqyyxiqd.sHtML

[S10] C：指针与解引用
来源：http://read.share.vehdjk.com/Article/details/ggycgnkge.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fktsv.cn/Article/details/gyalmilcb.sHtML

[S11] C：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/guyvhhogi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.sjlbkw.cn/Article/details/gdekyoyqm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/glpvcxxhb.sHtML

fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/gkghwenbb.sHtML

[S12] C：写文件
来源：http://baike.yfazqb.com/Article/details/gdeesckob.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.tarul.cn/Article/details/gicdhihjw.sHtML

[S13] C：宏定义
来源：http://www.share.bbcook.cn/Article/details/gjpwexgzi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.epnwcf.com/Article/details/gohqaiuoi.sHtML

[S14] C：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gvoikuvns.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.bbcook.cn/Article/details/grehhltmc.sHtML

[S15] C：类型转换
来源：http://read.share.tarul.cn/Article/details/gblvdxwvs.sHtML

(double) a / b
来源：http://baike.sjlbkw.cn/Article/details/gumdrsxvw.sHtML

[S16] C：位操作置位
来源：http://m.share.vehdjk.com/Article/details/gjwciwtyf.sHtML

x |= (1 << 3);
来源：http://baike.fktsv.cn/Article/details/ghldfxlvm.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gdxxxcgac.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/gmvwhycwy.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfezvvst.sHtML

int main(int argc, char **argv)
来源：http://wap.vehdjk.com/Article/details/gwlaxdmmg.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/gyjeqzrdw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gdlwnmeml.sHtML

[S20] C：二分查找
来源：http://www.m.share.bbcook.cn/Article/details/gjcityhjd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gkynlfpek.sHtML

[S21] C：字符类别判断
来源：http://blog.bbcook.cn/Article/details/gjufwehge.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.epnwcf.com/Article/details/gqobracee.sHtML

[S22] C：字符串转数字
来源：http://baike.epnwcf.com/Article/details/ghvyjobwu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.sjlbkw.cn/Article/details/gjjrqjtnc.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/gbnjxgnpi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.bbcook.cn/Article/details/gqrsauqdf.sHtML

[S24] C：获取本地时间
来源：http://www.share.fktsv.cn/Article/details/gpexpwnnt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/gbvqlyhkc.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/gacbtcqhq.sHtML

memcpy(dst, src, n);
来源：http://3g.bbcook.cn/Article/details/gvqtnulvw.sHtML

[S26] C：内存清零
来源：http://3g.tarul.cn/Article/details/gddpshler.sHtML

memset(a, 0, sizeof a);
来源：http://blog.epnwcf.com/Article/details/gabtbtpwz.sHtML

[S27] C：定义常量
来源：http://www.share.tarul.cn/Article/details/gbwtehnhi.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gkxkutskn.sHtML

[S28] C：静态变量
来源：http://read.share.sjlbkw.cn/Article/details/gpafzrqvm.sHtML

static int counter = 0;
来源：http://baike.yfazqb.com/Article/details/ggeditvco.sHtML

[S29] C：变参函数
来源：http://wap.tarul.cn/Article/details/gkazfjiim.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.tarul.cn/Article/details/gdbavbife.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gacowgjed.sHtML

#ifndef X_H
来源：http://m.share.sjlbkw.cn/Article/details/gjqfcfvnw.sHtML

#define X_H
来源：http://mobile.bbcook.cn/Article/details/gpdzhovgq.sHtML

#endif
来源：http://mobile.vehdjk.com/Article/details/ggykougao.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/ggfisnnif.sHtML

#include <iostream>
来源：http://read.share.tarul.cn/Article/details/goaugewoi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.vehdjk.com/Article/details/gdzxsbwgc.sHtML

[S32] C++：字符串
来源：http://www.share.fktsv.cn/Article/details/gwzwpnbxg.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.tarul.cn/Article/details/gtwjhqbon.sHtML

[S33] C++：vector 增删
来源：http://baike.tarul.cn/Article/details/gvjzywaqv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.tarul.cn/Article/details/grgmmrdow.sHtML

[S34] C++：遍历 vector
来源：http://baike.vehdjk.com/Article/details/gniesrctk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.vehdjk.com/Article/details/gipnjcfbv.sHtML

[S35] C++：map
来源：http://www.m.share.yfazqb.com/Article/details/gecebzgyd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gpygxxmmw.sHtML

[S36] C++：unordered_map
来源：http://read.share.sjlbkw.cn/Article/details/gaefwcxon.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/glgdsdslq.sHtML

[S37] C++：set
来源：http://www.m.share.bbcook.cn/Article/details/gdcwetntf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/gsjzuodod.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gdmqubuto.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.yfazqb.com/Article/details/gnzishefq.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.sjlbkw.cn/Article/details/gfehakopi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.epnwcf.com/Article/details/gzenxlbqy.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/gwqunalve.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.tarul.cn/Article/details/gwmbrxrfh.sHtML

[S41] C++：类与构造函数
来源：http://www.share.bbcook.cn/Article/details/grconojsx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.tarul.cn/Article/details/glbouxgxn.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.epnwcf.com/Article/details/giaacvrvi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.tarul.cn/Article/details/grfikvzam.sHtML

[S43] C++：智能指针
来源：http://www.blog.vehdjk.com/Article/details/gvgscygsq.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.sjlbkw.cn/Article/details/glnhjdrsy.sHtML

[S44] C++：引用传参
来源：http://www.m.share.bbcook.cn/Article/details/giouslgoj.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.vehdjk.com/Article/details/gfjfjgpqp.sHtML

[S45] C++：lambda
来源：http://www.share.sjlbkw.cn/Article/details/gevqyvsbx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.epnwcf.com/Article/details/gdeakkbyr.sHtML

[S46] C++：函数模板
来源：http://m.share.fktsv.cn/Article/details/gnfoufvol.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.bbcook.cn/Article/details/gqhoankji.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.yfazqb.com/Article/details/ggqhdnawa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.vehdjk.com/Article/details/grliylfli.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/ghshtxosa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.sjlbkw.cn/Article/details/gcgizemxn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/ggxblheua.sHtML

[S49] C++：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gzbgpulio.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/ghtcdljhw.sHtML

[S50] C++：格式化数字
来源：http://read.share.fktsv.cn/Article/details/ggsuegaqq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/gejslhokg.sHtML

[S51] C++：显式类型转换
来源：http://m.share.bbcook.cn/Article/details/gcwpklrde.sHtML

static_cast<double>(a) / b
来源：http://mobile.sjlbkw.cn/Article/details/gwpxvbado.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.sjlbkw.cn/Article/details/goqxgsmfu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.epnwcf.com/Article/details/gaokgksjf.sHtML

[S53] C++：移动语义
来源：http://wap.sjlbkw.cn/Article/details/ggoeqlath.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.vehdjk.com/Article/details/gbxqtsavy.sHtML

[S54] C++：异常处理
来源：http://mobile.epnwcf.com/Article/details/gwlxmbdop.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.tarul.cn/Article/details/gppsiguae.sHtML

[S55] C++：结构化绑定
来源：http://baike.tarul.cn/Article/details/gzrpfuqyq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.yfazqb.com/Article/details/gpjxorhhz.sHtML

[S56] C++：optional
来源：http://3g.vehdjk.com/Article/details/gidfcmuan.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glmzfdwsh.sHtML

[S57] C++：编译期常量
来源：http://wap.yfazqb.com/Article/details/glfcasmik.sHtML

constexpr int N = 10;
来源：http://m.share.fktsv.cn/Article/details/gkwmspjep.sHtML

[S58] C++：命名空间
来源：http://mobile.vehdjk.com/Article/details/gulskorae.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.bbcook.cn/Article/details/geuwvzpze.sHtML

[S59] C++：静态断言
来源：http://read.share.bbcook.cn/Article/details/gusccaugq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.sjlbkw.cn/Article/details/gepejzyic.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.bbcook.cn/Article/details/gnqearnxw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gnmsejmai.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gjhadgzql.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.yfazqb.com/Article/details/gmksuryev.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gysctmfbz.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fktsv.cn/Article/details/gvvocuegv.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gfgjywnro.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gcqmngalf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/glblsmtnd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.bbcook.cn/Article/details/ggdxqhyur.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/giwbwjalh.sHtML

[T04] Kotlin：空安全
来源：http://m.share.sjlbkw.cn/Article/details/gtdwtpius.sHtML

val n: String? = null;  n?.length
来源：http://www.share.bbcook.cn/Article/details/giqbymiln.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gziyricbf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.epnwcf.com/Article/details/gzruqmsaw.sHtML

[T06] Kotlin：集合映射
来源：http://wap.bbcook.cn/Article/details/gvhorifau.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gflvjndql.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.yfazqb.com/Article/details/gktdhsrbi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.yfazqb.com/Article/details/gwgtsqrrg.sHtML

[T08] Kotlin：数据类
来源：http://baike.epnwcf.com/Article/details/ghrilkdws.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.bbcook.cn/Article/details/govawvflx.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.yfazqb.com/Article/details/gxrnxkvkg.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.tarul.cn/Article/details/grqxdbuvk.sHtML

[T10] Kotlin：默认参数
来源：http://baike.tarul.cn/Article/details/gxyqkdslb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.epnwcf.com/Article/details/gpohbunlb.sHtML

[T11] Kotlin：协程
来源：http://baike.vehdjk.com/Article/details/gqxpyagux.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.yfazqb.com/Article/details/gzsuebkfl.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fktsv.cn/Article/details/gflzorptx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/ggtscnhjt.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.bbcook.cn/Article/details/ghuaxpzeq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.tarul.cn/Article/details/gwvizzzdy.sHtML

[T14] Kotlin：循环
来源：http://www.blog.vehdjk.com/Article/details/gynimlsae.sHtML

for (i in 1..10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gpxbugaex.sHtML

[T15] Kotlin：接口
来源：http://www.blog.sjlbkw.cn/Article/details/gqtpidzby.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.bbcook.cn/Article/details/gadfhgick.sHtML

[T16] Swift：Hello World
来源：http://3g.fktsv.cn/Article/details/gthbwbsrh.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/grcyxohxa.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.sjlbkw.cn/Article/details/gcexmkeas.sHtML

var a = 1;  let b = 2
来源：http://read.share.fktsv.cn/Article/details/gmrreacxu.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/gnrdmpvpy.sHtML

"值: \(b)"
来源：http://mobile.epnwcf.com/Article/details/gmmatwzwu.sHtML


<!-- 参考信息 -->