代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://blog.yfazqb.com/Article/details/gobmuwtcb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gcbpejysd.sHtML

[Q47] 与平均值比较
来源：http://mobile.yfazqb.com/Article/details/gdenxrjli.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.sjlbkw.cn/Article/details/gxdmbeego.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.vehdjk.com/Article/details/gukeqliya.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/ggyrqxvsw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.bbcook.cn/Article/details/gctbovnnd.sHtML

[Q49] 更新单行
来源：http://m.share.bbcook.cn/Article/details/gncsjwpbn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gckbafwxu.sHtML

[Q50] 批量更新
来源：http://wap.vehdjk.com/Article/details/gejgurjua.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gefpidqtc.sHtML

[Q51] 用子查询更新
来源：http://www.share.bbcook.cn/Article/details/gxubyzioa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.epnwcf.com/Article/details/gshqlnqir.sHtML

[Q52] 删除指定行
来源：http://3g.epnwcf.com/Article/details/gabdhzsze.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gvgqlmdui.sHtML

[Q53] 按条件删除
来源：http://blog.sjlbkw.cn/Article/details/gcgbxmxab.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.yfazqb.com/Article/details/grpyagtzo.sHtML

[Q54] 清空表
来源：http://www.m.share.vehdjk.com/Article/details/gbmppkwkp.sHtML

TRUNCATE TABLE logs;
来源：http://3g.bbcook.cn/Article/details/gcxzqmvch.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.sjlbkw.cn/Article/details/guzapqqjt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gkaysastz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.tarul.cn/Article/details/gevcaziun.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.bbcook.cn/Article/details/gamzmxekv.sHtML

[Q57] 行号
来源：http://baike.sjlbkw.cn/Article/details/gdwzyynzj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gsuuihdro.sHtML

[Q58] 累计求和
来源：http://read.share.bbcook.cn/Article/details/gqxwximxe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gfhirrdtf.sHtML

[Q59] 分组内累计
来源：http://3g.epnwcf.com/Article/details/gbxjahgzj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gpyudmgpk.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fktsv.cn/Article/details/gorlpepyz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.tarul.cn/Article/details/gxnjvlpyi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.bbcook.cn/Article/details/gozcbaucn.sHtML

[Q61] 移动平均
来源：http://blog.tarul.cn/Article/details/gvtlmyabl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gbcsilbaa.sHtML

[Q62] 分组占比
来源：http://www.blog.vehdjk.com/Article/details/gfkxiibaj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gcmstgjtw.sHtML

[Q63] 开启事务
来源：http://baike.tarul.cn/Article/details/gveiiyvir.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.epnwcf.com/Article/details/gnlojtvzm.sHtML

[Q64] 提交事务
来源：http://3g.sjlbkw.cn/Article/details/gflwfhqza.sHtML

COMMIT;
来源：http://read.share.tarul.cn/Article/details/gksdtzdna.sHtML

[Q65] 回滚事务
来源：http://blog.epnwcf.com/Article/details/gaedymqoh.sHtML

ROLLBACK;
来源：http://read.share.yfazqb.com/Article/details/gtztgekfx.sHtML

[Q66] 行锁查询
来源：http://wap.epnwcf.com/Article/details/glxcqhmec.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.vehdjk.com/Article/details/gwogjkcga.sHtML

[Q67] 设置隔离级别
来源：http://mobile.tarul.cn/Article/details/gbrssucuf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.tarul.cn/Article/details/gcrujlqwn.sHtML

[Q68] 保存点
来源：http://read.share.fktsv.cn/Article/details/gwyoyxtae.sHtML

SAVEPOINT sp1;
来源：http://wap.vehdjk.com/Article/details/gixgbkopv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fktsv.cn/Article/details/gagkiuvvt.sHtML

[Q69] 查看执行计划
来源：http://wap.epnwcf.com/Article/details/grqwjolxe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.epnwcf.com/Article/details/gsziaboea.sHtML

