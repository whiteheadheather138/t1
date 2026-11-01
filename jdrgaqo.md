代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gajlbcpbd.sHtML

[R10] 正则匹配
来源：http://blog.fktsv.cn/Article/details/gewxnwlyn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.yfazqb.com/Article/details/gtweynpgo.sHtML

[R11] case 多分支
来源：http://www.share.epnwcf.com/Article/details/gffvdyrtz.sHtML

case "$1" in
来源：http://wap.epnwcf.com/Article/details/gqhzqekuz.sHtML

start) echo "启动" ;;
来源：http://m.share.epnwcf.com/Article/details/gnbjtuymj.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gnesvbqmu.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gvkgmwdti.sHtML

esac
来源：http://www.share.bbcook.cn/Article/details/glvmtjiba.sHtML

[R12] for 遍历文件
来源：http://3g.tarul.cn/Article/details/gcwbqukei.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.sjlbkw.cn/Article/details/gumgvzimu.sHtML

[R13] for 计数循环
来源：http://blog.fktsv.cn/Article/details/guvdeiiam.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.yfazqb.com/Article/details/giwekqalt.sHtML

[R14] C 风格 for
来源：http://m.share.sjlbkw.cn/Article/details/gcssxceaw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/gqidzbzpf.sHtML

[R15] while 逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gjxntiwfn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fktsv.cn/Article/details/glnvuejun.sHtML

[R16] until 等待条件
来源：http://baike.fktsv.cn/Article/details/gplogbcuq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/ggsppnigm.sHtML

[R17] 数组定义与取值
来源：http://m.share.epnwcf.com/Article/details/gxfwpudxm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.epnwcf.com/Article/details/gnaavkxse.sHtML

[R18] 遍历数组
来源：http://blog.yfazqb.com/Article/details/gwntgtqfj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.epnwcf.com/Article/details/ghjiwihsk.sHtML

[R19] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjihysfu.sHtML

echo "${#arr[@]}"
来源：http://mobile.tarul.cn/Article/details/gtbjaoumy.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.yfazqb.com/Article/details/gdmmzyiku.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.vehdjk.com/Article/details/gtdxtmgxn.sHtML

[R21] 字符串长度
来源：http://wap.bbcook.cn/Article/details/gziemdwcj.sHtML

echo "${#s}"
来源：http://blog.yfazqb.com/Article/details/glfnstytq.sHtML

[R22] 截取子串
来源：http://www.blog.tarul.cn/Article/details/gwxuwhfyn.sHtML

echo "${s:0:5}"
来源：http://mobile.vehdjk.com/Article/details/gzthiinbh.sHtML

[R23] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/gtfqrfhex.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.epnwcf.com/Article/details/gkzxhsgmu.sHtML

[R24] 大小写转换
来源：http://wap.tarul.cn/Article/details/goxxctvrf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.tarul.cn/Article/details/gcvhqanfk.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.vehdjk.com/Article/details/ggtqcatdg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.sjlbkw.cn/Article/details/gxcgyqimf.sHtML

[R26] 命令替换
来源：http://baike.epnwcf.com/Article/details/gbujoqjtk.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.yfazqb.com/Article/details/gkmtnxujf.sHtML

[R27] 算术展开
来源：http://www.m.share.epnwcf.com/Article/details/gbtvfihie.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.tarul.cn/Article/details/gtfpamnvj.sHtML

[R28] 浮点运算
来源：http://wap.yfazqb.com/Article/details/gtzbbbhbl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fktsv.cn/Article/details/gbdicnxzu.sHtML

[R29] 定义函数
来源：http://baike.epnwcf.com/Article/details/gtgjglpjb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.yfazqb.com/Article/details/gagkncccp.sHtML

[R30] 函数返回状态码
来源：http://3g.yfazqb.com/Article/details/gdoalsztd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.epnwcf.com/Article/details/gdgpimgro.sHtML

[R31] 局部变量
来源：http://3g.tarul.cn/Article/details/gytvojofd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/gcibthyas.sHtML

[R32] 参数个数校验
来源：http://wap.sjlbkw.cn/Article/details/gfzyqqeng.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gkbnlyokl.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fktsv.cn/Article/details/gwbxqueox.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.yfazqb.com/Article/details/gwscbbvej.sHtML

[R34] 退出时清理
来源：http://mobile.bbcook.cn/Article/details/gzzmliprm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/geptpdwln.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/ggmhkbult.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.epnwcf.com/Article/details/gyzwaubrx.sHtML

