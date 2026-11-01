代发 wailian999

[Q82] 字符长度与字节长度
来源：http://read.share.epnwcf.com/Article/details/gyaljjqzf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gtrvlosvi.sHtML

[Q83] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gjigqdayq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/guicbkvca.sHtML

[Q84] 去除首尾空格
来源：http://wap.vehdjk.com/Article/details/gklckfmbv.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gzmorvypm.sHtML

[Q85] 数值取整
来源：http://m.share.epnwcf.com/Article/details/glaqpjfln.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.yfazqb.com/Article/details/ghdegyhpg.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.vehdjk.com/Article/details/givrohhil.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.epnwcf.com/Article/details/ghxetognu.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.sjlbkw.cn/Article/details/gxnbwrskm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.vehdjk.com/Article/details/gxxgbvrsd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.sjlbkw.cn/Article/details/glqlzvkzz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.yfazqb.com/Article/details/gzmretqmv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gdojvxueb.sHtML

[Q89] 判断表是否存在
来源：http://wap.tarul.cn/Article/details/gtloowwrw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.vehdjk.com/Article/details/gigrwzaly.sHtML

[Q90] 生成序号列
来源：http://wap.tarul.cn/Article/details/gopwughpc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fktsv.cn/Article/details/gtkmykxrc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdffsvwyc.sHtML

R. Bash 专题
来源：http://mobile.sjlbkw.cn/Article/details/gmrtcclig.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsrfegvcl.sHtML

[R01] shebang 与严格模式
来源：http://3g.yfazqb.com/Article/details/goywfgswv.sHtML

#!/usr/bin/env bash
来源：http://3g.sjlbkw.cn/Article/details/gxzvkrdca.sHtML

set -euo pipefail
来源：http://www.share.epnwcf.com/Article/details/glroohoxm.sHtML

[R02] 变量赋值与使用
来源：http://blog.tarul.cn/Article/details/gfoxrxham.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.bbcook.cn/Article/details/gvukstkot.sHtML

[R03] 只读变量
来源：http://read.share.epnwcf.com/Article/details/gtpfxnkbt.sHtML

readonly PI=3.14
来源：http://www.share.vehdjk.com/Article/details/gbmuxpfqb.sHtML

[R04] 位置参数
来源：http://wap.yfazqb.com/Article/details/gzlpkusux.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/grkejszwo.sHtML

[R05] 参数默认值
来源：http://www.blog.fktsv.cn/Article/details/gpqyxynyz.sHtML

name="${1:-default}"
来源：http://www.m.share.tarul.cn/Article/details/grradcncs.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gwwliqqwc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gkxnxjwjm.sHtML

[R07] if 判断文件
来源：http://www.blog.bbcook.cn/Article/details/garkrcpcq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.tarul.cn/Article/details/gmliriohe.sHtML

[R08] 数值比较
来源：http://www.m.share.epnwcf.com/Article/details/gcpqxyitv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.yfazqb.com/Article/details/gbbkhdlsr.sHtML

[R09] 字符串比较
来源：http://www.share.yfazqb.com/Article/details/glirlxawr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.yfazqb.com/Article/details/gxcfbdvan.sHtML

[R10] 正则匹配
来源：http://baike.epnwcf.com/Article/details/gicppaihp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.epnwcf.com/Article/details/gechonofn.sHtML

[R11] case 多分支
来源：http://mobile.tarul.cn/Article/details/gaszlbxhr.sHtML

case "$1" in
来源：http://read.share.sjlbkw.cn/Article/details/gfubhsiuc.sHtML

start) echo "启动" ;;
来源：http://wap.bbcook.cn/Article/details/geypyvslq.sHtML

stop)  echo "停止" ;;
来源：http://www.share.yfazqb.com/Article/details/gpziztjws.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.yfazqb.com/Article/details/gikbodezw.sHtML

esac
来源：http://www.m.share.vehdjk.com/Article/details/gritaiyyx.sHtML

