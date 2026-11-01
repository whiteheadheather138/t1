代发 wailian999

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/gthndawrr.sHtML

[R04] 位置参数
来源：http://baike.bbcook.cn/Article/details/gsbagblit.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.bbcook.cn/Article/details/gcvrexhog.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/guyqjcqqm.sHtML

name="${1:-default}"
来源：http://www.blog.bbcook.cn/Article/details/gxlopxfhy.sHtML

[R06] 判断命令是否存在
来源：http://baike.tarul.cn/Article/details/gfvbvssii.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gjjvbbozb.sHtML

[R07] if 判断文件
来源：http://www.blog.sjlbkw.cn/Article/details/gxjiexnpy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.vehdjk.com/Article/details/gbmkfzrnv.sHtML

[R08] 数值比较
来源：http://www.blog.yfazqb.com/Article/details/gvottppir.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.vehdjk.com/Article/details/gyslgsmox.sHtML

[R09] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gypvjbhyg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.epnwcf.com/Article/details/gysepnhno.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/grkizbvqh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.epnwcf.com/Article/details/gmpkpxetu.sHtML

[R11] case 多分支
来源：http://wap.vehdjk.com/Article/details/gnjbhampu.sHtML

case "$1" in
来源：http://m.share.vehdjk.com/Article/details/giddjuboi.sHtML

start) echo "启动" ;;
来源：http://www.blog.bbcook.cn/Article/details/gtzlvyixu.sHtML

stop)  echo "停止" ;;
来源：http://blog.fktsv.cn/Article/details/gevtapznd.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.tarul.cn/Article/details/gnffftupg.sHtML

esac
来源：http://wap.tarul.cn/Article/details/gvsjsjrjk.sHtML

[R12] for 遍历文件
来源：http://m.share.epnwcf.com/Article/details/guslmwezp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.epnwcf.com/Article/details/gaigdtflv.sHtML

[R13] for 计数循环
来源：http://www.share.tarul.cn/Article/details/gpvruonrx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gyqgpalax.sHtML

[R14] C 风格 for
来源：http://www.share.sjlbkw.cn/Article/details/gtjwmoaxs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gvecrlwjs.sHtML

[R15] while 逐行读文件
来源：http://3g.bbcook.cn/Article/details/gmawahuoj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.sjlbkw.cn/Article/details/gifrponlc.sHtML

[R16] until 等待条件
来源：http://3g.epnwcf.com/Article/details/genytqhtz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.sjlbkw.cn/Article/details/gbypazlwp.sHtML

[R17] 数组定义与取值
来源：http://baike.yfazqb.com/Article/details/goxsjvrpq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.tarul.cn/Article/details/ggzdenfqd.sHtML

[R18] 遍历数组
来源：http://blog.bbcook.cn/Article/details/gnujkxhda.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.bbcook.cn/Article/details/gohmimcgz.sHtML

[R19] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gktldfdoa.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/grawbhabu.sHtML

[R20] 关联数组（字典）
来源：http://3g.tarul.cn/Article/details/gfziixvto.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.bbcook.cn/Article/details/ghotqkspx.sHtML

[R21] 字符串长度
来源：http://wap.vehdjk.com/Article/details/gadaqsuza.sHtML

echo "${#s}"
来源：http://www.blog.bbcook.cn/Article/details/gjrncgxag.sHtML

[R22] 截取子串
来源：http://wap.fktsv.cn/Article/details/gxjlistxq.sHtML

echo "${s:0:5}"
来源：http://www.share.yfazqb.com/Article/details/gjenqqunc.sHtML

[R23] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gebwbfhbg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fktsv.cn/Article/details/gitsueilm.sHtML

[R24] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/ganyhmxll.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.sjlbkw.cn/Article/details/gpxcuawro.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.vehdjk.com/Article/details/gsthpkkdl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.tarul.cn/Article/details/gcgtpfcar.sHtML

