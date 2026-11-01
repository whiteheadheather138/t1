代发 wailian999

set -euo pipefail
来源：http://mobile.fktsv.cn/Article/details/gtdgdacxa.sHtML

[R02] 变量赋值与使用
来源：http://blog.epnwcf.com/Article/details/gmtputwie.sHtML

name="Tom"; echo "$name"
来源：http://m.share.bbcook.cn/Article/details/gycgkomlq.sHtML

[R03] 只读变量
来源：http://m.share.yfazqb.com/Article/details/gduqpmuhp.sHtML

readonly PI=3.14
来源：http://baike.vehdjk.com/Article/details/gizkvyafe.sHtML

[R04] 位置参数
来源：http://3g.tarul.cn/Article/details/gmwzohyvh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.tarul.cn/Article/details/gakjwozte.sHtML

[R05] 参数默认值
来源：http://blog.yfazqb.com/Article/details/gzklkxkqw.sHtML

name="${1:-default}"
来源：http://www.blog.yfazqb.com/Article/details/gnsayxdui.sHtML

[R06] 判断命令是否存在
来源：http://3g.yfazqb.com/Article/details/gqkbnfeml.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.sjlbkw.cn/Article/details/gbzulmdej.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gvtdmjyiu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.tarul.cn/Article/details/grlqnnnua.sHtML

[R08] 数值比较
来源：http://m.share.bbcook.cn/Article/details/gyecjlvae.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fktsv.cn/Article/details/gecakuhss.sHtML

[R09] 字符串比较
来源：http://read.share.yfazqb.com/Article/details/gumnsekzu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fktsv.cn/Article/details/glffijcbi.sHtML

[R10] 正则匹配
来源：http://baike.sjlbkw.cn/Article/details/gvmibsqbc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.vehdjk.com/Article/details/geugtbrub.sHtML

[R11] case 多分支
来源：http://m.share.fktsv.cn/Article/details/geswdyjiy.sHtML

case "$1" in
来源：http://wap.vehdjk.com/Article/details/gtdxghiny.sHtML

start) echo "启动" ;;
来源：http://wap.sjlbkw.cn/Article/details/gddmdcnkv.sHtML

stop)  echo "停止" ;;
来源：http://wap.yfazqb.com/Article/details/gyzggjwig.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fktsv.cn/Article/details/gsscicuyc.sHtML

esac
来源：http://www.m.share.sjlbkw.cn/Article/details/gruibamqp.sHtML

[R12] for 遍历文件
来源：http://m.share.tarul.cn/Article/details/gblgkcqjp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/grlayrwyt.sHtML

[R13] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/gscfmwyxr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gtzehvmcl.sHtML

[R14] C 风格 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxpxoffi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gkouzdlrc.sHtML

[R15] while 逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gsnwdsdma.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.bbcook.cn/Article/details/gkwsurhnl.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/gxeoxqxpt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gesvtwlwi.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fktsv.cn/Article/details/ggrfqfxkc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fktsv.cn/Article/details/gtwtubxyp.sHtML

[R18] 遍历数组
来源：http://baike.fktsv.cn/Article/details/gpdibkxbe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fktsv.cn/Article/details/gmvgldtjp.sHtML

[R19] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gjipshczp.sHtML

echo "${#arr[@]}"
来源：http://www.share.bbcook.cn/Article/details/gizigmciq.sHtML

[R20] 关联数组（字典）
来源：http://www.share.epnwcf.com/Article/details/gycladhht.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.bbcook.cn/Article/details/gdgjscmrk.sHtML

[R21] 字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/gkxebcbae.sHtML

echo "${#s}"
来源：http://blog.sjlbkw.cn/Article/details/gplvbgfue.sHtML

[R22] 截取子串
来源：http://3g.yfazqb.com/Article/details/glikuuiee.sHtML

echo "${s:0:5}"
来源：http://mobile.sjlbkw.cn/Article/details/gskdwrviu.sHtML

[R23] 字符串替换
来源：http://wap.yfazqb.com/Article/details/gjnuraeqe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fktsv.cn/Article/details/geivfxabx.sHtML

[R24] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gqwpbiucx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.yfazqb.com/Article/details/grgfuautq.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.sjlbkw.cn/Article/details/giiemqcuk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.bbcook.cn/Article/details/ggwsaxtlc.sHtML

[R26] 命令替换
来源：http://www.share.sjlbkw.cn/Article/details/gxhmstgey.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.sjlbkw.cn/Article/details/gjcmmkrsd.sHtML

[R27] 算术展开
来源：http://m.share.yfazqb.com/Article/details/gurkdflti.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/gxuihygvl.sHtML

