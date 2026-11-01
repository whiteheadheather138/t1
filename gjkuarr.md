代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.yfazqb.com/Article/details/gfrpdecln.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fktsv.cn/Article/details/gfivjlofi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fktsv.cn/Article/details/gcwjhgovm.sHtML

[Q41] 多表连接
来源：http://blog.bbcook.cn/Article/details/gcniafenj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fktsv.cn/Article/details/gskaftmot.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.tarul.cn/Article/details/gzqevjugq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gaccektay.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.sjlbkw.cn/Article/details/gdlohobei.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.vehdjk.com/Article/details/guhspzmvt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.yfazqb.com/Article/details/gxtpeyfod.sHtML

[Q43] 标量子查询
来源：http://baike.vehdjk.com/Article/details/gbeafdwfv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/gaqlxjbqz.sHtML

[Q44] IN 子查询
来源：http://www.blog.fktsv.cn/Article/details/gwrszvgds.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.sjlbkw.cn/Article/details/gkigoniyj.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/gfbodkoom.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gjssftmlc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.sjlbkw.cn/Article/details/gtjcexkdk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/gqbwjqayc.sHtML

[Q47] 与平均值比较
来源：http://blog.vehdjk.com/Article/details/gjslabbza.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.yfazqb.com/Article/details/giamqboda.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.yfazqb.com/Article/details/gzxpdiobg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.epnwcf.com/Article/details/gbzxkykpl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.vehdjk.com/Article/details/gxiyzbele.sHtML

[Q49] 更新单行
来源：http://www.share.bbcook.cn/Article/details/gaptntfeu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/ggmruohbc.sHtML

[Q50] 批量更新
来源：http://www.m.share.yfazqb.com/Article/details/gzeihblmb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/gjbphthht.sHtML

[Q51] 用子查询更新
来源：http://m.share.sjlbkw.cn/Article/details/gpicryhqt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.tarul.cn/Article/details/gwgupytjj.sHtML

[Q52] 删除指定行
来源：http://wap.vehdjk.com/Article/details/glcjxlywb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gocjchcsv.sHtML

[Q53] 按条件删除
来源：http://3g.yfazqb.com/Article/details/gxjbasmjt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.bbcook.cn/Article/details/gribyltbc.sHtML

[Q54] 清空表
来源：http://www.share.bbcook.cn/Article/details/gcbkrthjw.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fktsv.cn/Article/details/goigcftbz.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.sjlbkw.cn/Article/details/gmphnxhmo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.epnwcf.com/Article/details/gfpquokqt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fktsv.cn/Article/details/grgsqiwgy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fktsv.cn/Article/details/glonabxnh.sHtML

[Q57] 行号
来源：http://blog.yfazqb.com/Article/details/gzrpjligm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.yfazqb.com/Article/details/gvdaizagd.sHtML

[Q58] 累计求和
来源：http://blog.yfazqb.com/Article/details/gcfwtxzbw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.yfazqb.com/Article/details/gjwcngxar.sHtML

[Q59] 分组内累计
来源：http://www.m.share.sjlbkw.cn/Article/details/gssxcavjw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gunpezvfd.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.bbcook.cn/Article/details/guedgnfqh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlfgflcg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gqsfzstvp.sHtML

[Q61] 移动平均
来源：http://baike.fktsv.cn/Article/details/ghcvsxuia.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.bbcook.cn/Article/details/giyatocnc.sHtML

[Q62] 分组占比
来源：http://baike.yfazqb.com/Article/details/gefqsdnrd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gsrbkttkv.sHtML

[Q63] 开启事务
来源：http://www.blog.epnwcf.com/Article/details/gumlyhrsa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.sjlbkw.cn/Article/details/gxksfrabu.sHtML

[Q64] 提交事务
来源：http://www.blog.epnwcf.com/Article/details/gwvnuulty.sHtML

COMMIT;
来源：http://baike.fktsv.cn/Article/details/gvjxcextr.sHtML

[Q65] 回滚事务
来源：http://www.blog.vehdjk.com/Article/details/gafqrmbsn.sHtML

ROLLBACK;
来源：http://m.share.fktsv.cn/Article/details/ggtnggreu.sHtML

[Q66] 行锁查询
来源：http://blog.epnwcf.com/Article/details/ginyjfxir.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.sjlbkw.cn/Article/details/gkrbxaevv.sHtML

[Q67] 设置隔离级别
来源：http://wap.bbcook.cn/Article/details/glbdpbmas.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.yfazqb.com/Article/details/gthflmdbp.sHtML

