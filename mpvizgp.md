代发 wailian999

[Q61] 移动平均
来源：http://read.share.bbcook.cn/Article/details/gqecqqjnp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.yfazqb.com/Article/details/garspufyw.sHtML

[Q62] 分组占比
来源：http://baike.epnwcf.com/Article/details/gexonivym.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/ghueksckv.sHtML

[Q63] 开启事务
来源：http://mobile.vehdjk.com/Article/details/gddtrbpts.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fktsv.cn/Article/details/gcboczywy.sHtML

[Q64] 提交事务
来源：http://mobile.yfazqb.com/Article/details/gsmvtwdsx.sHtML

COMMIT;
来源：http://mobile.bbcook.cn/Article/details/gyfdkambb.sHtML

[Q65] 回滚事务
来源：http://baike.fktsv.cn/Article/details/ghfeprego.sHtML

ROLLBACK;
来源：http://www.m.share.bbcook.cn/Article/details/gaeoldslc.sHtML

[Q66] 行锁查询
来源：http://3g.yfazqb.com/Article/details/ghowgfkai.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.yfazqb.com/Article/details/grffxcjtu.sHtML

[Q67] 设置隔离级别
来源：http://blog.sjlbkw.cn/Article/details/gburdihnf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fktsv.cn/Article/details/gvcdziuno.sHtML

[Q68] 保存点
来源：http://read.share.fktsv.cn/Article/details/gepbyhvrk.sHtML

SAVEPOINT sp1;
来源：http://3g.tarul.cn/Article/details/ghplkavsb.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.yfazqb.com/Article/details/gmmcugxeu.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.vehdjk.com/Article/details/gpscitkru.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.sjlbkw.cn/Article/details/gyhxggfth.sHtML

[Q70] 更新统计信息
来源：http://www.blog.sjlbkw.cn/Article/details/gekergnur.sHtML

ANALYZE TABLE users;
来源：http://mobile.tarul.cn/Article/details/gxpdtdjqf.sHtML

[Q71] 查看建表语句
来源：http://read.share.yfazqb.com/Article/details/gyglghgxs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.tarul.cn/Article/details/gggjohmpw.sHtML

[Q72] 查看索引
来源：http://m.share.fktsv.cn/Article/details/gvasrjzrc.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gzlxzoork.sHtML

[Q73] 查看表状态
来源：http://blog.fktsv.cn/Article/details/gdmgzvgpb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fktsv.cn/Article/details/ggppjeegs.sHtML

[Q74] 强制使用索引
来源：http://blog.tarul.cn/Article/details/gttfmzeen.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fktsv.cn/Article/details/gxagoaecd.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/grxniqvqb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/gbtjyhkok.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.epnwcf.com/Article/details/gxekogzsy.sHtML

[Q76] 按天统计
来源：http://3g.bbcook.cn/Article/details/gjpajbjix.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/gqijhkvpz.sHtML

[Q77] 时间加减
来源：http://baike.sjlbkw.cn/Article/details/gogbiwiea.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.epnwcf.com/Article/details/gpcdczlcf.sHtML

[Q78] 当前时间
来源：http://read.share.fktsv.cn/Article/details/grqvfhmsb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.yfazqb.com/Article/details/glywgormy.sHtML

[Q79] 字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gdpnmzqfm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fktsv.cn/Article/details/guetjshej.sHtML

[Q80] 字符串截取
来源：http://www.m.share.vehdjk.com/Article/details/gznulvkwl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gutaqrfsh.sHtML

[Q81] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/gydrqijyv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gvzuewxup.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/gvobhubtv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gtmjzyqbk.sHtML

[Q83] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gohkpzohw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/ghsfxoxwz.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.vehdjk.com/Article/details/ghafdzbzv.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gfqnosywd.sHtML

[Q85] 数值取整
来源：http://www.m.share.epnwcf.com/Article/details/ggnthpfui.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.yfazqb.com/Article/details/gvznpstpd.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.tarul.cn/Article/details/grozthxay.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.tarul.cn/Article/details/ghfqtfxmg.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fktsv.cn/Article/details/gflnilhms.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.epnwcf.com/Article/details/gyzqythdl.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.vehdjk.com/Article/details/gvzhjdlse.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.sjlbkw.cn/Article/details/gmgggfilh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gxbamawzr.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fktsv.cn/Article/details/gwocmpamt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.yfazqb.com/Article/details/gizqjmlun.sHtML

[Q90] 生成序号列
来源：http://mobile.vehdjk.com/Article/details/gglfklsok.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.vehdjk.com/Article/details/gsggegcxf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gzdzvrltm.sHtML

