代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://3g.tarul.cn/Article/details/gbyjbsjwv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.epnwcf.com/Article/details/goabhepuh.sHtML

[Q43] 标量子查询
来源：http://baike.tarul.cn/Article/details/gbyaqhuvb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.bbcook.cn/Article/details/gtyqnhjlw.sHtML

[Q44] IN 子查询
来源：http://www.share.bbcook.cn/Article/details/gqpgnaywq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.vehdjk.com/Article/details/gclguqrrg.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.epnwcf.com/Article/details/gauryfmfc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/gdevuetef.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.yfazqb.com/Article/details/gtugweugh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gounfnlyv.sHtML

[Q47] 与平均值比较
来源：http://mobile.sjlbkw.cn/Article/details/grnufnryk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.vehdjk.com/Article/details/gmbrssggj.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.epnwcf.com/Article/details/gertjymcv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.yfazqb.com/Article/details/gzarnpehe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fktsv.cn/Article/details/gfhkoadpw.sHtML

[Q49] 更新单行
来源：http://m.share.vehdjk.com/Article/details/gviqrjyev.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/glhzrkhfq.sHtML

[Q50] 批量更新
来源：http://3g.yfazqb.com/Article/details/gznnrvkfr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gfqjqkcat.sHtML

[Q51] 用子查询更新
来源：http://www.blog.epnwcf.com/Article/details/goppsqnts.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.yfazqb.com/Article/details/gpgdcpwif.sHtML

[Q52] 删除指定行
来源：http://m.share.yfazqb.com/Article/details/gsxlbrblt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/groifkfpz.sHtML

[Q53] 按条件删除
来源：http://www.m.share.yfazqb.com/Article/details/guojvvylb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.tarul.cn/Article/details/gcebvsezj.sHtML

[Q54] 清空表
来源：http://read.share.vehdjk.com/Article/details/gduccfjfg.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.yfazqb.com/Article/details/gvnzfasbm.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.yfazqb.com/Article/details/gyljmvtrf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gtorwobmi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.sjlbkw.cn/Article/details/gfoqsmruu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gsqeoydvv.sHtML

[Q57] 行号
来源：http://3g.epnwcf.com/Article/details/gaffqqxdc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gdnsqgipb.sHtML

[Q58] 累计求和
来源：http://www.m.share.vehdjk.com/Article/details/gqgtcanrk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.tarul.cn/Article/details/gchbqzsyi.sHtML

[Q59] 分组内累计
来源：http://m.share.vehdjk.com/Article/details/gypkgynec.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gufjodfaa.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.bbcook.cn/Article/details/gouyldeos.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.yfazqb.com/Article/details/gdvwfldsw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gsrdametr.sHtML

[Q61] 移动平均
来源：http://www.m.share.fktsv.cn/Article/details/gopmxbztg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gjuipqzdg.sHtML

[Q62] 分组占比
来源：http://www.blog.sjlbkw.cn/Article/details/glszdrbyy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gjztowuxk.sHtML

[Q63] 开启事务
来源：http://baike.vehdjk.com/Article/details/gdvgvdard.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.sjlbkw.cn/Article/details/gowjtxatk.sHtML

[Q64] 提交事务
来源：http://www.share.bbcook.cn/Article/details/gedigdmns.sHtML

COMMIT;
来源：http://read.share.fktsv.cn/Article/details/ghthdrjmi.sHtML

[Q65] 回滚事务
来源：http://www.share.sjlbkw.cn/Article/details/gtiragfwm.sHtML

ROLLBACK;
来源：http://blog.yfazqb.com/Article/details/gompgojpo.sHtML

[Q66] 行锁查询
来源：http://baike.yfazqb.com/Article/details/gwvfhjgvf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.bbcook.cn/Article/details/gxlhtxpdo.sHtML

[Q67] 设置隔离级别
来源：http://www.share.yfazqb.com/Article/details/glbavtckl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.sjlbkw.cn/Article/details/gxcbfqhsp.sHtML

[Q68] 保存点
来源：http://wap.tarul.cn/Article/details/gpsuzsija.sHtML

SAVEPOINT sp1;
来源：http://blog.bbcook.cn/Article/details/gvdqeflck.sHtML

ROLLBACK TO sp1;
来源：http://3g.fktsv.cn/Article/details/gtmwijhge.sHtML

[Q69] 查看执行计划
来源：http://www.blog.tarul.cn/Article/details/gcgovzzno.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.vehdjk.com/Article/details/giqoxctec.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/glfeddsjj.sHtML

ANALYZE TABLE users;
来源：http://wap.sjlbkw.cn/Article/details/gxlrvkjbb.sHtML

