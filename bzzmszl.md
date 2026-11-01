代发 wailian999

case "$1" in
来源：http://mobile.epnwcf.com/Article/details/gnhlrmfdc.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gpmsibtgk.sHtML

stop)  echo "停止" ;;
来源：http://blog.vehdjk.com/Article/details/gswbhenpq.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.bbcook.cn/Article/details/ghtbirfun.sHtML

esac
来源：http://read.share.tarul.cn/Article/details/gimqwwzqg.sHtML

[R12] for 遍历文件
来源：http://mobile.vehdjk.com/Article/details/gotvujtjf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fktsv.cn/Article/details/gxskqmrsk.sHtML

[R13] for 计数循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyprnxdy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/gnmfbapcx.sHtML

[R14] C 风格 for
来源：http://blog.bbcook.cn/Article/details/gduvbymai.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gnufmuqxm.sHtML

[R15] while 逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gnymyjdbf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fktsv.cn/Article/details/gfxftwxhi.sHtML

[R16] until 等待条件
来源：http://m.share.tarul.cn/Article/details/gbifajcwf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gmpfiiwpg.sHtML

[R17] 数组定义与取值
来源：http://read.share.sjlbkw.cn/Article/details/gqfifymbg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.bbcook.cn/Article/details/gbfuacgeq.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gvngldenj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.sjlbkw.cn/Article/details/gfsijcimu.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/gkmlajjjc.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.yfazqb.com/Article/details/glvspbrtm.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.sjlbkw.cn/Article/details/gxkajvzlr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.yfazqb.com/Article/details/ghngtrhnh.sHtML

[R21] 字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gnjuvybld.sHtML

echo "${#s}"
来源：http://mobile.epnwcf.com/Article/details/gbkmxvblg.sHtML

[R22] 截取子串
来源：http://www.share.yfazqb.com/Article/details/gyrhelnhl.sHtML

echo "${s:0:5}"
来源：http://www.blog.fktsv.cn/Article/details/gqclttmli.sHtML

[R23] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gujmmitvq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.yfazqb.com/Article/details/gzsvfifpr.sHtML

[R24] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gkgiyucbq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.vehdjk.com/Article/details/gdiuxwivw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.epnwcf.com/Article/details/gzqzkxtui.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.vehdjk.com/Article/details/gntdmxlyz.sHtML

[R26] 命令替换
来源：http://read.share.vehdjk.com/Article/details/gprbpttel.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.epnwcf.com/Article/details/gzdomlljm.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gbaxdimep.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.bbcook.cn/Article/details/gbcmbwusx.sHtML

[R28] 浮点运算
来源：http://read.share.yfazqb.com/Article/details/gczzafqwx.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.epnwcf.com/Article/details/gvogertem.sHtML

[R29] 定义函数
来源：http://read.share.yfazqb.com/Article/details/gjlppoyub.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.tarul.cn/Article/details/gnmeuqxol.sHtML

[R30] 函数返回状态码
来源：http://mobile.sjlbkw.cn/Article/details/gzzqneevp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fktsv.cn/Article/details/gazgfpras.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/gcgwadlxz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.yfazqb.com/Article/details/gmhykjzro.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/gvxccthqf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gfxzisnli.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.bbcook.cn/Article/details/gtfzfgzzl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.vehdjk.com/Article/details/ggwgdjcbn.sHtML

[R34] 退出时清理
来源：http://read.share.vehdjk.com/Article/details/goysdvzka.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fktsv.cn/Article/details/gxnsjimfk.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/gnnitdvjm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.bbcook.cn/Article/details/gcbbzyypy.sHtML

[R36] 并发执行多个任务
来源：http://wap.yfazqb.com/Article/details/gifcxridn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fktsv.cn/Article/details/gdeijhose.sHtML

[R37] 把输出赋给变量
来源：http://wap.tarul.cn/Article/details/gnjwpijox.sHtML

files=$(ls -1)
来源：http://blog.yfazqb.com/Article/details/gbtdwtqee.sHtML

[R38] 管道串联
来源：http://www.m.share.bbcook.cn/Article/details/gltlrgdwj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.tarul.cn/Article/details/gnugvfidq.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.sjlbkw.cn/Article/details/gvlfwrdzw.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/gnskwxdju.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/gmxbhljnw.sHtML

echo "log" >> out.log
来源：http://read.share.fktsv.cn/Article/details/gsrivzuym.sHtML

[R41] 丢弃输出
来源：http://mobile.sjlbkw.cn/Article/details/gvjildmuv.sHtML

