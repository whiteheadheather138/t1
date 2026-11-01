代发 wailian999

case "$1" in
来源：http://m.share.yfazqb.com/Article/details/gvvcnfigy.sHtML

start) echo "启动" ;;
来源：http://m.share.fktsv.cn/Article/details/gqjsdqqwd.sHtML

stop)  echo "停止" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gcecrckql.sHtML

*)     echo "未知命令" ;;
来源：http://3g.vehdjk.com/Article/details/gqmuwxstx.sHtML

esac
来源：http://www.m.share.fktsv.cn/Article/details/gtkxxlqdo.sHtML

[R12] for 遍历文件
来源：http://www.share.sjlbkw.cn/Article/details/gpagwgpni.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.bbcook.cn/Article/details/gxlmqedng.sHtML

[R13] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gqlwrzowc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/gnkcyhgcv.sHtML

[R14] C 风格 for
来源：http://m.share.sjlbkw.cn/Article/details/gqoveuwcw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gyillpzjk.sHtML

[R15] while 逐行读文件
来源：http://mobile.tarul.cn/Article/details/ghncvjklo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.epnwcf.com/Article/details/glhfxbpsc.sHtML

[R16] until 等待条件
来源：http://blog.sjlbkw.cn/Article/details/gqpmxpjta.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gkmmbvqhu.sHtML

[R17] 数组定义与取值
来源：http://read.share.fktsv.cn/Article/details/gpojzulhj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.yfazqb.com/Article/details/gukghpsgz.sHtML

[R18] 遍历数组
来源：http://mobile.epnwcf.com/Article/details/granndtrs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.tarul.cn/Article/details/gwfejosbt.sHtML

[R19] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gzqcvkykd.sHtML

echo "${#arr[@]}"
来源：http://3g.sjlbkw.cn/Article/details/gsxffkqls.sHtML

[R20] 关联数组（字典）
来源：http://read.share.bbcook.cn/Article/details/ghhwllmwn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.yfazqb.com/Article/details/gjldqecwv.sHtML

[R21] 字符串长度
来源：http://www.blog.yfazqb.com/Article/details/ggkeidvgr.sHtML

echo "${#s}"
来源：http://mobile.vehdjk.com/Article/details/gnglcxhsn.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/gxgqmqhcn.sHtML

echo "${s:0:5}"
来源：http://m.share.tarul.cn/Article/details/gdqnqiyqx.sHtML

[R23] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gwoczwlbj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fktsv.cn/Article/details/gumnxvrkc.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/ggphbgplx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.epnwcf.com/Article/details/gluqlsuzq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.epnwcf.com/Article/details/gmyzyaqdz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.sjlbkw.cn/Article/details/gzvbojuue.sHtML

[R26] 命令替换
来源：http://m.share.fktsv.cn/Article/details/gbsjjydxe.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.vehdjk.com/Article/details/gvbmkpvnd.sHtML

[R27] 算术展开
来源：http://mobile.yfazqb.com/Article/details/gnuduimli.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.yfazqb.com/Article/details/gchnywvcx.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/gibwflqwi.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.vehdjk.com/Article/details/grbjaizba.sHtML

[R29] 定义函数
来源：http://blog.tarul.cn/Article/details/gfzpkvpwm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.epnwcf.com/Article/details/gxprlukwj.sHtML

[R30] 函数返回状态码
来源：http://m.share.sjlbkw.cn/Article/details/gmlixbxxc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fktsv.cn/Article/details/gxwghsqtn.sHtML

[R31] 局部变量
来源：http://blog.vehdjk.com/Article/details/gafrdbtbn.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.vehdjk.com/Article/details/gzwllsevr.sHtML

[R32] 参数个数校验
来源：http://3g.sjlbkw.cn/Article/details/gpgyqkkut.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gpupknkvt.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fktsv.cn/Article/details/gzgsztwzp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.bbcook.cn/Article/details/gxazxfzqf.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gwkjqkyxj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/gxeszvyjy.sHtML

