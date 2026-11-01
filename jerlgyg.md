代发 wailian999

readonly PI=3.14
来源：http://www.m.share.yfazqb.com/Article/details/gvesenatq.sHtML

[R04] 位置参数
来源：http://www.share.bbcook.cn/Article/details/gowmfjiig.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.sjlbkw.cn/Article/details/gkqversux.sHtML

[R05] 参数默认值
来源：http://read.share.bbcook.cn/Article/details/gkbegteoa.sHtML

name="${1:-default}"
来源：http://read.share.epnwcf.com/Article/details/gyrkrutvo.sHtML

[R06] 判断命令是否存在
来源：http://m.share.tarul.cn/Article/details/goiiaydwd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/grjnmmaex.sHtML

[R07] if 判断文件
来源：http://m.share.epnwcf.com/Article/details/gohtymfcd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.epnwcf.com/Article/details/geuqifxev.sHtML

[R08] 数值比较
来源：http://m.share.fktsv.cn/Article/details/grpyaghke.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.bbcook.cn/Article/details/gjebglmdg.sHtML

[R09] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gfwjdlndt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.bbcook.cn/Article/details/geucozkha.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/gtvnewgrd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fktsv.cn/Article/details/gnmyviiyi.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/gvasqfkeq.sHtML

case "$1" in
来源：http://blog.yfazqb.com/Article/details/gqjdlfmjg.sHtML

start) echo "启动" ;;
来源：http://blog.fktsv.cn/Article/details/gpyvapuos.sHtML

stop)  echo "停止" ;;
来源：http://wap.sjlbkw.cn/Article/details/gnszofbug.sHtML

*)     echo "未知命令" ;;
来源：http://3g.sjlbkw.cn/Article/details/gkwwwmwbt.sHtML

esac
来源：http://baike.epnwcf.com/Article/details/gnztcvbfv.sHtML

[R12] for 遍历文件
来源：http://3g.epnwcf.com/Article/details/gsddbjbbj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.bbcook.cn/Article/details/gscymnliu.sHtML

[R13] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gpdjdnppa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gzudpbqyc.sHtML

[R14] C 风格 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuorigym.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.bbcook.cn/Article/details/glmjgyasf.sHtML

[R15] while 逐行读文件
来源：http://read.share.fktsv.cn/Article/details/ghwjhmvvv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.epnwcf.com/Article/details/gkkqzagjg.sHtML

[R16] until 等待条件
来源：http://baike.vehdjk.com/Article/details/gvylsljrk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gtgpjboac.sHtML

[R17] 数组定义与取值
来源：http://blog.sjlbkw.cn/Article/details/gzeickvca.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.tarul.cn/Article/details/gcqiyhlak.sHtML

[R18] 遍历数组
来源：http://blog.yfazqb.com/Article/details/gtlkqmxcr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.bbcook.cn/Article/details/gofjmowei.sHtML

[R19] 数组长度
来源：http://3g.bbcook.cn/Article/details/guozbqidr.sHtML

echo "${#arr[@]}"
来源：http://3g.bbcook.cn/Article/details/givwbuzxf.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fktsv.cn/Article/details/gmhsblmra.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/gagmqnrsz.sHtML

[R21] 字符串长度
来源：http://3g.yfazqb.com/Article/details/geusphmoc.sHtML

echo "${#s}"
来源：http://wap.yfazqb.com/Article/details/gmisxpcyt.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/gpqbppien.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/gvfkdwyus.sHtML

[R23] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gvcljrech.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fktsv.cn/Article/details/geakwkdve.sHtML

[R24] 大小写转换
来源：http://blog.yfazqb.com/Article/details/godololof.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.bbcook.cn/Article/details/gljcrvpwk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.epnwcf.com/Article/details/giussnhvm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.epnwcf.com/Article/details/gbdlhdmwg.sHtML

[R26] 命令替换
来源：http://m.share.bbcook.cn/Article/details/gsokksnek.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fktsv.cn/Article/details/gavjokaga.sHtML

[R27] 算术展开
来源：http://baike.bbcook.cn/Article/details/gxjqyncgu.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.tarul.cn/Article/details/gdqcbinia.sHtML

[R28] 浮点运算
来源：http://www.blog.fktsv.cn/Article/details/gacxolihw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.tarul.cn/Article/details/gqvbmpzbl.sHtML

[R29] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/gohxzejcm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/gpxyaxfjz.sHtML

[R30] 函数返回状态码
来源：http://www.blog.sjlbkw.cn/Article/details/grykemptc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/goucrpxce.sHtML

