代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/gxvlvfznn.sHtML

[Q50] 批量更新
来源：http://read.share.sjlbkw.cn/Article/details/gjajgoceg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.tarul.cn/Article/details/gftccouas.sHtML

[Q51] 用子查询更新
来源：http://baike.tarul.cn/Article/details/gkqrqqsrb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gicrvncdf.sHtML

[Q52] 删除指定行
来源：http://www.m.share.sjlbkw.cn/Article/details/gkidawaqi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gthoxlylg.sHtML

[Q53] 按条件删除
来源：http://3g.sjlbkw.cn/Article/details/gnyejvruz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.tarul.cn/Article/details/gqplbdnab.sHtML

[Q54] 清空表
来源：http://www.m.share.fktsv.cn/Article/details/gelbtpinj.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.tarul.cn/Article/details/gxydcajes.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.yfazqb.com/Article/details/gwzdtxmyh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gaxamtxaq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/gkmslckhj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/gxbsvbnfa.sHtML

[Q57] 行号
来源：http://mobile.vehdjk.com/Article/details/gfzfozzit.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.epnwcf.com/Article/details/geoaoanxi.sHtML

[Q58] 累计求和
来源：http://www.blog.yfazqb.com/Article/details/gjnfaxuhh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.epnwcf.com/Article/details/ghxtadkqa.sHtML

[Q59] 分组内累计
来源：http://www.blog.fktsv.cn/Article/details/gcihuhbzk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/grubhsfmt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.bbcook.cn/Article/details/gpncoaoiw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.bbcook.cn/Article/details/ghweofqqy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fktsv.cn/Article/details/gqibyyhry.sHtML

[Q61] 移动平均
来源：http://www.share.bbcook.cn/Article/details/gkeajdaib.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gzgzuzqyh.sHtML

[Q62] 分组占比
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgwwbtuv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gstxidxqr.sHtML

[Q63] 开启事务
来源：http://blog.vehdjk.com/Article/details/gyrmkkhhf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.yfazqb.com/Article/details/gyginiiuu.sHtML

[Q64] 提交事务
来源：http://www.share.sjlbkw.cn/Article/details/gqutxuofv.sHtML

COMMIT;
来源：http://wap.vehdjk.com/Article/details/gvnauegbq.sHtML

[Q65] 回滚事务
来源：http://www.blog.tarul.cn/Article/details/gnlhxwfyl.sHtML

ROLLBACK;
来源：http://m.share.tarul.cn/Article/details/ghqicoeve.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/grzoohjll.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fktsv.cn/Article/details/gkvhlwrxc.sHtML

[Q67] 设置隔离级别
来源：http://baike.sjlbkw.cn/Article/details/gyhlomgau.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.tarul.cn/Article/details/gzbmobejs.sHtML

[Q68] 保存点
来源：http://read.share.vehdjk.com/Article/details/gjtskqswr.sHtML

SAVEPOINT sp1;
来源：http://mobile.sjlbkw.cn/Article/details/gzvrbphkq.sHtML

ROLLBACK TO sp1;
来源：http://m.share.bbcook.cn/Article/details/ggkrnxpav.sHtML

[Q69] 查看执行计划
来源：http://3g.tarul.cn/Article/details/gwdiixdpc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.epnwcf.com/Article/details/givenfcdu.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fktsv.cn/Article/details/gyplcfuve.sHtML

ANALYZE TABLE users;
来源：http://m.share.bbcook.cn/Article/details/gacukiehm.sHtML

[Q71] 查看建表语句
来源：http://3g.vehdjk.com/Article/details/gbzqqxdpn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fktsv.cn/Article/details/gdmkhbfyo.sHtML

[Q72] 查看索引
来源：http://www.blog.fktsv.cn/Article/details/gdsteqkmt.sHtML

SHOW INDEX FROM users;
来源：http://mobile.yfazqb.com/Article/details/gemlcwani.sHtML

[Q73] 查看表状态
来源：http://3g.fktsv.cn/Article/details/gmkkkwlgo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.sjlbkw.cn/Article/details/grccorypg.sHtML

[Q74] 强制使用索引
来源：http://3g.epnwcf.com/Article/details/gwexzssvt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fktsv.cn/Article/details/gfycqwizx.sHtML

[Q75] 日期格式化
来源：http://blog.bbcook.cn/Article/details/gmovnpjjg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.vehdjk.com/Article/details/gucicagwy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.vehdjk.com/Article/details/gnkmougkv.sHtML

