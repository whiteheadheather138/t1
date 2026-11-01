代发 wailian999

R. Bash 专题
来源：http://read.share.bbcook.cn/Article/details/gwrkpsxfa.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtdmzucjf.sHtML

[R01] shebang 与严格模式
来源：http://wap.epnwcf.com/Article/details/gcmdwojfh.sHtML

#!/usr/bin/env bash
来源：http://www.share.sjlbkw.cn/Article/details/ghfkaxcih.sHtML

set -euo pipefail
来源：http://www.blog.tarul.cn/Article/details/gzahemfnq.sHtML

[R02] 变量赋值与使用
来源：http://mobile.sjlbkw.cn/Article/details/gsjwvnlyt.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/guuerugox.sHtML

[R03] 只读变量
来源：http://m.share.vehdjk.com/Article/details/gdrndjhop.sHtML

readonly PI=3.14
来源：http://blog.bbcook.cn/Article/details/grdihmjnk.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/ghhfxgvqe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.yfazqb.com/Article/details/guvtstppi.sHtML

[R05] 参数默认值
来源：http://wap.yfazqb.com/Article/details/gnhoravkq.sHtML

name="${1:-default}"
来源：http://m.share.sjlbkw.cn/Article/details/gbhctnrrc.sHtML

[R06] 判断命令是否存在
来源：http://mobile.epnwcf.com/Article/details/gyfpisskf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/ggjfmamvg.sHtML

[R07] if 判断文件
来源：http://read.share.vehdjk.com/Article/details/gcuhtuiap.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.epnwcf.com/Article/details/gulnvcxfj.sHtML

[R08] 数值比较
来源：http://www.blog.tarul.cn/Article/details/ggspzavww.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gdvjeslci.sHtML

[R09] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gkrhgsscd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.epnwcf.com/Article/details/gdvcduass.sHtML

[R10] 正则匹配
来源：http://wap.fktsv.cn/Article/details/gumutmqzr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.epnwcf.com/Article/details/guoapcyoy.sHtML

[R11] case 多分支
来源：http://read.share.fktsv.cn/Article/details/gwbasozbm.sHtML

case "$1" in
来源：http://www.blog.sjlbkw.cn/Article/details/glydayklj.sHtML

start) echo "启动" ;;
来源：http://baike.vehdjk.com/Article/details/geecwjjlb.sHtML

stop)  echo "停止" ;;
来源：http://wap.bbcook.cn/Article/details/gauykqwsg.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gytjwkawb.sHtML

esac
来源：http://mobile.bbcook.cn/Article/details/gzybfmnlb.sHtML

[R12] for 遍历文件
来源：http://m.share.sjlbkw.cn/Article/details/gtiudrhui.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.epnwcf.com/Article/details/gloafbqac.sHtML

[R13] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/gydxqhmyu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/gmhjkvysk.sHtML

[R14] C 风格 for
来源：http://3g.bbcook.cn/Article/details/gnbpitzle.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gchvanach.sHtML

[R15] while 逐行读文件
来源：http://wap.bbcook.cn/Article/details/gzjotmqre.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.epnwcf.com/Article/details/gefbxiogz.sHtML

[R16] until 等待条件
来源：http://www.blog.epnwcf.com/Article/details/gkyjlmkgu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/ghpksswqs.sHtML

[R17] 数组定义与取值
来源：http://baike.yfazqb.com/Article/details/gsbnhupym.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/ggkywdotv.sHtML

[R18] 遍历数组
来源：http://www.m.share.bbcook.cn/Article/details/gzrkmpxcd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.sjlbkw.cn/Article/details/gdmobdpbx.sHtML

[R19] 数组长度
来源：http://baike.fktsv.cn/Article/details/gotdspqii.sHtML

echo "${#arr[@]}"
来源：http://baike.epnwcf.com/Article/details/gwrseozyb.sHtML

[R20] 关联数组（字典）
来源：http://3g.vehdjk.com/Article/details/gvdtxmsfb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.epnwcf.com/Article/details/gioshxpin.sHtML

[R21] 字符串长度
来源：http://m.share.tarul.cn/Article/details/gugpojsgx.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gbsptzson.sHtML

[R22] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/gvftjnieu.sHtML

echo "${s:0:5}"
来源：http://mobile.bbcook.cn/Article/details/gjgcatlfz.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/guxcstlge.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gtiirrebs.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gvbgtoawr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.tarul.cn/Article/details/gryzxhtrf.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.bbcook.cn/Article/details/ggafvcpto.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.epnwcf.com/Article/details/gnrrxuqha.sHtML