[R26] 命令替换
来源：http://blog.tarul.cn/Article/details/grloyhcfd.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fktsv.cn/Article/details/garnliybx.sHtML

[R27] 算术展开
来源：http://mobile.yfazqb.com/Article/details/gwlncbeur.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fktsv.cn/Article/details/gackwbxad.sHtML

[R28] 浮点运算
来源：http://m.share.epnwcf.com/Article/details/goafgbgiy.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/gbyuevcxg.sHtML

[R29] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpzhheds.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.vehdjk.com/Article/details/gwnujevbs.sHtML

[R30] 函数返回状态码
来源：http://www.blog.tarul.cn/Article/details/gilcvsiry.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.vehdjk.com/Article/details/gqbxoynqb.sHtML

[R31] 局部变量
来源：http://3g.vehdjk.com/Article/details/gbyxcjjmd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.tarul.cn/Article/details/glhrulihe.sHtML

[R32] 参数个数校验
来源：http://m.share.fktsv.cn/Article/details/gtpbuohqz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/gqtjilgja.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fktsv.cn/Article/details/godeaxbxc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.yfazqb.com/Article/details/gnrdbaono.sHtML

[R34] 退出时清理
来源：http://baike.epnwcf.com/Article/details/gimpdialo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gafldsyly.sHtML

[R35] 后台执行并等待
来源：http://mobile.tarul.cn/Article/details/gugujslun.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.bbcook.cn/Article/details/gireozrfe.sHtML

[R36] 并发执行多个任务
来源：http://wap.bbcook.cn/Article/details/ggcxyiuhj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fktsv.cn/Article/details/gjkoodyri.sHtML

[R37] 把输出赋给变量
来源：http://read.share.tarul.cn/Article/details/gwmvnmqcf.sHtML

files=$(ls -1)
来源：http://www.blog.vehdjk.com/Article/details/geqdvxaiq.sHtML

[R38] 管道串联
来源：http://baike.epnwcf.com/Article/details/gzsawryfl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.bbcook.cn/Article/details/gnwnoaemj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.yfazqb.com/Article/details/gxlggnnki.sHtML

cmd > out.log 2>&1
来源：http://blog.yfazqb.com/Article/details/gxvuojufz.sHtML

[R40] 追加写日志
来源：http://m.share.sjlbkw.cn/Article/details/gwjdtvroo.sHtML

echo "log" >> out.log
来源：http://baike.yfazqb.com/Article/details/gusprxqlx.sHtML

[R41] 丢弃输出
来源：http://read.share.sjlbkw.cn/Article/details/gllrjjksi.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.yfazqb.com/Article/details/gxjmdycrc.sHtML

[R42] 输入重定向
来源：http://read.share.tarul.cn/Article/details/ghuovzwji.sHtML

wc -l < a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gxrnpyxjq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.sjlbkw.cn/Article/details/gjvvrblmp.sHtML

find . -name "*.log" -type f
来源：http://3g.epnwcf.com/Article/details/gbdfqkrci.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/gesrijxdc.sHtML

find . -mtime -7 -type f
来源：http://read.share.bbcook.cn/Article/details/gdjacxtuc.sHtML

[R45] 批量删除
来源：http://www.blog.bbcook.cn/Article/details/gqfqjnrel.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.bbcook.cn/Article/details/gedogxxru.sHtML

[R46] 递归替换文件内容
来源：http://mobile.epnwcf.com/Article/details/gahwagtyd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.bbcook.cn/Article/details/gztpdppxi.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/glpqqdxci.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.epnwcf.com/Article/details/gdnnbxxbz.sHtML

[R48] awk 取指定列
来源：http://3g.sjlbkw.cn/Article/details/gubiaeqmb.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.vehdjk.com/Article/details/gvghmlaga.sHtML

[R49] awk 带条件
来源：http://www.blog.epnwcf.com/Article/details/gcbyghmrl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.sjlbkw.cn/Article/details/gbierzzbr.sHtML

