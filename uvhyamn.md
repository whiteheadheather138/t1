代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/ggmrrvgje.sHtML

[Q50] 批量更新
来源：http://www.blog.vehdjk.com/Article/details/gcryhhtyl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.epnwcf.com/Article/details/gdrbsyamk.sHtML

[Q51] 用子查询更新
来源：http://mobile.fktsv.cn/Article/details/gnsasbooq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gdgsmscrp.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/gyllwizbq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.epnwcf.com/Article/details/ggqvfhdun.sHtML

[Q53] 按条件删除
来源：http://www.m.share.tarul.cn/Article/details/glrcrsobn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.yfazqb.com/Article/details/gkjtnpnwp.sHtML

[Q54] 清空表
来源：http://m.share.vehdjk.com/Article/details/gptdsudcz.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fktsv.cn/Article/details/gveuhgvkb.sHtML

[Q55] 排名（并列占位）
来源：http://blog.epnwcf.com/Article/details/gtqhkywrd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gldriidhw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.tarul.cn/Article/details/gjouqcajb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.tarul.cn/Article/details/gbjlorgpo.sHtML

[Q57] 行号
来源：http://blog.sjlbkw.cn/Article/details/gdmgyijgx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.epnwcf.com/Article/details/gzonwxrji.sHtML

[Q58] 累计求和
来源：http://read.share.sjlbkw.cn/Article/details/gffklljpf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gpsqrvxxn.sHtML

[Q59] 分组内累计
来源：http://3g.yfazqb.com/Article/details/gflyiwxta.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gzaokienh.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.yfazqb.com/Article/details/gbkmhardc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.yfazqb.com/Article/details/gsvyqfzgq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gdrvhwzxd.sHtML

[Q61] 移动平均
来源：http://wap.tarul.cn/Article/details/gsafabkfu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/grrjimydy.sHtML

[Q62] 分组占比
来源：http://www.share.fktsv.cn/Article/details/gtbjbzhyx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gtjzwpkzs.sHtML

[Q63] 开启事务
来源：http://mobile.tarul.cn/Article/details/girlxweks.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.sjlbkw.cn/Article/details/gdxfqhkwr.sHtML

[Q64] 提交事务
来源：http://mobile.vehdjk.com/Article/details/gkuatyqeh.sHtML

COMMIT;
来源：http://read.share.bbcook.cn/Article/details/gscnqbpcz.sHtML

[Q65] 回滚事务
来源：http://www.share.yfazqb.com/Article/details/giqorsyna.sHtML

ROLLBACK;
来源：http://3g.fktsv.cn/Article/details/gsymgjefn.sHtML

[Q66] 行锁查询
来源：http://www.blog.epnwcf.com/Article/details/gimrijxxa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.yfazqb.com/Article/details/goyrfllbq.sHtML

[Q67] 设置隔离级别
来源：http://wap.tarul.cn/Article/details/gidhqvgsn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.vehdjk.com/Article/details/gqhhemjrz.sHtML

[Q68] 保存点
来源：http://baike.bbcook.cn/Article/details/gqvmsknqz.sHtML

SAVEPOINT sp1;
来源：http://m.share.yfazqb.com/Article/details/gmxpyivxv.sHtML

ROLLBACK TO sp1;
来源：http://3g.sjlbkw.cn/Article/details/geaipzonn.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/grddgwfys.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.sjlbkw.cn/Article/details/gztgwkkqf.sHtML

[Q70] 更新统计信息
来源：http://read.share.sjlbkw.cn/Article/details/gfiwijnvo.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/gxjngonoe.sHtML

[Q71] 查看建表语句
来源：http://mobile.tarul.cn/Article/details/gmohqduzb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.epnwcf.com/Article/details/gznqxdokc.sHtML

[Q72] 查看索引
来源：http://www.share.tarul.cn/Article/details/gxypjihmk.sHtML

SHOW INDEX FROM users;
来源：http://m.share.bbcook.cn/Article/details/gwnwtmatk.sHtML

[Q73] 查看表状态
来源：http://read.share.bbcook.cn/Article/details/gvyzervgn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.epnwcf.com/Article/details/gnqujvybo.sHtML

[Q74] 强制使用索引
来源：http://read.share.bbcook.cn/Article/details/gjoskexba.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.bbcook.cn/Article/details/gkwmlobzk.sHtML

[Q75] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gzhjubpog.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.tarul.cn/Article/details/gvmhurmdy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.bbcook.cn/Article/details/gwknioztn.sHtML

[Q76] 按天统计
来源：http://www.blog.fktsv.cn/Article/details/gjzshxxpt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.tarul.cn/Article/details/grlnqrppo.sHtML