[R26] 命令替换
来源：http://read.share.vehdjk.com/Article/details/gjoljrenq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.bbcook.cn/Article/details/gsvsllfro.sHtML

[R27] 算术展开
来源：http://blog.bbcook.cn/Article/details/gixvxnsyc.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/gesqzudil.sHtML

[R28] 浮点运算
来源：http://3g.epnwcf.com/Article/details/gffzrggvf.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/gzfqwvrux.sHtML

[R29] 定义函数
来源：http://blog.fktsv.cn/Article/details/gfjpjkmcn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.yfazqb.com/Article/details/geyvbgdyd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.yfazqb.com/Article/details/gtltiowgm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.yfazqb.com/Article/details/goatbjxgj.sHtML

[R31] 局部变量
来源：http://blog.vehdjk.com/Article/details/goaolzels.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.sjlbkw.cn/Article/details/gajjgysiy.sHtML

[R32] 参数个数校验
来源：http://read.share.sjlbkw.cn/Article/details/gillfajlt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gufypgoru.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.epnwcf.com/Article/details/gmdrxjnmw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.vehdjk.com/Article/details/gsgrosfqr.sHtML

[R34] 退出时清理
来源：http://m.share.tarul.cn/Article/details/gjkkkjkzz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gljfemjbi.sHtML

[R35] 后台执行并等待
来源：http://mobile.tarul.cn/Article/details/gcyfmhtxl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.vehdjk.com/Article/details/gheksllft.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.yfazqb.com/Article/details/gckfvnsvm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.tarul.cn/Article/details/ghmjdkiyi.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.tarul.cn/Article/details/gtxemlvpp.sHtML

files=$(ls -1)
来源：http://www.share.yfazqb.com/Article/details/ggwahtmsf.sHtML

[R38] 管道串联
来源：http://read.share.yfazqb.com/Article/details/ggwsvvpam.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.sjlbkw.cn/Article/details/gvsikdfbv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.bbcook.cn/Article/details/ghkmzhxot.sHtML

cmd > out.log 2>&1
来源：http://read.share.vehdjk.com/Article/details/giryyufle.sHtML

[R40] 追加写日志
来源：http://blog.epnwcf.com/Article/details/gsvdabncb.sHtML

echo "log" >> out.log
来源：http://3g.epnwcf.com/Article/details/glfogteiv.sHtML

[R41] 丢弃输出
来源：http://www.blog.yfazqb.com/Article/details/grrukmjwz.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gqsdbdhwo.sHtML

[R42] 输入重定向
来源：http://mobile.epnwcf.com/Article/details/gegavtnyo.sHtML

wc -l < a.txt
来源：http://blog.bbcook.cn/Article/details/gokrcdmqh.sHtML

[R43] 按名字查找文件
来源：http://m.share.vehdjk.com/Article/details/gccivhsrw.sHtML

find . -name "*.log" -type f
来源：http://baike.tarul.cn/Article/details/gbvyxpqoh.sHtML

[R44] 按修改时间查找
来源：http://blog.tarul.cn/Article/details/gdzshejgp.sHtML

find . -mtime -7 -type f
来源：http://m.share.tarul.cn/Article/details/gftuxrwdg.sHtML

[R45] 批量删除
来源：http://read.share.epnwcf.com/Article/details/ghbrtvpsu.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fktsv.cn/Article/details/grhwmytsc.sHtML

[R46] 递归替换文件内容
来源：http://read.share.vehdjk.com/Article/details/gxshwklfk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.sjlbkw.cn/Article/details/gdrfddroa.sHtML

[R47] sed 单行替换
来源：http://blog.bbcook.cn/Article/details/gmzmioibc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.sjlbkw.cn/Article/details/glszrzerl.sHtML

[R48] awk 取指定列
来源：http://www.blog.fktsv.cn/Article/details/gvfslwmzp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.bbcook.cn/Article/details/gzoqtjbcu.sHtML

[R49] awk 带条件
来源：http://blog.vehdjk.com/Article/details/gxdvtqqyp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.sjlbkw.cn/Article/details/gixwjwwez.sHtML

[R50] awk 求和
来源：http://www.blog.fktsv.cn/Article/details/gtpljuods.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.tarul.cn/Article/details/gyapsfltk.sHtML

[R51] 排序去重取前几
来源：http://wap.fktsv.cn/Article/details/gbcmoyxij.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.bbcook.cn/Article/details/gvtyvoslx.sHtML

[R52] 统计行数
来源：http://baike.yfazqb.com/Article/details/glchehjho.sHtML

