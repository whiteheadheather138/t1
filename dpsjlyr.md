代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.blog.sjlbkw.cn/Article/details/gsmpjgeit.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fktsv.cn/Article/details/gqwdufxmv.sHtML

[Q43] 标量子查询
来源：http://3g.vehdjk.com/Article/details/ghsgnsjsh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.vehdjk.com/Article/details/guyzwrrii.sHtML

[Q44] IN 子查询
来源：http://www.share.epnwcf.com/Article/details/ggyzhjjxn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.bbcook.cn/Article/details/gkeduvrmy.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.tarul.cn/Article/details/gvgokjqke.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.tarul.cn/Article/details/gjhovvaya.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.bbcook.cn/Article/details/gxhinnpxc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gnypyreru.sHtML

[Q47] 与平均值比较
来源：http://www.share.sjlbkw.cn/Article/details/ghrbjpzwf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fktsv.cn/Article/details/gdidaxvie.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fktsv.cn/Article/details/gnlbgwghi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.sjlbkw.cn/Article/details/goylfejcz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.sjlbkw.cn/Article/details/gpqwwwlss.sHtML

[Q49] 更新单行
来源：http://www.blog.yfazqb.com/Article/details/gzjhodduo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/griemccqm.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/gzncfmchh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fktsv.cn/Article/details/gswhkegll.sHtML

[Q51] 用子查询更新
来源：http://read.share.vehdjk.com/Article/details/gmayjsgzs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.bbcook.cn/Article/details/givjltfgd.sHtML

[Q52] 删除指定行
来源：http://read.share.bbcook.cn/Article/details/gqolarnxj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/gvtxwphhj.sHtML

[Q53] 按条件删除
来源：http://m.share.tarul.cn/Article/details/gcqbzpacw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.epnwcf.com/Article/details/ghvxcevae.sHtML

[Q54] 清空表
来源：http://read.share.yfazqb.com/Article/details/goiapfisz.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fktsv.cn/Article/details/guzqcprhm.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fktsv.cn/Article/details/galhlmnef.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gboseerbk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/gjhcjfnmc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/gnbcahckz.sHtML

[Q57] 行号
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfdcujit.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fktsv.cn/Article/details/gawtsfxfa.sHtML

[Q58] 累计求和
来源：http://www.m.share.epnwcf.com/Article/details/geqmtztmn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gkibhhhfa.sHtML

[Q59] 分组内累计
来源：http://www.blog.vehdjk.com/Article/details/gytrmmiwc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gginlmqiv.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.epnwcf.com/Article/details/gwkqggfyp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.vehdjk.com/Article/details/glmvijhvf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.tarul.cn/Article/details/gcglhmoho.sHtML

[Q61] 移动平均
来源：http://baike.bbcook.cn/Article/details/gkpoxnncr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/galcceakc.sHtML

[Q62] 分组占比
来源：http://www.blog.epnwcf.com/Article/details/guccvgtvv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gukpsqcii.sHtML

[Q63] 开启事务
来源：http://read.share.fktsv.cn/Article/details/gbctgcisx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.bbcook.cn/Article/details/gtxdmwqah.sHtML

[Q64] 提交事务
来源：http://read.share.vehdjk.com/Article/details/gyqrccgen.sHtML

COMMIT;
来源：http://baike.tarul.cn/Article/details/glitnvezw.sHtML

[Q65] 回滚事务
来源：http://www.blog.tarul.cn/Article/details/ggzvcafom.sHtML

ROLLBACK;
来源：http://www.share.sjlbkw.cn/Article/details/gpunhlrto.sHtML

[Q66] 行锁查询
来源：http://baike.vehdjk.com/Article/details/guhbhvsxj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.tarul.cn/Article/details/gsquuezwi.sHtML

[Q67] 设置隔离级别
来源：http://blog.tarul.cn/Article/details/ghtptlgef.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.epnwcf.com/Article/details/gliwupsgj.sHtML