[Q77] 时间加减
来源：http://www.share.bbcook.cn/Article/details/gxuhrlqxy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.vehdjk.com/Article/details/gyrfpeuwv.sHtML

[Q78] 当前时间
来源：http://m.share.sjlbkw.cn/Article/details/gjsdvldee.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.tarul.cn/Article/details/ggpnsnacm.sHtML

[Q79] 字符串拼接
来源：http://baike.bbcook.cn/Article/details/gwfclimiw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.epnwcf.com/Article/details/glkmgmzps.sHtML

[Q80] 字符串截取
来源：http://mobile.bbcook.cn/Article/details/gxlrfsvgi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gwcigcyts.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gwxgnwzfn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.tarul.cn/Article/details/gcdnagyzx.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.bbcook.cn/Article/details/gbccfoemv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gigsslswt.sHtML

[Q83] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/goftnhydw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/geukijbps.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/ghyqzccbb.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gskbnnqey.sHtML

[Q85] 数值取整
来源：http://read.share.fktsv.cn/Article/details/gtjcugcsy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.bbcook.cn/Article/details/givctxwyr.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.epnwcf.com/Article/details/gwcvtapcd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.sjlbkw.cn/Article/details/gfubdqhlo.sHtML

[Q87] JSON 字段做条件
来源：http://baike.vehdjk.com/Article/details/gwuuhxtbm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.epnwcf.com/Article/details/gkftnmxyp.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.bbcook.cn/Article/details/gckbrzono.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.vehdjk.com/Article/details/gaxnxqfet.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.vehdjk.com/Article/details/gzatqpdqm.sHtML

[Q89] 判断表是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gmmvsiwte.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.bbcook.cn/Article/details/gvsbnazmh.sHtML

[Q90] 生成序号列
来源：http://www.m.share.bbcook.cn/Article/details/goqkfhkwx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.tarul.cn/Article/details/gvkskipbr.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gogzytmtb.sHtML

R. Bash 专题
来源：http://m.share.tarul.cn/Article/details/gsakpakex.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/grcaaewsf.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gsyhwxfue.sHtML

#!/usr/bin/env bash
来源：http://baike.sjlbkw.cn/Article/details/galeuqarq.sHtML

set -euo pipefail
来源：http://www.share.tarul.cn/Article/details/gkmcjdnmi.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.tarul.cn/Article/details/gcquamlbq.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.tarul.cn/Article/details/gcngnohgn.sHtML

[R03] 只读变量
来源：http://www.blog.vehdjk.com/Article/details/gfozbgozv.sHtML

readonly PI=3.14
来源：http://wap.sjlbkw.cn/Article/details/gezhgfoxr.sHtML

[R04] 位置参数
来源：http://wap.sjlbkw.cn/Article/details/genfhftbs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.epnwcf.com/Article/details/ggfhpdmkd.sHtML

[R05] 参数默认值
来源：http://blog.yfazqb.com/Article/details/gkdgxqaez.sHtML

name="${1:-default}"
来源：http://blog.bbcook.cn/Article/details/gruhtedgc.sHtML

[R06] 判断命令是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gdcovpdfn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/ghsmexifx.sHtML

[R07] if 判断文件
来源：http://mobile.epnwcf.com/Article/details/gsqtnqnvm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gkdkrqprg.sHtML

[R08] 数值比较
来源：http://read.share.epnwcf.com/Article/details/gkyuelgsn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.yfazqb.com/Article/details/ghmoyyzfe.sHtML

[R09] 字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gyxbpjjpr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.tarul.cn/Article/details/ghtlipctr.sHtML

[R10] 正则匹配
来源：http://m.share.fktsv.cn/Article/details/gyhnshqnj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fktsv.cn/Article/details/grywunbwt.sHtML

[R11] case 多分支
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpcfjmys.sHtML

case "$1" in
来源：http://www.blog.yfazqb.com/Article/details/ghwqquwoj.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gxlknbdnt.sHtML

stop)  echo "停止" ;;
来源：http://blog.fktsv.cn/Article/details/gnkwdkayr.sHtML

*)     echo "未知命令" ;;
来源：http://blog.tarul.cn/Article/details/gawpvrvij.sHtML

esac
来源：http://baike.bbcook.cn/Article/details/goofzgulx.sHtML

[R12] for 遍历文件
来源：http://baike.fktsv.cn/Article/details/gpftoxxgb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gnocdqyne.sHtML

[R13] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gyejwludv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/giisnxuiw.sHtML

[R14] C 风格 for
来源：http://m.share.fktsv.cn/Article/details/gcgbalnnf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/gnvsfitkk.sHtML