wc -l a.txt
来源：http://blog.yfazqb.com/Article/details/grnxexrgw.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.bbcook.cn/Article/details/gvybbnbba.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fktsv.cn/Article/details/ggafrbefw.sHtML

[R54] 比较两个文件
来源：http://www.blog.bbcook.cn/Article/details/gmevxoesc.sHtML

diff a.txt b.txt
来源：http://baike.yfazqb.com/Article/details/gqnskuqsb.sHtML

[R55] 压缩与解压
来源：http://m.share.vehdjk.com/Article/details/gorpasiie.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.epnwcf.com/Article/details/ggznvpvnx.sHtML

[R56] 远程拷贝
来源：http://read.share.fktsv.cn/Article/details/gevkdyzsu.sHtML

scp file user@host:/path/
来源：http://www.share.epnwcf.com/Article/details/gsgdbobwc.sHtML

[R57] 远程执行命令
来源：http://read.share.vehdjk.com/Article/details/gynzzjunh.sHtML

ssh user@host 'uptime'
来源：http://mobile.epnwcf.com/Article/details/gphukjthz.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/grkbbcflf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fktsv.cn/Article/details/gxxhubvgi.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gnvwigbdc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.bbcook.cn/Article/details/gwzutqdwf.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/gdopjemgf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.yfazqb.com/Article/details/gtitozqem.sHtML

[R61] 磁盘占用
来源：http://www.blog.tarul.cn/Article/details/gmqpungqy.sHtML

df -h;  du -sh *
来源：http://www.share.yfazqb.com/Article/details/ggtduwofh.sHtML

[R62] 找最占空间的文件
来源：http://wap.vehdjk.com/Article/details/gdmvzsydl.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.vehdjk.com/Article/details/gtbuufkvi.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gwukihyjl.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.epnwcf.com/Article/details/gorysstyo.sHtML

[R64] 结束进程
来源：http://www.blog.sjlbkw.cn/Article/details/gwnmkihmw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.epnwcf.com/Article/details/grtzqqjnx.sHtML

[R65] 查看端口占用
来源：http://m.share.fktsv.cn/Article/details/gqgxqmjxm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.tarul.cn/Article/details/gbqggxvgl.sHtML

[R66] 定时任务
来源：http://wap.sjlbkw.cn/Article/details/ggwbyoxdx.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/gbbmyqcdh.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.yfazqb.com/Article/details/gduljsrbo.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/gqtvxlkwa.sHtML

[R68] 计算文件校验值
来源：http://m.share.yfazqb.com/Article/details/gfhghvbtg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.bbcook.cn/Article/details/gkiaoeqyt.sHtML

[R69] 生成随机密码
来源：http://3g.epnwcf.com/Article/details/gaxuxiroh.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.vehdjk.com/Article/details/ghbqkhvdl.sHtML

[R70] 时间戳与互转
来源：http://www.share.epnwcf.com/Article/details/groidqrye.sHtML

date +%s;  date -d @1700000000
来源：http://3g.epnwcf.com/Article/details/gjkvkcmgg.sHtML

[R71] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gjrocgwtd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.tarul.cn/Article/details/glacokkco.sHtML

[R72] 等待端口就绪
来源：http://baike.epnwcf.com/Article/details/gfkkyeyio.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gxmlgiogm.sHtML

[R73] 分割大日志
来源：http://wap.sjlbkw.cn/Article/details/gutkomfyp.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/gcebqokii.sHtML

[R74] 批量重命名
来源：http://www.blog.tarul.cn/Article/details/gjykebyvz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.yfazqb.com/Article/details/gidsnqajt.sHtML

[R75] 导出环境变量
来源：http://m.share.vehdjk.com/Article/details/gxjksuxmc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fktsv.cn/Article/details/gjsjzkplo.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/gdetqcpdu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/glopzgprf.sHtML

[R77] 读取用户输入
来源：http://mobile.fktsv.cn/Article/details/gwofdiwto.sHtML

read -rp "请输入: " ans
来源：http://blog.epnwcf.com/Article/details/gkvdmrmdg.sHtML

[R78] 交互式菜单
来源：http://www.share.epnwcf.com/Article/details/gduwaiqvu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.vehdjk.com/Article/details/gzqmaugco.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/gvyskmzxl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gktsubbxv.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.vehdjk.com/Article/details/glxwlzmxh.sHtML

time ./run.sh
来源：http://baike.fktsv.cn/Article/details/gzfdgxihz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gkyhtresn.sHtML

S. C / C++ 专题
来源：http://baike.vehdjk.com/Article/details/gizqxycoc.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gwseejydh.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/gcjxvruid.sHtML