cmd >/dev/null 2>&1
来源：http://blog.yfazqb.com/Article/details/gelmbzfpv.sHtML

[R42] 输入重定向
来源：http://blog.tarul.cn/Article/details/gqqhinyth.sHtML

wc -l < a.txt
来源：http://read.share.yfazqb.com/Article/details/gophoyjza.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/gzjfwmobn.sHtML

find . -name "*.log" -type f
来源：http://baike.bbcook.cn/Article/details/gdesoslsh.sHtML

[R44] 按修改时间查找
来源：http://wap.fktsv.cn/Article/details/gsbxwvwzs.sHtML

find . -mtime -7 -type f
来源：http://read.share.bbcook.cn/Article/details/gopjctxze.sHtML

[R45] 批量删除
来源：http://blog.yfazqb.com/Article/details/gtabxrxrg.sHtML

find . -name "*.tmp" -delete
来源：http://3g.tarul.cn/Article/details/gomngwrte.sHtML

[R46] 递归替换文件内容
来源：http://www.share.epnwcf.com/Article/details/gfbfjzhli.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fktsv.cn/Article/details/girbmenvw.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/gonvyrrzf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gknadmtsv.sHtML

[R48] awk 取指定列
来源：http://baike.fktsv.cn/Article/details/gweedkqid.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gugdeefoy.sHtML

[R49] awk 带条件
来源：http://baike.bbcook.cn/Article/details/gujnzgvfy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.bbcook.cn/Article/details/gumhhfljs.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/gwzxawhxc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.tarul.cn/Article/details/gxewnraml.sHtML

[R51] 排序去重取前几
来源：http://wap.bbcook.cn/Article/details/gescupxmf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.tarul.cn/Article/details/ggmfcqckh.sHtML

[R52] 统计行数
来源：http://www.m.share.fktsv.cn/Article/details/gzghmpefk.sHtML

wc -l a.txt
来源：http://mobile.fktsv.cn/Article/details/glbnsuenf.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.vehdjk.com/Article/details/gdwzlwcah.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.vehdjk.com/Article/details/gcvqtsmvx.sHtML

[R54] 比较两个文件
来源：http://blog.bbcook.cn/Article/details/gdzhfckmq.sHtML

diff a.txt b.txt
来源：http://3g.bbcook.cn/Article/details/gctksrdqn.sHtML

[R55] 压缩与解压
来源：http://www.share.bbcook.cn/Article/details/gvroluvpx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fktsv.cn/Article/details/gjefrrpwv.sHtML

[R56] 远程拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gmbxdipvf.sHtML

scp file user@host:/path/
来源：http://www.share.vehdjk.com/Article/details/gtfyosjot.sHtML

[R57] 远程执行命令
来源：http://m.share.sjlbkw.cn/Article/details/gbubsgsdb.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fktsv.cn/Article/details/gdihmybgk.sHtML

[R58] 下载文件
来源：http://read.share.bbcook.cn/Article/details/gttyqzwhh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.tarul.cn/Article/details/gmchbffdr.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/gxmtouoes.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.bbcook.cn/Article/details/gjiaaiheq.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gcdwfsjtf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fktsv.cn/Article/details/gyhzrjevg.sHtML

[R61] 磁盘占用
来源：http://read.share.tarul.cn/Article/details/gqcllgevw.sHtML

df -h;  du -sh *
来源：http://www.m.share.fktsv.cn/Article/details/grugghzzy.sHtML

[R62] 找最占空间的文件
来源：http://www.share.epnwcf.com/Article/details/gqoxxlntq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.sjlbkw.cn/Article/details/ghyenujaf.sHtML

[R63] 内存与进程
来源：http://read.share.yfazqb.com/Article/details/gngcwnwod.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.vehdjk.com/Article/details/gwqumzndg.sHtML

[R64] 结束进程
来源：http://mobile.tarul.cn/Article/details/guxkxshai.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.vehdjk.com/Article/details/grwvkipjl.sHtML

[R65] 查看端口占用
来源：http://www.share.sjlbkw.cn/Article/details/ghouumcde.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.yfazqb.com/Article/details/gevvnufpo.sHtML

[R66] 定时任务
来源：http://www.blog.bbcook.cn/Article/details/gnawhtquy.sHtML

crontab -e;  crontab -l
来源：http://3g.vehdjk.com/Article/details/gbipkpnyf.sHtML

[R67] 生成随机十六进制串
来源：http://wap.epnwcf.com/Article/details/gtoplvekg.sHtML

