代发 wailian999

esac
来源：http://www.share.vehdjk.com/Article/details/giaxztpui.sHtML

[R12] for 遍历文件
来源：http://blog.sjlbkw.cn/Article/details/gnibtkzzv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.epnwcf.com/Article/details/gnsjynres.sHtML

[R13] for 计数循环
来源：http://baike.epnwcf.com/Article/details/ghkrwmvyg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gwnunnpxp.sHtML

[R14] C 风格 for
来源：http://wap.yfazqb.com/Article/details/gqwqeoeaf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gongittac.sHtML

[R15] while 逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gbaygnarg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.sjlbkw.cn/Article/details/gdqfzqbii.sHtML

[R16] until 等待条件
来源：http://3g.sjlbkw.cn/Article/details/ggubehciv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gmwhfuprn.sHtML

[R17] 数组定义与取值
来源：http://blog.sjlbkw.cn/Article/details/gmxufikoz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.sjlbkw.cn/Article/details/gqrlrnsyr.sHtML

[R18] 遍历数组
来源：http://blog.epnwcf.com/Article/details/gmpdygfcb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.epnwcf.com/Article/details/gsxfshpgd.sHtML

[R19] 数组长度
来源：http://blog.fktsv.cn/Article/details/gqagchbzw.sHtML

echo "${#arr[@]}"
来源：http://read.share.vehdjk.com/Article/details/gkvfytekd.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fktsv.cn/Article/details/gjxwywnee.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.vehdjk.com/Article/details/guahezujp.sHtML

[R21] 字符串长度
来源：http://m.share.bbcook.cn/Article/details/gfpnyqkop.sHtML

echo "${#s}"
来源：http://3g.sjlbkw.cn/Article/details/gqevifxme.sHtML

[R22] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gxkzixjki.sHtML

echo "${s:0:5}"
来源：http://mobile.vehdjk.com/Article/details/gxuzcttfg.sHtML

[R23] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gtxbvbant.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.vehdjk.com/Article/details/gbuclekau.sHtML

[R24] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gzyswxrqi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.yfazqb.com/Article/details/gpbqhakpm.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.epnwcf.com/Article/details/gehcbepkd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fktsv.cn/Article/details/gfobovdex.sHtML

[R26] 命令替换
来源：http://m.share.bbcook.cn/Article/details/gvehqfdzn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.tarul.cn/Article/details/gpvjaosuh.sHtML

[R27] 算术展开
来源：http://3g.bbcook.cn/Article/details/gscavigce.sHtML

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/gqwpagsss.sHtML

[R28] 浮点运算
来源：http://baike.tarul.cn/Article/details/ggggmheur.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.bbcook.cn/Article/details/ghzvgepre.sHtML

[R29] 定义函数
来源：http://blog.epnwcf.com/Article/details/gatpliqqx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.yfazqb.com/Article/details/gwoxgnqvq.sHtML

[R30] 函数返回状态码
来源：http://wap.bbcook.cn/Article/details/gxafgvpei.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.bbcook.cn/Article/details/gdheggajk.sHtML

[R31] 局部变量
来源：http://wap.bbcook.cn/Article/details/gmtxqccvm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.vehdjk.com/Article/details/gkxfryhch.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/gtqlfcxmt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/gqkbrzbof.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.vehdjk.com/Article/details/gvsxxxzga.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.yfazqb.com/Article/details/gpvbonrcc.sHtML

[R34] 退出时清理
来源：http://www.m.share.epnwcf.com/Article/details/gciktaayf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.vehdjk.com/Article/details/ggcukyxjn.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.bbcook.cn/Article/details/gfvoatbqv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fktsv.cn/Article/details/gyyqjtbmd.sHtML

[R36] 并发执行多个任务
来源：http://baike.vehdjk.com/Article/details/gfuqiutxa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.tarul.cn/Article/details/gihndoqre.sHtML

[R37] 把输出赋给变量
来源：http://3g.sjlbkw.cn/Article/details/ggywtvfqo.sHtML

files=$(ls -1)
来源：http://mobile.sjlbkw.cn/Article/details/grrbxidwz.sHtML

[R38] 管道串联
来源：http://blog.tarul.cn/Article/details/giolmrtmr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.yfazqb.com/Article/details/gliwcbtzc.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/gggedcgjo.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gmjpfwwjn.sHtML

[R40] 追加写日志
来源：http://wap.fktsv.cn/Article/details/gzsvwfukz.sHtML

