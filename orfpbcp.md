代发 wailian999

[Q44] IN 子查询
来源：http://mobile.yfazqb.com/Article/details/glowjyzwl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.yfazqb.com/Article/details/gdddhmeaj.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.epnwcf.com/Article/details/gqsxissfd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gorkvemmm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.epnwcf.com/Article/details/gabdkmjab.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gkaiuqxun.sHtML

[Q47] 与平均值比较
来源：http://m.share.tarul.cn/Article/details/gfqaeqxgu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.tarul.cn/Article/details/gggsycspl.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.epnwcf.com/Article/details/gkaefobjw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.epnwcf.com/Article/details/gkjdpwybk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.tarul.cn/Article/details/gnuzptidr.sHtML

[Q49] 更新单行
来源：http://wap.vehdjk.com/Article/details/gcdlxntew.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/gzlylqcvt.sHtML

[Q50] 批量更新
来源：http://blog.epnwcf.com/Article/details/geylgmjir.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.vehdjk.com/Article/details/guzyfetix.sHtML

[Q51] 用子查询更新
来源：http://blog.epnwcf.com/Article/details/groagedlg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.yfazqb.com/Article/details/ggabkxkcv.sHtML

[Q52] 删除指定行
来源：http://wap.epnwcf.com/Article/details/gheethefe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.tarul.cn/Article/details/gdztgubpp.sHtML

[Q53] 按条件删除
来源：http://www.blog.sjlbkw.cn/Article/details/gcnoakxck.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.bbcook.cn/Article/details/gzvlqshos.sHtML

[Q54] 清空表
来源：http://blog.tarul.cn/Article/details/gmzmsldnf.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.sjlbkw.cn/Article/details/gyxmcakor.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.bbcook.cn/Article/details/gbbzxniyu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gkaqgxcrt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.tarul.cn/Article/details/gewmckkje.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gluepxbug.sHtML

[Q57] 行号
来源：http://read.share.vehdjk.com/Article/details/gseslrgxv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gwslkbxsh.sHtML

[Q58] 累计求和
来源：http://www.blog.tarul.cn/Article/details/glsonsgeb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.tarul.cn/Article/details/ghumkuaor.sHtML

[Q59] 分组内累计
来源：http://wap.yfazqb.com/Article/details/gyvuxhsgn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gvlyoalfv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.epnwcf.com/Article/details/gozqikmlu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.tarul.cn/Article/details/gvcxpbzno.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.vehdjk.com/Article/details/ghkkqlqka.sHtML

[Q61] 移动平均
来源：http://m.share.bbcook.cn/Article/details/gnuzzlpfi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gneyfopkq.sHtML

[Q62] 分组占比
来源：http://www.share.bbcook.cn/Article/details/gjkgdxsaf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gwoytddar.sHtML

[Q63] 开启事务
来源：http://mobile.fktsv.cn/Article/details/gmyqhtdtm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.sjlbkw.cn/Article/details/gllzzckwl.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/grrhxggod.sHtML

COMMIT;
来源：http://blog.bbcook.cn/Article/details/gnabybsdz.sHtML

[Q65] 回滚事务
来源：http://read.share.bbcook.cn/Article/details/gqrkcctrg.sHtML

ROLLBACK;
来源：http://wap.vehdjk.com/Article/details/gnokvhwii.sHtML

[Q66] 行锁查询
来源：http://blog.bbcook.cn/Article/details/gqwvblaxw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.tarul.cn/Article/details/glmwnmscq.sHtML

[Q67] 设置隔离级别
来源：http://mobile.vehdjk.com/Article/details/guonlxssn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.tarul.cn/Article/details/guwskopac.sHtML

[Q68] 保存点
来源：http://www.blog.bbcook.cn/Article/details/gqxluyhhl.sHtML

SAVEPOINT sp1;
来源：http://www.share.fktsv.cn/Article/details/glfvipawj.sHtML

