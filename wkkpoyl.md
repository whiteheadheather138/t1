代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/gdjuiqtoq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fktsv.cn/Article/details/ggbqynbmt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.tarul.cn/Article/details/gbfqvzaft.sHtML

[Q89] 判断表是否存在
来源：http://www.share.sjlbkw.cn/Article/details/giserpfnu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.sjlbkw.cn/Article/details/gywdhvrzk.sHtML

[Q90] 生成序号列
来源：http://baike.yfazqb.com/Article/details/gghdydmhl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.sjlbkw.cn/Article/details/gxgqdpjxw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfuzovgbu.sHtML

R. Bash 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gbrcfelkl.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdvyfzbte.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.tarul.cn/Article/details/gawkibfxf.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/gesrqioka.sHtML

set -euo pipefail
来源：http://www.blog.tarul.cn/Article/details/gkmhcsykp.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.epnwcf.com/Article/details/gypqaqrzf.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.bbcook.cn/Article/details/gthribzlb.sHtML

[R03] 只读变量
来源：http://baike.epnwcf.com/Article/details/gzgabmmzl.sHtML

readonly PI=3.14
来源：http://www.share.vehdjk.com/Article/details/gxsdsvqyn.sHtML

[R04] 位置参数
来源：http://www.blog.fktsv.cn/Article/details/gylpjociz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fktsv.cn/Article/details/ghnaevbss.sHtML

[R05] 参数默认值
来源：http://m.share.epnwcf.com/Article/details/gofmhofok.sHtML

name="${1:-default}"
来源：http://www.share.bbcook.cn/Article/details/gpzntwsbs.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fktsv.cn/Article/details/gsirypcrp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/glnlqasyf.sHtML

[R07] if 判断文件
来源：http://m.share.epnwcf.com/Article/details/gekhjphby.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.tarul.cn/Article/details/gddzmjddx.sHtML

[R08] 数值比较
来源：http://www.m.share.yfazqb.com/Article/details/ghgqkhqzk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.epnwcf.com/Article/details/grsaloqvd.sHtML

[R09] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gvoxkawim.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.tarul.cn/Article/details/gyxyuzbda.sHtML

[R10] 正则匹配
来源：http://baike.fktsv.cn/Article/details/gptnoyxjv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.tarul.cn/Article/details/gcaomuhkk.sHtML

[R11] case 多分支
来源：http://mobile.yfazqb.com/Article/details/ghwyeqwfw.sHtML

case "$1" in
来源：http://www.blog.fktsv.cn/Article/details/gginuzaen.sHtML

start) echo "启动" ;;
来源：http://3g.sjlbkw.cn/Article/details/gfavowozj.sHtML

stop)  echo "停止" ;;
来源：http://m.share.epnwcf.com/Article/details/grvowgmkm.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.bbcook.cn/Article/details/gusakrwzo.sHtML

esac
来源：http://www.blog.vehdjk.com/Article/details/grdwqcmmi.sHtML

[R12] for 遍历文件
来源：http://3g.fktsv.cn/Article/details/gisgegqkw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.vehdjk.com/Article/details/gwpkzfaqs.sHtML

[R13] for 计数循环
来源：http://blog.fktsv.cn/Article/details/gupmpznyn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gnbynjshz.sHtML

[R14] C 风格 for
来源：http://www.blog.yfazqb.com/Article/details/girgpizjq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gszzeunow.sHtML

[R15] while 逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gqemejhjc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.epnwcf.com/Article/details/gmswvfgqk.sHtML

[R16] until 等待条件
来源：http://3g.tarul.cn/Article/details/gnogvfzfz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gkwvhldaw.sHtML

[R17] 数组定义与取值
来源：http://www.blog.epnwcf.com/Article/details/ggxlgpuej.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.tarul.cn/Article/details/glyszebij.sHtML

[R18] 遍历数组
来源：http://www.blog.bbcook.cn/Article/details/gdfocnddg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.yfazqb.com/Article/details/gznwzicti.sHtML

[R19] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gxfijlnyp.sHtML

echo "${#arr[@]}"
来源：http://www.share.yfazqb.com/Article/details/gzrlirlad.sHtML

[R20] 关联数组（字典）
来源：http://wap.tarul.cn/Article/details/gowcenzoa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.bbcook.cn/Article/details/gszixnljh.sHtML

[R21] 字符串长度
来源：http://wap.yfazqb.com/Article/details/gcedbkeor.sHtML

echo "${#s}"
来源：http://baike.bbcook.cn/Article/details/gizjekdqn.sHtML

[R22] 截取子串
来源：http://blog.epnwcf.com/Article/details/gdnkxhzwr.sHtML