[Q70] 更新统计信息
来源：http://wap.yfazqb.com/Article/details/gycgihtiq.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.epnwcf.com/Article/details/geaiqwrdp.sHtML

[Q71] 查看建表语句
来源：http://wap.yfazqb.com/Article/details/gdqkzxtpr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fktsv.cn/Article/details/gsitqsveq.sHtML

[Q72] 查看索引
来源：http://read.share.sjlbkw.cn/Article/details/gqaahvtnp.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fktsv.cn/Article/details/goejplqfc.sHtML

[Q73] 查看表状态
来源：http://m.share.tarul.cn/Article/details/gndzgwftp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.yfazqb.com/Article/details/gtetctzfa.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.tarul.cn/Article/details/gogvyafxi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.epnwcf.com/Article/details/gcguztpod.sHtML

[Q75] 日期格式化
来源：http://baike.tarul.cn/Article/details/ggpbvruqs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.vehdjk.com/Article/details/grbmogghv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.tarul.cn/Article/details/gzxrlpcsr.sHtML

[Q76] 按天统计
来源：http://3g.sjlbkw.cn/Article/details/gnurxzjaq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.sjlbkw.cn/Article/details/ggmodexcf.sHtML

[Q77] 时间加减
来源：http://wap.sjlbkw.cn/Article/details/glkjbxpbp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.epnwcf.com/Article/details/gnxrserca.sHtML

[Q78] 当前时间
来源：http://m.share.yfazqb.com/Article/details/gicrnmzya.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fktsv.cn/Article/details/gphybrtor.sHtML

[Q79] 字符串拼接
来源：http://baike.tarul.cn/Article/details/gqwsxrqqg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.sjlbkw.cn/Article/details/grudpukwe.sHtML

[Q80] 字符串截取
来源：http://www.share.yfazqb.com/Article/details/grwnwsgld.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gpuoukjdc.sHtML

[Q81] 字符串替换
来源：http://read.share.tarul.cn/Article/details/ghijtkglp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fktsv.cn/Article/details/gazhgzxsg.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.bbcook.cn/Article/details/girqsukmr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gjqgqnpdj.sHtML

[Q83] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gdltowbxq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gneokoxpi.sHtML

[Q84] 去除首尾空格
来源：http://wap.tarul.cn/Article/details/gdkwiuuau.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gjggvmmtd.sHtML

[Q85] 数值取整
来源：http://mobile.yfazqb.com/Article/details/glsuqktcc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.epnwcf.com/Article/details/gsfcgxcwl.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fktsv.cn/Article/details/gubwslzda.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.bbcook.cn/Article/details/ggotzupvh.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.sjlbkw.cn/Article/details/gylswppmo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.sjlbkw.cn/Article/details/ghsmvakio.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.tarul.cn/Article/details/gdpgivhux.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.vehdjk.com/Article/details/ggaikkylu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.bbcook.cn/Article/details/gjatrkuyl.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.bbcook.cn/Article/details/gnjlaritj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.bbcook.cn/Article/details/gdubhidra.sHtML

[Q90] 生成序号列
来源：http://m.share.vehdjk.com/Article/details/glfcdrdqf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.bbcook.cn/Article/details/gdktclrsa.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkepwexae.sHtML

R. Bash 专题
来源：http://wap.tarul.cn/Article/details/gyzikoszb.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsnqgsvp.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/gnelisibx.sHtML

#!/usr/bin/env bash
来源：http://wap.fktsv.cn/Article/details/getyvxkea.sHtML

set -euo pipefail
来源：http://read.share.bbcook.cn/Article/details/gxymppnbt.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.vehdjk.com/Article/details/gwamqvjhw.sHtML

name="Tom"; echo "$name"
来源：http://baike.bbcook.cn/Article/details/gomujkzxh.sHtML

[R03] 只读变量
来源：http://baike.tarul.cn/Article/details/guyzrjzgr.sHtML