[R12] for 遍历文件
来源：http://read.share.sjlbkw.cn/Article/details/gxaxizgps.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.vehdjk.com/Article/details/gjgrpnggv.sHtML

[R13] for 计数循环
来源：http://blog.epnwcf.com/Article/details/gxtuekzvm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gkclzunwm.sHtML

[R14] C 风格 for
来源：http://3g.epnwcf.com/Article/details/gjegrzofq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/gtrudrclu.sHtML

[R15] while 逐行读文件
来源：http://3g.epnwcf.com/Article/details/gbwgabwbz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.sjlbkw.cn/Article/details/gahwvjwza.sHtML

[R16] until 等待条件
来源：http://read.share.sjlbkw.cn/Article/details/gqvorwiwh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gdhkqxvtj.sHtML

[R17] 数组定义与取值
来源：http://www.blog.epnwcf.com/Article/details/gldacdwnk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.epnwcf.com/Article/details/gtphyypoq.sHtML

[R18] 遍历数组
来源：http://m.share.vehdjk.com/Article/details/gzvsneapp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.bbcook.cn/Article/details/ggigdieng.sHtML

[R19] 数组长度
来源：http://wap.bbcook.cn/Article/details/gtrxuwcjv.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/gjoxhhkdg.sHtML

[R20] 关联数组（字典）
来源：http://blog.tarul.cn/Article/details/gyywvfpiz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.bbcook.cn/Article/details/gpwgnpned.sHtML

[R21] 字符串长度
来源：http://baike.vehdjk.com/Article/details/gtmyrtzzk.sHtML

echo "${#s}"
来源：http://m.share.yfazqb.com/Article/details/gztugjbmi.sHtML

[R22] 截取子串
来源：http://www.share.bbcook.cn/Article/details/gqohoayar.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/gsswhuuoi.sHtML

[R23] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/ghmccmexs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.epnwcf.com/Article/details/ghwiuwsrp.sHtML

[R24] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gfyathsgj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.epnwcf.com/Article/details/gygqehaqj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fktsv.cn/Article/details/gsubocwyu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.bbcook.cn/Article/details/gojbihyii.sHtML

[R26] 命令替换
来源：http://www.share.tarul.cn/Article/details/gkiwcqzxa.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.vehdjk.com/Article/details/gkhqyxcep.sHtML

[R27] 算术展开
来源：http://baike.fktsv.cn/Article/details/gxdgrtrjx.sHtML

echo $((1 + 2 * 3))
来源：http://3g.epnwcf.com/Article/details/gqvcrjycg.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/gohrjyfer.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.epnwcf.com/Article/details/gevhsborc.sHtML

[R29] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gfdzeerqt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fktsv.cn/Article/details/goutyfjli.sHtML

[R30] 函数返回状态码
来源：http://m.share.vehdjk.com/Article/details/gxrbymifh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.tarul.cn/Article/details/gmrfujrmc.sHtML

[R31] 局部变量
来源：http://www.blog.vehdjk.com/Article/details/gyoaledus.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.bbcook.cn/Article/details/giatarqea.sHtML

[R32] 参数个数校验
来源：http://read.share.tarul.cn/Article/details/gqhrmxcvi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fktsv.cn/Article/details/gjcxgtdzl.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.vehdjk.com/Article/details/gendrliim.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.tarul.cn/Article/details/gbktnpyoq.sHtML

[R34] 退出时清理
来源：http://baike.bbcook.cn/Article/details/gbcdgxvqx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gtispnytf.sHtML

[R35] 后台执行并等待
来源：http://wap.tarul.cn/Article/details/glfmcfsmz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.yfazqb.com/Article/details/ghybwlwgk.sHtML

[R36] 并发执行多个任务
来源：http://read.share.bbcook.cn/Article/details/gcizlwlwp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/gqoitthtk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.epnwcf.com/Article/details/goswbxdjh.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/gqncxlikk.sHtML

