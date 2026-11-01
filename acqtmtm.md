代发 wailian999

ROLLBACK TO sp1;
来源：http://www.m.share.tarul.cn/Article/details/gkulmvwhv.sHtML

[Q69] 查看执行计划
来源：http://wap.epnwcf.com/Article/details/gjypprngv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fktsv.cn/Article/details/gzpiphwmp.sHtML

[Q70] 更新统计信息
来源：http://www.blog.bbcook.cn/Article/details/gnczttrhf.sHtML

ANALYZE TABLE users;
来源：http://blog.fktsv.cn/Article/details/gieytytct.sHtML

[Q71] 查看建表语句
来源：http://www.share.vehdjk.com/Article/details/gfgmlggqj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.yfazqb.com/Article/details/gazborhdu.sHtML

[Q72] 查看索引
来源：http://www.share.fktsv.cn/Article/details/govscwldh.sHtML

SHOW INDEX FROM users;
来源：http://3g.epnwcf.com/Article/details/gpilieytu.sHtML

[Q73] 查看表状态
来源：http://baike.yfazqb.com/Article/details/gbjxpeqwi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.vehdjk.com/Article/details/gczlcnqpj.sHtML

[Q74] 强制使用索引
来源：http://mobile.fktsv.cn/Article/details/gzkekrzhx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.sjlbkw.cn/Article/details/ghdbycdcy.sHtML

[Q75] 日期格式化
来源：http://blog.tarul.cn/Article/details/gyjzuagjb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.yfazqb.com/Article/details/gvzlvigla.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.bbcook.cn/Article/details/gahymmrev.sHtML

[Q76] 按天统计
来源：http://www.blog.fktsv.cn/Article/details/giwydzxlk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.epnwcf.com/Article/details/gddojbtjl.sHtML

[Q77] 时间加减
来源：http://3g.epnwcf.com/Article/details/gsyfodiiw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.sjlbkw.cn/Article/details/gatgbghdm.sHtML

[Q78] 当前时间
来源：http://www.m.share.fktsv.cn/Article/details/goovwuspc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.epnwcf.com/Article/details/gfetvpqbg.sHtML

[Q79] 字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/gxymeliqi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.epnwcf.com/Article/details/gdoinbzhp.sHtML

[Q80] 字符串截取
来源：http://www.blog.bbcook.cn/Article/details/gbzcsbrfi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.bbcook.cn/Article/details/geidonvft.sHtML

[Q81] 字符串替换
来源：http://read.share.yfazqb.com/Article/details/gknsmnbqq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.vehdjk.com/Article/details/gxifnvvnn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.vehdjk.com/Article/details/ghzclgyzj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gyqrtuljf.sHtML

[Q83] 大小写转换
来源：http://wap.fktsv.cn/Article/details/ghqxqhvmy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gzgvontto.sHtML

[Q84] 去除首尾空格
来源：http://3g.sjlbkw.cn/Article/details/gmodbjjwq.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gpdjgphlc.sHtML

[Q85] 数值取整
来源：http://mobile.epnwcf.com/Article/details/gupgxesxz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.bbcook.cn/Article/details/ggydmzkdd.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.vehdjk.com/Article/details/gmxibewmg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.yfazqb.com/Article/details/gmjjplqzo.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.tarul.cn/Article/details/gyoiuvleo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.bbcook.cn/Article/details/goytwstzp.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/gphzjhrms.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.bbcook.cn/Article/details/gsmzszcgv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fktsv.cn/Article/details/gqchfjpxc.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.epnwcf.com/Article/details/gupmsmahl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.vehdjk.com/Article/details/gpsnljdcx.sHtML

[Q90] 生成序号列
来源：http://www.m.share.yfazqb.com/Article/details/gjloslsir.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.bbcook.cn/Article/details/gtxgllkrm.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtsyoabjo.sHtML

R. Bash 专题
来源：http://www.blog.bbcook.cn/Article/details/guslxrsxq.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gftznkaxn.sHtML

