代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.yfazqb.com/Article/details/gygjnnwgg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gchggnmdk.sHtML

[Q47] 与平均值比较
来源：http://www.blog.vehdjk.com/Article/details/gaounxtkd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.yfazqb.com/Article/details/gnsqvkjkq.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.sjlbkw.cn/Article/details/gosszfiej.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/gudkrsnxn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.tarul.cn/Article/details/gdgpkhege.sHtML

[Q49] 更新单行
来源：http://m.share.epnwcf.com/Article/details/gogijlyaw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gaskrjxuy.sHtML

[Q50] 批量更新
来源：http://read.share.tarul.cn/Article/details/gemhnwfff.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.yfazqb.com/Article/details/geujrikat.sHtML

[Q51] 用子查询更新
来源：http://3g.sjlbkw.cn/Article/details/gsxcqhzwz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.bbcook.cn/Article/details/guzgunkjc.sHtML

[Q52] 删除指定行
来源：http://www.blog.bbcook.cn/Article/details/gjpqtolqe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/givedyqyp.sHtML

[Q53] 按条件删除
来源：http://www.share.sjlbkw.cn/Article/details/gsjjlqgbl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.epnwcf.com/Article/details/gjgdftkmz.sHtML

[Q54] 清空表
来源：http://3g.bbcook.cn/Article/details/ghkngbknt.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.tarul.cn/Article/details/giefskkxn.sHtML

[Q55] 排名（并列占位）
来源：http://baike.epnwcf.com/Article/details/gohsicqvd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.tarul.cn/Article/details/gjugygawa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/gvhdedose.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/ggwiydepq.sHtML

[Q57] 行号
来源：http://blog.vehdjk.com/Article/details/gkauoznhr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.yfazqb.com/Article/details/gewromgaj.sHtML

[Q58] 累计求和
来源：http://m.share.sjlbkw.cn/Article/details/gqwafmirp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gbsfixpon.sHtML

[Q59] 分组内累计
来源：http://mobile.sjlbkw.cn/Article/details/gkrkeamxk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gduvwicmn.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fktsv.cn/Article/details/gsqynvpwe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fktsv.cn/Article/details/gxbeltdsd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/ghraequwu.sHtML

[Q61] 移动平均
来源：http://www.share.fktsv.cn/Article/details/goambouct.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/ghfjhedzl.sHtML

[Q62] 分组占比
来源：http://www.m.share.epnwcf.com/Article/details/gtqqduifa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gsejxezbn.sHtML

[Q63] 开启事务
来源：http://m.share.vehdjk.com/Article/details/gdmspwnrd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.epnwcf.com/Article/details/gjookqdgr.sHtML

[Q64] 提交事务
来源：http://www.blog.epnwcf.com/Article/details/gsifxauhb.sHtML

COMMIT;
来源：http://www.share.tarul.cn/Article/details/gpckvrnuz.sHtML

[Q65] 回滚事务
来源：http://www.m.share.vehdjk.com/Article/details/genxvazvc.sHtML

ROLLBACK;
来源：http://m.share.sjlbkw.cn/Article/details/gmovlxelp.sHtML

[Q66] 行锁查询
来源：http://read.share.fktsv.cn/Article/details/gaeufhbzd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.yfazqb.com/Article/details/gthuaihcr.sHtML

[Q67] 设置隔离级别
来源：http://3g.bbcook.cn/Article/details/gyvdyhedc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.epnwcf.com/Article/details/gzrzqcypf.sHtML

[Q68] 保存点
来源：http://www.blog.tarul.cn/Article/details/gmazghbfx.sHtML

SAVEPOINT sp1;
来源：http://m.share.vehdjk.com/Article/details/gsmycedkx.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fktsv.cn/Article/details/gdqgkzsmu.sHtML

[Q69] 查看执行计划
来源：http://mobile.epnwcf.com/Article/details/gnuexcbli.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.bbcook.cn/Article/details/gghslxsqx.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.yfazqb.com/Article/details/gbhjszuvq.sHtML