[R31] 局部变量
来源：http://mobile.yfazqb.com/Article/details/ghgozthnd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/gfnzsmdux.sHtML

[R32] 参数个数校验
来源：http://blog.epnwcf.com/Article/details/gfcacxjfk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/gngxogqfu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.vehdjk.com/Article/details/gpqlrxfjz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.yfazqb.com/Article/details/gtmkwqikb.sHtML

[R34] 退出时清理
来源：http://baike.yfazqb.com/Article/details/gjierryyb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/ggkrdvzcc.sHtML

[R35] 后台执行并等待
来源：http://read.share.tarul.cn/Article/details/graazmxvl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.bbcook.cn/Article/details/gylivaxgk.sHtML

[R36] 并发执行多个任务
来源：http://m.share.vehdjk.com/Article/details/gcmvwwewl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.vehdjk.com/Article/details/glpegnein.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.yfazqb.com/Article/details/gpdmkhiwl.sHtML

files=$(ls -1)
来源：http://wap.epnwcf.com/Article/details/gifcfenoo.sHtML

[R38] 管道串联
来源：http://read.share.tarul.cn/Article/details/gnaopoukk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.vehdjk.com/Article/details/gubmbllfb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/gjiwzorea.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/gokhodtkw.sHtML

[R40] 追加写日志
来源：http://www.m.share.bbcook.cn/Article/details/gjzcoseag.sHtML

echo "log" >> out.log
来源：http://3g.fktsv.cn/Article/details/ggkfvyqrx.sHtML

[R41] 丢弃输出
来源：http://www.share.yfazqb.com/Article/details/gnudoyhcm.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.tarul.cn/Article/details/ggdpnjpzr.sHtML

[R42] 输入重定向
来源：http://mobile.bbcook.cn/Article/details/gehslojjl.sHtML

wc -l < a.txt
来源：http://wap.bbcook.cn/Article/details/gepsdqzjp.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fktsv.cn/Article/details/gxwttyxth.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/gitkfantn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fktsv.cn/Article/details/gvzuwjxgd.sHtML

find . -mtime -7 -type f
来源：http://wap.fktsv.cn/Article/details/gavqzyvkh.sHtML

[R45] 批量删除
来源：http://blog.yfazqb.com/Article/details/gmhrbylmg.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.tarul.cn/Article/details/ghwpnejal.sHtML

[R46] 递归替换文件内容
来源：http://read.share.epnwcf.com/Article/details/grhiixpql.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.epnwcf.com/Article/details/gimfhlpqg.sHtML

[R47] sed 单行替换
来源：http://baike.vehdjk.com/Article/details/gnxvbkorq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.tarul.cn/Article/details/gshhaducu.sHtML

[R48] awk 取指定列
来源：http://read.share.epnwcf.com/Article/details/givxjejik.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fktsv.cn/Article/details/gvioutopx.sHtML

[R49] awk 带条件
来源：http://mobile.epnwcf.com/Article/details/gxonezeck.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.tarul.cn/Article/details/goqebgwzf.sHtML

[R50] awk 求和
来源：http://m.share.fktsv.cn/Article/details/gsalwryoz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gplpifkyj.sHtML

[R51] 排序去重取前几
来源：http://blog.epnwcf.com/Article/details/gdnqdexhh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.yfazqb.com/Article/details/gnjorpjow.sHtML

[R52] 统计行数
来源：http://mobile.sjlbkw.cn/Article/details/geykynegz.sHtML

wc -l a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gaidqrsjn.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.vehdjk.com/Article/details/gflcdvngy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.vehdjk.com/Article/details/gifnmynql.sHtML

[R54] 比较两个文件
来源：http://www.blog.bbcook.cn/Article/details/giljktiei.sHtML

diff a.txt b.txt
来源：http://baike.sjlbkw.cn/Article/details/gfezzwibz.sHtML

[R55] 压缩与解压
来源：http://www.m.share.bbcook.cn/Article/details/gsthyzvnz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fktsv.cn/Article/details/gvlddekgt.sHtML

[R56] 远程拷贝
来源：http://www.m.share.vehdjk.com/Article/details/glcpixjem.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gsamcktba.sHtML

[R57] 远程执行命令
来源：http://mobile.bbcook.cn/Article/details/gnwoffyzy.sHtML

ssh user@host 'uptime'
来源：http://baike.fktsv.cn/Article/details/gkntazgjc.sHtML

[R58] 下载文件
来源：http://blog.vehdjk.com/Article/details/ghvprryjs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.sjlbkw.cn/Article/details/gauhdtluj.sHtML