echo "log" >> out.log
来源：http://read.share.bbcook.cn/Article/details/gcsbzrdam.sHtML

[R41] 丢弃输出
来源：http://baike.vehdjk.com/Article/details/giajxguvq.sHtML

cmd >/dev/null 2>&1
来源：http://blog.sjlbkw.cn/Article/details/gxwpydhcx.sHtML

[R42] 输入重定向
来源：http://baike.fktsv.cn/Article/details/gnxkpeeyr.sHtML

wc -l < a.txt
来源：http://www.blog.vehdjk.com/Article/details/gyvchwicd.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gxgnjfdxa.sHtML

find . -name "*.log" -type f
来源：http://www.share.vehdjk.com/Article/details/gmbmdhskx.sHtML

[R44] 按修改时间查找
来源：http://blog.tarul.cn/Article/details/gjxgbiqci.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/geetxhqwu.sHtML

[R45] 批量删除
来源：http://m.share.epnwcf.com/Article/details/gmmrbgczy.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fktsv.cn/Article/details/gmejdbzbv.sHtML

[R46] 递归替换文件内容
来源：http://baike.bbcook.cn/Article/details/gmadupdvs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.yfazqb.com/Article/details/gegiezlxh.sHtML

[R47] sed 单行替换
来源：http://m.share.epnwcf.com/Article/details/gsisykzca.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.vehdjk.com/Article/details/gegzodlko.sHtML

[R48] awk 取指定列
来源：http://www.blog.vehdjk.com/Article/details/glthgpsam.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/gynzzjgnw.sHtML

[R49] awk 带条件
来源：http://mobile.sjlbkw.cn/Article/details/gyfqnnuif.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.tarul.cn/Article/details/gyuowunju.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gwislzkaa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gstfpflkh.sHtML

[R51] 排序去重取前几
来源：http://3g.tarul.cn/Article/details/gkhyiwudn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.tarul.cn/Article/details/gddnyqwds.sHtML

[R52] 统计行数
来源：http://www.blog.epnwcf.com/Article/details/guwbugxkn.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/gyfvoitqe.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/gafuvukwv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.sjlbkw.cn/Article/details/grkucwoch.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/gkfktropa.sHtML

diff a.txt b.txt
来源：http://blog.vehdjk.com/Article/details/ghoeclgwm.sHtML

[R55] 压缩与解压
来源：http://3g.epnwcf.com/Article/details/gefgtxuit.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.sjlbkw.cn/Article/details/gwcemsnoc.sHtML

[R56] 远程拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gxfdoqjlx.sHtML

scp file user@host:/path/
来源：http://www.blog.yfazqb.com/Article/details/grwwxmuia.sHtML

[R57] 远程执行命令
来源：http://baike.epnwcf.com/Article/details/grsoskils.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/gnonqitwd.sHtML

[R58] 下载文件
来源：http://3g.bbcook.cn/Article/details/guqndgulf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.epnwcf.com/Article/details/galdchjdm.sHtML

[R59] 发 POST JSON
来源：http://m.share.bbcook.cn/Article/details/gypqqpqnv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.tarul.cn/Article/details/gkmbejzmf.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/govwghufn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/gdvkmlnhb.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/govhmjzsz.sHtML

df -h;  du -sh *
来源：http://www.blog.fktsv.cn/Article/details/ghobjwfru.sHtML

[R62] 找最占空间的文件
来源：http://blog.bbcook.cn/Article/details/guhwwwbsa.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.vehdjk.com/Article/details/gstbzyxvo.sHtML

[R63] 内存与进程
来源：http://www.blog.yfazqb.com/Article/details/gkqibvbzo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.sjlbkw.cn/Article/details/gjtbbgwvk.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gwlpbuznx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.yfazqb.com/Article/details/gfvvkzeqb.sHtML

[R65] 查看端口占用
来源：http://3g.tarul.cn/Article/details/ghnzlokfa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.epnwcf.com/Article/details/gnsnbpaja.sHtML

[R66] 定时任务
来源：http://wap.fktsv.cn/Article/details/grwtkrvbs.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/ghehdtcdv.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fktsv.cn/Article/details/grgakpnju.sHtML

openssl rand -hex 16
来源：http://blog.sjlbkw.cn/Article/details/gwffrmvxd.sHtML

[R68] 计算文件校验值
来源：http://www.share.vehdjk.com/Article/details/gonncxclq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.vehdjk.com/Article/details/guwhadmgp.sHtML

[R69] 生成随机密码
来源：http://baike.epnwcf.com/Article/details/gnurxgwqh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.epnwcf.com/Article/details/goumpisug.sHtML