[R36] 并发执行多个任务
来源：http://read.share.bbcook.cn/Article/details/gmqrtpnoy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.epnwcf.com/Article/details/gzkeszuyu.sHtML

[R37] 把输出赋给变量
来源：http://baike.tarul.cn/Article/details/gorfonkvp.sHtML

files=$(ls -1)
来源：http://baike.epnwcf.com/Article/details/gxwapkcai.sHtML

[R38] 管道串联
来源：http://blog.yfazqb.com/Article/details/gvngjrgeg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.vehdjk.com/Article/details/geufkfoxm.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.sjlbkw.cn/Article/details/gpmlwuxdr.sHtML

cmd > out.log 2>&1
来源：http://baike.vehdjk.com/Article/details/gjcmtqhnu.sHtML

[R40] 追加写日志
来源：http://www.share.bbcook.cn/Article/details/gidijpokq.sHtML

echo "log" >> out.log
来源：http://www.share.fktsv.cn/Article/details/gqvcnlqpg.sHtML

[R41] 丢弃输出
来源：http://www.m.share.vehdjk.com/Article/details/gextjfffv.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.yfazqb.com/Article/details/gefynhejj.sHtML

[R42] 输入重定向
来源：http://www.m.share.bbcook.cn/Article/details/gvfpzvyez.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/gthnvkkks.sHtML

[R43] 按名字查找文件
来源：http://m.share.epnwcf.com/Article/details/gxehnylco.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fktsv.cn/Article/details/gzduzkybj.sHtML

[R44] 按修改时间查找
来源：http://www.share.epnwcf.com/Article/details/gwzhzvevs.sHtML

find . -mtime -7 -type f
来源：http://baike.vehdjk.com/Article/details/gaxdxaryc.sHtML

[R45] 批量删除
来源：http://www.share.epnwcf.com/Article/details/gauncbklo.sHtML

find . -name "*.tmp" -delete
来源：http://wap.epnwcf.com/Article/details/gvtusnjpc.sHtML

[R46] 递归替换文件内容
来源：http://blog.epnwcf.com/Article/details/grwuqhxcu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.vehdjk.com/Article/details/gkdtcvenw.sHtML

[R47] sed 单行替换
来源：http://blog.sjlbkw.cn/Article/details/gevmxhour.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.yfazqb.com/Article/details/gnzqqcqvy.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/gfuotpkch.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.tarul.cn/Article/details/giqtghdwp.sHtML

[R49] awk 带条件
来源：http://3g.fktsv.cn/Article/details/gttitliha.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.yfazqb.com/Article/details/gqliykmgc.sHtML

[R50] awk 求和
来源：http://baike.fktsv.cn/Article/details/gdlmuhrhy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gdsithhkh.sHtML

[R51] 排序去重取前几
来源：http://blog.fktsv.cn/Article/details/glexdlavx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.sjlbkw.cn/Article/details/gamhiztvl.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/gmmzojkcs.sHtML

wc -l a.txt
来源：http://blog.epnwcf.com/Article/details/glhzveayu.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.vehdjk.com/Article/details/gdgzqogyq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjwxdekw.sHtML

[R54] 比较两个文件
来源：http://wap.tarul.cn/Article/details/gakiejaqq.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/gfngfhxcg.sHtML

[R55] 压缩与解压
来源：http://read.share.tarul.cn/Article/details/gdbiyrftn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.yfazqb.com/Article/details/gxlleyksh.sHtML

[R56] 远程拷贝
来源：http://www.share.bbcook.cn/Article/details/gmaekwkwc.sHtML

scp file user@host:/path/
来源：http://www.blog.tarul.cn/Article/details/gvqcjutce.sHtML

[R57] 远程执行命令
来源：http://www.share.fktsv.cn/Article/details/gdgwtjuqp.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fktsv.cn/Article/details/gswfahczs.sHtML

[R58] 下载文件
来源：http://read.share.bbcook.cn/Article/details/gsegihrto.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fktsv.cn/Article/details/gfctubpmo.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/gsjaritmp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.tarul.cn/Article/details/ghlyriawq.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/gafaxafnp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/gpiixumlm.sHtML

[R61] 磁盘占用
来源：http://m.share.sjlbkw.cn/Article/details/grdluoadp.sHtML

df -h;  du -sh *
来源：http://www.blog.tarul.cn/Article/details/gkxujyppk.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/gjervcgvv.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.yfazqb.com/Article/details/guaxnyado.sHtML

[R63] 内存与进程
来源：http://www.share.yfazqb.com/Article/details/gjjziypyn.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.epnwcf.com/Article/details/glqoqvruk.sHtML