[Q76] 按天统计
来源：http://baike.vehdjk.com/Article/details/gbtxcrgym.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/ghdllvekw.sHtML

[Q77] 时间加减
来源：http://wap.sjlbkw.cn/Article/details/gefqfooxf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.tarul.cn/Article/details/gzukmmkmz.sHtML

[Q78] 当前时间
来源：http://baike.bbcook.cn/Article/details/getyscxiu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.tarul.cn/Article/details/grhwkkehq.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.tarul.cn/Article/details/gqpvwuxdt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.bbcook.cn/Article/details/gqifdlwgg.sHtML

[Q80] 字符串截取
来源：http://mobile.bbcook.cn/Article/details/gnzomxymh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gewsepxzl.sHtML

[Q81] 字符串替换
来源：http://read.share.yfazqb.com/Article/details/gbynrfceq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.tarul.cn/Article/details/gjiddnmge.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.tarul.cn/Article/details/garbfrsvh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gzqwfdkfh.sHtML

[Q83] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gbvxaieuz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhowxeoe.sHtML

[Q84] 去除首尾空格
来源：http://read.share.tarul.cn/Article/details/gzphzgdrd.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gabfermtq.sHtML

[Q85] 数值取整
来源：http://www.blog.yfazqb.com/Article/details/gsnyummjb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.epnwcf.com/Article/details/gwaoxfgsw.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fktsv.cn/Article/details/grwbslkrh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.tarul.cn/Article/details/gnasaeinx.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.sjlbkw.cn/Article/details/gtdmpjvdm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.vehdjk.com/Article/details/gswnqfdjk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.vehdjk.com/Article/details/gpafbrmwi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.sjlbkw.cn/Article/details/gnjpfxaoo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gbfzmwjub.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gnwiltxep.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.yfazqb.com/Article/details/gixykemut.sHtML

[Q90] 生成序号列
来源：http://mobile.tarul.cn/Article/details/gjyeuyxuh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fktsv.cn/Article/details/gnxmmipwt.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gvzgwtgoj.sHtML

R. Bash 专题
来源：http://wap.bbcook.cn/Article/details/gtgqteujy.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gezksyrqi.sHtML

[R01] shebang 与严格模式
来源：http://blog.vehdjk.com/Article/details/ghbohovkw.sHtML

#!/usr/bin/env bash
来源：http://blog.fktsv.cn/Article/details/gmrgydkwg.sHtML

set -euo pipefail
来源：http://wap.sjlbkw.cn/Article/details/grorkodsa.sHtML

[R02] 变量赋值与使用
来源：http://mobile.sjlbkw.cn/Article/details/gsicyqrta.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/gtfxgibnp.sHtML

[R03] 只读变量
来源：http://wap.bbcook.cn/Article/details/gfamoqnfg.sHtML

readonly PI=3.14
来源：http://wap.vehdjk.com/Article/details/gqxrgejot.sHtML

[R04] 位置参数
来源：http://www.share.fktsv.cn/Article/details/gdftazgvd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.yfazqb.com/Article/details/gfvdyhgyq.sHtML

[R05] 参数默认值
来源：http://m.share.bbcook.cn/Article/details/gyoundcka.sHtML

name="${1:-default}"
来源：http://www.share.tarul.cn/Article/details/gscbcimox.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/gxoonmyst.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/ghlzpznva.sHtML

[R07] if 判断文件
来源：http://3g.yfazqb.com/Article/details/gbkpzdjxi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.yfazqb.com/Article/details/glnvqrgxn.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/gszgnzivp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.tarul.cn/Article/details/ggdukfwyn.sHtML

[R09] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gmfffaodc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gxdfgowlj.sHtML

[R10] 正则匹配
来源：http://3g.bbcook.cn/Article/details/ggqezyvfh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.bbcook.cn/Article/details/ghtgdjdce.sHtML

[R11] case 多分支
来源：http://3g.vehdjk.com/Article/details/gusowhnwi.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/gcbbktpeg.sHtML

start) echo "启动" ;;
来源：http://blog.yfazqb.com/Article/details/gntctydqi.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.tarul.cn/Article/details/gqszucoew.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.yfazqb.com/Article/details/gqcerwnby.sHtML

esac
来源：http://wap.tarul.cn/Article/details/gqtttqhyj.sHtML

[R12] for 遍历文件
来源：http://wap.fktsv.cn/Article/details/gnawyzjim.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.epnwcf.com/Article/details/gqnvgkyyl.sHtML

[R13] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/gvisnzjmj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gcshkguff.sHtML