[R38] 管道串联
来源：http://blog.fktsv.cn/Article/details/gvttahwjk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.yfazqb.com/Article/details/gbwowdqlu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fktsv.cn/Article/details/gxgxuydrp.sHtML

cmd > out.log 2>&1
来源：http://www.blog.bbcook.cn/Article/details/gbdcbhcem.sHtML

[R40] 追加写日志
来源：http://m.share.tarul.cn/Article/details/gxxarecsu.sHtML

echo "log" >> out.log
来源：http://3g.tarul.cn/Article/details/gdhhubpyw.sHtML

[R41] 丢弃输出
来源：http://m.share.fktsv.cn/Article/details/gwfmsbazb.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fktsv.cn/Article/details/gjxhevkyc.sHtML

[R42] 输入重定向
来源：http://baike.yfazqb.com/Article/details/grfnahlrd.sHtML

wc -l < a.txt
来源：http://m.share.bbcook.cn/Article/details/glewaczqa.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/guzcvnond.sHtML

find . -name "*.log" -type f
来源：http://3g.bbcook.cn/Article/details/gofbesxka.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/geevjbquw.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/gqlnocfoe.sHtML

[R45] 批量删除
来源：http://blog.tarul.cn/Article/details/gqsotxqwd.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.vehdjk.com/Article/details/gujlrjono.sHtML

[R46] 递归替换文件内容
来源：http://3g.yfazqb.com/Article/details/gyyymjjmu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.vehdjk.com/Article/details/ghhlgayca.sHtML

[R47] sed 单行替换
来源：http://www.blog.epnwcf.com/Article/details/gsdhgpwpr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/ghogybjwu.sHtML

[R48] awk 取指定列
来源：http://read.share.epnwcf.com/Article/details/gqsklqyle.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.yfazqb.com/Article/details/gywztnqlk.sHtML

[R49] awk 带条件
来源：http://mobile.fktsv.cn/Article/details/gsspnpmbv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fktsv.cn/Article/details/gnxieyjqf.sHtML

[R50] awk 求和
来源：http://baike.tarul.cn/Article/details/ggsufhhug.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.bbcook.cn/Article/details/ggmyvjhfb.sHtML

[R51] 排序去重取前几
来源：http://blog.tarul.cn/Article/details/gtelsihpm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fktsv.cn/Article/details/gyyfyghin.sHtML

[R52] 统计行数
来源：http://www.blog.sjlbkw.cn/Article/details/glclxhkiw.sHtML

wc -l a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gzchwluur.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.yfazqb.com/Article/details/goedquumv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.vehdjk.com/Article/details/ggjqyzccz.sHtML

[R54] 比较两个文件
来源：http://www.m.share.vehdjk.com/Article/details/gjhcankpw.sHtML

diff a.txt b.txt
来源：http://www.blog.tarul.cn/Article/details/gghrbalrj.sHtML

[R55] 压缩与解压
来源：http://blog.sjlbkw.cn/Article/details/gfjqmyspa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.sjlbkw.cn/Article/details/gonvqspmk.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/gutwtvxcm.sHtML

scp file user@host:/path/
来源：http://m.share.yfazqb.com/Article/details/gzcsmoxyf.sHtML

[R57] 远程执行命令
来源：http://3g.yfazqb.com/Article/details/gxgtinqdx.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.yfazqb.com/Article/details/guofxiiby.sHtML

[R58] 下载文件
来源：http://blog.tarul.cn/Article/details/gxlcniuyh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/ggiakbaes.sHtML

[R59] 发 POST JSON
来源：http://baike.tarul.cn/Article/details/gjorpyrrs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.sjlbkw.cn/Article/details/gmmbahbdk.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/gvyevhtci.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.bbcook.cn/Article/details/gibwtsobk.sHtML

[R61] 磁盘占用
来源：http://blog.yfazqb.com/Article/details/gaqfzpsnv.sHtML

df -h;  du -sh *
来源：http://www.blog.sjlbkw.cn/Article/details/gunqyfmff.sHtML

