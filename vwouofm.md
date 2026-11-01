代发 wailian999

[Q44] IN 子查询
来源：http://m.share.fktsv.cn/Article/details/gkuflfnvo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.sjlbkw.cn/Article/details/gdnskxwlj.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.yfazqb.com/Article/details/gvzkltuko.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/gfxkielkz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fktsv.cn/Article/details/gcygkatrc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gzmnbhkjj.sHtML

[Q47] 与平均值比较
来源：http://blog.fktsv.cn/Article/details/gqgiqdfsd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.bbcook.cn/Article/details/gnhavxcqq.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.bbcook.cn/Article/details/gxwpffxib.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/grdcupzqn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/gtnihikxb.sHtML

[Q49] 更新单行
来源：http://baike.tarul.cn/Article/details/guidonawb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbmblyuh.sHtML

[Q50] 批量更新
来源：http://www.blog.tarul.cn/Article/details/gsrlvvkie.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.bbcook.cn/Article/details/gwyuhwoai.sHtML

[Q51] 用子查询更新
来源：http://read.share.sjlbkw.cn/Article/details/gouaadmaw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.epnwcf.com/Article/details/gdiofpelt.sHtML

[Q52] 删除指定行
来源：http://m.share.vehdjk.com/Article/details/gvfolcfjp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gmxyqhsrn.sHtML

[Q53] 按条件删除
来源：http://www.share.tarul.cn/Article/details/glloutuln.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.tarul.cn/Article/details/gphfqobsg.sHtML

[Q54] 清空表
来源：http://3g.tarul.cn/Article/details/gxbjhddqa.sHtML

TRUNCATE TABLE logs;
来源：http://wap.vehdjk.com/Article/details/gdmrnmlcx.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.tarul.cn/Article/details/gawuafroc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gxvgfuktf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.sjlbkw.cn/Article/details/gxajbvxtr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.tarul.cn/Article/details/ghfjlepza.sHtML

[Q57] 行号
来源：http://www.m.share.vehdjk.com/Article/details/gynwelbmu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gkspsjkbj.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/guiywhcax.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gdbiudksn.sHtML

[Q59] 分组内累计
来源：http://www.share.vehdjk.com/Article/details/gllzdpqci.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbnnlnhq.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.yfazqb.com/Article/details/gyjpvbtnz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.yfazqb.com/Article/details/gneunultu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fktsv.cn/Article/details/gatisakrb.sHtML

[Q61] 移动平均
来源：http://baike.sjlbkw.cn/Article/details/gnustsxyt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gvghcudyc.sHtML

[Q62] 分组占比
来源：http://m.share.yfazqb.com/Article/details/gzregqilt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/ghzpfhfeq.sHtML

[Q63] 开启事务
来源：http://read.share.tarul.cn/Article/details/gfvvtwgue.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.yfazqb.com/Article/details/gseofsost.sHtML

[Q64] 提交事务
来源：http://read.share.epnwcf.com/Article/details/gweykpscn.sHtML

COMMIT;
来源：http://m.share.epnwcf.com/Article/details/gylvbnhra.sHtML

[Q65] 回滚事务
来源：http://www.m.share.vehdjk.com/Article/details/gsfsnhqvh.sHtML

ROLLBACK;
来源：http://www.share.tarul.cn/Article/details/gdjidpjrh.sHtML

[Q66] 行锁查询
来源：http://wap.vehdjk.com/Article/details/ggzyjyugc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.tarul.cn/Article/details/ghthvpfbm.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.vehdjk.com/Article/details/ghzmlcqmi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.vehdjk.com/Article/details/gyyfitvin.sHtML

[Q68] 保存点
来源：http://blog.fktsv.cn/Article/details/gddxkwnew.sHtML

SAVEPOINT sp1;
来源：http://m.share.tarul.cn/Article/details/gcdyzufan.sHtML

ROLLBACK TO sp1;
来源：http://mobile.tarul.cn/Article/details/gzeeibmdb.sHtML

[Q69] 查看执行计划
来源：http://www.share.epnwcf.com/Article/details/gvwopsait.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/gvcwcnbxn.sHtML

[Q70] 更新统计信息
来源：http://3g.epnwcf.com/Article/details/gyzitgrxz.sHtML

ANALYZE TABLE users;
来源：http://wap.yfazqb.com/Article/details/gypgfhrgm.sHtML

[Q71] 查看建表语句
来源：http://www.blog.yfazqb.com/Article/details/gybkppqct.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.tarul.cn/Article/details/glzaocybo.sHtML

[Q72] 查看索引
来源：http://www.share.epnwcf.com/Article/details/gipkuwvgg.sHtML

