代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.bbcook.cn/Article/details/gkcmufbju.sHtML

[Q52] 删除指定行
来源：http://m.share.sjlbkw.cn/Article/details/gjmhadaub.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.yfazqb.com/Article/details/gryvgsyps.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/gxkoninuj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/gezvweixk.sHtML

[Q54] 清空表
来源：http://baike.bbcook.cn/Article/details/gddvmqrrp.sHtML

TRUNCATE TABLE logs;
来源：http://wap.yfazqb.com/Article/details/gyxyldbok.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/gspkmkpov.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.sjlbkw.cn/Article/details/gbgdaojsm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/gvzcnueiu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.bbcook.cn/Article/details/gwtfpnhao.sHtML

[Q57] 行号
来源：http://m.share.yfazqb.com/Article/details/gqhwhnhpc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.epnwcf.com/Article/details/gtofmfdqu.sHtML

[Q58] 累计求和
来源：http://www.blog.bbcook.cn/Article/details/gzpycpzoi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.yfazqb.com/Article/details/gxzngrkex.sHtML

[Q59] 分组内累计
来源：http://wap.bbcook.cn/Article/details/gcofehvjb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gcffxfoqu.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.epnwcf.com/Article/details/gyazbjfuy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.epnwcf.com/Article/details/gjbjxruby.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gysqiyrsh.sHtML

[Q61] 移动平均
来源：http://www.m.share.tarul.cn/Article/details/gprshgwpj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gunrxfgqm.sHtML

[Q62] 分组占比
来源：http://www.share.bbcook.cn/Article/details/goobyxfhp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gakdincxs.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/gfqaqpufu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.bbcook.cn/Article/details/gyxiwbeyo.sHtML

[Q64] 提交事务
来源：http://www.blog.sjlbkw.cn/Article/details/gqjtvsxxn.sHtML

COMMIT;
来源：http://blog.vehdjk.com/Article/details/gynvxbzak.sHtML

[Q65] 回滚事务
来源：http://mobile.fktsv.cn/Article/details/gquczfikf.sHtML

ROLLBACK;
来源：http://blog.bbcook.cn/Article/details/gslerjyjt.sHtML

[Q66] 行锁查询
来源：http://3g.sjlbkw.cn/Article/details/gdvrfqzac.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.sjlbkw.cn/Article/details/glpixleun.sHtML

[Q67] 设置隔离级别
来源：http://m.share.epnwcf.com/Article/details/gqaemuqiu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.sjlbkw.cn/Article/details/gwrnxgfxy.sHtML

[Q68] 保存点
来源：http://www.m.share.yfazqb.com/Article/details/gefxtdjhn.sHtML

SAVEPOINT sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gnwqwivph.sHtML

ROLLBACK TO sp1;
来源：http://baike.vehdjk.com/Article/details/gxuuoxivv.sHtML

[Q69] 查看执行计划
来源：http://www.share.epnwcf.com/Article/details/gkrhdzbzg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fktsv.cn/Article/details/gisjbzmmw.sHtML

[Q70] 更新统计信息
来源：http://blog.epnwcf.com/Article/details/gvwnyknzo.sHtML

ANALYZE TABLE users;
来源：http://wap.fktsv.cn/Article/details/gfmnyvxwy.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrefqpbl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.yfazqb.com/Article/details/gsslljeba.sHtML

[Q72] 查看索引
来源：http://wap.fktsv.cn/Article/details/gbzyfipis.sHtML

SHOW INDEX FROM users;
来源：http://blog.vehdjk.com/Article/details/gdbczbhjy.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/gwermjixo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.tarul.cn/Article/details/gkjwexvva.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.yfazqb.com/Article/details/gjsnbgpfl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.epnwcf.com/Article/details/gjpuiybsr.sHtML

[Q75] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gxtkmtiap.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gdubhvwgf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fktsv.cn/Article/details/gwjbscfoo.sHtML

[Q76] 按天统计
来源：http://mobile.bbcook.cn/Article/details/gjgsndqpw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/gdkyncooz.sHtML

[Q77] 时间加减
来源：http://www.blog.sjlbkw.cn/Article/details/gcfmormii.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.epnwcf.com/Article/details/gvfdvwici.sHtML

[Q78] 当前时间
来源：http://blog.sjlbkw.cn/Article/details/gnbyaysti.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.tarul.cn/Article/details/gyeoorbcr.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gqjcuqkxu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.sjlbkw.cn/Article/details/gslfcgfwz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.bbcook.cn/Article/details/groxiiqyk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gsonjfxvy.sHtML