[Q71] 查看建表语句
来源：http://3g.tarul.cn/Article/details/gvrmnnyut.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.epnwcf.com/Article/details/gqrmjpsqb.sHtML

[Q72] 查看索引
来源：http://www.m.share.fktsv.cn/Article/details/gaglwrbuw.sHtML

SHOW INDEX FROM users;
来源：http://read.share.tarul.cn/Article/details/grpxyguli.sHtML

[Q73] 查看表状态
来源：http://m.share.bbcook.cn/Article/details/gnmvcrssn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.bbcook.cn/Article/details/gqeduagqs.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/gwfsstlmj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.yfazqb.com/Article/details/gqetzmtpn.sHtML

[Q75] 日期格式化
来源：http://baike.tarul.cn/Article/details/gcdeuqvun.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gmecfwilu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fktsv.cn/Article/details/gqtjngrit.sHtML

[Q76] 按天统计
来源：http://mobile.epnwcf.com/Article/details/gzvsdceqa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.yfazqb.com/Article/details/gdfrxaqir.sHtML

[Q77] 时间加减
来源：http://www.blog.tarul.cn/Article/details/gjzuaodus.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.tarul.cn/Article/details/gftqcsrhi.sHtML

[Q78] 当前时间
来源：http://wap.vehdjk.com/Article/details/gfwiyowmp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.bbcook.cn/Article/details/gbpzslewj.sHtML

[Q79] 字符串拼接
来源：http://blog.tarul.cn/Article/details/ggudlelad.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.sjlbkw.cn/Article/details/guxhchpar.sHtML

[Q80] 字符串截取
来源：http://www.blog.yfazqb.com/Article/details/gijxsnoxz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gahxekuki.sHtML

[Q81] 字符串替换
来源：http://baike.tarul.cn/Article/details/glvpkalaf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/gwudononz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/gxktmfspn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/guaiukwhf.sHtML

[Q83] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/guwtwmnnq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gfzoqyydf.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.yfazqb.com/Article/details/gjdanytcq.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gmxhwplcd.sHtML

[Q85] 数值取整
来源：http://mobile.bbcook.cn/Article/details/gaeudgrzd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.bbcook.cn/Article/details/gyxtprgam.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.bbcook.cn/Article/details/grjemlldi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.epnwcf.com/Article/details/ggmlzkhag.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.yfazqb.com/Article/details/gdbrgrghq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.yfazqb.com/Article/details/gebdiulgx.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.sjlbkw.cn/Article/details/grbiavvos.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.vehdjk.com/Article/details/goayiyeve.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.yfazqb.com/Article/details/gqohchoxq.sHtML

[Q89] 判断表是否存在
来源：http://baike.vehdjk.com/Article/details/gubsuwxhu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fktsv.cn/Article/details/gqbjlzwsq.sHtML

[Q90] 生成序号列
来源：http://baike.yfazqb.com/Article/details/glypspdho.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.tarul.cn/Article/details/geepfrfyn.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gqgmzuocg.sHtML

R. Bash 专题
来源：http://www.blog.yfazqb.com/Article/details/gffburvgb.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gckidtgku.sHtML

[R01] shebang 与严格模式
来源：http://3g.yfazqb.com/Article/details/gsahtestn.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.bbcook.cn/Article/details/grbemkeyl.sHtML

set -euo pipefail
来源：http://3g.tarul.cn/Article/details/gahjyownk.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fktsv.cn/Article/details/gwrcnptel.sHtML

name="Tom"; echo "$name"
来源：http://mobile.tarul.cn/Article/details/gocomuqsn.sHtML

[R03] 只读变量
来源：http://www.share.vehdjk.com/Article/details/gnxgdaklz.sHtML

readonly PI=3.14
来源：http://blog.fktsv.cn/Article/details/gzjojpkni.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/ggiwxusoj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.yfazqb.com/Article/details/gvytfwhxr.sHtML

[R05] 参数默认值
来源：http://mobile.yfazqb.com/Article/details/gvnumcekq.sHtML

name="${1:-default}"
来源：http://blog.tarul.cn/Article/details/gabmzpnuz.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.tarul.cn/Article/details/gqnuqultp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gzpctvgtr.sHtML

[R07] if 判断文件
来源：http://mobile.yfazqb.com/Article/details/gceaafmqz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.yfazqb.com/Article/details/gxmhnugog.sHtML

[R08] 数值比较
来源：http://3g.vehdjk.com/Article/details/gblexrred.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.yfazqb.com/Article/details/gzwjhhole.sHtML