[R62] 找最占空间的文件
来源：http://blog.bbcook.cn/Article/details/gnrfvokbi.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.bbcook.cn/Article/details/geaijotgd.sHtML

[R63] 内存与进程
来源：http://www.blog.sjlbkw.cn/Article/details/gffoirpcv.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.vehdjk.com/Article/details/gxvevxoue.sHtML

[R64] 结束进程
来源：http://blog.fktsv.cn/Article/details/gwulxqrvt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.yfazqb.com/Article/details/ggyglyrlr.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/gnhpoutpl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.yfazqb.com/Article/details/geuhtgpdj.sHtML

[R66] 定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/gcyqyrkhe.sHtML

crontab -e;  crontab -l
来源：http://3g.fktsv.cn/Article/details/gwvwgutdr.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.bbcook.cn/Article/details/gjgrwapnf.sHtML

openssl rand -hex 16
来源：http://wap.yfazqb.com/Article/details/gwqdopzeg.sHtML

[R68] 计算文件校验值
来源：http://read.share.yfazqb.com/Article/details/gqnjgkdln.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.yfazqb.com/Article/details/grzfzuukq.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/gmcuekozl.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.yfazqb.com/Article/details/gwvirzwye.sHtML

[R70] 时间戳与互转
来源：http://3g.sjlbkw.cn/Article/details/gvqzdmgww.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.epnwcf.com/Article/details/grcohvrmf.sHtML

[R71] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gsemlzvzw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.sjlbkw.cn/Article/details/gfpyrjrvt.sHtML

[R72] 等待端口就绪
来源：http://m.share.yfazqb.com/Article/details/gcwmmnrgy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gczyukylj.sHtML

[R73] 分割大日志
来源：http://www.blog.vehdjk.com/Article/details/gllpoxngx.sHtML

split -l 1000 big.log part_
来源：http://wap.tarul.cn/Article/details/ggxpowvcg.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/ghkmgggth.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fktsv.cn/Article/details/gpcuqixma.sHtML

[R75] 导出环境变量
来源：http://www.m.share.tarul.cn/Article/details/gynvddibm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/gznjxfhlp.sHtML

[R76] 使用临时文件
来源：http://read.share.sjlbkw.cn/Article/details/ghlmwczwk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gtixkqdvr.sHtML

[R77] 读取用户输入
来源：http://baike.vehdjk.com/Article/details/gecgucexb.sHtML

read -rp "请输入: " ans
来源：http://mobile.bbcook.cn/Article/details/goigfwzzi.sHtML

[R78] 交互式菜单
来源：http://blog.sjlbkw.cn/Article/details/gcqpkqxbp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.sjlbkw.cn/Article/details/groxcfheu.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/gcdnzugug.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.sjlbkw.cn/Article/details/gepaibspo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.yfazqb.com/Article/details/gaojdbhsw.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/glbhsucsb.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfyyyqule.sHtML

S. C / C++ 专题
来源：http://blog.tarul.cn/Article/details/gkhhvimid.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gmgmptlaw.sHtML

[S01] C：Hello World
来源：http://m.share.epnwcf.com/Article/details/gesgestba.sHtML

#include <stdio.h>
来源：http://www.share.epnwcf.com/Article/details/gormqwddy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.sjlbkw.cn/Article/details/gyuvwubwp.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.sjlbkw.cn/Article/details/gglfcgzsj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.vehdjk.com/Article/details/ghuqfslpa.sHtML

[S03] C：读入整数
来源：http://www.blog.yfazqb.com/Article/details/gkgytnwjb.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/gubtqhiak.sHtML

[S04] C：字符串复制
来源：http://3g.sjlbkw.cn/Article/details/gjkkvimdz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.epnwcf.com/Article/details/girsrcijq.sHtML

[S05] C：字符串长度
来源：http://baike.yfazqb.com/Article/details/gcqbwaevq.sHtML

strlen(s)
来源：http://m.share.vehdjk.com/Article/details/gprlqelud.sHtML

[S06] C：字符串比较
来源：http://baike.tarul.cn/Article/details/ghybondit.sHtML