ROLLBACK TO sp1;
来源：http://www.share.yfazqb.com/Article/details/ghslsbiug.sHtML

[Q69] 查看执行计划
来源：http://www.share.tarul.cn/Article/details/glcydudrk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.bbcook.cn/Article/details/gpnkshauk.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/glyhiyifn.sHtML

ANALYZE TABLE users;
来源：http://blog.fktsv.cn/Article/details/gbuuoscar.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.yfazqb.com/Article/details/gydllhgts.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.vehdjk.com/Article/details/gzncchymk.sHtML

[Q72] 查看索引
来源：http://m.share.vehdjk.com/Article/details/gutpjrwfi.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gvddpiule.sHtML

[Q73] 查看表状态
来源：http://m.share.yfazqb.com/Article/details/gcptnfxoe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.bbcook.cn/Article/details/gmznyzbmz.sHtML

[Q74] 强制使用索引
来源：http://mobile.fktsv.cn/Article/details/ghrxznonm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.yfazqb.com/Article/details/gnddwpgjs.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/gkxhmiaex.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gyydtijda.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.epnwcf.com/Article/details/gsvgrzndr.sHtML

[Q76] 按天统计
来源：http://www.share.epnwcf.com/Article/details/gzmwqnsmf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.epnwcf.com/Article/details/gzuplknpx.sHtML

[Q77] 时间加减
来源：http://www.blog.sjlbkw.cn/Article/details/gzdypgfjz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.tarul.cn/Article/details/gtnygjbqk.sHtML

[Q78] 当前时间
来源：http://www.share.vehdjk.com/Article/details/gumhzfbdo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.epnwcf.com/Article/details/gkcboqjzc.sHtML

[Q79] 字符串拼接
来源：http://read.share.yfazqb.com/Article/details/grbtxmqtq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.bbcook.cn/Article/details/gdjpuqbnp.sHtML

[Q80] 字符串截取
来源：http://www.share.fktsv.cn/Article/details/gqffeknvt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gckrqgjrz.sHtML

[Q81] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gtisnpsog.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.epnwcf.com/Article/details/gmqiqlndq.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.yfazqb.com/Article/details/ghvgfzeyf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gmtzuuvei.sHtML

[Q83] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gvmpniypm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gjtuoezyf.sHtML

[Q84] 去除首尾空格
来源：http://blog.yfazqb.com/Article/details/gavkidflb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/guvpzuuou.sHtML

[Q85] 数值取整
来源：http://www.share.yfazqb.com/Article/details/ggmbdgkvd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.sjlbkw.cn/Article/details/gprpjxvug.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.vehdjk.com/Article/details/grrviupzs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.vehdjk.com/Article/details/gidhnjghm.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.tarul.cn/Article/details/ggvolfgdb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.epnwcf.com/Article/details/gxmrpgafl.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.epnwcf.com/Article/details/gieswrhcw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.sjlbkw.cn/Article/details/gslshjhdt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gvtcizttx.sHtML

[Q89] 判断表是否存在
来源：http://wap.vehdjk.com/Article/details/gdiunantm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fktsv.cn/Article/details/grfyzqntj.sHtML

[Q90] 生成序号列
来源：http://baike.bbcook.cn/Article/details/gqmtounfs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.bbcook.cn/Article/details/gtmkptroz.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/geyecyvvy.sHtML

R. Bash 专题
来源：http://mobile.yfazqb.com/Article/details/gnmipculs.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvsrspuaq.sHtML

[R01] shebang 与严格模式
来源：http://3g.fktsv.cn/Article/details/gsqtvlrir.sHtML

#!/usr/bin/env bash
来源：http://3g.yfazqb.com/Article/details/gvuzfvncb.sHtML

set -euo pipefail
来源：http://www.blog.vehdjk.com/Article/details/gxzmncbmf.sHtML

[R02] 变量赋值与使用
来源：http://read.share.epnwcf.com/Article/details/giodejeet.sHtML