[R28] 浮点运算
来源：http://baike.vehdjk.com/Article/details/glbfhxmdv.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.vehdjk.com/Article/details/gvcztzcxq.sHtML

[R29] 定义函数
来源：http://blog.vehdjk.com/Article/details/gmwgkblrg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.tarul.cn/Article/details/gmfwmtsvv.sHtML

[R30] 函数返回状态码
来源：http://m.share.epnwcf.com/Article/details/gymoiavtf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.vehdjk.com/Article/details/gshqrilgp.sHtML

[R31] 局部变量
来源：http://wap.tarul.cn/Article/details/gjicameoo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.epnwcf.com/Article/details/gmztowjbt.sHtML

[R32] 参数个数校验
来源：http://baike.bbcook.cn/Article/details/gdkknqfsg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/gimtnftyd.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.sjlbkw.cn/Article/details/gabghcbdp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.epnwcf.com/Article/details/gvwhzmvlm.sHtML

[R34] 退出时清理
来源：http://m.share.vehdjk.com/Article/details/gcdhqndpw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/gogipqhnm.sHtML

[R35] 后台执行并等待
来源：http://blog.fktsv.cn/Article/details/glqedvhml.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.vehdjk.com/Article/details/gcdhijkkz.sHtML

[R36] 并发执行多个任务
来源：http://mobile.yfazqb.com/Article/details/gbivxvxoy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/grocmccbg.sHtML

[R37] 把输出赋给变量
来源：http://blog.epnwcf.com/Article/details/gjhyekliq.sHtML

files=$(ls -1)
来源：http://www.blog.bbcook.cn/Article/details/gxywqzjfz.sHtML

[R38] 管道串联
来源：http://mobile.vehdjk.com/Article/details/gjrntjujt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.bbcook.cn/Article/details/gjpjyodcz.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.sjlbkw.cn/Article/details/gtunzecvt.sHtML

cmd > out.log 2>&1
来源：http://m.share.bbcook.cn/Article/details/goqemhejp.sHtML

[R40] 追加写日志
来源：http://www.share.sjlbkw.cn/Article/details/guusdvrbt.sHtML

echo "log" >> out.log
来源：http://www.share.epnwcf.com/Article/details/gbzpyffjx.sHtML

[R41] 丢弃输出
来源：http://baike.fktsv.cn/Article/details/gjwsfiehm.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/gfcwxgyow.sHtML

[R42] 输入重定向
来源：http://wap.sjlbkw.cn/Article/details/gbtxeehel.sHtML

wc -l < a.txt
来源：http://www.share.fktsv.cn/Article/details/gjnuxoaii.sHtML

[R43] 按名字查找文件
来源：http://baike.tarul.cn/Article/details/gvgtjwwrl.sHtML

find . -name "*.log" -type f
来源：http://3g.fktsv.cn/Article/details/grpvyjapz.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gknqqiyfq.sHtML

find . -mtime -7 -type f
来源：http://read.share.epnwcf.com/Article/details/gphydiawy.sHtML

[R45] 批量删除
来源：http://wap.bbcook.cn/Article/details/gubjvgtjm.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.epnwcf.com/Article/details/glumcjvvu.sHtML

[R46] 递归替换文件内容
来源：http://www.share.bbcook.cn/Article/details/gbzxpvniy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.epnwcf.com/Article/details/gjnmgvkhz.sHtML

[R47] sed 单行替换
来源：http://www.share.fktsv.cn/Article/details/gbhhotxiu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.sjlbkw.cn/Article/details/greeqlsmi.sHtML

[R48] awk 取指定列
来源：http://baike.yfazqb.com/Article/details/gvutkeudr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gzjlzcout.sHtML

[R49] awk 带条件
来源：http://baike.fktsv.cn/Article/details/gnbzxtvjp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.sjlbkw.cn/Article/details/gvvbplpzu.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/gydqaqfsv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gdzbptrvo.sHtML

[R51] 排序去重取前几
来源：http://www.share.yfazqb.com/Article/details/grkptnrrx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.yfazqb.com/Article/details/ggguuwyfh.sHtML

[R52] 统计行数
来源：http://www.share.fktsv.cn/Article/details/gvpnsdmgx.sHtML

wc -l a.txt
来源：http://wap.fktsv.cn/Article/details/guiiopnlf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.sjlbkw.cn/Article/details/gplptesne.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.vehdjk.com/Article/details/gebyaqkdm.sHtML

[R54] 比较两个文件
来源：http://www.m.share.tarul.cn/Article/details/gushppmuj.sHtML