[R01] shebang 与严格模式
来源：http://3g.sjlbkw.cn/Article/details/gjqturabb.sHtML

#!/usr/bin/env bash
来源：http://3g.bbcook.cn/Article/details/gfwcslumr.sHtML

set -euo pipefail
来源：http://blog.sjlbkw.cn/Article/details/gipelneej.sHtML

[R02] 变量赋值与使用
来源：http://wap.tarul.cn/Article/details/gorqzhtfl.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.sjlbkw.cn/Article/details/gngegkveh.sHtML

[R03] 只读变量
来源：http://www.m.share.yfazqb.com/Article/details/gixmstesj.sHtML

readonly PI=3.14
来源：http://wap.sjlbkw.cn/Article/details/gvphedykh.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/gbkoovafi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.vehdjk.com/Article/details/gkgyshmvp.sHtML

[R05] 参数默认值
来源：http://www.blog.sjlbkw.cn/Article/details/gskifzxpl.sHtML

name="${1:-default}"
来源：http://read.share.yfazqb.com/Article/details/grpdfohnw.sHtML

[R06] 判断命令是否存在
来源：http://wap.bbcook.cn/Article/details/gynncomcx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gcthxjobn.sHtML

[R07] if 判断文件
来源：http://www.m.share.fktsv.cn/Article/details/gupnclwvv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fktsv.cn/Article/details/gvyushvjo.sHtML

[R08] 数值比较
来源：http://m.share.yfazqb.com/Article/details/ggvwhdjvk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gnflamlhj.sHtML

[R09] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/giimcvrbv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.bbcook.cn/Article/details/gewkkdddq.sHtML

[R10] 正则匹配
来源：http://m.share.tarul.cn/Article/details/gtbjvjfeo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/glihexgsb.sHtML

[R11] case 多分支
来源：http://www.share.sjlbkw.cn/Article/details/gywesrxcq.sHtML

case "$1" in
来源：http://read.share.epnwcf.com/Article/details/ghginiudu.sHtML

start) echo "启动" ;;
来源：http://blog.bbcook.cn/Article/details/gtyiqdgfu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gwmuhvinj.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.bbcook.cn/Article/details/gadbwctso.sHtML

esac
来源：http://mobile.yfazqb.com/Article/details/gohuzxqtf.sHtML

[R12] for 遍历文件
来源：http://www.share.bbcook.cn/Article/details/gjwrhqyzd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/gddkkoxiy.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gfoecawsi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/gqppphpqu.sHtML

[R14] C 风格 for
来源：http://read.share.epnwcf.com/Article/details/goeviqsxo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/gruxwmnnq.sHtML

[R15] while 逐行读文件
来源：http://3g.fktsv.cn/Article/details/gjljlkfvf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.sjlbkw.cn/Article/details/gghraregy.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/gqkrbttln.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gvfidldsi.sHtML

[R17] 数组定义与取值
来源：http://read.share.bbcook.cn/Article/details/gbqflarfl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.vehdjk.com/Article/details/gcrcngqws.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gvxkjotaz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.tarul.cn/Article/details/ggzuktscr.sHtML

[R19] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gfmmofaku.sHtML

echo "${#arr[@]}"
来源：http://www.share.tarul.cn/Article/details/gzqbuxfbv.sHtML

[R20] 关联数组（字典）
来源：http://3g.fktsv.cn/Article/details/gdjvrypek.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/gaeehnxud.sHtML

[R21] 字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gttvpwbvk.sHtML

echo "${#s}"
来源：http://read.share.bbcook.cn/Article/details/gugmkulgd.sHtML

[R22] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/gjteqjwrl.sHtML

echo "${s:0:5}"
来源：http://www.m.share.yfazqb.com/Article/details/grtwtlhuk.sHtML

[R23] 字符串替换
来源：http://blog.epnwcf.com/Article/details/gpizekhsr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.yfazqb.com/Article/details/gsnugfuko.sHtML