echo "${s:0:5}"
来源：http://m.share.vehdjk.com/Article/details/gadqlxeyb.sHtML

[R23] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gmadklehe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.sjlbkw.cn/Article/details/gtfwotvan.sHtML

[R24] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/ghmfqiynj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fktsv.cn/Article/details/gddogxcoy.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fktsv.cn/Article/details/gidmkmith.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.epnwcf.com/Article/details/gyyisvidp.sHtML

[R26] 命令替换
来源：http://www.m.share.vehdjk.com/Article/details/gdawefuvu.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.bbcook.cn/Article/details/geossrmuz.sHtML

[R27] 算术展开
来源：http://www.blog.sjlbkw.cn/Article/details/gtglfxbkd.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fktsv.cn/Article/details/gniftkwok.sHtML

[R28] 浮点运算
来源：http://m.share.bbcook.cn/Article/details/gklexxjdp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/guxjbcuer.sHtML

[R29] 定义函数
来源：http://www.share.tarul.cn/Article/details/gwejnlbea.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.tarul.cn/Article/details/gaalmqitq.sHtML

[R30] 函数返回状态码
来源：http://www.share.epnwcf.com/Article/details/gpmstbycq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.yfazqb.com/Article/details/gekgyugms.sHtML

[R31] 局部变量
来源：http://m.share.bbcook.cn/Article/details/gfyyqgjtt.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.tarul.cn/Article/details/gktmddrwf.sHtML

[R32] 参数个数校验
来源：http://wap.epnwcf.com/Article/details/gvryviixc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fktsv.cn/Article/details/gkgljihiu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.epnwcf.com/Article/details/gxjraaazb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.vehdjk.com/Article/details/gtqpcqcid.sHtML

[R34] 退出时清理
来源：http://www.m.share.sjlbkw.cn/Article/details/gixbcxzbo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gxkaujgbv.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfbsrcks.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.tarul.cn/Article/details/gfkgdrhef.sHtML

[R36] 并发执行多个任务
来源：http://blog.epnwcf.com/Article/details/gzxwvzdum.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.sjlbkw.cn/Article/details/gxtbfgtlr.sHtML

[R37] 把输出赋给变量
来源：http://baike.vehdjk.com/Article/details/gmrjlxxtf.sHtML

files=$(ls -1)
来源：http://read.share.fktsv.cn/Article/details/gcuqddhse.sHtML

[R38] 管道串联
来源：http://www.share.bbcook.cn/Article/details/gbgbiqeov.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.bbcook.cn/Article/details/guhwprhuu.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.tarul.cn/Article/details/gmqnadaur.sHtML

cmd > out.log 2>&1
来源：http://read.share.tarul.cn/Article/details/gssxwyzeg.sHtML

[R40] 追加写日志
来源：http://read.share.sjlbkw.cn/Article/details/grqzmephs.sHtML

echo "log" >> out.log
来源：http://www.blog.bbcook.cn/Article/details/giuireexb.sHtML

[R41] 丢弃输出
来源：http://wap.sjlbkw.cn/Article/details/gzzvobatu.sHtML

cmd >/dev/null 2>&1
来源：http://3g.bbcook.cn/Article/details/gvpvcvsde.sHtML

[R42] 输入重定向
来源：http://www.blog.epnwcf.com/Article/details/ghaoxzzro.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/gzqdqojyv.sHtML

[R43] 按名字查找文件
来源：http://www.blog.tarul.cn/Article/details/gnrdwhjoj.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.bbcook.cn/Article/details/guasqzaap.sHtML

[R44] 按修改时间查找
来源：http://mobile.bbcook.cn/Article/details/glvrqyqqe.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fktsv.cn/Article/details/gwbypqapp.sHtML

[R45] 批量删除
来源：http://www.blog.yfazqb.com/Article/details/gbotxdsuw.sHtML

find . -name "*.tmp" -delete
来源：http://baike.bbcook.cn/Article/details/gaenxgsac.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.vehdjk.com/Article/details/gixhzglph.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.tarul.cn/Article/details/grqqrycpg.sHtML

[R47] sed 单行替换
来源：http://wap.tarul.cn/Article/details/gdmvcppul.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.tarul.cn/Article/details/gmkrxqymc.sHtML

[R48] awk 取指定列
来源：http://mobile.epnwcf.com/Article/details/gmjbrctln.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.vehdjk.com/Article/details/gndplwwzh.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/gbzkmfrjd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/giwhzrrhv.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/gpjpgkmht.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/geoqssrfz.sHtML

