代发 wailian999

[Q48] CTE 公用表表达式
来源：http://3g.yfazqb.com/Article/details/gxwrebgpa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.sjlbkw.cn/Article/details/gjiyqnhxj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.bbcook.cn/Article/details/gvjklefbc.sHtML

[Q49] 更新单行
来源：http://www.share.tarul.cn/Article/details/gvnysbjfr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/gkavkxdog.sHtML

[Q50] 批量更新
来源：http://m.share.vehdjk.com/Article/details/gfsoyytfu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwpogbmo.sHtML

[Q51] 用子查询更新
来源：http://www.share.yfazqb.com/Article/details/gyejgkptm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.sjlbkw.cn/Article/details/ggflxvajf.sHtML

[Q52] 删除指定行
来源：http://m.share.sjlbkw.cn/Article/details/gxunhzuqq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gzhnpzlzk.sHtML

[Q53] 按条件删除
来源：http://www.m.share.tarul.cn/Article/details/giuzkerit.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.yfazqb.com/Article/details/gokcydfig.sHtML

[Q54] 清空表
来源：http://3g.sjlbkw.cn/Article/details/gyekkgshy.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.vehdjk.com/Article/details/gybdzntfj.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.sjlbkw.cn/Article/details/genupuxnr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gqfvffbny.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.bbcook.cn/Article/details/gdudkvfzu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.yfazqb.com/Article/details/gdepsvlml.sHtML

[Q57] 行号
来源：http://3g.yfazqb.com/Article/details/gwpwdvacs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.yfazqb.com/Article/details/gotmahowc.sHtML

[Q58] 累计求和
来源：http://mobile.tarul.cn/Article/details/grekyzrwj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gadmxmcta.sHtML

[Q59] 分组内累计
来源：http://m.share.tarul.cn/Article/details/gemxqxggj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/grcpiqexh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.vehdjk.com/Article/details/gmtdqvpmg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.bbcook.cn/Article/details/gzjiongek.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.tarul.cn/Article/details/gqajckazm.sHtML

[Q61] 移动平均
来源：http://www.share.epnwcf.com/Article/details/gtlvpjfxn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gcbhrbrms.sHtML

[Q62] 分组占比
来源：http://mobile.epnwcf.com/Article/details/gkymsfnbb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gyzegqycn.sHtML

[Q63] 开启事务
来源：http://blog.bbcook.cn/Article/details/gqmynepck.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.epnwcf.com/Article/details/gvlmkzimx.sHtML

[Q64] 提交事务
来源：http://read.share.tarul.cn/Article/details/ggsksnxgd.sHtML

COMMIT;
来源：http://baike.yfazqb.com/Article/details/geudajnop.sHtML

[Q65] 回滚事务
来源：http://baike.sjlbkw.cn/Article/details/gcievgrnf.sHtML

ROLLBACK;
来源：http://www.share.bbcook.cn/Article/details/gecgwyssn.sHtML

[Q66] 行锁查询
来源：http://3g.sjlbkw.cn/Article/details/gsmsxcxht.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fktsv.cn/Article/details/gnvnvbbby.sHtML

[Q67] 设置隔离级别
来源：http://3g.bbcook.cn/Article/details/gpvgpxqup.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.bbcook.cn/Article/details/gvjxgcqcd.sHtML

[Q68] 保存点
来源：http://read.share.epnwcf.com/Article/details/gecoegatf.sHtML

SAVEPOINT sp1;
来源：http://www.share.bbcook.cn/Article/details/grbogqcnj.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gxshutunj.sHtML

[Q69] 查看执行计划
来源：http://m.share.epnwcf.com/Article/details/gwtwabxse.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.yfazqb.com/Article/details/gowmghjon.sHtML

[Q70] 更新统计信息
来源：http://mobile.bbcook.cn/Article/details/gguxxopfe.sHtML

ANALYZE TABLE users;
来源：http://read.share.epnwcf.com/Article/details/gcqhhjuei.sHtML

[Q71] 查看建表语句
来源：http://wap.vehdjk.com/Article/details/gzwibixwy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.yfazqb.com/Article/details/gtpzqxutf.sHtML

[Q72] 查看索引
来源：http://m.share.epnwcf.com/Article/details/gfnvekanl.sHtML

SHOW INDEX FROM users;
来源：http://mobile.bbcook.cn/Article/details/gwovnxsuv.sHtML

[Q73] 查看表状态
来源：http://blog.fktsv.cn/Article/details/gkjypwhoc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.sjlbkw.cn/Article/details/gnkuwysbk.sHtML