R. Bash 专题
来源：http://3g.fktsv.cn/Article/details/ggbrotrrq.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gypgytrqz.sHtML

[R01] shebang 与严格模式
来源：http://blog.bbcook.cn/Article/details/gmkdcrpsi.sHtML

#!/usr/bin/env bash
来源：http://3g.sjlbkw.cn/Article/details/gkcjkmvhm.sHtML

set -euo pipefail
来源：http://3g.yfazqb.com/Article/details/gadvfazll.sHtML

[R02] 变量赋值与使用
来源：http://3g.sjlbkw.cn/Article/details/ghjggmuxe.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/gbeaxdhog.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/goddooeri.sHtML

readonly PI=3.14
来源：http://www.share.vehdjk.com/Article/details/gurhlvpkh.sHtML

[R04] 位置参数
来源：http://read.share.sjlbkw.cn/Article/details/gzzutbkyt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.tarul.cn/Article/details/guozioppt.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gsqdfckyz.sHtML

name="${1:-default}"
来源：http://m.share.epnwcf.com/Article/details/glriujihj.sHtML

[R06] 判断命令是否存在
来源：http://mobile.tarul.cn/Article/details/ghhdcqymx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/glmzshmgr.sHtML

[R07] if 判断文件
来源：http://wap.epnwcf.com/Article/details/gvtovfnpj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.bbcook.cn/Article/details/gktkslxeu.sHtML

[R08] 数值比较
来源：http://blog.bbcook.cn/Article/details/gsyabiesb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.tarul.cn/Article/details/gpdfoxxww.sHtML

[R09] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gksdfhtjs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.yfazqb.com/Article/details/gwwzigezr.sHtML

[R10] 正则匹配
来源：http://mobile.fktsv.cn/Article/details/gewiewkwn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.epnwcf.com/Article/details/gcvesxeyo.sHtML

[R11] case 多分支
来源：http://read.share.epnwcf.com/Article/details/gnubulrle.sHtML

case "$1" in
来源：http://www.share.sjlbkw.cn/Article/details/gcuqhhhnh.sHtML

start) echo "启动" ;;
来源：http://www.share.vehdjk.com/Article/details/gqtwboton.sHtML

stop)  echo "停止" ;;
来源：http://mobile.vehdjk.com/Article/details/gmswbraij.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.tarul.cn/Article/details/gjhzfelfj.sHtML

esac
来源：http://m.share.fktsv.cn/Article/details/grxcsxwdo.sHtML

[R12] for 遍历文件
来源：http://mobile.tarul.cn/Article/details/guehtbvuw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzipdawq.sHtML

[R13] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/geineejmi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/gtobuznij.sHtML

[R14] C 风格 for
来源：http://wap.vehdjk.com/Article/details/gagkuvgvk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gkctznwah.sHtML

[R15] while 逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gftckklcg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.bbcook.cn/Article/details/gcttphvsq.sHtML

[R16] until 等待条件
来源：http://www.blog.fktsv.cn/Article/details/gmyxenvqa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.vehdjk.com/Article/details/gymtkmkes.sHtML

[R17] 数组定义与取值
来源：http://www.blog.tarul.cn/Article/details/gsdxhcswy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.tarul.cn/Article/details/grmicyydf.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/grfalwonq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.epnwcf.com/Article/details/gxprmgqaa.sHtML

[R19] 数组长度
来源：http://read.share.tarul.cn/Article/details/gvymdskde.sHtML

echo "${#arr[@]}"
来源：http://3g.sjlbkw.cn/Article/details/gpyeajros.sHtML

[R20] 关联数组（字典）
来源：http://wap.vehdjk.com/Article/details/gzjhjgpda.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.epnwcf.com/Article/details/goedaeemm.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/gmkegnvgv.sHtML

echo "${#s}"
来源：http://3g.sjlbkw.cn/Article/details/gdstxsvjf.sHtML

[R22] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjnzqryt.sHtML

echo "${s:0:5}"
来源：http://baike.yfazqb.com/Article/details/gusilayvw.sHtML

[R23] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gcakyatpb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.epnwcf.com/Article/details/gxfytolsa.sHtML

[R24] 大小写转换
来源：http://wap.yfazqb.com/Article/details/guewinufi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.tarul.cn/Article/details/gftewfmxt.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.yfazqb.com/Article/details/gjycnclcp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.sjlbkw.cn/Article/details/gipxjjyuk.sHtML

[R26] 命令替换
来源：http://wap.epnwcf.com/Article/details/gzbflvjlr.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.epnwcf.com/Article/details/gczttwqqc.sHtML