[R09] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/glzrwbbng.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.epnwcf.com/Article/details/gpguuwuow.sHtML

[R10] 正则匹配
来源：http://blog.yfazqb.com/Article/details/gwhlfpohq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.vehdjk.com/Article/details/gzlqsrkqm.sHtML

[R11] case 多分支
来源：http://baike.fktsv.cn/Article/details/gkxtorenr.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/gmvhnpmia.sHtML

start) echo "启动" ;;
来源：http://m.share.epnwcf.com/Article/details/gkmjbhffi.sHtML

stop)  echo "停止" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gbkouzocc.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzecvsdcn.sHtML

esac
来源：http://m.share.sjlbkw.cn/Article/details/ginpnrdsg.sHtML

[R12] for 遍历文件
来源：http://read.share.sjlbkw.cn/Article/details/gklfczzuh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.sjlbkw.cn/Article/details/glisbecks.sHtML

[R13] for 计数循环
来源：http://blog.fktsv.cn/Article/details/gousyavfd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gogoiuazz.sHtML

[R14] C 风格 for
来源：http://m.share.yfazqb.com/Article/details/gdmwwrpqc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gjorqmzdz.sHtML

[R15] while 逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/goxzmvoyh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.tarul.cn/Article/details/glywipngb.sHtML

[R16] until 等待条件
来源：http://wap.vehdjk.com/Article/details/glacbtilz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/ghutjpxun.sHtML

[R17] 数组定义与取值
来源：http://blog.vehdjk.com/Article/details/ggklrpqcd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.yfazqb.com/Article/details/gcjbguhzd.sHtML

[R18] 遍历数组
来源：http://www.m.share.vehdjk.com/Article/details/gdpuvbbez.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/glrwzsube.sHtML

[R19] 数组长度
来源：http://m.share.fktsv.cn/Article/details/gujgtamzh.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.bbcook.cn/Article/details/gsyyxxehe.sHtML

[R20] 关联数组（字典）
来源：http://baike.tarul.cn/Article/details/gmooyuggj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.tarul.cn/Article/details/gxvvbvcdl.sHtML

[R21] 字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gqhxqnyms.sHtML

echo "${#s}"
来源：http://blog.fktsv.cn/Article/details/gskmhtuhf.sHtML

[R22] 截取子串
来源：http://baike.bbcook.cn/Article/details/gypnmdbmb.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/gdcpmwejb.sHtML

[R23] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gkhnvfufj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.yfazqb.com/Article/details/gwiwvaiju.sHtML

[R24] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gbdfzeboi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fktsv.cn/Article/details/gmosmgfgg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/govwjbeld.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.sjlbkw.cn/Article/details/gfnkozrvg.sHtML

[R26] 命令替换
来源：http://www.share.sjlbkw.cn/Article/details/gzutsiadr.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.tarul.cn/Article/details/gfeykqdbn.sHtML

[R27] 算术展开
来源：http://read.share.vehdjk.com/Article/details/glxfwjbsi.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.bbcook.cn/Article/details/gakmoowrr.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gkrthuprm.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.epnwcf.com/Article/details/giegvujir.sHtML

[R29] 定义函数
来源：http://read.share.tarul.cn/Article/details/gqszfoixs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fktsv.cn/Article/details/gmyvkbtvv.sHtML

[R30] 函数返回状态码
来源：http://m.share.sjlbkw.cn/Article/details/gnhfbrcaz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.vehdjk.com/Article/details/gthpzqdfm.sHtML

[R31] 局部变量
来源：http://3g.vehdjk.com/Article/details/gkthktzwj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.bbcook.cn/Article/details/gulktnfpq.sHtML

[R32] 参数个数校验
来源：http://blog.vehdjk.com/Article/details/gmgpzakuq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gfzhrfgfe.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.tarul.cn/Article/details/ghtytvxhn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fktsv.cn/Article/details/goegpkbbv.sHtML

[R34] 退出时清理
来源：http://read.share.yfazqb.com/Article/details/gpacahapb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gnapucbhs.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/gvnvaifde.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fktsv.cn/Article/details/gbvmcisip.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.tarul.cn/Article/details/gwibdciee.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fktsv.cn/Article/details/gcyafqxqi.sHtML

[R37] 把输出赋给变量
来源：http://www.share.sjlbkw.cn/Article/details/gdwxkitez.sHtML

files=$(ls -1)
来源：http://mobile.epnwcf.com/Article/details/gjfmsrbwr.sHtML

[R38] 管道串联
来源：http://mobile.yfazqb.com/Article/details/gsgpbhjze.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.bbcook.cn/Article/details/gmpzvrktb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/gtcgjciyi.sHtML