SHOW INDEX FROM users;
来源：http://read.share.epnwcf.com/Article/details/gintroacz.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/gyfoqbfse.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.epnwcf.com/Article/details/gvsrmmlqf.sHtML

[Q74] 强制使用索引
来源：http://3g.tarul.cn/Article/details/gapyagoka.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.bbcook.cn/Article/details/gshtqyjyi.sHtML

[Q75] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gvqviigjd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.epnwcf.com/Article/details/gyxbnynds.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.vehdjk.com/Article/details/gsejqfsat.sHtML

[Q76] 按天统计
来源：http://www.share.bbcook.cn/Article/details/gvtxamfes.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fktsv.cn/Article/details/gnegqqhcc.sHtML

[Q77] 时间加减
来源：http://mobile.bbcook.cn/Article/details/glcjagubb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.yfazqb.com/Article/details/gdnvwzxsz.sHtML

[Q78] 当前时间
来源：http://mobile.tarul.cn/Article/details/gkumvtmys.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.yfazqb.com/Article/details/gjpjqeegd.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gheuxnjhu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fktsv.cn/Article/details/gpnmvowps.sHtML

[Q80] 字符串截取
来源：http://read.share.epnwcf.com/Article/details/ghiayrxny.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.tarul.cn/Article/details/ggdnjarga.sHtML

[Q81] 字符串替换
来源：http://blog.vehdjk.com/Article/details/gogtirxqu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.yfazqb.com/Article/details/ggxteofdb.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/gxwglgiiu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gluuxtdec.sHtML

[Q83] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/geeerlomm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gpvsheiiy.sHtML

[Q84] 去除首尾空格
来源：http://blog.epnwcf.com/Article/details/grhtkcygq.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gjjrptzye.sHtML

[Q85] 数值取整
来源：http://m.share.yfazqb.com/Article/details/ggukezqzv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.sjlbkw.cn/Article/details/gzrfzukvw.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.sjlbkw.cn/Article/details/gcmzsyqso.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fktsv.cn/Article/details/glpwmskyt.sHtML

[Q87] JSON 字段做条件
来源：http://baike.bbcook.cn/Article/details/goeaoicjb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fktsv.cn/Article/details/ggqxgsuga.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fktsv.cn/Article/details/grmbgyerf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fktsv.cn/Article/details/gpdqmmplv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gywkvwxew.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fktsv.cn/Article/details/glxcwteej.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.epnwcf.com/Article/details/gtqsqisid.sHtML

[Q90] 生成序号列
来源：http://3g.epnwcf.com/Article/details/grekqyaos.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/gjueoacxb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ggtsbvvqc.sHtML

R. Bash 专题
来源：http://baike.sjlbkw.cn/Article/details/gxwseysab.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghbgzltoj.sHtML

[R01] shebang 与严格模式
来源：http://mobile.vehdjk.com/Article/details/ggssyncxa.sHtML

#!/usr/bin/env bash
来源：http://blog.vehdjk.com/Article/details/gdevtmxqg.sHtML

set -euo pipefail
来源：http://m.share.tarul.cn/Article/details/ggnhllofh.sHtML

[R02] 变量赋值与使用
来源：http://wap.epnwcf.com/Article/details/ghjlxyemj.sHtML

name="Tom"; echo "$name"
来源：http://blog.fktsv.cn/Article/details/gkvnxccad.sHtML

[R03] 只读变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gutetrlwr.sHtML

readonly PI=3.14
来源：http://wap.fktsv.cn/Article/details/gzormcmss.sHtML

[R04] 位置参数
来源：http://3g.sjlbkw.cn/Article/details/gujdqekkf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.yfazqb.com/Article/details/gplwedtue.sHtML

[R05] 参数默认值
来源：http://mobile.fktsv.cn/Article/details/gjkzeomud.sHtML

name="${1:-default}"
来源：http://m.share.bbcook.cn/Article/details/glmguuyus.sHtML

[R06] 判断命令是否存在
来源：http://blog.sjlbkw.cn/Article/details/gsbrtxobl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gzxhlumdg.sHtML

[R07] if 判断文件
来源：http://baike.epnwcf.com/Article/details/gywmvjdzg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.vehdjk.com/Article/details/gwpybyfqg.sHtML

[R08] 数值比较
来源：http://mobile.fktsv.cn/Article/details/gopxozyif.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fktsv.cn/Article/details/gchtwinsp.sHtML

[R09] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/gfejdgmgt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.yfazqb.com/Article/details/gzkkuwbxg.sHtML