name="Tom"; echo "$name"
来源：http://baike.epnwcf.com/Article/details/gxvmncngq.sHtML

[R03] 只读变量
来源：http://read.share.fktsv.cn/Article/details/gpyxhiifq.sHtML

readonly PI=3.14
来源：http://www.share.fktsv.cn/Article/details/ghujycgdn.sHtML

[R04] 位置参数
来源：http://read.share.bbcook.cn/Article/details/gkggdkbej.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.bbcook.cn/Article/details/gdknoqeoi.sHtML

[R05] 参数默认值
来源：http://3g.vehdjk.com/Article/details/glgfvhjnh.sHtML

name="${1:-default}"
来源：http://baike.fktsv.cn/Article/details/gqvnpwgez.sHtML

[R06] 判断命令是否存在
来源：http://wap.bbcook.cn/Article/details/gvajxlorg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.yfazqb.com/Article/details/gvwjuqctn.sHtML

[R07] if 判断文件
来源：http://www.blog.vehdjk.com/Article/details/gqnilrjbm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.epnwcf.com/Article/details/gsfuwzcmr.sHtML

[R08] 数值比较
来源：http://www.blog.fktsv.cn/Article/details/gghhvylbw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.bbcook.cn/Article/details/gxgveoplo.sHtML

[R09] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gebafrvsl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/ginyjhirp.sHtML

[R10] 正则匹配
来源：http://mobile.tarul.cn/Article/details/goilxgwew.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gdhzjjqqc.sHtML

[R11] case 多分支
来源：http://read.share.bbcook.cn/Article/details/gndoayepq.sHtML

case "$1" in
来源：http://3g.fktsv.cn/Article/details/gscsorcqk.sHtML

start) echo "启动" ;;
来源：http://wap.fktsv.cn/Article/details/gwczozzng.sHtML

stop)  echo "停止" ;;
来源：http://blog.epnwcf.com/Article/details/gtfyzkglj.sHtML

*)     echo "未知命令" ;;
来源：http://3g.bbcook.cn/Article/details/ghnmklqel.sHtML

esac
来源：http://www.blog.fktsv.cn/Article/details/gybxyppfl.sHtML

[R12] for 遍历文件
来源：http://www.blog.yfazqb.com/Article/details/gwgwxaiqu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.epnwcf.com/Article/details/gjjdqifev.sHtML

[R13] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/ghcxdpqso.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gvmsoxeij.sHtML

[R14] C 风格 for
来源：http://www.blog.bbcook.cn/Article/details/gmfebcmyp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gvzqapsfc.sHtML

[R15] while 逐行读文件
来源：http://blog.vehdjk.com/Article/details/gpwuzxqve.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.tarul.cn/Article/details/gxjxupwkk.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/gzhpysjdl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/grukwuchr.sHtML

[R17] 数组定义与取值
来源：http://m.share.bbcook.cn/Article/details/gmmmgiqol.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fktsv.cn/Article/details/gkojedhde.sHtML

[R18] 遍历数组
来源：http://3g.yfazqb.com/Article/details/gmoedwrcd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.tarul.cn/Article/details/givonwnnf.sHtML

[R19] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gipwuvqxv.sHtML

echo "${#arr[@]}"
来源：http://www.blog.sjlbkw.cn/Article/details/ghxnhsnla.sHtML

[R20] 关联数组（字典）
来源：http://baike.tarul.cn/Article/details/gzrpkuxdw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.bbcook.cn/Article/details/ggffltbag.sHtML

[R21] 字符串长度
来源：http://m.share.tarul.cn/Article/details/gchbrgixj.sHtML

echo "${#s}"
来源：http://m.share.sjlbkw.cn/Article/details/ghjvdzknk.sHtML

[R22] 截取子串
来源：http://m.share.sjlbkw.cn/Article/details/gzpejrtzn.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gvavlmuwg.sHtML