[Q74] 强制使用索引
来源：http://mobile.bbcook.cn/Article/details/godnvqebv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.vehdjk.com/Article/details/gqsgjelgp.sHtML

[Q75] 日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/gbggtslqt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gvgnmfgqf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.yfazqb.com/Article/details/grnpqpguu.sHtML

[Q76] 按天统计
来源：http://baike.sjlbkw.cn/Article/details/gjqktrjvx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fktsv.cn/Article/details/gswdkvveu.sHtML

[Q77] 时间加减
来源：http://baike.epnwcf.com/Article/details/gknirwvwu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.epnwcf.com/Article/details/ghqgprkgp.sHtML

[Q78] 当前时间
来源：http://blog.tarul.cn/Article/details/ghzufkitc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.sjlbkw.cn/Article/details/glngpaxwg.sHtML

[Q79] 字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gtmkhmsvb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fktsv.cn/Article/details/ggsshlcvx.sHtML

[Q80] 字符串截取
来源：http://blog.yfazqb.com/Article/details/gonwxclzn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.bbcook.cn/Article/details/gtojqsjar.sHtML

[Q81] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/gbubekwmc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gekleuhul.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.bbcook.cn/Article/details/gyustdywi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gzwlichvz.sHtML

[Q83] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gyjhwczub.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gejbcpjvo.sHtML

[Q84] 去除首尾空格
来源：http://m.share.sjlbkw.cn/Article/details/gfwoxdhgd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gnjugevnt.sHtML

[Q85] 数值取整
来源：http://wap.epnwcf.com/Article/details/gzybyensb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.vehdjk.com/Article/details/glmsdezci.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.tarul.cn/Article/details/gthgymiom.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fktsv.cn/Article/details/gmexeylcj.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gdhmrvymh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.yfazqb.com/Article/details/gvfgcecqh.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.tarul.cn/Article/details/grprrocul.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.bbcook.cn/Article/details/grnmlzvjw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fktsv.cn/Article/details/gkyjqwfxz.sHtML

[Q89] 判断表是否存在
来源：http://m.share.epnwcf.com/Article/details/gifciqiib.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.epnwcf.com/Article/details/gbiamvedi.sHtML

[Q90] 生成序号列
来源：http://www.share.epnwcf.com/Article/details/geofzrrqx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.tarul.cn/Article/details/gbnofstco.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gtpegpqkt.sHtML

R. Bash 专题
来源：http://wap.vehdjk.com/Article/details/gdlxheojd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gjlswgmyw.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fktsv.cn/Article/details/gjtryuxlp.sHtML

#!/usr/bin/env bash
来源：http://m.share.tarul.cn/Article/details/glamaewib.sHtML

set -euo pipefail
来源：http://mobile.vehdjk.com/Article/details/gevrkmqfd.sHtML

[R02] 变量赋值与使用
来源：http://m.share.bbcook.cn/Article/details/gzapqhdek.sHtML

name="Tom"; echo "$name"
来源：http://m.share.yfazqb.com/Article/details/ggsodqnri.sHtML

[R03] 只读变量
来源：http://m.share.fktsv.cn/Article/details/goswuzdkt.sHtML

readonly PI=3.14
来源：http://blog.sjlbkw.cn/Article/details/gveejljxy.sHtML

[R04] 位置参数
来源：http://www.m.share.vehdjk.com/Article/details/gsyuoigbr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.bbcook.cn/Article/details/geudfknub.sHtML

[R05] 参数默认值
来源：http://read.share.epnwcf.com/Article/details/gvqcbeawo.sHtML

name="${1:-default}"
来源：http://www.m.share.yfazqb.com/Article/details/gowvifswk.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.tarul.cn/Article/details/gbvwozypc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gcglbowvs.sHtML

[R07] if 判断文件
来源：http://www.blog.yfazqb.com/Article/details/gjfhnjxmc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gmpacrjfk.sHtML

[R08] 数值比较
来源：http://3g.sjlbkw.cn/Article/details/ggrysjjby.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.yfazqb.com/Article/details/gedvppnfr.sHtML

[R09] 字符串比较
来源：http://baike.epnwcf.com/Article/details/glfipmysz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.epnwcf.com/Article/details/gkjhriyea.sHtML

[R10] 正则匹配
来源：http://mobile.bbcook.cn/Article/details/greatmhvp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.sjlbkw.cn/Article/details/ggsgoutwo.sHtML

[R11] case 多分支
来源：http://mobile.fktsv.cn/Article/details/gneqlrgwc.sHtML

case "$1" in
来源：http://www.blog.bbcook.cn/Article/details/gmqbumbgv.sHtML