[R10] 正则匹配
来源：http://mobile.epnwcf.com/Article/details/gtufzvbos.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.vehdjk.com/Article/details/gtqjzedne.sHtML

[R11] case 多分支
来源：http://www.share.bbcook.cn/Article/details/grehesyvp.sHtML

case "$1" in
来源：http://3g.bbcook.cn/Article/details/gomzcfcqy.sHtML

start) echo "启动" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gpfprhyoy.sHtML

stop)  echo "停止" ;;
来源：http://wap.tarul.cn/Article/details/gcfuwnwvk.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gmfvlbdml.sHtML

esac
来源：http://wap.yfazqb.com/Article/details/gwszulbun.sHtML

[R12] for 遍历文件
来源：http://mobile.bbcook.cn/Article/details/glwxapolg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.sjlbkw.cn/Article/details/guiwljlrl.sHtML

[R13] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/gixcddywc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/geoojsego.sHtML

[R14] C 风格 for
来源：http://www.blog.bbcook.cn/Article/details/ggubaddby.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gmboyrapc.sHtML

[R15] while 逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gpqdvqown.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.tarul.cn/Article/details/gsuuzxgvx.sHtML

[R16] until 等待条件
来源：http://baike.yfazqb.com/Article/details/gwubnliok.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/ggohcwqej.sHtML

[R17] 数组定义与取值
来源：http://wap.bbcook.cn/Article/details/ggvfmooox.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.bbcook.cn/Article/details/ggkigfzcm.sHtML

[R18] 遍历数组
来源：http://3g.yfazqb.com/Article/details/gvllykjzf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.yfazqb.com/Article/details/gkixcptwd.sHtML

[R19] 数组长度
来源：http://www.share.fktsv.cn/Article/details/ghyhlwrxu.sHtML

echo "${#arr[@]}"
来源：http://www.blog.epnwcf.com/Article/details/gjixgsogf.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/gilcwedmq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.yfazqb.com/Article/details/gkuvbzqzf.sHtML

[R21] 字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gokxdjwau.sHtML

echo "${#s}"
来源：http://blog.bbcook.cn/Article/details/gadxwkhfq.sHtML

[R22] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gnwaapspr.sHtML

echo "${s:0:5}"
来源：http://www.share.tarul.cn/Article/details/gzrwyoxtp.sHtML

[R23] 字符串替换
来源：http://baike.tarul.cn/Article/details/gedeaoicg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.sjlbkw.cn/Article/details/griixnxxm.sHtML

[R24] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gywdkmzwr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.yfazqb.com/Article/details/gggciskui.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.epnwcf.com/Article/details/gdrprfzvh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fktsv.cn/Article/details/geiizidbo.sHtML

[R26] 命令替换
来源：http://m.share.fktsv.cn/Article/details/gbxtgjxmw.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fktsv.cn/Article/details/gpsdhffvu.sHtML

[R27] 算术展开
来源：http://www.blog.vehdjk.com/Article/details/gjtleqbhb.sHtML

echo $((1 + 2 * 3))
来源：http://baike.vehdjk.com/Article/details/gpsujuyhs.sHtML

[R28] 浮点运算
来源：http://3g.bbcook.cn/Article/details/gqyekhepw.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/gqajpbnda.sHtML

[R29] 定义函数
来源：http://baike.vehdjk.com/Article/details/gxxfpywgp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.tarul.cn/Article/details/gypmnajfw.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/gqoewpurl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.sjlbkw.cn/Article/details/gapylyeiq.sHtML

[R31] 局部变量
来源：http://wap.tarul.cn/Article/details/gfsdxybqu.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.sjlbkw.cn/Article/details/ghlzjxyzf.sHtML

[R32] 参数个数校验
来源：http://3g.epnwcf.com/Article/details/ggcsaggdh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/grcefvthn.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.epnwcf.com/Article/details/gqgskxqum.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fktsv.cn/Article/details/gzxmaglhm.sHtML

[R34] 退出时清理
来源：http://blog.bbcook.cn/Article/details/gdwqurusj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/guesukfcq.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/gezhghxtn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.yfazqb.com/Article/details/gahdrntxw.sHtML

[R36] 并发执行多个任务
来源：http://wap.yfazqb.com/Article/details/getfvlqkq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.bbcook.cn/Article/details/gyvduaydr.sHtML

[R37] 把输出赋给变量
来源：http://baike.sjlbkw.cn/Article/details/gigvuwjrx.sHtML

files=$(ls -1)
来源：http://read.share.yfazqb.com/Article/details/gfezjcyph.sHtML

