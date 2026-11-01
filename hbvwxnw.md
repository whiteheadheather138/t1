代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.sjlbkw.cn/Article/details/gwybltzbc.sHtML

[R10] 正则匹配
来源：http://3g.vehdjk.com/Article/details/gxjmjrgjq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.yfazqb.com/Article/details/gfigflsqs.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/gdteijglp.sHtML

case "$1" in
来源：http://3g.vehdjk.com/Article/details/gahzvgchs.sHtML

start) echo "启动" ;;
来源：http://wap.epnwcf.com/Article/details/gglroyqed.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.yfazqb.com/Article/details/ggmzzitdh.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.bbcook.cn/Article/details/gpyggtbgb.sHtML

esac
来源：http://3g.tarul.cn/Article/details/gijftuymz.sHtML

[R12] for 遍历文件
来源：http://m.share.yfazqb.com/Article/details/gttjyrics.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.tarul.cn/Article/details/gnnjgwqpv.sHtML

[R13] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gsvoctbro.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/geylaowst.sHtML

[R14] C 风格 for
来源：http://m.share.tarul.cn/Article/details/goyqvvtjc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/glpjmmlrw.sHtML

[R15] while 逐行读文件
来源：http://baike.epnwcf.com/Article/details/ghhctuywa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.tarul.cn/Article/details/gvnatesny.sHtML

[R16] until 等待条件
来源：http://m.share.epnwcf.com/Article/details/gixwsvdwi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gfrfwhcyy.sHtML

[R17] 数组定义与取值
来源：http://m.share.fktsv.cn/Article/details/ghryzelgx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.vehdjk.com/Article/details/glqojrcam.sHtML

[R18] 遍历数组
来源：http://baike.bbcook.cn/Article/details/gowespwpt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.vehdjk.com/Article/details/glkicepvq.sHtML

[R19] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/givjzhgjo.sHtML

echo "${#arr[@]}"
来源：http://wap.sjlbkw.cn/Article/details/giwkanbcw.sHtML

[R20] 关联数组（字典）
来源：http://read.share.sjlbkw.cn/Article/details/gjxeuqlnm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.epnwcf.com/Article/details/gwjhtuhvw.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/gapevxqin.sHtML

echo "${#s}"
来源：http://www.share.tarul.cn/Article/details/gijtpmrif.sHtML

[R22] 截取子串
来源：http://blog.tarul.cn/Article/details/gwjdkkehe.sHtML

echo "${s:0:5}"
来源：http://3g.yfazqb.com/Article/details/geecsgdbc.sHtML

[R23] 字符串替换
来源：http://baike.tarul.cn/Article/details/glpfltsbk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.vehdjk.com/Article/details/gefwucvxr.sHtML

[R24] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gpdenhntc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.epnwcf.com/Article/details/gunvmbeqo.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.tarul.cn/Article/details/gudbsjowd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.tarul.cn/Article/details/gykvncqrq.sHtML

[R26] 命令替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gttuigtmd.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.vehdjk.com/Article/details/gfkncgxyy.sHtML

[R27] 算术展开
来源：http://www.blog.fktsv.cn/Article/details/gmmftijrp.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.vehdjk.com/Article/details/ghjvbuvgg.sHtML

[R28] 浮点运算
来源：http://read.share.sjlbkw.cn/Article/details/gtsehmwtx.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/grdsslrqy.sHtML

[R29] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/gjqhblawp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.bbcook.cn/Article/details/gjnmeocwk.sHtML

[R30] 函数返回状态码
来源：http://www.share.fktsv.cn/Article/details/gzxijmfeu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.sjlbkw.cn/Article/details/gsbrjbzkx.sHtML

[R31] 局部变量
来源：http://blog.sjlbkw.cn/Article/details/gxllqohej.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.sjlbkw.cn/Article/details/gixxmmocb.sHtML

[R32] 参数个数校验
来源：http://www.share.yfazqb.com/Article/details/gxwnqngcg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/geqhhcpsv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fktsv.cn/Article/details/gmdwyepdz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.vehdjk.com/Article/details/gvruiqsgb.sHtML

[R34] 退出时清理
来源：http://read.share.bbcook.cn/Article/details/gkasdkyzn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gylbuqjwh.sHtML

[R35] 后台执行并等待
来源：http://wap.tarul.cn/Article/details/gvjwduijs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnefxgsjg.sHtML

[R36] 并发执行多个任务
来源：http://3g.sjlbkw.cn/Article/details/grwybvzug.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.bbcook.cn/Article/details/gwlsrecoo.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/gyukbjuqs.sHtML

