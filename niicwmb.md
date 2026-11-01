代发 wailian999

SHOW INDEX FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gcffobbwd.sHtML

[Q73] 查看表状态
来源：http://www.m.share.yfazqb.com/Article/details/gvmydvgex.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.tarul.cn/Article/details/gdyepvmki.sHtML

[Q74] 强制使用索引
来源：http://read.share.fktsv.cn/Article/details/gezxsbxry.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.bbcook.cn/Article/details/gwpqjotrq.sHtML

[Q75] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gtfnshhez.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.bbcook.cn/Article/details/gwfpmkhbw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.epnwcf.com/Article/details/gscwsatcx.sHtML

[Q76] 按天统计
来源：http://www.m.share.fktsv.cn/Article/details/gwncsmejz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.bbcook.cn/Article/details/gqfosocjy.sHtML

[Q77] 时间加减
来源：http://wap.epnwcf.com/Article/details/gupntswxj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.vehdjk.com/Article/details/gxhjylyrt.sHtML

[Q78] 当前时间
来源：http://read.share.vehdjk.com/Article/details/gadsyrpon.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.yfazqb.com/Article/details/gkuhgyknl.sHtML

[Q79] 字符串拼接
来源：http://blog.tarul.cn/Article/details/gbrdetzar.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fktsv.cn/Article/details/gadjnxnyx.sHtML

[Q80] 字符串截取
来源：http://baike.yfazqb.com/Article/details/gdnakebkt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/grfuglsvp.sHtML

[Q81] 字符串替换
来源：http://baike.epnwcf.com/Article/details/gkisfllsh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.epnwcf.com/Article/details/gapgblolu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.vehdjk.com/Article/details/gbvubndos.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gcemqemyt.sHtML

[Q83] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/guwwonhlp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/ghpbvyvmp.sHtML

[Q84] 去除首尾空格
来源：http://www.share.bbcook.cn/Article/details/girmzvybk.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/ghfvbtkgn.sHtML

[Q85] 数值取整
来源：http://wap.tarul.cn/Article/details/gmqwpywth.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.vehdjk.com/Article/details/gumongcbn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.vehdjk.com/Article/details/grytimfoy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.epnwcf.com/Article/details/gybhrpuol.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fktsv.cn/Article/details/gwoshmdhu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.sjlbkw.cn/Article/details/gxidqnhqy.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.vehdjk.com/Article/details/gbgsjbqvz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.vehdjk.com/Article/details/gpobxyzqv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.vehdjk.com/Article/details/gqxonsrav.sHtML

[Q89] 判断表是否存在
来源：http://www.share.yfazqb.com/Article/details/glnsthjnj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.epnwcf.com/Article/details/gaimeglpq.sHtML

[Q90] 生成序号列
来源：http://3g.tarul.cn/Article/details/gvauyzpvk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.sjlbkw.cn/Article/details/gdgwefggo.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjxrqmwom.sHtML

R. Bash 专题
来源：http://www.share.yfazqb.com/Article/details/gdgalrbxw.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gzpsnauoh.sHtML

[R01] shebang 与严格模式
来源：http://www.share.bbcook.cn/Article/details/gcbzayunt.sHtML

#!/usr/bin/env bash
来源：http://wap.epnwcf.com/Article/details/gaqslehsk.sHtML

set -euo pipefail
来源：http://mobile.bbcook.cn/Article/details/gqfovskql.sHtML

[R02] 变量赋值与使用
来源：http://blog.epnwcf.com/Article/details/gsnfzudbb.sHtML

name="Tom"; echo "$name"
来源：http://mobile.yfazqb.com/Article/details/gaoadlaqb.sHtML

[R03] 只读变量
来源：http://wap.tarul.cn/Article/details/guynicpym.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/gifdzzlvs.sHtML

[R04] 位置参数
来源：http://mobile.vehdjk.com/Article/details/gvbpuhyae.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.bbcook.cn/Article/details/gevrkbaak.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gmzsvkanw.sHtML