[R64] 结束进程
来源：http://wap.vehdjk.com/Article/details/glhvcrnsz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.sjlbkw.cn/Article/details/goxcpuwst.sHtML

[R65] 查看端口占用
来源：http://baike.vehdjk.com/Article/details/gmalczmif.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.yfazqb.com/Article/details/gsjasqiwq.sHtML

[R66] 定时任务
来源：http://read.share.bbcook.cn/Article/details/gqfrwetyq.sHtML

crontab -e;  crontab -l
来源：http://3g.fktsv.cn/Article/details/geuomoemi.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.sjlbkw.cn/Article/details/gwrertnld.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/gligmlzdl.sHtML

[R68] 计算文件校验值
来源：http://blog.yfazqb.com/Article/details/gmpsdxjhl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fktsv.cn/Article/details/gzvknwvuw.sHtML

[R69] 生成随机密码
来源：http://www.share.fktsv.cn/Article/details/gmzhgaebu.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.bbcook.cn/Article/details/gxxdryhbu.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.bbcook.cn/Article/details/gzchevgyu.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.tarul.cn/Article/details/gqxopdtyc.sHtML

[R71] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gjmbjiscp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.tarul.cn/Article/details/gmdfgegev.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fktsv.cn/Article/details/gptneyymp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gafvphidz.sHtML

[R73] 分割大日志
来源：http://m.share.fktsv.cn/Article/details/gsqnyvxjt.sHtML

split -l 1000 big.log part_
来源：http://baike.vehdjk.com/Article/details/gsaqeumia.sHtML

[R74] 批量重命名
来源：http://blog.sjlbkw.cn/Article/details/gokfpajux.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/gqsbzopii.sHtML

[R75] 导出环境变量
来源：http://3g.bbcook.cn/Article/details/ggyxsazqx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fktsv.cn/Article/details/ggqvbidbb.sHtML

[R76] 使用临时文件
来源：http://baike.vehdjk.com/Article/details/gytyprzqf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/gihvnbnmc.sHtML

[R77] 读取用户输入
来源：http://wap.epnwcf.com/Article/details/gbbfsqnqy.sHtML

read -rp "请输入: " ans
来源：http://www.blog.vehdjk.com/Article/details/gmrawtpdp.sHtML

[R78] 交互式菜单
来源：http://blog.vehdjk.com/Article/details/ggovgyxow.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.vehdjk.com/Article/details/gckrvgues.sHtML

[R79] 解析命令行选项
来源：http://baike.sjlbkw.cn/Article/details/gxdxvjkxo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.yfazqb.com/Article/details/glvxhzkid.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/gsuzptcwq.sHtML

time ./run.sh
来源：http://3g.sjlbkw.cn/Article/details/gokvkclvk.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glshiblyk.sHtML

S. C / C++ 专题
来源：http://3g.sjlbkw.cn/Article/details/gncakstqe.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvxospnhj.sHtML

[S01] C：Hello World
来源：http://wap.fktsv.cn/Article/details/gfezgtctf.sHtML

#include <stdio.h>
来源：http://baike.vehdjk.com/Article/details/ghaeievou.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.vehdjk.com/Article/details/gbdgutblb.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.yfazqb.com/Article/details/ghgwdkzow.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/girluwnjd.sHtML

[S03] C：读入整数
来源：http://read.share.sjlbkw.cn/Article/details/gvbqgygbi.sHtML

int x; scanf("%d", &x);
来源：http://wap.bbcook.cn/Article/details/grgwwaggm.sHtML

[S04] C：字符串复制
来源：http://3g.tarul.cn/Article/details/gozyudsho.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/gvaulznwj.sHtML

[S05] C：字符串长度
来源：http://3g.fktsv.cn/Article/details/gkmcrjcsb.sHtML

strlen(s)
来源：http://3g.tarul.cn/Article/details/gvzqmmmah.sHtML

[S06] C：字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gvcfmhdzh.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.epnwcf.com/Article/details/gfkbsatsq.sHtML

[S07] C：数组遍历求和
来源：http://3g.bbcook.cn/Article/details/gqvnmaqwq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fktsv.cn/Article/details/ghzqweslq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fktsv.cn/Article/details/gflbomiaa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.sjlbkw.cn/Article/details/gyvlwlgxe.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fktsv.cn/Article/details/gkmefqixf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.epnwcf.com/Article/details/gqdfiezdn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.epnwcf.com/Article/details/gdwtcakfg.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.tarul.cn/Article/details/genhifkfx.sHtML

