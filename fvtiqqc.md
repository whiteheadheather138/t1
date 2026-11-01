代发 wailian999

set -euo pipefail
来源：http://wap.tarul.cn/Article/details/gmhpozphe.sHtML

[R02] 变量赋值与使用
来源：http://read.share.sjlbkw.cn/Article/details/gourkfxri.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fktsv.cn/Article/details/gzgbeabxs.sHtML

[R03] 只读变量
来源：http://blog.epnwcf.com/Article/details/gvksqvcin.sHtML

readonly PI=3.14
来源：http://3g.epnwcf.com/Article/details/gyemqmohb.sHtML

[R04] 位置参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gcheaiblr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.yfazqb.com/Article/details/gfvloptmw.sHtML

[R05] 参数默认值
来源：http://blog.sjlbkw.cn/Article/details/gnczanaqs.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/gclbqxxed.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.yfazqb.com/Article/details/gokrkfqxz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/gbivngbza.sHtML

[R07] if 判断文件
来源：http://3g.epnwcf.com/Article/details/gnqlqrkdx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fktsv.cn/Article/details/gsakcvyqa.sHtML

[R08] 数值比较
来源：http://wap.tarul.cn/Article/details/gvgkhateq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.tarul.cn/Article/details/ggihidoxn.sHtML

[R09] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/grlnfshwl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fktsv.cn/Article/details/gyfmxpdxt.sHtML

[R10] 正则匹配
来源：http://mobile.sjlbkw.cn/Article/details/gjahvklgr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.bbcook.cn/Article/details/geuypmnmx.sHtML

[R11] case 多分支
来源：http://www.m.share.tarul.cn/Article/details/gjvvpuuve.sHtML

case "$1" in
来源：http://3g.vehdjk.com/Article/details/gufidyyid.sHtML

start) echo "启动" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gybijpibo.sHtML

stop)  echo "停止" ;;
来源：http://wap.vehdjk.com/Article/details/gocahcucs.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gpoqslgzz.sHtML

esac
来源：http://www.m.share.tarul.cn/Article/details/gqhigqbjr.sHtML

[R12] for 遍历文件
来源：http://mobile.yfazqb.com/Article/details/gqkcaihhp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.epnwcf.com/Article/details/gbhgjfhqm.sHtML

[R13] for 计数循环
来源：http://3g.sjlbkw.cn/Article/details/gfsfcodxo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gjfveqcqe.sHtML

[R14] C 风格 for
来源：http://read.share.vehdjk.com/Article/details/glhzewoux.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gvflgzfbq.sHtML

[R15] while 逐行读文件
来源：http://read.share.tarul.cn/Article/details/gkxkmlnps.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.bbcook.cn/Article/details/gopzysvug.sHtML

[R16] until 等待条件
来源：http://read.share.sjlbkw.cn/Article/details/guzbsvijq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/gqjjwpucx.sHtML

[R17] 数组定义与取值
来源：http://m.share.yfazqb.com/Article/details/gmyfgyanu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.vehdjk.com/Article/details/gkjcsehmf.sHtML

[R18] 遍历数组
来源：http://3g.yfazqb.com/Article/details/gwujeavyx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.bbcook.cn/Article/details/gsczheoiy.sHtML

[R19] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gktaubsqa.sHtML

echo "${#arr[@]}"
来源：http://m.share.sjlbkw.cn/Article/details/gzoegitnd.sHtML

[R20] 关联数组（字典）
来源：http://blog.bbcook.cn/Article/details/gcwzbnayp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.sjlbkw.cn/Article/details/gkkjhrrlq.sHtML

[R21] 字符串长度
来源：http://3g.bbcook.cn/Article/details/gfnhvnunx.sHtML

echo "${#s}"
来源：http://www.share.tarul.cn/Article/details/gusldtrrd.sHtML

[R22] 截取子串
来源：http://3g.yfazqb.com/Article/details/gcopuljta.sHtML