name="${1:-default}"
来源：http://wap.tarul.cn/Article/details/gxbjwaiwo.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.yfazqb.com/Article/details/gdzcfqplc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnqddaehy.sHtML

[R07] if 判断文件
来源：http://read.share.epnwcf.com/Article/details/goipyacmg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gnroveavf.sHtML

[R08] 数值比较
来源：http://m.share.sjlbkw.cn/Article/details/gsazybdvm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fktsv.cn/Article/details/gkfqfzufu.sHtML

[R09] 字符串比较
来源：http://blog.yfazqb.com/Article/details/geqabddfd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.tarul.cn/Article/details/gpbcypkqj.sHtML

[R10] 正则匹配
来源：http://read.share.bbcook.cn/Article/details/gxzdtabyh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.tarul.cn/Article/details/gtyltpyxj.sHtML

[R11] case 多分支
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhrloxua.sHtML

case "$1" in
来源：http://read.share.bbcook.cn/Article/details/giogwmfhi.sHtML

start) echo "启动" ;;
来源：http://blog.fktsv.cn/Article/details/gnpipvjlf.sHtML

stop)  echo "停止" ;;
来源：http://baike.sjlbkw.cn/Article/details/gqjvmekec.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.epnwcf.com/Article/details/gdrkpvgpd.sHtML

esac
来源：http://3g.fktsv.cn/Article/details/gqaqcedko.sHtML

[R12] for 遍历文件
来源：http://3g.tarul.cn/Article/details/gfpzjulxf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.epnwcf.com/Article/details/gkanooyck.sHtML

[R13] for 计数循环
来源：http://read.share.sjlbkw.cn/Article/details/gfsdxcbmn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gmlqnzype.sHtML

[R14] C 风格 for
来源：http://m.share.tarul.cn/Article/details/gmnvsacuc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gzlmxybxh.sHtML

[R15] while 逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gfqmkrcnx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhfdaqvl.sHtML

[R16] until 等待条件
来源：http://mobile.sjlbkw.cn/Article/details/gxnjkpubn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/geqvtoqni.sHtML

[R17] 数组定义与取值
来源：http://blog.bbcook.cn/Article/details/gzubngdfy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.yfazqb.com/Article/details/gzdbipgvc.sHtML

[R18] 遍历数组
来源：http://m.share.bbcook.cn/Article/details/ghhpjozqy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.bbcook.cn/Article/details/gkmcxjpvh.sHtML

[R19] 数组长度
来源：http://m.share.fktsv.cn/Article/details/grgzfxsex.sHtML

echo "${#arr[@]}"
来源：http://read.share.yfazqb.com/Article/details/gznqognuy.sHtML

[R20] 关联数组（字典）
来源：http://read.share.tarul.cn/Article/details/gplsgrzyy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.bbcook.cn/Article/details/ggyojhkmv.sHtML

[R21] 字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gvtdlhcyu.sHtML

echo "${#s}"
来源：http://baike.vehdjk.com/Article/details/gxaezwgqn.sHtML

[R22] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/gkajzewpq.sHtML

echo "${s:0:5}"
来源：http://mobile.epnwcf.com/Article/details/gfimqpits.sHtML

[R23] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gwpzjdatv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fktsv.cn/Article/details/gaqnlblks.sHtML

[R24] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gttzksysm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.vehdjk.com/Article/details/gxvmrlarm.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.yfazqb.com/Article/details/gqbpgezuf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.bbcook.cn/Article/details/gixyhqrah.sHtML

[R26] 命令替换
来源：http://wap.bbcook.cn/Article/details/gtkosrgxf.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.yfazqb.com/Article/details/gyghmailt.sHtML

[R27] 算术展开
来源：http://read.share.fktsv.cn/Article/details/gbuxqagis.sHtML

echo $((1 + 2 * 3))
来源：http://blog.epnwcf.com/Article/details/gvzctlfwk.sHtML

[R28] 浮点运算
来源：http://wap.epnwcf.com/Article/details/gqlfjghij.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.epnwcf.com/Article/details/gqkgailla.sHtML