ANALYZE TABLE users;
来源：http://wap.vehdjk.com/Article/details/glourrdsk.sHtML

[Q71] 查看建表语句
来源：http://www.blog.bbcook.cn/Article/details/giekrqbwl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.yfazqb.com/Article/details/gciwtyfiv.sHtML

[Q72] 查看索引
来源：http://blog.fktsv.cn/Article/details/gubzqdrzl.sHtML

SHOW INDEX FROM users;
来源：http://baike.tarul.cn/Article/details/gqjxxjpzq.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/gsbvjdcln.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fktsv.cn/Article/details/griucctib.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/gkdcazjet.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.bbcook.cn/Article/details/gnqtdlrbc.sHtML

[Q75] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gqtfihpju.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gsjmyejxa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fktsv.cn/Article/details/gughueoyo.sHtML

[Q76] 按天统计
来源：http://www.blog.yfazqb.com/Article/details/gyvyaxeac.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fktsv.cn/Article/details/gmutyzupm.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/gdnphklys.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/gcctaekqn.sHtML

[Q78] 当前时间
来源：http://www.blog.fktsv.cn/Article/details/gpjkvbfiy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.vehdjk.com/Article/details/gjzqjpwsw.sHtML

[Q79] 字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gayjepypw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.yfazqb.com/Article/details/gebpaqprh.sHtML

[Q80] 字符串截取
来源：http://www.blog.fktsv.cn/Article/details/ggbrnaxha.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.tarul.cn/Article/details/gfwcshixu.sHtML

[Q81] 字符串替换
来源：http://www.m.share.vehdjk.com/Article/details/gntnzunwf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.bbcook.cn/Article/details/gghcyphju.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.bbcook.cn/Article/details/grreymybt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gkqvaqcln.sHtML

[Q83] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gjnfpbpjj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gojpglndy.sHtML

[Q84] 去除首尾空格
来源：http://wap.fktsv.cn/Article/details/gheeqxgok.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gyzhbnfdf.sHtML

[Q85] 数值取整
来源：http://wap.sjlbkw.cn/Article/details/gmoaxjrgu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.vehdjk.com/Article/details/gfnpixhqg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.yfazqb.com/Article/details/gplaihuzc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.sjlbkw.cn/Article/details/gpuquahfd.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.tarul.cn/Article/details/ghbrhmjpv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.sjlbkw.cn/Article/details/gptaqhwmb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/gxndqehhd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fktsv.cn/Article/details/grrjlyqvq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.vehdjk.com/Article/details/gqopkelfu.sHtML

[Q89] 判断表是否存在
来源：http://3g.bbcook.cn/Article/details/gxtrfnaep.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.vehdjk.com/Article/details/ggrmnezup.sHtML

[Q90] 生成序号列
来源：http://baike.vehdjk.com/Article/details/gidhkdvli.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.tarul.cn/Article/details/gwikrkbbd.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghlmxhlxt.sHtML

R. Bash 专题
来源：http://3g.bbcook.cn/Article/details/gcrvdbgty.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gnwavqjos.sHtML

[R01] shebang 与严格模式
来源：http://www.share.vehdjk.com/Article/details/gykzwkzfp.sHtML

#!/usr/bin/env bash
来源：http://blog.bbcook.cn/Article/details/gxbbipcnd.sHtML

set -euo pipefail
来源：http://mobile.fktsv.cn/Article/details/gsvgaesoi.sHtML

[R02] 变量赋值与使用
来源：http://mobile.sjlbkw.cn/Article/details/gfxqjoloh.sHtML

name="Tom"; echo "$name"
来源：http://mobile.epnwcf.com/Article/details/gllkuwlwk.sHtML

[R03] 只读变量
来源：http://3g.sjlbkw.cn/Article/details/gelzpfiuf.sHtML

readonly PI=3.14
来源：http://blog.sjlbkw.cn/Article/details/gljfssiqn.sHtML

