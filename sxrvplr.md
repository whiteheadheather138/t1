代发 wailian999

[Q76] 按天统计
来源：http://3g.fktsv.cn/Article/details/gonhxkyfr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/gsriwcokb.sHtML

[Q77] 时间加减
来源：http://3g.tarul.cn/Article/details/gvxlfddvd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.bbcook.cn/Article/details/gcpktpdob.sHtML

[Q78] 当前时间
来源：http://m.share.tarul.cn/Article/details/ggblddfpu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/gbxmdkepg.sHtML

[Q79] 字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gwzwjznjv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.sjlbkw.cn/Article/details/gvdjigjlh.sHtML

[Q80] 字符串截取
来源：http://wap.epnwcf.com/Article/details/gloemtsoc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fktsv.cn/Article/details/ghgpvdwhc.sHtML

[Q81] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/gcjejbntw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fktsv.cn/Article/details/gdrmyupzb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.sjlbkw.cn/Article/details/gebmkwuos.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/giilukuxy.sHtML

[Q83] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gqnorautf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gwckjnclb.sHtML

[Q84] 去除首尾空格
来源：http://3g.fktsv.cn/Article/details/ggfowhdlr.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gthiezalw.sHtML

[Q85] 数值取整
来源：http://mobile.tarul.cn/Article/details/gvjoyzyzn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.epnwcf.com/Article/details/gfkdvvsjy.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.epnwcf.com/Article/details/grmsueyyt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.tarul.cn/Article/details/gpnatullu.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gbeaiehid.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fktsv.cn/Article/details/grfszdlay.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.bbcook.cn/Article/details/gepqvkpnr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.yfazqb.com/Article/details/gtyiodnsc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/ggdibasfm.sHtML

[Q89] 判断表是否存在
来源：http://baike.vehdjk.com/Article/details/grrujharh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.vehdjk.com/Article/details/gkojyedtj.sHtML

[Q90] 生成序号列
来源：http://baike.epnwcf.com/Article/details/gzsjpnfat.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.yfazqb.com/Article/details/gdgzneise.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvicnkbro.sHtML

R. Bash 专题
来源：http://wap.vehdjk.com/Article/details/gpbtgjwad.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/govapzgmt.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fktsv.cn/Article/details/gvhnofjna.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/gtndpynzn.sHtML

set -euo pipefail
来源：http://www.blog.epnwcf.com/Article/details/gppupyzpf.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/ggnzoyuhn.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.tarul.cn/Article/details/gucaexdtn.sHtML

[R03] 只读变量
来源：http://wap.sjlbkw.cn/Article/details/gdkgwdqqi.sHtML

readonly PI=3.14
来源：http://read.share.tarul.cn/Article/details/gesiuirha.sHtML

[R04] 位置参数
来源：http://www.share.tarul.cn/Article/details/gruwwibeu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.bbcook.cn/Article/details/gtabqnfzz.sHtML

[R05] 参数默认值
来源：http://mobile.tarul.cn/Article/details/gigpewjlw.sHtML

name="${1:-default}"
来源：http://3g.sjlbkw.cn/Article/details/gebjwmogh.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.yfazqb.com/Article/details/gdhjodygo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gndnxkdck.sHtML

[R07] if 判断文件
来源：http://baike.epnwcf.com/Article/details/ghulklzfy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.tarul.cn/Article/details/glfxtwvxv.sHtML

[R08] 数值比较
来源：http://baike.sjlbkw.cn/Article/details/gefctcqfm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.tarul.cn/Article/details/gcfdlstnf.sHtML

[R09] 字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/gosoyucet.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fktsv.cn/Article/details/gswsvemkz.sHtML

[R10] 正则匹配
来源：http://3g.bbcook.cn/Article/details/gwfakaamc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.bbcook.cn/Article/details/gjlxeycjw.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/gepgxnqdn.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/gjchoillg.sHtML

