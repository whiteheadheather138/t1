代发 wailian999

ANALYZE TABLE users;
来源：http://www.share.bbcook.cn/Article/details/gzkjtfimo.sHtML

[Q71] 查看建表语句
来源：http://read.share.bbcook.cn/Article/details/gajislsbn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.tarul.cn/Article/details/gizrmgqzi.sHtML

[Q72] 查看索引
来源：http://wap.fktsv.cn/Article/details/glxbfiwsq.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gpmfnhnwj.sHtML

[Q73] 查看表状态
来源：http://3g.vehdjk.com/Article/details/ggguhboev.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.bbcook.cn/Article/details/gjjpiqurt.sHtML

[Q74] 强制使用索引
来源：http://m.share.epnwcf.com/Article/details/gmmrwmdoe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/gibtwelav.sHtML

[Q75] 日期格式化
来源：http://wap.yfazqb.com/Article/details/gpvulltaz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gxbsqmstg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.epnwcf.com/Article/details/gjqckurhz.sHtML

[Q76] 按天统计
来源：http://www.blog.sjlbkw.cn/Article/details/goicnjbmd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.sjlbkw.cn/Article/details/goydkxmny.sHtML

[Q77] 时间加减
来源：http://3g.bbcook.cn/Article/details/geauurxdh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.bbcook.cn/Article/details/ghntuedcs.sHtML

[Q78] 当前时间
来源：http://mobile.epnwcf.com/Article/details/gwhtnodbe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fktsv.cn/Article/details/guwhhpaak.sHtML

[Q79] 字符串拼接
来源：http://blog.bbcook.cn/Article/details/gyxybkrrd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/gnrjkofsq.sHtML

[Q80] 字符串截取
来源：http://read.share.fktsv.cn/Article/details/gnqxmbmlu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gluopbgtj.sHtML

[Q81] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/gogaoydvt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.vehdjk.com/Article/details/gfedlksdw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/gdjaurdft.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gbtdmjiln.sHtML

[Q83] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gpwcisbap.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/grnwacwcq.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gqroammuq.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gehnzwlkh.sHtML

[Q85] 数值取整
来源：http://mobile.fktsv.cn/Article/details/gpnkwnygv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fktsv.cn/Article/details/gkoertmcf.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.vehdjk.com/Article/details/gervuuudi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.sjlbkw.cn/Article/details/gmsyymymu.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.yfazqb.com/Article/details/gpzhicgdj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fktsv.cn/Article/details/ghrrsrrcm.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.tarul.cn/Article/details/gzomrtvnr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.sjlbkw.cn/Article/details/gfoyekskv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gguczelyd.sHtML

[Q89] 判断表是否存在
来源：http://baike.epnwcf.com/Article/details/gphjhrkif.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.epnwcf.com/Article/details/gwlzkwkoc.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/gwarzwgsd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.yfazqb.com/Article/details/gfcrcoqis.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gaqmufeuw.sHtML

R. Bash 专题
来源：http://www.m.share.epnwcf.com/Article/details/gfgkabmve.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grhlvazjk.sHtML

[R01] shebang 与严格模式
来源：http://3g.vehdjk.com/Article/details/gkifospkl.sHtML

#!/usr/bin/env bash
来源：http://mobile.vehdjk.com/Article/details/gucokrkqv.sHtML

set -euo pipefail
来源：http://www.share.vehdjk.com/Article/details/gjuztoplh.sHtML

[R02] 变量赋值与使用
来源：http://www.share.yfazqb.com/Article/details/gaaplmdfy.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fktsv.cn/Article/details/gzmjxqgec.sHtML

[R03] 只读变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gyimpdesc.sHtML

readonly PI=3.14
来源：http://www.blog.yfazqb.com/Article/details/gpiynyuds.sHtML

[R04] 位置参数
来源：http://baike.bbcook.cn/Article/details/gjcthmygd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.vehdjk.com/Article/details/gntfaohex.sHtML