[R04] 位置参数
来源：http://m.share.sjlbkw.cn/Article/details/gkhkfzkzh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.bbcook.cn/Article/details/gutptovkx.sHtML

[R05] 参数默认值
来源：http://www.blog.vehdjk.com/Article/details/gwlncsvms.sHtML

name="${1:-default}"
来源：http://www.share.bbcook.cn/Article/details/gmfxlyewx.sHtML

[R06] 判断命令是否存在
来源：http://m.share.vehdjk.com/Article/details/gbenchhbr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gxdiexxeg.sHtML

[R07] if 判断文件
来源：http://mobile.vehdjk.com/Article/details/gtxcqkagk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fktsv.cn/Article/details/gazmxvdif.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/ganyzvvpt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.epnwcf.com/Article/details/glmbmfkrc.sHtML

[R09] 字符串比较
来源：http://blog.epnwcf.com/Article/details/gbvlelstw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fktsv.cn/Article/details/gwfgxdcgq.sHtML

[R10] 正则匹配
来源：http://www.m.share.epnwcf.com/Article/details/gzpqrmjgm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fktsv.cn/Article/details/gswzyeajv.sHtML

[R11] case 多分支
来源：http://read.share.fktsv.cn/Article/details/gymhmpxhi.sHtML

case "$1" in
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmpempaz.sHtML

start) echo "启动" ;;
来源：http://read.share.fktsv.cn/Article/details/gvxesbftx.sHtML

stop)  echo "停止" ;;
来源：http://wap.sjlbkw.cn/Article/details/gvqrgitia.sHtML

*)     echo "未知命令" ;;
来源：http://3g.sjlbkw.cn/Article/details/ghdxlbdtm.sHtML

esac
来源：http://blog.epnwcf.com/Article/details/gfwarwcsv.sHtML

[R12] for 遍历文件
来源：http://m.share.sjlbkw.cn/Article/details/gnmianpbx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.tarul.cn/Article/details/gyvqmohly.sHtML

[R13] for 计数循环
来源：http://wap.vehdjk.com/Article/details/ggzlxwuzo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.yfazqb.com/Article/details/gqdsnatmu.sHtML

[R14] C 风格 for
来源：http://blog.bbcook.cn/Article/details/gajhvhzmy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gklypcixz.sHtML

[R15] while 逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gjbakrzsd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.epnwcf.com/Article/details/gyavfauos.sHtML

[R16] until 等待条件
来源：http://www.share.bbcook.cn/Article/details/gylgrudgy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfjgxluq.sHtML

[R17] 数组定义与取值
来源：http://m.share.epnwcf.com/Article/details/gyipaskzc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.sjlbkw.cn/Article/details/gkrniormf.sHtML

[R18] 遍历数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gxeswjklg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/goryabbor.sHtML

[R19] 数组长度
来源：http://3g.epnwcf.com/Article/details/gsggtpfmd.sHtML

echo "${#arr[@]}"
来源：http://wap.bbcook.cn/Article/details/gmpuzimij.sHtML

[R20] 关联数组（字典）
来源：http://baike.bbcook.cn/Article/details/gxlixjtxj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.bbcook.cn/Article/details/gwzmuukji.sHtML

[R21] 字符串长度
来源：http://3g.bbcook.cn/Article/details/gwhxwjuec.sHtML

echo "${#s}"
来源：http://baike.epnwcf.com/Article/details/gqbfzyffq.sHtML

[R22] 截取子串
来源：http://blog.epnwcf.com/Article/details/gweqqtogo.sHtML

echo "${s:0:5}"
来源：http://read.share.epnwcf.com/Article/details/gunvhhnrb.sHtML

[R23] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/gyyseuvmz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fktsv.cn/Article/details/gqjyfexdt.sHtML

[R24] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/ghbsqbixr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.sjlbkw.cn/Article/details/ghfykyvdq.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.vehdjk.com/Article/details/gobdwjkxu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fktsv.cn/Article/details/gfrbafakc.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/gclnmiajm.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.yfazqb.com/Article/details/gzdpvsere.sHtML