[R15] while 逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gzwzxmykt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.yfazqb.com/Article/details/gejrfhbyd.sHtML

[R16] until 等待条件
来源：http://blog.epnwcf.com/Article/details/gqszowyee.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/gpnqzoswj.sHtML

[R17] 数组定义与取值
来源：http://mobile.bbcook.cn/Article/details/ggbhyusnl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fktsv.cn/Article/details/gtcbkhczc.sHtML

[R18] 遍历数组
来源：http://baike.bbcook.cn/Article/details/gyjkfunrs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.tarul.cn/Article/details/gsjodbcsd.sHtML

[R19] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/gflhovqas.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.epnwcf.com/Article/details/gvhmneqll.sHtML

[R20] 关联数组（字典）
来源：http://3g.yfazqb.com/Article/details/gifujrjps.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.tarul.cn/Article/details/gusbujnvn.sHtML

[R21] 字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/ghsiqbomu.sHtML

echo "${#s}"
来源：http://mobile.yfazqb.com/Article/details/glohmrkak.sHtML

[R22] 截取子串
来源：http://baike.vehdjk.com/Article/details/gxwlyboli.sHtML

echo "${s:0:5}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnakcwmk.sHtML

[R23] 字符串替换
来源：http://blog.bbcook.cn/Article/details/grzsawjlt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fktsv.cn/Article/details/gegmkaedd.sHtML

[R24] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gfhvnteue.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.bbcook.cn/Article/details/gkqeyfujn.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.bbcook.cn/Article/details/gntjfwvdf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fktsv.cn/Article/details/grgewvwvl.sHtML

[R26] 命令替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvrkdwva.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.bbcook.cn/Article/details/gqfnvyqor.sHtML

[R27] 算术展开
来源：http://baike.sjlbkw.cn/Article/details/gytsipfyv.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.bbcook.cn/Article/details/gbluelhvi.sHtML

[R28] 浮点运算
来源：http://blog.epnwcf.com/Article/details/gixtktwym.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/gahgxvgjw.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gdyrmewkk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.bbcook.cn/Article/details/gcdvebtfp.sHtML

[R30] 函数返回状态码
来源：http://www.share.epnwcf.com/Article/details/gxzfnqttv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.bbcook.cn/Article/details/gmzdinfli.sHtML

[R31] 局部变量
来源：http://mobile.bbcook.cn/Article/details/ggtdgmoex.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fktsv.cn/Article/details/glgsskcyg.sHtML

[R32] 参数个数校验
来源：http://blog.bbcook.cn/Article/details/gimthlvzl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/gulwsugee.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.vehdjk.com/Article/details/grzviqvcq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.vehdjk.com/Article/details/gngxxrehx.sHtML

[R34] 退出时清理
来源：http://www.share.yfazqb.com/Article/details/gkozogfut.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/gxszdpkoc.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/gkxmjqcsr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fktsv.cn/Article/details/gnpqqyvwb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.epnwcf.com/Article/details/gphmdnpzv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/givyaspkr.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.epnwcf.com/Article/details/gtwkoxtcm.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/gglusqgxh.sHtML

[R38] 管道串联
来源：http://baike.bbcook.cn/Article/details/guehnbzbv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.bbcook.cn/Article/details/grcpkuwdv.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.epnwcf.com/Article/details/gizrgnvhw.sHtML

cmd > out.log 2>&1
来源：http://mobile.epnwcf.com/Article/details/gdgwdzjmy.sHtML

[R40] 追加写日志
来源：http://m.share.yfazqb.com/Article/details/gouygqmkj.sHtML

echo "log" >> out.log
来源：http://baike.tarul.cn/Article/details/gxucsejbg.sHtML

[R41] 丢弃输出
来源：http://read.share.vehdjk.com/Article/details/ggauoeaow.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.vehdjk.com/Article/details/glxgakwvk.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/ghpgzdnwr.sHtML

wc -l < a.txt
来源：http://read.share.tarul.cn/Article/details/grauonqih.sHtML

[R43] 按名字查找文件
来源：http://m.share.sjlbkw.cn/Article/details/gdrrzxmtb.sHtML

find . -name "*.log" -type f
来源：http://m.share.tarul.cn/Article/details/gdahwkhsf.sHtML

[R44] 按修改时间查找
来源：http://wap.fktsv.cn/Article/details/gkzhpenwn.sHtML

find . -mtime -7 -type f
来源：http://wap.fktsv.cn/Article/details/gtasemetf.sHtML

[R45] 批量删除
来源：http://blog.bbcook.cn/Article/details/goncupkjq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fktsv.cn/Article/details/ggrttggyh.sHtML