strcmp(a, b) == 0
来源：http://read.share.sjlbkw.cn/Article/details/gecngrktv.sHtML

[S07] C：数组遍历求和
来源：http://baike.bbcook.cn/Article/details/gpeckgxge.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/geswhdbeb.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.bbcook.cn/Article/details/gonzgatpl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fktsv.cn/Article/details/gcqootytn.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.yfazqb.com/Article/details/ghcopykpj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.tarul.cn/Article/details/gmakeeauy.sHtML

[S10] C：指针与解引用
来源：http://mobile.tarul.cn/Article/details/gbssmucdv.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.bbcook.cn/Article/details/gkfnaaqwt.sHtML

[S11] C：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gokrweqau.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.sjlbkw.cn/Article/details/gxgblkyxt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.yfazqb.com/Article/details/gymzkanrr.sHtML

fclose(f);
来源：http://blog.tarul.cn/Article/details/grjnntzeq.sHtML

[S12] C：写文件
来源：http://baike.fktsv.cn/Article/details/gnsdufvjb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gomfeilax.sHtML

[S13] C：宏定义
来源：http://www.m.share.tarul.cn/Article/details/gntkyiyuk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fktsv.cn/Article/details/gjkofsgtj.sHtML

[S14] C：枚举
来源：http://blog.tarul.cn/Article/details/gbbbmrfyx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.epnwcf.com/Article/details/gmbvjymdf.sHtML

[S15] C：类型转换
来源：http://m.share.epnwcf.com/Article/details/giogpyklp.sHtML

(double) a / b
来源：http://www.blog.bbcook.cn/Article/details/galiynruw.sHtML

[S16] C：位操作置位
来源：http://baike.bbcook.cn/Article/details/gnofjcumb.sHtML

x |= (1 << 3);
来源：http://3g.yfazqb.com/Article/details/ghofgeufp.sHtML

[S17] C：安全拼接字符串
来源：http://wap.tarul.cn/Article/details/ggcwddnty.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.vehdjk.com/Article/details/gwqqsvacj.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gnfqmalrt.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.sjlbkw.cn/Article/details/grgukdjyb.sHtML

[S19] C：快速排序
来源：http://www.blog.bbcook.cn/Article/details/gmnqpbfoq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gyjxdjdbv.sHtML

[S20] C：二分查找
来源：http://baike.fktsv.cn/Article/details/gbcspoupd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gwyomqtmh.sHtML

[S21] C：字符类别判断
来源：http://baike.bbcook.cn/Article/details/gpwijckck.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.yfazqb.com/Article/details/gwpptntix.sHtML

[S22] C：字符串转数字
来源：http://mobile.vehdjk.com/Article/details/gzzfbhuga.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/gdxolsgjg.sHtML

[S23] C：随机数
来源：http://wap.tarul.cn/Article/details/gheknjaql.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.vehdjk.com/Article/details/gegliqofw.sHtML

[S24] C：获取本地时间
来源：http://read.share.sjlbkw.cn/Article/details/gflllsajh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.sjlbkw.cn/Article/details/geasolimo.sHtML

[S25] C：内存拷贝
来源：http://read.share.fktsv.cn/Article/details/gatklcycf.sHtML

memcpy(dst, src, n);
来源：http://www.blog.tarul.cn/Article/details/gqcdaundb.sHtML

[S26] C：内存清零
来源：http://baike.bbcook.cn/Article/details/gqfaqlgsx.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/gwstfqjms.sHtML

[S27] C：定义常量
来源：http://read.share.tarul.cn/Article/details/gkxpqfurr.sHtML

const double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gffxptotr.sHtML

[S28] C：静态变量
来源：http://3g.fktsv.cn/Article/details/geoivsgzg.sHtML

static int counter = 0;
来源：http://m.share.sjlbkw.cn/Article/details/gimukfmlk.sHtML

[S29] C：变参函数
来源：http://m.share.bbcook.cn/Article/details/grexilmgh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.bbcook.cn/Article/details/gmrihfiwf.sHtML