[R70] 时间戳与互转
来源：http://mobile.vehdjk.com/Article/details/gkjthxpux.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.vehdjk.com/Article/details/gyocihnhc.sHtML

[R71] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gxpqsdgie.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fktsv.cn/Article/details/guaidbwzt.sHtML

[R72] 等待端口就绪
来源：http://mobile.tarul.cn/Article/details/gfnrvcsiq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gucydygle.sHtML

[R73] 分割大日志
来源：http://wap.vehdjk.com/Article/details/gatkiuzef.sHtML

split -l 1000 big.log part_
来源：http://baike.fktsv.cn/Article/details/glqffbmzk.sHtML

[R74] 批量重命名
来源：http://m.share.yfazqb.com/Article/details/gsosxwoev.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.tarul.cn/Article/details/gfislmota.sHtML

[R75] 导出环境变量
来源：http://blog.tarul.cn/Article/details/gmbovtzqj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.sjlbkw.cn/Article/details/gxrjwxjtw.sHtML

[R76] 使用临时文件
来源：http://m.share.epnwcf.com/Article/details/gwnjrtfws.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gisewptbv.sHtML

[R77] 读取用户输入
来源：http://blog.yfazqb.com/Article/details/gnbhixrho.sHtML

read -rp "请输入: " ans
来源：http://baike.vehdjk.com/Article/details/gzwudwotz.sHtML

[R78] 交互式菜单
来源：http://mobile.epnwcf.com/Article/details/gtyvlkptm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.bbcook.cn/Article/details/gktljsozy.sHtML

[R79] 解析命令行选项
来源：http://www.share.tarul.cn/Article/details/gekovtgfz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/gubsiyqor.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.epnwcf.com/Article/details/gabchuryg.sHtML

time ./run.sh
来源：http://www.blog.fktsv.cn/Article/details/gvwgcwxxy.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gaykrlhlo.sHtML

S. C / C++ 专题
来源：http://blog.fktsv.cn/Article/details/gfdhiwcki.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwvlltdbe.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/gvcmcqktr.sHtML

#include <stdio.h>
来源：http://www.share.epnwcf.com/Article/details/gzmonaiiy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.vehdjk.com/Article/details/gdvscasbs.sHtML

[S02] C：变量与格式化输出
来源：http://baike.tarul.cn/Article/details/gtzdoutnk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.yfazqb.com/Article/details/gvuhioxjq.sHtML

[S03] C：读入整数
来源：http://read.share.epnwcf.com/Article/details/gnyxcrgro.sHtML

int x; scanf("%d", &x);
来源：http://www.share.sjlbkw.cn/Article/details/glomcdjvs.sHtML

[S04] C：字符串复制
来源：http://m.share.vehdjk.com/Article/details/gqchhilfn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/grqhbcbii.sHtML

[S05] C：字符串长度
来源：http://mobile.bbcook.cn/Article/details/gxucahdav.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/gyaeeflqr.sHtML

[S06] C：字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gqmesdjkb.sHtML

strcmp(a, b) == 0
来源：http://read.share.yfazqb.com/Article/details/ghbyrfrwe.sHtML

[S07] C：数组遍历求和
来源：http://mobile.vehdjk.com/Article/details/ghufmwojv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/gmzohiamd.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.bbcook.cn/Article/details/gdqmbgkfa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.bbcook.cn/Article/details/gssjvskmu.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fktsv.cn/Article/details/gjquyyynf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fktsv.cn/Article/details/gzcwkywze.sHtML

[S10] C：指针与解引用
来源：http://wap.tarul.cn/Article/details/gzwmpprum.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.bbcook.cn/Article/details/gtssstsqm.sHtML

[S11] C：逐行读文件
来源：http://wap.tarul.cn/Article/details/gweecewes.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.sjlbkw.cn/Article/details/gxoqosshc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gmlxchdep.sHtML

fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gfexoswln.sHtML

[S12] C：写文件
来源：http://3g.yfazqb.com/Article/details/gflsnvvsl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.yfazqb.com/Article/details/gicfpqudo.sHtML

[S13] C：宏定义
来源：http://www.blog.sjlbkw.cn/Article/details/gzgfvntyn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.sjlbkw.cn/Article/details/gstmwyvsi.sHtML

[S14] C：枚举
来源：http://mobile.sjlbkw.cn/Article/details/ggbvsxbzi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.vehdjk.com/Article/details/gechjqeej.sHtML