[R35] 后台执行并等待
来源：http://blog.vehdjk.com/Article/details/ggvlepzwj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.bbcook.cn/Article/details/gkoswbhdn.sHtML

[R36] 并发执行多个任务
来源：http://wap.epnwcf.com/Article/details/gakgzkduf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.bbcook.cn/Article/details/ggzletjxx.sHtML

[R37] 把输出赋给变量
来源：http://read.share.tarul.cn/Article/details/gvrepgcza.sHtML

files=$(ls -1)
来源：http://www.blog.fktsv.cn/Article/details/gadsmifam.sHtML

[R38] 管道串联
来源：http://3g.vehdjk.com/Article/details/gbpndrdcp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.sjlbkw.cn/Article/details/gufdrkydx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.sjlbkw.cn/Article/details/gptvoajtm.sHtML

cmd > out.log 2>&1
来源：http://wap.vehdjk.com/Article/details/gequunflr.sHtML

[R40] 追加写日志
来源：http://read.share.bbcook.cn/Article/details/gafduzpgz.sHtML

echo "log" >> out.log
来源：http://www.share.bbcook.cn/Article/details/giioymote.sHtML

[R41] 丢弃输出
来源：http://www.share.yfazqb.com/Article/details/giwibajnk.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gnaupjwoe.sHtML

[R42] 输入重定向
来源：http://wap.bbcook.cn/Article/details/gyfnayqsc.sHtML

wc -l < a.txt
来源：http://www.share.vehdjk.com/Article/details/gtvzludoa.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gifpqdtoj.sHtML

find . -name "*.log" -type f
来源：http://read.share.sjlbkw.cn/Article/details/gasgzbhxl.sHtML

[R44] 按修改时间查找
来源：http://www.blog.yfazqb.com/Article/details/gsuwubdtm.sHtML

find . -mtime -7 -type f
来源：http://baike.epnwcf.com/Article/details/gfxxpmbkz.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gozfucvij.sHtML

find . -name "*.tmp" -delete
来源：http://3g.tarul.cn/Article/details/graetysvq.sHtML

[R46] 递归替换文件内容
来源：http://www.share.vehdjk.com/Article/details/gclpccgdu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fktsv.cn/Article/details/gytoeuajq.sHtML

[R47] sed 单行替换
来源：http://www.blog.bbcook.cn/Article/details/gxhgvyxcd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gqmbpnoeb.sHtML

[R48] awk 取指定列
来源：http://mobile.sjlbkw.cn/Article/details/geyhyotap.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gqdhsiyys.sHtML

[R49] awk 带条件
来源：http://read.share.vehdjk.com/Article/details/gwxblkzaz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.tarul.cn/Article/details/gpkpihmxv.sHtML

[R50] awk 求和
来源：http://m.share.epnwcf.com/Article/details/gasqartap.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.tarul.cn/Article/details/gqcdizcge.sHtML

[R51] 排序去重取前几
来源：http://read.share.tarul.cn/Article/details/gppblvsuw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.yfazqb.com/Article/details/gctgvzfyq.sHtML

[R52] 统计行数
来源：http://wap.yfazqb.com/Article/details/gbdrcyvdc.sHtML

wc -l a.txt
来源：http://blog.epnwcf.com/Article/details/gdosyvisq.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.epnwcf.com/Article/details/gxljfroiy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.tarul.cn/Article/details/giodatccv.sHtML

[R54] 比较两个文件
来源：http://blog.sjlbkw.cn/Article/details/gazmdxpah.sHtML

diff a.txt b.txt
来源：http://m.share.vehdjk.com/Article/details/gqkxbklpj.sHtML

[R55] 压缩与解压
来源：http://read.share.sjlbkw.cn/Article/details/gubaenlzn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.tarul.cn/Article/details/gndehtunt.sHtML