echo "${s:0:5}"
来源：http://blog.fktsv.cn/Article/details/gvggjwljy.sHtML

[R23] 字符串替换
来源：http://blog.vehdjk.com/Article/details/ghurheovp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fktsv.cn/Article/details/gutukvpqc.sHtML

[R24] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gyqadavmr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.tarul.cn/Article/details/glzkgizec.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.yfazqb.com/Article/details/gftlijwyd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.tarul.cn/Article/details/gjnsohcih.sHtML

[R26] 命令替换
来源：http://www.share.tarul.cn/Article/details/gcsjjuizp.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.bbcook.cn/Article/details/glqxmlxja.sHtML

[R27] 算术展开
来源：http://www.m.share.sjlbkw.cn/Article/details/gdafpiqap.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fktsv.cn/Article/details/girvnlbyp.sHtML

[R28] 浮点运算
来源：http://3g.sjlbkw.cn/Article/details/gfmyxhwvo.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.bbcook.cn/Article/details/gyxzoztps.sHtML

[R29] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtamioox.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.bbcook.cn/Article/details/glazmezay.sHtML

[R30] 函数返回状态码
来源：http://www.share.tarul.cn/Article/details/gvtjjjewe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.vehdjk.com/Article/details/gbfvegetq.sHtML

[R31] 局部变量
来源：http://3g.bbcook.cn/Article/details/ghvkusprn.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.bbcook.cn/Article/details/gcozvowam.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/ggwxeeztd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/gohwfgngj.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.epnwcf.com/Article/details/gwexszvjy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.vehdjk.com/Article/details/gakkwstgc.sHtML

[R34] 退出时清理
来源：http://m.share.sjlbkw.cn/Article/details/gkrybiadx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.vehdjk.com/Article/details/ghlmoxuig.sHtML

[R35] 后台执行并等待
来源：http://read.share.fktsv.cn/Article/details/gfcycbhyc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.bbcook.cn/Article/details/glfokowfw.sHtML

[R36] 并发执行多个任务
来源：http://blog.epnwcf.com/Article/details/gjlgfpmxv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.sjlbkw.cn/Article/details/gbyfrtyih.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/grnyoftrx.sHtML

files=$(ls -1)
来源：http://www.blog.bbcook.cn/Article/details/gofqoomti.sHtML

[R38] 管道串联
来源：http://www.share.vehdjk.com/Article/details/gkveoqnzh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.epnwcf.com/Article/details/gicetsfgd.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.epnwcf.com/Article/details/gzehnvede.sHtML

cmd > out.log 2>&1
来源：http://read.share.epnwcf.com/Article/details/gkqnmjdts.sHtML

[R40] 追加写日志
来源：http://blog.sjlbkw.cn/Article/details/gplugdsnw.sHtML

echo "log" >> out.log
来源：http://read.share.yfazqb.com/Article/details/gnkokbqsd.sHtML

[R41] 丢弃输出
来源：http://3g.epnwcf.com/Article/details/grbjnrnvk.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fktsv.cn/Article/details/gtbovqbgf.sHtML

[R42] 输入重定向
来源：http://read.share.bbcook.cn/Article/details/girkpmvcr.sHtML

wc -l < a.txt
来源：http://www.share.bbcook.cn/Article/details/gbsfllrbg.sHtML

[R43] 按名字查找文件
来源：http://read.share.sjlbkw.cn/Article/details/gqjintvqe.sHtML

find . -name "*.log" -type f
来源：http://3g.tarul.cn/Article/details/glkzugwjr.sHtML

[R44] 按修改时间查找
来源：http://baike.yfazqb.com/Article/details/grmweqkan.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/glcefvenf.sHtML

[R45] 批量删除
来源：http://www.blog.vehdjk.com/Article/details/gudomeqyz.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.yfazqb.com/Article/details/gzqqfqsqv.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/gnuejbuxz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.epnwcf.com/Article/details/gwxvayhrs.sHtML