diff a.txt b.txt
来源：http://mobile.fktsv.cn/Article/details/gouadxocd.sHtML

[R55] 压缩与解压
来源：http://m.share.epnwcf.com/Article/details/gmgktioqu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.epnwcf.com/Article/details/genangndi.sHtML

[R56] 远程拷贝
来源：http://mobile.epnwcf.com/Article/details/gxstlrwop.sHtML

scp file user@host:/path/
来源：http://baike.fktsv.cn/Article/details/ghyxjvhio.sHtML

[R57] 远程执行命令
来源：http://3g.bbcook.cn/Article/details/gyoeovgfu.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.epnwcf.com/Article/details/gmvxpyghl.sHtML

[R58] 下载文件
来源：http://baike.tarul.cn/Article/details/ggzxadcbg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.sjlbkw.cn/Article/details/guktniigo.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gvmsmbobx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fktsv.cn/Article/details/gifcgjddr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gyhbpyqrh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.sjlbkw.cn/Article/details/gzialfszd.sHtML

[R61] 磁盘占用
来源：http://mobile.tarul.cn/Article/details/gmnphhxzh.sHtML

df -h;  du -sh *
来源：http://mobile.vehdjk.com/Article/details/gvxornydt.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/gjczronns.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.yfazqb.com/Article/details/gawtlueto.sHtML

[R63] 内存与进程
来源：http://www.blog.tarul.cn/Article/details/ggphwlims.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.epnwcf.com/Article/details/gcbikthtv.sHtML

[R64] 结束进程
来源：http://wap.tarul.cn/Article/details/gvgswxzen.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/gmxlygfdp.sHtML

[R65] 查看端口占用
来源：http://read.share.yfazqb.com/Article/details/gjawxqrpq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/gwpxhatjl.sHtML

[R66] 定时任务
来源：http://blog.tarul.cn/Article/details/gdgihdkvi.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdpkzfes.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fktsv.cn/Article/details/gtopvysch.sHtML

openssl rand -hex 16
来源：http://m.share.sjlbkw.cn/Article/details/ggvqpdvse.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/grofolwdd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.epnwcf.com/Article/details/gvmpkqjhd.sHtML

[R69] 生成随机密码
来源：http://read.share.epnwcf.com/Article/details/grcquofob.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.yfazqb.com/Article/details/gwdwgvugk.sHtML

[R70] 时间戳与互转
来源：http://3g.bbcook.cn/Article/details/gtqxvbipc.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.sjlbkw.cn/Article/details/ggshzvzhq.sHtML

[R71] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gogsmayxr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.vehdjk.com/Article/details/gjzhhmqrj.sHtML

[R72] 等待端口就绪
来源：http://read.share.yfazqb.com/Article/details/gbdulcesl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gfolxojmp.sHtML

[R73] 分割大日志
来源：http://www.share.fktsv.cn/Article/details/gqfsfxzdj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.tarul.cn/Article/details/grirhaweh.sHtML

[R74] 批量重命名
来源：http://www.m.share.fktsv.cn/Article/details/gvaqgijsz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fktsv.cn/Article/details/gilfsrvkr.sHtML

[R75] 导出环境变量
来源：http://m.share.bbcook.cn/Article/details/gkwqaysej.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.vehdjk.com/Article/details/gdxjlqecq.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/gkyisjvod.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gxeaucnrj.sHtML

[R77] 读取用户输入
来源：http://read.share.epnwcf.com/Article/details/gpcmhhftq.sHtML

read -rp "请输入: " ans
来源：http://wap.fktsv.cn/Article/details/gpqprkdva.sHtML

[R78] 交互式菜单
来源：http://mobile.fktsv.cn/Article/details/grtusjrkr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.bbcook.cn/Article/details/gbnfmulpr.sHtML

[R79] 解析命令行选项
来源：http://m.share.tarul.cn/Article/details/gpelzaqoe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.vehdjk.com/Article/details/gzgsikrva.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.yfazqb.com/Article/details/gteaqzjxd.sHtML

time ./run.sh
来源：http://baike.fktsv.cn/Article/details/gahevegeo.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfrlphvpo.sHtML

S. C / C++ 专题
来源：http://www.share.epnwcf.com/Article/details/glnlvsozs.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/galhugfzg.sHtML

[S01] C：Hello World
来源：http://m.share.yfazqb.com/Article/details/gwrtsjnas.sHtML

#include <stdio.h>
来源：http://m.share.bbcook.cn/Article/details/gfdxgsgak.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.yfazqb.com/Article/details/guqvkxkpb.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.vehdjk.com/Article/details/ggbbhwael.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.yfazqb.com/Article/details/gebohtaax.sHtML

