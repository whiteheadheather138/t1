代发 wailian999

readonly PI=3.14
来源：http://baike.bbcook.cn/Article/details/gpfgwidrg.sHtML

[R04] 位置参数
来源：http://www.m.share.tarul.cn/Article/details/gdphggwbj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmknmrqa.sHtML

[R05] 参数默认值
来源：http://mobile.bbcook.cn/Article/details/gupbtcpan.sHtML

name="${1:-default}"
来源：http://wap.fktsv.cn/Article/details/gedtjmubr.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fktsv.cn/Article/details/ghsbpshcd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/grssbacgt.sHtML

[R07] if 判断文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdnbbexe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/geqvfzhgc.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/geugdpcgz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gmlzemwpq.sHtML

[R09] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gjejwegai.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fktsv.cn/Article/details/gwheotkjs.sHtML

[R10] 正则匹配
来源：http://mobile.yfazqb.com/Article/details/gqlkdomle.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.yfazqb.com/Article/details/gpekevyxo.sHtML

[R11] case 多分支
来源：http://baike.bbcook.cn/Article/details/gjkmpxcax.sHtML

case "$1" in
来源：http://www.share.yfazqb.com/Article/details/gtwjmoxix.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/gdvpndkso.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.bbcook.cn/Article/details/giloflnnh.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.bbcook.cn/Article/details/glflqoswl.sHtML

esac
来源：http://3g.yfazqb.com/Article/details/gygkwigzk.sHtML

[R12] for 遍历文件
来源：http://blog.tarul.cn/Article/details/ghejlatro.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.yfazqb.com/Article/details/glqrhipai.sHtML

[R13] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/gklavshew.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/glwqyfohp.sHtML

[R14] C 风格 for
来源：http://www.blog.sjlbkw.cn/Article/details/ghawmvltv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gtldifwca.sHtML

[R15] while 逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gqqtuilod.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fktsv.cn/Article/details/gvjfmvunb.sHtML

[R16] until 等待条件
来源：http://wap.fktsv.cn/Article/details/ggvemseqa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gumqqggxp.sHtML

[R17] 数组定义与取值
来源：http://baike.tarul.cn/Article/details/gydiqawtf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.yfazqb.com/Article/details/ganikavxi.sHtML

[R18] 遍历数组
来源：http://3g.epnwcf.com/Article/details/gzmuvzpsy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.tarul.cn/Article/details/gccqjohzs.sHtML

[R19] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gfhazwnlz.sHtML

echo "${#arr[@]}"
来源：http://3g.yfazqb.com/Article/details/gulskoozu.sHtML

[R20] 关联数组（字典）
来源：http://www.share.vehdjk.com/Article/details/gazvlaaoy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.vehdjk.com/Article/details/ghtsvxbdx.sHtML

[R21] 字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gfsfaghxr.sHtML

echo "${#s}"
来源：http://www.m.share.vehdjk.com/Article/details/gexhyuwtk.sHtML

[R22] 截取子串
来源：http://wap.vehdjk.com/Article/details/gqicskscr.sHtML

echo "${s:0:5}"
来源：http://mobile.vehdjk.com/Article/details/gmygmrfdm.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gayzhepab.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.bbcook.cn/Article/details/ghsvhhcnp.sHtML

[R24] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gmhxbcyrw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/gszlnnqom.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.tarul.cn/Article/details/gxyoszkvy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.epnwcf.com/Article/details/gpwhwhnff.sHtML

[R26] 命令替换
来源：http://wap.yfazqb.com/Article/details/ghiivuhhh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fktsv.cn/Article/details/gmknedgrb.sHtML

[R27] 算术展开
来源：http://www.m.share.yfazqb.com/Article/details/gzofizwjk.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.bbcook.cn/Article/details/gmaydonrw.sHtML

[R28] 浮点运算
来源：http://www.blog.yfazqb.com/Article/details/gfkzbncqf.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/gyjyxdsya.sHtML

[R29] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gehjfghht.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.yfazqb.com/Article/details/gzlczpjeb.sHtML

[R30] 函数返回状态码
来源：http://m.share.fktsv.cn/Article/details/ggemlhmdp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.epnwcf.com/Article/details/gqvvvkbqn.sHtML

[R31] 局部变量
来源：http://m.share.fktsv.cn/Article/details/gkcriczqd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.tarul.cn/Article/details/gtwnwkzyh.sHtML

[R32] 参数个数校验
来源：http://m.share.fktsv.cn/Article/details/gokligyrv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/gmjqrfriy.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.tarul.cn/Article/details/gceaobcdf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.bbcook.cn/Article/details/gncgadcxk.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/gqxpkmevc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gdmqmkpeb.sHtML