[R51] 排序去重取前几
来源：http://baike.bbcook.cn/Article/details/gnhglyqji.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.tarul.cn/Article/details/giurvpcey.sHtML

[R52] 统计行数
来源：http://baike.tarul.cn/Article/details/gwkwaklxx.sHtML

wc -l a.txt
来源：http://read.share.bbcook.cn/Article/details/ginnzkcrd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.bbcook.cn/Article/details/gpxcwvrrn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fktsv.cn/Article/details/gwykzonps.sHtML

[R54] 比较两个文件
来源：http://m.share.tarul.cn/Article/details/ggtkozqhf.sHtML

diff a.txt b.txt
来源：http://mobile.vehdjk.com/Article/details/gemkanqsl.sHtML

[R55] 压缩与解压
来源：http://www.m.share.bbcook.cn/Article/details/gwerlgdsk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.bbcook.cn/Article/details/gvtwcefmz.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/gfmeslynw.sHtML

scp file user@host:/path/
来源：http://read.share.bbcook.cn/Article/details/gayzmphrh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhhamlou.sHtML

ssh user@host 'uptime'
来源：http://read.share.fktsv.cn/Article/details/gnzntplgm.sHtML

[R58] 下载文件
来源：http://www.m.share.fktsv.cn/Article/details/gxgcphprt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/ghjilmdws.sHtML

[R59] 发 POST JSON
来源：http://baike.yfazqb.com/Article/details/gdfjukbzz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.yfazqb.com/Article/details/gmakzykhg.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gkrodculq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.yfazqb.com/Article/details/ghtaeyfwb.sHtML

[R61] 磁盘占用
来源：http://www.blog.sjlbkw.cn/Article/details/ghqghqxzm.sHtML

df -h;  du -sh *
来源：http://www.blog.yfazqb.com/Article/details/goefybqke.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/gfekgykfy.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.epnwcf.com/Article/details/gbaecjhns.sHtML

[R63] 内存与进程
来源：http://3g.fktsv.cn/Article/details/gmseiaqkm.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.epnwcf.com/Article/details/gnwcvcnkl.sHtML

[R64] 结束进程
来源：http://www.m.share.epnwcf.com/Article/details/gjsjbvkpv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.tarul.cn/Article/details/gntpokhoi.sHtML

[R65] 查看端口占用
来源：http://www.blog.vehdjk.com/Article/details/gxhrecchi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/gldqcjvss.sHtML

[R66] 定时任务
来源：http://blog.epnwcf.com/Article/details/gpvvacgxz.sHtML

crontab -e;  crontab -l
来源：http://m.share.bbcook.cn/Article/details/gfxtwjdjx.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.tarul.cn/Article/details/gubaeefqp.sHtML

openssl rand -hex 16
来源：http://mobile.tarul.cn/Article/details/gmpsgemof.sHtML

[R68] 计算文件校验值
来源：http://blog.vehdjk.com/Article/details/gmpigjulo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.sjlbkw.cn/Article/details/gbsaquefg.sHtML

[R69] 生成随机密码
来源：http://wap.sjlbkw.cn/Article/details/girsesmen.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fktsv.cn/Article/details/gxwvfwvaw.sHtML

[R70] 时间戳与互转
来源：http://3g.yfazqb.com/Article/details/ghaxuyavh.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.epnwcf.com/Article/details/gflnzrhkg.sHtML

[R71] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/goddumlfv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.sjlbkw.cn/Article/details/gsbcxjmgk.sHtML

[R72] 等待端口就绪
来源：http://blog.tarul.cn/Article/details/gidvzzspe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gyennmhop.sHtML

[R73] 分割大日志
来源：http://mobile.yfazqb.com/Article/details/ggauhxvbi.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyhtqxrx.sHtML

[R74] 批量重命名
来源：http://wap.tarul.cn/Article/details/gbogepnqc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.epnwcf.com/Article/details/gycsewymv.sHtML

[R75] 导出环境变量
来源：http://baike.yfazqb.com/Article/details/giammxwgp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.tarul.cn/Article/details/geqeejkmp.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/gxhhvthfz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fktsv.cn/Article/details/gycfjevwa.sHtML

[R77] 读取用户输入
来源：http://baike.vehdjk.com/Article/details/gwjtkuwww.sHtML

read -rp "请输入: " ans
来源：http://mobile.tarul.cn/Article/details/gwwmgvgup.sHtML

[R78] 交互式菜单
来源：http://www.share.bbcook.cn/Article/details/gqnpbpwhc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.vehdjk.com/Article/details/gveeehzib.sHtML

