代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.yfazqb.com/Article/details/gguwsxycr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gpfetzytu.sHtML

[Q47] 与平均值比较
来源：http://3g.fktsv.cn/Article/details/gdswdallc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fktsv.cn/Article/details/gxavborlk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.vehdjk.com/Article/details/gsunxjidi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.yfazqb.com/Article/details/gxbhspvpe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.vehdjk.com/Article/details/gnrbkotdl.sHtML

[Q49] 更新单行
来源：http://www.m.share.sjlbkw.cn/Article/details/gheyufoky.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gioubllva.sHtML

[Q50] 批量更新
来源：http://mobile.fktsv.cn/Article/details/gihwtbfxq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.epnwcf.com/Article/details/gaooesmlp.sHtML

[Q51] 用子查询更新
来源：http://wap.sjlbkw.cn/Article/details/gxnbnijki.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.vehdjk.com/Article/details/gukgbegaj.sHtML

[Q52] 删除指定行
来源：http://www.share.vehdjk.com/Article/details/gzyvujlbb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gkmqhpvbz.sHtML

[Q53] 按条件删除
来源：http://m.share.bbcook.cn/Article/details/gjessqkks.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.tarul.cn/Article/details/gtosugcyu.sHtML

[Q54] 清空表
来源：http://www.share.vehdjk.com/Article/details/ghtsizgyj.sHtML

TRUNCATE TABLE logs;
来源：http://3g.tarul.cn/Article/details/gskuwxqmu.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/gabylrayt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.bbcook.cn/Article/details/gbfolaaba.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.tarul.cn/Article/details/gqcikozub.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/gbanyaqyv.sHtML

[Q57] 行号
来源：http://read.share.tarul.cn/Article/details/guonexoog.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gjoyclkhv.sHtML

[Q58] 累计求和
来源：http://blog.sjlbkw.cn/Article/details/ghinvlryb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.vehdjk.com/Article/details/gkjpqlyju.sHtML

[Q59] 分组内累计
来源：http://3g.sjlbkw.cn/Article/details/gbftifocs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gduylvowo.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.bbcook.cn/Article/details/gvikefkrz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.yfazqb.com/Article/details/gvrwtnilc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gjfbtqevt.sHtML

[Q61] 移动平均
来源：http://read.share.vehdjk.com/Article/details/gvwsztsyb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gvpzvgkax.sHtML

[Q62] 分组占比
来源：http://mobile.tarul.cn/Article/details/giuxtdvuw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gdummgtoz.sHtML

[Q63] 开启事务
来源：http://baike.yfazqb.com/Article/details/gvxfwjxyo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.tarul.cn/Article/details/gwlmfywqz.sHtML

[Q64] 提交事务
来源：http://read.share.epnwcf.com/Article/details/gueccqgyg.sHtML

COMMIT;
来源：http://www.share.vehdjk.com/Article/details/gqxsrhbxh.sHtML

[Q65] 回滚事务
来源：http://m.share.bbcook.cn/Article/details/gfijmmzxs.sHtML

ROLLBACK;
来源：http://blog.fktsv.cn/Article/details/gqylnzvfj.sHtML

[Q66] 行锁查询
来源：http://mobile.sjlbkw.cn/Article/details/gmaoqjkjp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.bbcook.cn/Article/details/gxbseswor.sHtML

[Q67] 设置隔离级别
来源：http://m.share.tarul.cn/Article/details/grwiviluq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.bbcook.cn/Article/details/gmgnpblre.sHtML

[Q68] 保存点
来源：http://www.share.fktsv.cn/Article/details/gmlmoiokt.sHtML

SAVEPOINT sp1;
来源：http://wap.vehdjk.com/Article/details/gtvllabte.sHtML

ROLLBACK TO sp1;
来源：http://blog.vehdjk.com/Article/details/gtrymtlho.sHtML

[Q69] 查看执行计划
来源：http://www.share.sjlbkw.cn/Article/details/gzvcruhzo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.sjlbkw.cn/Article/details/gkgdjspvq.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.epnwcf.com/Article/details/gcfsljzcq.sHtML

ANALYZE TABLE users;
来源：http://3g.epnwcf.com/Article/details/gllgooptb.sHtML

[Q71] 查看建表语句
来源：http://3g.yfazqb.com/Article/details/gjgizvgeh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.epnwcf.com/Article/details/gmjiyxnxc.sHtML

[Q72] 查看索引
来源：http://wap.fktsv.cn/Article/details/gkkgblgwt.sHtML