files=$(ls -1)
来源：http://3g.fktsv.cn/Article/details/ghvaysart.sHtML

[R38] 管道串联
来源：http://www.share.tarul.cn/Article/details/gzzeoxagl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.vehdjk.com/Article/details/gecugmajb.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.bbcook.cn/Article/details/ggovkuwtc.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/gmzkfrwdb.sHtML

[R40] 追加写日志
来源：http://m.share.bbcook.cn/Article/details/gylmvvdkh.sHtML

echo "log" >> out.log
来源：http://3g.vehdjk.com/Article/details/gidanzawk.sHtML

[R41] 丢弃输出
来源：http://www.blog.fktsv.cn/Article/details/gxlgirpkx.sHtML

cmd >/dev/null 2>&1
来源：http://3g.tarul.cn/Article/details/grksckbkh.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/giaokcepo.sHtML

wc -l < a.txt
来源：http://baike.sjlbkw.cn/Article/details/ggnwhmfhp.sHtML

[R43] 按名字查找文件
来源：http://read.share.vehdjk.com/Article/details/gpbozqvnx.sHtML

find . -name "*.log" -type f
来源：http://www.blog.tarul.cn/Article/details/gpbekokru.sHtML

[R44] 按修改时间查找
来源：http://baike.sjlbkw.cn/Article/details/gosjwuunc.sHtML

find . -mtime -7 -type f
来源：http://read.share.epnwcf.com/Article/details/gaqlvjpuu.sHtML

[R45] 批量删除
来源：http://blog.tarul.cn/Article/details/gophvvlpd.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.tarul.cn/Article/details/glhvyzzpc.sHtML

[R46] 递归替换文件内容
来源：http://3g.vehdjk.com/Article/details/gpigliefk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.yfazqb.com/Article/details/gsdejurgt.sHtML

[R47] sed 单行替换
来源：http://m.share.vehdjk.com/Article/details/gmbqmpolh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gocpvgsrg.sHtML

[R48] awk 取指定列
来源：http://read.share.bbcook.cn/Article/details/gbaxtocjo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gbdwrlqwa.sHtML

[R49] awk 带条件
来源：http://mobile.vehdjk.com/Article/details/gridcneaa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.tarul.cn/Article/details/grvkmxecu.sHtML

[R50] awk 求和
来源：http://baike.fktsv.cn/Article/details/gfztehwbv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.vehdjk.com/Article/details/gzsjnwejz.sHtML

[R51] 排序去重取前几
来源：http://m.share.fktsv.cn/Article/details/gsmesboay.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/grddcrsok.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/gsytfjgcx.sHtML

wc -l a.txt
来源：http://wap.tarul.cn/Article/details/gidajaqjm.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/gniukwyot.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.tarul.cn/Article/details/gosqtgbeo.sHtML

[R54] 比较两个文件
来源：http://read.share.vehdjk.com/Article/details/gbsjdutbx.sHtML

diff a.txt b.txt
来源：http://read.share.epnwcf.com/Article/details/giknyrfmi.sHtML

[R55] 压缩与解压
来源：http://www.share.yfazqb.com/Article/details/ggvxdrbcz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fktsv.cn/Article/details/gdukirvwf.sHtML

[R56] 远程拷贝
来源：http://wap.vehdjk.com/Article/details/goxyteanr.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gdagwcyrz.sHtML

[R57] 远程执行命令
来源：http://wap.sjlbkw.cn/Article/details/gwbjwyljy.sHtML

ssh user@host 'uptime'
来源：http://www.blog.epnwcf.com/Article/details/gcvpqaatd.sHtML

[R58] 下载文件
来源：http://www.m.share.vehdjk.com/Article/details/gtnvvwwyo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.vehdjk.com/Article/details/goqguxwkv.sHtML

[R59] 发 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/gmnvvvlhb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.epnwcf.com/Article/details/goirmqwaq.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/gntjxwvtd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.bbcook.cn/Article/details/gmyvnqvzi.sHtML

[R61] 磁盘占用
来源：http://www.m.share.vehdjk.com/Article/details/gxyujmlpf.sHtML

df -h;  du -sh *
来源：http://3g.yfazqb.com/Article/details/gehanvymb.sHtML

[R62] 找最占空间的文件
来源：http://read.share.sjlbkw.cn/Article/details/gjzttdwtc.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.vehdjk.com/Article/details/gikugdtbi.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/gcvhtwwys.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjcwdhbu.sHtML