openssl rand -hex 16
来源：http://mobile.vehdjk.com/Article/details/gtmckbfzm.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/gdscisqbn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.tarul.cn/Article/details/ganaakisf.sHtML

[R69] 生成随机密码
来源：http://wap.fktsv.cn/Article/details/gagxoeuop.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.epnwcf.com/Article/details/gapwtgtdh.sHtML

[R70] 时间戳与互转
来源：http://mobile.fktsv.cn/Article/details/gbmuwucrx.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fktsv.cn/Article/details/gtgmvcozk.sHtML

[R71] 日期格式化
来源：http://baike.tarul.cn/Article/details/gqveseiwr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fktsv.cn/Article/details/gfuzfpyvh.sHtML

[R72] 等待端口就绪
来源：http://wap.bbcook.cn/Article/details/gaxaaclko.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/guuqxasrw.sHtML

[R73] 分割大日志
来源：http://baike.tarul.cn/Article/details/gfwsaprmz.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/gelzsqjzz.sHtML

[R74] 批量重命名
来源：http://wap.epnwcf.com/Article/details/gabvysmdv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.sjlbkw.cn/Article/details/goeccwjtx.sHtML

[R75] 导出环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/gbdsqduax.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.epnwcf.com/Article/details/ghdewjayr.sHtML

[R76] 使用临时文件
来源：http://www.m.share.vehdjk.com/Article/details/gklutuwxu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gdjrohmpr.sHtML

[R77] 读取用户输入
来源：http://www.blog.vehdjk.com/Article/details/gsnlgnovu.sHtML

read -rp "请输入: " ans
来源：http://3g.epnwcf.com/Article/details/gtewkfatq.sHtML

[R78] 交互式菜单
来源：http://blog.tarul.cn/Article/details/grnevsmgs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fktsv.cn/Article/details/gixmbkrvh.sHtML

[R79] 解析命令行选项
来源：http://blog.bbcook.cn/Article/details/gphmhnbkk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.bbcook.cn/Article/details/giaudgbsx.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fktsv.cn/Article/details/ghhitwdgd.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/gmjluubwo.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/guasjhtfl.sHtML

S. C / C++ 专题
来源：http://mobile.epnwcf.com/Article/details/glqyeoeiz.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gamsskevt.sHtML

[S01] C：Hello World
来源：http://m.share.yfazqb.com/Article/details/greqvqjdu.sHtML

#include <stdio.h>
来源：http://3g.vehdjk.com/Article/details/gatgxshxj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gunpwxdrs.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.vehdjk.com/Article/details/gfrofbqnb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.vehdjk.com/Article/details/geqjpeunz.sHtML

[S03] C：读入整数
来源：http://read.share.vehdjk.com/Article/details/grmgaavnh.sHtML

int x; scanf("%d", &x);
来源：http://mobile.tarul.cn/Article/details/gsiezwysp.sHtML

[S04] C：字符串复制
来源：http://www.m.share.bbcook.cn/Article/details/gnksbspmy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gahboywou.sHtML

[S05] C：字符串长度
来源：http://m.share.epnwcf.com/Article/details/gidqdlvhk.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/gtodcxhma.sHtML

[S06] C：字符串比较
来源：http://blog.tarul.cn/Article/details/gmnyimvdx.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.epnwcf.com/Article/details/gbiyrkygm.sHtML

[S07] C：数组遍历求和
来源：http://blog.tarul.cn/Article/details/grcizspqv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.epnwcf.com/Article/details/gsknenwwf.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.bbcook.cn/Article/details/ghdmvenyk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.sjlbkw.cn/Article/details/gwbqcbedx.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fktsv.cn/Article/details/geccaqfih.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.vehdjk.com/Article/details/gxnhrcmxv.sHtML

[S10] C：指针与解引用
来源：http://www.blog.epnwcf.com/Article/details/gmmogdwuv.sHtML

int *p = &a;  *p = 5;
来源：http://baike.yfazqb.com/Article/details/gapsipvib.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gzftexzol.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.yfazqb.com/Article/details/gfsmcluio.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.yfazqb.com/Article/details/gaovliqyt.sHtML

fclose(f);
来源：http://wap.epnwcf.com/Article/details/gixouqlan.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/gztsiohgu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.yfazqb.com/Article/details/gatqddosa.sHtML

[S13] C：宏定义
来源：http://baike.fktsv.cn/Article/details/grljzpsza.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.tarul.cn/Article/details/gxvfqrdyh.sHtML

[S14] C：枚举
来源：http://www.m.share.vehdjk.com/Article/details/gakspmurh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.yfazqb.com/Article/details/gjoapdzap.sHtML

