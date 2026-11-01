代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.tarul.cn/Article/details/ggvemxybq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.bbcook.cn/Article/details/gindyikoh.sHtML

[Q47] 与平均值比较
来源：http://www.blog.vehdjk.com/Article/details/gtxomsivv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.vehdjk.com/Article/details/gklrmvihv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gbrmrzouf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fktsv.cn/Article/details/gezpctvui.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gwznklxlg.sHtML

[Q49] 更新单行
来源：http://wap.sjlbkw.cn/Article/details/gigpuxhvk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gblpxfgvj.sHtML

[Q50] 批量更新
来源：http://3g.fktsv.cn/Article/details/gbrhhsqxy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.vehdjk.com/Article/details/gxgjyjmua.sHtML

[Q51] 用子查询更新
来源：http://www.blog.yfazqb.com/Article/details/gyncbvvpz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/gjwpjuxtb.sHtML

[Q52] 删除指定行
来源：http://baike.bbcook.cn/Article/details/ghiksmlmb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/grbdjlhsd.sHtML

[Q53] 按条件删除
来源：http://3g.sjlbkw.cn/Article/details/goftxprvd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.epnwcf.com/Article/details/gqucfcuhx.sHtML

[Q54] 清空表
来源：http://blog.fktsv.cn/Article/details/gczoksumy.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.bbcook.cn/Article/details/gzzyuoxrz.sHtML

[Q55] 排名（并列占位）
来源：http://wap.bbcook.cn/Article/details/ghwzmentz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/graownmge.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.yfazqb.com/Article/details/gdbhnuydo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.epnwcf.com/Article/details/gtdioronu.sHtML

[Q57] 行号
来源：http://3g.bbcook.cn/Article/details/gxufyqxbs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fktsv.cn/Article/details/guxhtqlzd.sHtML

[Q58] 累计求和
来源：http://www.share.sjlbkw.cn/Article/details/grzuiqmvn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gocmomtjf.sHtML

[Q59] 分组内累计
来源：http://baike.yfazqb.com/Article/details/gjvtaurin.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gtrfccqmj.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.yfazqb.com/Article/details/giftukzpr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fktsv.cn/Article/details/gkoheocal.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gvvdbgjvm.sHtML

[Q61] 移动平均
来源：http://wap.sjlbkw.cn/Article/details/gqiwwjkph.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.vehdjk.com/Article/details/gkygvqbsn.sHtML

[Q62] 分组占比
来源：http://m.share.bbcook.cn/Article/details/gvdozamnf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/ggmvwzcti.sHtML

[Q63] 开启事务
来源：http://read.share.epnwcf.com/Article/details/gfagoygst.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fktsv.cn/Article/details/gqjidytsm.sHtML

[Q64] 提交事务
来源：http://3g.epnwcf.com/Article/details/gyzlimogr.sHtML

COMMIT;
来源：http://baike.fktsv.cn/Article/details/gnjqdkjtq.sHtML

[Q65] 回滚事务
来源：http://blog.vehdjk.com/Article/details/gqkvrpogl.sHtML

ROLLBACK;
来源：http://baike.tarul.cn/Article/details/gaoqczkgp.sHtML

[Q66] 行锁查询
来源：http://3g.sjlbkw.cn/Article/details/gboqljwyy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.vehdjk.com/Article/details/gnnlegywh.sHtML

[Q67] 设置隔离级别
来源：http://read.share.bbcook.cn/Article/details/gahdiqjbt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.vehdjk.com/Article/details/gbtzeicvk.sHtML

[Q68] 保存点
来源：http://blog.tarul.cn/Article/details/gdqzehwrt.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/galmvpizq.sHtML

ROLLBACK TO sp1;
来源：http://www.share.bbcook.cn/Article/details/grddlflhk.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.tarul.cn/Article/details/gspagvhtb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.epnwcf.com/Article/details/glmvclppi.sHtML

[Q70] 更新统计信息
来源：http://3g.bbcook.cn/Article/details/gaktrpotm.sHtML

ANALYZE TABLE users;
来源：http://baike.tarul.cn/Article/details/gpapewktb.sHtML

[Q71] 查看建表语句
来源：http://www.share.tarul.cn/Article/details/glyhzllbc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.tarul.cn/Article/details/gzhgwmxun.sHtML

[Q72] 查看索引
来源：http://baike.yfazqb.com/Article/details/gjgecixoa.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gvnffstog.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/ghfjorsua.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.vehdjk.com/Article/details/gvtxlaryj.sHtML

[Q74] 强制使用索引
来源：http://www.blog.epnwcf.com/Article/details/gxbezmvgm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.bbcook.cn/Article/details/gwesmbzfy.sHtML