[Q81] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/gcykqcvxo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.epnwcf.com/Article/details/ganhxagff.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.yfazqb.com/Article/details/gkbfhwrwm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gkwoixvbq.sHtML

[Q83] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gfhjddtmx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gpmmaofaw.sHtML

[Q84] 去除首尾空格
来源：http://3g.bbcook.cn/Article/details/gckiedltr.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/guhszyljb.sHtML

[Q85] 数值取整
来源：http://www.share.sjlbkw.cn/Article/details/geikgkusm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.yfazqb.com/Article/details/glsbixete.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.sjlbkw.cn/Article/details/gsrdbeekt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.sjlbkw.cn/Article/details/gabprdiuu.sHtML

[Q87] JSON 字段做条件
来源：http://wap.sjlbkw.cn/Article/details/gurziaesr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.bbcook.cn/Article/details/gjidxfpkr.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.sjlbkw.cn/Article/details/goiccjpph.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fktsv.cn/Article/details/gbozffxxa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.vehdjk.com/Article/details/gxfawjfxk.sHtML

[Q89] 判断表是否存在
来源：http://blog.bbcook.cn/Article/details/gnkaitrrx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.vehdjk.com/Article/details/gdzfmzoyv.sHtML

[Q90] 生成序号列
来源：http://baike.vehdjk.com/Article/details/gbhevdmrg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.vehdjk.com/Article/details/gffpxrftz.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gdhgiuoxl.sHtML

R. Bash 专题
来源：http://read.share.sjlbkw.cn/Article/details/gvydnkbao.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtbdbaehh.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.sjlbkw.cn/Article/details/gbylklvsv.sHtML

#!/usr/bin/env bash
来源：http://3g.fktsv.cn/Article/details/gqorekjju.sHtML

set -euo pipefail
来源：http://read.share.bbcook.cn/Article/details/gdumrrxou.sHtML

[R02] 变量赋值与使用
来源：http://3g.yfazqb.com/Article/details/grnvexbhb.sHtML

name="Tom"; echo "$name"
来源：http://baike.sjlbkw.cn/Article/details/glweahiyb.sHtML

[R03] 只读变量
来源：http://blog.vehdjk.com/Article/details/ghqtagvji.sHtML

readonly PI=3.14
来源：http://baike.tarul.cn/Article/details/govgasyxn.sHtML

[R04] 位置参数
来源：http://3g.bbcook.cn/Article/details/gevewrvqa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.tarul.cn/Article/details/ghuabzsng.sHtML

[R05] 参数默认值
来源：http://baike.yfazqb.com/Article/details/gjnfpfgxj.sHtML

name="${1:-default}"
来源：http://www.blog.vehdjk.com/Article/details/gbviberjk.sHtML

[R06] 判断命令是否存在
来源：http://baike.vehdjk.com/Article/details/gfrfvveoy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvqnodekp.sHtML

[R07] if 判断文件
来源：http://3g.epnwcf.com/Article/details/gidynwzjk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.vehdjk.com/Article/details/gkmjaebjp.sHtML

[R08] 数值比较
来源：http://m.share.yfazqb.com/Article/details/guzqlxmts.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.yfazqb.com/Article/details/gobdwssgm.sHtML

[R09] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gextvenum.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.yfazqb.com/Article/details/gaytvsrbs.sHtML

[R10] 正则匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gdcgrgiqn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.vehdjk.com/Article/details/gymfwoqfw.sHtML

[R11] case 多分支
来源：http://3g.sjlbkw.cn/Article/details/ganometnm.sHtML

case "$1" in
来源：http://wap.sjlbkw.cn/Article/details/guwpafmbo.sHtML

start) echo "启动" ;;
来源：http://3g.yfazqb.com/Article/details/gvhbqrmbv.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fktsv.cn/Article/details/ghqyqvrtk.sHtML

*)     echo "未知命令" ;;
来源：http://blog.tarul.cn/Article/details/gfpzdohuh.sHtML

esac
来源：http://blog.epnwcf.com/Article/details/gihdkaoto.sHtML

[R12] for 遍历文件
来源：http://wap.bbcook.cn/Article/details/gymjvzjkv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.yfazqb.com/Article/details/gtmxrvcvw.sHtML

[R13] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/gwuvgcxih.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gzdepfvhz.sHtML

[R14] C 风格 for
来源：http://mobile.sjlbkw.cn/Article/details/gkajhsyat.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gppimuydh.sHtML

[R15] while 逐行读文件
来源：http://baike.vehdjk.com/Article/details/gmblfmkcv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.tarul.cn/Article/details/giuayuhsy.sHtML