[Q68] 保存点
来源：http://www.m.share.epnwcf.com/Article/details/golqmxnox.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gfxdydxjj.sHtML

ROLLBACK TO sp1;
来源：http://blog.fktsv.cn/Article/details/ghrhjgdux.sHtML

[Q69] 查看执行计划
来源：http://baike.epnwcf.com/Article/details/gjehncguv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.yfazqb.com/Article/details/glrjnzgof.sHtML

[Q70] 更新统计信息
来源：http://wap.fktsv.cn/Article/details/gwpccbadr.sHtML

ANALYZE TABLE users;
来源：http://mobile.bbcook.cn/Article/details/gxrjbyyzb.sHtML

[Q71] 查看建表语句
来源：http://www.blog.epnwcf.com/Article/details/gwzwngshy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.epnwcf.com/Article/details/gflunnpvh.sHtML

[Q72] 查看索引
来源：http://www.blog.fktsv.cn/Article/details/gedtkigao.sHtML

SHOW INDEX FROM users;
来源：http://baike.tarul.cn/Article/details/gagklmams.sHtML

[Q73] 查看表状态
来源：http://blog.fktsv.cn/Article/details/gpxdsvpmn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.sjlbkw.cn/Article/details/gthrunpjb.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.tarul.cn/Article/details/ggeffmkxv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.yfazqb.com/Article/details/ggdakimiu.sHtML

[Q75] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/ghddhncie.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gewltuoou.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fktsv.cn/Article/details/glwdlsgfi.sHtML

[Q76] 按天统计
来源：http://wap.vehdjk.com/Article/details/gzlsxeiui.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.bbcook.cn/Article/details/gtwlzdkpm.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/gshtnwngb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.epnwcf.com/Article/details/gpkijfxok.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/gugoiofle.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.sjlbkw.cn/Article/details/gntinqltq.sHtML

[Q79] 字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/gypsczfxd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fktsv.cn/Article/details/gsynpwayi.sHtML

[Q80] 字符串截取
来源：http://3g.sjlbkw.cn/Article/details/gjwdyksfk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.vehdjk.com/Article/details/gyotstcog.sHtML

[Q81] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gxptgjeyz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.vehdjk.com/Article/details/gfxwfrngl.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.yfazqb.com/Article/details/gxauskstc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gucnuzxah.sHtML

[Q83] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gbxiapfbk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gtwbuclpw.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fktsv.cn/Article/details/gzqjicxql.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gcbwygfod.sHtML

[Q85] 数值取整
来源：http://www.share.vehdjk.com/Article/details/gsvrvckxb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.bbcook.cn/Article/details/ggjrafnmt.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.vehdjk.com/Article/details/gdmfaotyh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.yfazqb.com/Article/details/gekvgmfig.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fktsv.cn/Article/details/gduvojyuy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.tarul.cn/Article/details/gytcdnlwl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.tarul.cn/Article/details/gkutghomg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.tarul.cn/Article/details/gdzqhczzp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcpzocie.sHtML

[Q89] 判断表是否存在
来源：http://read.share.epnwcf.com/Article/details/gnionapfv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fktsv.cn/Article/details/gvwkyeqjj.sHtML

[Q90] 生成序号列
来源：http://www.blog.sjlbkw.cn/Article/details/gvuifytcb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.sjlbkw.cn/Article/details/glabjqdzt.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtxutdbyi.sHtML

R. Bash 专题
来源：http://www.m.share.bbcook.cn/Article/details/gwlavxret.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/glzocxbix.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fktsv.cn/Article/details/gmdikqxer.sHtML

#!/usr/bin/env bash
来源：http://www.share.epnwcf.com/Article/details/gijlvoekd.sHtML

set -euo pipefail
来源：http://www.m.share.vehdjk.com/Article/details/gsjrnszgp.sHtML

[R02] 变量赋值与使用
来源：http://www.share.tarul.cn/Article/details/gjnsnqxfm.sHtML

name="Tom"; echo "$name"
来源：http://blog.yfazqb.com/Article/details/gshaivkhe.sHtML

[R03] 只读变量
来源：http://baike.vehdjk.com/Article/details/gikqnutso.sHtML

readonly PI=3.14
来源：http://www.m.share.sjlbkw.cn/Article/details/gsauubzdm.sHtML

[R04] 位置参数
来源：http://blog.yfazqb.com/Article/details/gpsymqgsy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.sjlbkw.cn/Article/details/ggwvplhlp.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gryyirwuf.sHtML

name="${1:-default}"
来源：http://www.m.share.epnwcf.com/Article/details/gjrnworby.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fktsv.cn/Article/details/gskmhtkak.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/grmagxcni.sHtML

