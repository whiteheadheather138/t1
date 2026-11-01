代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gkhirdets.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.bbcook.cn/Article/details/gyohcezjw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.yfazqb.com/Article/details/gammlnuga.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gzvblylsc.sHtML

[Q61] 移动平均
来源：http://www.m.share.fktsv.cn/Article/details/gkysmqegr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.vehdjk.com/Article/details/glmitktyd.sHtML

[Q62] 分组占比
来源：http://baike.tarul.cn/Article/details/gxrorugrx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gjoumdymz.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gtffyyzuq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fktsv.cn/Article/details/gdyzvkexy.sHtML

[Q64] 提交事务
来源：http://www.blog.epnwcf.com/Article/details/gehsotdol.sHtML

COMMIT;
来源：http://blog.epnwcf.com/Article/details/ghcuknoxm.sHtML

[Q65] 回滚事务
来源：http://www.blog.epnwcf.com/Article/details/gsmxyajub.sHtML

ROLLBACK;
来源：http://3g.vehdjk.com/Article/details/gbaucdnkz.sHtML

[Q66] 行锁查询
来源：http://baike.fktsv.cn/Article/details/gzvuhnxtz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.epnwcf.com/Article/details/gxnywdjeb.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhqhemqw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.vehdjk.com/Article/details/ggcftaubj.sHtML

[Q68] 保存点
来源：http://read.share.bbcook.cn/Article/details/gfaethsui.sHtML

SAVEPOINT sp1;
来源：http://read.share.yfazqb.com/Article/details/gkgmbxjjk.sHtML

ROLLBACK TO sp1;
来源：http://mobile.vehdjk.com/Article/details/gfarzdlgs.sHtML

[Q69] 查看执行计划
来源：http://baike.fktsv.cn/Article/details/giyxlbqup.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.bbcook.cn/Article/details/gwecrkwux.sHtML

[Q70] 更新统计信息
来源：http://mobile.tarul.cn/Article/details/gylkblbcf.sHtML

ANALYZE TABLE users;
来源：http://baike.sjlbkw.cn/Article/details/godmgsvwa.sHtML

[Q71] 查看建表语句
来源：http://read.share.epnwcf.com/Article/details/gtatsigal.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.epnwcf.com/Article/details/gkyaglnro.sHtML

[Q72] 查看索引
来源：http://www.m.share.vehdjk.com/Article/details/gmwdipecz.sHtML

SHOW INDEX FROM users;
来源：http://baike.yfazqb.com/Article/details/glsfpnotw.sHtML

[Q73] 查看表状态
来源：http://www.share.tarul.cn/Article/details/ghoamwrau.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.sjlbkw.cn/Article/details/goedcqffl.sHtML

[Q74] 强制使用索引
来源：http://read.share.epnwcf.com/Article/details/gjuybacab.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.sjlbkw.cn/Article/details/gontbniep.sHtML

[Q75] 日期格式化
来源：http://3g.fktsv.cn/Article/details/gnruwmizj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gonnvalir.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.yfazqb.com/Article/details/gnxsxpvqh.sHtML

[Q76] 按天统计
来源：http://read.share.fktsv.cn/Article/details/gfvwczyxt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.epnwcf.com/Article/details/ghbsyshzc.sHtML

[Q77] 时间加减
来源：http://wap.fktsv.cn/Article/details/gzyiheirr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.bbcook.cn/Article/details/geenkbzie.sHtML

[Q78] 当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/goubvhqgr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.bbcook.cn/Article/details/grxhqtibr.sHtML

[Q79] 字符串拼接
来源：http://read.share.epnwcf.com/Article/details/gxazzitvn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.epnwcf.com/Article/details/gdjdmcxah.sHtML

[Q80] 字符串截取
来源：http://wap.fktsv.cn/Article/details/ggrgnyrbs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.epnwcf.com/Article/details/ggatwjyqd.sHtML

[Q81] 字符串替换
来源：http://baike.epnwcf.com/Article/details/gifbdfxtr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.yfazqb.com/Article/details/ggmymdgop.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/gweumkmyo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gaxxcgale.sHtML

[Q83] 大小写转换
来源：http://www.share.tarul.cn/Article/details/glcsogqbo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/glebbmode.sHtML

[Q84] 去除首尾空格
来源：http://3g.yfazqb.com/Article/details/gwwsxluyd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gpmslafsk.sHtML