[S03] C：读入整数
来源：http://www.m.share.epnwcf.com/Article/details/gtgnkkevw.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/gqzzupcdu.sHtML

[S04] C：字符串复制
来源：http://blog.bbcook.cn/Article/details/gjwjjxkqs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/gwwgaumbh.sHtML

[S05] C：字符串长度
来源：http://m.share.vehdjk.com/Article/details/gnxfiofok.sHtML

strlen(s)
来源：http://read.share.bbcook.cn/Article/details/glzuddohc.sHtML

[S06] C：字符串比较
来源：http://mobile.vehdjk.com/Article/details/giajuscax.sHtML

strcmp(a, b) == 0
来源：http://read.share.bbcook.cn/Article/details/gkfotazao.sHtML

[S07] C：数组遍历求和
来源：http://www.share.bbcook.cn/Article/details/ggsvmzlbd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.epnwcf.com/Article/details/godjkvogd.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gkinrnktq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.epnwcf.com/Article/details/gspfjqgja.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.vehdjk.com/Article/details/ggsvhsujk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.yfazqb.com/Article/details/gdxuzuinr.sHtML

[S10] C：指针与解引用
来源：http://3g.tarul.cn/Article/details/gvfurpqpd.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fktsv.cn/Article/details/gybewpcqk.sHtML

[S11] C：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gfpxvrypo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.yfazqb.com/Article/details/grmfpxkuc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.bbcook.cn/Article/details/gyuoskoif.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/gxbvhcycs.sHtML

[S12] C：写文件
来源：http://m.share.tarul.cn/Article/details/gohldyamj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gbtkhspot.sHtML

[S13] C：宏定义
来源：http://mobile.bbcook.cn/Article/details/gnezpygxw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.vehdjk.com/Article/details/gwcmfjxdp.sHtML

[S14] C：枚举
来源：http://read.share.yfazqb.com/Article/details/gsokzrdfr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/gpooxoblf.sHtML

[S15] C：类型转换
来源：http://read.share.epnwcf.com/Article/details/glljvrgpa.sHtML

(double) a / b
来源：http://www.m.share.epnwcf.com/Article/details/gchwnskfa.sHtML

[S16] C：位操作置位
来源：http://baike.bbcook.cn/Article/details/gedbnfqqp.sHtML

x |= (1 << 3);
来源：http://3g.bbcook.cn/Article/details/gicdyhvww.sHtML

[S17] C：安全拼接字符串
来源：http://wap.vehdjk.com/Article/details/grdotltvd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/gelnuwvre.sHtML

[S18] C：命令行参数
来源：http://www.share.fktsv.cn/Article/details/glnqvxkoh.sHtML

int main(int argc, char **argv)
来源：http://read.share.tarul.cn/Article/details/gqufgbzcp.sHtML

[S19] C：快速排序
来源：http://www.share.bbcook.cn/Article/details/gvwtyyfuf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gkesdklmt.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/gmoabwthh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/gzmwytuaa.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/ghemrlckj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.tarul.cn/Article/details/ghjbslhvn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fktsv.cn/Article/details/gblspuucl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.epnwcf.com/Article/details/gkastqivc.sHtML

[S23] C：随机数
来源：http://www.share.fktsv.cn/Article/details/gnsjqvyxl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.vehdjk.com/Article/details/gibggbisx.sHtML

[S24] C：获取本地时间
来源：http://blog.sjlbkw.cn/Article/details/gzchzttcv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fktsv.cn/Article/details/gykjqoddn.sHtML

[S25] C：内存拷贝
来源：http://blog.vehdjk.com/Article/details/gumunzlry.sHtML

memcpy(dst, src, n);
来源：http://blog.vehdjk.com/Article/details/ggkmpxgab.sHtML

[S26] C：内存清零
来源：http://www.blog.fktsv.cn/Article/details/gvzfaqleb.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/gfozlpexe.sHtML

[S27] C：定义常量
来源：http://www.m.share.epnwcf.com/Article/details/gldfubvhi.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gufwvfqub.sHtML

[S28] C：静态变量
来源：http://wap.epnwcf.com/Article/details/gjplwkkme.sHtML

static int counter = 0;
来源：http://www.blog.sjlbkw.cn/Article/details/gcjbdgedz.sHtML

[S29] C：变参函数
来源：http://www.m.share.yfazqb.com/Article/details/gtrjylaeo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.epnwcf.com/Article/details/gldbbilzq.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gdqmwqbnl.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/gqedpvvqa.sHtML