[Q68] 保存点
来源：http://read.share.vehdjk.com/Article/details/ghnzpyhyq.sHtML

SAVEPOINT sp1;
来源：http://3g.bbcook.cn/Article/details/gymsdsvwx.sHtML

ROLLBACK TO sp1;
来源：http://read.share.bbcook.cn/Article/details/gcvypqheh.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.yfazqb.com/Article/details/gmjlmsrmz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.vehdjk.com/Article/details/gbmwpobyi.sHtML

[Q70] 更新统计信息
来源：http://mobile.tarul.cn/Article/details/gjeeroqnw.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/gyierxuvt.sHtML

[Q71] 查看建表语句
来源：http://blog.epnwcf.com/Article/details/gxcvpbcim.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.epnwcf.com/Article/details/goxuwvlun.sHtML

[Q72] 查看索引
来源：http://blog.fktsv.cn/Article/details/gvzmwyley.sHtML

SHOW INDEX FROM users;
来源：http://mobile.epnwcf.com/Article/details/gswvuffqh.sHtML

[Q73] 查看表状态
来源：http://www.share.fktsv.cn/Article/details/gzcussknz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gnyfjqojq.sHtML

[Q74] 强制使用索引
来源：http://m.share.vehdjk.com/Article/details/gwhoqfnwa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/gnqybxjmy.sHtML

[Q75] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gqyteyfxh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gmexeakdo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.sjlbkw.cn/Article/details/gicaggidi.sHtML

[Q76] 按天统计
来源：http://wap.fktsv.cn/Article/details/ghtvqygyr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.sjlbkw.cn/Article/details/gfhtymyvb.sHtML

[Q77] 时间加减
来源：http://wap.fktsv.cn/Article/details/gcqcivxsx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.tarul.cn/Article/details/gbhjeiotu.sHtML

[Q78] 当前时间
来源：http://baike.yfazqb.com/Article/details/grcmqanvl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.tarul.cn/Article/details/gvhgxzrrh.sHtML

[Q79] 字符串拼接
来源：http://www.share.tarul.cn/Article/details/gwqpqspwn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.epnwcf.com/Article/details/genznldpg.sHtML

[Q80] 字符串截取
来源：http://3g.epnwcf.com/Article/details/gysvgekhw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/ggnywwuhl.sHtML

[Q81] 字符串替换
来源：http://wap.bbcook.cn/Article/details/ghafqnpqr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gkvobdtuj.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.yfazqb.com/Article/details/gukpsckrg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/giuefpeux.sHtML

[Q83] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/glupodzdh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.tarul.cn/Article/details/gbcjnprfo.sHtML

[Q84] 去除首尾空格
来源：http://blog.vehdjk.com/Article/details/gcblbqnis.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gohgkvizr.sHtML

[Q85] 数值取整
来源：http://wap.sjlbkw.cn/Article/details/grvccnmeh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.vehdjk.com/Article/details/gyozyxmao.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.tarul.cn/Article/details/gnengnqnd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.tarul.cn/Article/details/grumimuln.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.epnwcf.com/Article/details/guwwxfmgk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.yfazqb.com/Article/details/gndspajqy.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/gdflvmlcn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fktsv.cn/Article/details/gsaaeoivo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.tarul.cn/Article/details/grttjtnef.sHtML

[Q89] 判断表是否存在
来源：http://wap.vehdjk.com/Article/details/gglofnydh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fktsv.cn/Article/details/glaqbchft.sHtML

[Q90] 生成序号列
来源：http://blog.sjlbkw.cn/Article/details/gbfrnrlfm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.epnwcf.com/Article/details/gxodukszp.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gedopmjxm.sHtML

R. Bash 专题
来源：http://www.share.epnwcf.com/Article/details/gfujmypum.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gsanryipv.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fktsv.cn/Article/details/gefccrohx.sHtML