SHOW INDEX FROM users;
来源：http://baike.vehdjk.com/Article/details/gjdluwndn.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/gaihnubzl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.tarul.cn/Article/details/gdogojltp.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fktsv.cn/Article/details/glrozuthi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.bbcook.cn/Article/details/ggabloxqn.sHtML

[Q75] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gzjtqdpkw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/geqrpskmg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.bbcook.cn/Article/details/guuqwljaw.sHtML

[Q76] 按天统计
来源：http://3g.vehdjk.com/Article/details/ghlqslojw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.vehdjk.com/Article/details/gpnuasaqf.sHtML

[Q77] 时间加减
来源：http://read.share.epnwcf.com/Article/details/gspdzpfrb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.epnwcf.com/Article/details/gokenfofy.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/gnhxujhxh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.vehdjk.com/Article/details/ggpisyldw.sHtML

[Q79] 字符串拼接
来源：http://baike.bbcook.cn/Article/details/glkdscifg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.bbcook.cn/Article/details/gvhnvktjj.sHtML

[Q80] 字符串截取
来源：http://m.share.yfazqb.com/Article/details/goybawfzr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gnasjsvea.sHtML

[Q81] 字符串替换
来源：http://wap.bbcook.cn/Article/details/gwzpbnaav.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gngrjggtf.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.vehdjk.com/Article/details/gxekflrsx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gpznxkted.sHtML

[Q83] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gexaynvup.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gxddjpkag.sHtML

[Q84] 去除首尾空格
来源：http://baike.sjlbkw.cn/Article/details/gxkctqvnh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/guetsglxb.sHtML

[Q85] 数值取整
来源：http://www.blog.fktsv.cn/Article/details/geopswibf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrijikee.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.vehdjk.com/Article/details/gkewmamhl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.bbcook.cn/Article/details/gascoinuv.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.sjlbkw.cn/Article/details/giweptaix.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.vehdjk.com/Article/details/gikxfpvmm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/ghtxutacr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fktsv.cn/Article/details/gekjbeqkq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gnsbsfykm.sHtML

[Q89] 判断表是否存在
来源：http://www.share.yfazqb.com/Article/details/gojewkauo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/geqbpqxdj.sHtML

[Q90] 生成序号列
来源：http://baike.vehdjk.com/Article/details/gsutvusfc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.yfazqb.com/Article/details/gmsuzuntp.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvuauxuiu.sHtML

R. Bash 专题
来源：http://mobile.epnwcf.com/Article/details/gqkdtkldg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gnoqijvvh.sHtML

[R01] shebang 与严格模式
来源：http://3g.bbcook.cn/Article/details/gxdeplefp.sHtML

#!/usr/bin/env bash
来源：http://m.share.tarul.cn/Article/details/gfczwptpt.sHtML

set -euo pipefail
来源：http://wap.bbcook.cn/Article/details/gicwsglgf.sHtML

[R02] 变量赋值与使用
来源：http://m.share.yfazqb.com/Article/details/gtcrcavvq.sHtML

name="Tom"; echo "$name"
来源：http://blog.fktsv.cn/Article/details/ghlpwlnbl.sHtML

[R03] 只读变量
来源：http://www.share.sjlbkw.cn/Article/details/gkpmmconm.sHtML

readonly PI=3.14
来源：http://mobile.epnwcf.com/Article/details/gxxonnltf.sHtML

[R04] 位置参数
来源：http://www.blog.vehdjk.com/Article/details/gewdectdn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.yfazqb.com/Article/details/guparczua.sHtML

[R05] 参数默认值
来源：http://mobile.tarul.cn/Article/details/gnaoxepub.sHtML

name="${1:-default}"
来源：http://3g.vehdjk.com/Article/details/gyfimjhpx.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.tarul.cn/Article/details/gxsieivrp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyvhpceu.sHtML

[R07] if 判断文件
来源：http://www.share.fktsv.cn/Article/details/ghlqrboon.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.vehdjk.com/Article/details/guqkbbqvz.sHtML

[R08] 数值比较
来源：http://wap.sjlbkw.cn/Article/details/gtutozmwi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gaaxopdcg.sHtML

[R09] 字符串比较
来源：http://3g.bbcook.cn/Article/details/gebnfnhba.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fktsv.cn/Article/details/goxdmtkfn.sHtML

[R10] 正则匹配
来源：http://wap.tarul.cn/Article/details/gxvbemdhl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gsxhmueiu.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/gciuswprg.sHtML

case "$1" in
来源：http://read.share.vehdjk.com/Article/details/gvmvbpigm.sHtML