[R16] until 等待条件
来源：http://3g.bbcook.cn/Article/details/gzukwywcd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gujmrgliy.sHtML

[R17] 数组定义与取值
来源：http://baike.bbcook.cn/Article/details/gqagbruag.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.sjlbkw.cn/Article/details/gakvdwbpi.sHtML

[R18] 遍历数组
来源：http://www.share.yfazqb.com/Article/details/gzzzlbago.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.vehdjk.com/Article/details/gbjiqtljm.sHtML

[R19] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gbzfegzop.sHtML

echo "${#arr[@]}"
来源：http://baike.tarul.cn/Article/details/gwobfpirn.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fktsv.cn/Article/details/gwpahcxwq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.vehdjk.com/Article/details/gdmuqmjxx.sHtML

[R21] 字符串长度
来源：http://blog.tarul.cn/Article/details/gmfiduoit.sHtML

echo "${#s}"
来源：http://read.share.vehdjk.com/Article/details/gzecqtdwu.sHtML

[R22] 截取子串
来源：http://wap.tarul.cn/Article/details/ghhjuzfyr.sHtML

echo "${s:0:5}"
来源：http://blog.fktsv.cn/Article/details/gzzzueubq.sHtML

[R23] 字符串替换
来源：http://blog.fktsv.cn/Article/details/gnncgaqcg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.tarul.cn/Article/details/gobicuzsc.sHtML

[R24] 大小写转换
来源：http://wap.fktsv.cn/Article/details/glockvpzc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.vehdjk.com/Article/details/gievgitnh.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.tarul.cn/Article/details/gxetyhzlu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/gkxhpells.sHtML

[R26] 命令替换
来源：http://www.m.share.epnwcf.com/Article/details/golukysac.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.bbcook.cn/Article/details/gunkfygpb.sHtML

[R27] 算术展开
来源：http://baike.epnwcf.com/Article/details/godrjiifw.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.sjlbkw.cn/Article/details/gqzpwvxaf.sHtML

[R28] 浮点运算
来源：http://baike.vehdjk.com/Article/details/gfppjwvqa.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.bbcook.cn/Article/details/gaxgqfhmg.sHtML

[R29] 定义函数
来源：http://wap.yfazqb.com/Article/details/gclpfsxsy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgmprfrk.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fktsv.cn/Article/details/gdwwkapst.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.sjlbkw.cn/Article/details/gztjuwerq.sHtML

[R31] 局部变量
来源：http://wap.epnwcf.com/Article/details/gojbvvdxa.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.yfazqb.com/Article/details/gjpipckyr.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/gtbltsiui.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gfufmiqra.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.tarul.cn/Article/details/gqahsulux.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.epnwcf.com/Article/details/gpkuiyjlu.sHtML

[R34] 退出时清理
来源：http://read.share.bbcook.cn/Article/details/gzjrpmcor.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gsplvxiqs.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/gexovdjoy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.bbcook.cn/Article/details/gqptjgbmk.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fktsv.cn/Article/details/galrvhdui.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/gksjnexts.sHtML

[R37] 把输出赋给变量
来源：http://mobile.epnwcf.com/Article/details/gzhutkknk.sHtML

files=$(ls -1)
来源：http://3g.fktsv.cn/Article/details/gczcntzyf.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/gsaglluno.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.epnwcf.com/Article/details/grqooytct.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.yfazqb.com/Article/details/gzqzsfldn.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/gfoqpcmac.sHtML

[R40] 追加写日志
来源：http://3g.tarul.cn/Article/details/gnkhfibww.sHtML

echo "log" >> out.log
来源：http://mobile.vehdjk.com/Article/details/gxitlminc.sHtML

[R41] 丢弃输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxhhlawo.sHtML

cmd >/dev/null 2>&1
来源：http://blog.bbcook.cn/Article/details/gqumhddio.sHtML

[R42] 输入重定向
来源：http://www.share.sjlbkw.cn/Article/details/ghpxqavby.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/gevawjoxp.sHtML

[R43] 按名字查找文件
来源：http://www.share.tarul.cn/Article/details/gkrtfwqid.sHtML

find . -name "*.log" -type f
来源：http://baike.fktsv.cn/Article/details/gforfjetu.sHtML

[R44] 按修改时间查找
来源：http://wap.vehdjk.com/Article/details/gnwygsydj.sHtML

find . -mtime -7 -type f
来源：http://read.share.tarul.cn/Article/details/gunyzxcsn.sHtML

[R45] 批量删除
来源：http://baike.tarul.cn/Article/details/gbtteaxuo.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.epnwcf.com/Article/details/gbkqxjiwm.sHtML