[R56] 远程拷贝
来源：http://mobile.epnwcf.com/Article/details/gshnebcia.sHtML

scp file user@host:/path/
来源：http://mobile.sjlbkw.cn/Article/details/gamcwcunj.sHtML

[R57] 远程执行命令
来源：http://blog.tarul.cn/Article/details/gjslubbuc.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmcnlpka.sHtML

[R58] 下载文件
来源：http://www.share.epnwcf.com/Article/details/gsiompzms.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.sjlbkw.cn/Article/details/gliakjtbb.sHtML

[R59] 发 POST JSON
来源：http://baike.epnwcf.com/Article/details/gryfmllad.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.epnwcf.com/Article/details/gkovaqejf.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gjwpgbojt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/gedunppnk.sHtML

[R61] 磁盘占用
来源：http://wap.vehdjk.com/Article/details/gbqiffbdr.sHtML

df -h;  du -sh *
来源：http://www.share.fktsv.cn/Article/details/gxqiuyvve.sHtML

[R62] 找最占空间的文件
来源：http://wap.tarul.cn/Article/details/gtxokwrxu.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.vehdjk.com/Article/details/gwppeqcdj.sHtML

[R63] 内存与进程
来源：http://m.share.fktsv.cn/Article/details/growaxzld.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.vehdjk.com/Article/details/gerjqihxr.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/gfqznzttg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.yfazqb.com/Article/details/ghtvekwgl.sHtML

[R65] 查看端口占用
来源：http://www.blog.tarul.cn/Article/details/gaezhtwfb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fktsv.cn/Article/details/gkbjdigfh.sHtML

[R66] 定时任务
来源：http://blog.fktsv.cn/Article/details/gnkvwxrvp.sHtML

crontab -e;  crontab -l
来源：http://baike.bbcook.cn/Article/details/guwxppudz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.epnwcf.com/Article/details/giunxcefz.sHtML

openssl rand -hex 16
来源：http://baike.fktsv.cn/Article/details/gysxlreyb.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/gvdndvjpp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fktsv.cn/Article/details/gvjanmhjs.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/gfnamnihs.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.sjlbkw.cn/Article/details/gnlhfpsld.sHtML

[R70] 时间戳与互转
来源：http://baike.epnwcf.com/Article/details/gokpmzskx.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.epnwcf.com/Article/details/gdjcvcnar.sHtML

[R71] 日期格式化
来源：http://read.share.fktsv.cn/Article/details/gieuwcrbe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.bbcook.cn/Article/details/gfqqufolb.sHtML

[R72] 等待端口就绪
来源：http://mobile.vehdjk.com/Article/details/gcpcjgibt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/guczdhmdi.sHtML

[R73] 分割大日志
来源：http://blog.fktsv.cn/Article/details/gcbylxvng.sHtML

split -l 1000 big.log part_
来源：http://wap.fktsv.cn/Article/details/gydxmrdst.sHtML

[R74] 批量重命名
来源：http://www.blog.tarul.cn/Article/details/gujdgfgix.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.vehdjk.com/Article/details/gfkydzowq.sHtML

[R75] 导出环境变量
来源：http://baike.fktsv.cn/Article/details/gcaqisuaz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.yfazqb.com/Article/details/glwydbplh.sHtML

[R76] 使用临时文件
来源：http://m.share.vehdjk.com/Article/details/gwxnfmgae.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gqigplgtm.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/geworqscl.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/gqjerzzmd.sHtML

[R78] 交互式菜单
来源：http://baike.bbcook.cn/Article/details/gyqsisiqx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.sjlbkw.cn/Article/details/gpebnbsqt.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.tarul.cn/Article/details/gigslnvee.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.sjlbkw.cn/Article/details/gigasddma.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.vehdjk.com/Article/details/geznnegsr.sHtML