[R59] 发 POST JSON
来源：http://wap.tarul.cn/Article/details/gwphxnqcz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.yfazqb.com/Article/details/gfqpgvfke.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/ghwsbgehl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.sjlbkw.cn/Article/details/ggbucaexy.sHtML

[R61] 磁盘占用
来源：http://baike.vehdjk.com/Article/details/gjzqilxdu.sHtML

df -h;  du -sh *
来源：http://read.share.tarul.cn/Article/details/gamqlxnba.sHtML

[R62] 找最占空间的文件
来源：http://mobile.sjlbkw.cn/Article/details/gerikucks.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.tarul.cn/Article/details/gueaxjgfy.sHtML

[R63] 内存与进程
来源：http://mobile.yfazqb.com/Article/details/gkyuyuhzh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.yfazqb.com/Article/details/gcmemmfvf.sHtML

[R64] 结束进程
来源：http://www.share.vehdjk.com/Article/details/gsznnkwfd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fktsv.cn/Article/details/grejkozkc.sHtML

[R65] 查看端口占用
来源：http://www.blog.bbcook.cn/Article/details/grjhwcgjg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.tarul.cn/Article/details/ggkvpwzto.sHtML

[R66] 定时任务
来源：http://mobile.vehdjk.com/Article/details/gfyuyooqa.sHtML

crontab -e;  crontab -l
来源：http://3g.bbcook.cn/Article/details/gdjhhozlt.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fktsv.cn/Article/details/gzoruvghx.sHtML

openssl rand -hex 16
来源：http://wap.sjlbkw.cn/Article/details/gkjisejvi.sHtML

[R68] 计算文件校验值
来源：http://blog.epnwcf.com/Article/details/gpckyossv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.epnwcf.com/Article/details/geywmjoqb.sHtML

[R69] 生成随机密码
来源：http://mobile.tarul.cn/Article/details/ghmoylswu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.vehdjk.com/Article/details/ggmckpkgi.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/gcepmpqti.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.epnwcf.com/Article/details/gryripbob.sHtML

[R71] 日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/guaoquwgp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.yfazqb.com/Article/details/gnooorzlz.sHtML

[R72] 等待端口就绪
来源：http://3g.sjlbkw.cn/Article/details/gtoyodzrw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gvxuawulb.sHtML

[R73] 分割大日志
来源：http://blog.vehdjk.com/Article/details/gbklwddxq.sHtML

split -l 1000 big.log part_
来源：http://www.blog.vehdjk.com/Article/details/gobjgeiot.sHtML

[R74] 批量重命名
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpofhuwp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.epnwcf.com/Article/details/ghkpkovrm.sHtML

[R75] 导出环境变量
来源：http://baike.tarul.cn/Article/details/gusstulkv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.bbcook.cn/Article/details/gaqzyxfuj.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/gjrtepkkf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gfixfmdsx.sHtML

[R77] 读取用户输入
来源：http://read.share.yfazqb.com/Article/details/gtmzjepjg.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/goxcjpxgx.sHtML

[R78] 交互式菜单
来源：http://mobile.epnwcf.com/Article/details/gnmuroegb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/gsijwdesm.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gbjanvfdf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.sjlbkw.cn/Article/details/gjwwhddwf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.yfazqb.com/Article/details/giwrtvoyx.sHtML

time ./run.sh
来源：http://mobile.epnwcf.com/Article/details/gjdanuwsh.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzyybfqgy.sHtML

S. C / C++ 专题
来源：http://www.blog.fktsv.cn/Article/details/gtuixchxx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtbgjputg.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gbwwdqier.sHtML

#include <stdio.h>
来源：http://mobile.bbcook.cn/Article/details/gtgoigvhy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.yfazqb.com/Article/details/glxyxtsxi.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.bbcook.cn/Article/details/gaumnsjlz.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/gtibetfon.sHtML

[S03] C：读入整数
来源：http://www.share.vehdjk.com/Article/details/gqhbanjjb.sHtML

int x; scanf("%d", &x);
来源：http://wap.epnwcf.com/Article/details/gohrnzavw.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/gqkvcesmw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.vehdjk.com/Article/details/gdhvxhwch.sHtML

[S05] C：字符串长度
来源：http://baike.epnwcf.com/Article/details/gerbrezih.sHtML

strlen(s)
来源：http://wap.sjlbkw.cn/Article/details/gehqucbnr.sHtML

[S06] C：字符串比较
来源：http://www.share.tarul.cn/Article/details/gnirpdhlg.sHtML

strcmp(a, b) == 0
来源：http://www.share.sjlbkw.cn/Article/details/gmekutodv.sHtML