[R27] 算术展开
来源：http://wap.epnwcf.com/Article/details/grbszowrg.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gywxvkptl.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/gdboiqqyi.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/gpaejbcim.sHtML

[R29] 定义函数
来源：http://www.share.bbcook.cn/Article/details/gtcmnakvw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.yfazqb.com/Article/details/gemgnlqcr.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gurknkdtq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.tarul.cn/Article/details/gkspzlftk.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gjkzhpiix.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.bbcook.cn/Article/details/gfheyhnxn.sHtML

[R32] 参数个数校验
来源：http://blog.bbcook.cn/Article/details/gcktjjfnx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.vehdjk.com/Article/details/getowpmgl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.yfazqb.com/Article/details/gfmyjncwa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.yfazqb.com/Article/details/gzsyrruci.sHtML

[R34] 退出时清理
来源：http://baike.bbcook.cn/Article/details/gyhlzgbqv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/gpbnctgie.sHtML

[R35] 后台执行并等待
来源：http://3g.vehdjk.com/Article/details/geqbkmqih.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.epnwcf.com/Article/details/guqoludlp.sHtML

[R36] 并发执行多个任务
来源：http://wap.vehdjk.com/Article/details/gsxznwkci.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/gxfgwqein.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.sjlbkw.cn/Article/details/gwslegfeo.sHtML

files=$(ls -1)
来源：http://blog.yfazqb.com/Article/details/gjrgmkwqm.sHtML

[R38] 管道串联
来源：http://www.share.vehdjk.com/Article/details/gbtwitbsh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.vehdjk.com/Article/details/gosaohtfu.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.tarul.cn/Article/details/gnngkrxek.sHtML

cmd > out.log 2>&1
来源：http://read.share.bbcook.cn/Article/details/gcbjcglms.sHtML

[R40] 追加写日志
来源：http://read.share.yfazqb.com/Article/details/grxzresst.sHtML

echo "log" >> out.log
来源：http://mobile.yfazqb.com/Article/details/gukmvrqsl.sHtML

[R41] 丢弃输出
来源：http://wap.fktsv.cn/Article/details/gsrnbnufd.sHtML

cmd >/dev/null 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gjqjurjmp.sHtML

[R42] 输入重定向
来源：http://read.share.fktsv.cn/Article/details/gvcrwhbfm.sHtML

wc -l < a.txt
来源：http://mobile.vehdjk.com/Article/details/gtpazwnoq.sHtML

[R43] 按名字查找文件
来源：http://m.share.yfazqb.com/Article/details/gzedefjrf.sHtML

find . -name "*.log" -type f
来源：http://baike.vehdjk.com/Article/details/gobhttydg.sHtML

[R44] 按修改时间查找
来源：http://wap.bbcook.cn/Article/details/gnckfkkam.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.sjlbkw.cn/Article/details/gflsfhqnc.sHtML

[R45] 批量删除
来源：http://3g.epnwcf.com/Article/details/gxdcbeixr.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fktsv.cn/Article/details/gihqnxtzf.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gofqhtqpf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.sjlbkw.cn/Article/details/guutsigbd.sHtML

[R47] sed 单行替换
来源：http://www.blog.yfazqb.com/Article/details/gtkvckcaq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gkcxmpamh.sHtML

[R48] awk 取指定列
来源：http://baike.bbcook.cn/Article/details/gidbebaes.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gajxwqfez.sHtML

[R49] awk 带条件
来源：http://mobile.yfazqb.com/Article/details/gxveuofaz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.tarul.cn/Article/details/ghlnueabd.sHtML

[R50] awk 求和
来源：http://3g.yfazqb.com/Article/details/gayxgscyu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfzdvgqe.sHtML

[R51] 排序去重取前几
来源：http://blog.vehdjk.com/Article/details/gsvdtpdrd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.tarul.cn/Article/details/gdwjsecrr.sHtML

[R52] 统计行数
来源：http://m.share.fktsv.cn/Article/details/gocrwwatw.sHtML

wc -l a.txt
来源：http://wap.epnwcf.com/Article/details/glusczjki.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.tarul.cn/Article/details/gqxwprboy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.sjlbkw.cn/Article/details/gnftnfgnp.sHtML

[R54] 比较两个文件
来源：http://wap.fktsv.cn/Article/details/gdwgttxmz.sHtML

diff a.txt b.txt
来源：http://3g.fktsv.cn/Article/details/grwdnewja.sHtML

[R55] 压缩与解压
来源：http://www.m.share.vehdjk.com/Article/details/gzovzrcdq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.vehdjk.com/Article/details/gorodevwh.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/gczbyrekv.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gvqdzxmkn.sHtML