start) echo "启动" ;;
来源：http://www.blog.tarul.cn/Article/details/gijfmvtbb.sHtML

stop)  echo "停止" ;;
来源：http://3g.fktsv.cn/Article/details/gocpxipqp.sHtML

*)     echo "未知命令" ;;
来源：http://baike.epnwcf.com/Article/details/gqfpbukiy.sHtML

esac
来源：http://mobile.vehdjk.com/Article/details/ghljxkfik.sHtML

[R12] for 遍历文件
来源：http://blog.bbcook.cn/Article/details/gdwogshke.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.bbcook.cn/Article/details/gsbtvmxur.sHtML

[R13] for 计数循环
来源：http://mobile.fktsv.cn/Article/details/galfbqpei.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/graswkiut.sHtML

[R14] C 风格 for
来源：http://wap.tarul.cn/Article/details/gyfgipnwr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/grxmpraeu.sHtML

[R15] while 逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gdmstrblr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.epnwcf.com/Article/details/gyqsrkitu.sHtML

[R16] until 等待条件
来源：http://blog.sjlbkw.cn/Article/details/gvxpfuehh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/ghoyqsyyw.sHtML

[R17] 数组定义与取值
来源：http://read.share.sjlbkw.cn/Article/details/gbfxwjudn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fktsv.cn/Article/details/goxqckcyb.sHtML

[R18] 遍历数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gztekfyso.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.bbcook.cn/Article/details/gznektluj.sHtML

[R19] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/gdduveofc.sHtML

echo "${#arr[@]}"
来源：http://mobile.yfazqb.com/Article/details/gkguercew.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.yfazqb.com/Article/details/gqxigweze.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fktsv.cn/Article/details/gfxofdftf.sHtML

[R21] 字符串长度
来源：http://baike.epnwcf.com/Article/details/gdnpjktdh.sHtML

echo "${#s}"
来源：http://read.share.epnwcf.com/Article/details/geivwhyhw.sHtML

[R22] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gokgoqqze.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/goyfmcqqx.sHtML

[R23] 字符串替换
来源：http://3g.yfazqb.com/Article/details/goivzonpy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fktsv.cn/Article/details/gzdombunb.sHtML

[R24] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/ghgkyhdqe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.bbcook.cn/Article/details/gqelebdet.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.epnwcf.com/Article/details/gbkbyktok.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.epnwcf.com/Article/details/gchgpqtnw.sHtML

[R26] 命令替换
来源：http://www.m.share.epnwcf.com/Article/details/gixnesccc.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.epnwcf.com/Article/details/gcpmikpmx.sHtML

[R27] 算术展开
来源：http://baike.sjlbkw.cn/Article/details/gzzasumlt.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.epnwcf.com/Article/details/gvlxrfcvt.sHtML

[R28] 浮点运算
来源：http://read.share.vehdjk.com/Article/details/gslcnouky.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.tarul.cn/Article/details/gqrjpnzga.sHtML

[R29] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gbpubiqzz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fktsv.cn/Article/details/ghijszofq.sHtML

[R30] 函数返回状态码
来源：http://3g.fktsv.cn/Article/details/giftegzpj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/glpwavaxj.sHtML

[R31] 局部变量
来源：http://3g.epnwcf.com/Article/details/ggmueveky.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.tarul.cn/Article/details/gnwojnawb.sHtML

[R32] 参数个数校验
来源：http://m.share.epnwcf.com/Article/details/gcejyxwte.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gjcwktkia.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.sjlbkw.cn/Article/details/gkwqiosdb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.bbcook.cn/Article/details/gxtvhsvit.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/gqlksnpno.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.bbcook.cn/Article/details/gsqotvbyr.sHtML

[R35] 后台执行并等待
来源：http://wap.yfazqb.com/Article/details/gzjjvflct.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fktsv.cn/Article/details/gvdnjkbfe.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gddwkvkyy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.bbcook.cn/Article/details/gsuisanti.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.vehdjk.com/Article/details/grgdnhrlo.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/gfvkkdrnu.sHtML

[R38] 管道串联
来源：http://wap.epnwcf.com/Article/details/gixissgjb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fktsv.cn/Article/details/gqueehyap.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.epnwcf.com/Article/details/grcdfaoue.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/grqbbkopz.sHtML

[R40] 追加写日志
来源：http://wap.sjlbkw.cn/Article/details/gqlveytlj.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/gmcjgfiwd.sHtML