[R27] 算术展开
来源：http://www.share.tarul.cn/Article/details/gycokumug.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/ggvrmteao.sHtML

[R28] 浮点运算
来源：http://3g.vehdjk.com/Article/details/ghmvhjozo.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.epnwcf.com/Article/details/guuwkuluh.sHtML

[R29] 定义函数
来源：http://mobile.epnwcf.com/Article/details/glrtmqewx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.vehdjk.com/Article/details/glppusgts.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.tarul.cn/Article/details/gsmxbrtia.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.yfazqb.com/Article/details/ghwkzdqzo.sHtML

[R31] 局部变量
来源：http://blog.epnwcf.com/Article/details/gqcmxnxus.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.vehdjk.com/Article/details/gmbvrrxvp.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fktsv.cn/Article/details/glrfpduax.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gihvgctup.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.epnwcf.com/Article/details/glvrvydmj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fktsv.cn/Article/details/gxdifggfx.sHtML

[R34] 退出时清理
来源：http://m.share.tarul.cn/Article/details/gyryesaka.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gowiocyjn.sHtML

[R35] 后台执行并等待
来源：http://blog.vehdjk.com/Article/details/gywvpaxys.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.tarul.cn/Article/details/gikjvlviw.sHtML

[R36] 并发执行多个任务
来源：http://baike.sjlbkw.cn/Article/details/gmxfucjcy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.vehdjk.com/Article/details/ggxcqxjfi.sHtML

[R37] 把输出赋给变量
来源：http://mobile.tarul.cn/Article/details/gfscgrcot.sHtML

files=$(ls -1)
来源：http://www.m.share.tarul.cn/Article/details/grehllyjk.sHtML

[R38] 管道串联
来源：http://m.share.fktsv.cn/Article/details/gzevtyswp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.epnwcf.com/Article/details/gyudvqooh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fktsv.cn/Article/details/gtxtsinzs.sHtML

cmd > out.log 2>&1
来源：http://3g.bbcook.cn/Article/details/gwwyignff.sHtML

[R40] 追加写日志
来源：http://m.share.epnwcf.com/Article/details/gwwhjsjcp.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/gqkeaqfyc.sHtML

[R41] 丢弃输出
来源：http://wap.sjlbkw.cn/Article/details/ghqxdrucr.sHtML

cmd >/dev/null 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gxskmoudi.sHtML

[R42] 输入重定向
来源：http://wap.epnwcf.com/Article/details/gjsbmuemp.sHtML

wc -l < a.txt
来源：http://blog.epnwcf.com/Article/details/gbgrhxewd.sHtML

[R43] 按名字查找文件
来源：http://3g.tarul.cn/Article/details/ggkvkwkov.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gsxiqkvey.sHtML

[R44] 按修改时间查找
来源：http://3g.tarul.cn/Article/details/ggeglfprm.sHtML

find . -mtime -7 -type f
来源：http://baike.fktsv.cn/Article/details/gepyxvvyd.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxfwtkfa.sHtML

find . -name "*.tmp" -delete
来源：http://wap.yfazqb.com/Article/details/gwemstbbl.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.epnwcf.com/Article/details/gfmhjsnps.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.bbcook.cn/Article/details/gpmxllzgg.sHtML

[R47] sed 单行替换
来源：http://3g.bbcook.cn/Article/details/gnlirwkua.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gnobfglbu.sHtML

[R48] awk 取指定列
来源：http://read.share.fktsv.cn/Article/details/gpasinsub.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.vehdjk.com/Article/details/grnglsmre.sHtML

[R49] awk 带条件
来源：http://www.share.fktsv.cn/Article/details/gugnqrtvm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.bbcook.cn/Article/details/gqhyiybqc.sHtML

[R50] awk 求和
来源：http://wap.tarul.cn/Article/details/gruxadiao.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.tarul.cn/Article/details/guaweuxvy.sHtML