[R46] 递归替换文件内容
来源：http://read.share.tarul.cn/Article/details/gucnbprjf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.bbcook.cn/Article/details/glyrrlrlp.sHtML

[R47] sed 单行替换
来源：http://m.share.tarul.cn/Article/details/ghxkbxiaa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/gmnwdfwzc.sHtML

[R48] awk 取指定列
来源：http://baike.epnwcf.com/Article/details/goqppxpwq.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.yfazqb.com/Article/details/ggmkxzxex.sHtML

[R49] awk 带条件
来源：http://m.share.bbcook.cn/Article/details/gfydduxyp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.yfazqb.com/Article/details/glmhbuxrb.sHtML

[R50] awk 求和
来源：http://blog.vehdjk.com/Article/details/gpedbrxll.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gdcugkijq.sHtML

[R51] 排序去重取前几
来源：http://blog.vehdjk.com/Article/details/gmfuffzdk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.epnwcf.com/Article/details/ggxhsiklq.sHtML

[R52] 统计行数
来源：http://baike.tarul.cn/Article/details/gybkzpshv.sHtML

wc -l a.txt
来源：http://read.share.tarul.cn/Article/details/gytrckpqd.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/gqrbyfbrc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.vehdjk.com/Article/details/gewymteeq.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/gjqbjohjs.sHtML

diff a.txt b.txt
来源：http://www.blog.bbcook.cn/Article/details/gddxpufjz.sHtML

[R55] 压缩与解压
来源：http://read.share.yfazqb.com/Article/details/gvcdsnmzv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/grlrswaqm.sHtML

[R56] 远程拷贝
来源：http://read.share.epnwcf.com/Article/details/gtrzbrrma.sHtML

scp file user@host:/path/
来源：http://www.share.fktsv.cn/Article/details/glisrrodk.sHtML

[R57] 远程执行命令
来源：http://www.share.yfazqb.com/Article/details/gzlhgcfsh.sHtML

ssh user@host 'uptime'
来源：http://3g.yfazqb.com/Article/details/gteimbexk.sHtML

[R58] 下载文件
来源：http://baike.tarul.cn/Article/details/gceqnumjo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/gqmfpdyrg.sHtML

[R59] 发 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gyeprgwie.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.bbcook.cn/Article/details/grssvnczi.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gbfskqnvb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.yfazqb.com/Article/details/gkiwfnnnb.sHtML

[R61] 磁盘占用
来源：http://m.share.vehdjk.com/Article/details/gfzpywina.sHtML

df -h;  du -sh *
来源：http://blog.vehdjk.com/Article/details/gaeihfayo.sHtML

[R62] 找最占空间的文件
来源：http://baike.fktsv.cn/Article/details/gvfjwzugj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.vehdjk.com/Article/details/gvjmhoqzn.sHtML

[R63] 内存与进程
来源：http://mobile.tarul.cn/Article/details/gkpqnbyzw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.epnwcf.com/Article/details/ghsntbhdm.sHtML

[R64] 结束进程
来源：http://3g.tarul.cn/Article/details/gwvkqifth.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.tarul.cn/Article/details/gaczxesgy.sHtML

[R65] 查看端口占用
来源：http://blog.yfazqb.com/Article/details/gezxaiqvp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.sjlbkw.cn/Article/details/gfyhbxmzt.sHtML

[R66] 定时任务
来源：http://www.blog.fktsv.cn/Article/details/gpassvpss.sHtML

crontab -e;  crontab -l
来源：http://www.blog.tarul.cn/Article/details/ghudlbstv.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/ghjlwrhyu.sHtML

openssl rand -hex 16
来源：http://www.share.tarul.cn/Article/details/gtbfffled.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.yfazqb.com/Article/details/gfrzfkcig.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.epnwcf.com/Article/details/gtpvxilhc.sHtML

[R69] 生成随机密码
来源：http://www.m.share.yfazqb.com/Article/details/gugthxden.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fktsv.cn/Article/details/gemcjcvqj.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.vehdjk.com/Article/details/gceqtaifv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/ggqrlsacf.sHtML

[R71] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gxdirgiye.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.sjlbkw.cn/Article/details/gepivddof.sHtML

[R72] 等待端口就绪
来源：http://3g.sjlbkw.cn/Article/details/gmtlddyke.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/glygvhzsc.sHtML

[R73] 分割大日志
来源：http://mobile.sjlbkw.cn/Article/details/gbjaldldg.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.vehdjk.com/Article/details/glatbtdzc.sHtML