readonly PI=3.14
来源：http://blog.sjlbkw.cn/Article/details/gotwuvafw.sHtML

[R04] 位置参数
来源：http://baike.tarul.cn/Article/details/gutazkauh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fktsv.cn/Article/details/gpzexnorc.sHtML

[R05] 参数默认值
来源：http://blog.fktsv.cn/Article/details/gmpkajyrz.sHtML

name="${1:-default}"
来源：http://read.share.yfazqb.com/Article/details/gzorstesd.sHtML

[R06] 判断命令是否存在
来源：http://m.share.tarul.cn/Article/details/gkdggmjxr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/gthgzausm.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gfmjkxmvz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.sjlbkw.cn/Article/details/gzpcarnia.sHtML

[R08] 数值比较
来源：http://baike.sjlbkw.cn/Article/details/gczxfrewx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.tarul.cn/Article/details/gaawbhgad.sHtML

[R09] 字符串比较
来源：http://wap.yfazqb.com/Article/details/gbxozfibk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/gucsbgawr.sHtML

[R10] 正则匹配
来源：http://www.blog.vehdjk.com/Article/details/gaefzrssr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.bbcook.cn/Article/details/gjbbqhegt.sHtML

[R11] case 多分支
来源：http://read.share.sjlbkw.cn/Article/details/gokupxlok.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/gtbznwlhd.sHtML

start) echo "启动" ;;
来源：http://wap.fktsv.cn/Article/details/gepypuhxd.sHtML

stop)  echo "停止" ;;
来源：http://3g.vehdjk.com/Article/details/gxnsbzyvo.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.sjlbkw.cn/Article/details/ghvhadqgh.sHtML

esac
来源：http://www.blog.bbcook.cn/Article/details/gmriderge.sHtML

[R12] for 遍历文件
来源：http://wap.vehdjk.com/Article/details/gvqhxgklh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.sjlbkw.cn/Article/details/gcqpmfeit.sHtML

[R13] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/gfcgzzcnh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gykzrdfvz.sHtML

[R14] C 风格 for
来源：http://blog.sjlbkw.cn/Article/details/gtfmgevbk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gnnpmsdsb.sHtML

[R15] while 逐行读文件
来源：http://3g.epnwcf.com/Article/details/gyaqzjcdp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.bbcook.cn/Article/details/gelyclmcp.sHtML

[R16] until 等待条件
来源：http://baike.fktsv.cn/Article/details/ggjxmannc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/gitjupfvh.sHtML

[R17] 数组定义与取值
来源：http://mobile.yfazqb.com/Article/details/gxkdmdsps.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.tarul.cn/Article/details/geqicvayf.sHtML

[R18] 遍历数组
来源：http://3g.tarul.cn/Article/details/ginddhqrc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.vehdjk.com/Article/details/gbuwffbsy.sHtML

[R19] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gfziuqxhx.sHtML

echo "${#arr[@]}"
来源：http://www.share.tarul.cn/Article/details/gzycncaee.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.epnwcf.com/Article/details/glwbmbzni.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gltbofjpi.sHtML

[R21] 字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gepocheom.sHtML

echo "${#s}"
来源：http://read.share.tarul.cn/Article/details/gyszigltc.sHtML

[R22] 截取子串
来源：http://baike.epnwcf.com/Article/details/gntjmsnpl.sHtML

echo "${s:0:5}"
来源：http://blog.sjlbkw.cn/Article/details/gnkzfecpi.sHtML

[R23] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gqjxdptbj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.epnwcf.com/Article/details/gmqpekskb.sHtML

[R24] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gnhpxdwkg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.sjlbkw.cn/Article/details/goxqrfjgh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.tarul.cn/Article/details/gqrautetl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.bbcook.cn/Article/details/gxobcqfqd.sHtML