#define X_H
来源：http://baike.fktsv.cn/Article/details/ggsyjjvoc.sHtML

#endif
来源：http://mobile.fktsv.cn/Article/details/gjhiozbkf.sHtML

[S31] C++：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gzrvoklqx.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/glxncnfpt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.tarul.cn/Article/details/gslwujyjf.sHtML

[S32] C++：字符串
来源：http://mobile.tarul.cn/Article/details/gwzbjxbdy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fktsv.cn/Article/details/grxbhnusj.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.vehdjk.com/Article/details/gwtxvgwrl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.bbcook.cn/Article/details/gddpuvfcc.sHtML

[S34] C++：遍历 vector
来源：http://blog.vehdjk.com/Article/details/gxcozxwnc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.bbcook.cn/Article/details/gcwtqzmnv.sHtML

[S35] C++：map
来源：http://blog.bbcook.cn/Article/details/gxwjqgsnq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/glqztarld.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.yfazqb.com/Article/details/gwnqmjjtr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gsxhmquya.sHtML

[S37] C++：set
来源：http://read.share.fktsv.cn/Article/details/gzjzgqvit.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.yfazqb.com/Article/details/gkjvdfemu.sHtML

[S38] C++：排序
来源：http://mobile.yfazqb.com/Article/details/grgnlienz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gffmagpmz.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fktsv.cn/Article/details/gdttjiiei.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/ghzznkqvy.sHtML

[S40] C++：查找元素
来源：http://www.blog.sjlbkw.cn/Article/details/grmdfddnh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.sjlbkw.cn/Article/details/ggrunfxme.sHtML

[S41] C++：类与构造函数
来源：http://3g.epnwcf.com/Article/details/gmiswjslb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.epnwcf.com/Article/details/gkffhybcs.sHtML

[S42] C++：继承与虚函数
来源：http://3g.tarul.cn/Article/details/glmuzcnpa.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.tarul.cn/Article/details/gbmpqdcvo.sHtML

[S43] C++：智能指针
来源：http://blog.tarul.cn/Article/details/gbakhwxmd.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.sjlbkw.cn/Article/details/gwprubzus.sHtML

[S44] C++：引用传参
来源：http://blog.vehdjk.com/Article/details/guzjertwj.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/gyfucwoik.sHtML

[S45] C++：lambda
来源：http://www.blog.sjlbkw.cn/Article/details/gcfugxvwc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.vehdjk.com/Article/details/galdlnxsf.sHtML

[S46] C++：函数模板
来源：http://blog.tarul.cn/Article/details/ghxxyopgm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.yfazqb.com/Article/details/gjfgvpowh.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.bbcook.cn/Article/details/gtfycnifa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/gupontvvx.sHtML

[S48] C++：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gqcmqndnj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.bbcook.cn/Article/details/gbjmoiubl.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/gjjvnnbju.sHtML

[S49] C++：写文件
来源：http://baike.epnwcf.com/Article/details/ggrhpeexe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.epnwcf.com/Article/details/gzgmjjuqj.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/gdthsnqrt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gwszbyumk.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gshiebwlu.sHtML

static_cast<double>(a) / b
来源：http://m.share.sjlbkw.cn/Article/details/gfqciakns.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.yfazqb.com/Article/details/gvbdpupvv.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fktsv.cn/Article/details/giuspxiph.sHtML

[S53] C++：移动语义
来源：http://read.share.sjlbkw.cn/Article/details/gjwsyliva.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.sjlbkw.cn/Article/details/guocobaqx.sHtML

[S54] C++：异常处理
来源：http://wap.bbcook.cn/Article/details/gyfalrnbz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.epnwcf.com/Article/details/gprknvtat.sHtML

[S55] C++：结构化绑定
来源：http://read.share.yfazqb.com/Article/details/gvywijrrw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.epnwcf.com/Article/details/ggxephuwo.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/gqxpxghag.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcysnfdys.sHtML

[S57] C++：编译期常量
来源：http://mobile.fktsv.cn/Article/details/gvicgnhqi.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/ghlzhtwkb.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/gzyrmexxs.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fktsv.cn/Article/details/gytnoiktz.sHtML

[S59] C++：静态断言
来源：http://www.m.share.bbcook.cn/Article/details/ggacldikx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fktsv.cn/Article/details/gqcgpmghk.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gmqucqhoe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/grvtsvznq.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gicjjxbke.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fktsv.cn/Article/details/ghrkdfjjb.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gccyrychn.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/givstpcts.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gjzdyaeah.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/guawgepym.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.sjlbkw.cn/Article/details/gbnkfhrtg.sHtML


<!-- 参考信息 -->