[R07] if 判断文件
来源：http://wap.sjlbkw.cn/Article/details/glzppmscn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.bbcook.cn/Article/details/gnjlentpu.sHtML

[R08] 数值比较
来源：http://m.share.fktsv.cn/Article/details/guutbwpll.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.epnwcf.com/Article/details/gvobigaof.sHtML

[R09] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/gmfjtylmy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.epnwcf.com/Article/details/gyjxdljof.sHtML

[R10] 正则匹配
来源：http://www.blog.vehdjk.com/Article/details/gnlaqaavg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.bbcook.cn/Article/details/gyffuphvi.sHtML

[R11] case 多分支
来源：http://blog.fktsv.cn/Article/details/grhljwafl.sHtML

case "$1" in
来源：http://www.blog.yfazqb.com/Article/details/gembwwiql.sHtML

start) echo "启动" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gnwxizkvi.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fktsv.cn/Article/details/gmljfpvha.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.yfazqb.com/Article/details/gvebudzbc.sHtML

esac
来源：http://3g.vehdjk.com/Article/details/gkkxzqveq.sHtML

[R12] for 遍历文件
来源：http://read.share.tarul.cn/Article/details/gojtnvgfk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.yfazqb.com/Article/details/guyfenlhy.sHtML

[R13] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gdikyxktn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.bbcook.cn/Article/details/gjcjnkscs.sHtML

[R14] C 风格 for
来源：http://www.share.tarul.cn/Article/details/gtgywvprc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/genqnqely.sHtML

[R15] while 逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gwdgibpkq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.yfazqb.com/Article/details/gxynjhsua.sHtML

[R16] until 等待条件
来源：http://wap.yfazqb.com/Article/details/gbyhdguaa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/gbdipcvac.sHtML

[R17] 数组定义与取值
来源：http://m.share.vehdjk.com/Article/details/getuvuqos.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.sjlbkw.cn/Article/details/griomyqxl.sHtML

[R18] 遍历数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gysupeepo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.tarul.cn/Article/details/gvzgrsumf.sHtML

[R19] 数组长度
来源：http://blog.yfazqb.com/Article/details/geojggqyk.sHtML

echo "${#arr[@]}"
来源：http://m.share.yfazqb.com/Article/details/gpgvxxuwl.sHtML

[R20] 关联数组（字典）
来源：http://www.share.tarul.cn/Article/details/guaszvxuc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.vehdjk.com/Article/details/gmyhkmgse.sHtML

[R21] 字符串长度
来源：http://wap.epnwcf.com/Article/details/gcufchsqt.sHtML

echo "${#s}"
来源：http://blog.bbcook.cn/Article/details/gvqvgolgp.sHtML

[R22] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gtrzqfmtj.sHtML

echo "${s:0:5}"
来源：http://wap.sjlbkw.cn/Article/details/gwrxzikxn.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gvocrkofy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.bbcook.cn/Article/details/gwpoaapnw.sHtML

[R24] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gkgupgrii.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.tarul.cn/Article/details/gvjuidspc.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/gbtfyetyx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/gvirgzbei.sHtML

[R26] 命令替换
来源：http://wap.bbcook.cn/Article/details/gaaogtwig.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.vehdjk.com/Article/details/gctlhbcdf.sHtML

[R27] 算术展开
来源：http://read.share.sjlbkw.cn/Article/details/guqxhspbz.sHtML

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/gumblqtnt.sHtML

[R28] 浮点运算
来源：http://m.share.epnwcf.com/Article/details/gdkyggryg.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.vehdjk.com/Article/details/gxywggycu.sHtML

[R29] 定义函数
来源：http://mobile.fktsv.cn/Article/details/gctbaytyt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.epnwcf.com/Article/details/gcgnfwfsg.sHtML

[R30] 函数返回状态码
来源：http://www.share.yfazqb.com/Article/details/gddoqfvpt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.bbcook.cn/Article/details/gvdoisfwk.sHtML

[R31] 局部变量
来源：http://baike.sjlbkw.cn/Article/details/gfaisxzue.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.tarul.cn/Article/details/gcilodshn.sHtML

[R32] 参数个数校验
来源：http://3g.fktsv.cn/Article/details/gatxaitnb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/glzjpikqh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.sjlbkw.cn/Article/details/gtgxflsva.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.bbcook.cn/Article/details/gmibukbig.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/gehbwgpqx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gcobtjxpw.sHtML

[R35] 后台执行并等待
来源：http://read.share.vehdjk.com/Article/details/gopzwdmvy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.sjlbkw.cn/Article/details/gpxnrdewc.sHtML