[R74] 批量重命名
来源：http://www.m.share.yfazqb.com/Article/details/gndvpsojb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/gxvlvdtgn.sHtML

[R75] 导出环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gvvckrhvw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.bbcook.cn/Article/details/gbobtmdto.sHtML

[R76] 使用临时文件
来源：http://wap.bbcook.cn/Article/details/gfixbmkmy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gjgjdcvwj.sHtML

[R77] 读取用户输入
来源：http://www.share.epnwcf.com/Article/details/gckhzssgl.sHtML

read -rp "请输入: " ans
来源：http://wap.tarul.cn/Article/details/gtfjvxvdk.sHtML

[R78] 交互式菜单
来源：http://www.share.tarul.cn/Article/details/gphphhiky.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.yfazqb.com/Article/details/gjkvdhkeu.sHtML

[R79] 解析命令行选项
来源：http://m.share.bbcook.cn/Article/details/gehwffeog.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.vehdjk.com/Article/details/gkdlfksdn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.sjlbkw.cn/Article/details/gksghztpm.sHtML

time ./run.sh
来源：http://blog.yfazqb.com/Article/details/ghjdyhmam.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/geciwqhji.sHtML

S. C / C++ 专题
来源：http://m.share.yfazqb.com/Article/details/ghrpebafd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfzsbyvup.sHtML

[S01] C：Hello World
来源：http://3g.vehdjk.com/Article/details/ghhyekodl.sHtML

#include <stdio.h>
来源：http://www.blog.fktsv.cn/Article/details/gvdyylzby.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.epnwcf.com/Article/details/gxalqljqd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.epnwcf.com/Article/details/griewolki.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gzkcnhxhn.sHtML

[S03] C：读入整数
来源：http://blog.fktsv.cn/Article/details/gkvgcmlou.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gvgybhreh.sHtML

[S04] C：字符串复制
来源：http://wap.yfazqb.com/Article/details/gtsyvaopv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/gjbeejipo.sHtML

[S05] C：字符串长度
来源：http://blog.bbcook.cn/Article/details/gxpjnrfvr.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/gditytlrq.sHtML

[S06] C：字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gwefkubtv.sHtML

strcmp(a, b) == 0
来源：http://baike.vehdjk.com/Article/details/gqxxujefr.sHtML

[S07] C：数组遍历求和
来源：http://3g.epnwcf.com/Article/details/gasrdsvne.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/goupdvcnn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.yfazqb.com/Article/details/gjpfaduga.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.bbcook.cn/Article/details/gobxqdama.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.vehdjk.com/Article/details/gcebyhlmq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.vehdjk.com/Article/details/gitxpmsmz.sHtML

[S10] C：指针与解引用
来源：http://www.blog.sjlbkw.cn/Article/details/ghvcdjmyr.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.bbcook.cn/Article/details/gvhswcnhe.sHtML

[S11] C：逐行读文件
来源：http://read.share.tarul.cn/Article/details/goitwmcat.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.tarul.cn/Article/details/gwgcynuba.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.vehdjk.com/Article/details/gqljexjfq.sHtML

fclose(f);
来源：http://blog.bbcook.cn/Article/details/grjsnytmq.sHtML

[S12] C：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gijjkbqji.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gmqyvwguf.sHtML

[S13] C：宏定义
来源：http://3g.tarul.cn/Article/details/gddrufrxr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.epnwcf.com/Article/details/guqivyayy.sHtML

[S14] C：枚举
来源：http://3g.sjlbkw.cn/Article/details/gtexcxbdx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.bbcook.cn/Article/details/gfqwrjpmr.sHtML

[S15] C：类型转换
来源：http://baike.bbcook.cn/Article/details/gatntahyu.sHtML

(double) a / b
来源：http://mobile.fktsv.cn/Article/details/gmirnfnaq.sHtML

[S16] C：位操作置位
来源：http://3g.epnwcf.com/Article/details/gusjmtzrc.sHtML

x |= (1 << 3);
来源：http://wap.bbcook.cn/Article/details/gluxxastg.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.tarul.cn/Article/details/geoexxwbe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.bbcook.cn/Article/details/gxalrlqpl.sHtML

[S18] C：命令行参数
来源：http://mobile.fktsv.cn/Article/details/ggsoysoiu.sHtML

int main(int argc, char **argv)
来源：http://read.share.vehdjk.com/Article/details/gznmqguax.sHtML

[S19] C：快速排序
来源：http://www.m.share.sjlbkw.cn/Article/details/goiiafwus.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gymfflhfg.sHtML

[S20] C：二分查找
来源：http://baike.sjlbkw.cn/Article/details/gnmqyyqvi.sHtML


<!-- 参考信息 -->