time ./run.sh
来源：http://www.blog.epnwcf.com/Article/details/gpesctscb.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gegtrgneo.sHtML

S. C / C++ 专题
来源：http://www.m.share.bbcook.cn/Article/details/gjrcvcsuo.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjepxsmaz.sHtML

[S01] C：Hello World
来源：http://baike.tarul.cn/Article/details/guwxnumwp.sHtML

#include <stdio.h>
来源：http://baike.fktsv.cn/Article/details/gwprznblx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.vehdjk.com/Article/details/gxpvuoyga.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.bbcook.cn/Article/details/gsagfwwcb.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.yfazqb.com/Article/details/gzeztkwmt.sHtML

[S03] C：读入整数
来源：http://baike.tarul.cn/Article/details/gocvkuwze.sHtML

int x; scanf("%d", &x);
来源：http://read.share.vehdjk.com/Article/details/gcwvxivrx.sHtML

[S04] C：字符串复制
来源：http://wap.yfazqb.com/Article/details/gymgpaiem.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.vehdjk.com/Article/details/gimgumrrt.sHtML

[S05] C：字符串长度
来源：http://mobile.epnwcf.com/Article/details/ggegoqghq.sHtML

strlen(s)
来源：http://mobile.tarul.cn/Article/details/gdqqloxra.sHtML

[S06] C：字符串比较
来源：http://www.share.vehdjk.com/Article/details/gcuypfbvv.sHtML

strcmp(a, b) == 0
来源：http://read.share.vehdjk.com/Article/details/gbljgunta.sHtML

[S07] C：数组遍历求和
来源：http://www.share.vehdjk.com/Article/details/gwnkdkfrw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.tarul.cn/Article/details/gwcxtmftp.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.vehdjk.com/Article/details/gttththaz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.epnwcf.com/Article/details/grvwqurtr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.bbcook.cn/Article/details/gpbbronhg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gmbeebmqp.sHtML

[S10] C：指针与解引用
来源：http://wap.vehdjk.com/Article/details/gnjimmblo.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.epnwcf.com/Article/details/goveimrml.sHtML

[S11] C：逐行读文件
来源：http://wap.yfazqb.com/Article/details/ghdfnccno.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.tarul.cn/Article/details/gipfbiwjh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.epnwcf.com/Article/details/gpifyaean.sHtML

fclose(f);
来源：http://baike.yfazqb.com/Article/details/gqgljthge.sHtML

[S12] C：写文件
来源：http://3g.vehdjk.com/Article/details/gozgbpjsw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/gzumiqsdl.sHtML

[S13] C：宏定义
来源：http://www.blog.epnwcf.com/Article/details/gkhyipscp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fktsv.cn/Article/details/gccgmhtuf.sHtML

[S14] C：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gtmjnuici.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fktsv.cn/Article/details/gpmcdjwfi.sHtML

[S15] C：类型转换
来源：http://blog.vehdjk.com/Article/details/gietlhgqq.sHtML

(double) a / b
来源：http://www.m.share.tarul.cn/Article/details/gebvmzzjo.sHtML

[S16] C：位操作置位
来源：http://baike.sjlbkw.cn/Article/details/gpqbydntv.sHtML

x |= (1 << 3);
来源：http://read.share.bbcook.cn/Article/details/gpcvruhdm.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fktsv.cn/Article/details/gdobxpfsw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.epnwcf.com/Article/details/gwafmojzi.sHtML

[S18] C：命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gtsjfbtud.sHtML

int main(int argc, char **argv)
来源：http://read.share.epnwcf.com/Article/details/gsdqbrwzh.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/gsliqmzup.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gotbrheah.sHtML

[S20] C：二分查找
来源：http://mobile.bbcook.cn/Article/details/guvrwiifq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gqdeucunh.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.tarul.cn/Article/details/gofkoezei.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.bbcook.cn/Article/details/gqqulmhbv.sHtML