[R14] C 风格 for
来源：http://m.share.vehdjk.com/Article/details/gcaowxhrc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.yfazqb.com/Article/details/gllnfxjsc.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/govnmiweg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.vehdjk.com/Article/details/gfdyghvyg.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/gwudisofz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gealvjubx.sHtML

[R17] 数组定义与取值
来源：http://blog.yfazqb.com/Article/details/gycnmhgxk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.yfazqb.com/Article/details/gndzdvuki.sHtML

[R18] 遍历数组
来源：http://3g.tarul.cn/Article/details/gskkjokok.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fktsv.cn/Article/details/glbmrlpzw.sHtML

[R19] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gyohykvon.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.yfazqb.com/Article/details/goldhxkny.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fktsv.cn/Article/details/gcgirwusn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.sjlbkw.cn/Article/details/gastvruzp.sHtML

[R21] 字符串长度
来源：http://blog.tarul.cn/Article/details/gyhqwaeim.sHtML

echo "${#s}"
来源：http://www.m.share.tarul.cn/Article/details/gpngwgqiq.sHtML

[R22] 截取子串
来源：http://3g.yfazqb.com/Article/details/gbacclwbn.sHtML

echo "${s:0:5}"
来源：http://www.share.bbcook.cn/Article/details/gwhzbzdtg.sHtML

[R23] 字符串替换
来源：http://baike.epnwcf.com/Article/details/ggeipedgp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.tarul.cn/Article/details/glcfipiwa.sHtML

[R24] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gnpumjljw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.epnwcf.com/Article/details/gzxlkrclk.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fktsv.cn/Article/details/grkepqqnj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.bbcook.cn/Article/details/gzldcnzbl.sHtML

[R26] 命令替换
来源：http://blog.yfazqb.com/Article/details/gidjaqfay.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fktsv.cn/Article/details/gtugohrdw.sHtML

[R27] 算术展开
来源：http://www.blog.tarul.cn/Article/details/gqvytugeo.sHtML

echo $((1 + 2 * 3))
来源：http://blog.epnwcf.com/Article/details/gfxdmxtux.sHtML

[R28] 浮点运算
来源：http://www.m.share.epnwcf.com/Article/details/gybowkvcu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/ggvespyyu.sHtML

[R29] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gcolmslwe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fktsv.cn/Article/details/gehsxvmof.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/gguradvet.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.bbcook.cn/Article/details/ggqbzawlf.sHtML

[R31] 局部变量
来源：http://baike.sjlbkw.cn/Article/details/grrsaarbj.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.epnwcf.com/Article/details/gdqqelcic.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fktsv.cn/Article/details/gjczssknq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gkbqwjvnb.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fktsv.cn/Article/details/ghvqxkvac.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.epnwcf.com/Article/details/grzmpuppl.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gojqplemo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/gqitxaqpz.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/giywggqjn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/guzsmswwj.sHtML

[R36] 并发执行多个任务
来源：http://baike.yfazqb.com/Article/details/ggnvdvobq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.vehdjk.com/Article/details/gijchjzjj.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fktsv.cn/Article/details/gkdfszpas.sHtML

files=$(ls -1)
来源：http://www.share.epnwcf.com/Article/details/goqcnqjvl.sHtML

[R38] 管道串联
来源：http://baike.bbcook.cn/Article/details/gwlmbnina.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.bbcook.cn/Article/details/gfysqccdi.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fktsv.cn/Article/details/gxfkruluz.sHtML

cmd > out.log 2>&1
来源：http://mobile.epnwcf.com/Article/details/gkrzpwmbc.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/grvwhvire.sHtML

echo "log" >> out.log
来源：http://wap.vehdjk.com/Article/details/grgfsifjp.sHtML

[R41] 丢弃输出
来源：http://3g.yfazqb.com/Article/details/ghzdpesoi.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/geudivvuv.sHtML

[R42] 输入重定向
来源：http://blog.sjlbkw.cn/Article/details/gifgyaplj.sHtML

wc -l < a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gzvgpghgo.sHtML

[R43] 按名字查找文件
来源：http://baike.fktsv.cn/Article/details/gzvxxqajr.sHtML

find . -name "*.log" -type f
来源：http://www.share.yfazqb.com/Article/details/gmypciwcs.sHtML

[R44] 按修改时间查找
来源：http://www.blog.yfazqb.com/Article/details/ggqpflxyb.sHtML

find . -mtime -7 -type f
来源：http://mobile.yfazqb.com/Article/details/gkxrpluzv.sHtML