#include <stdio.h>
来源：http://read.share.yfazqb.com/Article/details/gmoirayhy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.epnwcf.com/Article/details/gypxphtga.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.vehdjk.com/Article/details/gkqddngkz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.epnwcf.com/Article/details/gxiopgprh.sHtML

[S03] C：读入整数
来源：http://3g.sjlbkw.cn/Article/details/geqhrxpvg.sHtML

int x; scanf("%d", &x);
来源：http://3g.sjlbkw.cn/Article/details/gjzrqarmt.sHtML

[S04] C：字符串复制
来源：http://www.blog.sjlbkw.cn/Article/details/gnyrfpdhf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.tarul.cn/Article/details/gatpwwrsb.sHtML

[S05] C：字符串长度
来源：http://read.share.vehdjk.com/Article/details/gxlwkxbjd.sHtML

strlen(s)
来源：http://www.m.share.vehdjk.com/Article/details/gilzqvkbd.sHtML

[S06] C：字符串比较
来源：http://blog.yfazqb.com/Article/details/gcollwlyt.sHtML

strcmp(a, b) == 0
来源：http://mobile.bbcook.cn/Article/details/gjhimbwai.sHtML

[S07] C：数组遍历求和
来源：http://mobile.vehdjk.com/Article/details/gozjswgfg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.yfazqb.com/Article/details/gofokafsj.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.epnwcf.com/Article/details/gnhlkgimy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.bbcook.cn/Article/details/glpfizexy.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.yfazqb.com/Article/details/gbgxbdbuo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.epnwcf.com/Article/details/gnpmkljfk.sHtML

[S10] C：指针与解引用
来源：http://www.share.fktsv.cn/Article/details/glxveivuh.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fktsv.cn/Article/details/gxxkculdk.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gqmlywlkd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.epnwcf.com/Article/details/govfcuzjt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.sjlbkw.cn/Article/details/gutsjlilb.sHtML

fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gfhgtydua.sHtML

[S12] C：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gcphrlnvm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.vehdjk.com/Article/details/gfhohecse.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/gsiiqncgp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.bbcook.cn/Article/details/glyajuuso.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/glbourgzr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.yfazqb.com/Article/details/gduzhxkqc.sHtML

[S15] C：类型转换
来源：http://www.share.yfazqb.com/Article/details/gmaibkqhw.sHtML

(double) a / b
来源：http://read.share.fktsv.cn/Article/details/giptsiefj.sHtML

[S16] C：位操作置位
来源：http://www.blog.vehdjk.com/Article/details/ghkxfgmvt.sHtML

x |= (1 << 3);
来源：http://wap.tarul.cn/Article/details/gemlhyygb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.yfazqb.com/Article/details/glelseluz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.tarul.cn/Article/details/grguvoate.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/giuylrwgp.sHtML

int main(int argc, char **argv)
来源：http://mobile.tarul.cn/Article/details/ggtwyhxmj.sHtML

[S19] C：快速排序
来源：http://3g.bbcook.cn/Article/details/gahehmxos.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gzxmfsgla.sHtML

[S20] C：二分查找
来源：http://m.share.yfazqb.com/Article/details/gdyyfmqlo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gseucmlxh.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/gqbkvrafa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/gyrzmermv.sHtML

[S22] C：字符串转数字
来源：http://m.share.yfazqb.com/Article/details/gbqbjoutu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.sjlbkw.cn/Article/details/glgeeegox.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/glhcpijzl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fktsv.cn/Article/details/gaztelljb.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.epnwcf.com/Article/details/grrqiitle.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/ghiwpkgft.sHtML

[S25] C：内存拷贝
来源：http://wap.sjlbkw.cn/Article/details/gwhzlzghp.sHtML

memcpy(dst, src, n);
来源：http://blog.fktsv.cn/Article/details/gayngcppc.sHtML

[S26] C：内存清零
来源：http://3g.fktsv.cn/Article/details/gcjuhsfrj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/grvtpaoot.sHtML

[S27] C：定义常量
来源：http://baike.yfazqb.com/Article/details/gmszpcasn.sHtML

const double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gfkevmpdc.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/grwkdjhet.sHtML

static int counter = 0;
来源：http://read.share.sjlbkw.cn/Article/details/gmtkyritj.sHtML

[S29] C：变参函数
来源：http://www.share.yfazqb.com/Article/details/grhucjdwb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.tarul.cn/Article/details/gllojxjvr.sHtML

[S30] C：头文件保护
来源：http://baike.yfazqb.com/Article/details/gbwkfuins.sHtML