start) echo "启动" ;;
来源：http://mobile.yfazqb.com/Article/details/gkjezlafv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gacbwytoz.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gbcxbulkl.sHtML

esac
来源：http://blog.epnwcf.com/Article/details/gwktexavm.sHtML

[R12] for 遍历文件
来源：http://www.share.tarul.cn/Article/details/gedzuouhp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.bbcook.cn/Article/details/gnsmzphga.sHtML

[R13] for 计数循环
来源：http://www.share.tarul.cn/Article/details/gkpwhzxio.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/ghacvatxf.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gsvvpcceo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/gkappucme.sHtML

[R15] while 逐行读文件
来源：http://wap.vehdjk.com/Article/details/gmrgvwcxj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.vehdjk.com/Article/details/gfiygwgga.sHtML

[R16] until 等待条件
来源：http://www.blog.vehdjk.com/Article/details/galmggkuu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/gatdhxsom.sHtML

[R17] 数组定义与取值
来源：http://www.share.epnwcf.com/Article/details/gdyqksnhi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.sjlbkw.cn/Article/details/gxgdwobjy.sHtML

[R18] 遍历数组
来源：http://www.m.share.fktsv.cn/Article/details/gfftnvhrz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.vehdjk.com/Article/details/gdiazrsss.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/gaqqninnb.sHtML

echo "${#arr[@]}"
来源：http://m.share.yfazqb.com/Article/details/glngotrne.sHtML

[R20] 关联数组（字典）
来源：http://blog.bbcook.cn/Article/details/grjbnqhiv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.tarul.cn/Article/details/gsknkkdro.sHtML

[R21] 字符串长度
来源：http://3g.yfazqb.com/Article/details/gpbhdixka.sHtML

echo "${#s}"
来源：http://read.share.fktsv.cn/Article/details/gyxylennx.sHtML

[R22] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gkccvjrbb.sHtML

echo "${s:0:5}"
来源：http://read.share.epnwcf.com/Article/details/gxxiydwud.sHtML

[R23] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/gsxtbdjfy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.tarul.cn/Article/details/ggahdobml.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/glgwwyzws.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.yfazqb.com/Article/details/gohrjiicv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.tarul.cn/Article/details/gimpowwye.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.bbcook.cn/Article/details/gueoczkos.sHtML

[R26] 命令替换
来源：http://wap.sjlbkw.cn/Article/details/ggmpzvthe.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.sjlbkw.cn/Article/details/gpdwgdrgn.sHtML

[R27] 算术展开
来源：http://wap.tarul.cn/Article/details/ghgxbjeww.sHtML

echo $((1 + 2 * 3))
来源：http://wap.bbcook.cn/Article/details/gijiolgez.sHtML

[R28] 浮点运算
来源：http://mobile.epnwcf.com/Article/details/ganoesmev.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.epnwcf.com/Article/details/gggbboimc.sHtML

[R29] 定义函数
来源：http://blog.vehdjk.com/Article/details/gzhdmcexp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gesmxklkz.sHtML

[R30] 函数返回状态码
来源：http://read.share.epnwcf.com/Article/details/gwppznwjd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fktsv.cn/Article/details/gugetylyg.sHtML

[R31] 局部变量
来源：http://read.share.bbcook.cn/Article/details/galubnnwy.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.tarul.cn/Article/details/grjwiifwg.sHtML

[R32] 参数个数校验
来源：http://mobile.epnwcf.com/Article/details/gynuwbqxq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gmcdmkjuz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.epnwcf.com/Article/details/glwtxoivf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.sjlbkw.cn/Article/details/gywefclso.sHtML

[R34] 退出时清理
来源：http://www.blog.yfazqb.com/Article/details/grehqekzi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/glfshcerx.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/gxnxstdxn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.yfazqb.com/Article/details/guloqszkx.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.yfazqb.com/Article/details/gskzjrexx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.vehdjk.com/Article/details/ghbuneftz.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.yfazqb.com/Article/details/gewrgtoqt.sHtML

files=$(ls -1)
来源：http://baike.tarul.cn/Article/details/gabbpmlgi.sHtML

[R38] 管道串联
来源：http://www.share.bbcook.cn/Article/details/gmlrfxkca.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.epnwcf.com/Article/details/ghjnohygj.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.bbcook.cn/Article/details/gdvsgygvt.sHtML

cmd > out.log 2>&1
来源：http://read.share.epnwcf.com/Article/details/godrpgtcy.sHtML

[R40] 追加写日志
来源：http://baike.vehdjk.com/Article/details/gokvtnnvi.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/grgklwbwi.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/gxciyutus.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fktsv.cn/Article/details/gsgfdsbee.sHtML