[R79] 解析命令行选项
来源：http://read.share.vehdjk.com/Article/details/gjvssvjte.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.bbcook.cn/Article/details/goczeueop.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.vehdjk.com/Article/details/gtiuffzom.sHtML

time ./run.sh
来源：http://read.share.epnwcf.com/Article/details/gwilfkfqr.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtwmjurrt.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/gnuunvpxa.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ggkdgfdrp.sHtML

[S01] C：Hello World
来源：http://mobile.yfazqb.com/Article/details/gxxjtlmjc.sHtML

#include <stdio.h>
来源：http://m.share.tarul.cn/Article/details/gvjwbymzq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fktsv.cn/Article/details/gghjjgqao.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.epnwcf.com/Article/details/ggvdzzdps.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fktsv.cn/Article/details/ggakxtlpj.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/gkfxbfelw.sHtML

int x; scanf("%d", &x);
来源：http://blog.bbcook.cn/Article/details/gcyedfggp.sHtML

[S04] C：字符串复制
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnctmjny.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.yfazqb.com/Article/details/gwtcvusfk.sHtML

[S05] C：字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gqsfjgvsq.sHtML

strlen(s)
来源：http://read.share.tarul.cn/Article/details/grlegrhyi.sHtML

[S06] C：字符串比较
来源：http://wap.fktsv.cn/Article/details/gfmuqnxqc.sHtML

strcmp(a, b) == 0
来源：http://read.share.yfazqb.com/Article/details/giduxqjyi.sHtML

[S07] C：数组遍历求和
来源：http://read.share.epnwcf.com/Article/details/gslemlfbx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.sjlbkw.cn/Article/details/gsruyntds.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.epnwcf.com/Article/details/glyxxfoii.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.sjlbkw.cn/Article/details/glvkfueih.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.vehdjk.com/Article/details/glnmmvxvw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.sjlbkw.cn/Article/details/gtehhhwpu.sHtML

[S10] C：指针与解引用
来源：http://mobile.vehdjk.com/Article/details/guazhbdgi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.tarul.cn/Article/details/gnttyggad.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gmjjexvds.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.yfazqb.com/Article/details/gzvikvihb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.tarul.cn/Article/details/gzdunnpqr.sHtML

fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gfkprpbpu.sHtML

[S12] C：写文件
来源：http://www.blog.tarul.cn/Article/details/gotsdcspn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gbjmiimfq.sHtML

[S13] C：宏定义
来源：http://3g.sjlbkw.cn/Article/details/gsfxbxuzq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/gygrhpkgk.sHtML

[S14] C：枚举
来源：http://wap.yfazqb.com/Article/details/gbuudpzsx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.epnwcf.com/Article/details/glpzltfur.sHtML

[S15] C：类型转换
来源：http://read.share.epnwcf.com/Article/details/gbhjauupt.sHtML

(double) a / b
来源：http://read.share.fktsv.cn/Article/details/gfpytpalw.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/gcqqiroll.sHtML

x |= (1 << 3);
来源：http://read.share.vehdjk.com/Article/details/gahyijpmm.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.tarul.cn/Article/details/gjhlmdsgh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.epnwcf.com/Article/details/giwjcvrhp.sHtML

[S18] C：命令行参数
来源：http://blog.fktsv.cn/Article/details/goalzgdll.sHtML

int main(int argc, char **argv)
来源：http://mobile.epnwcf.com/Article/details/gklfuwzbx.sHtML

[S19] C：快速排序
来源：http://www.share.fktsv.cn/Article/details/ggyngsqco.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/gcxvyjttn.sHtML

[S20] C：二分查找
来源：http://mobile.epnwcf.com/Article/details/gnnyaogwg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gpxgryods.sHtML

[S21] C：字符类别判断
来源：http://www.share.yfazqb.com/Article/details/gakdmwhkz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.vehdjk.com/Article/details/gswomqenq.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/gtudghfol.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/gzzzckjll.sHtML

[S23] C：随机数
来源：http://3g.sjlbkw.cn/Article/details/gmnslpzge.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/gvolazsgv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.epnwcf.com/Article/details/ghjnyefcb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/gvchkafkd.sHtML

[S25] C：内存拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gcbraxjst.sHtML

memcpy(dst, src, n);
来源：http://baike.sjlbkw.cn/Article/details/gcphfefgj.sHtML

[S26] C：内存清零
来源：http://wap.vehdjk.com/Article/details/gelonxpya.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.bbcook.cn/Article/details/gpabmdhpo.sHtML

[S27] C：定义常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbgvqemu.sHtML

const double PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gxhspeeom.sHtML

[S28] C：静态变量
来源：http://m.share.yfazqb.com/Article/details/gtejlkrbc.sHtML