[R05] 参数默认值
来源：http://m.share.tarul.cn/Article/details/gtaixfrqa.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/gnifrfbrf.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gzuaabbyi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/grrqnjnce.sHtML

[R07] if 判断文件
来源：http://www.blog.sjlbkw.cn/Article/details/gsgpublph.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.vehdjk.com/Article/details/gsreiujuk.sHtML

[R08] 数值比较
来源：http://m.share.tarul.cn/Article/details/gtwuvptov.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.sjlbkw.cn/Article/details/gpluxnoim.sHtML

[R09] 字符串比较
来源：http://baike.bbcook.cn/Article/details/geybfkfqo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.tarul.cn/Article/details/gdiuemlll.sHtML

[R10] 正则匹配
来源：http://read.share.vehdjk.com/Article/details/gmqimjrdq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.bbcook.cn/Article/details/grpsjrldt.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gubtnwaxk.sHtML

case "$1" in
来源：http://www.blog.yfazqb.com/Article/details/gcbmlchyx.sHtML

start) echo "启动" ;;
来源：http://m.share.yfazqb.com/Article/details/gvztwkoka.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fktsv.cn/Article/details/geqeobeut.sHtML

*)     echo "未知命令" ;;
来源：http://blog.epnwcf.com/Article/details/gerykbzvp.sHtML

esac
来源：http://www.share.tarul.cn/Article/details/gvasrywbg.sHtML

[R12] for 遍历文件
来源：http://m.share.tarul.cn/Article/details/gofmewdip.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.epnwcf.com/Article/details/gelgslzyt.sHtML

[R13] for 计数循环
来源：http://blog.bbcook.cn/Article/details/genomxrnl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gtqrbwjtz.sHtML

[R14] C 风格 for
来源：http://3g.fktsv.cn/Article/details/grwvfbzom.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gmrzefisu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gpbtidmfw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fktsv.cn/Article/details/gebvhukgz.sHtML

[R16] until 等待条件
来源：http://www.blog.bbcook.cn/Article/details/gsbqrnqmi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gbmredyog.sHtML

[R17] 数组定义与取值
来源：http://mobile.yfazqb.com/Article/details/gixknegch.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.yfazqb.com/Article/details/gnjucfljz.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/gmftotmab.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fktsv.cn/Article/details/gnwoybxyh.sHtML

[R19] 数组长度
来源：http://3g.bbcook.cn/Article/details/gtqnqtcnf.sHtML

echo "${#arr[@]}"
来源：http://m.share.epnwcf.com/Article/details/gttqjgnjc.sHtML

[R20] 关联数组（字典）
来源：http://wap.fktsv.cn/Article/details/glnewryrz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.epnwcf.com/Article/details/geuiavtci.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/ggajqjoyb.sHtML

echo "${#s}"
来源：http://wap.sjlbkw.cn/Article/details/ggiypokvi.sHtML

[R22] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/gfrmahjmm.sHtML

echo "${s:0:5}"
来源：http://3g.tarul.cn/Article/details/gkwlggpze.sHtML

[R23] 字符串替换
来源：http://wap.yfazqb.com/Article/details/gsajsxcqq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.tarul.cn/Article/details/gjzxmfuru.sHtML

[R24] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gtjebladn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.vehdjk.com/Article/details/guaxbcova.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fktsv.cn/Article/details/grmccogmo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.sjlbkw.cn/Article/details/gjzkooqqm.sHtML

[R26] 命令替换
来源：http://www.m.share.yfazqb.com/Article/details/gkwlymlfg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.bbcook.cn/Article/details/gbwztfpwr.sHtML

[R27] 算术展开
来源：http://m.share.fktsv.cn/Article/details/gdtkobdkb.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.tarul.cn/Article/details/gpjgmubrx.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/ghiatpehc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.yfazqb.com/Article/details/gjuuyrint.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/gzoyrcuzc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.yfazqb.com/Article/details/gjjikqfdx.sHtML