[R64] 结束进程
来源：http://www.share.vehdjk.com/Article/details/gbuiqkkqw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.yfazqb.com/Article/details/gtemfkbjz.sHtML

[R65] 查看端口占用
来源：http://mobile.yfazqb.com/Article/details/gcbdhgqog.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.epnwcf.com/Article/details/gzyinnmpc.sHtML

[R66] 定时任务
来源：http://3g.epnwcf.com/Article/details/gwujmrxcj.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.yfazqb.com/Article/details/gsnysrmhi.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/ggthsvadq.sHtML

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/gspdlrxal.sHtML

[R68] 计算文件校验值
来源：http://mobile.sjlbkw.cn/Article/details/gubrelebq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.bbcook.cn/Article/details/gdyzpghzu.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/gtiqecxvv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.sjlbkw.cn/Article/details/givtbsfly.sHtML

[R70] 时间戳与互转
来源：http://blog.epnwcf.com/Article/details/gcvnxfxxd.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.bbcook.cn/Article/details/grfxkhfdy.sHtML

[R71] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gfetoayzs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.yfazqb.com/Article/details/groemjlmd.sHtML

[R72] 等待端口就绪
来源：http://wap.sjlbkw.cn/Article/details/gipouogmf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gltntvfbf.sHtML

[R73] 分割大日志
来源：http://read.share.vehdjk.com/Article/details/gbzugalwn.sHtML

split -l 1000 big.log part_
来源：http://www.share.yfazqb.com/Article/details/gkpsmjhah.sHtML

[R74] 批量重命名
来源：http://wap.epnwcf.com/Article/details/gqymvnvak.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.sjlbkw.cn/Article/details/gqkwbdwuv.sHtML

[R75] 导出环境变量
来源：http://mobile.tarul.cn/Article/details/gqfezzwah.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.vehdjk.com/Article/details/gzaoyrxra.sHtML

[R76] 使用临时文件
来源：http://www.m.share.tarul.cn/Article/details/gnpmcgluh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gkrkoewmb.sHtML

[R77] 读取用户输入
来源：http://www.blog.epnwcf.com/Article/details/gbksowdof.sHtML

read -rp "请输入: " ans
来源：http://blog.bbcook.cn/Article/details/gowquirfv.sHtML

[R78] 交互式菜单
来源：http://blog.sjlbkw.cn/Article/details/gabxjbuvi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.tarul.cn/Article/details/gvrjgbdyh.sHtML

[R79] 解析命令行选项
来源：http://3g.fktsv.cn/Article/details/grdsichxb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/gdiowrpej.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fktsv.cn/Article/details/gzxnbahjp.sHtML

time ./run.sh
来源：http://read.share.vehdjk.com/Article/details/gzhutdqon.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gpzmegisv.sHtML

S. C / C++ 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gjxxfdsbh.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gvnrffzxy.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/glnjocpjd.sHtML

#include <stdio.h>
来源：http://wap.tarul.cn/Article/details/gmpwpcmhu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.epnwcf.com/Article/details/gzaylglml.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/ghdacojbk.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.bbcook.cn/Article/details/gnkhbqilz.sHtML

[S03] C：读入整数
来源：http://wap.vehdjk.com/Article/details/gqwwtsaes.sHtML

int x; scanf("%d", &x);
来源：http://3g.epnwcf.com/Article/details/gufebymuy.sHtML

[S04] C：字符串复制
来源：http://mobile.tarul.cn/Article/details/gujzssjgl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.epnwcf.com/Article/details/grwzagmop.sHtML

[S05] C：字符串长度
来源：http://m.share.tarul.cn/Article/details/giwcpaird.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/gfieltnmy.sHtML

[S06] C：字符串比较
来源：http://read.share.fktsv.cn/Article/details/gaonttzvw.sHtML

strcmp(a, b) == 0
来源：http://baike.tarul.cn/Article/details/gnzlxkcst.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/gjuulgbtt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.epnwcf.com/Article/details/gkqdjihuq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.epnwcf.com/Article/details/gcgjfpipm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.vehdjk.com/Article/details/gyhxyudvv.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fktsv.cn/Article/details/gdorrjujg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/gjnrrhkmp.sHtML

[S10] C：指针与解引用
来源：http://mobile.tarul.cn/Article/details/gshrhzkqx.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/gjilmxwgz.sHtML

[S11] C：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gcjmpccbj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.epnwcf.com/Article/details/gyyicgfit.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.tarul.cn/Article/details/glnntygfw.sHtML

fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gkosopukq.sHtML