[R57] 远程执行命令
来源：http://wap.yfazqb.com/Article/details/gjutjkqfi.sHtML

ssh user@host 'uptime'
来源：http://wap.sjlbkw.cn/Article/details/gybmocbvm.sHtML

[R58] 下载文件
来源：http://www.share.epnwcf.com/Article/details/gppdawxag.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fktsv.cn/Article/details/gwtiqbrpc.sHtML

[R59] 发 POST JSON
来源：http://m.share.yfazqb.com/Article/details/gbfqqrjtj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/gfvcnlctj.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.sjlbkw.cn/Article/details/gdztdyiip.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.yfazqb.com/Article/details/gqzamxdnb.sHtML

[R61] 磁盘占用
来源：http://www.share.sjlbkw.cn/Article/details/gwomuqnkv.sHtML

df -h;  du -sh *
来源：http://baike.epnwcf.com/Article/details/gzmrbznzr.sHtML

[R62] 找最占空间的文件
来源：http://baike.epnwcf.com/Article/details/gbeshvkcf.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.vehdjk.com/Article/details/gzmqknjnj.sHtML

[R63] 内存与进程
来源：http://mobile.bbcook.cn/Article/details/gtylxqzmg.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.vehdjk.com/Article/details/grqpyirku.sHtML

[R64] 结束进程
来源：http://mobile.fktsv.cn/Article/details/gmirlhfue.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.epnwcf.com/Article/details/gynpbguhe.sHtML

[R65] 查看端口占用
来源：http://www.blog.yfazqb.com/Article/details/gmidvefcb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.epnwcf.com/Article/details/gxqnrgxxx.sHtML

[R66] 定时任务
来源：http://3g.sjlbkw.cn/Article/details/gvraqzvgo.sHtML

crontab -e;  crontab -l
来源：http://mobile.fktsv.cn/Article/details/gfwqihkii.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.epnwcf.com/Article/details/gzojvyore.sHtML

openssl rand -hex 16
来源：http://read.share.sjlbkw.cn/Article/details/guxzerjbh.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/gipawzakj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.yfazqb.com/Article/details/grmgweejo.sHtML

[R69] 生成随机密码
来源：http://baike.yfazqb.com/Article/details/ghlckeseh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.yfazqb.com/Article/details/gbexscqaf.sHtML

[R70] 时间戳与互转
来源：http://read.share.yfazqb.com/Article/details/goiavcudo.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/gfdtxophz.sHtML

[R71] 日期格式化
来源：http://baike.bbcook.cn/Article/details/geyfhpwsw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.epnwcf.com/Article/details/gnnesqgaa.sHtML

[R72] 等待端口就绪
来源：http://mobile.fktsv.cn/Article/details/gwdnczdyq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gjgxdcebl.sHtML

[R73] 分割大日志
来源：http://www.m.share.vehdjk.com/Article/details/gbjbymvni.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/grvrsdwmr.sHtML

[R74] 批量重命名
来源：http://blog.bbcook.cn/Article/details/ggnwgdcnw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/goxtttkjc.sHtML

[R75] 导出环境变量
来源：http://m.share.tarul.cn/Article/details/guksyfslz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.bbcook.cn/Article/details/gkwcyqgsw.sHtML

[R76] 使用临时文件
来源：http://m.share.sjlbkw.cn/Article/details/gwunttsnr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/gmwxldeib.sHtML

[R77] 读取用户输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gpahxbnac.sHtML

read -rp "请输入: " ans
来源：http://blog.vehdjk.com/Article/details/ghqhzgztg.sHtML

[R78] 交互式菜单
来源：http://mobile.yfazqb.com/Article/details/gymgyrmsz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.yfazqb.com/Article/details/gucpktrcn.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gvektzqik.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.vehdjk.com/Article/details/gfdyfsplb.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.tarul.cn/Article/details/gzbqmuvxd.sHtML

time ./run.sh
来源：http://wap.fktsv.cn/Article/details/gwwipylkx.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmzpghngy.sHtML

S. C / C++ 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gtsaolnrk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxjkpvbmg.sHtML

[S01] C：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gsheyqqfu.sHtML

#include <stdio.h>
来源：http://www.m.share.vehdjk.com/Article/details/ghspirrlh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fktsv.cn/Article/details/gfggfrvko.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gemppyjsk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gwfytyvqr.sHtML

[S03] C：读入整数
来源：http://www.blog.epnwcf.com/Article/details/gdudjrlnm.sHtML

int x; scanf("%d", &x);
来源：http://www.share.bbcook.cn/Article/details/gdzvvtczv.sHtML