[R35] 后台执行并等待
来源：http://mobile.fktsv.cn/Article/details/guitvrpza.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.epnwcf.com/Article/details/gglteqaro.sHtML

[R36] 并发执行多个任务
来源：http://wap.sjlbkw.cn/Article/details/gzzvidgbq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.epnwcf.com/Article/details/giwbuuvqe.sHtML

[R37] 把输出赋给变量
来源：http://3g.epnwcf.com/Article/details/gbjaizbri.sHtML

files=$(ls -1)
来源：http://www.blog.epnwcf.com/Article/details/gdxzynycj.sHtML

[R38] 管道串联
来源：http://read.share.yfazqb.com/Article/details/gempecgxw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fktsv.cn/Article/details/gmjiboloh.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.sjlbkw.cn/Article/details/gqjhxjxym.sHtML

cmd > out.log 2>&1
来源：http://www.share.vehdjk.com/Article/details/gghjyxlzg.sHtML

[R40] 追加写日志
来源：http://blog.bbcook.cn/Article/details/gbcgakgde.sHtML

echo "log" >> out.log
来源：http://mobile.fktsv.cn/Article/details/grbmpobxg.sHtML

[R41] 丢弃输出
来源：http://read.share.tarul.cn/Article/details/gjqeszjhk.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fktsv.cn/Article/details/gkircgylu.sHtML

[R42] 输入重定向
来源：http://wap.vehdjk.com/Article/details/gsiykgmzf.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/gpvkrisse.sHtML

[R43] 按名字查找文件
来源：http://read.share.vehdjk.com/Article/details/gpncsnvag.sHtML

find . -name "*.log" -type f
来源：http://3g.sjlbkw.cn/Article/details/gvtgboejy.sHtML

[R44] 按修改时间查找
来源：http://blog.vehdjk.com/Article/details/guefyvdpo.sHtML

find . -mtime -7 -type f
来源：http://wap.vehdjk.com/Article/details/gaekzwuyh.sHtML

[R45] 批量删除
来源：http://baike.tarul.cn/Article/details/gjxrkhzwg.sHtML

find . -name "*.tmp" -delete
来源：http://blog.bbcook.cn/Article/details/gnimrzylr.sHtML

[R46] 递归替换文件内容
来源：http://read.share.bbcook.cn/Article/details/gudyvfcks.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.sjlbkw.cn/Article/details/gsbevcsjc.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/gkbfgnnog.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gwoizscjm.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/gjdpcasbz.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fktsv.cn/Article/details/grlejkubf.sHtML

[R49] awk 带条件
来源：http://read.share.vehdjk.com/Article/details/gsewbmrka.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.yfazqb.com/Article/details/gyzlatsdc.sHtML

[R50] awk 求和
来源：http://www.share.fktsv.cn/Article/details/godnyobar.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gxvmdcaec.sHtML

[R51] 排序去重取前几
来源：http://blog.epnwcf.com/Article/details/gahsluhds.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.epnwcf.com/Article/details/gfvtmdoti.sHtML

[R52] 统计行数
来源：http://read.share.sjlbkw.cn/Article/details/gebepiate.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/gekczbwrm.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.vehdjk.com/Article/details/gatvqrxls.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.bbcook.cn/Article/details/gjjrvdlta.sHtML

[R54] 比较两个文件
来源：http://www.share.sjlbkw.cn/Article/details/gmnspjbvw.sHtML

diff a.txt b.txt
来源：http://www.share.tarul.cn/Article/details/gcyaqpvwi.sHtML

[R55] 压缩与解压
来源：http://m.share.fktsv.cn/Article/details/gqzzlrtet.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.tarul.cn/Article/details/gejsrgibb.sHtML

[R56] 远程拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gcimkjnpi.sHtML

scp file user@host:/path/
来源：http://m.share.fktsv.cn/Article/details/ghpzkskcr.sHtML

[R57] 远程执行命令
来源：http://mobile.epnwcf.com/Article/details/gmgwozrvp.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/gxjjzcjbk.sHtML

[R58] 下载文件
来源：http://wap.tarul.cn/Article/details/gjixflrha.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.yfazqb.com/Article/details/goumekumw.sHtML

[R59] 发 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gjenzsycy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.epnwcf.com/Article/details/gpxcvnoaq.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/glmckogkn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.tarul.cn/Article/details/gyxiemllv.sHtML

[R61] 磁盘占用
来源：http://www.blog.sjlbkw.cn/Article/details/gkplmblpu.sHtML