[R26] 命令替换
来源：http://mobile.epnwcf.com/Article/details/gyyzcsrmq.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.yfazqb.com/Article/details/gozijpbjr.sHtML

[R27] 算术展开
来源：http://m.share.sjlbkw.cn/Article/details/gxkzbagdk.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.vehdjk.com/Article/details/guvvmruri.sHtML

[R28] 浮点运算
来源：http://wap.fktsv.cn/Article/details/glafrhvxz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.yfazqb.com/Article/details/gqxzkzima.sHtML

[R29] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/ganpymqdd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.tarul.cn/Article/details/girtavzkl.sHtML

[R30] 函数返回状态码
来源：http://read.share.bbcook.cn/Article/details/gxspzppee.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.sjlbkw.cn/Article/details/ghdmyaywr.sHtML

[R31] 局部变量
来源：http://www.blog.epnwcf.com/Article/details/gaieiuowh.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.vehdjk.com/Article/details/gombpkfcf.sHtML

[R32] 参数个数校验
来源：http://baike.fktsv.cn/Article/details/geajwhlhq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/ggkzehach.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.vehdjk.com/Article/details/ggnraxhbw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.yfazqb.com/Article/details/gfarsjvqz.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/gmfcjgbcy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/ghjgtyxox.sHtML

[R35] 后台执行并等待
来源：http://3g.tarul.cn/Article/details/gmcljvdvp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.tarul.cn/Article/details/gykoikavl.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/geaxybdno.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.yfazqb.com/Article/details/ggmiaqjqg.sHtML

[R37] 把输出赋给变量
来源：http://wap.yfazqb.com/Article/details/gvpuifvup.sHtML

files=$(ls -1)
来源：http://wap.vehdjk.com/Article/details/gzzdwqomb.sHtML

[R38] 管道串联
来源：http://3g.bbcook.cn/Article/details/gerntjosh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.vehdjk.com/Article/details/gkgietsmg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.yfazqb.com/Article/details/gdhgcsckd.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gcjngkhjv.sHtML

[R40] 追加写日志
来源：http://wap.vehdjk.com/Article/details/grkpvtrrm.sHtML

echo "log" >> out.log
来源：http://wap.vehdjk.com/Article/details/gxapryulm.sHtML

[R41] 丢弃输出
来源：http://mobile.bbcook.cn/Article/details/godumvmho.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.yfazqb.com/Article/details/ghhiogvtd.sHtML

[R42] 输入重定向
来源：http://baike.tarul.cn/Article/details/gjfiblwts.sHtML

wc -l < a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gugnjeafv.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/gabrpmabi.sHtML

find . -name "*.log" -type f
来源：http://www.blog.vehdjk.com/Article/details/gmtnimyae.sHtML

[R44] 按修改时间查找
来源：http://wap.epnwcf.com/Article/details/gzbsetkld.sHtML

find . -mtime -7 -type f
来源：http://read.share.bbcook.cn/Article/details/gasgxygrw.sHtML

[R45] 批量删除
来源：http://mobile.epnwcf.com/Article/details/gdiqljbcv.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.yfazqb.com/Article/details/gqeixpafp.sHtML

[R46] 递归替换文件内容
来源：http://www.share.vehdjk.com/Article/details/gtbrewblr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fktsv.cn/Article/details/gwouodvag.sHtML

[R47] sed 单行替换
来源：http://www.share.tarul.cn/Article/details/gunzzcdiy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.tarul.cn/Article/details/gbuzlxzbh.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/gmyoxrpoe.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.yfazqb.com/Article/details/gdeetmrim.sHtML

[R49] awk 带条件
来源：http://3g.epnwcf.com/Article/details/gaiapaghd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.vehdjk.com/Article/details/gpgnprylh.sHtML

[R50] awk 求和
来源：http://m.share.fktsv.cn/Article/details/gqvlxgnyt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gpfbeluso.sHtML