[S04] C：字符串复制
来源：http://read.share.bbcook.cn/Article/details/gatjohgbt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.yfazqb.com/Article/details/gpkskcebf.sHtML

[S05] C：字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gfotvynlh.sHtML

strlen(s)
来源：http://blog.tarul.cn/Article/details/ggeietnnx.sHtML

[S06] C：字符串比较
来源：http://mobile.fktsv.cn/Article/details/gmnjpkpno.sHtML

strcmp(a, b) == 0
来源：http://www.share.tarul.cn/Article/details/guokdfamg.sHtML

[S07] C：数组遍历求和
来源：http://read.share.vehdjk.com/Article/details/gkiyizhir.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gcqiaqtju.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fktsv.cn/Article/details/giqzzivqp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.sjlbkw.cn/Article/details/gnunxcjjc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.sjlbkw.cn/Article/details/glntniryj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.yfazqb.com/Article/details/gmtlqpkno.sHtML

[S10] C：指针与解引用
来源：http://blog.tarul.cn/Article/details/gijdhbauk.sHtML

int *p = &a;  *p = 5;
来源：http://blog.tarul.cn/Article/details/gzlccrdfg.sHtML

[S11] C：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/goexczwdu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.vehdjk.com/Article/details/gsbzbxtau.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.yfazqb.com/Article/details/gvgnbteky.sHtML

fclose(f);
来源：http://www.blog.tarul.cn/Article/details/glbfffybd.sHtML

[S12] C：写文件
来源：http://baike.yfazqb.com/Article/details/gbqektpfs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gmewoxvre.sHtML

[S13] C：宏定义
来源：http://m.share.fktsv.cn/Article/details/gfyujdfec.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.bbcook.cn/Article/details/gxtbbjnxv.sHtML

[S14] C：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gciybgxsv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.bbcook.cn/Article/details/glzojpnvk.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/gdfkajrzx.sHtML

(double) a / b
来源：http://m.share.bbcook.cn/Article/details/gzvdlezex.sHtML

[S16] C：位操作置位
来源：http://www.m.share.vehdjk.com/Article/details/gvfpmnhjl.sHtML

x |= (1 << 3);
来源：http://3g.fktsv.cn/Article/details/gomuzdyih.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/ghyrulzam.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/gmjjibbxa.sHtML

[S18] C：命令行参数
来源：http://blog.vehdjk.com/Article/details/glbvdmweh.sHtML

int main(int argc, char **argv)
来源：http://www.blog.tarul.cn/Article/details/gbcxbsxzq.sHtML

[S19] C：快速排序
来源：http://wap.bbcook.cn/Article/details/goadfjycw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/gwrmwkcry.sHtML

[S20] C：二分查找
来源：http://baike.sjlbkw.cn/Article/details/gxndymebf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gxfhiwhoq.sHtML

[S21] C：字符类别判断
来源：http://read.share.sjlbkw.cn/Article/details/giwoshnix.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.vehdjk.com/Article/details/gyqytlkkt.sHtML

[S22] C：字符串转数字
来源：http://baike.vehdjk.com/Article/details/gpdqwiemv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fktsv.cn/Article/details/gumcivbad.sHtML

[S23] C：随机数
来源：http://baike.epnwcf.com/Article/details/gyjtrlkdl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.yfazqb.com/Article/details/gsjsoyzmp.sHtML

[S24] C：获取本地时间
来源：http://m.share.yfazqb.com/Article/details/gwvurtdad.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.bbcook.cn/Article/details/guinjymab.sHtML

[S25] C：内存拷贝
来源：http://baike.fktsv.cn/Article/details/gcueqeemm.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/gfucpgycn.sHtML

[S26] C：内存清零
来源：http://www.share.epnwcf.com/Article/details/gdjwgxhkb.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.epnwcf.com/Article/details/gzzdizcov.sHtML

[S27] C：定义常量
来源：http://read.share.yfazqb.com/Article/details/gezrlxcxy.sHtML

const double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gjhyjwfzi.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gpwgbvsza.sHtML

static int counter = 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gybskfadv.sHtML

[S29] C：变参函数
来源：http://wap.bbcook.cn/Article/details/gnfickbmu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.vehdjk.com/Article/details/geytmqkff.sHtML

[S30] C：头文件保护
来源：http://www.share.bbcook.cn/Article/details/gtqvpzqvi.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/gsnngjabp.sHtML

#define X_H
来源：http://m.share.tarul.cn/Article/details/gchxehwct.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/gvqttykig.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/gngdkxpwi.sHtML


<!-- 参考信息 -->