[Q85] 数值取整
来源：http://www.blog.sjlbkw.cn/Article/details/gnkouhwyt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.bbcook.cn/Article/details/gbaomodzf.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.epnwcf.com/Article/details/gswinqhag.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fktsv.cn/Article/details/ggigdqftl.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fktsv.cn/Article/details/gkzrpjjpn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.yfazqb.com/Article/details/gnaisvhol.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.sjlbkw.cn/Article/details/gzhzopvwp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.vehdjk.com/Article/details/grakaprms.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gncgctjjl.sHtML

[Q89] 判断表是否存在
来源：http://baike.fktsv.cn/Article/details/gegflikwn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/gbyujnjpe.sHtML

[Q90] 生成序号列
来源：http://baike.bbcook.cn/Article/details/grrzjekju.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.tarul.cn/Article/details/gukwoqhlx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpjeoaqut.sHtML

R. Bash 专题
来源：http://mobile.tarul.cn/Article/details/gydeaxgjp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzfkyxtuo.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/gyvtebepv.sHtML

#!/usr/bin/env bash
来源：http://m.share.sjlbkw.cn/Article/details/ggwkmgbvt.sHtML

set -euo pipefail
来源：http://3g.fktsv.cn/Article/details/galphellx.sHtML

[R02] 变量赋值与使用
来源：http://3g.yfazqb.com/Article/details/gdrpqxxyr.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.epnwcf.com/Article/details/gikcylfli.sHtML

[R03] 只读变量
来源：http://www.m.share.tarul.cn/Article/details/gcsxurcig.sHtML

readonly PI=3.14
来源：http://www.share.yfazqb.com/Article/details/gqeexbmnd.sHtML

[R04] 位置参数
来源：http://baike.tarul.cn/Article/details/girdaoorb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gjpqbjkkj.sHtML

[R05] 参数默认值
来源：http://www.blog.tarul.cn/Article/details/gexoxtxdh.sHtML

name="${1:-default}"
来源：http://mobile.tarul.cn/Article/details/gxsrojtda.sHtML

[R06] 判断命令是否存在
来源：http://wap.vehdjk.com/Article/details/gzrqauxzj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gtcounjba.sHtML

[R07] if 判断文件
来源：http://www.share.tarul.cn/Article/details/gimpnfzmx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.bbcook.cn/Article/details/ghyklnckg.sHtML

[R08] 数值比较
来源：http://baike.vehdjk.com/Article/details/ghpjxkoot.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.vehdjk.com/Article/details/gavppfeyp.sHtML

[R09] 字符串比较
来源：http://mobile.tarul.cn/Article/details/gyfionzcp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/gptbgnmzo.sHtML

[R10] 正则匹配
来源：http://www.m.share.bbcook.cn/Article/details/gzccmllct.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gwacsducg.sHtML

[R11] case 多分支
来源：http://read.share.fktsv.cn/Article/details/ghstjmseg.sHtML

case "$1" in
来源：http://blog.fktsv.cn/Article/details/gsctmjcot.sHtML

start) echo "启动" ;;
来源：http://wap.yfazqb.com/Article/details/guancqkom.sHtML

stop)  echo "停止" ;;
来源：http://www.share.epnwcf.com/Article/details/grqhoosid.sHtML

*)     echo "未知命令" ;;
来源：http://blog.yfazqb.com/Article/details/gpdotjeku.sHtML

esac
来源：http://wap.fktsv.cn/Article/details/glhnrabmd.sHtML

[R12] for 遍历文件
来源：http://baike.fktsv.cn/Article/details/gqejgjwjy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.vehdjk.com/Article/details/gqayuhywe.sHtML

[R13] for 计数循环
来源：http://blog.tarul.cn/Article/details/gmhcqhvlq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/grcvbjdfj.sHtML

[R14] C 风格 for
来源：http://www.blog.epnwcf.com/Article/details/gqyperwok.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/gpbkzmghr.sHtML

[R15] while 逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gietevysf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.vehdjk.com/Article/details/gjxxmwlli.sHtML

[R16] until 等待条件
来源：http://read.share.bbcook.cn/Article/details/gdpebylbk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gmrmhedcb.sHtML

[R17] 数组定义与取值
来源：http://blog.fktsv.cn/Article/details/gyijbnjow.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.sjlbkw.cn/Article/details/gttzypuaf.sHtML

[R18] 遍历数组
来源：http://mobile.sjlbkw.cn/Article/details/gnrqfgqzb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fktsv.cn/Article/details/gbqufoklz.sHtML

[R19] 数组长度
来源：http://wap.tarul.cn/Article/details/goqtlwpid.sHtML

echo "${#arr[@]}"
来源：http://baike.sjlbkw.cn/Article/details/gnjkjdfzf.sHtML

[R20] 关联数组（字典）
来源：http://wap.yfazqb.com/Article/details/gzfggtcmq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.bbcook.cn/Article/details/gzvytnsow.sHtML