[R23] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/ggelgyzzv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.epnwcf.com/Article/details/gyvcofyqy.sHtML

[R24] 大小写转换
来源：http://baike.fktsv.cn/Article/details/gjjmpivfm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.epnwcf.com/Article/details/ghqqpigye.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.epnwcf.com/Article/details/gdkgptjdm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.sjlbkw.cn/Article/details/gvvvzleyo.sHtML

[R26] 命令替换
来源：http://baike.epnwcf.com/Article/details/gfzdnuhso.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.epnwcf.com/Article/details/gcmzvrxqw.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/gequzezir.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.epnwcf.com/Article/details/gurrociow.sHtML

[R28] 浮点运算
来源：http://www.share.fktsv.cn/Article/details/glszhruzb.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.tarul.cn/Article/details/gzflmfixs.sHtML

[R29] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gyehqdwos.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.tarul.cn/Article/details/gwamgpueu.sHtML

[R30] 函数返回状态码
来源：http://mobile.fktsv.cn/Article/details/gfjvxdjxg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.epnwcf.com/Article/details/gjlpxqvka.sHtML

[R31] 局部变量
来源：http://www.blog.tarul.cn/Article/details/grammgrcj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fktsv.cn/Article/details/gwlgqdiea.sHtML

[R32] 参数个数校验
来源：http://www.share.tarul.cn/Article/details/gikpzealh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/ggeajvypv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.bbcook.cn/Article/details/gwkzmnrqz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.epnwcf.com/Article/details/gneebppud.sHtML

[R34] 退出时清理
来源：http://blog.epnwcf.com/Article/details/gxomgjjbi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gacrnbkrp.sHtML

[R35] 后台执行并等待
来源：http://wap.sjlbkw.cn/Article/details/gbxhkrkmo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.vehdjk.com/Article/details/gcjtnrvhb.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gvrjbhdln.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.bbcook.cn/Article/details/gspgwqkma.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/gkzwnyidm.sHtML