[R47] sed 单行替换
来源：http://3g.epnwcf.com/Article/details/gmqkwbknp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.epnwcf.com/Article/details/gcglctauc.sHtML

[R48] awk 取指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gyluvoknx.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.epnwcf.com/Article/details/ghcjtyrjs.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/grevrlqmg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.sjlbkw.cn/Article/details/grqxdqidx.sHtML

[R50] awk 求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnwfeqnb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fktsv.cn/Article/details/giujnhqkj.sHtML

[R51] 排序去重取前几
来源：http://3g.epnwcf.com/Article/details/gvogbkgtu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.yfazqb.com/Article/details/glewfxtmy.sHtML

[R52] 统计行数
来源：http://www.blog.fktsv.cn/Article/details/glbuhgqej.sHtML

wc -l a.txt
来源：http://mobile.tarul.cn/Article/details/gwmafbxjz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/grhtvjcoi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.sjlbkw.cn/Article/details/glnjqqclb.sHtML

[R54] 比较两个文件
来源：http://3g.tarul.cn/Article/details/gxpxomrel.sHtML

diff a.txt b.txt
来源：http://blog.bbcook.cn/Article/details/gkvclfasu.sHtML

[R55] 压缩与解压
来源：http://www.share.tarul.cn/Article/details/gjdyytjje.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.sjlbkw.cn/Article/details/goefqiotc.sHtML

[R56] 远程拷贝
来源：http://baike.sjlbkw.cn/Article/details/gbxyswfnl.sHtML

scp file user@host:/path/
来源：http://mobile.fktsv.cn/Article/details/ghvmvnwuu.sHtML

[R57] 远程执行命令
来源：http://blog.vehdjk.com/Article/details/gbrdclnlz.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/gsgunijvz.sHtML

[R58] 下载文件
来源：http://mobile.fktsv.cn/Article/details/ghomezffc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.epnwcf.com/Article/details/ggegmmgnx.sHtML

[R59] 发 POST JSON
来源：http://blog.vehdjk.com/Article/details/gxrifpfoo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.tarul.cn/Article/details/ggahmwpke.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/geilucuxi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.tarul.cn/Article/details/gxhdvjodh.sHtML

[R61] 磁盘占用
来源：http://3g.epnwcf.com/Article/details/gqjdahrsc.sHtML

df -h;  du -sh *
来源：http://blog.yfazqb.com/Article/details/grerqajrt.sHtML

[R62] 找最占空间的文件
来源：http://read.share.vehdjk.com/Article/details/guchlfvyz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/gcmnbwuck.sHtML

[R63] 内存与进程
来源：http://www.blog.tarul.cn/Article/details/gmnnbygwf.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.vehdjk.com/Article/details/gbvzjqozc.sHtML

[R64] 结束进程
来源：http://blog.bbcook.cn/Article/details/gwkxlkvnt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.tarul.cn/Article/details/giddnlmhl.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/gavlhqfjk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.vehdjk.com/Article/details/gpuviovwl.sHtML

[R66] 定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gedffbjcs.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/gpuebpsuj.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.tarul.cn/Article/details/gksynppvu.sHtML

openssl rand -hex 16
来源：http://wap.sjlbkw.cn/Article/details/gaaxjnkbu.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/gtljfpttz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.yfazqb.com/Article/details/genvzeuob.sHtML

[R69] 生成随机密码
来源：http://mobile.bbcook.cn/Article/details/gubgpyqif.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fktsv.cn/Article/details/gtzzkiskc.sHtML

[R70] 时间戳与互转
来源：http://baike.bbcook.cn/Article/details/glamsiopl.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/gajyintdo.sHtML

[R71] 日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/grsznugbv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.sjlbkw.cn/Article/details/ghzfrngcy.sHtML

[R72] 等待端口就绪
来源：http://m.share.vehdjk.com/Article/details/gxogwuuez.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/gzgduaran.sHtML