start) echo "启动" ;;
来源：http://3g.vehdjk.com/Article/details/guipavmcv.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gjwzzjxoz.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fktsv.cn/Article/details/gerenhypa.sHtML

esac
来源：http://wap.fktsv.cn/Article/details/gsrcfyzql.sHtML

[R12] for 遍历文件
来源：http://3g.bbcook.cn/Article/details/gpmacjzyo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.bbcook.cn/Article/details/gtojardpd.sHtML

[R13] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gnnbvuixt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/ghxyjtpgc.sHtML

[R14] C 风格 for
来源：http://www.m.share.fktsv.cn/Article/details/glueppgjj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gjyroxtvm.sHtML

[R15] while 逐行读文件
来源：http://blog.vehdjk.com/Article/details/gmfvpygow.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.tarul.cn/Article/details/gtspipjmj.sHtML

[R16] until 等待条件
来源：http://read.share.sjlbkw.cn/Article/details/gyrgchpzq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gruftqsfj.sHtML

[R17] 数组定义与取值
来源：http://www.blog.sjlbkw.cn/Article/details/galbjtblt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.epnwcf.com/Article/details/gxaobjtrb.sHtML

[R18] 遍历数组
来源：http://mobile.bbcook.cn/Article/details/gcranurww.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/gwdihfhbj.sHtML

[R19] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gtairtygg.sHtML

echo "${#arr[@]}"
来源：http://mobile.fktsv.cn/Article/details/groazphra.sHtML

[R20] 关联数组（字典）
来源：http://wap.epnwcf.com/Article/details/gioutwbld.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.tarul.cn/Article/details/gpkwichie.sHtML

[R21] 字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/grdnwhdub.sHtML

echo "${#s}"
来源：http://wap.yfazqb.com/Article/details/glnkpuxgj.sHtML

[R22] 截取子串
来源：http://3g.yfazqb.com/Article/details/gzwipbvoc.sHtML

echo "${s:0:5}"
来源：http://blog.sjlbkw.cn/Article/details/guohavjwn.sHtML

[R23] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/ghzcmotll.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.sjlbkw.cn/Article/details/gbnsdkzoy.sHtML

[R24] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gdezftxns.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fktsv.cn/Article/details/gsxeosnyc.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fktsv.cn/Article/details/gcvtiqcod.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.vehdjk.com/Article/details/gvnsohhsi.sHtML

[R26] 命令替换
来源：http://baike.fktsv.cn/Article/details/garkpynky.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.tarul.cn/Article/details/gnmxkewvi.sHtML

[R27] 算术展开
来源：http://mobile.fktsv.cn/Article/details/giuhtdicp.sHtML

echo $((1 + 2 * 3))
来源：http://baike.tarul.cn/Article/details/gymcvsdfj.sHtML

[R28] 浮点运算
来源：http://blog.fktsv.cn/Article/details/gcnmapqws.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/gdeviunnq.sHtML

[R29] 定义函数
来源：http://wap.bbcook.cn/Article/details/gvkamcaxi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.sjlbkw.cn/Article/details/glnrvvghc.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gjgjzmdlp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.tarul.cn/Article/details/gloaizont.sHtML

[R31] 局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gbkvlqsyp.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.epnwcf.com/Article/details/gbfavhcgr.sHtML

[R32] 参数个数校验
来源：http://3g.bbcook.cn/Article/details/gtnetshyx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gmovoxkow.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.vehdjk.com/Article/details/gehomfbbs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.bbcook.cn/Article/details/gwysgpqal.sHtML

[R34] 退出时清理
来源：http://mobile.bbcook.cn/Article/details/gyfhgxdyq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqzadzkr.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.yfazqb.com/Article/details/gtvzrmovb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.yfazqb.com/Article/details/ghukhvcmr.sHtML

[R36] 并发执行多个任务
来源：http://3g.tarul.cn/Article/details/gaeizhlsz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.epnwcf.com/Article/details/gcwiwadem.sHtML