[R42] 输入重定向
来源：http://m.share.sjlbkw.cn/Article/details/gakpddtbw.sHtML

wc -l < a.txt
来源：http://www.blog.fktsv.cn/Article/details/gpqbyiwrr.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.vehdjk.com/Article/details/gwqbjrizx.sHtML

find . -name "*.log" -type f
来源：http://www.share.fktsv.cn/Article/details/gfddsbwiv.sHtML

[R44] 按修改时间查找
来源：http://baike.sjlbkw.cn/Article/details/gnjoyigbd.sHtML

find . -mtime -7 -type f
来源：http://mobile.tarul.cn/Article/details/gkunoghma.sHtML

[R45] 批量删除
来源：http://m.share.yfazqb.com/Article/details/gkvjyvxnf.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.epnwcf.com/Article/details/gauafgwzb.sHtML

[R46] 递归替换文件内容
来源：http://read.share.epnwcf.com/Article/details/gqirnbbjc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.sjlbkw.cn/Article/details/gvjihiibi.sHtML

[R47] sed 单行替换
来源：http://baike.sjlbkw.cn/Article/details/gysrprbag.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/ginethgeh.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/gmbfpddyy.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.tarul.cn/Article/details/gqytokeyg.sHtML

[R49] awk 带条件
来源：http://blog.vehdjk.com/Article/details/grlblsdnk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fktsv.cn/Article/details/ghcenzovr.sHtML

[R50] awk 求和
来源：http://www.share.vehdjk.com/Article/details/gqmfqeppg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gkjurbfei.sHtML

[R51] 排序去重取前几
来源：http://www.share.epnwcf.com/Article/details/glugeizlt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.vehdjk.com/Article/details/gwzsqifiq.sHtML

[R52] 统计行数
来源：http://3g.tarul.cn/Article/details/gxqzfavem.sHtML

wc -l a.txt
来源：http://mobile.tarul.cn/Article/details/gcukjlpfq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.vehdjk.com/Article/details/ghpyuifhs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.bbcook.cn/Article/details/gjxldlwpo.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fktsv.cn/Article/details/gjqjutlhv.sHtML

diff a.txt b.txt
来源：http://blog.fktsv.cn/Article/details/gqkzpvrnf.sHtML

[R55] 压缩与解压
来源：http://mobile.bbcook.cn/Article/details/gadliaakf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fktsv.cn/Article/details/gegeyryrv.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/gmhbdvdqx.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gehriqilx.sHtML

[R57] 远程执行命令
来源：http://3g.yfazqb.com/Article/details/ghxcnbgvy.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.yfazqb.com/Article/details/gmowjkoty.sHtML

[R58] 下载文件
来源：http://read.share.yfazqb.com/Article/details/gfhwewctv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.sjlbkw.cn/Article/details/glyjllhhf.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gwhmcbotk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.vehdjk.com/Article/details/guzawxxqt.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gpektzvgc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fktsv.cn/Article/details/gblgfjrqf.sHtML

[R61] 磁盘占用
来源：http://www.share.bbcook.cn/Article/details/gcpukbhwy.sHtML

df -h;  du -sh *
来源：http://read.share.bbcook.cn/Article/details/gltlnsudh.sHtML

[R62] 找最占空间的文件
来源：http://m.share.sjlbkw.cn/Article/details/galrtrpxc.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fktsv.cn/Article/details/gvcefukgu.sHtML

[R63] 内存与进程
来源：http://wap.epnwcf.com/Article/details/gdymnxtxc.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.tarul.cn/Article/details/gpchxiwpj.sHtML

[R64] 结束进程
来源：http://read.share.bbcook.cn/Article/details/gtvfuriul.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.bbcook.cn/Article/details/gborjoivr.sHtML

[R65] 查看端口占用
来源：http://m.share.yfazqb.com/Article/details/gaikodbpi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.yfazqb.com/Article/details/gxuahdwfl.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/gbvtolkop.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/gvvhogbmi.sHtML

[R67] 生成随机十六进制串
来源：http://blog.vehdjk.com/Article/details/gevzctxtt.sHtML

openssl rand -hex 16
来源：http://www.share.bbcook.cn/Article/details/gxuhvwxbx.sHtML

[R68] 计算文件校验值
来源：http://read.share.epnwcf.com/Article/details/giqfwqkop.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.sjlbkw.cn/Article/details/geldwqtbc.sHtML

[R69] 生成随机密码
来源：http://mobile.bbcook.cn/Article/details/gijmzsljo.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/gkkqcpkoc.sHtML