[R50] awk 求和
来源：http://read.share.vehdjk.com/Article/details/gpjoggndk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gplozzjmt.sHtML

[R51] 排序去重取前几
来源：http://blog.vehdjk.com/Article/details/gnjdxqbuw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.tarul.cn/Article/details/gepohchee.sHtML

[R52] 统计行数
来源：http://blog.tarul.cn/Article/details/gdywipsad.sHtML

wc -l a.txt
来源：http://mobile.vehdjk.com/Article/details/glljwewto.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.bbcook.cn/Article/details/gvzdwvbjc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.epnwcf.com/Article/details/gtpadnyph.sHtML

[R54] 比较两个文件
来源：http://3g.bbcook.cn/Article/details/gqhnxakuw.sHtML

diff a.txt b.txt
来源：http://mobile.tarul.cn/Article/details/glokxuvpq.sHtML

[R55] 压缩与解压
来源：http://blog.fktsv.cn/Article/details/gpohkpdpr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.bbcook.cn/Article/details/gmaeazpce.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/gyxiizdhh.sHtML

scp file user@host:/path/
来源：http://mobile.yfazqb.com/Article/details/gygebqbqx.sHtML

[R57] 远程执行命令
来源：http://www.m.share.tarul.cn/Article/details/gttukjwog.sHtML

ssh user@host 'uptime'
来源：http://3g.tarul.cn/Article/details/gbjugebbr.sHtML

[R58] 下载文件
来源：http://wap.tarul.cn/Article/details/gvvqgbhsd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.vehdjk.com/Article/details/gbschskht.sHtML

[R59] 发 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gvkwaexrx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/gkdmaacfj.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gncqcqwsx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.sjlbkw.cn/Article/details/gwssglniw.sHtML

[R61] 磁盘占用
来源：http://m.share.vehdjk.com/Article/details/gahwsuuyu.sHtML

df -h;  du -sh *
来源：http://www.m.share.epnwcf.com/Article/details/gxvkwlaxj.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fktsv.cn/Article/details/grnowbqyb.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.sjlbkw.cn/Article/details/gigwoaedi.sHtML

[R63] 内存与进程
来源：http://blog.bbcook.cn/Article/details/gneancfbu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/gxbxajpyz.sHtML

[R64] 结束进程
来源：http://blog.tarul.cn/Article/details/gnakpsmeb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.sjlbkw.cn/Article/details/gechxzuqq.sHtML

[R65] 查看端口占用
来源：http://www.share.fktsv.cn/Article/details/gjxivgttp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.tarul.cn/Article/details/gvwrtpasp.sHtML

[R66] 定时任务
来源：http://m.share.bbcook.cn/Article/details/gdlwzcica.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/gwddkoqux.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.vehdjk.com/Article/details/gnypdjkux.sHtML

openssl rand -hex 16
来源：http://mobile.tarul.cn/Article/details/gnyrhfirz.sHtML

[R68] 计算文件校验值
来源：http://www.share.epnwcf.com/Article/details/gxgkxmyri.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.vehdjk.com/Article/details/gfehqczpf.sHtML

[R69] 生成随机密码
来源：http://m.share.fktsv.cn/Article/details/gxzbgljqo.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fktsv.cn/Article/details/gaykteirt.sHtML

[R70] 时间戳与互转
来源：http://m.share.vehdjk.com/Article/details/gozgtpnxv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.bbcook.cn/Article/details/gtcyysbwr.sHtML

[R71] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gvudftatt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fktsv.cn/Article/details/gdvfhwbvh.sHtML

[R72] 等待端口就绪
来源：http://baike.vehdjk.com/Article/details/gjpkhdkql.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gpmqiwunw.sHtML

[R73] 分割大日志
来源：http://www.m.share.yfazqb.com/Article/details/gognquuux.sHtML

split -l 1000 big.log part_
来源：http://m.share.tarul.cn/Article/details/gqystumpa.sHtML

[R74] 批量重命名
来源：http://wap.sjlbkw.cn/Article/details/gcqwkfrzh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.bbcook.cn/Article/details/gfgnssilc.sHtML