cmd > out.log 2>&1
来源：http://baike.fktsv.cn/Article/details/gnjlxskdq.sHtML

[R40] 追加写日志
来源：http://www.share.yfazqb.com/Article/details/gzplbvxgh.sHtML

echo "log" >> out.log
来源：http://baike.tarul.cn/Article/details/gqabwgjhh.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/gcnqqgxkc.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.tarul.cn/Article/details/glmvhkkxc.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/grwpzpgon.sHtML

wc -l < a.txt
来源：http://mobile.epnwcf.com/Article/details/gpablnwgp.sHtML

[R43] 按名字查找文件
来源：http://m.share.bbcook.cn/Article/details/gbytuowdw.sHtML

find . -name "*.log" -type f
来源：http://3g.bbcook.cn/Article/details/gtcbnxjia.sHtML

[R44] 按修改时间查找
来源：http://baike.sjlbkw.cn/Article/details/gspdjkrlf.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/glaodrwvq.sHtML

[R45] 批量删除
来源：http://mobile.vehdjk.com/Article/details/grotqiqhg.sHtML

find . -name "*.tmp" -delete
来源：http://baike.tarul.cn/Article/details/glydytgar.sHtML

[R46] 递归替换文件内容
来源：http://m.share.tarul.cn/Article/details/gbocdnmev.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.sjlbkw.cn/Article/details/gvuustdgk.sHtML

[R47] sed 单行替换
来源：http://www.blog.fktsv.cn/Article/details/glhmpwfss.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fktsv.cn/Article/details/gbwqkbvoy.sHtML

[R48] awk 取指定列
来源：http://www.share.tarul.cn/Article/details/gayqibndl.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fktsv.cn/Article/details/gsotktkft.sHtML

[R49] awk 带条件
来源：http://baike.epnwcf.com/Article/details/ghkeajxap.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.yfazqb.com/Article/details/glnqlwild.sHtML

[R50] awk 求和
来源：http://blog.yfazqb.com/Article/details/gshzwsiyh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.bbcook.cn/Article/details/gcvqzlikd.sHtML

[R51] 排序去重取前几
来源：http://www.share.sjlbkw.cn/Article/details/gvgvlijyl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fktsv.cn/Article/details/giggypexj.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/grwiejwwu.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gtuafgnoe.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.yfazqb.com/Article/details/gqhcwumpx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.yfazqb.com/Article/details/gbdlnglkn.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjqgenrz.sHtML

diff a.txt b.txt
来源：http://www.m.share.tarul.cn/Article/details/gyagbdzmp.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/gqutmmnab.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fktsv.cn/Article/details/goqpwkglq.sHtML

[R56] 远程拷贝
来源：http://baike.sjlbkw.cn/Article/details/gyzmaxcms.sHtML

scp file user@host:/path/
来源：http://www.share.vehdjk.com/Article/details/gkifeplka.sHtML

[R57] 远程执行命令
来源：http://m.share.yfazqb.com/Article/details/grtvezbua.sHtML

ssh user@host 'uptime'
来源：http://baike.fktsv.cn/Article/details/gfdedmnlj.sHtML

[R58] 下载文件
来源：http://www.blog.bbcook.cn/Article/details/gjvrzfecm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.vehdjk.com/Article/details/gzscdggoy.sHtML

[R59] 发 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gmoukvhko.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.epnwcf.com/Article/details/gogkvpmqk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gewfbnnfa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.bbcook.cn/Article/details/gvzmutxmj.sHtML

[R61] 磁盘占用
来源：http://read.share.epnwcf.com/Article/details/gzmgnpzbw.sHtML

df -h;  du -sh *
来源：http://read.share.fktsv.cn/Article/details/gqixeugdo.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fktsv.cn/Article/details/gnhwtoqmv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.vehdjk.com/Article/details/gatiupzdr.sHtML

[R63] 内存与进程
来源：http://3g.epnwcf.com/Article/details/gaatwxmze.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.epnwcf.com/Article/details/gghbbothf.sHtML

[R64] 结束进程
来源：http://wap.bbcook.cn/Article/details/gtyawerjr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.bbcook.cn/Article/details/gecvdboly.sHtML

[R65] 查看端口占用
来源：http://www.share.epnwcf.com/Article/details/grevkynvh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.vehdjk.com/Article/details/gdepzmygx.sHtML

[R66] 定时任务
来源：http://baike.epnwcf.com/Article/details/gpdzveksa.sHtML

crontab -e;  crontab -l
来源：http://blog.epnwcf.com/Article/details/gjdnubcaj.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.epnwcf.com/Article/details/ggkdrfqvm.sHtML