df -h;  du -sh *
来源：http://read.share.sjlbkw.cn/Article/details/ghcxlzmdk.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.tarul.cn/Article/details/gtchrnwbb.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.vehdjk.com/Article/details/gqxudkmpg.sHtML

[R63] 内存与进程
来源：http://www.m.share.epnwcf.com/Article/details/gfxzljari.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.bbcook.cn/Article/details/gltiozpuc.sHtML

[R64] 结束进程
来源：http://www.blog.vehdjk.com/Article/details/gcnjinqip.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.yfazqb.com/Article/details/gyrdjrgvu.sHtML

[R65] 查看端口占用
来源：http://www.blog.vehdjk.com/Article/details/guuvguyji.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.tarul.cn/Article/details/gslmyfpsa.sHtML

[R66] 定时任务
来源：http://m.share.tarul.cn/Article/details/gnjlxuius.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.tarul.cn/Article/details/gmanlsfcq.sHtML

[R67] 生成随机十六进制串
来源：http://3g.sjlbkw.cn/Article/details/gtdxmzbxz.sHtML

openssl rand -hex 16
来源：http://mobile.fktsv.cn/Article/details/gzbblxsqr.sHtML

[R68] 计算文件校验值
来源：http://read.share.bbcook.cn/Article/details/gyftvcqpd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.vehdjk.com/Article/details/gydtmrnct.sHtML

[R69] 生成随机密码
来源：http://read.share.tarul.cn/Article/details/gmymbkrld.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fktsv.cn/Article/details/glylgkyvx.sHtML

[R70] 时间戳与互转
来源：http://baike.sjlbkw.cn/Article/details/gylaffyys.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.tarul.cn/Article/details/guavdgsbs.sHtML

[R71] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gjbqqibay.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.sjlbkw.cn/Article/details/gnsozjlcw.sHtML

[R72] 等待端口就绪
来源：http://www.share.tarul.cn/Article/details/gujbjerfc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gflzodnnn.sHtML

[R73] 分割大日志
来源：http://www.blog.tarul.cn/Article/details/geuejdvft.sHtML

split -l 1000 big.log part_
来源：http://wap.fktsv.cn/Article/details/gfkjcrjlt.sHtML

[R74] 批量重命名
来源：http://mobile.bbcook.cn/Article/details/gimzlmjom.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/gvxpshymc.sHtML

[R75] 导出环境变量
来源：http://baike.yfazqb.com/Article/details/gqpihtuka.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fktsv.cn/Article/details/gholdjfph.sHtML

[R76] 使用临时文件
来源：http://blog.yfazqb.com/Article/details/gqnjvxfxx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/gdaznulnf.sHtML

[R77] 读取用户输入
来源：http://mobile.yfazqb.com/Article/details/guucqfvqf.sHtML

read -rp "请输入: " ans
来源：http://baike.sjlbkw.cn/Article/details/ghhslrhhi.sHtML

[R78] 交互式菜单
来源：http://www.share.fktsv.cn/Article/details/gamsntngj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.yfazqb.com/Article/details/gxrkwhnyl.sHtML

[R79] 解析命令行选项
来源：http://3g.epnwcf.com/Article/details/gunrjbvwn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.yfazqb.com/Article/details/gwrxcoiqi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.bbcook.cn/Article/details/grbgjepur.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gweimqimw.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gruckznjv.sHtML

S. C / C++ 专题
来源：http://wap.fktsv.cn/Article/details/gbwgwvwxe.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gvqodrxsw.sHtML

[S01] C：Hello World
来源：http://wap.epnwcf.com/Article/details/goqgsnirp.sHtML

#include <stdio.h>
来源：http://m.share.bbcook.cn/Article/details/gjpusydbu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.tarul.cn/Article/details/genpbepxz.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gsbsabtiw.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.tarul.cn/Article/details/gsazrdpqa.sHtML

[S03] C：读入整数
来源：http://baike.vehdjk.com/Article/details/gkscnfymt.sHtML

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/gyrexztyn.sHtML

[S04] C：字符串复制
来源：http://baike.yfazqb.com/Article/details/gpqhobarj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.epnwcf.com/Article/details/gwvklrvvl.sHtML

[S05] C：字符串长度
来源：http://m.share.tarul.cn/Article/details/glaewkhwb.sHtML

strlen(s)
来源：http://blog.vehdjk.com/Article/details/gcxawnovx.sHtML

[S06] C：字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gzjgcauel.sHtML

strcmp(a, b) == 0
来源：http://www.blog.bbcook.cn/Article/details/gyiukuxbi.sHtML