[S11] C：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gwqigebrf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fktsv.cn/Article/details/ggrzhayvs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.yfazqb.com/Article/details/gjcqatcle.sHtML

fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/grflyxghi.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/gqbjfocnh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.vehdjk.com/Article/details/gxxyampme.sHtML

[S13] C：宏定义
来源：http://www.share.fktsv.cn/Article/details/gbamlyszh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.bbcook.cn/Article/details/gktrpaoec.sHtML

[S14] C：枚举
来源：http://3g.fktsv.cn/Article/details/glzbxkzga.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.vehdjk.com/Article/details/guuudqbqe.sHtML

[S15] C：类型转换
来源：http://baike.sjlbkw.cn/Article/details/gdbjwxbox.sHtML

(double) a / b
来源：http://www.m.share.bbcook.cn/Article/details/gzmacxyww.sHtML

[S16] C：位操作置位
来源：http://www.blog.vehdjk.com/Article/details/guuxzyqew.sHtML

x |= (1 << 3);
来源：http://read.share.vehdjk.com/Article/details/gqsnrwujl.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gsmamxhcd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.sjlbkw.cn/Article/details/gwmyloian.sHtML

[S18] C：命令行参数
来源：http://www.m.share.tarul.cn/Article/details/gjcefpbql.sHtML

int main(int argc, char **argv)
来源：http://mobile.epnwcf.com/Article/details/gpxaibkll.sHtML

[S19] C：快速排序
来源：http://www.share.tarul.cn/Article/details/gwhcbbwet.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/gqbfhuzrc.sHtML

[S20] C：二分查找
来源：http://baike.bbcook.cn/Article/details/gdsoagdoa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gnnetqkak.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/gyiosbvnn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.bbcook.cn/Article/details/gkizpgmlg.sHtML

[S22] C：字符串转数字
来源：http://m.share.sjlbkw.cn/Article/details/gybrkpdsn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.epnwcf.com/Article/details/gbierfyeb.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gmcmleswn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.tarul.cn/Article/details/gxwsjgdnm.sHtML

[S24] C：获取本地时间
来源：http://m.share.epnwcf.com/Article/details/gmosgqzvv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fktsv.cn/Article/details/guwgacuwa.sHtML

[S25] C：内存拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gvxoujgvn.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gwcxjfolq.sHtML

[S26] C：内存清零
来源：http://read.share.tarul.cn/Article/details/gputqpwkq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzslklchu.sHtML

[S27] C：定义常量
来源：http://read.share.bbcook.cn/Article/details/ggtotczzx.sHtML

const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gmexdbbla.sHtML

[S28] C：静态变量
来源：http://m.share.vehdjk.com/Article/details/gtktolkgw.sHtML

static int counter = 0;
来源：http://baike.yfazqb.com/Article/details/gbsryjvcu.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/gbdjaeyqk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.vehdjk.com/Article/details/ghwlsxaan.sHtML

[S30] C：头文件保护
来源：http://www.m.share.sjlbkw.cn/Article/details/gebzlxcgc.sHtML

#ifndef X_H
来源：http://www.share.bbcook.cn/Article/details/gfndsvuql.sHtML

#define X_H
来源：http://mobile.fktsv.cn/Article/details/gjahrtarz.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/grxwpamls.sHtML

[S31] C++：Hello World
来源：http://wap.bbcook.cn/Article/details/gjjawbdvd.sHtML

#include <iostream>
来源：http://3g.fktsv.cn/Article/details/ghkkdqagf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.sjlbkw.cn/Article/details/gwsapwnuw.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gxddzdszr.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.tarul.cn/Article/details/gfprtwetb.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/gigafgovf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.yfazqb.com/Article/details/gyqeekrmr.sHtML

[S34] C++：遍历 vector
来源：http://read.share.vehdjk.com/Article/details/gdgbkabew.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fktsv.cn/Article/details/gefxwikds.sHtML

[S35] C++：map
来源：http://baike.epnwcf.com/Article/details/gkfuyzela.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/ghwplvstq.sHtML

[S36] C++：unordered_map
来源：http://baike.epnwcf.com/Article/details/gyyjhxbdp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gwrdbyqty.sHtML

[S37] C++：set
来源：http://3g.sjlbkw.cn/Article/details/gnencipnk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.vehdjk.com/Article/details/gyjimrtzx.sHtML

[S38] C++：排序
来源：http://wap.tarul.cn/Article/details/gqtrudyed.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.tarul.cn/Article/details/goaazyqgn.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/gccpvlcxr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fktsv.cn/Article/details/gryauidve.sHtML