openssl rand -hex 16
来源：http://3g.tarul.cn/Article/details/gvujnepis.sHtML

[R68] 计算文件校验值
来源：http://blog.vehdjk.com/Article/details/gvjasdxpx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fktsv.cn/Article/details/gcmkejjtr.sHtML

[R69] 生成随机密码
来源：http://read.share.bbcook.cn/Article/details/gpovvgxnn.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fktsv.cn/Article/details/gzupogvyz.sHtML

[R70] 时间戳与互转
来源：http://wap.vehdjk.com/Article/details/guayrgetn.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/gzvnvyldd.sHtML

[R71] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gtzimkwid.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fktsv.cn/Article/details/ggjoxzbvt.sHtML

[R72] 等待端口就绪
来源：http://www.share.yfazqb.com/Article/details/ghwieyzpf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gmsfudkmt.sHtML

[R73] 分割大日志
来源：http://m.share.fktsv.cn/Article/details/gzhbfwdyu.sHtML

split -l 1000 big.log part_
来源：http://m.share.tarul.cn/Article/details/gxyzsorfj.sHtML

[R74] 批量重命名
来源：http://read.share.vehdjk.com/Article/details/grqpyxoch.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/gtekslsvr.sHtML

[R75] 导出环境变量
来源：http://3g.vehdjk.com/Article/details/gendgjqgm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.yfazqb.com/Article/details/gcgbqapzw.sHtML

[R76] 使用临时文件
来源：http://m.share.tarul.cn/Article/details/ggemqsakd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/geppzorel.sHtML

[R77] 读取用户输入
来源：http://wap.sjlbkw.cn/Article/details/goxexzaim.sHtML

read -rp "请输入: " ans
来源：http://wap.yfazqb.com/Article/details/gqmkpftmu.sHtML

[R78] 交互式菜单
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsmgtigo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.vehdjk.com/Article/details/gltcsjpik.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/gruguqxgb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.bbcook.cn/Article/details/gnvwuwulf.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fktsv.cn/Article/details/gictjafvv.sHtML

time ./run.sh
来源：http://www.share.sjlbkw.cn/Article/details/gzjpmhtod.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/guyoohrwb.sHtML

S. C / C++ 专题
来源：http://blog.tarul.cn/Article/details/gzwanqqwm.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gpxkenqsr.sHtML

[S01] C：Hello World
来源：http://read.share.tarul.cn/Article/details/ghohdobwb.sHtML

#include <stdio.h>
来源：http://baike.tarul.cn/Article/details/gsyfqaecr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.sjlbkw.cn/Article/details/gyofzcuoa.sHtML

[S02] C：变量与格式化输出
来源：http://baike.vehdjk.com/Article/details/gzbhiwmxy.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.sjlbkw.cn/Article/details/gupugjwnh.sHtML

[S03] C：读入整数
来源：http://m.share.tarul.cn/Article/details/gbbeoilhu.sHtML

int x; scanf("%d", &x);
来源：http://baike.fktsv.cn/Article/details/gqvazhnnq.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/gqryknfkl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/gbbeqjpkv.sHtML

[S05] C：字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gwjasmbuh.sHtML

strlen(s)
来源：http://wap.epnwcf.com/Article/details/gcdmfvzvs.sHtML

[S06] C：字符串比较
来源：http://read.share.yfazqb.com/Article/details/gdyhrrpeb.sHtML

strcmp(a, b) == 0
来源：http://3g.tarul.cn/Article/details/ghfxirkeb.sHtML

[S07] C：数组遍历求和
来源：http://wap.sjlbkw.cn/Article/details/gttbjglgs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.bbcook.cn/Article/details/ggvusgeem.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gzposvoop.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.epnwcf.com/Article/details/ggpqutcvj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.vehdjk.com/Article/details/gjnukkbqy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.epnwcf.com/Article/details/gmysggixk.sHtML

[S10] C：指针与解引用
来源：http://blog.epnwcf.com/Article/details/gsbcqbgta.sHtML

int *p = &a;  *p = 5;
来源：http://3g.bbcook.cn/Article/details/gqrqmchzh.sHtML

[S11] C：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gdjuxbdpp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.tarul.cn/Article/details/gdelruozu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.bbcook.cn/Article/details/gqyrhcowo.sHtML

fclose(f);
来源：http://www.share.tarul.cn/Article/details/gsxcedezk.sHtML

[S12] C：写文件
来源：http://wap.fktsv.cn/Article/details/gtacbcwkc.sHtML


<!-- 参考信息 -->