[R46] 递归替换文件内容
来源：http://3g.fktsv.cn/Article/details/gwtjhemsa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.epnwcf.com/Article/details/grhnumxck.sHtML

[R47] sed 单行替换
来源：http://www.blog.epnwcf.com/Article/details/gbnkbnmnh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.bbcook.cn/Article/details/gshznbiis.sHtML

[R48] awk 取指定列
来源：http://mobile.yfazqb.com/Article/details/gcbgaztft.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gcbijjsgy.sHtML

[R49] awk 带条件
来源：http://mobile.tarul.cn/Article/details/gdyeplevr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fktsv.cn/Article/details/giimmitlk.sHtML

[R50] awk 求和
来源：http://m.share.sjlbkw.cn/Article/details/gnitmmeik.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.bbcook.cn/Article/details/gjigxepnz.sHtML

[R51] 排序去重取前几
来源：http://read.share.vehdjk.com/Article/details/gjoqrjewd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.vehdjk.com/Article/details/gktllyqbv.sHtML

[R52] 统计行数
来源：http://blog.yfazqb.com/Article/details/govxfxfrl.sHtML

wc -l a.txt
来源：http://mobile.vehdjk.com/Article/details/gqjttfxle.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.yfazqb.com/Article/details/gznmvwgdg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/gbknzelmx.sHtML

[R54] 比较两个文件
来源：http://www.share.bbcook.cn/Article/details/gitaavzqr.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/grdmhzipl.sHtML

[R55] 压缩与解压
来源：http://www.m.share.yfazqb.com/Article/details/golpcwoib.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.bbcook.cn/Article/details/gquuibsuy.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/gggrpmpqq.sHtML

scp file user@host:/path/
来源：http://read.share.sjlbkw.cn/Article/details/gaxidvdqn.sHtML

[R57] 远程执行命令
来源：http://mobile.bbcook.cn/Article/details/gisfiyhpp.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gtxatddqe.sHtML

[R58] 下载文件
来源：http://3g.epnwcf.com/Article/details/gqcjgeypz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.sjlbkw.cn/Article/details/gbijnyagc.sHtML

[R59] 发 POST JSON
来源：http://www.share.bbcook.cn/Article/details/gvvnltprz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.epnwcf.com/Article/details/gpvgmgjbw.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/glpastsus.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.sjlbkw.cn/Article/details/gtnepvmrk.sHtML

[R61] 磁盘占用
来源：http://3g.vehdjk.com/Article/details/guayjfjbp.sHtML

df -h;  du -sh *
来源：http://read.share.fktsv.cn/Article/details/gvfpcigym.sHtML

[R62] 找最占空间的文件
来源：http://baike.fktsv.cn/Article/details/gtektaxxl.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.epnwcf.com/Article/details/gwvnqsmdv.sHtML

[R63] 内存与进程
来源：http://wap.bbcook.cn/Article/details/gqhwdbyrd.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.epnwcf.com/Article/details/gfupfdjph.sHtML

[R64] 结束进程
来源：http://www.share.fktsv.cn/Article/details/gbgppzpzn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fktsv.cn/Article/details/gjjtahxbl.sHtML

[R65] 查看端口占用
来源：http://www.share.fktsv.cn/Article/details/ghjjbcsaa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.sjlbkw.cn/Article/details/gqbkgwzsa.sHtML

[R66] 定时任务
来源：http://read.share.vehdjk.com/Article/details/ginbndilw.sHtML

crontab -e;  crontab -l
来源：http://mobile.sjlbkw.cn/Article/details/gxfnfexyp.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.epnwcf.com/Article/details/gkfotiuod.sHtML

openssl rand -hex 16
来源：http://baike.tarul.cn/Article/details/ghkmunhly.sHtML

[R68] 计算文件校验值
来源：http://3g.epnwcf.com/Article/details/gnwezywoi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.bbcook.cn/Article/details/gwfmianba.sHtML

[R69] 生成随机密码
来源：http://m.share.vehdjk.com/Article/details/gbdjectsr.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.yfazqb.com/Article/details/gpxnxpwew.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/gaysjvuae.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fktsv.cn/Article/details/gbxryodyj.sHtML

[R71] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gkfapnfuo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fktsv.cn/Article/details/ghlbrwfra.sHtML

[R72] 等待端口就绪
来源：http://baike.bbcook.cn/Article/details/gjiezkggo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gorblmbal.sHtML

[R73] 分割大日志
来源：http://blog.fktsv.cn/Article/details/ghxakztuw.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/gyyxmeavt.sHtML