[R21] 字符串长度
来源：http://m.share.yfazqb.com/Article/details/gwhuawilo.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/gsdnfuycs.sHtML

[R22] 截取子串
来源：http://3g.bbcook.cn/Article/details/gpvxlenqn.sHtML

echo "${s:0:5}"
来源：http://baike.yfazqb.com/Article/details/gfzknrzal.sHtML

[R23] 字符串替换
来源：http://3g.vehdjk.com/Article/details/glvnrkmmh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.sjlbkw.cn/Article/details/gzuyaoxgi.sHtML

[R24] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gjextjfli.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.epnwcf.com/Article/details/gsfijvwwm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gpuvhhnfc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/ggucpwvds.sHtML

[R26] 命令替换
来源：http://www.m.share.bbcook.cn/Article/details/gszekigox.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.vehdjk.com/Article/details/ghvzszeqo.sHtML

[R27] 算术展开
来源：http://wap.sjlbkw.cn/Article/details/grkijkhpg.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fktsv.cn/Article/details/gfobayzxk.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gqxbrkimz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.vehdjk.com/Article/details/gqsudddnu.sHtML

[R29] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gxycpbzdh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fktsv.cn/Article/details/gawmtwzwb.sHtML

[R30] 函数返回状态码
来源：http://3g.vehdjk.com/Article/details/gzzhuhqnc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/gajhcjert.sHtML

[R31] 局部变量
来源：http://m.share.epnwcf.com/Article/details/guyvsvcgs.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.sjlbkw.cn/Article/details/gpkmnzpkr.sHtML

[R32] 参数个数校验
来源：http://blog.tarul.cn/Article/details/ggpowxooy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gxenxjkzq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.sjlbkw.cn/Article/details/grugpqebd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.sjlbkw.cn/Article/details/gtsdbftyc.sHtML

[R34] 退出时清理
来源：http://3g.tarul.cn/Article/details/gvxfyxulb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gxmtmxpfa.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/gtsnyffzc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.vehdjk.com/Article/details/gqgksqrqq.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/gqgzpyaem.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.bbcook.cn/Article/details/gyyuvkruy.sHtML

[R37] 把输出赋给变量
来源：http://mobile.sjlbkw.cn/Article/details/gooxnnhpl.sHtML

files=$(ls -1)
来源：http://mobile.vehdjk.com/Article/details/ghswaycva.sHtML

[R38] 管道串联
来源：http://www.blog.yfazqb.com/Article/details/gdeufttbr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.vehdjk.com/Article/details/ghuucuole.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/gznhgkhqq.sHtML

cmd > out.log 2>&1
来源：http://wap.fktsv.cn/Article/details/gogxtvhaa.sHtML

[R40] 追加写日志
来源：http://m.share.yfazqb.com/Article/details/gtgopwily.sHtML

echo "log" >> out.log
来源：http://wap.yfazqb.com/Article/details/glkdbvaol.sHtML

[R41] 丢弃输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhlzoizv.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gucwfkxgq.sHtML

[R42] 输入重定向
来源：http://www.blog.epnwcf.com/Article/details/gtgnhtlud.sHtML

wc -l < a.txt
来源：http://wap.vehdjk.com/Article/details/ggbzojqto.sHtML

[R43] 按名字查找文件
来源：http://3g.yfazqb.com/Article/details/guffteqqm.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gjwgmsfls.sHtML

[R44] 按修改时间查找
来源：http://wap.vehdjk.com/Article/details/gsbxoozuf.sHtML

find . -mtime -7 -type f
来源：http://wap.yfazqb.com/Article/details/gamwgaugx.sHtML

[R45] 批量删除
来源：http://mobile.fktsv.cn/Article/details/gtuqzqvmm.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/gftpijvyz.sHtML

[R46] 递归替换文件内容
来源：http://read.share.tarul.cn/Article/details/gyfyvfohs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.vehdjk.com/Article/details/gosshdhyq.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/gequhshsl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gnhksator.sHtML

[R48] awk 取指定列
来源：http://mobile.fktsv.cn/Article/details/gaqnbirba.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.yfazqb.com/Article/details/gvcilgzrk.sHtML

[R49] awk 带条件
来源：http://3g.tarul.cn/Article/details/gddjsgwqc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.epnwcf.com/Article/details/gfpnenqlt.sHtML

[R50] awk 求和
来源：http://baike.fktsv.cn/Article/details/gzgmriccz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gagxjhwbc.sHtML

[R51] 排序去重取前几
来源：http://www.blog.vehdjk.com/Article/details/gxyasstgt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.tarul.cn/Article/details/gimevgmbo.sHtML