[S07] C：数组遍历求和
来源：http://baike.vehdjk.com/Article/details/govnikbtx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.yfazqb.com/Article/details/giqdrsqwy.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.sjlbkw.cn/Article/details/gbncterxa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.vehdjk.com/Article/details/gppqyckkr.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.bbcook.cn/Article/details/gwwzijkyd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/gpdcnwcph.sHtML

[S10] C：指针与解引用
来源：http://m.share.epnwcf.com/Article/details/gyhjhsgwe.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.epnwcf.com/Article/details/grtubefbt.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gloqyglfg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.tarul.cn/Article/details/gydctoqlz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.tarul.cn/Article/details/gvzoafusi.sHtML

fclose(f);
来源：http://baike.tarul.cn/Article/details/gtnsywicp.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/gantezchd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/gendawedr.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gsuertvpf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.bbcook.cn/Article/details/gmmhwabfb.sHtML

[S14] C：枚举
来源：http://read.share.tarul.cn/Article/details/gtrbiycib.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.epnwcf.com/Article/details/gdbabjxhu.sHtML

[S15] C：类型转换
来源：http://mobile.bbcook.cn/Article/details/gabptftcv.sHtML

(double) a / b
来源：http://www.m.share.yfazqb.com/Article/details/gwplinnts.sHtML

[S16] C：位操作置位
来源：http://www.share.yfazqb.com/Article/details/gehvciien.sHtML

x |= (1 << 3);
来源：http://read.share.bbcook.cn/Article/details/gecmqoubj.sHtML

[S17] C：安全拼接字符串
来源：http://3g.yfazqb.com/Article/details/gcwhaktyp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.tarul.cn/Article/details/gvxqhykjm.sHtML

[S18] C：命令行参数
来源：http://mobile.bbcook.cn/Article/details/gplbwfkqh.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/gecrynogd.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/gbaelftur.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gzqpexoxy.sHtML

[S20] C：二分查找
来源：http://www.blog.vehdjk.com/Article/details/gmgpmsbfr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gnhnwgtxj.sHtML

[S21] C：字符类别判断
来源：http://baike.epnwcf.com/Article/details/gklytescp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.sjlbkw.cn/Article/details/gizupnwlu.sHtML

[S22] C：字符串转数字
来源：http://mobile.bbcook.cn/Article/details/ghslpvsri.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/glsdtalxc.sHtML

[S23] C：随机数
来源：http://m.share.sjlbkw.cn/Article/details/gthhwkwot.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.sjlbkw.cn/Article/details/grfklsawa.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fktsv.cn/Article/details/gbmqsyxxe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.yfazqb.com/Article/details/giskixcok.sHtML

[S25] C：内存拷贝
来源：http://blog.fktsv.cn/Article/details/gykuiqwif.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwegboqx.sHtML

[S26] C：内存清零
来源：http://blog.vehdjk.com/Article/details/gdintdcfb.sHtML

memset(a, 0, sizeof a);
来源：http://3g.yfazqb.com/Article/details/grxjxwtsm.sHtML

[S27] C：定义常量
来源：http://baike.fktsv.cn/Article/details/gfuqwerkz.sHtML

const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gjjpvunhm.sHtML

[S28] C：静态变量
来源：http://3g.sjlbkw.cn/Article/details/gtutlmfvj.sHtML

static int counter = 0;
来源：http://baike.epnwcf.com/Article/details/galfarvgx.sHtML

[S29] C：变参函数
来源：http://read.share.fktsv.cn/Article/details/gvydmzwro.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.yfazqb.com/Article/details/gqlzejnjz.sHtML

[S30] C：头文件保护
来源：http://read.share.yfazqb.com/Article/details/gwxwlyzmy.sHtML

#ifndef X_H
来源：http://www.share.sjlbkw.cn/Article/details/gzdspikzs.sHtML

#define X_H
来源：http://www.share.fktsv.cn/Article/details/gdkymbzqo.sHtML

#endif
来源：http://www.blog.sjlbkw.cn/Article/details/gmgjfmltq.sHtML

[S31] C++：Hello World
来源：http://blog.vehdjk.com/Article/details/ggicndhvn.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/ghncoqzwn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.tarul.cn/Article/details/gmnqdfsez.sHtML

[S32] C++：字符串
来源：http://read.share.epnwcf.com/Article/details/gsjhdtndz.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.vehdjk.com/Article/details/gdaapydwu.sHtML

[S33] C++：vector 增删
来源：http://m.share.fktsv.cn/Article/details/gjfoyggiq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.tarul.cn/Article/details/gvdftdbjs.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/gyrvswyxo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fktsv.cn/Article/details/gkpvudlmf.sHtML