files=$(ls -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gnihudfgd.sHtML

[R38] 管道串联
来源：http://www.m.share.tarul.cn/Article/details/gznhvanja.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.epnwcf.com/Article/details/glyhzxtte.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.sjlbkw.cn/Article/details/gqdakfmwj.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gezdksifa.sHtML

[R40] 追加写日志
来源：http://baike.vehdjk.com/Article/details/gwrzgmppt.sHtML

echo "log" >> out.log
来源：http://blog.sjlbkw.cn/Article/details/gvlhkjrnr.sHtML

[R41] 丢弃输出
来源：http://www.share.vehdjk.com/Article/details/gkztlonfc.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/gwjobamgq.sHtML

[R42] 输入重定向
来源：http://blog.sjlbkw.cn/Article/details/glcdjywug.sHtML

wc -l < a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gufygdnbf.sHtML

[R43] 按名字查找文件
来源：http://blog.epnwcf.com/Article/details/gtaqhoflz.sHtML

find . -name "*.log" -type f
来源：http://wap.vehdjk.com/Article/details/gtakzmfha.sHtML

[R44] 按修改时间查找
来源：http://wap.bbcook.cn/Article/details/gtryyjpkp.sHtML

find . -mtime -7 -type f
来源：http://blog.yfazqb.com/Article/details/gxoiakmal.sHtML

[R45] 批量删除
来源：http://www.share.fktsv.cn/Article/details/gorixhoox.sHtML

find . -name "*.tmp" -delete
来源：http://wap.tarul.cn/Article/details/gxylmvpsq.sHtML

[R46] 递归替换文件内容
来源：http://m.share.epnwcf.com/Article/details/gwrxejffm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.sjlbkw.cn/Article/details/gpjxxftjo.sHtML

[R47] sed 单行替换
来源：http://read.share.tarul.cn/Article/details/gzqprutyc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.bbcook.cn/Article/details/gnouonngf.sHtML

[R48] awk 取指定列
来源：http://www.m.share.epnwcf.com/Article/details/gqvvrdeuo.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fktsv.cn/Article/details/ggsvfjnwd.sHtML

[R49] awk 带条件
来源：http://www.m.share.yfazqb.com/Article/details/gmalgqhkh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.vehdjk.com/Article/details/gurkpqjlf.sHtML

[R50] awk 求和
来源：http://read.share.bbcook.cn/Article/details/ggjskzdge.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gaoqshsed.sHtML

[R51] 排序去重取前几
来源：http://m.share.fktsv.cn/Article/details/grkkjdnfx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/gdfqnvpxn.sHtML

[R52] 统计行数
来源：http://www.blog.epnwcf.com/Article/details/garnmivcw.sHtML

wc -l a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gcnommfha.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.epnwcf.com/Article/details/gfwumaeye.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.epnwcf.com/Article/details/gqmxqaagc.sHtML

[R54] 比较两个文件
来源：http://read.share.epnwcf.com/Article/details/gdltcebhz.sHtML

diff a.txt b.txt
来源：http://blog.vehdjk.com/Article/details/gjqgjyheb.sHtML

[R55] 压缩与解压
来源：http://mobile.fktsv.cn/Article/details/gwazgmgfn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fktsv.cn/Article/details/gjsbmtmpx.sHtML

[R56] 远程拷贝
来源：http://wap.yfazqb.com/Article/details/gheelpkay.sHtML

scp file user@host:/path/
来源：http://m.share.tarul.cn/Article/details/gxhoveozs.sHtML

[R57] 远程执行命令
来源：http://www.blog.vehdjk.com/Article/details/gxkdomkvj.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gdavxgsql.sHtML

[R58] 下载文件
来源：http://blog.yfazqb.com/Article/details/gpkbbfied.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.sjlbkw.cn/Article/details/gptkzkttx.sHtML

[R59] 发 POST JSON
来源：http://wap.bbcook.cn/Article/details/gguzwaehj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.bbcook.cn/Article/details/gwqkijofa.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gospxrlgr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fktsv.cn/Article/details/gyxzfoulj.sHtML

[R61] 磁盘占用
来源：http://wap.sjlbkw.cn/Article/details/gbxrozdda.sHtML

df -h;  du -sh *
来源：http://www.share.sjlbkw.cn/Article/details/gvrlhnutv.sHtML

[R62] 找最占空间的文件
来源：http://blog.bbcook.cn/Article/details/gayckupjm.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.tarul.cn/Article/details/gpmpkunar.sHtML

[R63] 内存与进程
来源：http://www.blog.fktsv.cn/Article/details/gvfsbpgau.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.yfazqb.com/Article/details/gwnvqtdtg.sHtML

[R64] 结束进程
来源：http://blog.tarul.cn/Article/details/gacramnar.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/glwuvaevt.sHtML

[R65] 查看端口占用
来源：http://baike.sjlbkw.cn/Article/details/ghohofsba.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fktsv.cn/Article/details/genrqcyxy.sHtML

[R66] 定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gonmobdet.sHtML

crontab -e;  crontab -l
来源：http://3g.vehdjk.com/Article/details/ghyothugy.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.sjlbkw.cn/Article/details/geeijjkme.sHtML

openssl rand -hex 16
来源：http://www.share.vehdjk.com/Article/details/gaggjozja.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/gaaxaiaxn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/gdxcuvxwk.sHtML

[R69] 生成随机密码
来源：http://m.share.tarul.cn/Article/details/glqumbhlw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.vehdjk.com/Article/details/gexpfvaad.sHtML

[R70] 时间戳与互转
来源：http://mobile.vehdjk.com/Article/details/gnhkfuigg.sHtML

date +%s;  date -d @1700000000
来源：http://3g.yfazqb.com/Article/details/gnoddkxjx.sHtML

[R71] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/gszhmombr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.epnwcf.com/Article/details/ggymmrexc.sHtML

[R72] 等待端口就绪
来源：http://read.share.fktsv.cn/Article/details/ggmtxqtmq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gbntfjewf.sHtML

[R73] 分割大日志
来源：http://www.share.epnwcf.com/Article/details/gwbflsxrn.sHtML

split -l 1000 big.log part_
来源：http://www.blog.tarul.cn/Article/details/gluqwywrx.sHtML

[R74] 批量重命名
来源：http://blog.sjlbkw.cn/Article/details/ghqdwuhff.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.vehdjk.com/Article/details/giaurmsvu.sHtML

[R75] 导出环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/gsdvqzump.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.tarul.cn/Article/details/gqyfqwfgl.sHtML

[R76] 使用临时文件
来源：http://www.share.vehdjk.com/Article/details/geqxgxhbx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/gohvvgfqp.sHtML

[R77] 读取用户输入
来源：http://read.share.tarul.cn/Article/details/grmednuxk.sHtML

read -rp "请输入: " ans
来源：http://blog.yfazqb.com/Article/details/gtbjgzrss.sHtML

[R78] 交互式菜单
来源：http://wap.bbcook.cn/Article/details/gclavaquz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.vehdjk.com/Article/details/gokyxdjhw.sHtML

[R79] 解析命令行选项
来源：http://www.share.epnwcf.com/Article/details/ghylmfbst.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.yfazqb.com/Article/details/gewvokngb.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fktsv.cn/Article/details/gnoczcocz.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/gytmbcklz.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxmyiqrmh.sHtML

S. C / C++ 专题
来源：http://www.blog.epnwcf.com/Article/details/gvhylwcwq.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gixvhexgo.sHtML

[S01] C：Hello World
来源：http://blog.bbcook.cn/Article/details/ghwmjipco.sHtML

#include <stdio.h>
来源：http://baike.bbcook.cn/Article/details/gsxhimnkx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.vehdjk.com/Article/details/glbwtnwqh.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.tarul.cn/Article/details/gafpxqckc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpqmebtc.sHtML

[S03] C：读入整数
来源：http://read.share.sjlbkw.cn/Article/details/gvdcdaxlh.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.epnwcf.com/Article/details/gdgqxqons.sHtML

[S04] C：字符串复制
来源：http://blog.tarul.cn/Article/details/gcxnykdpo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gnlmbthjt.sHtML

[S05] C：字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gwkjxkvjv.sHtML

strlen(s)
来源：http://blog.vehdjk.com/Article/details/gtfgpzhhw.sHtML

[S06] C：字符串比较
来源：http://read.share.bbcook.cn/Article/details/gviiccqdn.sHtML

strcmp(a, b) == 0
来源：http://3g.fktsv.cn/Article/details/gpnepmeqa.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/gzysmjven.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.epnwcf.com/Article/details/ggnxkkdhk.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gxpdfjbso.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fktsv.cn/Article/details/gqrritzyz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fktsv.cn/Article/details/gvuwpkhmk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fktsv.cn/Article/details/gjzpnpfct.sHtML

[S10] C：指针与解引用
来源：http://www.share.epnwcf.com/Article/details/gybqwsqim.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.yfazqb.com/Article/details/guclsfkmi.sHtML

[S11] C：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gstmutpal.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.tarul.cn/Article/details/gckmithlj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.epnwcf.com/Article/details/gsurtffrc.sHtML

fclose(f);
来源：http://m.share.epnwcf.com/Article/details/gyassjdcr.sHtML

[S12] C：写文件
来源：http://mobile.fktsv.cn/Article/details/ghfdwpnmq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gktdxexfx.sHtML

[S13] C：宏定义
来源：http://mobile.tarul.cn/Article/details/gocwhxrca.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fktsv.cn/Article/details/ghejcmopo.sHtML

[S14] C：枚举
来源：http://m.share.fktsv.cn/Article/details/gicrpxrep.sHtML


<!-- 参考信息 -->