[S07] C：数组遍历求和
来源：http://3g.bbcook.cn/Article/details/gyvapkpgu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.yfazqb.com/Article/details/gxeonydkz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.epnwcf.com/Article/details/gnlomytey.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.bbcook.cn/Article/details/ghldugdow.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.yfazqb.com/Article/details/ghzwzllyr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/gpvyrjqpn.sHtML

[S10] C：指针与解引用
来源：http://mobile.fktsv.cn/Article/details/gououuojc.sHtML

int *p = &a;  *p = 5;
来源：http://baike.yfazqb.com/Article/details/gqyjdlqvd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gdopoyfil.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.epnwcf.com/Article/details/gyvhydirq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.yfazqb.com/Article/details/ghctrnvfl.sHtML

fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gdiipdksk.sHtML

[S12] C：写文件
来源：http://wap.tarul.cn/Article/details/gqwbvawew.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.epnwcf.com/Article/details/goostngun.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gcgtoafks.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.yfazqb.com/Article/details/gnfowhlwa.sHtML

[S14] C：枚举
来源：http://wap.vehdjk.com/Article/details/gyeulrnig.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.epnwcf.com/Article/details/gzqtyparl.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/gfmzemzcr.sHtML

(double) a / b
来源：http://3g.tarul.cn/Article/details/gmxgjnqlx.sHtML

[S16] C：位操作置位
来源：http://www.m.share.bbcook.cn/Article/details/gjzeltrrv.sHtML

x |= (1 << 3);
来源：http://blog.vehdjk.com/Article/details/gajyvkbxw.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gnhhiufxi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/guhlakost.sHtML

[S18] C：命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gnirdyqhm.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.bbcook.cn/Article/details/gldnrpnmh.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/gzltqdhcf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/glhzbbwdf.sHtML

[S20] C：二分查找
来源：http://m.share.vehdjk.com/Article/details/gyjuicoig.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gdqtmpbcf.sHtML

[S21] C：字符类别判断
来源：http://3g.bbcook.cn/Article/details/gyqltltxp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fktsv.cn/Article/details/gdxqrixox.sHtML

[S22] C：字符串转数字
来源：http://blog.bbcook.cn/Article/details/gslnltmie.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/gsxrhygbe.sHtML

[S23] C：随机数
来源：http://3g.epnwcf.com/Article/details/gmkxwawpp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.vehdjk.com/Article/details/gtssezihn.sHtML

[S24] C：获取本地时间
来源：http://www.share.vehdjk.com/Article/details/gjaucijnx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fktsv.cn/Article/details/gmuiuyumc.sHtML

[S25] C：内存拷贝
来源：http://m.share.vehdjk.com/Article/details/gyeztqrgy.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fktsv.cn/Article/details/gneawmkhf.sHtML

[S26] C：内存清零
来源：http://m.share.yfazqb.com/Article/details/gpqzwurof.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.bbcook.cn/Article/details/gnplmkxih.sHtML

[S27] C：定义常量
来源：http://www.m.share.yfazqb.com/Article/details/gepdluolw.sHtML

const double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gfdganllo.sHtML

[S28] C：静态变量
来源：http://m.share.fktsv.cn/Article/details/gzqcegrei.sHtML

static int counter = 0;
来源：http://mobile.yfazqb.com/Article/details/gvnpvdrxk.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/grfwtyugl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/gzqpzxavg.sHtML

[S30] C：头文件保护
来源：http://blog.fktsv.cn/Article/details/ghxszmcqp.sHtML

#ifndef X_H
来源：http://baike.epnwcf.com/Article/details/grfvizwwt.sHtML

#define X_H
来源：http://www.blog.epnwcf.com/Article/details/gpuiommhf.sHtML

#endif
来源：http://3g.bbcook.cn/Article/details/gbzimhqyd.sHtML

[S31] C++：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gympehxyh.sHtML

#include <iostream>
来源：http://mobile.vehdjk.com/Article/details/gmlgmdypy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/gckoryrcn.sHtML

[S32] C++：字符串
来源：http://3g.fktsv.cn/Article/details/guvtnyytw.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/gjyvjrgxi.sHtML

[S33] C++：vector 增删
来源：http://wap.sjlbkw.cn/Article/details/gjivwfxyv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.vehdjk.com/Article/details/gpmhvwdlw.sHtML

[S34] C++：遍历 vector
来源：http://blog.fktsv.cn/Article/details/gcmdzgmqi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.bbcook.cn/Article/details/gxssxqzcq.sHtML

[S35] C++：map
来源：http://www.share.tarul.cn/Article/details/gpegqgxro.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gjdlmdbhk.sHtML