[R36] 并发执行多个任务
来源：http://baike.tarul.cn/Article/details/gearjgodc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fktsv.cn/Article/details/gkrjvdlmz.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.vehdjk.com/Article/details/gmusizovg.sHtML

files=$(ls -1)
来源：http://www.m.share.bbcook.cn/Article/details/gozsrsarx.sHtML

[R38] 管道串联
来源：http://www.m.share.fktsv.cn/Article/details/ggmnhoxlp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.vehdjk.com/Article/details/gevjzqwod.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.epnwcf.com/Article/details/gndgrknzr.sHtML

cmd > out.log 2>&1
来源：http://www.share.bbcook.cn/Article/details/gnvzepfez.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gigeapswb.sHtML

echo "log" >> out.log
来源：http://www.blog.tarul.cn/Article/details/gjrasznfm.sHtML

[R41] 丢弃输出
来源：http://read.share.epnwcf.com/Article/details/gyitgyago.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.yfazqb.com/Article/details/gpykrptax.sHtML

[R42] 输入重定向
来源：http://m.share.tarul.cn/Article/details/gcplvzmwm.sHtML

wc -l < a.txt
来源：http://blog.sjlbkw.cn/Article/details/gcbdlohlz.sHtML

[R43] 按名字查找文件
来源：http://3g.bbcook.cn/Article/details/ggihqmrmn.sHtML

find . -name "*.log" -type f
来源：http://www.share.bbcook.cn/Article/details/ggoxdbchq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.vehdjk.com/Article/details/ggtzzhbun.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.bbcook.cn/Article/details/grfgudhsm.sHtML

[R45] 批量删除
来源：http://3g.bbcook.cn/Article/details/gywjchnbm.sHtML

find . -name "*.tmp" -delete
来源：http://wap.bbcook.cn/Article/details/gbtosckim.sHtML

[R46] 递归替换文件内容
来源：http://baike.epnwcf.com/Article/details/gavqwlypt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.yfazqb.com/Article/details/gbfbsbzbq.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fktsv.cn/Article/details/gotvrdbev.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.bbcook.cn/Article/details/gzvtgtctq.sHtML

[R48] awk 取指定列
来源：http://wap.sjlbkw.cn/Article/details/gqmzmekhp.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.tarul.cn/Article/details/griekpvht.sHtML

[R49] awk 带条件
来源：http://m.share.fktsv.cn/Article/details/gxbvqudhu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.sjlbkw.cn/Article/details/grhkrxzmw.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gglprocgp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gpeumracr.sHtML

[R51] 排序去重取前几
来源：http://mobile.fktsv.cn/Article/details/gdrtxuubh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhnoswfl.sHtML

[R52] 统计行数
来源：http://wap.epnwcf.com/Article/details/gqtvyfcww.sHtML

wc -l a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gyqyztipz.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.yfazqb.com/Article/details/getjshryk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.bbcook.cn/Article/details/gejulkwxb.sHtML

[R54] 比较两个文件
来源：http://read.share.yfazqb.com/Article/details/ghpwyoqkz.sHtML

diff a.txt b.txt
来源：http://blog.tarul.cn/Article/details/gpwyyknzn.sHtML

[R55] 压缩与解压
来源：http://www.blog.bbcook.cn/Article/details/gdnjapahz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.sjlbkw.cn/Article/details/gavwyeils.sHtML

[R56] 远程拷贝
来源：http://www.share.vehdjk.com/Article/details/gunohxdix.sHtML

scp file user@host:/path/
来源：http://wap.bbcook.cn/Article/details/gjrwahyor.sHtML

[R57] 远程执行命令
来源：http://wap.sjlbkw.cn/Article/details/gccrgogso.sHtML

ssh user@host 'uptime'
来源：http://m.share.vehdjk.com/Article/details/gdsqffwjs.sHtML

[R58] 下载文件
来源：http://blog.fktsv.cn/Article/details/ghiebzfmp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.yfazqb.com/Article/details/grsgunshd.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/gxqrptbdp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.sjlbkw.cn/Article/details/gaqffgalf.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gxapooruk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.sjlbkw.cn/Article/details/ganzajrhh.sHtML

[R61] 磁盘占用
来源：http://www.share.yfazqb.com/Article/details/gwycvjziv.sHtML

df -h;  du -sh *
来源：http://www.share.yfazqb.com/Article/details/gjonyazre.sHtML

[R62] 找最占空间的文件
来源：http://baike.yfazqb.com/Article/details/goufqdkar.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.vehdjk.com/Article/details/gqwfvduka.sHtML