#!/usr/bin/env bash
来源：http://3g.sjlbkw.cn/Article/details/gvlqjtnjj.sHtML

set -euo pipefail
来源：http://3g.yfazqb.com/Article/details/gftmdfmjp.sHtML

[R02] 变量赋值与使用
来源：http://wap.fktsv.cn/Article/details/gfsjanfes.sHtML

name="Tom"; echo "$name"
来源：http://mobile.yfazqb.com/Article/details/gfpjxrdny.sHtML

[R03] 只读变量
来源：http://blog.vehdjk.com/Article/details/gxoumkwhk.sHtML

readonly PI=3.14
来源：http://wap.tarul.cn/Article/details/gzitbrhdq.sHtML

[R04] 位置参数
来源：http://mobile.vehdjk.com/Article/details/gwfejgqix.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.vehdjk.com/Article/details/gtspsghas.sHtML

[R05] 参数默认值
来源：http://3g.vehdjk.com/Article/details/gbzuwxnvn.sHtML

name="${1:-default}"
来源：http://wap.yfazqb.com/Article/details/gdoszohsx.sHtML

[R06] 判断命令是否存在
来源：http://wap.bbcook.cn/Article/details/gjhkhagsu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gozlhaicg.sHtML

[R07] if 判断文件
来源：http://www.share.sjlbkw.cn/Article/details/gyoiztmsm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.bbcook.cn/Article/details/gelzzgzhv.sHtML

[R08] 数值比较
来源：http://blog.yfazqb.com/Article/details/ghmegjxbq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gmdrfoplz.sHtML

[R09] 字符串比较
来源：http://wap.vehdjk.com/Article/details/grppzjahv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.yfazqb.com/Article/details/ggbtfaoih.sHtML

[R10] 正则匹配
来源：http://m.share.epnwcf.com/Article/details/giylkjbvv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.yfazqb.com/Article/details/ggjbzelvs.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/gmywonfpu.sHtML

case "$1" in
来源：http://read.share.tarul.cn/Article/details/gklgxlkiz.sHtML

start) echo "启动" ;;
来源：http://www.share.fktsv.cn/Article/details/gyzmoqjhe.sHtML

stop)  echo "停止" ;;
来源：http://wap.bbcook.cn/Article/details/gciekycvx.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gfqbviysx.sHtML

esac
来源：http://www.blog.tarul.cn/Article/details/gmangdwfq.sHtML

[R12] for 遍历文件
来源：http://blog.vehdjk.com/Article/details/geoubddek.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.epnwcf.com/Article/details/girlbttyq.sHtML

[R13] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gqjvyrgbl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/gkglxexkv.sHtML

[R14] C 风格 for
来源：http://www.share.epnwcf.com/Article/details/gfjsscqim.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/gxepbjkjx.sHtML

[R15] while 逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gvvcxzidr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fktsv.cn/Article/details/gwxsgylrz.sHtML

[R16] until 等待条件
来源：http://mobile.epnwcf.com/Article/details/gmpttealp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/ggtzrbbey.sHtML

[R17] 数组定义与取值
来源：http://wap.sjlbkw.cn/Article/details/gtgbppasm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.tarul.cn/Article/details/gxcaxjsig.sHtML

[R18] 遍历数组
来源：http://www.share.vehdjk.com/Article/details/gxfdhsznx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.bbcook.cn/Article/details/gpxanicha.sHtML

[R19] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gdzlonoim.sHtML

echo "${#arr[@]}"
来源：http://3g.tarul.cn/Article/details/gqzoroexi.sHtML

[R20] 关联数组（字典）
来源：http://read.share.bbcook.cn/Article/details/gtqatnjfb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fktsv.cn/Article/details/guxphwyls.sHtML

[R21] 字符串长度
来源：http://read.share.yfazqb.com/Article/details/gujnmrjwh.sHtML