[R45] 批量删除
来源：http://3g.yfazqb.com/Article/details/glxkdpdiu.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.tarul.cn/Article/details/grbfquxxd.sHtML

[R46] 递归替换文件内容
来源：http://m.share.vehdjk.com/Article/details/gmdkgbxda.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.yfazqb.com/Article/details/gtikcsflu.sHtML

[R47] sed 单行替换
来源：http://www.share.epnwcf.com/Article/details/gfazkuwqq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fktsv.cn/Article/details/gzchkwtym.sHtML

[R48] awk 取指定列
来源：http://baike.yfazqb.com/Article/details/gwmsemsck.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/gpbccvoij.sHtML

[R49] awk 带条件
来源：http://m.share.epnwcf.com/Article/details/gggjtxfzo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.bbcook.cn/Article/details/gledrpbcv.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gechztzld.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.bbcook.cn/Article/details/geukkisij.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/gjxkhpgvu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.tarul.cn/Article/details/ghnpfhuip.sHtML

[R52] 统计行数
来源：http://3g.fktsv.cn/Article/details/guwcoqtwj.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/gxusewbwh.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/gaalunyed.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.vehdjk.com/Article/details/gimfkufes.sHtML

[R54] 比较两个文件
来源：http://read.share.epnwcf.com/Article/details/gkitvcrcn.sHtML

diff a.txt b.txt
来源：http://www.m.share.bbcook.cn/Article/details/gogshtqsl.sHtML

[R55] 压缩与解压
来源：http://www.share.epnwcf.com/Article/details/gssvvkvlc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/gicgpscsg.sHtML

[R56] 远程拷贝
来源：http://mobile.sjlbkw.cn/Article/details/grnwnazor.sHtML

scp file user@host:/path/
来源：http://3g.epnwcf.com/Article/details/gdfgmzjky.sHtML

[R57] 远程执行命令
来源：http://wap.sjlbkw.cn/Article/details/gbvugglga.sHtML

ssh user@host 'uptime'
来源：http://mobile.sjlbkw.cn/Article/details/ggoelxjvg.sHtML

[R58] 下载文件
来源：http://mobile.yfazqb.com/Article/details/gohltxwse.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gylsxngvj.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/guenwdcvt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.epnwcf.com/Article/details/ggqoyuppf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gqzzrusee.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.sjlbkw.cn/Article/details/gzkbtlmrj.sHtML

[R61] 磁盘占用
来源：http://www.share.sjlbkw.cn/Article/details/ggptnphki.sHtML

df -h;  du -sh *
来源：http://read.share.epnwcf.com/Article/details/gaygvnunv.sHtML

[R62] 找最占空间的文件
来源：http://3g.fktsv.cn/Article/details/gbwgqpwwq.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.yfazqb.com/Article/details/ggrrblgwn.sHtML

[R63] 内存与进程
来源：http://www.blog.fktsv.cn/Article/details/gsubjabye.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.vehdjk.com/Article/details/gufhagrjr.sHtML

[R64] 结束进程
来源：http://www.blog.fktsv.cn/Article/details/gyjjcskoy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.vehdjk.com/Article/details/gyxjbksgk.sHtML

[R65] 查看端口占用
来源：http://www.blog.vehdjk.com/Article/details/gucjjcwud.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.bbcook.cn/Article/details/gaymjpjcr.sHtML

[R66] 定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gezkestfj.sHtML

crontab -e;  crontab -l
来源：http://3g.bbcook.cn/Article/details/gbcpbgnxl.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.yfazqb.com/Article/details/gcqrxdcpo.sHtML

openssl rand -hex 16
来源：http://read.share.bbcook.cn/Article/details/gddculaaw.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.bbcook.cn/Article/details/glxlztgil.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.tarul.cn/Article/details/gjcnhilvb.sHtML

[R69] 生成随机密码
来源：http://www.m.share.yfazqb.com/Article/details/glgelusyx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.sjlbkw.cn/Article/details/gamxfzbhp.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/gfefkklsn.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fktsv.cn/Article/details/gtnlpymdi.sHtML

[R71] 日期格式化
来源：http://baike.tarul.cn/Article/details/gxfcyvqde.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/gcqdhgwhi.sHtML

[R72] 等待端口就绪
来源：http://baike.yfazqb.com/Article/details/gjqlhccxv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/glxgkrobq.sHtML

[R73] 分割大日志
来源：http://m.share.sjlbkw.cn/Article/details/gnzbeabfs.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/ghoriizdi.sHtML

[R74] 批量重命名
来源：http://wap.yfazqb.com/Article/details/gejnsibpy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.bbcook.cn/Article/details/gkrltujqc.sHtML