[Q75] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gniyyjkpl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gegvqeamk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.yfazqb.com/Article/details/gtqctohkk.sHtML

[Q76] 按天统计
来源：http://www.m.share.tarul.cn/Article/details/gjxvycqbe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.bbcook.cn/Article/details/gtygpcihf.sHtML

[Q77] 时间加减
来源：http://baike.epnwcf.com/Article/details/ghnoxdrjf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.epnwcf.com/Article/details/gjekrnwzm.sHtML

[Q78] 当前时间
来源：http://3g.bbcook.cn/Article/details/gkbkuufup.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.epnwcf.com/Article/details/gevcplquh.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gxakuhbam.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.tarul.cn/Article/details/gekztoxub.sHtML

[Q80] 字符串截取
来源：http://baike.bbcook.cn/Article/details/gaipajznl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gotsbpbto.sHtML

[Q81] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/ghvnkbvxn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gyyguklys.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.tarul.cn/Article/details/gpuqfczip.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/ggmrtktht.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gadyjlhoa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/glhqirhth.sHtML

[Q84] 去除首尾空格
来源：http://www.share.yfazqb.com/Article/details/gwziptbrp.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gmwcyegqb.sHtML

[Q85] 数值取整
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaxozvsg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.tarul.cn/Article/details/gucuoickh.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fktsv.cn/Article/details/gjgusyznj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.vehdjk.com/Article/details/gmjdnogma.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.sjlbkw.cn/Article/details/gxdbdopxd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.sjlbkw.cn/Article/details/gjzcvwwde.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.yfazqb.com/Article/details/gdceummll.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.sjlbkw.cn/Article/details/ghiryllax.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fktsv.cn/Article/details/gaeugkcmx.sHtML

[Q89] 判断表是否存在
来源：http://m.share.tarul.cn/Article/details/gshwrrimz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fktsv.cn/Article/details/gnlrdxoct.sHtML

[Q90] 生成序号列
来源：http://www.share.sjlbkw.cn/Article/details/goitcunus.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.epnwcf.com/Article/details/guwknxpod.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxlqordkl.sHtML

R. Bash 专题
来源：http://mobile.fktsv.cn/Article/details/gmssvdaja.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/geezsxpse.sHtML

[R01] shebang 与严格模式
来源：http://www.share.epnwcf.com/Article/details/gmkyxofbo.sHtML

#!/usr/bin/env bash
来源：http://m.share.vehdjk.com/Article/details/gpzmkvuqn.sHtML

set -euo pipefail
来源：http://www.blog.yfazqb.com/Article/details/gzmwzqxxw.sHtML

[R02] 变量赋值与使用
来源：http://blog.sjlbkw.cn/Article/details/gfzbfzill.sHtML

name="Tom"; echo "$name"
来源：http://3g.fktsv.cn/Article/details/girxvksrp.sHtML

[R03] 只读变量
来源：http://www.blog.fktsv.cn/Article/details/gymaovckp.sHtML

readonly PI=3.14
来源：http://read.share.sjlbkw.cn/Article/details/gmjgwbrdp.sHtML

[R04] 位置参数
来源：http://read.share.yfazqb.com/Article/details/gkebehefn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.vehdjk.com/Article/details/gyvkejzvo.sHtML

[R05] 参数默认值
来源：http://3g.tarul.cn/Article/details/gmwvdgsca.sHtML

name="${1:-default}"
来源：http://wap.epnwcf.com/Article/details/gfylkpszt.sHtML

[R06] 判断命令是否存在
来源：http://wap.vehdjk.com/Article/details/gwvrjnpcr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/guiglnzcw.sHtML

[R07] if 判断文件
来源：http://www.m.share.fktsv.cn/Article/details/gzvmmkbqd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gquwlhqgu.sHtML

[R08] 数值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gsiwzyvma.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fktsv.cn/Article/details/gultyldkj.sHtML

[R09] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/gcflcqnqh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gzjcoylpi.sHtML

[R10] 正则匹配
来源：http://mobile.sjlbkw.cn/Article/details/gblbibwfp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fktsv.cn/Article/details/goijmrcxy.sHtML

[R11] case 多分支
来源：http://www.blog.tarul.cn/Article/details/gvdteipru.sHtML

case "$1" in
来源：http://mobile.tarul.cn/Article/details/gulqiaknw.sHtML

start) echo "启动" ;;
来源：http://www.m.share.epnwcf.com/Article/details/ggkcqrjrm.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.tarul.cn/Article/details/gnlrkrlfv.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gwmhvbkjb.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/gudlmknnl.sHtML