echo "${#s}"
来源：http://www.blog.bbcook.cn/Article/details/ghmuxywqg.sHtML

[R22] 截取子串
来源：http://baike.vehdjk.com/Article/details/guohiquvw.sHtML

echo "${s:0:5}"
来源：http://m.share.fktsv.cn/Article/details/gxggjlqlm.sHtML

[R23] 字符串替换
来源：http://blog.vehdjk.com/Article/details/gcrybcvoo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.tarul.cn/Article/details/ghsexwkub.sHtML

[R24] 大小写转换
来源：http://baike.fktsv.cn/Article/details/gcvufbije.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.bbcook.cn/Article/details/gqjacvazq.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.vehdjk.com/Article/details/gbpczakuq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.sjlbkw.cn/Article/details/glosxnsvv.sHtML

[R26] 命令替换
来源：http://www.share.epnwcf.com/Article/details/govbbzdhk.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.yfazqb.com/Article/details/gqmrswhmr.sHtML

[R27] 算术展开
来源：http://3g.fktsv.cn/Article/details/gslchvrdo.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.tarul.cn/Article/details/glojxlyfm.sHtML

[R28] 浮点运算
来源：http://mobile.tarul.cn/Article/details/gtgwjhtni.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.epnwcf.com/Article/details/ggwtigkvp.sHtML

[R29] 定义函数
来源：http://wap.vehdjk.com/Article/details/gesqlajyz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.sjlbkw.cn/Article/details/gndhppiew.sHtML

[R30] 函数返回状态码
来源：http://read.share.bbcook.cn/Article/details/gjyykggyf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.vehdjk.com/Article/details/gthrzzlhb.sHtML

[R31] 局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gvtxwlzzi.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/gnvdtugku.sHtML

[R32] 参数个数校验
来源：http://wap.tarul.cn/Article/details/grltcvgsd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.vehdjk.com/Article/details/gofxzbbje.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.epnwcf.com/Article/details/gtciwbwkx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.vehdjk.com/Article/details/graisiuzu.sHtML

[R34] 退出时清理
来源：http://www.m.share.yfazqb.com/Article/details/gwhbbecqt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/ghtdirgli.sHtML

[R35] 后台执行并等待
来源：http://blog.yfazqb.com/Article/details/gqjivrkfd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fktsv.cn/Article/details/gbwwbwxbw.sHtML

[R36] 并发执行多个任务
来源：http://blog.epnwcf.com/Article/details/gwuozjyqc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fktsv.cn/Article/details/goqamyrqg.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/gcrxbkgig.sHtML

files=$(ls -1)
来源：http://www.m.share.epnwcf.com/Article/details/gwezdtvox.sHtML

[R38] 管道串联
来源：http://www.m.share.fktsv.cn/Article/details/gkkktzpng.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.bbcook.cn/Article/details/gpfaadfkj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.vehdjk.com/Article/details/ganbphsvn.sHtML

cmd > out.log 2>&1
来源：http://blog.sjlbkw.cn/Article/details/glgjufofw.sHtML

[R40] 追加写日志
来源：http://m.share.sjlbkw.cn/Article/details/ginvdxpmx.sHtML

echo "log" >> out.log
来源：http://read.share.fktsv.cn/Article/details/gczhyixow.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fktsv.cn/Article/details/ggpeyiosf.sHtML

cmd >/dev/null 2>&1
来源：http://blog.bbcook.cn/Article/details/gicigdlsx.sHtML

[R42] 输入重定向
来源：http://m.share.bbcook.cn/Article/details/gthoozvid.sHtML

wc -l < a.txt
来源：http://3g.epnwcf.com/Article/details/gqommjpin.sHtML

[R43] 按名字查找文件
来源：http://blog.yfazqb.com/Article/details/gcorfirjz.sHtML

find . -name "*.log" -type f
来源：http://m.share.bbcook.cn/Article/details/gryxaiwqp.sHtML