[R70] 时间戳与互转
来源：http://mobile.tarul.cn/Article/details/gcpkntzji.sHtML

date +%s;  date -d @1700000000
来源：http://3g.yfazqb.com/Article/details/gsqdeelof.sHtML

[R71] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gnllyhhah.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.vehdjk.com/Article/details/glwiqbrfb.sHtML

[R72] 等待端口就绪
来源：http://3g.tarul.cn/Article/details/gmvucnylw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/glerjpcyu.sHtML

[R73] 分割大日志
来源：http://www.blog.fktsv.cn/Article/details/gqsegrmhv.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.yfazqb.com/Article/details/gsktxrgmy.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/glzalhadz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/gsgdevcgu.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/gwjgyqlkr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.bbcook.cn/Article/details/gcbkzwlqm.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/gekrgxbli.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gtqvtjgdh.sHtML

[R77] 读取用户输入
来源：http://mobile.yfazqb.com/Article/details/gyowguiev.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.tarul.cn/Article/details/gwiaawekx.sHtML

[R78] 交互式菜单
来源：http://blog.bbcook.cn/Article/details/gqvgfrtyq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.epnwcf.com/Article/details/gfqjalmmx.sHtML

[R79] 解析命令行选项
来源：http://www.blog.vehdjk.com/Article/details/gzitctwkr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.yfazqb.com/Article/details/gsffsfizh.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.bbcook.cn/Article/details/gffbyvvgt.sHtML

time ./run.sh
来源：http://www.share.bbcook.cn/Article/details/gwuruusmv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gixuapeeh.sHtML

S. C / C++ 专题
来源：http://www.blog.yfazqb.com/Article/details/gsgeznjmv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnbgksmtg.sHtML

[S01] C：Hello World
来源：http://www.share.fktsv.cn/Article/details/giqyhbtnr.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/gociikblq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fktsv.cn/Article/details/guozuespe.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fktsv.cn/Article/details/gtidbsvrz.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.tarul.cn/Article/details/gpihklngb.sHtML

[S03] C：读入整数
来源：http://www.blog.yfazqb.com/Article/details/goxtavxip.sHtML

int x; scanf("%d", &x);
来源：http://blog.bbcook.cn/Article/details/gvmjsymio.sHtML

[S04] C：字符串复制
来源：http://wap.tarul.cn/Article/details/gulsvhtkb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gkcnruqzh.sHtML

[S05] C：字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gilzdxfsp.sHtML

strlen(s)
来源：http://m.share.sjlbkw.cn/Article/details/gwneiloja.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/gfngfufzm.sHtML

strcmp(a, b) == 0
来源：http://www.blog.vehdjk.com/Article/details/geeeareah.sHtML

[S07] C：数组遍历求和
来源：http://wap.epnwcf.com/Article/details/gkikxcijd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fktsv.cn/Article/details/gcehjzxkb.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/gscjjxdur.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/ggdclgrxt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.sjlbkw.cn/Article/details/gaomdffjy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.epnwcf.com/Article/details/gbvbtvqia.sHtML

[S10] C：指针与解引用
来源：http://read.share.tarul.cn/Article/details/gahhgtvju.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.vehdjk.com/Article/details/gpmwevios.sHtML

[S11] C：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/golhsaibr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.vehdjk.com/Article/details/gqhbtwwfe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.vehdjk.com/Article/details/glrgncrad.sHtML

fclose(f);
来源：http://wap.yfazqb.com/Article/details/gzhkjbktt.sHtML

[S12] C：写文件
来源：http://www.share.fktsv.cn/Article/details/gqjxmiauo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gmwtezqzg.sHtML

[S13] C：宏定义
来源：http://baike.fktsv.cn/Article/details/gtkgnijuz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.vehdjk.com/Article/details/gphnbbyrk.sHtML

[S14] C：枚举
来源：http://www.blog.yfazqb.com/Article/details/gdacjyqxw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fktsv.cn/Article/details/gxzdmfthh.sHtML

[S15] C：类型转换
来源：http://m.share.epnwcf.com/Article/details/gsqqvcvvt.sHtML

(double) a / b
来源：http://blog.fktsv.cn/Article/details/gmkldtzwc.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fktsv.cn/Article/details/ginzakhwo.sHtML

x |= (1 << 3);
来源：http://baike.tarul.cn/Article/details/gxutvjgtj.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gykrqbjtc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.epnwcf.com/Article/details/ggnzraejl.sHtML

[S18] C：命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gnaeamqow.sHtML


<!-- 参考信息 -->