[R51] 排序去重取前几
来源：http://www.share.sjlbkw.cn/Article/details/gaxkwabux.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.sjlbkw.cn/Article/details/gofpohhzo.sHtML

[R52] 统计行数
来源：http://blog.yfazqb.com/Article/details/grgyfgasd.sHtML

wc -l a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gdyhhylkp.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.vehdjk.com/Article/details/glrkzbcmi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.sjlbkw.cn/Article/details/gsfeiypbx.sHtML

[R54] 比较两个文件
来源：http://m.share.epnwcf.com/Article/details/gxgixsfmg.sHtML

diff a.txt b.txt
来源：http://www.blog.vehdjk.com/Article/details/ghzqgsdyz.sHtML

[R55] 压缩与解压
来源：http://wap.tarul.cn/Article/details/gfdwzigdb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.vehdjk.com/Article/details/gosfvgthm.sHtML

[R56] 远程拷贝
来源：http://baike.epnwcf.com/Article/details/gpccbpbhp.sHtML

scp file user@host:/path/
来源：http://www.m.share.epnwcf.com/Article/details/gtfvvbtwr.sHtML

[R57] 远程执行命令
来源：http://baike.tarul.cn/Article/details/gsehwdisg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.epnwcf.com/Article/details/glseshhby.sHtML

[R58] 下载文件
来源：http://mobile.yfazqb.com/Article/details/gatzoffse.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.tarul.cn/Article/details/ghaqqvbnh.sHtML

[R59] 发 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/glvoukjdn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.tarul.cn/Article/details/gdduekqkh.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/gwnxxnekx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.yfazqb.com/Article/details/gjhgtscxi.sHtML

[R61] 磁盘占用
来源：http://www.blog.yfazqb.com/Article/details/gptgignhh.sHtML

df -h;  du -sh *
来源：http://m.share.tarul.cn/Article/details/gbldjulpl.sHtML

[R62] 找最占空间的文件
来源：http://baike.tarul.cn/Article/details/gjchrchuv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fktsv.cn/Article/details/gcwweaxtn.sHtML

[R63] 内存与进程
来源：http://baike.fktsv.cn/Article/details/gsmmyhfxw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.yfazqb.com/Article/details/gzkgxdnlk.sHtML

[R64] 结束进程
来源：http://read.share.tarul.cn/Article/details/gqdyococn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/gmbdjokqp.sHtML

[R65] 查看端口占用
来源：http://mobile.sjlbkw.cn/Article/details/gbvncqncu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.sjlbkw.cn/Article/details/geajkqsyu.sHtML

[R66] 定时任务
来源：http://blog.yfazqb.com/Article/details/gqastmiby.sHtML

crontab -e;  crontab -l
来源：http://mobile.sjlbkw.cn/Article/details/gwthgepdg.sHtML

[R67] 生成随机十六进制串
来源：http://3g.yfazqb.com/Article/details/gokwfgido.sHtML

openssl rand -hex 16
来源：http://3g.yfazqb.com/Article/details/gqfipmnlg.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/gudclkudj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.sjlbkw.cn/Article/details/gknfcbswl.sHtML

[R69] 生成随机密码
来源：http://read.share.sjlbkw.cn/Article/details/grjmylqki.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.epnwcf.com/Article/details/gqlphgvza.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/gtigfxavn.sHtML

date +%s;  date -d @1700000000
来源：http://blog.epnwcf.com/Article/details/gvypnbtzm.sHtML

[R71] 日期格式化
来源：http://blog.epnwcf.com/Article/details/gmcvnyemi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.yfazqb.com/Article/details/gmmptvuwl.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.vehdjk.com/Article/details/glygnqgcg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gtwisayrr.sHtML

[R73] 分割大日志
来源：http://3g.yfazqb.com/Article/details/ggqcrykmx.sHtML

split -l 1000 big.log part_
来源：http://baike.yfazqb.com/Article/details/gtcqcrxsp.sHtML