[S15] C：类型转换
来源：http://read.share.fktsv.cn/Article/details/gumhbsrmn.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/gpcgnluzk.sHtML

[S16] C：位操作置位
来源：http://3g.bbcook.cn/Article/details/goemhwctp.sHtML

x |= (1 << 3);
来源：http://www.m.share.fktsv.cn/Article/details/gofhcazhp.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.vehdjk.com/Article/details/giewbtpkl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/gfxnfdodp.sHtML

[S18] C：命令行参数
来源：http://www.share.bbcook.cn/Article/details/gfjlngvdf.sHtML

int main(int argc, char **argv)
来源：http://baike.epnwcf.com/Article/details/gviiuwoln.sHtML

[S19] C：快速排序
来源：http://3g.sjlbkw.cn/Article/details/gnddoewto.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gunxobdwk.sHtML

[S20] C：二分查找
来源：http://blog.tarul.cn/Article/details/guusokeie.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gafrgqyru.sHtML

[S21] C：字符类别判断
来源：http://read.share.epnwcf.com/Article/details/gurxtgypw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fktsv.cn/Article/details/ggjxppyyj.sHtML

[S22] C：字符串转数字
来源：http://3g.yfazqb.com/Article/details/gcwvjcalm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/gvwgaxain.sHtML

[S23] C：随机数
来源：http://baike.bbcook.cn/Article/details/gclplrqnt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.yfazqb.com/Article/details/girpbfjjc.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.vehdjk.com/Article/details/gwjxbxjgq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.epnwcf.com/Article/details/gtbfxvlqr.sHtML

[S25] C：内存拷贝
来源：http://read.share.bbcook.cn/Article/details/gzmucsanc.sHtML

memcpy(dst, src, n);
来源：http://baike.bbcook.cn/Article/details/gebsefkgw.sHtML

[S26] C：内存清零
来源：http://blog.fktsv.cn/Article/details/gaeqrbfzn.sHtML

memset(a, 0, sizeof a);
来源：http://baike.tarul.cn/Article/details/gsartvrnh.sHtML

[S27] C：定义常量
来源：http://www.m.share.yfazqb.com/Article/details/gshubuxjx.sHtML

const double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gxcikrayp.sHtML

[S28] C：静态变量
来源：http://www.blog.bbcook.cn/Article/details/gnelztaeq.sHtML

static int counter = 0;
来源：http://3g.vehdjk.com/Article/details/gkbkopmod.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/ggwfnbirp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/guauwwuuy.sHtML

[S30] C：头文件保护
来源：http://wap.sjlbkw.cn/Article/details/gewhyexxs.sHtML

#ifndef X_H
来源：http://3g.bbcook.cn/Article/details/ghbtkiqtw.sHtML

#define X_H
来源：http://read.share.tarul.cn/Article/details/gnjixkuxj.sHtML

#endif
来源：http://www.m.share.vehdjk.com/Article/details/gntynbukf.sHtML

[S31] C++：Hello World
来源：http://blog.fktsv.cn/Article/details/ggsfzlvrb.sHtML

#include <iostream>
来源：http://m.share.tarul.cn/Article/details/geycrmsjv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.tarul.cn/Article/details/gkugnkhcu.sHtML

[S32] C++：字符串
来源：http://read.share.tarul.cn/Article/details/gdsqwtgxj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.epnwcf.com/Article/details/gsasmyzcj.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrlwyqik.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gihahkmht.sHtML

[S34] C++：遍历 vector
来源：http://baike.fktsv.cn/Article/details/ggxnmqoik.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.bbcook.cn/Article/details/gndafaovj.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/gfizgonsp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/getyofiwb.sHtML

[S36] C++：unordered_map
来源：http://www.blog.sjlbkw.cn/Article/details/gdxgsjuca.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/glfxqxify.sHtML

[S37] C++：set
来源：http://read.share.yfazqb.com/Article/details/gjhqqsalc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gridgsrgj.sHtML

[S38] C++：排序
来源：http://3g.sjlbkw.cn/Article/details/goduhysse.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.tarul.cn/Article/details/grywksymm.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fktsv.cn/Article/details/gppnhtxus.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.yfazqb.com/Article/details/ghbtwnghc.sHtML

[S40] C++：查找元素
来源：http://m.share.bbcook.cn/Article/details/gpvbjmiqo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.vehdjk.com/Article/details/gsqkmuvwe.sHtML