[R29] 定义函数
来源：http://www.share.bbcook.cn/Article/details/glzleidjk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.tarul.cn/Article/details/grwukumjt.sHtML

[R30] 函数返回状态码
来源：http://blog.yfazqb.com/Article/details/gyaqclsqv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.epnwcf.com/Article/details/ggnxkkxzh.sHtML

[R31] 局部变量
来源：http://mobile.bbcook.cn/Article/details/gastfffdm.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.sjlbkw.cn/Article/details/gavydidap.sHtML

[R32] 参数个数校验
来源：http://blog.vehdjk.com/Article/details/ghkffeled.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.sjlbkw.cn/Article/details/gbqfjlyrr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.epnwcf.com/Article/details/gokzkugeb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.tarul.cn/Article/details/gskhefmog.sHtML

[R34] 退出时清理
来源：http://www.m.share.epnwcf.com/Article/details/gwoblxmgz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gdqppvalj.sHtML

[R35] 后台执行并等待
来源：http://mobile.tarul.cn/Article/details/gxwzpeibc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.yfazqb.com/Article/details/gnirdwysv.sHtML

[R36] 并发执行多个任务
来源：http://www.share.vehdjk.com/Article/details/gqmdxfhxg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.bbcook.cn/Article/details/gwlvokpzf.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.tarul.cn/Article/details/gkjqejwfp.sHtML