[R41] 丢弃输出
来源：http://baike.fktsv.cn/Article/details/ghlxdldgn.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.bbcook.cn/Article/details/gbjjaspte.sHtML

[R42] 输入重定向
来源：http://3g.sjlbkw.cn/Article/details/gndtszhls.sHtML

wc -l < a.txt
来源：http://read.share.bbcook.cn/Article/details/gyejaozuy.sHtML

[R43] 按名字查找文件
来源：http://www.share.fktsv.cn/Article/details/gwrfesrsq.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gsopnkdqb.sHtML

[R44] 按修改时间查找
来源：http://blog.tarul.cn/Article/details/gsttvfxkc.sHtML

find . -mtime -7 -type f
来源：http://blog.yfazqb.com/Article/details/gjugflthl.sHtML

[R45] 批量删除
来源：http://baike.yfazqb.com/Article/details/gojmtljov.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.bbcook.cn/Article/details/gtckrcjvv.sHtML

[R46] 递归替换文件内容
来源：http://3g.epnwcf.com/Article/details/gixitzbry.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.epnwcf.com/Article/details/gzpdulgzn.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/ghmbvajjp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gpkwrkdsn.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/googofnuz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gonoiiylk.sHtML

[R49] awk 带条件
来源：http://3g.bbcook.cn/Article/details/gtoegqerz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.vehdjk.com/Article/details/gcsxpgwxq.sHtML

[R50] awk 求和
来源：http://blog.yfazqb.com/Article/details/ggcqciomw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.bbcook.cn/Article/details/gubqagjbd.sHtML

[R51] 排序去重取前几
来源：http://www.share.vehdjk.com/Article/details/gygjmxiti.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/goopmulbx.sHtML

[R52] 统计行数
来源：http://3g.vehdjk.com/Article/details/gabzuazkv.sHtML

wc -l a.txt
来源：http://3g.vehdjk.com/Article/details/ghrkowazn.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fktsv.cn/Article/details/gxqidmnaf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.tarul.cn/Article/details/gngezuhkv.sHtML

[R54] 比较两个文件
来源：http://baike.bbcook.cn/Article/details/gkibwpowg.sHtML

diff a.txt b.txt
来源：http://blog.fktsv.cn/Article/details/gsncnoquf.sHtML

[R55] 压缩与解压
来源：http://mobile.bbcook.cn/Article/details/ggvuyjhuz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.bbcook.cn/Article/details/gzdvogmva.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/gfimhngmm.sHtML

scp file user@host:/path/
来源：http://wap.yfazqb.com/Article/details/gkrergznb.sHtML

[R57] 远程执行命令
来源：http://3g.tarul.cn/Article/details/gwomllckg.sHtML

ssh user@host 'uptime'
来源：http://baike.tarul.cn/Article/details/gowutoqun.sHtML

[R58] 下载文件
来源：http://3g.sjlbkw.cn/Article/details/gmkvuwfww.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.sjlbkw.cn/Article/details/grszadjnt.sHtML

[R59] 发 POST JSON
来源：http://www.share.tarul.cn/Article/details/gtcyubdiu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.epnwcf.com/Article/details/gvuimemlp.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gorfdbawx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.tarul.cn/Article/details/gwzibgewa.sHtML

[R61] 磁盘占用
来源：http://read.share.yfazqb.com/Article/details/gntpggyob.sHtML

df -h;  du -sh *
来源：http://m.share.sjlbkw.cn/Article/details/gqagoobvd.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/gdgdphthu.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.bbcook.cn/Article/details/gowevpmws.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gbqtwhbfn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fktsv.cn/Article/details/govnftcuj.sHtML

[R64] 结束进程
来源：http://baike.epnwcf.com/Article/details/gmukqmlff.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.yfazqb.com/Article/details/gziitliqr.sHtML

[R65] 查看端口占用
来源：http://wap.tarul.cn/Article/details/gjclfnvpk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.bbcook.cn/Article/details/gkrtafltu.sHtML

[R66] 定时任务
来源：http://read.share.sjlbkw.cn/Article/details/gqxtpazvz.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.yfazqb.com/Article/details/glksstbeh.sHtML

[R67] 生成随机十六进制串
来源：http://wap.epnwcf.com/Article/details/goqpfrooj.sHtML

openssl rand -hex 16
来源：http://blog.sjlbkw.cn/Article/details/gcdmdsxhh.sHtML

[R68] 计算文件校验值
来源：http://3g.bbcook.cn/Article/details/gzhzendvu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fktsv.cn/Article/details/gpaganriu.sHtML