[R75] 导出环境变量
来源：http://m.share.bbcook.cn/Article/details/gtmcvggtm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.vehdjk.com/Article/details/gnesmmjdz.sHtML

[R76] 使用临时文件
来源：http://www.blog.yfazqb.com/Article/details/gloigeizg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gaqrlsfqi.sHtML

[R77] 读取用户输入
来源：http://blog.yfazqb.com/Article/details/gogydsyrz.sHtML

read -rp "请输入: " ans
来源：http://www.share.yfazqb.com/Article/details/gnrkpennr.sHtML

[R78] 交互式菜单
来源：http://mobile.vehdjk.com/Article/details/gmvtampgi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/gbndjrfin.sHtML

[R79] 解析命令行选项
来源：http://blog.fktsv.cn/Article/details/giifxcnyx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.vehdjk.com/Article/details/ggefjooxr.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.epnwcf.com/Article/details/ggiyfzwgj.sHtML

time ./run.sh
来源：http://baike.bbcook.cn/Article/details/grpxdogxm.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gmwumcwrp.sHtML

S. C / C++ 专题
来源：http://3g.epnwcf.com/Article/details/gqaoexhal.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gyrpbrdaw.sHtML

[S01] C：Hello World
来源：http://wap.epnwcf.com/Article/details/gebxtfetd.sHtML

#include <stdio.h>
来源：http://mobile.bbcook.cn/Article/details/gafyjmhli.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.bbcook.cn/Article/details/goyselxte.sHtML

[S02] C：变量与格式化输出
来源：http://blog.vehdjk.com/Article/details/gfwielsix.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.tarul.cn/Article/details/gemeoxvdo.sHtML

[S03] C：读入整数
来源：http://read.share.epnwcf.com/Article/details/gwfrfqupj.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.yfazqb.com/Article/details/ggdijbkcl.sHtML

[S04] C：字符串复制
来源：http://read.share.tarul.cn/Article/details/gvynpujpq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.vehdjk.com/Article/details/gykmynqlt.sHtML

[S05] C：字符串长度
来源：http://wap.bbcook.cn/Article/details/grsypcdmr.sHtML

strlen(s)
来源：http://m.share.sjlbkw.cn/Article/details/gobiahxck.sHtML

[S06] C：字符串比较
来源：http://read.share.bbcook.cn/Article/details/guhqcjhim.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.bbcook.cn/Article/details/ggfsjyiuu.sHtML

[S07] C：数组遍历求和
来源：http://m.share.tarul.cn/Article/details/ggezpsyhr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fktsv.cn/Article/details/ggyvmxynq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.tarul.cn/Article/details/gcbqveitu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.sjlbkw.cn/Article/details/gsymzbpbt.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.tarul.cn/Article/details/ggthimxkp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.sjlbkw.cn/Article/details/glyfycluh.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gnuoibnaj.sHtML

int *p = &a;  *p = 5;
来源：http://3g.vehdjk.com/Article/details/gmnvilrxo.sHtML

[S11] C：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gqyrfnwmq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.tarul.cn/Article/details/gyxvmlrbu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.epnwcf.com/Article/details/gdljctlyw.sHtML

fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gwgmhxnxm.sHtML

[S12] C：写文件
来源：http://mobile.tarul.cn/Article/details/gkokfudqb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.tarul.cn/Article/details/gaocvienr.sHtML

[S13] C：宏定义
来源：http://www.m.share.vehdjk.com/Article/details/gopmwzbrq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.sjlbkw.cn/Article/details/gwmsesbnj.sHtML

[S14] C：枚举
来源：http://wap.bbcook.cn/Article/details/goqdpqwzi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.vehdjk.com/Article/details/ghxearsmk.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gxpmxsghv.sHtML

(double) a / b
来源：http://baike.sjlbkw.cn/Article/details/giodtzzzs.sHtML

[S16] C：位操作置位
来源：http://3g.vehdjk.com/Article/details/gxasddvmh.sHtML

x |= (1 << 3);
来源：http://m.share.epnwcf.com/Article/details/ghuxbawks.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gvtikegre.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fktsv.cn/Article/details/gesqjgdsh.sHtML

[S18] C：命令行参数
来源：http://m.share.yfazqb.com/Article/details/giyddnlwn.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyixrdxim.sHtML

[S19] C：快速排序
来源：http://read.share.vehdjk.com/Article/details/gyuurpqnq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gbgsttlfz.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/gsooefnyn.sHtML


<!-- 参考信息 -->