[R37] 把输出赋给变量
来源：http://m.share.tarul.cn/Article/details/gpbzvrqpx.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/gumuvlrmb.sHtML

[R38] 管道串联
来源：http://mobile.vehdjk.com/Article/details/gpeewdgwt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.yfazqb.com/Article/details/glowfynqy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fktsv.cn/Article/details/grzwditjq.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/gnsyyauoo.sHtML

[R40] 追加写日志
来源：http://www.blog.bbcook.cn/Article/details/gadubneen.sHtML

echo "log" >> out.log
来源：http://mobile.vehdjk.com/Article/details/glozbamal.sHtML

[R41] 丢弃输出
来源：http://mobile.bbcook.cn/Article/details/gqmuxnloa.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.vehdjk.com/Article/details/gmazufgkm.sHtML

[R42] 输入重定向
来源：http://baike.tarul.cn/Article/details/grjrpzbkl.sHtML

wc -l < a.txt
来源：http://baike.vehdjk.com/Article/details/ghmaiolaz.sHtML

[R43] 按名字查找文件
来源：http://baike.yfazqb.com/Article/details/gxsdaakom.sHtML

find . -name "*.log" -type f
来源：http://read.share.yfazqb.com/Article/details/gioynpeex.sHtML

[R44] 按修改时间查找
来源：http://blog.epnwcf.com/Article/details/gvmuxblfi.sHtML

find . -mtime -7 -type f
来源：http://www.share.bbcook.cn/Article/details/gejpjcgdf.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/gpnqwjznj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.tarul.cn/Article/details/gwgcmsmfk.sHtML

[R46] 递归替换文件内容
来源：http://wap.sjlbkw.cn/Article/details/gogvqjiga.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.yfazqb.com/Article/details/gjuievuyw.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/gxxwseget.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.tarul.cn/Article/details/ggakgximp.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/grryuzctt.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.tarul.cn/Article/details/gcjpglnch.sHtML

[R49] awk 带条件
来源：http://wap.epnwcf.com/Article/details/gcxbpqjjb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.epnwcf.com/Article/details/gnukfqypg.sHtML

[R50] awk 求和
来源：http://read.share.epnwcf.com/Article/details/gixxpxaem.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gsxcdibxu.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/gsskvxjhm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.bbcook.cn/Article/details/ghdazfbit.sHtML

[R52] 统计行数
来源：http://www.share.epnwcf.com/Article/details/gxwarmtgc.sHtML

wc -l a.txt
来源：http://www.blog.bbcook.cn/Article/details/gdmtwavnm.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.tarul.cn/Article/details/gmqccjxpq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.vehdjk.com/Article/details/gyfidaxqi.sHtML

[R54] 比较两个文件
来源：http://www.share.yfazqb.com/Article/details/gsllzukjg.sHtML

diff a.txt b.txt
来源：http://m.share.yfazqb.com/Article/details/gqeltlyyg.sHtML

[R55] 压缩与解压
来源：http://blog.bbcook.cn/Article/details/gqpttxhci.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.tarul.cn/Article/details/gizucesxt.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/glwugljuu.sHtML

scp file user@host:/path/
来源：http://mobile.bbcook.cn/Article/details/glucnirzx.sHtML

[R57] 远程执行命令
来源：http://www.blog.vehdjk.com/Article/details/gzpvocbyz.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/gfcilwmrv.sHtML

[R58] 下载文件
来源：http://blog.fktsv.cn/Article/details/gfsfwthux.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.sjlbkw.cn/Article/details/gibkuhknr.sHtML

[R59] 发 POST JSON
来源：http://blog.epnwcf.com/Article/details/gjrdkeuye.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/giybuhhnp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/ggetwiwhm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.tarul.cn/Article/details/gskzwpquy.sHtML

[R61] 磁盘占用
来源：http://mobile.vehdjk.com/Article/details/gindouhzx.sHtML