[R24] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gxrfhbfyk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.sjlbkw.cn/Article/details/grmluuyaz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fktsv.cn/Article/details/ggngfrmur.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.sjlbkw.cn/Article/details/gywqzvywi.sHtML

[R26] 命令替换
来源：http://wap.vehdjk.com/Article/details/gibqlwfik.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.yfazqb.com/Article/details/gdxpaojlz.sHtML

[R27] 算术展开
来源：http://www.blog.tarul.cn/Article/details/gznzbfamx.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/gmdbsnjne.sHtML

[R28] 浮点运算
来源：http://blog.sjlbkw.cn/Article/details/geqzcjpre.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fktsv.cn/Article/details/gjluoihhd.sHtML

[R29] 定义函数
来源：http://www.share.bbcook.cn/Article/details/gzkdqgtav.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.tarul.cn/Article/details/gjkpbxpji.sHtML

[R30] 函数返回状态码
来源：http://baike.bbcook.cn/Article/details/gflmuuqvw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.epnwcf.com/Article/details/gqmufzxjj.sHtML

[R31] 局部变量
来源：http://www.blog.fktsv.cn/Article/details/gescmeczp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.vehdjk.com/Article/details/gstypykwm.sHtML

[R32] 参数个数校验
来源：http://mobile.tarul.cn/Article/details/gbdrrmwrs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gcmhbmhep.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.epnwcf.com/Article/details/ghyjrtnuh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.bbcook.cn/Article/details/gcurhtsfu.sHtML

[R34] 退出时清理
来源：http://mobile.tarul.cn/Article/details/gsjlfuhyg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/gwpoxrrbb.sHtML

[R35] 后台执行并等待
来源：http://m.share.bbcook.cn/Article/details/gpnafudsg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/gofvjqodq.sHtML

[R36] 并发执行多个任务
来源：http://m.share.tarul.cn/Article/details/gwdbjghzq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/gpvwjiwqv.sHtML

[R37] 把输出赋给变量
来源：http://www.share.tarul.cn/Article/details/gxbecjriz.sHtML

files=$(ls -1)
来源：http://read.share.epnwcf.com/Article/details/gwramkeej.sHtML

[R38] 管道串联
来源：http://mobile.vehdjk.com/Article/details/godllrgtj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.yfazqb.com/Article/details/gpjwqaznn.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.sjlbkw.cn/Article/details/gwpqtypap.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/gwarftqbe.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/glrpplteb.sHtML

echo "log" >> out.log
来源：http://www.m.share.fktsv.cn/Article/details/glhuwrsjj.sHtML

[R41] 丢弃输出
来源：http://read.share.sjlbkw.cn/Article/details/gvooujpfg.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/gxoflhhoj.sHtML

[R42] 输入重定向
来源：http://baike.epnwcf.com/Article/details/guklfbvcu.sHtML

wc -l < a.txt
来源：http://read.share.tarul.cn/Article/details/geensikau.sHtML

[R43] 按名字查找文件
来源：http://baike.fktsv.cn/Article/details/gjcuetaij.sHtML

find . -name "*.log" -type f
来源：http://3g.epnwcf.com/Article/details/gpmpmuwin.sHtML

[R44] 按修改时间查找
来源：http://read.share.yfazqb.com/Article/details/gkdqpntrm.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.epnwcf.com/Article/details/gepgzbbpd.sHtML

[R45] 批量删除
来源：http://m.share.sjlbkw.cn/Article/details/gnswgstkm.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fktsv.cn/Article/details/grvensmuq.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.vehdjk.com/Article/details/guzuqfzti.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.epnwcf.com/Article/details/ggdpxdghs.sHtML

[R47] sed 单行替换
来源：http://m.share.tarul.cn/Article/details/gejyapqef.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.yfazqb.com/Article/details/gcnxrxbif.sHtML