[R74] 批量重命名
来源：http://3g.fktsv.cn/Article/details/gtqbmagxy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.sjlbkw.cn/Article/details/gefplbcrg.sHtML

[R75] 导出环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gbrufduib.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.bbcook.cn/Article/details/gulyabqof.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fktsv.cn/Article/details/gzxmjkzkd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gqnxdfesh.sHtML

[R77] 读取用户输入
来源：http://mobile.yfazqb.com/Article/details/gfrjibegi.sHtML

read -rp "请输入: " ans
来源：http://3g.vehdjk.com/Article/details/gpcndzzqc.sHtML

[R78] 交互式菜单
来源：http://3g.yfazqb.com/Article/details/gifwsppyu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.sjlbkw.cn/Article/details/ggvxeytxr.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/gheirpmev.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.bbcook.cn/Article/details/gxznmlpqa.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.vehdjk.com/Article/details/gsxvanclu.sHtML

time ./run.sh
来源：http://baike.epnwcf.com/Article/details/glulflpxf.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gdlihlvoa.sHtML

S. C / C++ 专题
来源：http://read.share.sjlbkw.cn/Article/details/gqkoyoaqq.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ggjzgxiwh.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/gjyegmsbz.sHtML

#include <stdio.h>
来源：http://www.m.share.tarul.cn/Article/details/gcflcpony.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.yfazqb.com/Article/details/gfwagbjlv.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.tarul.cn/Article/details/ghgbjyfky.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.bbcook.cn/Article/details/gzkgogxya.sHtML

[S03] C：读入整数
来源：http://baike.yfazqb.com/Article/details/gnuorsdcn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.bbcook.cn/Article/details/grlthrvma.sHtML

[S04] C：字符串复制
来源：http://read.share.bbcook.cn/Article/details/geiuamhqa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.vehdjk.com/Article/details/gvtdmkcnb.sHtML

[S05] C：字符串长度
来源：http://read.share.fktsv.cn/Article/details/gvsyrtkkg.sHtML

strlen(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzybypvrh.sHtML

[S06] C：字符串比较
来源：http://read.share.fktsv.cn/Article/details/gxmilzihp.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.bbcook.cn/Article/details/gzyicjzek.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.yfazqb.com/Article/details/griolsajc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.sjlbkw.cn/Article/details/gmozzzctt.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gsrcxgdju.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.yfazqb.com/Article/details/gekgdijbs.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/gftibqrcu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.tarul.cn/Article/details/grdcbjshi.sHtML

[S10] C：指针与解引用
来源：http://m.share.yfazqb.com/Article/details/gzqnyuijk.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.tarul.cn/Article/details/gaswnyoza.sHtML

[S11] C：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gsktzghul.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fktsv.cn/Article/details/gqnuyjsmp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.tarul.cn/Article/details/gmteagtiq.sHtML

fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gbwfleaah.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gpudmmzob.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gptxxkqfr.sHtML

[S13] C：宏定义
来源：http://www.share.vehdjk.com/Article/details/gfvkwtabj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.bbcook.cn/Article/details/gnwxdeefq.sHtML

[S14] C：枚举
来源：http://mobile.bbcook.cn/Article/details/giadlhefk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.vehdjk.com/Article/details/genwtpwrx.sHtML

[S15] C：类型转换
来源：http://baike.tarul.cn/Article/details/gddlxenqe.sHtML

(double) a / b
来源：http://wap.tarul.cn/Article/details/gfqpylgwi.sHtML

[S16] C：位操作置位
来源：http://www.blog.vehdjk.com/Article/details/gdymkxwap.sHtML

x |= (1 << 3);
来源：http://3g.sjlbkw.cn/Article/details/gthxtmhxq.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gtxctqsuw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.tarul.cn/Article/details/gnmkmjnhe.sHtML

[S18] C：命令行参数
来源：http://www.share.vehdjk.com/Article/details/gmzxuiuwb.sHtML

int main(int argc, char **argv)
来源：http://blog.bbcook.cn/Article/details/gpuubjtns.sHtML

[S19] C：快速排序
来源：http://wap.epnwcf.com/Article/details/gyzvocfye.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gyfayvptl.sHtML

[S20] C：二分查找
来源：http://3g.epnwcf.com/Article/details/gmzvibcsm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gcbomofbn.sHtML

[S21] C：字符类别判断
来源：http://read.share.vehdjk.com/Article/details/gnlwlpwpr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.yfazqb.com/Article/details/grsaegmxh.sHtML

[S22] C：字符串转数字
来源：http://wap.fktsv.cn/Article/details/glbrkszos.sHtML


<!-- 参考信息 -->