files=$(ls -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxsfgdeg.sHtML

[R38] 管道串联
来源：http://m.share.tarul.cn/Article/details/gqddbbzam.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.yfazqb.com/Article/details/gekkcyfjz.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.sjlbkw.cn/Article/details/glpteylgc.sHtML

cmd > out.log 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gerroruvx.sHtML

[R40] 追加写日志
来源：http://3g.sjlbkw.cn/Article/details/gmwciqokn.sHtML

echo "log" >> out.log
来源：http://mobile.tarul.cn/Article/details/glldchkxi.sHtML

[R41] 丢弃输出
来源：http://blog.fktsv.cn/Article/details/gbaaaezuf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gpffzbctu.sHtML

[R42] 输入重定向
来源：http://www.blog.fktsv.cn/Article/details/gshewheid.sHtML

wc -l < a.txt
来源：http://m.share.fktsv.cn/Article/details/gcmvtihfr.sHtML

[R43] 按名字查找文件
来源：http://m.share.epnwcf.com/Article/details/grsfiuoix.sHtML

find . -name "*.log" -type f
来源：http://wap.fktsv.cn/Article/details/gdcamhxvk.sHtML

[R44] 按修改时间查找
来源：http://3g.tarul.cn/Article/details/gxadttfhd.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fktsv.cn/Article/details/gdovyyrhn.sHtML

[R45] 批量删除
来源：http://www.m.share.tarul.cn/Article/details/gtxrgqxms.sHtML

find . -name "*.tmp" -delete
来源：http://wap.bbcook.cn/Article/details/gqqqoltjn.sHtML

[R46] 递归替换文件内容
来源：http://mobile.bbcook.cn/Article/details/gfaccfcvf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.epnwcf.com/Article/details/gxvkyyxva.sHtML

[R47] sed 单行替换
来源：http://wap.bbcook.cn/Article/details/gnzkgmyau.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gzfjzzbjw.sHtML

[R48] awk 取指定列
来源：http://blog.sjlbkw.cn/Article/details/gawscitpf.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fktsv.cn/Article/details/gioztojte.sHtML

[R49] awk 带条件
来源：http://mobile.bbcook.cn/Article/details/ghrebdgst.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/gdqcvjibs.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/gwedkvoly.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gahqnkxbb.sHtML

[R51] 排序去重取前几
来源：http://3g.tarul.cn/Article/details/ghzxplwzg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.bbcook.cn/Article/details/gwotivpak.sHtML

[R52] 统计行数
来源：http://3g.epnwcf.com/Article/details/gbvjadvaa.sHtML

wc -l a.txt
来源：http://www.blog.epnwcf.com/Article/details/ghxsqqedq.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.vehdjk.com/Article/details/gsplrzmmx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/gencpjhtb.sHtML

[R54] 比较两个文件
来源：http://baike.vehdjk.com/Article/details/goahyreuu.sHtML

diff a.txt b.txt
来源：http://mobile.yfazqb.com/Article/details/gkjfsbsva.sHtML

[R55] 压缩与解压
来源：http://m.share.bbcook.cn/Article/details/gjlrwwpbl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fktsv.cn/Article/details/gcknhhzxe.sHtML

[R56] 远程拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gafniqnzn.sHtML

scp file user@host:/path/
来源：http://m.share.yfazqb.com/Article/details/giixnwdnu.sHtML

[R57] 远程执行命令
来源：http://wap.bbcook.cn/Article/details/gwlalcofr.sHtML

ssh user@host 'uptime'
来源：http://www.share.bbcook.cn/Article/details/gifwnryzs.sHtML

[R58] 下载文件
来源：http://www.blog.fktsv.cn/Article/details/gugcmjppp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.bbcook.cn/Article/details/ggkxtborz.sHtML

[R59] 发 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gtkqijvrd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.sjlbkw.cn/Article/details/gtsbnkktk.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/giacwsnjj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.sjlbkw.cn/Article/details/gqlprupct.sHtML

[R61] 磁盘占用
来源：http://blog.vehdjk.com/Article/details/gahtxlsir.sHtML

df -h;  du -sh *
来源：http://www.blog.epnwcf.com/Article/details/gtzfsdtrl.sHtML

[R62] 找最占空间的文件
来源：http://3g.yfazqb.com/Article/details/gudhaiwke.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.epnwcf.com/Article/details/gxnhrrqfa.sHtML

[R63] 内存与进程
来源：http://www.m.share.fktsv.cn/Article/details/ggphqvhkv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.vehdjk.com/Article/details/ghttpzokc.sHtML

[R64] 结束进程
来源：http://www.share.vehdjk.com/Article/details/gaystdgpx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.yfazqb.com/Article/details/gcddfvvqh.sHtML

[R65] 查看端口占用
来源：http://www.share.bbcook.cn/Article/details/gnycabhmi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.tarul.cn/Article/details/ghhxpweth.sHtML

[R66] 定时任务
来源：http://www.m.share.tarul.cn/Article/details/gomihgsrt.sHtML

crontab -e;  crontab -l
来源：http://www.blog.bbcook.cn/Article/details/gkqyiuqdv.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.vehdjk.com/Article/details/gnjghrxuf.sHtML

openssl rand -hex 16
来源：http://3g.yfazqb.com/Article/details/gxtpftbpu.sHtML

[R68] 计算文件校验值
来源：http://baike.epnwcf.com/Article/details/gcvbakybq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.sjlbkw.cn/Article/details/gzchjiczg.sHtML

[R69] 生成随机密码
来源：http://www.share.sjlbkw.cn/Article/details/gknnjxdgd.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.sjlbkw.cn/Article/details/gxjycakln.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fktsv.cn/Article/details/gmncvvsem.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/gflwxmruv.sHtML

[R71] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gmrblkqia.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/gbjyyzqxo.sHtML

[R72] 等待端口就绪
来源：http://www.blog.bbcook.cn/Article/details/gqldjturw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/gteytkqew.sHtML

[R73] 分割大日志
来源：http://read.share.fktsv.cn/Article/details/gbkyypucw.sHtML

split -l 1000 big.log part_
来源：http://mobile.bbcook.cn/Article/details/gxgfydccc.sHtML

[R74] 批量重命名
来源：http://read.share.fktsv.cn/Article/details/gnbqdsuwh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.tarul.cn/Article/details/gudnvyvpk.sHtML

[R75] 导出环境变量
来源：http://wap.tarul.cn/Article/details/gugkdrbxs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.sjlbkw.cn/Article/details/gatwlajwo.sHtML

[R76] 使用临时文件
来源：http://www.m.share.vehdjk.com/Article/details/gdoflivmo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/gnjzjxczz.sHtML

[R77] 读取用户输入
来源：http://www.blog.yfazqb.com/Article/details/gfnndampk.sHtML

read -rp "请输入: " ans
来源：http://wap.fktsv.cn/Article/details/gyzdvhaff.sHtML

[R78] 交互式菜单
来源：http://www.share.fktsv.cn/Article/details/gddejkpzg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.yfazqb.com/Article/details/gmdndwpiz.sHtML

[R79] 解析命令行选项
来源：http://mobile.vehdjk.com/Article/details/guvwzivkl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.sjlbkw.cn/Article/details/gagjazcej.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.bbcook.cn/Article/details/grfirtzka.sHtML

time ./run.sh
来源：http://www.m.share.epnwcf.com/Article/details/gfrpztofh.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpzhxpxqi.sHtML

S. C / C++ 专题
来源：http://3g.bbcook.cn/Article/details/gxddwejqb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gnvjgmhtn.sHtML

[S01] C：Hello World
来源：http://3g.epnwcf.com/Article/details/gtcjotits.sHtML

#include <stdio.h>
来源：http://3g.tarul.cn/Article/details/gpejuzuae.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/gjfnonprp.sHtML

[S02] C：变量与格式化输出
来源：http://blog.sjlbkw.cn/Article/details/gbbdsflts.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.vehdjk.com/Article/details/gbwxbxost.sHtML

[S03] C：读入整数
来源：http://wap.fktsv.cn/Article/details/gdvyxuksb.sHtML

int x; scanf("%d", &x);
来源：http://read.share.vehdjk.com/Article/details/gwqsbtltu.sHtML

[S04] C：字符串复制
来源：http://3g.yfazqb.com/Article/details/gcrkugbgt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.vehdjk.com/Article/details/grtupqtem.sHtML

[S05] C：字符串长度
来源：http://baike.tarul.cn/Article/details/gacqtlxww.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/glowdfmuy.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/geqesyrhx.sHtML

strcmp(a, b) == 0
来源：http://mobile.fktsv.cn/Article/details/gqrrvlgqd.sHtML

[S07] C：数组遍历求和
来源：http://m.share.sjlbkw.cn/Article/details/gtwobpwfn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.tarul.cn/Article/details/gvohgylgu.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.tarul.cn/Article/details/gwsspsrvo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.epnwcf.com/Article/details/gbhyrfqsb.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fktsv.cn/Article/details/gcpoadcoq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/gpayhbvcw.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.vehdjk.com/Article/details/gndrkcodc.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.bbcook.cn/Article/details/grisqxuti.sHtML

[S11] C：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gluyljrcl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.yfazqb.com/Article/details/gxrjdokch.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gctqgblzd.sHtML

fclose(f);
来源：http://3g.epnwcf.com/Article/details/glpzpxzay.sHtML

[S12] C：写文件
来源：http://blog.tarul.cn/Article/details/gchvrjzkd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.vehdjk.com/Article/details/gcwzdcfko.sHtML

[S13] C：宏定义
来源：http://read.share.tarul.cn/Article/details/gmfqvskfh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.bbcook.cn/Article/details/gupclweiv.sHtML

[S14] C：枚举
来源：http://3g.epnwcf.com/Article/details/gswzordir.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.epnwcf.com/Article/details/gekqwjgoi.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/gxwqnnosl.sHtML

(double) a / b
来源：http://3g.bbcook.cn/Article/details/guaxoiryj.sHtML

[S16] C：位操作置位
来源：http://wap.sjlbkw.cn/Article/details/gqtbihljt.sHtML

x |= (1 << 3);
来源：http://www.share.tarul.cn/Article/details/gpxqpkntb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.epnwcf.com/Article/details/gostdjchf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fktsv.cn/Article/details/ggvutkvnd.sHtML

[S18] C：命令行参数
来源：http://www.m.share.tarul.cn/Article/details/glhbdyhnu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.bbcook.cn/Article/details/gekanqnoi.sHtML

[S19] C：快速排序
来源：http://blog.bbcook.cn/Article/details/gynbtlqbt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gnbyboqxv.sHtML

[S20] C：二分查找
来源：http://read.share.tarul.cn/Article/details/gvgyyopsl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gtjgcaqha.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gsawegjxq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.tarul.cn/Article/details/gdodyumro.sHtML

[S22] C：字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gjxqwdjsl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.sjlbkw.cn/Article/details/grolnulqk.sHtML

[S23] C：随机数
来源：http://m.share.yfazqb.com/Article/details/gwgcflidg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.vehdjk.com/Article/details/gmxkgxbcn.sHtML

[S24] C：获取本地时间
来源：http://mobile.epnwcf.com/Article/details/gldvkcocl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.vehdjk.com/Article/details/gfuqjhqcn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/glfzjfjxe.sHtML

memcpy(dst, src, n);
来源：http://baike.sjlbkw.cn/Article/details/gjrgqwouo.sHtML

[S26] C：内存清零
来源：http://baike.epnwcf.com/Article/details/ggewkmvok.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gjhalvyzt.sHtML

[S27] C：定义常量
来源：http://www.share.sjlbkw.cn/Article/details/gxoeatjpu.sHtML

const double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gjzvkhdjs.sHtML

[S28] C：静态变量
来源：http://blog.epnwcf.com/Article/details/gcylnisdm.sHtML

static int counter = 0;
来源：http://blog.yfazqb.com/Article/details/gcasptrcq.sHtML

[S29] C：变参函数
来源：http://baike.fktsv.cn/Article/details/glmvezsrq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.tarul.cn/Article/details/ginkvzgah.sHtML

[S30] C：头文件保护
来源：http://3g.fktsv.cn/Article/details/gqzuecscs.sHtML

#ifndef X_H
来源：http://mobile.vehdjk.com/Article/details/gyfeiznlt.sHtML

#define X_H
来源：http://mobile.yfazqb.com/Article/details/gorztbpid.sHtML

#endif
来源：http://wap.vehdjk.com/Article/details/grgsfgtpo.sHtML

[S31] C++：Hello World
来源：http://m.share.bbcook.cn/Article/details/gcztqlubx.sHtML

#include <iostream>
来源：http://read.share.yfazqb.com/Article/details/gpyrmsemh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.bbcook.cn/Article/details/gpxyiwhsr.sHtML

[S32] C++：字符串
来源：http://read.share.epnwcf.com/Article/details/guekmwujn.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.tarul.cn/Article/details/gvwjcsiax.sHtML

[S33] C++：vector 增删
来源：http://wap.epnwcf.com/Article/details/gbjbkenrx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.tarul.cn/Article/details/gyqktlywn.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/gjnezxeca.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.bbcook.cn/Article/details/gcnicztme.sHtML

[S35] C++：map
来源：http://wap.vehdjk.com/Article/details/gjpfsvuzr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gjhqcqrqy.sHtML

[S36] C++：unordered_map
来源：http://www.share.bbcook.cn/Article/details/gfqdpxeaa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gjbpkbosg.sHtML

[S37] C++：set
来源：http://www.blog.epnwcf.com/Article/details/gvzaaudjp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.epnwcf.com/Article/details/gzfegtkqa.sHtML

[S38] C++：排序
来源：http://wap.sjlbkw.cn/Article/details/gvjmeegby.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gwiqnzlbx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.epnwcf.com/Article/details/gimxnsdrh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.tarul.cn/Article/details/ggabtzdvt.sHtML

[S40] C++：查找元素
来源：http://m.share.epnwcf.com/Article/details/gzkavkgss.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.bbcook.cn/Article/details/gwcbabsbj.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gerdtiawj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.yfazqb.com/Article/details/gtmpwxnta.sHtML

[S42] C++：继承与虚函数
来源：http://wap.sjlbkw.cn/Article/details/gnywxyjzx.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.vehdjk.com/Article/details/gacnfirmx.sHtML


<!-- 参考信息 -->