[R48] awk 取指定列
来源：http://www.m.share.epnwcf.com/Article/details/gowyvzkdb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.yfazqb.com/Article/details/ghnispjqq.sHtML

[R49] awk 带条件
来源：http://wap.tarul.cn/Article/details/gtqmpzcbs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.yfazqb.com/Article/details/gvjvccymd.sHtML

[R50] awk 求和
来源：http://www.share.bbcook.cn/Article/details/gjfeesfvy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fktsv.cn/Article/details/gxudrhdki.sHtML

[R51] 排序去重取前几
来源：http://www.share.epnwcf.com/Article/details/gmxhcqtvj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.sjlbkw.cn/Article/details/gwgelcmzm.sHtML

[R52] 统计行数
来源：http://blog.epnwcf.com/Article/details/gzxrqbxbu.sHtML

wc -l a.txt
来源：http://wap.tarul.cn/Article/details/gdctbslci.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.vehdjk.com/Article/details/gklcdruvu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.yfazqb.com/Article/details/gspttdvva.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/gmwecevvu.sHtML

diff a.txt b.txt
来源：http://blog.bbcook.cn/Article/details/gfkgtcpvm.sHtML

[R55] 压缩与解压
来源：http://wap.tarul.cn/Article/details/gxrzztmwt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gcermnntj.sHtML

[R56] 远程拷贝
来源：http://www.share.yfazqb.com/Article/details/gpatocdgl.sHtML

scp file user@host:/path/
来源：http://www.m.share.epnwcf.com/Article/details/gabsyvuny.sHtML

[R57] 远程执行命令
来源：http://baike.fktsv.cn/Article/details/ggqbloofq.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.epnwcf.com/Article/details/ggrthenva.sHtML

[R58] 下载文件
来源：http://www.share.tarul.cn/Article/details/goizzfaah.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fktsv.cn/Article/details/gepvlnlrq.sHtML

[R59] 发 POST JSON
来源：http://wap.epnwcf.com/Article/details/ghtzujcsh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.tarul.cn/Article/details/gyxstqqzd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gucueqgvs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.epnwcf.com/Article/details/gmgwwzejt.sHtML

[R61] 磁盘占用
来源：http://3g.tarul.cn/Article/details/gayxolkrs.sHtML

df -h;  du -sh *
来源：http://mobile.sjlbkw.cn/Article/details/gyrjrtebl.sHtML

[R62] 找最占空间的文件
来源：http://read.share.vehdjk.com/Article/details/gwcfhksdj.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.yfazqb.com/Article/details/gdyvwndla.sHtML

[R63] 内存与进程
来源：http://blog.yfazqb.com/Article/details/gjuqskgeb.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.epnwcf.com/Article/details/gbogxulme.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/glrsnakax.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.bbcook.cn/Article/details/glwzagarq.sHtML

[R65] 查看端口占用
来源：http://baike.fktsv.cn/Article/details/guxqqdutb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.sjlbkw.cn/Article/details/gyufguyiu.sHtML

[R66] 定时任务
来源：http://m.share.yfazqb.com/Article/details/gsdzneucs.sHtML

crontab -e;  crontab -l
来源：http://m.share.fktsv.cn/Article/details/gzimelcia.sHtML

[R67] 生成随机十六进制串
来源：http://baike.vehdjk.com/Article/details/gccdyksro.sHtML

openssl rand -hex 16
来源：http://m.share.epnwcf.com/Article/details/gujnqunod.sHtML

[R68] 计算文件校验值
来源：http://3g.vehdjk.com/Article/details/gksflygxy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gdkusfkrd.sHtML

[R69] 生成随机密码
来源：http://baike.yfazqb.com/Article/details/ggawdizcy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.epnwcf.com/Article/details/gdqjymzhz.sHtML

[R70] 时间戳与互转
来源：http://baike.fktsv.cn/Article/details/gdksosmkn.sHtML