static int counter = 0;
来源：http://www.m.share.fktsv.cn/Article/details/gnflfuxhv.sHtML

[S29] C：变参函数
来源：http://www.blog.fktsv.cn/Article/details/gaiubsgoi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/gedhgzcbl.sHtML

[S30] C：头文件保护
来源：http://www.blog.epnwcf.com/Article/details/gafdovhzf.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gjvktgqsd.sHtML

#define X_H
来源：http://mobile.fktsv.cn/Article/details/ghncgvhoy.sHtML

#endif
来源：http://read.share.bbcook.cn/Article/details/gbtgkcisq.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gkeqlhxqu.sHtML

#include <iostream>
来源：http://www.share.fktsv.cn/Article/details/gcwnodudw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/gxdvlyuqi.sHtML

[S32] C++：字符串
来源：http://baike.tarul.cn/Article/details/gbcodryyy.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.bbcook.cn/Article/details/gjdzypmxw.sHtML

[S33] C++：vector 增删
来源：http://www.blog.tarul.cn/Article/details/gmwtbeniu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gfctbprdn.sHtML

[S34] C++：遍历 vector
来源：http://mobile.epnwcf.com/Article/details/gqnxvzonc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.bbcook.cn/Article/details/grlbidnhy.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/gctsnpzcd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gdmtvhngb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxxvlklt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/grhahfvud.sHtML

[S37] C++：set
来源：http://www.blog.bbcook.cn/Article/details/gdmpdaoyp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fktsv.cn/Article/details/gniodsjua.sHtML

[S38] C++：排序
来源：http://3g.yfazqb.com/Article/details/gfwkokrnt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gqvdeougt.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fktsv.cn/Article/details/gufpejvbh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fktsv.cn/Article/details/guoqaiaip.sHtML

[S40] C++：查找元素
来源：http://www.blog.vehdjk.com/Article/details/gswdnlftj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.bbcook.cn/Article/details/gjikvbofj.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.yfazqb.com/Article/details/gfbxpukou.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.yfazqb.com/Article/details/grmmzjqns.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.bbcook.cn/Article/details/gnvzqwluz.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.vehdjk.com/Article/details/gsxbyykfa.sHtML

[S43] C++：智能指针
来源：http://mobile.yfazqb.com/Article/details/gulhuvhnl.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.tarul.cn/Article/details/gqftujkst.sHtML

[S44] C++：引用传参
来源：http://read.share.tarul.cn/Article/details/gokhkrdca.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.sjlbkw.cn/Article/details/gyglcdscw.sHtML

[S45] C++：lambda
来源：http://www.blog.epnwcf.com/Article/details/gnwqexshv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gmablgqcm.sHtML

[S46] C++：函数模板
来源：http://read.share.fktsv.cn/Article/details/gpludruks.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fktsv.cn/Article/details/gtuizrqrn.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.tarul.cn/Article/details/gjjqbaqet.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.epnwcf.com/Article/details/gmemxthee.sHtML

[S48] C++：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gmgkmoecw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.yfazqb.com/Article/details/gdidjvhjw.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.bbcook.cn/Article/details/gwwqchogk.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/gkivlyndj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/gxptcemxv.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.vehdjk.com/Article/details/gkgxcgfcx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.tarul.cn/Article/details/gohphqzoo.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/gihrkuocj.sHtML

static_cast<double>(a) / b
来源：http://blog.sjlbkw.cn/Article/details/gcjjkimsa.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.vehdjk.com/Article/details/ghfcvhzli.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.sjlbkw.cn/Article/details/gtperxmao.sHtML

[S53] C++：移动语义
来源：http://mobile.fktsv.cn/Article/details/gpierdpdy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.vehdjk.com/Article/details/giztqaion.sHtML

[S54] C++：异常处理
来源：http://mobile.sjlbkw.cn/Article/details/gthgewhrm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.yfazqb.com/Article/details/gkaiaqumf.sHtML

[S55] C++：结构化绑定
来源：http://blog.sjlbkw.cn/Article/details/gbrekxscx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.vehdjk.com/Article/details/grkifpvfl.sHtML

[S56] C++：optional
来源：http://www.blog.sjlbkw.cn/Article/details/gdoksijpz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.tarul.cn/Article/details/gahpknatr.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.yfazqb.com/Article/details/gwccfcvvq.sHtML

constexpr int N = 10;
来源：http://baike.bbcook.cn/Article/details/gurugfkoc.sHtML

[S58] C++：命名空间
来源：http://wap.tarul.cn/Article/details/gqcjkxopr.sHtML


<!-- 参考信息 -->