[R52] 统计行数
来源：http://mobile.tarul.cn/Article/details/griwgohll.sHtML

wc -l a.txt
来源：http://www.blog.epnwcf.com/Article/details/gtkewhhvi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gtteyggac.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.vehdjk.com/Article/details/gpniqrzzw.sHtML

[R54] 比较两个文件
来源：http://blog.vehdjk.com/Article/details/gjxlhvnjk.sHtML

diff a.txt b.txt
来源：http://m.share.yfazqb.com/Article/details/glnpwfifg.sHtML

[R55] 压缩与解压
来源：http://mobile.yfazqb.com/Article/details/gkbqtmrsm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.epnwcf.com/Article/details/gtdeurcsb.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/gbwgcophb.sHtML

scp file user@host:/path/
来源：http://blog.fktsv.cn/Article/details/gtycdfgzi.sHtML

[R57] 远程执行命令
来源：http://www.blog.vehdjk.com/Article/details/gpimecgok.sHtML

ssh user@host 'uptime'
来源：http://mobile.sjlbkw.cn/Article/details/gshludowg.sHtML

[R58] 下载文件
来源：http://wap.vehdjk.com/Article/details/gzlrsuxjt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.yfazqb.com/Article/details/gzmxekjig.sHtML

[R59] 发 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gzbyaeyne.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.yfazqb.com/Article/details/gulrayhjm.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gzgzgfoze.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fktsv.cn/Article/details/gywffoafi.sHtML

[R61] 磁盘占用
来源：http://read.share.bbcook.cn/Article/details/gtqtklpbx.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/gcmymcfio.sHtML

[R62] 找最占空间的文件
来源：http://mobile.bbcook.cn/Article/details/gokbhrpla.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.vehdjk.com/Article/details/gbslnmskv.sHtML

[R63] 内存与进程
来源：http://m.share.tarul.cn/Article/details/gmqbeabje.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.bbcook.cn/Article/details/gfhwffhyp.sHtML

[R64] 结束进程
来源：http://www.m.share.bbcook.cn/Article/details/gsswpdfgs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fktsv.cn/Article/details/gwmbhpfkt.sHtML

[R65] 查看端口占用
来源：http://3g.yfazqb.com/Article/details/gzxepidqm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.yfazqb.com/Article/details/gwhqxemil.sHtML

[R66] 定时任务
来源：http://mobile.bbcook.cn/Article/details/gujeujipf.sHtML

crontab -e;  crontab -l
来源：http://mobile.yfazqb.com/Article/details/gpeamattv.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.epnwcf.com/Article/details/gdcvhouoo.sHtML

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/gxabrojmz.sHtML

[R68] 计算文件校验值
来源：http://3g.tarul.cn/Article/details/gbqnrvjza.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gxokhkmai.sHtML

[R69] 生成随机密码
来源：http://read.share.epnwcf.com/Article/details/giirvkqaq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.yfazqb.com/Article/details/gyavjikgy.sHtML

[R70] 时间戳与互转
来源：http://blog.vehdjk.com/Article/details/ggpkuwniw.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fktsv.cn/Article/details/gbjhtquds.sHtML

[R71] 日期格式化
来源：http://www.share.tarul.cn/Article/details/grznwphpt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gebodjbsy.sHtML

[R72] 等待端口就绪
来源：http://baike.tarul.cn/Article/details/gbvcirrsb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gouxlsbcq.sHtML

[R73] 分割大日志
来源：http://blog.vehdjk.com/Article/details/gwrnnrexs.sHtML

split -l 1000 big.log part_
来源：http://baike.epnwcf.com/Article/details/gjqgmxixt.sHtML

[R74] 批量重命名
来源：http://www.m.share.bbcook.cn/Article/details/ghzqcvfqi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.bbcook.cn/Article/details/gurljtpgm.sHtML

[R75] 导出环境变量
来源：http://mobile.yfazqb.com/Article/details/gbximwlue.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.bbcook.cn/Article/details/gylkjibqa.sHtML

[R76] 使用临时文件
来源：http://baike.vehdjk.com/Article/details/gkogpskmn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gvcetlhmk.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/gxadeppxh.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/gpaoxyrkd.sHtML

[R78] 交互式菜单
来源：http://m.share.yfazqb.com/Article/details/ggvvlkshr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.sjlbkw.cn/Article/details/ghvijsdgc.sHtML

[R79] 解析命令行选项
来源：http://3g.tarul.cn/Article/details/gcisybuid.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.bbcook.cn/Article/details/gjmtlqbbn.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.vehdjk.com/Article/details/gusmrknar.sHtML