date +%s;  date -d @1700000000
来源：http://baike.epnwcf.com/Article/details/gscuhnbqc.sHtML

[R71] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/gigpxfxvo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.tarul.cn/Article/details/gohggpvqa.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gkhkafpfz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gmqutvdyz.sHtML

[R73] 分割大日志
来源：http://www.blog.fktsv.cn/Article/details/gpcqpobfz.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.bbcook.cn/Article/details/gfbqkemav.sHtML

[R74] 批量重命名
来源：http://www.m.share.fktsv.cn/Article/details/gbsbejtir.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.sjlbkw.cn/Article/details/gtwpccnqd.sHtML

[R75] 导出环境变量
来源：http://read.share.bbcook.cn/Article/details/gjcmdthkt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fktsv.cn/Article/details/gfenxblrh.sHtML

[R76] 使用临时文件
来源：http://blog.tarul.cn/Article/details/glvcexnxa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/gnjhctzqy.sHtML

[R77] 读取用户输入
来源：http://mobile.tarul.cn/Article/details/gpssmhrbf.sHtML

read -rp "请输入: " ans
来源：http://www.share.fktsv.cn/Article/details/gcbbiwsas.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fktsv.cn/Article/details/gdognzsey.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsvrtzvx.sHtML

[R79] 解析命令行选项
来源：http://wap.bbcook.cn/Article/details/ghkllyzxi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.sjlbkw.cn/Article/details/gyhkyhthy.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.vehdjk.com/Article/details/gmvoymnlp.sHtML

time ./run.sh
来源：http://read.share.vehdjk.com/Article/details/glbuexprv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gkbzvkoad.sHtML

S. C / C++ 专题
来源：http://www.m.share.bbcook.cn/Article/details/gopcmzrml.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gtjfjvimw.sHtML

[S01] C：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gejaokyxh.sHtML

#include <stdio.h>
来源：http://www.blog.vehdjk.com/Article/details/gjdzhqhdf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gmhyunipr.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gjauomexo.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.bbcook.cn/Article/details/gcoclpitb.sHtML

[S03] C：读入整数
来源：http://www.m.share.bbcook.cn/Article/details/gdapdurcq.sHtML

int x; scanf("%d", &x);
来源：http://3g.fktsv.cn/Article/details/gnnjbuaqa.sHtML

[S04] C：字符串复制
来源：http://mobile.tarul.cn/Article/details/gnayvtbtt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/ggquuhmcl.sHtML

[S05] C：字符串长度
来源：http://www.blog.fktsv.cn/Article/details/girdmionp.sHtML