[R63] 内存与进程
来源：http://www.share.epnwcf.com/Article/details/gyudzzzhr.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/ggqfjfdcf.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gbksafunx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.bbcook.cn/Article/details/gdiseaaxl.sHtML

[R65] 查看端口占用
来源：http://blog.bbcook.cn/Article/details/gyrukclic.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.sjlbkw.cn/Article/details/gpmcrpdkt.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/guuoktxut.sHtML

crontab -e;  crontab -l
来源：http://read.share.yfazqb.com/Article/details/guflsqoaz.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/gqpzpejdu.sHtML

openssl rand -hex 16
来源：http://read.share.sjlbkw.cn/Article/details/gpddhnkhg.sHtML

[R68] 计算文件校验值
来源：http://wap.yfazqb.com/Article/details/gljrsaiky.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.epnwcf.com/Article/details/gbdgunvlt.sHtML

[R69] 生成随机密码
来源：http://blog.fktsv.cn/Article/details/ghtbfnkoq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.tarul.cn/Article/details/ghkvrwfxv.sHtML

[R70] 时间戳与互转
来源：http://blog.vehdjk.com/Article/details/gugaqkijz.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.epnwcf.com/Article/details/gdvtmhspk.sHtML

[R71] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gwfpsrknk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.bbcook.cn/Article/details/ggyttpncy.sHtML

[R72] 等待端口就绪
来源：http://wap.yfazqb.com/Article/details/guzzlpgtg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gvrbfkufd.sHtML

[R73] 分割大日志
来源：http://read.share.fktsv.cn/Article/details/giqeqdwib.sHtML

split -l 1000 big.log part_
来源：http://wap.vehdjk.com/Article/details/gxssnuush.sHtML

[R74] 批量重命名
来源：http://read.share.tarul.cn/Article/details/gfvjncqbm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.tarul.cn/Article/details/gcilgvbev.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/gahtbwilg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.epnwcf.com/Article/details/gvqmkebwd.sHtML

[R76] 使用临时文件
来源：http://www.m.share.vehdjk.com/Article/details/gfgknrnmq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/ggbhlnqgn.sHtML

[R77] 读取用户输入
来源：http://mobile.fktsv.cn/Article/details/ghmvuvgzj.sHtML

read -rp "请输入: " ans
来源：http://wap.sjlbkw.cn/Article/details/gdstpunrv.sHtML

[R78] 交互式菜单
来源：http://read.share.vehdjk.com/Article/details/gaphmmmzw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fktsv.cn/Article/details/gewmljtpm.sHtML

[R79] 解析命令行选项
来源：http://baike.bbcook.cn/Article/details/gchjrdqmb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.epnwcf.com/Article/details/gaprvktve.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.vehdjk.com/Article/details/gshfvakoo.sHtML

time ./run.sh
来源：http://read.share.tarul.cn/Article/details/gnhksnvmx.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gvrmymmpu.sHtML

S. C / C++ 专题
来源：http://read.share.bbcook.cn/Article/details/gxkezixtt.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gofsdvwmi.sHtML

[S01] C：Hello World
来源：http://mobile.tarul.cn/Article/details/gidqrcgrr.sHtML

#include <stdio.h>
来源：http://3g.epnwcf.com/Article/details/gmckmfjor.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.vehdjk.com/Article/details/gvbwdbwtn.sHtML

[S02] C：变量与格式化输出
来源：http://wap.tarul.cn/Article/details/gnspfplug.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.vehdjk.com/Article/details/gpkctwjgr.sHtML

[S03] C：读入整数
来源：http://3g.fktsv.cn/Article/details/gnxsowhhi.sHtML

int x; scanf("%d", &x);
来源：http://read.share.tarul.cn/Article/details/guyebmhwr.sHtML

[S04] C：字符串复制
来源：http://www.blog.fktsv.cn/Article/details/gftawizxk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.epnwcf.com/Article/details/gcohcnsmt.sHtML

[S05] C：字符串长度
来源：http://3g.vehdjk.com/Article/details/gfexzlfsm.sHtML

strlen(s)
来源：http://baike.bbcook.cn/Article/details/ggwxmoikv.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/gqmohdqgy.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/gxkpdvggy.sHtML

[S07] C：数组遍历求和
来源：http://read.share.bbcook.cn/Article/details/gjtnjzioo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/gkxvbxuou.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.yfazqb.com/Article/details/gbhxmixdr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.epnwcf.com/Article/details/ggyzlnlsu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.sjlbkw.cn/Article/details/gaorrubkz.sHtML


<!-- 参考信息 -->