df -h;  du -sh *
来源：http://blog.bbcook.cn/Article/details/gwwrtgcmy.sHtML

[R62] 找最占空间的文件
来源：http://3g.yfazqb.com/Article/details/gbmjaxynn.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.vehdjk.com/Article/details/grdeuvnqo.sHtML

[R63] 内存与进程
来源：http://m.share.sjlbkw.cn/Article/details/gntpxaiwz.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.tarul.cn/Article/details/gslqxdcxw.sHtML

[R64] 结束进程
来源：http://blog.fktsv.cn/Article/details/gqexaanpp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fktsv.cn/Article/details/glpdcguqq.sHtML

[R65] 查看端口占用
来源：http://m.share.tarul.cn/Article/details/gutcqtwmt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.yfazqb.com/Article/details/gsjtfzhuy.sHtML

[R66] 定时任务
来源：http://www.m.share.fktsv.cn/Article/details/gcdolpyiz.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/gqtoamanr.sHtML

[R67] 生成随机十六进制串
来源：http://3g.tarul.cn/Article/details/gzkmixhoh.sHtML

openssl rand -hex 16
来源：http://www.share.sjlbkw.cn/Article/details/gosyryqug.sHtML

[R68] 计算文件校验值
来源：http://baike.bbcook.cn/Article/details/guwrhybex.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.bbcook.cn/Article/details/gvhuqyeju.sHtML

[R69] 生成随机密码
来源：http://wap.epnwcf.com/Article/details/gtzjadqdx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fktsv.cn/Article/details/gtpgzckhf.sHtML

[R70] 时间戳与互转
来源：http://baike.sjlbkw.cn/Article/details/gmqyshszj.sHtML

date +%s;  date -d @1700000000
来源：http://wap.bbcook.cn/Article/details/gyydkzczg.sHtML

[R71] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/ggwlpdioe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.vehdjk.com/Article/details/gzixljihj.sHtML

[R72] 等待端口就绪
来源：http://baike.fktsv.cn/Article/details/gsryccqyu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gznpgvkgw.sHtML

[R73] 分割大日志
来源：http://www.share.epnwcf.com/Article/details/gqwmyafrz.sHtML

split -l 1000 big.log part_
来源：http://mobile.yfazqb.com/Article/details/glcgcbnys.sHtML

[R74] 批量重命名
来源：http://blog.fktsv.cn/Article/details/gyvaymskh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fktsv.cn/Article/details/gselwgizr.sHtML

[R75] 导出环境变量
来源：http://3g.tarul.cn/Article/details/gcxoebsmu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.tarul.cn/Article/details/gsiyddrya.sHtML

[R76] 使用临时文件
来源：http://www.blog.tarul.cn/Article/details/gpcsfqpna.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gzinzmfry.sHtML

[R77] 读取用户输入
来源：http://3g.sjlbkw.cn/Article/details/gghmduivz.sHtML

read -rp "请输入: " ans
来源：http://mobile.epnwcf.com/Article/details/gracbwpnl.sHtML

[R78] 交互式菜单
来源：http://mobile.epnwcf.com/Article/details/gxpzpjjtl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.yfazqb.com/Article/details/gaqmvfewl.sHtML

[R79] 解析命令行选项
来源：http://baike.tarul.cn/Article/details/ggmrihqqx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.vehdjk.com/Article/details/gvgrfnsbv.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.yfazqb.com/Article/details/ggnzwvhqq.sHtML

time ./run.sh
来源：http://mobile.epnwcf.com/Article/details/gtroaxkkh.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzxmwovij.sHtML

S. C / C++ 专题
来源：http://www.share.epnwcf.com/Article/details/gxoegxmli.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjlzgggnp.sHtML

[S01] C：Hello World
来源：http://blog.tarul.cn/Article/details/gxsvqynwo.sHtML