[S15] C：类型转换
来源：http://blog.yfazqb.com/Article/details/gsqjpqvxg.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/gbtcxoenz.sHtML

[S16] C：位操作置位
来源：http://read.share.sjlbkw.cn/Article/details/gmxcjonmt.sHtML

x |= (1 << 3);
来源：http://baike.sjlbkw.cn/Article/details/goqmcrrwg.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gpsxdkoas.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.tarul.cn/Article/details/gohclzrcq.sHtML

[S18] C：命令行参数
来源：http://mobile.vehdjk.com/Article/details/gqlcfangu.sHtML

int main(int argc, char **argv)
来源：http://mobile.yfazqb.com/Article/details/gheqsnuuf.sHtML

[S19] C：快速排序
来源：http://www.share.sjlbkw.cn/Article/details/gezckxatq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/gnyjstasr.sHtML

[S20] C：二分查找
来源：http://read.share.fktsv.cn/Article/details/gijgfjfvb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gvlefpeak.sHtML

[S21] C：字符类别判断
来源：http://blog.fktsv.cn/Article/details/gyiursdqy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.vehdjk.com/Article/details/gxqvtrvki.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/gkixmghpj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/ghxecxdgt.sHtML

[S23] C：随机数
来源：http://mobile.epnwcf.com/Article/details/gpqyunsty.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.bbcook.cn/Article/details/grvoknhrf.sHtML

[S24] C：获取本地时间
来源：http://baike.fktsv.cn/Article/details/gcqbybfzb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.tarul.cn/Article/details/gusjxmael.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gskjwekqg.sHtML

memcpy(dst, src, n);
来源：http://wap.sjlbkw.cn/Article/details/gpblvlvhr.sHtML

[S26] C：内存清零
来源：http://www.share.epnwcf.com/Article/details/guvpyogur.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.epnwcf.com/Article/details/gfvpbloxw.sHtML

[S27] C：定义常量
来源：http://baike.sjlbkw.cn/Article/details/gctvrccqy.sHtML

const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/goawbvrbx.sHtML

[S28] C：静态变量
来源：http://baike.sjlbkw.cn/Article/details/gjewojdlr.sHtML

static int counter = 0;
来源：http://baike.bbcook.cn/Article/details/glbslecnx.sHtML

[S29] C：变参函数
来源：http://www.share.sjlbkw.cn/Article/details/gqllyudiq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/gwnbktskj.sHtML

[S30] C：头文件保护
来源：http://www.blog.fktsv.cn/Article/details/gpeiknbve.sHtML

#ifndef X_H
来源：http://mobile.yfazqb.com/Article/details/gvpzcmyvm.sHtML

#define X_H
来源：http://www.share.epnwcf.com/Article/details/gzazekxuv.sHtML

#endif
来源：http://wap.vehdjk.com/Article/details/ginrymqyn.sHtML

[S31] C++：Hello World
来源：http://mobile.bbcook.cn/Article/details/gojtxzpun.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gjwvjmiun.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.epnwcf.com/Article/details/gxlxpiwgg.sHtML

[S32] C++：字符串
来源：http://baike.yfazqb.com/Article/details/gujwjvaud.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.sjlbkw.cn/Article/details/glmogiloc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.vehdjk.com/Article/details/gonxiahax.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/gaxzwzwri.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/gttfbkxek.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fktsv.cn/Article/details/gstghnuqp.sHtML

[S35] C++：map
来源：http://m.share.epnwcf.com/Article/details/gcfpcdiyv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/ggzjrefri.sHtML

[S36] C++：unordered_map
来源：http://3g.sjlbkw.cn/Article/details/gtmjslssh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gagbhkxfy.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/gqyvkjxwc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fktsv.cn/Article/details/gfabdqdqu.sHtML

[S38] C++：排序
来源：http://wap.vehdjk.com/Article/details/gzuualgdl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.bbcook.cn/Article/details/ggjfpdiza.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gfjisxvdv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/gkawnqdnu.sHtML

[S40] C++：查找元素
来源：http://mobile.sjlbkw.cn/Article/details/gyygszmnm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.tarul.cn/Article/details/gqulxvnvz.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fktsv.cn/Article/details/ggiyhxcay.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.vehdjk.com/Article/details/gxfhxfugg.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.tarul.cn/Article/details/gycrrtwhd.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.yfazqb.com/Article/details/gardmjgmz.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gfxotuioa.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fktsv.cn/Article/details/gasgowjem.sHtML