#ifndef X_H
来源：http://www.m.share.vehdjk.com/Article/details/ggutakqcx.sHtML

#define X_H
来源：http://blog.yfazqb.com/Article/details/gqbahxjuj.sHtML

#endif
来源：http://read.share.fktsv.cn/Article/details/glnbczyyl.sHtML

[S31] C++：Hello World
来源：http://wap.vehdjk.com/Article/details/gjkecugit.sHtML

#include <iostream>
来源：http://www.m.share.epnwcf.com/Article/details/gnaowfynh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.vehdjk.com/Article/details/grrcvmzml.sHtML

[S32] C++：字符串
来源：http://read.share.tarul.cn/Article/details/gkaglyago.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.tarul.cn/Article/details/gaknkhoso.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fktsv.cn/Article/details/gdbjrdhko.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.tarul.cn/Article/details/giigtdggv.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.bbcook.cn/Article/details/gtvorgdfb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.vehdjk.com/Article/details/gpncljwnm.sHtML

[S35] C++：map
来源：http://www.share.yfazqb.com/Article/details/grhxmyjgq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gxycoohnq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.tarul.cn/Article/details/gfvciznle.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/ghqwfvcue.sHtML

[S37] C++：set
来源：http://www.blog.yfazqb.com/Article/details/gfwefzciu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gmwnvojet.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/ghxctfxin.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.yfazqb.com/Article/details/gyspqqbrw.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.vehdjk.com/Article/details/gvildexsd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.vehdjk.com/Article/details/gpynlzmbx.sHtML

[S40] C++：查找元素
来源：http://www.m.share.bbcook.cn/Article/details/gkturvlaj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.sjlbkw.cn/Article/details/gnxswzuyb.sHtML

[S41] C++：类与构造函数
来源：http://www.share.tarul.cn/Article/details/gzegawzxb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.vehdjk.com/Article/details/gdtgayxak.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/gimxaawln.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.vehdjk.com/Article/details/gxbqcvpkv.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fktsv.cn/Article/details/gfnomgxgm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fktsv.cn/Article/details/gmeuoxnuh.sHtML

[S44] C++：引用传参
来源：http://3g.epnwcf.com/Article/details/gkolwyzxi.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.epnwcf.com/Article/details/gpekxmsjj.sHtML

[S45] C++：lambda
来源：http://blog.fktsv.cn/Article/details/gdkqxusyu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gefqdhoye.sHtML

[S46] C++：函数模板
来源：http://read.share.vehdjk.com/Article/details/gorkrwwkk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.vehdjk.com/Article/details/ggvurxlpv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fktsv.cn/Article/details/gpvryucip.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.vehdjk.com/Article/details/giihvctzi.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gbqgalvdr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.vehdjk.com/Article/details/gaxbzebsz.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.epnwcf.com/Article/details/gyhrrbnvz.sHtML

[S49] C++：写文件
来源：http://www.share.vehdjk.com/Article/details/gskpomnps.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.epnwcf.com/Article/details/gbepnrwrd.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/ghcjkymkr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.bbcook.cn/Article/details/gaftqjfmq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.tarul.cn/Article/details/gsingvgxc.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.vehdjk.com/Article/details/glqxwzzti.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fktsv.cn/Article/details/gupeiptng.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.sjlbkw.cn/Article/details/gllkoicsj.sHtML

[S53] C++：移动语义
来源：http://blog.epnwcf.com/Article/details/gzkrxwyyv.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/gaongwsut.sHtML

[S54] C++：异常处理
来源：http://3g.vehdjk.com/Article/details/gjsavvjqk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.yfazqb.com/Article/details/gvrkuuddf.sHtML

[S55] C++：结构化绑定
来源：http://wap.epnwcf.com/Article/details/ghcxldiwf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fktsv.cn/Article/details/gynnrpjom.sHtML

[S56] C++：optional
来源：http://baike.sjlbkw.cn/Article/details/gjlkkfxzw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.vehdjk.com/Article/details/gaykmkswp.sHtML

[S57] C++：编译期常量
来源：http://wap.vehdjk.com/Article/details/gwmamlknn.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/gylumduhw.sHtML

[S58] C++：命名空间
来源：http://www.blog.vehdjk.com/Article/details/gyjfdehsw.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/gqiqyxqzg.sHtML

[S59] C++：静态断言
来源：http://m.share.bbcook.cn/Article/details/gvmexpmit.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fktsv.cn/Article/details/gaijwlvaz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.vehdjk.com/Article/details/gpjigjxil.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gsyntzpgc.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grhptqryk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gusxwvmla.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gasakkvax.sHtML


<!-- 参考信息 -->