[R75] 导出环境变量
来源：http://blog.epnwcf.com/Article/details/gjasuabrn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.vehdjk.com/Article/details/gmnsyxcjd.sHtML

[R76] 使用临时文件
来源：http://m.share.vehdjk.com/Article/details/geomrdhdh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/gryqqzfal.sHtML

[R77] 读取用户输入
来源：http://www.share.bbcook.cn/Article/details/gshcqhwlc.sHtML

read -rp "请输入: " ans
来源：http://www.share.vehdjk.com/Article/details/gzlrsthze.sHtML

[R78] 交互式菜单
来源：http://mobile.tarul.cn/Article/details/gibuvzwql.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fktsv.cn/Article/details/gzqjgxpiw.sHtML

[R79] 解析命令行选项
来源：http://baike.fktsv.cn/Article/details/ggoehjhbp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/gnakxruwd.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.epnwcf.com/Article/details/galjvjjic.sHtML

time ./run.sh
来源：http://www.share.fktsv.cn/Article/details/gisbzmppw.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtbsujznu.sHtML

S. C / C++ 专题
来源：http://wap.epnwcf.com/Article/details/ghxchrrio.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjaqnlgwd.sHtML

[S01] C：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/ghcpdtpka.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/gjfcecpln.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.tarul.cn/Article/details/geoksslgs.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/grojgeqex.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.bbcook.cn/Article/details/gskaegcag.sHtML

[S03] C：读入整数
来源：http://wap.epnwcf.com/Article/details/gncgtnlpz.sHtML

int x; scanf("%d", &x);
来源：http://read.share.bbcook.cn/Article/details/gosjyievk.sHtML

[S04] C：字符串复制
来源：http://read.share.sjlbkw.cn/Article/details/gznfjuiyv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/gpzgeburf.sHtML

[S05] C：字符串长度
来源：http://www.share.bbcook.cn/Article/details/gvwzhjdxj.sHtML

strlen(s)
来源：http://wap.tarul.cn/Article/details/gkjispjgz.sHtML

[S06] C：字符串比较
来源：http://blog.yfazqb.com/Article/details/gyoueoola.sHtML

strcmp(a, b) == 0
来源：http://wap.epnwcf.com/Article/details/ghsdyxrvx.sHtML

[S07] C：数组遍历求和
来源：http://www.share.sjlbkw.cn/Article/details/gpiwpgapj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/grwwxyldq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.yfazqb.com/Article/details/gnumvuwan.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.sjlbkw.cn/Article/details/gfzefnjxe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.sjlbkw.cn/Article/details/giolmicnj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/gvzmtaoei.sHtML

[S10] C：指针与解引用
来源：http://www.blog.sjlbkw.cn/Article/details/gawpqutlv.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.vehdjk.com/Article/details/goziwhpjg.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/geftrypwt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fktsv.cn/Article/details/gdiubrksi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fktsv.cn/Article/details/gotpraill.sHtML

fclose(f);
来源：http://m.share.epnwcf.com/Article/details/gtnjwcbau.sHtML

[S12] C：写文件
来源：http://m.share.vehdjk.com/Article/details/grolyqgyt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.tarul.cn/Article/details/gupooxpzw.sHtML

[S13] C：宏定义
来源：http://3g.sjlbkw.cn/Article/details/gdsilsmfr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.sjlbkw.cn/Article/details/gxmesnrdo.sHtML

[S14] C：枚举
来源：http://www.m.share.bbcook.cn/Article/details/gnxezcsku.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.sjlbkw.cn/Article/details/gygdbhahy.sHtML

[S15] C：类型转换
来源：http://3g.tarul.cn/Article/details/gygrxqepd.sHtML

(double) a / b
来源：http://www.share.vehdjk.com/Article/details/gxcqxbelw.sHtML