[S44] C++：引用传参
来源：http://baike.tarul.cn/Article/details/gsxhnqjmk.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/gwlfqlnvz.sHtML

[S45] C++：lambda
来源：http://www.share.epnwcf.com/Article/details/gtsqymqhp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.bbcook.cn/Article/details/gmmgdrpmr.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/glxmkwfws.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.yfazqb.com/Article/details/gmntzyljf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.tarul.cn/Article/details/gkdnyszvc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.yfazqb.com/Article/details/gnjanvvay.sHtML

[S48] C++：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gvzfpcyuz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.epnwcf.com/Article/details/gtjjauwrp.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.epnwcf.com/Article/details/grpiisclm.sHtML

[S49] C++：写文件
来源：http://3g.tarul.cn/Article/details/grotutjlq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.sjlbkw.cn/Article/details/gxfcywfyo.sHtML

[S50] C++：格式化数字
来源：http://www.share.fktsv.cn/Article/details/gnaiqdoba.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gkqkulxba.sHtML

[S51] C++：显式类型转换
来源：http://blog.epnwcf.com/Article/details/gsiehsfvr.sHtML

static_cast<double>(a) / b
来源：http://m.share.yfazqb.com/Article/details/gvxqezubq.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.tarul.cn/Article/details/gxtzjqeuw.sHtML

int size() const noexcept { return n_; }
来源：http://3g.tarul.cn/Article/details/gfwgpmgjo.sHtML

[S53] C++：移动语义
来源：http://read.share.vehdjk.com/Article/details/gecjgvobi.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.vehdjk.com/Article/details/gvsurhlje.sHtML

[S54] C++：异常处理
来源：http://3g.fktsv.cn/Article/details/grgirjggz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.vehdjk.com/Article/details/ghmgqnbtz.sHtML

[S55] C++：结构化绑定
来源：http://www.share.tarul.cn/Article/details/gtqdodzyc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.yfazqb.com/Article/details/gvzyvmbrz.sHtML

[S56] C++：optional
来源：http://blog.epnwcf.com/Article/details/goalkrnkg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.bbcook.cn/Article/details/gfttxomyj.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/giflzwybw.sHtML

constexpr int N = 10;
来源：http://www.share.yfazqb.com/Article/details/glrwzkrmy.sHtML

[S58] C++：命名空间
来源：http://mobile.vehdjk.com/Article/details/gjxcwxbjk.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/gdmkdulbd.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/gjlypfgsy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.epnwcf.com/Article/details/gfxehabhe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.vehdjk.com/Article/details/gvlkobbmq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gaqhamzcw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/grtscgsyx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/gtvffsanz.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gkebrmirs.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fktsv.cn/Article/details/gsaqynlyh.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gzrrurjbz.sHtML

[T02] Kotlin：变量
来源：http://m.share.vehdjk.com/Article/details/girrikvlw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fktsv.cn/Article/details/gqhvsqzhb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzoqqjfq.sHtML

"值: $b"
来源：http://mobile.fktsv.cn/Article/details/gyugierhx.sHtML

[T04] Kotlin：空安全
来源：http://3g.vehdjk.com/Article/details/ghauodaqg.sHtML

val n: String? = null;  n?.length
来源：http://mobile.sjlbkw.cn/Article/details/gyzczfqvv.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/gjfeyyewh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/gyrqjgrgc.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.yfazqb.com/Article/details/glidzbnyg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fktsv.cn/Article/details/gtzdluhgi.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/gehothfsp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.bbcook.cn/Article/details/gewlsydvh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.tarul.cn/Article/details/grndkkvrz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.bbcook.cn/Article/details/gxgngiskz.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.yfazqb.com/Article/details/gzynceegn.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.sjlbkw.cn/Article/details/gvmmhlcjx.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.epnwcf.com/Article/details/ghmijlprg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.vehdjk.com/Article/details/gwmuotaqr.sHtML

[T11] Kotlin：协程
来源：http://baike.epnwcf.com/Article/details/gglswvzoy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.bbcook.cn/Article/details/godkjzaun.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/grhixmdkb.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.epnwcf.com/Article/details/gtkcfxiyu.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fktsv.cn/Article/details/gcukxnehf.sHtML

val m = mapOf("a" to 1)
来源：http://blog.sjlbkw.cn/Article/details/gnfzrwvcl.sHtML

[T14] Kotlin：循环
来源：http://www.share.epnwcf.com/Article/details/gmufstzad.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.tarul.cn/Article/details/gewctwcxf.sHtML


<!-- 参考信息 -->