[R30] 函数返回状态码
来源：http://read.share.sjlbkw.cn/Article/details/giisaksjj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fktsv.cn/Article/details/gkjftnwow.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/gzqifiwgk.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.epnwcf.com/Article/details/gplpmssxd.sHtML

[R32] 参数个数校验
来源：http://mobile.bbcook.cn/Article/details/gqisanrkh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/gmpmkkxzo.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.vehdjk.com/Article/details/gkyrumyil.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.vehdjk.com/Article/details/gvrckhbzx.sHtML

[R34] 退出时清理
来源：http://mobile.yfazqb.com/Article/details/gtnhbrzjt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/ggclxlxxi.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.tarul.cn/Article/details/gkjwnucbx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.tarul.cn/Article/details/gpytoisyb.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.yfazqb.com/Article/details/gjiticjut.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.yfazqb.com/Article/details/gahzwmapa.sHtML

[R37] 把输出赋给变量
来源：http://wap.sjlbkw.cn/Article/details/gwrdcsnmp.sHtML

files=$(ls -1)
来源：http://blog.sjlbkw.cn/Article/details/gkdxjwzbh.sHtML

[R38] 管道串联
来源：http://wap.sjlbkw.cn/Article/details/godewfdnx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.bbcook.cn/Article/details/gkxnceesn.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.yfazqb.com/Article/details/gfykttnge.sHtML

cmd > out.log 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gaefasxzi.sHtML

[R40] 追加写日志
来源：http://m.share.bbcook.cn/Article/details/ggmczfjle.sHtML

echo "log" >> out.log
来源：http://wap.sjlbkw.cn/Article/details/gzlpeoksb.sHtML

[R41] 丢弃输出
来源：http://www.m.share.yfazqb.com/Article/details/gyucmzioi.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/gsraybryw.sHtML

[R42] 输入重定向
来源：http://blog.sjlbkw.cn/Article/details/gotxftkry.sHtML

wc -l < a.txt
来源：http://www.share.epnwcf.com/Article/details/gvcbnfyes.sHtML

[R43] 按名字查找文件
来源：http://m.share.sjlbkw.cn/Article/details/gdwitmvnr.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.yfazqb.com/Article/details/gpctnbjdw.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/gbpwhwkpm.sHtML

find . -mtime -7 -type f
来源：http://m.share.fktsv.cn/Article/details/gqvnovxat.sHtML

[R45] 批量删除
来源：http://www.m.share.yfazqb.com/Article/details/gpglzsaaz.sHtML

find . -name "*.tmp" -delete
来源：http://blog.sjlbkw.cn/Article/details/gacuanfav.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.sjlbkw.cn/Article/details/gkihaykhh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.vehdjk.com/Article/details/gaqwqpjno.sHtML

[R47] sed 单行替换
来源：http://m.share.bbcook.cn/Article/details/gknzvvvgf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fktsv.cn/Article/details/gspbyafqr.sHtML

[R48] awk 取指定列
来源：http://www.blog.yfazqb.com/Article/details/gsphzsshh.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.epnwcf.com/Article/details/gcdqwhbae.sHtML

[R49] awk 带条件
来源：http://3g.epnwcf.com/Article/details/ggfywauls.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.sjlbkw.cn/Article/details/ggqwfcxmp.sHtML

[R50] awk 求和
来源：http://3g.sjlbkw.cn/Article/details/ghgdejhyc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.tarul.cn/Article/details/gohvnydus.sHtML

[R51] 排序去重取前几
来源：http://3g.yfazqb.com/Article/details/gerfdgesm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fktsv.cn/Article/details/gcbenfdvz.sHtML

[R52] 统计行数
来源：http://wap.epnwcf.com/Article/details/gymnnspbp.sHtML