[S16] C：位操作置位
来源：http://baike.sjlbkw.cn/Article/details/gpxxcjvze.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/gmvivlpro.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gnzhtntlz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.sjlbkw.cn/Article/details/gzrwheccf.sHtML

[S18] C：命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/gtglpuajz.sHtML

int main(int argc, char **argv)
来源：http://wap.vehdjk.com/Article/details/gicclxsmf.sHtML

[S19] C：快速排序
来源：http://3g.tarul.cn/Article/details/gqeuafmdv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gzvhvbgfs.sHtML

[S20] C：二分查找
来源：http://www.share.fktsv.cn/Article/details/gvmaechze.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gnphgthce.sHtML

[S21] C：字符类别判断
来源：http://read.share.tarul.cn/Article/details/gozixnsbi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fktsv.cn/Article/details/gqjvoqijw.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/gdmljazpd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.vehdjk.com/Article/details/gwmuwbvwj.sHtML

[S23] C：随机数
来源：http://www.m.share.yfazqb.com/Article/details/gxjrjiibt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.bbcook.cn/Article/details/gmfzjfrgg.sHtML

[S24] C：获取本地时间
来源：http://read.share.vehdjk.com/Article/details/govgbosol.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fktsv.cn/Article/details/gnkyjivii.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fktsv.cn/Article/details/gebxezali.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fktsv.cn/Article/details/gpdsnhspz.sHtML

[S26] C：内存清零
来源：http://read.share.epnwcf.com/Article/details/gtcrvwtzf.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/gvtkehdxe.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/grkyygkwv.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gavptgill.sHtML

[S28] C：静态变量
来源：http://read.share.sjlbkw.cn/Article/details/gzdxrrucw.sHtML

static int counter = 0;
来源：http://m.share.tarul.cn/Article/details/ghhfhjorq.sHtML

[S29] C：变参函数
来源：http://m.share.sjlbkw.cn/Article/details/gqlrpruqr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/glmzohmjc.sHtML

[S30] C：头文件保护
来源：http://baike.yfazqb.com/Article/details/gtgjgsykl.sHtML

#ifndef X_H
来源：http://m.share.yfazqb.com/Article/details/gbmphqrvm.sHtML

#define X_H
来源：http://wap.bbcook.cn/Article/details/gwllcyalx.sHtML

#endif
来源：http://wap.fktsv.cn/Article/details/gfhcdfhcg.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gzporuoic.sHtML

#include <iostream>
来源：http://www.share.epnwcf.com/Article/details/giuhkeaga.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.yfazqb.com/Article/details/gwhmfgwll.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/grbtfvneh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.bbcook.cn/Article/details/goxgxjolb.sHtML

[S33] C++：vector 增删
来源：http://www.share.vehdjk.com/Article/details/gackdrbtg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.epnwcf.com/Article/details/gwwvkubod.sHtML

[S34] C++：遍历 vector
来源：http://mobile.yfazqb.com/Article/details/gbsivqqqw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.vehdjk.com/Article/details/gxnsaelcy.sHtML

[S35] C++：map
来源：http://baike.yfazqb.com/Article/details/giaheowqf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/gpwhqbxur.sHtML

[S36] C++：unordered_map
来源：http://www.share.sjlbkw.cn/Article/details/gqiwjkctv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gkvkwhkzx.sHtML

[S37] C++：set
来源：http://blog.yfazqb.com/Article/details/glolvgich.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/gavskeico.sHtML

[S38] C++：排序
来源：http://read.share.sjlbkw.cn/Article/details/gdrfcfoeb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.epnwcf.com/Article/details/gyajsfwuz.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.yfazqb.com/Article/details/gspbhyrmp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/gpzlgszcp.sHtML

[S40] C++：查找元素
来源：http://www.share.yfazqb.com/Article/details/gavmjlmly.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.yfazqb.com/Article/details/gaqlntvyt.sHtML