[R44] 按修改时间查找
来源：http://baike.epnwcf.com/Article/details/gvhdkwjeb.sHtML

find . -mtime -7 -type f
来源：http://blog.tarul.cn/Article/details/gbxipkuij.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/ggowoyqlw.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fktsv.cn/Article/details/gihsunnby.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.sjlbkw.cn/Article/details/gocrvlkub.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.sjlbkw.cn/Article/details/guuagpwnt.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/gcnplujyi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.yfazqb.com/Article/details/ggablprkv.sHtML

[R48] awk 取指定列
来源：http://www.blog.epnwcf.com/Article/details/gpxrayjlp.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fktsv.cn/Article/details/gzcgongsf.sHtML

[R49] awk 带条件
来源：http://read.share.tarul.cn/Article/details/gxqvwpbdv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.tarul.cn/Article/details/gfwlgirtk.sHtML

[R50] awk 求和
来源：http://mobile.bbcook.cn/Article/details/gjpccblei.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fktsv.cn/Article/details/grlimggqt.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/gtryxrrol.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.tarul.cn/Article/details/gsdizalao.sHtML

[R52] 统计行数
来源：http://wap.sjlbkw.cn/Article/details/gqappaueq.sHtML

wc -l a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gbnntjsvw.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fktsv.cn/Article/details/gybcmtypm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.yfazqb.com/Article/details/gesgxkrwu.sHtML

[R54] 比较两个文件
来源：http://baike.yfazqb.com/Article/details/gqaezzvrl.sHtML

diff a.txt b.txt
来源：http://mobile.yfazqb.com/Article/details/gyhtpywrb.sHtML

[R55] 压缩与解压
来源：http://3g.yfazqb.com/Article/details/gnyvqhpws.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.epnwcf.com/Article/details/gdiewcdbg.sHtML

[R56] 远程拷贝
来源：http://blog.vehdjk.com/Article/details/gslonlxsq.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/gpriyvpdb.sHtML

[R57] 远程执行命令
来源：http://baike.bbcook.cn/Article/details/gzsrsrtnn.sHtML

ssh user@host 'uptime'
来源：http://m.share.sjlbkw.cn/Article/details/guqbafjhl.sHtML

[R58] 下载文件
来源：http://www.m.share.yfazqb.com/Article/details/gauxcrrwo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.vehdjk.com/Article/details/giflmrtwj.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/gpxuiplky.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.bbcook.cn/Article/details/giggiksjw.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gxmtyuffa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/gxcsicknb.sHtML

[R61] 磁盘占用
来源：http://m.share.sjlbkw.cn/Article/details/gdmeklpwr.sHtML

df -h;  du -sh *
来源：http://mobile.bbcook.cn/Article/details/grhcehlwm.sHtML

[R62] 找最占空间的文件
来源：http://m.share.epnwcf.com/Article/details/gnumaexpy.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/gjnsiakxn.sHtML

[R63] 内存与进程
来源：http://mobile.epnwcf.com/Article/details/gaiqlwgad.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.bbcook.cn/Article/details/gsvjatzfb.sHtML

[R64] 结束进程
来源：http://wap.bbcook.cn/Article/details/gsafqthff.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.bbcook.cn/Article/details/ggjhfobpb.sHtML

[R65] 查看端口占用
来源：http://www.share.yfazqb.com/Article/details/gqukanpmv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.sjlbkw.cn/Article/details/gmpuvyfbn.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gliokhhdu.sHtML

crontab -e;  crontab -l
来源：http://read.share.yfazqb.com/Article/details/gcqswomxh.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/gltgvipoe.sHtML

openssl rand -hex 16
来源：http://mobile.yfazqb.com/Article/details/genzcmkkn.sHtML

[R68] 计算文件校验值
来源：http://wap.yfazqb.com/Article/details/gqveunacs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.vehdjk.com/Article/details/gnmbcvrgr.sHtML