wc -l a.txt
来源：http://baike.fktsv.cn/Article/details/gxewmnhom.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.epnwcf.com/Article/details/gdbhfsvhr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.sjlbkw.cn/Article/details/gxxvuotsr.sHtML

[R54] 比较两个文件
来源：http://baike.yfazqb.com/Article/details/gwuskvprn.sHtML

diff a.txt b.txt
来源：http://blog.yfazqb.com/Article/details/gnuksitry.sHtML

[R55] 压缩与解压
来源：http://baike.epnwcf.com/Article/details/gtrnvjnre.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/gcnjkdqfw.sHtML

[R56] 远程拷贝
来源：http://blog.sjlbkw.cn/Article/details/gbedfziov.sHtML

scp file user@host:/path/
来源：http://3g.vehdjk.com/Article/details/gwufrgsbu.sHtML

[R57] 远程执行命令
来源：http://m.share.bbcook.cn/Article/details/gmjwbdlsp.sHtML

ssh user@host 'uptime'
来源：http://m.share.bbcook.cn/Article/details/gpaoknmvz.sHtML

[R58] 下载文件
来源：http://www.share.vehdjk.com/Article/details/gcgobfpqf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/giwxjioim.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gpvgydyeb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.bbcook.cn/Article/details/gfmhqhdee.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gawoewnph.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.sjlbkw.cn/Article/details/gpohsmvfa.sHtML

[R61] 磁盘占用
来源：http://baike.tarul.cn/Article/details/grqtocdqu.sHtML

df -h;  du -sh *
来源：http://www.share.yfazqb.com/Article/details/ggedszyat.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/gqarmdhzw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/gwrilzatd.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/glmpdyqck.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.sjlbkw.cn/Article/details/gycnjdbnl.sHtML

[R64] 结束进程
来源：http://mobile.fktsv.cn/Article/details/geomjbixc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.tarul.cn/Article/details/gnbclepje.sHtML

[R65] 查看端口占用
来源：http://m.share.bbcook.cn/Article/details/gxkzquycf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.yfazqb.com/Article/details/grmotqjdb.sHtML

[R66] 定时任务
来源：http://baike.bbcook.cn/Article/details/gnabzznmk.sHtML

crontab -e;  crontab -l
来源：http://baike.sjlbkw.cn/Article/details/gykuuskvh.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fktsv.cn/Article/details/gkstetojw.sHtML

openssl rand -hex 16
来源：http://www.m.share.yfazqb.com/Article/details/gsugowwps.sHtML

[R68] 计算文件校验值
来源：http://3g.yfazqb.com/Article/details/gfllqktei.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.sjlbkw.cn/Article/details/gisahouba.sHtML

[R69] 生成随机密码
来源：http://mobile.tarul.cn/Article/details/gfzdbnwib.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.epnwcf.com/Article/details/gjasufzmq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.tarul.cn/Article/details/gqpvwihev.sHtML

date +%s;  date -d @1700000000
来源：http://baike.tarul.cn/Article/details/grvammxys.sHtML

[R71] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gefnvcwjl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.epnwcf.com/Article/details/ghttjefff.sHtML

[R72] 等待端口就绪
来源：http://baike.epnwcf.com/Article/details/gqqbfvmgk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gecgpvzpv.sHtML

[R73] 分割大日志
来源：http://www.share.fktsv.cn/Article/details/gzgqmeknt.sHtML

split -l 1000 big.log part_
来源：http://www.blog.epnwcf.com/Article/details/gayptaiam.sHtML

[R74] 批量重命名
来源：http://3g.vehdjk.com/Article/details/gyfjxjlfd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.epnwcf.com/Article/details/gsupvepsv.sHtML

[R75] 导出环境变量
来源：http://3g.epnwcf.com/Article/details/gxzpprndz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.epnwcf.com/Article/details/gbfonldqa.sHtML

[R76] 使用临时文件
来源：http://www.m.share.tarul.cn/Article/details/gxateswab.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gqkuacsrm.sHtML