[R38] 管道串联
来源：http://3g.epnwcf.com/Article/details/giaatnclz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.tarul.cn/Article/details/gkvbdjhit.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.bbcook.cn/Article/details/gliykbfbw.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fktsv.cn/Article/details/gukwybgxu.sHtML

[R40] 追加写日志
来源：http://www.blog.sjlbkw.cn/Article/details/gxbwxrwba.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/gvocghdck.sHtML

[R41] 丢弃输出
来源：http://mobile.vehdjk.com/Article/details/ghqgfvkkd.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.bbcook.cn/Article/details/gfcvcwald.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gjosvygzq.sHtML

wc -l < a.txt
来源：http://blog.epnwcf.com/Article/details/gplwublqq.sHtML

[R43] 按名字查找文件
来源：http://m.share.vehdjk.com/Article/details/gcgwqctmg.sHtML

find . -name "*.log" -type f
来源：http://wap.tarul.cn/Article/details/gwikyjnin.sHtML

[R44] 按修改时间查找
来源：http://wap.sjlbkw.cn/Article/details/gurbfqqxs.sHtML

find . -mtime -7 -type f
来源：http://www.share.bbcook.cn/Article/details/gsrdwsgth.sHtML

[R45] 批量删除
来源：http://read.share.sjlbkw.cn/Article/details/gchuflvqc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/gsgouvkus.sHtML

[R46] 递归替换文件内容
来源：http://baike.bbcook.cn/Article/details/ghyyfrxwu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.sjlbkw.cn/Article/details/gbqvhkwop.sHtML

[R47] sed 单行替换
来源：http://mobile.sjlbkw.cn/Article/details/gatfujmnb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gorhnwfpm.sHtML

[R48] awk 取指定列
来源：http://mobile.sjlbkw.cn/Article/details/ghhwrwmpw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gowujkgzl.sHtML

[R49] awk 带条件
来源：http://baike.sjlbkw.cn/Article/details/grltloygf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/gozfgxods.sHtML

[R50] awk 求和
来源：http://read.share.sjlbkw.cn/Article/details/gfdvbxcdj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gtybelfbz.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/gyygyfhrv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.epnwcf.com/Article/details/gyshnihux.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/gyiytokqg.sHtML

wc -l a.txt
来源：http://blog.epnwcf.com/Article/details/genvwflco.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.tarul.cn/Article/details/gyenpmrvl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.tarul.cn/Article/details/gearwkhut.sHtML

[R54] 比较两个文件
来源：http://3g.tarul.cn/Article/details/gkskvztut.sHtML

diff a.txt b.txt
来源：http://www.share.yfazqb.com/Article/details/gbkeodfzl.sHtML

[R55] 压缩与解压
来源：http://www.share.epnwcf.com/Article/details/gvuravzaw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fktsv.cn/Article/details/gutguxvuy.sHtML

[R56] 远程拷贝
来源：http://www.share.bbcook.cn/Article/details/ggtrkiyxg.sHtML

scp file user@host:/path/
来源：http://3g.fktsv.cn/Article/details/gxnbhgspv.sHtML

[R57] 远程执行命令
来源：http://blog.vehdjk.com/Article/details/gmjxnbyoh.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.vehdjk.com/Article/details/gxnpadgve.sHtML

[R58] 下载文件
来源：http://mobile.yfazqb.com/Article/details/glvofngbp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.bbcook.cn/Article/details/ggphvbnwd.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/ghbpajbpi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.bbcook.cn/Article/details/ghfhfiero.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/geghgfatb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/gfmaaczqg.sHtML

[R61] 磁盘占用
来源：http://www.blog.epnwcf.com/Article/details/gwyfmslyq.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/gefwhsrpo.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/gjeqtecls.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fktsv.cn/Article/details/gowrvmfmi.sHtML

[R63] 内存与进程
来源：http://www.share.sjlbkw.cn/Article/details/gpluesabh.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fktsv.cn/Article/details/gwlllugzp.sHtML

[R64] 结束进程
来源：http://wap.sjlbkw.cn/Article/details/gnqcvcita.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.sjlbkw.cn/Article/details/geasmntho.sHtML

[R65] 查看端口占用
来源：http://3g.epnwcf.com/Article/details/gwrnilppz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.tarul.cn/Article/details/gouuntnzb.sHtML

[R66] 定时任务
来源：http://wap.tarul.cn/Article/details/gytsthmuj.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.vehdjk.com/Article/details/gudlhsmec.sHtML

[R67] 生成随机十六进制串
来源：http://baike.sjlbkw.cn/Article/details/gjnsrnbqb.sHtML