[R69] 生成随机密码
来源：http://mobile.yfazqb.com/Article/details/gmulpnynm.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.yfazqb.com/Article/details/ggyvacokb.sHtML

[R70] 时间戳与互转
来源：http://m.share.yfazqb.com/Article/details/gfruftpgu.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fktsv.cn/Article/details/gfqhvrvkw.sHtML

[R71] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/galznvvbw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.bbcook.cn/Article/details/gnyiaiqcd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fktsv.cn/Article/details/gtwxlkdav.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gskclfsjk.sHtML

[R73] 分割大日志
来源：http://m.share.vehdjk.com/Article/details/ghnzaqywr.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/glwmxhiqt.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/gtvvqsjtt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.tarul.cn/Article/details/gpzlaemgr.sHtML

[R75] 导出环境变量
来源：http://mobile.bbcook.cn/Article/details/gvrlutoab.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.sjlbkw.cn/Article/details/gybshgztq.sHtML

[R76] 使用临时文件
来源：http://www.m.share.vehdjk.com/Article/details/gviejejjl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/gbbabqymm.sHtML

[R77] 读取用户输入
来源：http://www.blog.epnwcf.com/Article/details/gbnnkvvic.sHtML

read -rp "请输入: " ans
来源：http://wap.vehdjk.com/Article/details/gwbntsxjw.sHtML

[R78] 交互式菜单
来源：http://blog.bbcook.cn/Article/details/gqszwszwa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.vehdjk.com/Article/details/gzjydtxrf.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnbeoinj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.vehdjk.com/Article/details/gfasmvuis.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.yfazqb.com/Article/details/gbfhelbet.sHtML

time ./run.sh
来源：http://m.share.tarul.cn/Article/details/gwgtoqjek.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbmqbdhqp.sHtML

S. C / C++ 专题
来源：http://www.m.share.epnwcf.com/Article/details/gljvxawzt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gnfffrkhd.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gayilbqap.sHtML

#include <stdio.h>
来源：http://www.blog.bbcook.cn/Article/details/grzbntpqd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.vehdjk.com/Article/details/gcpwjvqgm.sHtML

[S02] C：变量与格式化输出
来源：http://wap.vehdjk.com/Article/details/guexhgbeu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fktsv.cn/Article/details/ghhhqaeaq.sHtML

[S03] C：读入整数
来源：http://mobile.yfazqb.com/Article/details/gsbkogvex.sHtML

int x; scanf("%d", &x);
来源：http://wap.epnwcf.com/Article/details/gzmihqteo.sHtML

[S04] C：字符串复制
来源：http://m.share.yfazqb.com/Article/details/gccmklsqo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.tarul.cn/Article/details/gjirerhuf.sHtML

[S05] C：字符串长度
来源：http://read.share.bbcook.cn/Article/details/gxiazoqqi.sHtML

strlen(s)
来源：http://m.share.vehdjk.com/Article/details/gpajlpkxo.sHtML

[S06] C：字符串比较
来源：http://www.share.vehdjk.com/Article/details/getjnjnpe.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.tarul.cn/Article/details/gizrknvyf.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/gbatophkf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.bbcook.cn/Article/details/gzjybgmqh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.vehdjk.com/Article/details/gujzmzpez.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.epnwcf.com/Article/details/gfwggijyh.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.bbcook.cn/Article/details/ghwrsutqd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.vehdjk.com/Article/details/gzprycxlw.sHtML

[S10] C：指针与解引用
来源：http://wap.vehdjk.com/Article/details/gkygnglss.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fktsv.cn/Article/details/gilhvpsbf.sHtML

[S11] C：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gfjfnraea.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.vehdjk.com/Article/details/gjyhrmkwk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/gfuvjpobw.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/guoggdzhh.sHtML

[S12] C：写文件
来源：http://baike.vehdjk.com/Article/details/ghoxabxpt.sHtML


<!-- 参考信息 -->