[R51] 排序去重取前几
来源：http://mobile.bbcook.cn/Article/details/gkvceoeea.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fktsv.cn/Article/details/gzyjyhjmr.sHtML

[R52] 统计行数
来源：http://3g.yfazqb.com/Article/details/gvjqnmndi.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gwledcsmv.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.tarul.cn/Article/details/gmraqxpia.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.sjlbkw.cn/Article/details/gioveaeow.sHtML

[R54] 比较两个文件
来源：http://wap.tarul.cn/Article/details/gktzadjko.sHtML

diff a.txt b.txt
来源：http://www.share.fktsv.cn/Article/details/gxevyaglt.sHtML

[R55] 压缩与解压
来源：http://read.share.fktsv.cn/Article/details/ghlryyksd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/gfwzawnhb.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/gehkhfgzi.sHtML

scp file user@host:/path/
来源：http://3g.yfazqb.com/Article/details/gtqlgdmyb.sHtML

[R57] 远程执行命令
来源：http://m.share.fktsv.cn/Article/details/gpubphixp.sHtML

ssh user@host 'uptime'
来源：http://www.blog.epnwcf.com/Article/details/gnikvyhxr.sHtML

[R58] 下载文件
来源：http://read.share.bbcook.cn/Article/details/gdjvuypvb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.bbcook.cn/Article/details/gjkuikaem.sHtML

[R59] 发 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gucvublwk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.vehdjk.com/Article/details/gczzgarqi.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/glxqjlzea.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.sjlbkw.cn/Article/details/gujxutjmf.sHtML

[R61] 磁盘占用
来源：http://3g.vehdjk.com/Article/details/gtgriqyei.sHtML

df -h;  du -sh *
来源：http://read.share.vehdjk.com/Article/details/grmesagjb.sHtML

[R62] 找最占空间的文件
来源：http://www.share.epnwcf.com/Article/details/gadnqptvj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.sjlbkw.cn/Article/details/gtgmueupn.sHtML

[R63] 内存与进程
来源：http://www.blog.bbcook.cn/Article/details/gpdegdxsk.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.tarul.cn/Article/details/goxwxqzvt.sHtML

[R64] 结束进程
来源：http://www.share.yfazqb.com/Article/details/gvssoexda.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.epnwcf.com/Article/details/gnrdhxusz.sHtML

[R65] 查看端口占用
来源：http://3g.vehdjk.com/Article/details/gpfhdteaa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.tarul.cn/Article/details/gbypeketw.sHtML

[R66] 定时任务
来源：http://mobile.yfazqb.com/Article/details/gtphdqhko.sHtML

crontab -e;  crontab -l
来源：http://www.blog.epnwcf.com/Article/details/gxfbfxaie.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.vehdjk.com/Article/details/gnpvfijcm.sHtML

openssl rand -hex 16
来源：http://blog.epnwcf.com/Article/details/gmegbatrk.sHtML

[R68] 计算文件校验值
来源：http://www.blog.vehdjk.com/Article/details/grpvfdlok.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.yfazqb.com/Article/details/glaauqoef.sHtML

[R69] 生成随机密码
来源：http://wap.tarul.cn/Article/details/gebpcdfnf.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.tarul.cn/Article/details/galyquejo.sHtML

[R70] 时间戳与互转
来源：http://www.blog.sjlbkw.cn/Article/details/gcdtjbzdi.sHtML

date +%s;  date -d @1700000000
来源：http://blog.tarul.cn/Article/details/gbtbzbkag.sHtML

[R71] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/gxjfwusgd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.bbcook.cn/Article/details/gujfmzvzb.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fktsv.cn/Article/details/gtnvokhiw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gqxyzjise.sHtML

[R73] 分割大日志
来源：http://read.share.sjlbkw.cn/Article/details/gidjsrqti.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fktsv.cn/Article/details/ghpwwnxis.sHtML