[S36] C++：unordered_map
来源：http://mobile.sjlbkw.cn/Article/details/gqpcpqvtu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/gznwiawjm.sHtML

[S37] C++：set
来源：http://www.share.epnwcf.com/Article/details/giiwozssp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fktsv.cn/Article/details/gtjbotcdq.sHtML

[S38] C++：排序
来源：http://mobile.bbcook.cn/Article/details/gddxqxgnk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.bbcook.cn/Article/details/gpzhqipqd.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/gvzzjmogk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.sjlbkw.cn/Article/details/gfpjlyobp.sHtML

[S40] C++：查找元素
来源：http://baike.fktsv.cn/Article/details/gmlmfijzf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.tarul.cn/Article/details/gzcfourcg.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.yfazqb.com/Article/details/gqrvyzjzv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.sjlbkw.cn/Article/details/gcoddhjuk.sHtML

[S42] C++：继承与虚函数
来源：http://3g.vehdjk.com/Article/details/gqztilsrg.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.yfazqb.com/Article/details/gdfbzitfy.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/ggnwchexk.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.epnwcf.com/Article/details/gewohtpbv.sHtML

[S44] C++：引用传参
来源：http://www.m.share.epnwcf.com/Article/details/gtojqmvmm.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.yfazqb.com/Article/details/gqizujynv.sHtML

[S45] C++：lambda
来源：http://wap.fktsv.cn/Article/details/gfongppfz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gfekepygn.sHtML

[S46] C++：函数模板
来源：http://blog.epnwcf.com/Article/details/gzltktpxv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.sjlbkw.cn/Article/details/guqosacyb.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.sjlbkw.cn/Article/details/gfbgbjxzx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.bbcook.cn/Article/details/glzibbvub.sHtML

[S48] C++：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/grlfllvhq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.epnwcf.com/Article/details/gdytjdhmg.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/gichbnlho.sHtML

[S49] C++：写文件
来源：http://blog.epnwcf.com/Article/details/gytghdsfn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.sjlbkw.cn/Article/details/ghwgtuwtk.sHtML

[S50] C++：格式化数字
来源：http://mobile.fktsv.cn/Article/details/gfuacylmm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.tarul.cn/Article/details/givecrkmn.sHtML

[S51] C++：显式类型转换
来源：http://wap.vehdjk.com/Article/details/gbvdnxrkb.sHtML

static_cast<double>(a) / b
来源：http://3g.fktsv.cn/Article/details/gmlwkapaz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.sjlbkw.cn/Article/details/gbqiiazsv.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fktsv.cn/Article/details/gahordend.sHtML

[S53] C++：移动语义
来源：http://mobile.yfazqb.com/Article/details/ggsxekfwu.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.sjlbkw.cn/Article/details/gcfozieli.sHtML

[S54] C++：异常处理
来源：http://read.share.fktsv.cn/Article/details/gzigmwyvt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.vehdjk.com/Article/details/gcwvewgvu.sHtML

[S55] C++：结构化绑定
来源：http://www.share.epnwcf.com/Article/details/geuimvpyg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gfdztjgux.sHtML

[S56] C++：optional
来源：http://www.share.sjlbkw.cn/Article/details/gkqofaqqc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.vehdjk.com/Article/details/gqwxvcdqz.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fktsv.cn/Article/details/gfmzhsdyd.sHtML

constexpr int N = 10;
来源：http://read.share.vehdjk.com/Article/details/gxkviyfhs.sHtML

[S58] C++：命名空间
来源：http://www.m.share.epnwcf.com/Article/details/gfjbqnvts.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.vehdjk.com/Article/details/ghfedbzfu.sHtML

[S59] C++：静态断言
来源：http://blog.fktsv.cn/Article/details/gwlfmftdl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/gfyrnfpnn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.tarul.cn/Article/details/gfprsenag.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.tarul.cn/Article/details/goypybtqx.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gvvwqklkv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gwxzcnelt.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gnzlbywas.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fktsv.cn/Article/details/gxzfvtjnb.sHtML

println("Hello")
来源：http://wap.tarul.cn/Article/details/gqnmpvxlk.sHtML

[T02] Kotlin：变量
来源：http://wap.sjlbkw.cn/Article/details/gqqrdxknk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.vehdjk.com/Article/details/gclemqwvn.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/gmamvktro.sHtML

"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/gqfzztcuy.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gplpxrqdl.sHtML

val n: String? = null;  n?.length
来源：http://www.share.bbcook.cn/Article/details/gkftetykq.sHtML


<!-- 参考信息 -->