#include <stdio.h>
来源：http://blog.vehdjk.com/Article/details/gnhcvezjt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.epnwcf.com/Article/details/gzxzlzdnj.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.epnwcf.com/Article/details/gvjmtmudk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.bbcook.cn/Article/details/gizgkjjgk.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/gtfzcypvu.sHtML

int x; scanf("%d", &x);
来源：http://www.share.yfazqb.com/Article/details/glgzzvyqh.sHtML

[S04] C：字符串复制
来源：http://www.blog.bbcook.cn/Article/details/gtfjoltzm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.epnwcf.com/Article/details/grkuujsxj.sHtML

[S05] C：字符串长度
来源：http://blog.vehdjk.com/Article/details/gyvxgwckr.sHtML

strlen(s)
来源：http://wap.epnwcf.com/Article/details/gkqmpdxyn.sHtML

[S06] C：字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gavqwdjbl.sHtML

strcmp(a, b) == 0
来源：http://3g.sjlbkw.cn/Article/details/grvdctfso.sHtML

[S07] C：数组遍历求和
来源：http://wap.epnwcf.com/Article/details/gllezubam.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.yfazqb.com/Article/details/gzcsuygif.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.sjlbkw.cn/Article/details/guljnngrs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.tarul.cn/Article/details/gipzxgxlb.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.yfazqb.com/Article/details/glikxjdac.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.yfazqb.com/Article/details/gmddhzavx.sHtML

[S10] C：指针与解引用
来源：http://www.share.sjlbkw.cn/Article/details/gyyggbpvp.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/gcpfochhq.sHtML

[S11] C：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gzrjlpsbq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.bbcook.cn/Article/details/gblxvkflm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.sjlbkw.cn/Article/details/gewperyar.sHtML

fclose(f);
来源：http://wap.vehdjk.com/Article/details/gktrzhkxm.sHtML

[S12] C：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gxnlcxstn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.tarul.cn/Article/details/gyauyqsav.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/gxdrqwmtc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.tarul.cn/Article/details/gkapnftcl.sHtML

[S14] C：枚举
来源：http://blog.tarul.cn/Article/details/gzkbmmqdw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fktsv.cn/Article/details/gsigdgifk.sHtML

[S15] C：类型转换
来源：http://wap.bbcook.cn/Article/details/gcxrclsxs.sHtML

(double) a / b
来源：http://wap.epnwcf.com/Article/details/ghrszrohd.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/gcqcoxhse.sHtML

x |= (1 << 3);
来源：http://mobile.sjlbkw.cn/Article/details/gsxvqwnvf.sHtML

[S17] C：安全拼接字符串
来源：http://3g.yfazqb.com/Article/details/gmzodjdjo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.bbcook.cn/Article/details/gjshamzal.sHtML

[S18] C：命令行参数
来源：http://mobile.sjlbkw.cn/Article/details/gagzoeave.sHtML

int main(int argc, char **argv)
来源：http://www.blog.epnwcf.com/Article/details/gmrfosrot.sHtML

[S19] C：快速排序
来源：http://m.share.bbcook.cn/Article/details/gnrceipqc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gngbouqfz.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gfievnobq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gyozmxeef.sHtML

[S21] C：字符类别判断
来源：http://blog.yfazqb.com/Article/details/gctnhdynl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/gynpuaxih.sHtML

[S22] C：字符串转数字
来源：http://wap.yfazqb.com/Article/details/gycizuefe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.tarul.cn/Article/details/gqvkqlipq.sHtML

[S23] C：随机数
来源：http://wap.yfazqb.com/Article/details/gxyyuoaqf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.epnwcf.com/Article/details/galxmvasl.sHtML

[S24] C：获取本地时间
来源：http://read.share.tarul.cn/Article/details/gcevobvpv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/gxfeaovtd.sHtML

[S25] C：内存拷贝
来源：http://mobile.vehdjk.com/Article/details/gdikqmmil.sHtML

memcpy(dst, src, n);
来源：http://wap.vehdjk.com/Article/details/gralycwdd.sHtML