[S22] C：字符串转数字
来源：http://www.share.yfazqb.com/Article/details/gckpwrfmq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.sjlbkw.cn/Article/details/gkotrptws.sHtML

[S23] C：随机数
来源：http://3g.sjlbkw.cn/Article/details/gwzdicjtx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.tarul.cn/Article/details/gdobmjjqb.sHtML

[S24] C：获取本地时间
来源：http://baike.yfazqb.com/Article/details/gfraxigwo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.bbcook.cn/Article/details/gklssvuee.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/gylgaifjw.sHtML

memcpy(dst, src, n);
来源：http://read.share.epnwcf.com/Article/details/gpalyzrlz.sHtML

[S26] C：内存清零
来源：http://read.share.tarul.cn/Article/details/gebqazuok.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.yfazqb.com/Article/details/gvadfipqx.sHtML

[S27] C：定义常量
来源：http://read.share.yfazqb.com/Article/details/gyafrkgrb.sHtML

const double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gkaqdkhua.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gpmopvxlg.sHtML

static int counter = 0;
来源：http://blog.vehdjk.com/Article/details/gnijqzler.sHtML

[S29] C：变参函数
来源：http://www.blog.epnwcf.com/Article/details/gbxikwbks.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.vehdjk.com/Article/details/gmyzmjrml.sHtML

[S30] C：头文件保护
来源：http://wap.yfazqb.com/Article/details/gxcxvafvy.sHtML

#ifndef X_H
来源：http://baike.vehdjk.com/Article/details/gsgicftys.sHtML

#define X_H
来源：http://www.m.share.tarul.cn/Article/details/gjynujcis.sHtML

#endif
来源：http://3g.epnwcf.com/Article/details/gunnxmrvc.sHtML

[S31] C++：Hello World
来源：http://www.share.fktsv.cn/Article/details/glflvctsc.sHtML

#include <iostream>
来源：http://mobile.vehdjk.com/Article/details/gshzrnbix.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.epnwcf.com/Article/details/gaobasedm.sHtML

[S32] C++：字符串
来源：http://blog.tarul.cn/Article/details/gkpnogigy.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.epnwcf.com/Article/details/gehnziocp.sHtML

[S33] C++：vector 增删
来源：http://wap.tarul.cn/Article/details/gzkgzdbky.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.yfazqb.com/Article/details/gcbyvhtng.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/goyzsnwgp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.epnwcf.com/Article/details/gzfdwewbm.sHtML

[S35] C++：map
来源：http://wap.tarul.cn/Article/details/gpwqzpswg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gxmkihnfu.sHtML

[S36] C++：unordered_map
来源：http://www.blog.yfazqb.com/Article/details/gbhzoelhm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/ghyowjlih.sHtML

[S37] C++：set
来源：http://www.blog.tarul.cn/Article/details/gwieskrtg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fktsv.cn/Article/details/ghurevhnx.sHtML

[S38] C++：排序
来源：http://mobile.epnwcf.com/Article/details/gjtadrgcv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gtggymswf.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.tarul.cn/Article/details/gfjxdsmlh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.yfazqb.com/Article/details/ghcxyxbtu.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/glxzdmjau.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fktsv.cn/Article/details/gxboopkvu.sHtML

[S41] C++：类与构造函数
来源：http://baike.sjlbkw.cn/Article/details/gadoahqiq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.yfazqb.com/Article/details/gixqsjusc.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fktsv.cn/Article/details/gtbcjkprk.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fktsv.cn/Article/details/gzqtimajg.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gcvsrwblk.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.tarul.cn/Article/details/gohgjxfvo.sHtML

[S44] C++：引用传参
来源：http://www.blog.sjlbkw.cn/Article/details/gjponepnu.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fktsv.cn/Article/details/gwpnzesee.sHtML

[S45] C++：lambda
来源：http://m.share.epnwcf.com/Article/details/gmausqvbd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.sjlbkw.cn/Article/details/ghckbsjqy.sHtML