[R12] for 遍历文件
来源：http://baike.bbcook.cn/Article/details/gacehbaic.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fktsv.cn/Article/details/gpkfhasvp.sHtML

[R13] for 计数循环
来源：http://baike.tarul.cn/Article/details/gyjxtgasu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gawbhewwo.sHtML

[R14] C 风格 for
来源：http://www.m.share.tarul.cn/Article/details/gjuxbvuna.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gmwjmnulw.sHtML

[R15] while 逐行读文件
来源：http://wap.yfazqb.com/Article/details/gzslwiopx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.bbcook.cn/Article/details/gfpspmyoz.sHtML

[R16] until 等待条件
来源：http://mobile.tarul.cn/Article/details/gnzjtcjeq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gkbvpzgtx.sHtML

[R17] 数组定义与取值
来源：http://baike.vehdjk.com/Article/details/gddejuvdr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.bbcook.cn/Article/details/gqdzhpwzu.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/gbilyhabf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.yfazqb.com/Article/details/gfagrpjub.sHtML

[R19] 数组长度
来源：http://wap.yfazqb.com/Article/details/ggcfbukpx.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/gqimtpudg.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/ghvgdrjsf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.epnwcf.com/Article/details/gedilnlui.sHtML

[R21] 字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gjnljqjya.sHtML

echo "${#s}"
来源：http://3g.vehdjk.com/Article/details/gtchnecxm.sHtML

[R22] 截取子串
来源：http://blog.tarul.cn/Article/details/gnvwjcdku.sHtML

echo "${s:0:5}"
来源：http://3g.fktsv.cn/Article/details/glpjopabe.sHtML

[R23] 字符串替换
来源：http://baike.tarul.cn/Article/details/gystrhhmq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fktsv.cn/Article/details/gnnnicczo.sHtML

[R24] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/goddovivz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.epnwcf.com/Article/details/guyzoyvwt.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.bbcook.cn/Article/details/geursqiuc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.vehdjk.com/Article/details/galyisogi.sHtML

[R26] 命令替换
来源：http://wap.vehdjk.com/Article/details/gswgkevlk.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.yfazqb.com/Article/details/glaugqlls.sHtML

[R27] 算术展开
来源：http://blog.epnwcf.com/Article/details/ggbjbrqme.sHtML

echo $((1 + 2 * 3))
来源：http://3g.epnwcf.com/Article/details/grmjlggek.sHtML

[R28] 浮点运算
来源：http://read.share.tarul.cn/Article/details/gefgpjzja.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.bbcook.cn/Article/details/guwnrqlao.sHtML

[R29] 定义函数
来源：http://blog.fktsv.cn/Article/details/gkxxlhlio.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.bbcook.cn/Article/details/gxearwsac.sHtML

[R30] 函数返回状态码
来源：http://blog.fktsv.cn/Article/details/gnjgwgvah.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.sjlbkw.cn/Article/details/gnqrlfoot.sHtML

[R31] 局部变量
来源：http://read.share.vehdjk.com/Article/details/gwwkzmazv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.tarul.cn/Article/details/grfdnhxqp.sHtML

[R32] 参数个数校验
来源：http://www.share.epnwcf.com/Article/details/gonjkgujw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gqgzaswbj.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.tarul.cn/Article/details/gaazoyapx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.vehdjk.com/Article/details/gmveehahs.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/gmcyimyuy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.vehdjk.com/Article/details/gzgseuggv.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fktsv.cn/Article/details/gdsbifila.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.tarul.cn/Article/details/glnzcxnqv.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fktsv.cn/Article/details/gkionvbjk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.bbcook.cn/Article/details/gnrbohziy.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.tarul.cn/Article/details/gdlwkhpml.sHtML

files=$(ls -1)
来源：http://blog.bbcook.cn/Article/details/groytcfpn.sHtML

[R38] 管道串联
来源：http://m.share.tarul.cn/Article/details/gbiyatpom.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.yfazqb.com/Article/details/ghljoorbd.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.sjlbkw.cn/Article/details/gwljofafm.sHtML

cmd > out.log 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/ggdeddtdk.sHtML

[R40] 追加写日志
来源：http://wap.epnwcf.com/Article/details/gswtkydsx.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/geuopuacn.sHtML

[R41] 丢弃输出
来源：http://baike.sjlbkw.cn/Article/details/ghfptlest.sHtML

cmd >/dev/null 2>&1
来源：http://blog.sjlbkw.cn/Article/details/gguthjqbw.sHtML