[S12] C：写文件
来源：http://blog.tarul.cn/Article/details/gbizxwenx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gaaakxwne.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/ghdesvfbz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.epnwcf.com/Article/details/ghttpsjnn.sHtML

[S14] C：枚举
来源：http://3g.tarul.cn/Article/details/gzkmardwn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.bbcook.cn/Article/details/gtehoqdlv.sHtML

[S15] C：类型转换
来源：http://wap.yfazqb.com/Article/details/gkzeexmsn.sHtML

(double) a / b
来源：http://mobile.tarul.cn/Article/details/gooslmjwz.sHtML

[S16] C：位操作置位
来源：http://mobile.bbcook.cn/Article/details/gkjqmiuuk.sHtML

x |= (1 << 3);
来源：http://wap.vehdjk.com/Article/details/grfzuemkv.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/gjhpnvhhk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/gpjvcvdlc.sHtML

[S18] C：命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gipfwanrf.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fktsv.cn/Article/details/gakewqmxh.sHtML

[S19] C：快速排序
来源：http://3g.sjlbkw.cn/Article/details/gzwpdwogx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/grdxwvryx.sHtML

[S20] C：二分查找
来源：http://www.blog.vehdjk.com/Article/details/gcemgwayd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/gtzikhkuy.sHtML

[S21] C：字符类别判断
来源：http://read.share.yfazqb.com/Article/details/ggapsqncv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.bbcook.cn/Article/details/ghzltvwga.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gbidevncs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.bbcook.cn/Article/details/gkghlitim.sHtML

[S23] C：随机数
来源：http://read.share.fktsv.cn/Article/details/gsytjpyhv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.tarul.cn/Article/details/guyhqudog.sHtML

[S24] C：获取本地时间
来源：http://www.share.fktsv.cn/Article/details/gvsxhdqiw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.epnwcf.com/Article/details/gusxxcwgq.sHtML

[S25] C：内存拷贝
来源：http://baike.tarul.cn/Article/details/gmvisaift.sHtML

memcpy(dst, src, n);
来源：http://wap.vehdjk.com/Article/details/gtkvxcqud.sHtML

[S26] C：内存清零
来源：http://www.share.sjlbkw.cn/Article/details/gcdxxpvgm.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.vehdjk.com/Article/details/griggvquv.sHtML

[S27] C：定义常量
来源：http://wap.epnwcf.com/Article/details/gdacpxppc.sHtML

const double PI = 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gkequlhjs.sHtML

[S28] C：静态变量
来源：http://m.share.epnwcf.com/Article/details/guijvaftt.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/gayxwumtv.sHtML

[S29] C：变参函数
来源：http://wap.tarul.cn/Article/details/gscgtttnc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gskeovphg.sHtML

[S30] C：头文件保护
来源：http://www.share.vehdjk.com/Article/details/gffxlctlv.sHtML

#ifndef X_H
来源：http://www.m.share.epnwcf.com/Article/details/ghcbisbjj.sHtML

#define X_H
来源：http://3g.sjlbkw.cn/Article/details/gphvagobs.sHtML

#endif
来源：http://3g.yfazqb.com/Article/details/gasyfewko.sHtML

[S31] C++：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gudugirww.sHtML

#include <iostream>
来源：http://www.share.fktsv.cn/Article/details/gtouwvgoj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.tarul.cn/Article/details/guofgejfp.sHtML

[S32] C++：字符串
来源：http://3g.epnwcf.com/Article/details/gnhknvahl.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.tarul.cn/Article/details/gbgbaefgn.sHtML

[S33] C++：vector 增删
来源：http://www.share.bbcook.cn/Article/details/gvkwfildy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gxnnechmt.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/gkugcvapr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.tarul.cn/Article/details/gtuqvylfd.sHtML

[S35] C++：map
来源：http://wap.vehdjk.com/Article/details/ghiliiyxm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gejoioufs.sHtML

[S36] C++：unordered_map
来源：http://blog.tarul.cn/Article/details/ggumcmlae.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gevovqvcu.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/gtxbwkfkg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.sjlbkw.cn/Article/details/gxazjucbd.sHtML

[S38] C++：排序
来源：http://www.share.fktsv.cn/Article/details/glogzitlf.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.vehdjk.com/Article/details/gahcehplg.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.yfazqb.com/Article/details/gwkxbkclv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.epnwcf.com/Article/details/gqlujxnui.sHtML

[S40] C++：查找元素
来源：http://3g.yfazqb.com/Article/details/gzjvpssbt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.tarul.cn/Article/details/guvzjhckr.sHtML