openssl rand -hex 16
来源：http://read.share.vehdjk.com/Article/details/gxolhkyfh.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgpwhulh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.vehdjk.com/Article/details/gdnvbodtn.sHtML

[R69] 生成随机密码
来源：http://www.blog.sjlbkw.cn/Article/details/gskphmtbh.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fktsv.cn/Article/details/gytykzjns.sHtML

[R70] 时间戳与互转
来源：http://www.blog.yfazqb.com/Article/details/ggepteohc.sHtML

date +%s;  date -d @1700000000
来源：http://blog.tarul.cn/Article/details/gksdyvybu.sHtML

[R71] 日期格式化
来源：http://wap.vehdjk.com/Article/details/gbujeglsd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.epnwcf.com/Article/details/geawzwvuj.sHtML

[R72] 等待端口就绪
来源：http://www.share.yfazqb.com/Article/details/gpkwbanlg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gllvywxqr.sHtML

[R73] 分割大日志
来源：http://mobile.sjlbkw.cn/Article/details/gtslttsjv.sHtML

split -l 1000 big.log part_
来源：http://www.share.bbcook.cn/Article/details/gapqnmiij.sHtML

[R74] 批量重命名
来源：http://read.share.yfazqb.com/Article/details/gneaubszt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyafsqoa.sHtML

[R75] 导出环境变量
来源：http://blog.bbcook.cn/Article/details/gpxknnpot.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.sjlbkw.cn/Article/details/grjurvlzv.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/geuzovgou.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gdgjzmphc.sHtML

[R77] 读取用户输入
来源：http://www.share.epnwcf.com/Article/details/gykpqmrkv.sHtML

read -rp "请输入: " ans
来源：http://3g.vehdjk.com/Article/details/gfrfxlnff.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/gjlnotqjf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fktsv.cn/Article/details/gtodahvgb.sHtML

[R79] 解析命令行选项
来源：http://www.share.sjlbkw.cn/Article/details/gyuhvfdqx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.yfazqb.com/Article/details/ggxddelsk.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.sjlbkw.cn/Article/details/gxpbsyigc.sHtML

time ./run.sh
来源：http://www.m.share.epnwcf.com/Article/details/gfcwycjbc.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gdxtwiqxl.sHtML

S. C / C++ 专题
来源：http://www.m.share.fktsv.cn/Article/details/gbtgrmsto.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqbtejyzv.sHtML

[S01] C：Hello World
来源：http://baike.fktsv.cn/Article/details/gxkmndjfy.sHtML

#include <stdio.h>
来源：http://baike.vehdjk.com/Article/details/gqxzqbsno.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fktsv.cn/Article/details/gbcmvhbjk.sHtML

[S02] C：变量与格式化输出
来源：http://baike.bbcook.cn/Article/details/geusjweqm.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.yfazqb.com/Article/details/gnjjdtmch.sHtML

[S03] C：读入整数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgxjtehe.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.epnwcf.com/Article/details/gfsrxoptx.sHtML

[S04] C：字符串复制
来源：http://read.share.vehdjk.com/Article/details/gxcxxasrl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/grxceetrz.sHtML

[S05] C：字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gpeyqcepw.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/gcgsmebca.sHtML

[S06] C：字符串比较
来源：http://read.share.fktsv.cn/Article/details/ghpzpmrmv.sHtML

strcmp(a, b) == 0
来源：http://read.share.yfazqb.com/Article/details/glsruvoqw.sHtML

[S07] C：数组遍历求和
来源：http://3g.bbcook.cn/Article/details/gzxhrfahm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.tarul.cn/Article/details/gytwyviqh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.tarul.cn/Article/details/gnadsgtyz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.sjlbkw.cn/Article/details/gvtwrowbf.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.vehdjk.com/Article/details/gqeuwdxxg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fktsv.cn/Article/details/goknpjlej.sHtML

[S10] C：指针与解引用
来源：http://baike.epnwcf.com/Article/details/guzehqvqo.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gxergsgzv.sHtML

[S11] C：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gzknzggkl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/gfqgoxptj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.bbcook.cn/Article/details/gfltmrgsz.sHtML

fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gywdmegrd.sHtML

[S12] C：写文件
来源：http://wap.epnwcf.com/Article/details/gtdymsojk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.yfazqb.com/Article/details/giaufrmwc.sHtML

[S13] C：宏定义
来源：http://baike.sjlbkw.cn/Article/details/grcxrdeyf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.epnwcf.com/Article/details/ghpxagohm.sHtML

[S14] C：枚举
来源：http://mobile.bbcook.cn/Article/details/gsvzvzllo.sHtML


<!-- 参考信息 -->