[S26] C：内存清零
来源：http://www.m.share.vehdjk.com/Article/details/gyrdawvoa.sHtML

memset(a, 0, sizeof a);
来源：http://3g.vehdjk.com/Article/details/gmkgyaxds.sHtML

[S27] C：定义常量
来源：http://www.blog.epnwcf.com/Article/details/gkenffmpp.sHtML

const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gzajytfbr.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/gwjlclkbx.sHtML

static int counter = 0;
来源：http://www.share.fktsv.cn/Article/details/geybwdvbm.sHtML

[S29] C：变参函数
来源：http://m.share.fktsv.cn/Article/details/gsdbudrka.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.sjlbkw.cn/Article/details/giwnokiov.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/gzcjefwge.sHtML

#ifndef X_H
来源：http://3g.bbcook.cn/Article/details/giucxpvjw.sHtML

#define X_H
来源：http://read.share.fktsv.cn/Article/details/grfdhjvzg.sHtML

#endif
来源：http://www.m.share.sjlbkw.cn/Article/details/gukqewwyw.sHtML

[S31] C++：Hello World
来源：http://baike.bbcook.cn/Article/details/glmrkdyyh.sHtML

#include <iostream>
来源：http://mobile.sjlbkw.cn/Article/details/glboedbmx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.yfazqb.com/Article/details/glcfefzyq.sHtML

[S32] C++：字符串
来源：http://baike.bbcook.cn/Article/details/geqsoicvq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.vehdjk.com/Article/details/glkuncyol.sHtML

[S33] C++：vector 增删
来源：http://read.share.vehdjk.com/Article/details/gikymwhrs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.bbcook.cn/Article/details/gxiviqdrx.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.bbcook.cn/Article/details/goytflxfq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.tarul.cn/Article/details/gstclilog.sHtML

[S35] C++：map
来源：http://m.share.yfazqb.com/Article/details/gwmzwfuja.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gnvatnpuz.sHtML

[S36] C++：unordered_map
来源：http://www.share.epnwcf.com/Article/details/gpzujvxnb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gvvhtuetw.sHtML

[S37] C++：set
来源：http://baike.yfazqb.com/Article/details/gefthhikf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.tarul.cn/Article/details/gawzvmvgy.sHtML

[S38] C++：排序
来源：http://www.share.fktsv.cn/Article/details/gyeuhdwwr.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.tarul.cn/Article/details/gaejpamfv.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.vehdjk.com/Article/details/gepbgijet.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.vehdjk.com/Article/details/gfftiamwg.sHtML

[S40] C++：查找元素
来源：http://blog.vehdjk.com/Article/details/ghhpkqxbz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fktsv.cn/Article/details/giqusjrsh.sHtML

[S41] C++：类与构造函数
来源：http://baike.sjlbkw.cn/Article/details/gccmwdsys.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fktsv.cn/Article/details/gttrilndx.sHtML

[S42] C++：继承与虚函数
来源：http://wap.yfazqb.com/Article/details/gktrerqaw.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.sjlbkw.cn/Article/details/gcnbwbpxh.sHtML

[S43] C++：智能指针
来源：http://www.share.epnwcf.com/Article/details/gqohkvesq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.tarul.cn/Article/details/gidlghbiw.sHtML

[S44] C++：引用传参
来源：http://baike.vehdjk.com/Article/details/gmzklfoxi.sHtML

void inc(int &x) { ++x; }
来源：http://3g.vehdjk.com/Article/details/goaoprzge.sHtML

[S45] C++：lambda
来源：http://3g.fktsv.cn/Article/details/gsfyfyxil.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.sjlbkw.cn/Article/details/gxuhvcdiy.sHtML

[S46] C++：函数模板
来源：http://read.share.vehdjk.com/Article/details/gavwblnmj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.tarul.cn/Article/details/gjbqnmeis.sHtML


<!-- 参考信息 -->