[S40] C++：查找元素
来源：http://blog.sjlbkw.cn/Article/details/gdynqzxax.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fktsv.cn/Article/details/gbafyfibw.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/ghfmhsiuy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/gyeawdvgv.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.sjlbkw.cn/Article/details/gtjgafnvx.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/gmdtuuubo.sHtML

[S43] C++：智能指针
来源：http://www.share.epnwcf.com/Article/details/georkzqlj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.epnwcf.com/Article/details/glufqctis.sHtML

[S44] C++：引用传参
来源：http://baike.sjlbkw.cn/Article/details/gekznquov.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.bbcook.cn/Article/details/gujhamfxg.sHtML

[S45] C++：lambda
来源：http://www.blog.fktsv.cn/Article/details/geqtdhtui.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.sjlbkw.cn/Article/details/gjpdiroda.sHtML

[S46] C++：函数模板
来源：http://blog.fktsv.cn/Article/details/ghxxsejdv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.tarul.cn/Article/details/georvtotn.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fktsv.cn/Article/details/grqafnund.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.epnwcf.com/Article/details/ggacjcxod.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gwnwojlev.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.tarul.cn/Article/details/gpniwlrph.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.tarul.cn/Article/details/glrphuioj.sHtML

[S49] C++：写文件
来源：http://www.m.share.tarul.cn/Article/details/gvofgjbhx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.yfazqb.com/Article/details/gdimqvqnp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.yfazqb.com/Article/details/gwdjnxutr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.bbcook.cn/Article/details/glbjpbdvk.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gdnkdzhmm.sHtML

static_cast<double>(a) / b
来源：http://blog.tarul.cn/Article/details/gqecdfoba.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.vehdjk.com/Article/details/gjxxwscrn.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fktsv.cn/Article/details/gouyyykmb.sHtML

[S53] C++：移动语义
来源：http://blog.epnwcf.com/Article/details/gsoeedxxt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.yfazqb.com/Article/details/gztolnpyo.sHtML

[S54] C++：异常处理
来源：http://m.share.sjlbkw.cn/Article/details/gdxrmgssj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.sjlbkw.cn/Article/details/gdkevgnta.sHtML

[S55] C++：结构化绑定
来源：http://mobile.bbcook.cn/Article/details/ggnrbxfjf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gkmhtilil.sHtML

[S56] C++：optional
来源：http://m.share.epnwcf.com/Article/details/gpzzgoccq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/ghohwazug.sHtML

[S57] C++：编译期常量
来源：http://baike.sjlbkw.cn/Article/details/gndmzwrbc.sHtML

constexpr int N = 10;
来源：http://3g.sjlbkw.cn/Article/details/gjlygjnhi.sHtML

[S58] C++：命名空间
来源：http://baike.yfazqb.com/Article/details/gplbtcrfz.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.epnwcf.com/Article/details/gffubbkum.sHtML

[S59] C++：静态断言
来源：http://mobile.vehdjk.com/Article/details/gxbgzbzts.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fktsv.cn/Article/details/gqozaarln.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fktsv.cn/Article/details/gocaknjvj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.bbcook.cn/Article/details/gtixmtjrx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gzmcxpudq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.vehdjk.com/Article/details/gxkgetqoa.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gpggfggpu.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.tarul.cn/Article/details/giayjhkaj.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/ggchivmcx.sHtML

[T02] Kotlin：变量
来源：http://baike.bbcook.cn/Article/details/gvnfzvwdl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.sjlbkw.cn/Article/details/gduavkste.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/gabitbmvc.sHtML

"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/ghaiooabh.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gyrmhhnvi.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fktsv.cn/Article/details/gamojbncq.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.sjlbkw.cn/Article/details/guypgzvpm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.yfazqb.com/Article/details/gjaxnjcws.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fktsv.cn/Article/details/gpyiukxyb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.bbcook.cn/Article/details/gzwxkihcu.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.yfazqb.com/Article/details/gbqsnluct.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fktsv.cn/Article/details/gvkrsaejf.sHtML

[T08] Kotlin：数据类
来源：http://3g.bbcook.cn/Article/details/gebtpcimn.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gbmyppknm.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.bbcook.cn/Article/details/gdsihjoim.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.yfazqb.com/Article/details/gnwwoftae.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.yfazqb.com/Article/details/gedffpvrd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.epnwcf.com/Article/details/gcxkfcaga.sHtML


<!-- 参考信息 -->