[R74] 批量重命名
来源：http://wap.vehdjk.com/Article/details/gikbmomxl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.epnwcf.com/Article/details/gpsucoaqf.sHtML

[R75] 导出环境变量
来源：http://m.share.vehdjk.com/Article/details/gkdwvzxsr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.bbcook.cn/Article/details/gvvhvjdse.sHtML

[R76] 使用临时文件
来源：http://m.share.tarul.cn/Article/details/gbnqibeqw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gcipteycn.sHtML

[R77] 读取用户输入
来源：http://www.m.share.epnwcf.com/Article/details/gomumimdr.sHtML

read -rp "请输入: " ans
来源：http://mobile.tarul.cn/Article/details/gbihdgkqg.sHtML

[R78] 交互式菜单
来源：http://3g.bbcook.cn/Article/details/gpxwdvnwj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.yfazqb.com/Article/details/gynyfutrz.sHtML

[R79] 解析命令行选项
来源：http://www.share.sjlbkw.cn/Article/details/gscvigzlj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.bbcook.cn/Article/details/gvhfxrxcl.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.epnwcf.com/Article/details/gszvhbgsd.sHtML

time ./run.sh
来源：http://blog.tarul.cn/Article/details/gthixfjcn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpmolgkwh.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/gwtkwgmrh.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gtjasjqii.sHtML

[S01] C：Hello World
来源：http://3g.tarul.cn/Article/details/gqchmgtdb.sHtML

#include <stdio.h>
来源：http://mobile.sjlbkw.cn/Article/details/gcvlzydzv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fktsv.cn/Article/details/gjvdhjzgq.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gjorajlgb.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.tarul.cn/Article/details/gqxwdsgic.sHtML

[S03] C：读入整数
来源：http://wap.bbcook.cn/Article/details/gmvtfeswi.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.bbcook.cn/Article/details/gqmhifojm.sHtML

[S04] C：字符串复制
来源：http://read.share.sjlbkw.cn/Article/details/gysgyndqu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gwokapdnl.sHtML

[S05] C：字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gqzhnwose.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/gffosetmy.sHtML

[S06] C：字符串比较
来源：http://read.share.tarul.cn/Article/details/gtzjprurf.sHtML

strcmp(a, b) == 0
来源：http://3g.bbcook.cn/Article/details/gkztzbphh.sHtML

[S07] C：数组遍历求和
来源：http://www.share.bbcook.cn/Article/details/gzjjoxpdi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/gijgzgily.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.tarul.cn/Article/details/gqaugmgum.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.tarul.cn/Article/details/gfkulqlnp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.vehdjk.com/Article/details/gbpvxdrde.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/gffuelnbp.sHtML

[S10] C：指针与解引用
来源：http://read.share.yfazqb.com/Article/details/gstjodzsn.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.tarul.cn/Article/details/gbkagqktn.sHtML

[S11] C：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gicxzexpa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.yfazqb.com/Article/details/gwenmenri.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fktsv.cn/Article/details/gflelnwld.sHtML

fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtccgwum.sHtML

[S12] C：写文件
来源：http://read.share.vehdjk.com/Article/details/gpxjnizkt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.epnwcf.com/Article/details/gurwimscv.sHtML

[S13] C：宏定义
来源：http://wap.sjlbkw.cn/Article/details/glzbozepu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.yfazqb.com/Article/details/gbbtfjqlq.sHtML

[S14] C：枚举
来源：http://m.share.yfazqb.com/Article/details/gaiptaapz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.bbcook.cn/Article/details/gkizfrwoz.sHtML

[S15] C：类型转换
来源：http://3g.epnwcf.com/Article/details/gxfcmplyf.sHtML

(double) a / b
来源：http://3g.tarul.cn/Article/details/guoapewne.sHtML

[S16] C：位操作置位
来源：http://wap.epnwcf.com/Article/details/gzlxmetjw.sHtML


<!-- 参考信息 -->