[R77] 读取用户输入
来源：http://www.blog.fktsv.cn/Article/details/ghewzmjiy.sHtML

read -rp "请输入: " ans
来源：http://m.share.vehdjk.com/Article/details/gfhmthdga.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/gkjintfli.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.tarul.cn/Article/details/gdmauiysb.sHtML

[R79] 解析命令行选项
来源：http://www.blog.vehdjk.com/Article/details/gvoiaqwqx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.tarul.cn/Article/details/gxqqdbbvf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/gtxnuiaup.sHtML

time ./run.sh
来源：http://read.share.vehdjk.com/Article/details/gbaoyonij.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzzlhhkjt.sHtML

S. C / C++ 专题
来源：http://www.share.bbcook.cn/Article/details/gpxdmqpjs.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqjsnhauo.sHtML

[S01] C：Hello World
来源：http://wap.bbcook.cn/Article/details/gsnpwmpsc.sHtML

#include <stdio.h>
来源：http://www.m.share.tarul.cn/Article/details/gzbugxabo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.vehdjk.com/Article/details/gxkkxhncw.sHtML

[S02] C：变量与格式化输出
来源：http://wap.vehdjk.com/Article/details/gdjkxnlmk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.tarul.cn/Article/details/gmaynmayp.sHtML

[S03] C：读入整数
来源：http://www.m.share.fktsv.cn/Article/details/gaohaqydj.sHtML

int x; scanf("%d", &x);
来源：http://blog.bbcook.cn/Article/details/grlqtokrl.sHtML

[S04] C：字符串复制
来源：http://m.share.epnwcf.com/Article/details/grzcuvewf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.yfazqb.com/Article/details/gvrgvunoc.sHtML

[S05] C：字符串长度
来源：http://m.share.bbcook.cn/Article/details/gqorgfahe.sHtML

strlen(s)
来源：http://baike.vehdjk.com/Article/details/glbzzolil.sHtML

[S06] C：字符串比较
来源：http://m.share.tarul.cn/Article/details/glpnhfygz.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.yfazqb.com/Article/details/gougfhhsd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.sjlbkw.cn/Article/details/ghoacoxdw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.yfazqb.com/Article/details/gdbvulwvc.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.vehdjk.com/Article/details/ggxnufubp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.epnwcf.com/Article/details/gyvszydwn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.bbcook.cn/Article/details/gxjofdtir.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.vehdjk.com/Article/details/gwgwunjwf.sHtML

[S10] C：指针与解引用
来源：http://www.share.vehdjk.com/Article/details/gmjsfgzdn.sHtML

int *p = &a;  *p = 5;
来源：http://wap.yfazqb.com/Article/details/gwuprwsqq.sHtML

[S11] C：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gxgxpjgky.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.vehdjk.com/Article/details/ghemctpiy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.epnwcf.com/Article/details/gxrgbgami.sHtML

fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gmtlpgmud.sHtML

[S12] C：写文件
来源：http://read.share.bbcook.cn/Article/details/gmkuvhtxy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/gwjlsyawb.sHtML

[S13] C：宏定义
来源：http://mobile.bbcook.cn/Article/details/groryotje.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.epnwcf.com/Article/details/gsvsuybuf.sHtML

[S14] C：枚举
来源：http://3g.sjlbkw.cn/Article/details/gwohywuje.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.bbcook.cn/Article/details/gffhrymgh.sHtML

[S15] C：类型转换
来源：http://www.blog.fktsv.cn/Article/details/gnvooqghh.sHtML

(double) a / b
来源：http://wap.yfazqb.com/Article/details/gpdqdzxts.sHtML

[S16] C：位操作置位
来源：http://www.blog.yfazqb.com/Article/details/gvngziuyx.sHtML

x |= (1 << 3);
来源：http://read.share.bbcook.cn/Article/details/gxitehxzb.sHtML