[R74] 批量重命名
来源：http://m.share.bbcook.cn/Article/details/gejihebye.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.tarul.cn/Article/details/gvzddqhry.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gkktaxniz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.yfazqb.com/Article/details/gnpvzhtcl.sHtML

[R76] 使用临时文件
来源：http://3g.bbcook.cn/Article/details/gzsewnamn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gikfhlrlb.sHtML

[R77] 读取用户输入
来源：http://www.share.sjlbkw.cn/Article/details/gmtcderwt.sHtML

read -rp "请输入: " ans
来源：http://blog.bbcook.cn/Article/details/gaeukmpyl.sHtML

[R78] 交互式菜单
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrqaxkpq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.vehdjk.com/Article/details/gkglnsgkt.sHtML

[R79] 解析命令行选项
来源：http://mobile.yfazqb.com/Article/details/gkgsrqlfh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.yfazqb.com/Article/details/ggvtbadqr.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.bbcook.cn/Article/details/gvbtnovab.sHtML

time ./run.sh
来源：http://mobile.fktsv.cn/Article/details/gzmcqqumj.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gpovvcqjn.sHtML

S. C / C++ 专题
来源：http://blog.sjlbkw.cn/Article/details/gmlpfjmjx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtgjwffxx.sHtML

[S01] C：Hello World
来源：http://wap.bbcook.cn/Article/details/geughhcza.sHtML

#include <stdio.h>
来源：http://read.share.sjlbkw.cn/Article/details/gfsgeijxo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.bbcook.cn/Article/details/gxsbxwuhf.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.yfazqb.com/Article/details/grclvapsa.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/grslvtvuc.sHtML

[S03] C：读入整数
来源：http://baike.vehdjk.com/Article/details/gzucdcdeu.sHtML

int x; scanf("%d", &x);
来源：http://baike.bbcook.cn/Article/details/gtlzpermh.sHtML

[S04] C：字符串复制
来源：http://mobile.tarul.cn/Article/details/gmsmxzwpz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.sjlbkw.cn/Article/details/gkcxqcfiu.sHtML

[S05] C：字符串长度
来源：http://wap.vehdjk.com/Article/details/gazkvdern.sHtML

strlen(s)
来源：http://blog.vehdjk.com/Article/details/ghvfovvka.sHtML

[S06] C：字符串比较
来源：http://wap.epnwcf.com/Article/details/gofmmbxzh.sHtML

strcmp(a, b) == 0
来源：http://www.share.fktsv.cn/Article/details/geojydawk.sHtML

[S07] C：数组遍历求和
来源：http://3g.tarul.cn/Article/details/gltqcyany.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.vehdjk.com/Article/details/gygkttzej.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.bbcook.cn/Article/details/greylfust.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.tarul.cn/Article/details/gsoflfpyn.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fktsv.cn/Article/details/gjuqklpjt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.bbcook.cn/Article/details/gshsgmsvb.sHtML

[S10] C：指针与解引用
来源：http://wap.epnwcf.com/Article/details/gxlrwdwqy.sHtML

int *p = &a;  *p = 5;
来源：http://3g.epnwcf.com/Article/details/grkybqqos.sHtML

[S11] C：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gdqcibuue.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.epnwcf.com/Article/details/grdwirebs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.tarul.cn/Article/details/gcwiurbjp.sHtML

fclose(f);
来源：http://wap.vehdjk.com/Article/details/gtlldksgn.sHtML

[S12] C：写文件
来源：http://3g.vehdjk.com/Article/details/gkudbibud.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.epnwcf.com/Article/details/gezuhwxjz.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/gjzddlgtf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.bbcook.cn/Article/details/gtabmrisn.sHtML

[S14] C：枚举
来源：http://wap.epnwcf.com/Article/details/gnnyvwxff.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.vehdjk.com/Article/details/goswqlxsj.sHtML

[S15] C：类型转换
来源：http://wap.vehdjk.com/Article/details/ghewzkqwn.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/glhrbyxcj.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/gaswlstcx.sHtML


<!-- 参考信息 -->