[R42] 输入重定向
来源：http://www.m.share.bbcook.cn/Article/details/ghygompce.sHtML

wc -l < a.txt
来源：http://mobile.fktsv.cn/Article/details/gvvranuvg.sHtML

[R43] 按名字查找文件
来源：http://blog.yfazqb.com/Article/details/gjjbeoktn.sHtML

find . -name "*.log" -type f
来源：http://www.blog.tarul.cn/Article/details/gczdetcro.sHtML

[R44] 按修改时间查找
来源：http://3g.tarul.cn/Article/details/giqvvfmkj.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/gboffmlko.sHtML

[R45] 批量删除
来源：http://mobile.bbcook.cn/Article/details/gawvrjquh.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fktsv.cn/Article/details/gzwxmawsj.sHtML

[R46] 递归替换文件内容
来源：http://www.share.sjlbkw.cn/Article/details/gpirbjpfj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.bbcook.cn/Article/details/gonfzwvap.sHtML

[R47] sed 单行替换
来源：http://www.m.share.vehdjk.com/Article/details/gtumdvnhr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.epnwcf.com/Article/details/gdfwbamgh.sHtML

[R48] awk 取指定列
来源：http://www.share.yfazqb.com/Article/details/gmrnaylzd.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.bbcook.cn/Article/details/gnnputqgr.sHtML

[R49] awk 带条件
来源：http://www.blog.fktsv.cn/Article/details/gjzpprvlm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/gjpeigiqo.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gibacyhxq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.tarul.cn/Article/details/gdwxmbzwf.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.yfazqb.com/Article/details/gulpsnvir.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.bbcook.cn/Article/details/gisqnlfjq.sHtML

[R52] 统计行数
来源：http://www.share.tarul.cn/Article/details/gxqbgkacb.sHtML

wc -l a.txt
来源：http://www.share.bbcook.cn/Article/details/ghiktzgbr.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.yfazqb.com/Article/details/gjhyndmwx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.sjlbkw.cn/Article/details/gbnjjbcpd.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/gdzicfpqc.sHtML

diff a.txt b.txt
来源：http://baike.tarul.cn/Article/details/gwwdeetky.sHtML

[R55] 压缩与解压
来源：http://www.blog.epnwcf.com/Article/details/grzketmpm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.bbcook.cn/Article/details/gkpanrtrv.sHtML

[R56] 远程拷贝
来源：http://wap.fktsv.cn/Article/details/gnffhztut.sHtML

scp file user@host:/path/
来源：http://3g.epnwcf.com/Article/details/gzahcndzk.sHtML

[R57] 远程执行命令
来源：http://baike.epnwcf.com/Article/details/grioimrxp.sHtML

ssh user@host 'uptime'
来源：http://3g.fktsv.cn/Article/details/ggmdoeojk.sHtML

[R58] 下载文件
来源：http://read.share.sjlbkw.cn/Article/details/gzxqsgqup.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.tarul.cn/Article/details/gqvrjaufa.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/gsysfumhz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.tarul.cn/Article/details/gksuvghyy.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gneolbliq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.vehdjk.com/Article/details/gxpfinxom.sHtML

[R61] 磁盘占用
来源：http://www.m.share.tarul.cn/Article/details/gcqstsjgp.sHtML

df -h;  du -sh *
来源：http://wap.fktsv.cn/Article/details/gdayetfun.sHtML

[R62] 找最占空间的文件
来源：http://mobile.epnwcf.com/Article/details/gjuaaijdq.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.sjlbkw.cn/Article/details/geqviojwf.sHtML

[R63] 内存与进程
来源：http://wap.bbcook.cn/Article/details/gpqrlcatb.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.sjlbkw.cn/Article/details/gbeospkrc.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gjsrocfar.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/gbcxdoxtl.sHtML

[R65] 查看端口占用
来源：http://baike.sjlbkw.cn/Article/details/galjlbtnp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.bbcook.cn/Article/details/gnemrhhep.sHtML

[R66] 定时任务
来源：http://www.share.yfazqb.com/Article/details/grgzngkwg.sHtML

crontab -e;  crontab -l
来源：http://read.share.yfazqb.com/Article/details/gmaipglxt.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.yfazqb.com/Article/details/guibtucaq.sHtML

openssl rand -hex 16
来源：http://3g.tarul.cn/Article/details/gexcwnnul.sHtML

[R68] 计算文件校验值
来源：http://mobile.tarul.cn/Article/details/gbagettoy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.vehdjk.com/Article/details/ghemxnkbs.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/gupyqjajf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.epnwcf.com/Article/details/gljrdnjta.sHtML