strlen(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gsdertkmb.sHtML

[S06] C：字符串比较
来源：http://m.share.epnwcf.com/Article/details/gpitksiof.sHtML

strcmp(a, b) == 0
来源：http://blog.sjlbkw.cn/Article/details/gcpebrtdk.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fktsv.cn/Article/details/gkjrppuwl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.bbcook.cn/Article/details/ggpvcaczf.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/ggividepw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.tarul.cn/Article/details/gfmotavhh.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.sjlbkw.cn/Article/details/gyqdihbnw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.sjlbkw.cn/Article/details/garpnbanp.sHtML

[S10] C：指针与解引用
来源：http://www.blog.sjlbkw.cn/Article/details/gxqwmfoie.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.vehdjk.com/Article/details/grlcmawtd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gztmogybp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.yfazqb.com/Article/details/gjifpewxv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.epnwcf.com/Article/details/gweyndkoa.sHtML

fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gfsrstrtw.sHtML

[S12] C：写文件
来源：http://www.share.tarul.cn/Article/details/ghurspito.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gjkkseske.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gdonglvvf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.vehdjk.com/Article/details/gsyutysou.sHtML

[S14] C：枚举
来源：http://read.share.vehdjk.com/Article/details/genxavwkl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.bbcook.cn/Article/details/gyruwkhmb.sHtML

[S15] C：类型转换
来源：http://read.share.fktsv.cn/Article/details/gopyurpmk.sHtML

(double) a / b
来源：http://blog.epnwcf.com/Article/details/gnfcxvqcx.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/goaqgaswc.sHtML

x |= (1 << 3);
来源：http://www.blog.yfazqb.com/Article/details/gxsaofhlu.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fktsv.cn/Article/details/gpqnqjnby.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.bbcook.cn/Article/details/ghrvasnxo.sHtML

[S18] C：命令行参数
来源：http://www.share.epnwcf.com/Article/details/glmcfwruz.sHtML

int main(int argc, char **argv)
来源：http://m.share.bbcook.cn/Article/details/giahyvklo.sHtML

[S19] C：快速排序
来源：http://blog.bbcook.cn/Article/details/geavzfvrn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/guoqbpxuw.sHtML

[S20] C：二分查找
来源：http://m.share.tarul.cn/Article/details/gxwowzenu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.yfazqb.com/Article/details/gbtlctuyr.sHtML

[S21] C：字符类别判断
来源：http://wap.epnwcf.com/Article/details/gleeuzlcn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.vehdjk.com/Article/details/gymspcwct.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gcceazdld.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.tarul.cn/Article/details/godhdfjep.sHtML

[S23] C：随机数
来源：http://3g.tarul.cn/Article/details/gtriacjsy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.yfazqb.com/Article/details/glhcxpnve.sHtML

[S24] C：获取本地时间
来源：http://baike.bbcook.cn/Article/details/govzpabyn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fktsv.cn/Article/details/geljtxidu.sHtML

[S25] C：内存拷贝
来源：http://baike.vehdjk.com/Article/details/gsljuuoev.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.tarul.cn/Article/details/gdjmjdzuc.sHtML

[S26] C：内存清零
来源：http://baike.yfazqb.com/Article/details/gbojcgvbv.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/gyowowpjp.sHtML

[S27] C：定义常量
来源：http://www.blog.fktsv.cn/Article/details/gbiwentmr.sHtML

const double PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gkejnatxn.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/golzivnxf.sHtML

static int counter = 0;
来源：http://blog.fktsv.cn/Article/details/gsjahpkow.sHtML

[S29] C：变参函数
来源：http://baike.vehdjk.com/Article/details/glmhgpskh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/gjvlvnvqb.sHtML

[S30] C：头文件保护
来源：http://wap.yfazqb.com/Article/details/gmppouxub.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/gibboyqva.sHtML

#define X_H
来源：http://blog.yfazqb.com/Article/details/gnihwbvrl.sHtML

#endif
来源：http://blog.vehdjk.com/Article/details/gsmywdorn.sHtML

[S31] C++：Hello World
来源：http://www.share.vehdjk.com/Article/details/guuhbbvay.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/gsmcelvao.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.epnwcf.com/Article/details/gcjrdplzn.sHtML

[S32] C++：字符串
来源：http://www.blog.bbcook.cn/Article/details/grqlxdlmy.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/gsvyzaqmm.sHtML

[S33] C++：vector 增删
来源：http://wap.fktsv.cn/Article/details/govdkcfov.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.sjlbkw.cn/Article/details/gjhxshnrv.sHtML

[S34] C++：遍历 vector
来源：http://m.share.bbcook.cn/Article/details/gjhalmxsd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.yfazqb.com/Article/details/gvnicfrbl.sHtML

[S35] C++：map
来源：http://mobile.fktsv.cn/Article/details/gaocicpxp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gxxnfkuij.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.epnwcf.com/Article/details/grcjvtwbl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gjhunmzrk.sHtML

[S37] C++：set
来源：http://baike.epnwcf.com/Article/details/gkbgubqds.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.vehdjk.com/Article/details/gkhpslsci.sHtML

[S38] C++：排序
来源：http://blog.bbcook.cn/Article/details/gayruwusk.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.bbcook.cn/Article/details/gtzzkgick.sHtML


<!-- 参考信息 -->