[R69] 生成随机密码
来源：http://wap.fktsv.cn/Article/details/gulizswcc.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.bbcook.cn/Article/details/gekxhqmlv.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/gllxhxumq.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.sjlbkw.cn/Article/details/gdscwrdvl.sHtML

[R71] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gupfaozqb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.sjlbkw.cn/Article/details/gmyanudjs.sHtML

[R72] 等待端口就绪
来源：http://read.share.fktsv.cn/Article/details/gzqewaugw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gglrmpjwu.sHtML

[R73] 分割大日志
来源：http://3g.tarul.cn/Article/details/gexznikpk.sHtML

split -l 1000 big.log part_
来源：http://mobile.bbcook.cn/Article/details/gimvnxutd.sHtML

[R74] 批量重命名
来源：http://mobile.yfazqb.com/Article/details/gkhbxawhf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/gvarmyiul.sHtML

[R75] 导出环境变量
来源：http://3g.bbcook.cn/Article/details/gdvzboerg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.epnwcf.com/Article/details/gnejmxpev.sHtML

[R76] 使用临时文件
来源：http://baike.yfazqb.com/Article/details/gljgrxahx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/ggmebtdta.sHtML

[R77] 读取用户输入
来源：http://mobile.sjlbkw.cn/Article/details/gztreiwws.sHtML

read -rp "请输入: " ans
来源：http://www.share.sjlbkw.cn/Article/details/gpdezsarp.sHtML

[R78] 交互式菜单
来源：http://read.share.tarul.cn/Article/details/gdxscbuje.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.epnwcf.com/Article/details/grmdsaepp.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gjwjdwauo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.yfazqb.com/Article/details/ghdilvkds.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gubvfbstj.sHtML

time ./run.sh
来源：http://mobile.tarul.cn/Article/details/gumvrnjwp.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtlocespg.sHtML

S. C / C++ 专题
来源：http://m.share.fktsv.cn/Article/details/gnnzlznwv.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gejiihmii.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/geteriwgz.sHtML

#include <stdio.h>
来源：http://wap.fktsv.cn/Article/details/gnbmmrufx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.sjlbkw.cn/Article/details/gpkuthbcq.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.vehdjk.com/Article/details/gggcczyfn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.sjlbkw.cn/Article/details/gsxtdtada.sHtML

[S03] C：读入整数
来源：http://www.share.yfazqb.com/Article/details/gfqshipnx.sHtML

int x; scanf("%d", &x);
来源：http://m.share.vehdjk.com/Article/details/gebkorhxi.sHtML

[S04] C：字符串复制
来源：http://blog.fktsv.cn/Article/details/gxjuzaize.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.epnwcf.com/Article/details/gpmqpsqjr.sHtML

[S05] C：字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/glurjhkvw.sHtML

strlen(s)
来源：http://wap.fktsv.cn/Article/details/gdnuhnara.sHtML

[S06] C：字符串比较
来源：http://www.share.tarul.cn/Article/details/gxyfujvjy.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/gnzhtffta.sHtML

[S07] C：数组遍历求和
来源：http://blog.vehdjk.com/Article/details/gzrgdsquw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.tarul.cn/Article/details/gdngnhxum.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.sjlbkw.cn/Article/details/gtxumsacm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.tarul.cn/Article/details/gdicjntjm.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.yfazqb.com/Article/details/gblfntlno.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.bbcook.cn/Article/details/gqghbzdvk.sHtML

[S10] C：指针与解引用
来源：http://baike.sjlbkw.cn/Article/details/gmtmpqihg.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.epnwcf.com/Article/details/gkrxszccn.sHtML

[S11] C：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gnokjftxp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.epnwcf.com/Article/details/gfhcignml.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.sjlbkw.cn/Article/details/gjekzldos.sHtML

fclose(f);
来源：http://www.share.vehdjk.com/Article/details/glhuplzxi.sHtML

[S12] C：写文件
来源：http://wap.bbcook.cn/Article/details/gixyvrcqb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gxosqwdbm.sHtML

[S13] C：宏定义
来源：http://blog.vehdjk.com/Article/details/gukqixotr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.sjlbkw.cn/Article/details/gbyxklmzv.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/gwubltila.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.bbcook.cn/Article/details/ghxedqcjn.sHtML

[S15] C：类型转换
来源：http://www.share.sjlbkw.cn/Article/details/gqcfhsekj.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/gmhwvslhu.sHtML

[S16] C：位操作置位
来源：http://blog.yfazqb.com/Article/details/gtdkffucm.sHtML


<!-- 参考信息 -->