[R73] 分割大日志
来源：http://baike.vehdjk.com/Article/details/goxhxybrs.sHtML

split -l 1000 big.log part_
来源：http://www.blog.vehdjk.com/Article/details/gllwkfdkt.sHtML

[R74] 批量重命名
来源：http://wap.fktsv.cn/Article/details/gocnajkpb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.bbcook.cn/Article/details/gxlnsyjpf.sHtML

[R75] 导出环境变量
来源：http://mobile.tarul.cn/Article/details/gifyxvvph.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.vehdjk.com/Article/details/gzsptnyev.sHtML

[R76] 使用临时文件
来源：http://wap.vehdjk.com/Article/details/gsfrmwvpn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/gvgwrtzci.sHtML

[R77] 读取用户输入
来源：http://mobile.tarul.cn/Article/details/gbzeemxzq.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fktsv.cn/Article/details/gskandawy.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/gyumjpttp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.bbcook.cn/Article/details/gebphwypv.sHtML

[R79] 解析命令行选项
来源：http://read.share.bbcook.cn/Article/details/gmmszrtuu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.tarul.cn/Article/details/gkjflaxoq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.vehdjk.com/Article/details/gawtgicyv.sHtML

time ./run.sh
来源：http://m.share.sjlbkw.cn/Article/details/glgadjctg.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/goeoscuzu.sHtML

S. C / C++ 专题
来源：http://www.m.share.yfazqb.com/Article/details/ggqseqbpl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grjcsgkqh.sHtML

[S01] C：Hello World
来源：http://wap.vehdjk.com/Article/details/gbbcdoegm.sHtML

#include <stdio.h>
来源：http://wap.vehdjk.com/Article/details/gvfwqrata.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.tarul.cn/Article/details/gqgrtrodn.sHtML

[S02] C：变量与格式化输出
来源：http://3g.tarul.cn/Article/details/gfjrbidso.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.yfazqb.com/Article/details/gzedzounf.sHtML

[S03] C：读入整数
来源：http://3g.tarul.cn/Article/details/ggzjomqlu.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fktsv.cn/Article/details/gmnztmjeq.sHtML

[S04] C：字符串复制
来源：http://www.share.bbcook.cn/Article/details/gcoudbqhc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fktsv.cn/Article/details/gzjqbftpn.sHtML

[S05] C：字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gxhwfqkup.sHtML

strlen(s)
来源：http://m.share.sjlbkw.cn/Article/details/gdydsboeb.sHtML

[S06] C：字符串比较
来源：http://m.share.yfazqb.com/Article/details/ggnyjxbjm.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/gvfbidfqq.sHtML

[S07] C：数组遍历求和
来源：http://blog.yfazqb.com/Article/details/gztvhuuyz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.yfazqb.com/Article/details/gwyfwjapt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fktsv.cn/Article/details/gqbcueuqh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.sjlbkw.cn/Article/details/gynkfeush.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.sjlbkw.cn/Article/details/ghuaeudws.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.tarul.cn/Article/details/gooexdzso.sHtML

[S10] C：指针与解引用
来源：http://read.share.fktsv.cn/Article/details/gpchdpjce.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.sjlbkw.cn/Article/details/gnxkmgtxz.sHtML

[S11] C：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gihlphtjt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fktsv.cn/Article/details/gziouxsno.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.yfazqb.com/Article/details/gfzljoitv.sHtML

fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gfaasggux.sHtML

[S12] C：写文件
来源：http://m.share.tarul.cn/Article/details/gxptjnfas.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gudhibumi.sHtML

[S13] C：宏定义
来源：http://baike.bbcook.cn/Article/details/gjhmcnlaa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.yfazqb.com/Article/details/gwukiytbn.sHtML

[S14] C：枚举
来源：http://www.share.tarul.cn/Article/details/gxbemparn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.epnwcf.com/Article/details/goimozccv.sHtML