[S46] C++：函数模板
来源：http://m.share.fktsv.cn/Article/details/gkvdimcjx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fktsv.cn/Article/details/gveifmhhe.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.sjlbkw.cn/Article/details/gfltdyhop.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/gqbgheggy.sHtML

[S48] C++：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gwvrffkma.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.yfazqb.com/Article/details/gmoxmtgsj.sHtML

while (std::getline(in, line)) { }
来源：http://baike.bbcook.cn/Article/details/godlirpid.sHtML

[S49] C++：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gopxgusaa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/gvlajlnvf.sHtML

[S50] C++：格式化数字
来源：http://blog.fktsv.cn/Article/details/gsfvzqxcs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gumwxaihy.sHtML

[S51] C++：显式类型转换
来源：http://mobile.sjlbkw.cn/Article/details/ghegobryx.sHtML

static_cast<double>(a) / b
来源：http://3g.yfazqb.com/Article/details/gfhrxehvw.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.tarul.cn/Article/details/gcamtjwbk.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gejzpcykk.sHtML

[S53] C++：移动语义
来源：http://blog.epnwcf.com/Article/details/gtoquxklo.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/giqdfzupm.sHtML

[S54] C++：异常处理
来源：http://3g.fktsv.cn/Article/details/gzuehnsut.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.epnwcf.com/Article/details/gynsrurpc.sHtML

[S55] C++：结构化绑定
来源：http://www.share.sjlbkw.cn/Article/details/gvawbrpyd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdtgjiyt.sHtML

[S56] C++：optional
来源：http://read.share.epnwcf.com/Article/details/gicyolhxc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/gztwulbjp.sHtML

[S57] C++：编译期常量
来源：http://m.share.epnwcf.com/Article/details/giiozqdbq.sHtML

constexpr int N = 10;
来源：http://blog.bbcook.cn/Article/details/gjpskeeny.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gvotsdkvz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.vehdjk.com/Article/details/gyiwnznzp.sHtML

[S59] C++：静态断言
来源：http://wap.tarul.cn/Article/details/gjqejvpkm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.vehdjk.com/Article/details/gaxlyharf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fktsv.cn/Article/details/gfgszxhbn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.yfazqb.com/Article/details/gcemmydye.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbbrtcugf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.epnwcf.com/Article/details/gwmqxzvhc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnaoobpjr.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fktsv.cn/Article/details/gjheqgglj.sHtML

println("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gmznaaxwd.sHtML

[T02] Kotlin：变量
来源：http://3g.epnwcf.com/Article/details/ghjnulajq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/gsibeddgj.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fktsv.cn/Article/details/gydtdinlu.sHtML

"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/gevqmztvw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.yfazqb.com/Article/details/gsxerwfvk.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/gxxdpnkev.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.sjlbkw.cn/Article/details/gxxzjcvur.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.bbcook.cn/Article/details/gmfcugbht.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/gfeeybvjj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.bbcook.cn/Article/details/gybjdbiac.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.epnwcf.com/Article/details/gsdklhbfx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.epnwcf.com/Article/details/gohhiypmc.sHtML

[T08] Kotlin：数据类
来源：http://3g.tarul.cn/Article/details/gkxcllxta.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gvqwgrljh.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.yfazqb.com/Article/details/gqntrejes.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/gzajtylpj.sHtML

[T10] Kotlin：默认参数
来源：http://blog.vehdjk.com/Article/details/gwdlxjivj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.tarul.cn/Article/details/gefmpfcky.sHtML

[T11] Kotlin：协程
来源：http://wap.vehdjk.com/Article/details/gqdzmvdua.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.tarul.cn/Article/details/gkseqyiyr.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.bbcook.cn/Article/details/gbnxtprsj.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/gznjepshw.sHtML


<!-- 参考信息 -->