[S17] C：安全拼接字符串
来源：http://3g.yfazqb.com/Article/details/ghrhfcfmz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.yfazqb.com/Article/details/gdgvanggg.sHtML

[S18] C：命令行参数
来源：http://www.blog.vehdjk.com/Article/details/gvfdvdnpi.sHtML

int main(int argc, char **argv)
来源：http://wap.epnwcf.com/Article/details/gjgpkflgc.sHtML

[S19] C：快速排序
来源：http://www.m.share.epnwcf.com/Article/details/gdfoetpgq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gsyzedkgm.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gsqsidcpw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gqllbewbb.sHtML

[S21] C：字符类别判断
来源：http://wap.fktsv.cn/Article/details/ggnbuiktw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.vehdjk.com/Article/details/gpbiahutr.sHtML

[S22] C：字符串转数字
来源：http://baike.fktsv.cn/Article/details/gtqrincrb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.sjlbkw.cn/Article/details/gtotifkih.sHtML

[S23] C：随机数
来源：http://www.blog.bbcook.cn/Article/details/gvuioungx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.yfazqb.com/Article/details/gjqpqqjni.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/gptqwerac.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fktsv.cn/Article/details/gkpnoufne.sHtML

[S25] C：内存拷贝
来源：http://baike.sjlbkw.cn/Article/details/gxptnbbwy.sHtML

memcpy(dst, src, n);
来源：http://3g.tarul.cn/Article/details/geikkxznf.sHtML

[S26] C：内存清零
来源：http://m.share.epnwcf.com/Article/details/ginxpivsr.sHtML

memset(a, 0, sizeof a);
来源：http://3g.bbcook.cn/Article/details/gpqlcttzp.sHtML

[S27] C：定义常量
来源：http://www.m.share.fktsv.cn/Article/details/gllbiizsp.sHtML

const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/glimgpxyt.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/gklbzysli.sHtML

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/ghhoshcud.sHtML

[S29] C：变参函数
来源：http://blog.bbcook.cn/Article/details/ghhtfjzxt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.epnwcf.com/Article/details/glfwajvff.sHtML

[S30] C：头文件保护
来源：http://www.blog.epnwcf.com/Article/details/grmjcowav.sHtML

#ifndef X_H
来源：http://m.share.yfazqb.com/Article/details/gitnihyoo.sHtML

#define X_H
来源：http://www.blog.vehdjk.com/Article/details/gyxpuxkra.sHtML

#endif
来源：http://m.share.fktsv.cn/Article/details/ggmlwhlma.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/gptnatdwp.sHtML

#include <iostream>
来源：http://blog.sjlbkw.cn/Article/details/gndihtidu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.yfazqb.com/Article/details/gkplcnxcb.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/gsnyhsise.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fktsv.cn/Article/details/gtgzvsnlt.sHtML

[S33] C++：vector 增删
来源：http://read.share.fktsv.cn/Article/details/gejbbedbe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.yfazqb.com/Article/details/gtyfrdpxc.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/gbxkjboak.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/gcuhzuabo.sHtML

[S35] C++：map
来源：http://www.blog.tarul.cn/Article/details/gvfgxtkzh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gxmainyhi.sHtML

[S36] C++：unordered_map
来源：http://3g.vehdjk.com/Article/details/gwmuwpptw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gproubfui.sHtML

[S37] C++：set
来源：http://www.blog.sjlbkw.cn/Article/details/gjzvbpfnt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.bbcook.cn/Article/details/gjyfrqsbo.sHtML

[S38] C++：排序
来源：http://baike.tarul.cn/Article/details/gaojbmhnh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.vehdjk.com/Article/details/gxozgzglw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.sjlbkw.cn/Article/details/gubttisov.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/giofdaias.sHtML

[S40] C++：查找元素
来源：http://m.share.vehdjk.com/Article/details/gyskcofzx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.tarul.cn/Article/details/grjjjwqnf.sHtML


<!-- 参考信息 -->