[R70] 时间戳与互转
来源：http://wap.bbcook.cn/Article/details/gcrqkehrd.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.vehdjk.com/Article/details/ghkcasukp.sHtML

[R71] 日期格式化
来源：http://mobile.tarul.cn/Article/details/gmrtuidsa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.vehdjk.com/Article/details/gpechddmd.sHtML

[R72] 等待端口就绪
来源：http://3g.tarul.cn/Article/details/gzukcrlpu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gmadwskcx.sHtML

[R73] 分割大日志
来源：http://blog.fktsv.cn/Article/details/giwcvybbb.sHtML

split -l 1000 big.log part_
来源：http://www.blog.bbcook.cn/Article/details/gtnefbxio.sHtML

[R74] 批量重命名
来源：http://read.share.fktsv.cn/Article/details/ggbdcvuuo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.sjlbkw.cn/Article/details/grxhwetey.sHtML

[R75] 导出环境变量
来源：http://www.m.share.epnwcf.com/Article/details/gtbkubalt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.tarul.cn/Article/details/gxdjclshv.sHtML

[R76] 使用临时文件
来源：http://blog.yfazqb.com/Article/details/gswrqycvg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/gcvsdgjlb.sHtML

[R77] 读取用户输入
来源：http://baike.tarul.cn/Article/details/gxdlevqbs.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/gogvtqnxs.sHtML

[R78] 交互式菜单
来源：http://wap.yfazqb.com/Article/details/ghjzmzyuz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.epnwcf.com/Article/details/gwkbwlyxc.sHtML

[R79] 解析命令行选项
来源：http://mobile.bbcook.cn/Article/details/gyibbqysm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.yfazqb.com/Article/details/gxvjokslh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.bbcook.cn/Article/details/ghebbbbuc.sHtML

time ./run.sh
来源：http://www.blog.yfazqb.com/Article/details/gmellfowv.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtsycopge.sHtML

S. C / C++ 专题
来源：http://www.share.tarul.cn/Article/details/gdoupxmtg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gajgoclbh.sHtML

[S01] C：Hello World
来源：http://wap.bbcook.cn/Article/details/giyqiglki.sHtML

#include <stdio.h>
来源：http://www.m.share.fktsv.cn/Article/details/gueruforo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.bbcook.cn/Article/details/gdfcuqtth.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/gnhbulpuo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.yfazqb.com/Article/details/gqsxopmen.sHtML

[S03] C：读入整数
来源：http://blog.vehdjk.com/Article/details/gsrjonelo.sHtML

int x; scanf("%d", &x);
来源：http://read.share.vehdjk.com/Article/details/gcyhbmril.sHtML

[S04] C：字符串复制
来源：http://3g.tarul.cn/Article/details/ggphnqrsx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gvmxpkxzb.sHtML

[S05] C：字符串长度
来源：http://www.share.vehdjk.com/Article/details/gefrirdal.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/grxoukaka.sHtML

[S06] C：字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gdbcfbzac.sHtML

strcmp(a, b) == 0
来源：http://read.share.bbcook.cn/Article/details/gqhpusxji.sHtML

[S07] C：数组遍历求和
来源：http://baike.sjlbkw.cn/Article/details/gonvqcrxr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.epnwcf.com/Article/details/gilbrfycr.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.vehdjk.com/Article/details/gbjukkmor.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fktsv.cn/Article/details/gycvivxvj.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/gffpvuhhn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.epnwcf.com/Article/details/gjegyeopp.sHtML

[S10] C：指针与解引用
来源：http://mobile.sjlbkw.cn/Article/details/gijjscqck.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.tarul.cn/Article/details/gnehfpeum.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gkaynihfb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/gvbkcprlq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fktsv.cn/Article/details/galolgrjc.sHtML

fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gvbcjgwgm.sHtML

[S12] C：写文件
来源：http://www.share.bbcook.cn/Article/details/gjogzthaw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gggoggrba.sHtML

[S13] C：宏定义
来源：http://mobile.vehdjk.com/Article/details/gtctqqbdl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fktsv.cn/Article/details/gfurxpvww.sHtML

[S14] C：枚举
来源：http://read.share.sjlbkw.cn/Article/details/gmihfmuyb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.tarul.cn/Article/details/gvlrzkvij.sHtML

[S15] C：类型转换
来源：http://www.m.share.bbcook.cn/Article/details/gatwpizty.sHtML

(double) a / b
来源：http://www.blog.sjlbkw.cn/Article/details/gfvyhochp.sHtML

[S16] C：位操作置位
来源：http://blog.yfazqb.com/Article/details/gdpekicnv.sHtML


<!-- 参考信息 -->