[S15] C：类型转换
来源：http://www.m.share.tarul.cn/Article/details/gbujetgrg.sHtML

(double) a / b
来源：http://3g.epnwcf.com/Article/details/gbcwgodyp.sHtML

[S16] C：位操作置位
来源：http://read.share.bbcook.cn/Article/details/gomtwldal.sHtML

x |= (1 << 3);
来源：http://blog.vehdjk.com/Article/details/gstywizrk.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gbyrjlrqz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.bbcook.cn/Article/details/ggtzvxoxz.sHtML

[S18] C：命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gbxkgjpaa.sHtML

int main(int argc, char **argv)
来源：http://baike.bbcook.cn/Article/details/ggtozuxnq.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/gavgzbkas.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gbpsqcaci.sHtML

[S20] C：二分查找
来源：http://3g.epnwcf.com/Article/details/gvugfdgzk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gafxvcquh.sHtML

[S21] C：字符类别判断
来源：http://baike.bbcook.cn/Article/details/gxdqxzwji.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fktsv.cn/Article/details/glqxnqyyd.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.sjlbkw.cn/Article/details/grbyxwpen.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/gudogpjwo.sHtML

[S23] C：随机数
来源：http://www.share.epnwcf.com/Article/details/gaiuvifuy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fktsv.cn/Article/details/ghkvymdxw.sHtML

[S24] C：获取本地时间
来源：http://read.share.sjlbkw.cn/Article/details/gjecjkrom.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.bbcook.cn/Article/details/gebtxzncd.sHtML

[S25] C：内存拷贝
来源：http://www.blog.yfazqb.com/Article/details/gjefsxmuy.sHtML

memcpy(dst, src, n);
来源：http://www.share.vehdjk.com/Article/details/goqyfcuaz.sHtML

[S26] C：内存清零
来源：http://wap.bbcook.cn/Article/details/gavyullsw.sHtML

memset(a, 0, sizeof a);
来源：http://blog.yfazqb.com/Article/details/gggucuuue.sHtML

[S27] C：定义常量
来源：http://baike.epnwcf.com/Article/details/gcfjpnumn.sHtML

const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gziamujwe.sHtML

[S28] C：静态变量
来源：http://mobile.fktsv.cn/Article/details/ghbqeuqeh.sHtML

static int counter = 0;
来源：http://www.m.share.fktsv.cn/Article/details/gsiruxpoc.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/gtlrxffss.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.sjlbkw.cn/Article/details/gbuezztjg.sHtML

[S30] C：头文件保护
来源：http://mobile.tarul.cn/Article/details/gdkyfrykw.sHtML

#ifndef X_H
来源：http://www.blog.fktsv.cn/Article/details/gjibmcpmv.sHtML

#define X_H
来源：http://3g.bbcook.cn/Article/details/gpbeqvpec.sHtML

#endif
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgrcejuk.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/gwalvlcjq.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gzxeahgwa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.bbcook.cn/Article/details/gzpqgqyex.sHtML

[S32] C++：字符串
来源：http://blog.yfazqb.com/Article/details/gcvqrgneg.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fktsv.cn/Article/details/gobyryczk.sHtML

[S33] C++：vector 增删
来源：http://wap.yfazqb.com/Article/details/gbwrzhcni.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.bbcook.cn/Article/details/guadsrtlw.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/gxbjqkbie.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.bbcook.cn/Article/details/gwcjqrgtn.sHtML

[S35] C++：map
来源：http://read.share.bbcook.cn/Article/details/gcaoksghx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/ghhsafosk.sHtML

[S36] C++：unordered_map
来源：http://www.blog.epnwcf.com/Article/details/giifegyge.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gojgtgjjy.sHtML

[S37] C++：set
来源：http://www.share.epnwcf.com/Article/details/gjrfbssam.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.epnwcf.com/Article/details/gzfehezij.sHtML