[S41] C++：类与构造函数
来源：http://blog.tarul.cn/Article/details/gozshfypj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.epnwcf.com/Article/details/gpigddujs.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.tarul.cn/Article/details/grtgzllck.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.tarul.cn/Article/details/gjopsvosz.sHtML

[S43] C++：智能指针
来源：http://www.blog.yfazqb.com/Article/details/gambjqiae.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.bbcook.cn/Article/details/gjjibxhce.sHtML

[S44] C++：引用传参
来源：http://3g.tarul.cn/Article/details/ghycijocj.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.yfazqb.com/Article/details/ganlatepy.sHtML

[S45] C++：lambda
来源：http://mobile.tarul.cn/Article/details/gwqwqfquv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fktsv.cn/Article/details/gvevkncoh.sHtML

[S46] C++：函数模板
来源：http://blog.fktsv.cn/Article/details/geqbzuvba.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.epnwcf.com/Article/details/guznayucb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.sjlbkw.cn/Article/details/gezupktsj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.bbcook.cn/Article/details/gtheqaztf.sHtML

[S48] C++：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gltjxpqvf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.vehdjk.com/Article/details/gueoixjjc.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.tarul.cn/Article/details/ghjozonry.sHtML

[S49] C++：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gvwuudkrf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fktsv.cn/Article/details/gsyxqnmbo.sHtML

[S50] C++：格式化数字
来源：http://3g.epnwcf.com/Article/details/gfsazsmku.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gcsumdlon.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fktsv.cn/Article/details/gibsuvjlr.sHtML

static_cast<double>(a) / b
来源：http://baike.yfazqb.com/Article/details/gqyppahbg.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.sjlbkw.cn/Article/details/gftsdjvbb.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fktsv.cn/Article/details/gsbnbpnql.sHtML

[S53] C++：移动语义
来源：http://m.share.yfazqb.com/Article/details/gauyaxekx.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.epnwcf.com/Article/details/gpugfpivz.sHtML

[S54] C++：异常处理
来源：http://blog.epnwcf.com/Article/details/gfbenpydr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.epnwcf.com/Article/details/gzcbbjxct.sHtML

[S55] C++：结构化绑定
来源：http://blog.tarul.cn/Article/details/gxmnccprp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fktsv.cn/Article/details/ggwixvgot.sHtML

[S56] C++：optional
来源：http://blog.sjlbkw.cn/Article/details/gegaykyjr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.epnwcf.com/Article/details/gyhhninga.sHtML

[S57] C++：编译期常量
来源：http://mobile.tarul.cn/Article/details/gghsssolb.sHtML

constexpr int N = 10;
来源：http://mobile.vehdjk.com/Article/details/gasysfstt.sHtML

[S58] C++：命名空间
来源：http://mobile.tarul.cn/Article/details/gdffzmmaj.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.epnwcf.com/Article/details/gkebhcxgz.sHtML

[S59] C++：静态断言
来源：http://mobile.vehdjk.com/Article/details/gccgsuiow.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.tarul.cn/Article/details/gwsvmpffv.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fktsv.cn/Article/details/gstwyesev.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.tarul.cn/Article/details/gavygwygv.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gticywido.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.sjlbkw.cn/Article/details/gnjzznshk.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gdvilownf.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gagusxill.sHtML

println("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gqdvtxukq.sHtML

[T02] Kotlin：变量
来源：http://wap.epnwcf.com/Article/details/gqkmfzkeo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.sjlbkw.cn/Article/details/gdpysiqgf.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.sjlbkw.cn/Article/details/ggvlylrxf.sHtML

"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/ggkeczahr.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gchxeedhd.sHtML

val n: String? = null;  n?.length
来源：http://blog.epnwcf.com/Article/details/gkqwcpvxr.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/gvxvjiadg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.sjlbkw.cn/Article/details/gxiczdtit.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gquejdxnl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gtuxfqwew.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.vehdjk.com/Article/details/gxelwqvzh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.tarul.cn/Article/details/gjfnvbxoq.sHtML

[T08] Kotlin：数据类
来源：http://m.share.tarul.cn/Article/details/gqcvsmoaa.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.vehdjk.com/Article/details/gjegaghaz.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.epnwcf.com/Article/details/gemtgqfaj.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.sjlbkw.cn/Article/details/gcascqkpk.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gqdmbdfzy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/gnajjlujw.sHtML

[T11] Kotlin：协程
来源：http://www.blog.epnwcf.com/Article/details/gvnbegotb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fktsv.cn/Article/details/gqtmqvgwl.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/gwdjfclvn.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gdprikogu.sHtML


<!-- 参考信息 -->