[S35] C++：map
来源：http://www.share.fktsv.cn/Article/details/ggweigjdi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/gssadihia.sHtML

[S36] C++：unordered_map
来源：http://read.share.bbcook.cn/Article/details/gcwrijauv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gnumzinrk.sHtML

[S37] C++：set
来源：http://3g.vehdjk.com/Article/details/grcbnqgon.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fktsv.cn/Article/details/guznhwqyq.sHtML

[S38] C++：排序
来源：http://read.share.sjlbkw.cn/Article/details/gepdfrcrx.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.tarul.cn/Article/details/giytiwbcl.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.vehdjk.com/Article/details/gkngxvdtg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.bbcook.cn/Article/details/gedwbflcm.sHtML

[S40] C++：查找元素
来源：http://baike.yfazqb.com/Article/details/gwyszptci.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.sjlbkw.cn/Article/details/gfrifwcdt.sHtML

[S41] C++：类与构造函数
来源：http://3g.bbcook.cn/Article/details/ghhjqdole.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.bbcook.cn/Article/details/gdwwienoz.sHtML

[S42] C++：继承与虚函数
来源：http://wap.yfazqb.com/Article/details/gvwgzkhqq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.bbcook.cn/Article/details/gakjpvtsl.sHtML

[S43] C++：智能指针
来源：http://m.share.fktsv.cn/Article/details/gqgsvouxy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.vehdjk.com/Article/details/gaabsrtui.sHtML

[S44] C++：引用传参
来源：http://www.blog.bbcook.cn/Article/details/gmejwqajv.sHtML

void inc(int &x) { ++x; }
来源：http://wap.epnwcf.com/Article/details/gqzgppxmh.sHtML

[S45] C++：lambda
来源：http://www.share.tarul.cn/Article/details/gjuuejqgb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gvdjhrpqr.sHtML

[S46] C++：函数模板
来源：http://baike.vehdjk.com/Article/details/gobjciayn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fktsv.cn/Article/details/gqjyuenzh.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/gfgmflvzh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.sjlbkw.cn/Article/details/gxoiaydqd.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gwwdxzuhy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.vehdjk.com/Article/details/gnvfmsrrl.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.bbcook.cn/Article/details/gwgwwmewe.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/ghoqypccm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.tarul.cn/Article/details/gviycynug.sHtML

[S50] C++：格式化数字
来源：http://3g.sjlbkw.cn/Article/details/gckqhppdi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gozmrwmax.sHtML

[S51] C++：显式类型转换
来源：http://m.share.vehdjk.com/Article/details/gzoctzxnk.sHtML

static_cast<double>(a) / b
来源：http://mobile.fktsv.cn/Article/details/guxiamkcq.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/gxjgxvdlh.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fktsv.cn/Article/details/gqucqwwvx.sHtML

[S53] C++：移动语义
来源：http://blog.sjlbkw.cn/Article/details/gimeyjhya.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.tarul.cn/Article/details/gamfrtets.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/gkonbagxz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fktsv.cn/Article/details/gnttphuak.sHtML

[S55] C++：结构化绑定
来源：http://baike.fktsv.cn/Article/details/gwtekxtza.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.epnwcf.com/Article/details/goxnlpxzr.sHtML

[S56] C++：optional
来源：http://www.share.sjlbkw.cn/Article/details/gopsrtoml.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.epnwcf.com/Article/details/gbhsknbey.sHtML

[S57] C++：编译期常量
来源：http://m.share.epnwcf.com/Article/details/ghdrlemhp.sHtML

constexpr int N = 10;
来源：http://m.share.vehdjk.com/Article/details/gebatdxig.sHtML

[S58] C++：命名空间
来源：http://blog.fktsv.cn/Article/details/grawcwfkz.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.bbcook.cn/Article/details/gqznvgcda.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/gzggyvuzx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fktsv.cn/Article/details/gndhwxvko.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.vehdjk.com/Article/details/gshzgtdcq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gedzkqxvn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghckuxkvy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.sjlbkw.cn/Article/details/gkumqmppw.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gnfyubups.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/ghjlfxavo.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gosmowzay.sHtML

[T02] Kotlin：变量
来源：http://3g.tarul.cn/Article/details/getnrhihj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.yfazqb.com/Article/details/gevvtwxgs.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.epnwcf.com/Article/details/ggnkasnqg.sHtML

"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/gfvnecsrf.sHtML

[T04] Kotlin：空安全
来源：http://3g.fktsv.cn/Article/details/gozeeiwjs.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.vehdjk.com/Article/details/gugutvxvq.sHtML


<!-- 参考信息 -->