[S38] C++：排序
来源：http://blog.epnwcf.com/Article/details/gtscejbmk.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.tarul.cn/Article/details/gsmygdgfw.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fktsv.cn/Article/details/gaknmykkg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.tarul.cn/Article/details/gruehsgzm.sHtML

[S40] C++：查找元素
来源：http://www.m.share.epnwcf.com/Article/details/ggxxkciqv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.vehdjk.com/Article/details/gyrikkvkd.sHtML

[S41] C++：类与构造函数
来源：http://blog.sjlbkw.cn/Article/details/gdjsiuoqt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fktsv.cn/Article/details/gbphuuuht.sHtML

[S42] C++：继承与虚函数
来源：http://3g.epnwcf.com/Article/details/gjgetqfzj.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/greqohjvn.sHtML

[S43] C++：智能指针
来源：http://mobile.bbcook.cn/Article/details/gfbytvvsc.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.vehdjk.com/Article/details/guhacngtn.sHtML

[S44] C++：引用传参
来源：http://3g.bbcook.cn/Article/details/gvbhywzty.sHtML

void inc(int &x) { ++x; }
来源：http://blog.vehdjk.com/Article/details/gtlcqxoql.sHtML

[S45] C++：lambda
来源：http://read.share.tarul.cn/Article/details/gbayzlkzl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.epnwcf.com/Article/details/gngxdccrk.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gghjjdzdx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.epnwcf.com/Article/details/gkvkbtbhd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.yfazqb.com/Article/details/gkjnmjyrl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.yfazqb.com/Article/details/gtbtkqeuu.sHtML

[S48] C++：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gvtfbkqxe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.sjlbkw.cn/Article/details/gkdovrcnw.sHtML

while (std::getline(in, line)) { }
来源：http://3g.tarul.cn/Article/details/genfxtmzj.sHtML

[S49] C++：写文件
来源：http://3g.epnwcf.com/Article/details/gstfqvreh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.tarul.cn/Article/details/gqabttbfw.sHtML

[S50] C++：格式化数字
来源：http://wap.epnwcf.com/Article/details/gwqhrgqdh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gjkuqnfhx.sHtML

[S51] C++：显式类型转换
来源：http://baike.tarul.cn/Article/details/gqqbbimbu.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.tarul.cn/Article/details/gqbmzqczt.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gdwrokkxt.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.epnwcf.com/Article/details/gzhcmlnrw.sHtML

[S53] C++：移动语义
来源：http://www.share.epnwcf.com/Article/details/gmafzngbs.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.vehdjk.com/Article/details/gtfxmhwms.sHtML

[S54] C++：异常处理
来源：http://blog.fktsv.cn/Article/details/gtojkcqrt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/gsdrglqka.sHtML

[S55] C++：结构化绑定
来源：http://blog.yfazqb.com/Article/details/gzxnxupzg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.yfazqb.com/Article/details/gerjlovrk.sHtML

[S56] C++：optional
来源：http://read.share.fktsv.cn/Article/details/garsjkzdb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.epnwcf.com/Article/details/gldnenxkj.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.epnwcf.com/Article/details/gnaahisrl.sHtML

constexpr int N = 10;
来源：http://3g.sjlbkw.cn/Article/details/gcobalvzf.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gcptjhhfq.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.bbcook.cn/Article/details/gfsjqddko.sHtML

[S59] C++：静态断言
来源：http://www.m.share.vehdjk.com/Article/details/glqgpyvtb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.vehdjk.com/Article/details/ggfjqmfvl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/gqendlzrx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fktsv.cn/Article/details/gfgvxqirg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grirvvfqz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fktsv.cn/Article/details/gzfridpbr.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvmgpgvwa.sHtML

[T01] Kotlin：Hello World
来源：http://blog.tarul.cn/Article/details/gnfgraxcz.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gflptzkqk.sHtML

[T02] Kotlin：变量
来源：http://baike.tarul.cn/Article/details/glpdsjkrl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.tarul.cn/Article/details/gjhtviura.sHtML


<!-- 参考信息 -->