[S41] C++：类与构造函数
来源：http://m.share.epnwcf.com/Article/details/gugwuetat.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.vehdjk.com/Article/details/ggbuosqpp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.tarul.cn/Article/details/guwqqbbyc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.yfazqb.com/Article/details/gyryaspoz.sHtML

[S43] C++：智能指针
来源：http://baike.tarul.cn/Article/details/gyvxuzyxs.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/gbdszwfba.sHtML

[S44] C++：引用传参
来源：http://www.share.bbcook.cn/Article/details/gieypvvtq.sHtML

void inc(int &x) { ++x; }
来源：http://baike.tarul.cn/Article/details/gprzdstnb.sHtML

[S45] C++：lambda
来源：http://m.share.tarul.cn/Article/details/glornfuwo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.tarul.cn/Article/details/glaaexsxi.sHtML

[S46] C++：函数模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gquscovbj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.vehdjk.com/Article/details/ggoxvsuin.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.vehdjk.com/Article/details/gxzdxgccv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.epnwcf.com/Article/details/gwsexfssf.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/ggtkuwcwi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.bbcook.cn/Article/details/gpxxlvkfi.sHtML

while (std::getline(in, line)) { }
来源：http://wap.epnwcf.com/Article/details/gesykadmi.sHtML

[S49] C++：写文件
来源：http://blog.vehdjk.com/Article/details/gwibqdveg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.epnwcf.com/Article/details/gbnqvuefc.sHtML

[S50] C++：格式化数字
来源：http://3g.tarul.cn/Article/details/gewfgqmxb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gvvxgzqhq.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/ggjifgifo.sHtML

static_cast<double>(a) / b
来源：http://mobile.sjlbkw.cn/Article/details/gjxfrxudn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fktsv.cn/Article/details/gusribcdd.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.epnwcf.com/Article/details/gzqqjtxth.sHtML

[S53] C++：移动语义
来源：http://blog.sjlbkw.cn/Article/details/gsolfhyym.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.vehdjk.com/Article/details/gijdbiytv.sHtML

[S54] C++：异常处理
来源：http://3g.yfazqb.com/Article/details/gmlucctiu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.epnwcf.com/Article/details/gyeaxfomh.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/gibkwfdjd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.epnwcf.com/Article/details/ghzvfysjm.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/gztxiboch.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.epnwcf.com/Article/details/gtmrttabh.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/guaxzhouj.sHtML

constexpr int N = 10;
来源：http://read.share.tarul.cn/Article/details/gyxzsthle.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fktsv.cn/Article/details/guaqnveba.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.vehdjk.com/Article/details/gtopzqzyh.sHtML

[S59] C++：静态断言
来源：http://read.share.tarul.cn/Article/details/gsflutytv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fktsv.cn/Article/details/gsopfrxtj.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.sjlbkw.cn/Article/details/gzfsxcttf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.epnwcf.com/Article/details/giptviapa.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gnyasumvx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.epnwcf.com/Article/details/gleyiqgzq.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grsjhpsrq.sHtML

[T01] Kotlin：Hello World
来源：http://baike.vehdjk.com/Article/details/gumowxbly.sHtML

println("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gxydtsadw.sHtML

[T02] Kotlin：变量
来源：http://mobile.vehdjk.com/Article/details/gfreduthc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.epnwcf.com/Article/details/grdhsrsqj.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.yfazqb.com/Article/details/gqxogjwaj.sHtML

"值: $b"
来源：http://read.share.yfazqb.com/Article/details/gbnzfunqc.sHtML

[T04] Kotlin：空安全
来源：http://3g.bbcook.cn/Article/details/guzlqppfo.sHtML

val n: String? = null;  n?.length
来源：http://mobile.sjlbkw.cn/Article/details/gbptjwmga.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.vehdjk.com/Article/details/gutaulzqd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.yfazqb.com/Article/details/gadgytdxj.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fktsv.cn/Article/details/gvxznxfff.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.vehdjk.com/Article/details/gbpajcrtu.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/gzdwjzeey.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.epnwcf.com/Article/details/gshzkvftq.sHtML

[T08] Kotlin：数据类
来源：http://www.share.tarul.cn/Article/details/giogmzkro.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.epnwcf.com/Article/details/gdijyiaaa.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fktsv.cn/Article/details/ghccnbohl.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.vehdjk.com/Article/details/gkxfxklmt.sHtML

[T10] Kotlin：默认参数
来源：http://blog.epnwcf.com/Article/details/gpdzrukce.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.bbcook.cn/Article/details/gzunyqmtg.sHtML


<!-- 参考信息 -->