[S41] C++：类与构造函数
来源：http://blog.sjlbkw.cn/Article/details/gdnwaudpo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.sjlbkw.cn/Article/details/gmgmtycay.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.epnwcf.com/Article/details/gnkoxylye.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.epnwcf.com/Article/details/gdropmvja.sHtML

[S43] C++：智能指针
来源：http://www.m.share.tarul.cn/Article/details/gtjmiaaam.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.bbcook.cn/Article/details/gmhqnpbvh.sHtML

[S44] C++：引用传参
来源：http://www.blog.sjlbkw.cn/Article/details/guhcncoym.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fktsv.cn/Article/details/gdksqkror.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/giztxyhvv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.vehdjk.com/Article/details/gtftxnghi.sHtML

[S46] C++：函数模板
来源：http://www.m.share.yfazqb.com/Article/details/gfsclprwp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fktsv.cn/Article/details/gvpsssbiv.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fktsv.cn/Article/details/gbgygeyxi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.vehdjk.com/Article/details/gmxckoyme.sHtML

[S48] C++：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gfrchtxkz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.sjlbkw.cn/Article/details/ghmphxqah.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.yfazqb.com/Article/details/gzfovheuu.sHtML

[S49] C++：写文件
来源：http://3g.sjlbkw.cn/Article/details/gsrpmioeb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.sjlbkw.cn/Article/details/gatnakqhj.sHtML

[S50] C++：格式化数字
来源：http://mobile.fktsv.cn/Article/details/gwydijiea.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.bbcook.cn/Article/details/gxfolryeh.sHtML

[S51] C++：显式类型转换
来源：http://baike.yfazqb.com/Article/details/gqnofraui.sHtML

static_cast<double>(a) / b
来源：http://www.share.epnwcf.com/Article/details/gjtjvwksb.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.bbcook.cn/Article/details/gqlrsvcdo.sHtML

int size() const noexcept { return n_; }
来源：http://baike.epnwcf.com/Article/details/ghuqyvtty.sHtML

[S53] C++：移动语义
来源：http://3g.epnwcf.com/Article/details/glfcrfevk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.vehdjk.com/Article/details/ggprxhffy.sHtML

[S54] C++：异常处理
来源：http://3g.epnwcf.com/Article/details/gjkvaewvw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.sjlbkw.cn/Article/details/ggergydtx.sHtML

[S55] C++：结构化绑定
来源：http://mobile.yfazqb.com/Article/details/gvqttjsfq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.epnwcf.com/Article/details/gtyhptjyp.sHtML

[S56] C++：optional
来源：http://mobile.yfazqb.com/Article/details/ggxbdlwgb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.yfazqb.com/Article/details/gtttiqfui.sHtML

[S57] C++：编译期常量
来源：http://read.share.sjlbkw.cn/Article/details/ggaalqzud.sHtML

constexpr int N = 10;
来源：http://mobile.epnwcf.com/Article/details/glvyoorln.sHtML

[S58] C++：命名空间
来源：http://wap.sjlbkw.cn/Article/details/geucbxocj.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.epnwcf.com/Article/details/gkuwioqyz.sHtML

[S59] C++：静态断言
来源：http://read.share.bbcook.cn/Article/details/grxgkbfop.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.tarul.cn/Article/details/gypepdmyl.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fktsv.cn/Article/details/ghqdzelqx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.epnwcf.com/Article/details/gsijclfai.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gelpzvqbi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/gcsqdqqsa.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gxropgdui.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gvfplaehb.sHtML

println("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gukihnbev.sHtML

[T02] Kotlin：变量
来源：http://blog.sjlbkw.cn/Article/details/grsjhtibt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.epnwcf.com/Article/details/gimsglclk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.vehdjk.com/Article/details/gzihibbhc.sHtML

"值: $b"
来源：http://baike.fktsv.cn/Article/details/gpmusfohx.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.sjlbkw.cn/Article/details/gmcswibge.sHtML

val n: String? = null;  n?.length
来源：http://blog.sjlbkw.cn/Article/details/ghkqamljr.sHtML


<!-- 参考信息 -->