[S30] C：头文件保护
来源：http://blog.fktsv.cn/Article/details/gjfahkfgu.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/gbwyvnera.sHtML

#define X_H
来源：http://mobile.vehdjk.com/Article/details/ggkvhqhpu.sHtML

#endif
来源：http://www.share.yfazqb.com/Article/details/gwfnaorrw.sHtML

[S31] C++：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gaehlhwcd.sHtML

#include <iostream>
来源：http://m.share.tarul.cn/Article/details/grtshmdtu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.tarul.cn/Article/details/gsixonaix.sHtML

[S32] C++：字符串
来源：http://wap.bbcook.cn/Article/details/gnnzpasuf.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.tarul.cn/Article/details/gkibhqwni.sHtML

[S33] C++：vector 增删
来源：http://mobile.vehdjk.com/Article/details/ggqquukwd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.vehdjk.com/Article/details/gdnspchhe.sHtML

[S34] C++：遍历 vector
来源：http://baike.sjlbkw.cn/Article/details/giqduftjp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.tarul.cn/Article/details/ghavnvlqw.sHtML

[S35] C++：map
来源：http://www.m.share.fktsv.cn/Article/details/gsmuhetqa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/ghfrsfxwv.sHtML

[S36] C++：unordered_map
来源：http://mobile.sjlbkw.cn/Article/details/gtedejhvi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gvidcnauq.sHtML

[S37] C++：set
来源：http://read.share.tarul.cn/Article/details/gfeszfpns.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fktsv.cn/Article/details/gbrbkzujd.sHtML

[S38] C++：排序
来源：http://3g.epnwcf.com/Article/details/gjhhhdfdv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gexaazway.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.tarul.cn/Article/details/gjygemkmm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.vehdjk.com/Article/details/gdvravhwp.sHtML

[S40] C++：查找元素
来源：http://read.share.sjlbkw.cn/Article/details/gcblvtoxk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.sjlbkw.cn/Article/details/gulvbvhji.sHtML

[S41] C++：类与构造函数
来源：http://read.share.yfazqb.com/Article/details/gnomvmepn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.sjlbkw.cn/Article/details/grclcgezp.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/gnjwmrcme.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fktsv.cn/Article/details/grnntavvf.sHtML

[S43] C++：智能指针
来源：http://www.share.sjlbkw.cn/Article/details/gnuntyrnr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/gwwtygkcf.sHtML

[S44] C++：引用传参
来源：http://m.share.bbcook.cn/Article/details/gqkloumxc.sHtML

void inc(int &x) { ++x; }
来源：http://3g.sjlbkw.cn/Article/details/gcderoxsg.sHtML

[S45] C++：lambda
来源：http://blog.vehdjk.com/Article/details/gqtxhngaq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/gmicgfbqy.sHtML

[S46] C++：函数模板
来源：http://mobile.fktsv.cn/Article/details/gabysgquo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.vehdjk.com/Article/details/giwcwanbw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.epnwcf.com/Article/details/gevtcyfav.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/gdmvqbzxw.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gfgrfliwy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fktsv.cn/Article/details/goerefkux.sHtML

while (std::getline(in, line)) { }
来源：http://baike.vehdjk.com/Article/details/gvvbgfpji.sHtML

[S49] C++：写文件
来源：http://blog.sjlbkw.cn/Article/details/gomkpyttt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.sjlbkw.cn/Article/details/gtagkegdh.sHtML

[S50] C++：格式化数字
来源：http://3g.yfazqb.com/Article/details/gidwfqdiv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.bbcook.cn/Article/details/gjgkvaavg.sHtML

[S51] C++：显式类型转换
来源：http://blog.fktsv.cn/Article/details/gitnfqknq.sHtML

static_cast<double>(a) / b
来源：http://3g.sjlbkw.cn/Article/details/gznsknrbx.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/grjjzdcki.sHtML


<!-- 参考信息 -->