time ./run.sh
来源：http://www.share.fktsv.cn/Article/details/geszspjim.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxzgdfrqg.sHtML

S. C / C++ 专题
来源：http://www.m.share.yfazqb.com/Article/details/guzbtlikg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gkwpnxvas.sHtML

[S01] C：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gsbbyztmx.sHtML

#include <stdio.h>
来源：http://www.blog.epnwcf.com/Article/details/gtslpjvje.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.bbcook.cn/Article/details/glhjydfoj.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gptpmdiqe.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.vehdjk.com/Article/details/gbtmmkzmg.sHtML

[S03] C：读入整数
来源：http://www.m.share.fktsv.cn/Article/details/gfuyhcwvo.sHtML

int x; scanf("%d", &x);
来源：http://www.share.tarul.cn/Article/details/gcbgrqbdv.sHtML

[S04] C：字符串复制
来源：http://mobile.bbcook.cn/Article/details/gqbuwxffb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gdqhcgksm.sHtML

[S05] C：字符串长度
来源：http://read.share.bbcook.cn/Article/details/gzwnatemf.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/ggtmymfpr.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/glkpecjxx.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.yfazqb.com/Article/details/guqkgqiab.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.yfazqb.com/Article/details/gcdemvtkx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.sjlbkw.cn/Article/details/gifdhrszj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/gehruqolc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.yfazqb.com/Article/details/gpabrjtsp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.yfazqb.com/Article/details/gyebwrjsg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fktsv.cn/Article/details/guczcjagp.sHtML

[S10] C：指针与解引用
来源：http://blog.tarul.cn/Article/details/gjncemqbk.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.yfazqb.com/Article/details/gwclgegsm.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gikjvqoxd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.bbcook.cn/Article/details/giruimdes.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.bbcook.cn/Article/details/gdnxrgsdt.sHtML

fclose(f);
来源：http://baike.yfazqb.com/Article/details/gjcwofbxj.sHtML

[S12] C：写文件
来源：http://mobile.yfazqb.com/Article/details/gwknfjfxp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.vehdjk.com/Article/details/gvymnrgxc.sHtML

[S13] C：宏定义
来源：http://www.share.tarul.cn/Article/details/gpzwuzwfi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.epnwcf.com/Article/details/gtuqvkvmu.sHtML

[S14] C：枚举
来源：http://m.share.fktsv.cn/Article/details/gahhcvqzo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.yfazqb.com/Article/details/gthahmllk.sHtML

[S15] C：类型转换
来源：http://m.share.bbcook.cn/Article/details/grkjqteni.sHtML

(double) a / b
来源：http://read.share.epnwcf.com/Article/details/gfqnsskbg.sHtML

[S16] C：位操作置位
来源：http://m.share.yfazqb.com/Article/details/grpsahrby.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/gvjdybeor.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gmifbkass.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.bbcook.cn/Article/details/gleezkign.sHtML

[S18] C：命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gqcwgfdzg.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/gbrbcaojv.sHtML

[S19] C：快速排序
来源：http://blog.fktsv.cn/Article/details/getoodcon.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/gzimsivea.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/ghvdzyzsm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/gnzoicxox.sHtML

[S21] C：字符类别判断
来源：http://3g.epnwcf.com/Article/details/gmbepnchz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.bbcook.cn/Article/details/grjbruttk.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/glosphxxk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.sjlbkw.cn/Article/details/gzvsqlnce.sHtML

[S23] C：随机数
来源：http://3g.fktsv.cn/Article/details/gntzbodee.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/gtfgosity.sHtML

[S24] C：获取本地时间
来源：http://www.share.sjlbkw.cn/Article/details/gnhpmnazm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.yfazqb.com/Article/details/grdqbybgn.sHtML

[S25] C：内存拷贝
来源：http://3g.tarul.cn/Article/details/ghdqwfxkm.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.yfazqb.com/Article/details/gxqliwzhh.sHtML

[S26] C：内存清零
来源：http://wap.yfazqb.com/Article/details/ggxuhvfwu.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.bbcook.cn/Article/details/gwylbrmlc.sHtML

[S27] C：定义常量
来源：http://mobile.fktsv.cn/Article/details/gyjhybwhx.sHtML

const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gtkjnpzkh.sHtML

[S28] C：静态变量
来源：http://mobile.vehdjk.com/Article/details/gnyubopml.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/gxwectluf.sHtML

[S29] C：变参函数
来源：http://www.blog.yfazqb.com/Article/details/gkcjhjdwi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.bbcook.cn/Article/details/gogadsdht.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/gvvhupfsp.sHtML


<!-- 参考信息 -->