代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.bbcook.cn/Article/details/gttbczsyy.sHtML

[Q52] 删除指定行
来源：http://www.share.bbcook.cn/Article/details/gkwmwqmhb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/ghomkdgvk.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fktsv.cn/Article/details/gungqlsdk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fktsv.cn/Article/details/glmftkves.sHtML

[Q54] 清空表
来源：http://3g.tarul.cn/Article/details/gwlfhbjzp.sHtML

TRUNCATE TABLE logs;
来源：http://blog.epnwcf.com/Article/details/gkxkfsblc.sHtML

[Q55] 排名（并列占位）
来源：http://3g.sjlbkw.cn/Article/details/gzrjvcknf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gxukwhrdu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.yfazqb.com/Article/details/gzldibloa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.tarul.cn/Article/details/gacsqpdrn.sHtML

[Q57] 行号
来源：http://m.share.bbcook.cn/Article/details/gbbohlkqh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gjbvesuqx.sHtML

[Q58] 累计求和
来源：http://3g.bbcook.cn/Article/details/gqdqhbjnu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gpbsrizig.sHtML

[Q59] 分组内累计
来源：http://mobile.epnwcf.com/Article/details/gduhwqhnw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gvtezuspf.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.epnwcf.com/Article/details/gmmkwabrr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.vehdjk.com/Article/details/gqybgjsck.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.bbcook.cn/Article/details/grgykrfzl.sHtML

[Q61] 移动平均
来源：http://blog.vehdjk.com/Article/details/gjmwdxgjl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gwgiuvqsy.sHtML

[Q62] 分组占比
来源：http://baike.sjlbkw.cn/Article/details/gqastbclc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gviojclxu.sHtML

[Q63] 开启事务
来源：http://m.share.yfazqb.com/Article/details/gseyotrch.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.tarul.cn/Article/details/gzouaedxt.sHtML

[Q64] 提交事务
来源：http://www.m.share.epnwcf.com/Article/details/glgoxqryn.sHtML

COMMIT;
来源：http://www.blog.tarul.cn/Article/details/guyvddxvr.sHtML

[Q65] 回滚事务
来源：http://blog.vehdjk.com/Article/details/goqgptlys.sHtML

ROLLBACK;
来源：http://wap.epnwcf.com/Article/details/gsgrdsmaa.sHtML

[Q66] 行锁查询
来源：http://baike.sjlbkw.cn/Article/details/gkerwdelw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.yfazqb.com/Article/details/gjjbqcbyk.sHtML

[Q67] 设置隔离级别
来源：http://blog.bbcook.cn/Article/details/gcmuyqtfh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.tarul.cn/Article/details/ghahqnhvj.sHtML

[Q68] 保存点
来源：http://mobile.yfazqb.com/Article/details/gblvneegt.sHtML

SAVEPOINT sp1;
来源：http://m.share.fktsv.cn/Article/details/gbmnztuod.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fktsv.cn/Article/details/glmvmfvid.sHtML

[Q69] 查看执行计划
来源：http://wap.bbcook.cn/Article/details/gfvadxbit.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fktsv.cn/Article/details/gqmymrfcv.sHtML

[Q70] 更新统计信息
来源：http://www.blog.tarul.cn/Article/details/gvrxpukae.sHtML

ANALYZE TABLE users;
来源：http://baike.yfazqb.com/Article/details/gdjncdupj.sHtML

[Q71] 查看建表语句
来源：http://www.share.yfazqb.com/Article/details/gicaaxjxa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.epnwcf.com/Article/details/guzugwvou.sHtML

[Q72] 查看索引
来源：http://m.share.fktsv.cn/Article/details/gmsgdcffz.sHtML

SHOW INDEX FROM users;
来源：http://baike.vehdjk.com/Article/details/gueseadig.sHtML

[Q73] 查看表状态
来源：http://wap.yfazqb.com/Article/details/gsgqthzxd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.yfazqb.com/Article/details/gzxdkpjgf.sHtML

[Q74] 强制使用索引
来源：http://3g.sjlbkw.cn/Article/details/gwrnhenlv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxmbaeai.sHtML

[Q75] 日期格式化
来源：http://baike.vehdjk.com/Article/details/ggzjcntun.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fktsv.cn/Article/details/ggucgakyd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.bbcook.cn/Article/details/gnthqcsmm.sHtML

[Q76] 按天统计
来源：http://www.blog.sjlbkw.cn/Article/details/gpvwxesnj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.tarul.cn/Article/details/gtdvvwdev.sHtML

[Q77] 时间加减
来源：http://www.blog.fktsv.cn/Article/details/gtqmhihuw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.bbcook.cn/Article/details/gehaxhvvb.sHtML

[Q78] 当前时间
来源：http://www.blog.tarul.cn/Article/details/ggmwukogt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.tarul.cn/Article/details/goqlzkkwq.sHtML

[Q79] 字符串拼接
来源：http://baike.bbcook.cn/Article/details/gvkbyckie.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.vehdjk.com/Article/details/gubnturxw.sHtML

[Q80] 字符串截取
来源：http://mobile.vehdjk.com/Article/details/gnwxztgtb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fktsv.cn/Article/details/grlwghdmf.sHtML

[Q81] 字符串替换
来源：http://3g.fktsv.cn/Article/details/guyyovdpi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.yfazqb.com/Article/details/gvocdrqjc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.vehdjk.com/Article/details/gnpvxmzzu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/ghpzuvctf.sHtML

[Q83] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gwhkngxub.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gbagxeitn.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fktsv.cn/Article/details/gmttokbyn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gfyerxztm.sHtML

[Q85] 数值取整
来源：http://mobile.epnwcf.com/Article/details/gojkbkchc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.tarul.cn/Article/details/grursthwf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.yfazqb.com/Article/details/ghsvnviyd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.sjlbkw.cn/Article/details/gpunpsnej.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fktsv.cn/Article/details/gupvglswu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.yfazqb.com/Article/details/gbcpnxzmp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fktsv.cn/Article/details/gftimariv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.vehdjk.com/Article/details/galvvbocx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.bbcook.cn/Article/details/gifqhplpx.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.tarul.cn/Article/details/ghklqvljn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/gcnrkyzzg.sHtML

[Q90] 生成序号列
来源：http://mobile.epnwcf.com/Article/details/glysaxnit.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.epnwcf.com/Article/details/gkltjasqx.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gouunwebq.sHtML

R. Bash 专题
来源：http://mobile.epnwcf.com/Article/details/gqnkfnjwh.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ggkuipnvl.sHtML

[R01] shebang 与严格模式
来源：http://3g.sjlbkw.cn/Article/details/gwwijttol.sHtML

#!/usr/bin/env bash
来源：http://wap.sjlbkw.cn/Article/details/gghszycxu.sHtML

set -euo pipefail
来源：http://read.share.yfazqb.com/Article/details/gjgtprqxl.sHtML

[R02] 变量赋值与使用
来源：http://m.share.tarul.cn/Article/details/gmnesdyyd.sHtML

name="Tom"; echo "$name"
来源：http://blog.epnwcf.com/Article/details/gntmwgybd.sHtML

[R03] 只读变量
来源：http://baike.epnwcf.com/Article/details/gislmqnoi.sHtML

readonly PI=3.14
来源：http://blog.fktsv.cn/Article/details/gbsccznfg.sHtML

[R04] 位置参数
来源：http://baike.tarul.cn/Article/details/gvjpabeqz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.bbcook.cn/Article/details/gseftmqjm.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gedgutbrf.sHtML

name="${1:-default}"
来源：http://www.blog.sjlbkw.cn/Article/details/gnurlaprc.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.epnwcf.com/Article/details/gsifkaykg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/gtlozimlj.sHtML

[R07] if 判断文件
来源：http://read.share.tarul.cn/Article/details/gwlvybupf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gsxsjykeo.sHtML

[R08] 数值比较
来源：http://www.m.share.tarul.cn/Article/details/gpsprqlks.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.vehdjk.com/Article/details/gcndkymes.sHtML

[R09] 字符串比较
来源：http://baike.vehdjk.com/Article/details/giwykqvgb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gzqhgijgi.sHtML

[R10] 正则匹配
来源：http://3g.sjlbkw.cn/Article/details/guiampjwu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.yfazqb.com/Article/details/ghowyzqdl.sHtML

[R11] case 多分支
来源：http://www.share.bbcook.cn/Article/details/gwhjvmcet.sHtML

case "$1" in
来源：http://mobile.yfazqb.com/Article/details/gmjrrcafx.sHtML

start) echo "启动" ;;
来源：http://www.share.yfazqb.com/Article/details/gunmptbmf.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gfjseizxh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.yfazqb.com/Article/details/gremfysfd.sHtML

esac
来源：http://www.m.share.bbcook.cn/Article/details/gjdygdape.sHtML

[R12] for 遍历文件
来源：http://3g.epnwcf.com/Article/details/gmcducume.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.epnwcf.com/Article/details/gfzegctmv.sHtML

[R13] for 计数循环
来源：http://baike.tarul.cn/Article/details/gxsrdkddc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/gycoodwtn.sHtML

[R14] C 风格 for
来源：http://wap.vehdjk.com/Article/details/gsrdtwjdl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/geqqbsgbu.sHtML

[R15] while 逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gcsundwus.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fktsv.cn/Article/details/gxqvzshwj.sHtML

[R16] until 等待条件
来源：http://baike.tarul.cn/Article/details/gfazzstwa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/ggumxdkow.sHtML

[R17] 数组定义与取值
来源：http://www.share.vehdjk.com/Article/details/gqtvtkpvx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.bbcook.cn/Article/details/gpnceurwj.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/ggqnfklln.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.yfazqb.com/Article/details/greqvxwkz.sHtML

[R19] 数组长度
来源：http://read.share.fktsv.cn/Article/details/gptppatmg.sHtML

echo "${#arr[@]}"
来源：http://wap.vehdjk.com/Article/details/gvceowqoc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.sjlbkw.cn/Article/details/gebkocifi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.yfazqb.com/Article/details/gyejczwgk.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/gieomltof.sHtML

echo "${#s}"
来源：http://baike.fktsv.cn/Article/details/gsnpwetil.sHtML

[R22] 截取子串
来源：http://m.share.epnwcf.com/Article/details/ghwcnmzzr.sHtML

echo "${s:0:5}"
来源：http://www.blog.tarul.cn/Article/details/gmjxdcxne.sHtML

[R23] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/gyeljpdtm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.vehdjk.com/Article/details/gtdugofrw.sHtML

[R24] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gfkjnxqic.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.epnwcf.com/Article/details/gujudzxlq.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.sjlbkw.cn/Article/details/gxewjcioi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/glknhthyu.sHtML

[R26] 命令替换
来源：http://www.share.fktsv.cn/Article/details/gtpeivnfy.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.tarul.cn/Article/details/gcxpchsmg.sHtML

[R27] 算术展开
来源：http://m.share.yfazqb.com/Article/details/gdcoeptkp.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmohoivc.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/gfhpfwovl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.sjlbkw.cn/Article/details/gdvtvppbb.sHtML

[R29] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/ghabbxtkn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.tarul.cn/Article/details/goupjntod.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/gbnbabjrt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.vehdjk.com/Article/details/gqmmaxgwy.sHtML

[R31] 局部变量
来源：http://m.share.epnwcf.com/Article/details/gvgduebvh.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fktsv.cn/Article/details/gbbstbaoc.sHtML

[R32] 参数个数校验
来源：http://blog.vehdjk.com/Article/details/gfbycdubw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/ghkzidwdq.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.vehdjk.com/Article/details/gcgdhhwyg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.bbcook.cn/Article/details/galrcnwty.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/gyshhraxb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/gopvovkrt.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/gapsqatsu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.yfazqb.com/Article/details/ggoqyjanj.sHtML

[R36] 并发执行多个任务
来源：http://m.share.bbcook.cn/Article/details/gcyblrttc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.sjlbkw.cn/Article/details/gnyfoierz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.tarul.cn/Article/details/gptwgiqtw.sHtML

files=$(ls -1)
来源：http://www.blog.yfazqb.com/Article/details/giarjxkst.sHtML

[R38] 管道串联
来源：http://www.m.share.epnwcf.com/Article/details/gyyzmqgxx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.tarul.cn/Article/details/gfzbmeygn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.sjlbkw.cn/Article/details/gtuqlvzgh.sHtML

cmd > out.log 2>&1
来源：http://www.blog.tarul.cn/Article/details/gtschpeep.sHtML

[R40] 追加写日志
来源：http://www.share.bbcook.cn/Article/details/gizhytoaa.sHtML

echo "log" >> out.log
来源：http://wap.fktsv.cn/Article/details/gsdrhgqfx.sHtML

[R41] 丢弃输出
来源：http://m.share.vehdjk.com/Article/details/gxmqmmeja.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fktsv.cn/Article/details/gyxiarrrt.sHtML

[R42] 输入重定向
来源：http://www.blog.sjlbkw.cn/Article/details/glxcducnr.sHtML

wc -l < a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gqefyrznx.sHtML

[R43] 按名字查找文件
来源：http://mobile.yfazqb.com/Article/details/ghkogvojb.sHtML

find . -name "*.log" -type f
来源：http://baike.bbcook.cn/Article/details/gnvuwcvup.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/gfvvkbxxw.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/gqsalpakq.sHtML

[R45] 批量删除
来源：http://blog.fktsv.cn/Article/details/gpzktivli.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.tarul.cn/Article/details/gjpizaajp.sHtML

[R46] 递归替换文件内容
来源：http://www.share.yfazqb.com/Article/details/gaqlahbea.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.sjlbkw.cn/Article/details/guqqjfytq.sHtML

[R47] sed 单行替换
来源：http://m.share.sjlbkw.cn/Article/details/ghusmscob.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.epnwcf.com/Article/details/glwoiscah.sHtML

[R48] awk 取指定列
来源：http://wap.tarul.cn/Article/details/gzsrgjmac.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.epnwcf.com/Article/details/gmpgzzwum.sHtML

[R49] awk 带条件
来源：http://baike.sjlbkw.cn/Article/details/ghkrueazt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.vehdjk.com/Article/details/gyqrrgndr.sHtML

[R50] awk 求和
来源：http://m.share.tarul.cn/Article/details/gmhfjwqup.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/glnumtklx.sHtML

[R51] 排序去重取前几
来源：http://3g.epnwcf.com/Article/details/gxkwrqsgg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.vehdjk.com/Article/details/glusrmoyc.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/gkjwoicfj.sHtML

wc -l a.txt
来源：http://read.share.vehdjk.com/Article/details/gnoeboyvl.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.epnwcf.com/Article/details/gqldeqxtz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.epnwcf.com/Article/details/gjokwsgrs.sHtML

[R54] 比较两个文件
来源：http://baike.yfazqb.com/Article/details/gwfxtcemh.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/guczcwrcj.sHtML

[R55] 压缩与解压
来源：http://read.share.fktsv.cn/Article/details/gwqvmvqdj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/gdphvqofq.sHtML

[R56] 远程拷贝
来源：http://3g.fktsv.cn/Article/details/ggelbitvd.sHtML

scp file user@host:/path/
来源：http://mobile.bbcook.cn/Article/details/gbtttzbff.sHtML

[R57] 远程执行命令
来源：http://3g.bbcook.cn/Article/details/gdbdudbno.sHtML

ssh user@host 'uptime'
来源：http://www.share.sjlbkw.cn/Article/details/gozuryfkw.sHtML

[R58] 下载文件
来源：http://baike.bbcook.cn/Article/details/gxrlxdlqo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.yfazqb.com/Article/details/giexfcfxd.sHtML

[R59] 发 POST JSON
来源：http://m.share.epnwcf.com/Article/details/galezgizu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gwvlctwiv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gerfywptw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.vehdjk.com/Article/details/grkdqyphg.sHtML

[R61] 磁盘占用
来源：http://www.blog.fktsv.cn/Article/details/gwbburzlc.sHtML

df -h;  du -sh *
来源：http://www.m.share.yfazqb.com/Article/details/gyrzlpvqe.sHtML

[R62] 找最占空间的文件
来源：http://wap.fktsv.cn/Article/details/glfbkkcgm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/gbimcimlp.sHtML

[R63] 内存与进程
来源：http://read.share.epnwcf.com/Article/details/gweazpubs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.vehdjk.com/Article/details/gwcpyephp.sHtML

[R64] 结束进程
来源：http://www.share.vehdjk.com/Article/details/gzuqekfca.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.bbcook.cn/Article/details/ggdiermab.sHtML

[R65] 查看端口占用
来源：http://mobile.vehdjk.com/Article/details/guwmdsgws.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.yfazqb.com/Article/details/gidjjsgaj.sHtML

[R66] 定时任务
来源：http://baike.bbcook.cn/Article/details/gvcwkoghy.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.tarul.cn/Article/details/gzhlyaegm.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.epnwcf.com/Article/details/gdacshjls.sHtML

openssl rand -hex 16
来源：http://wap.fktsv.cn/Article/details/gtbbasait.sHtML

[R68] 计算文件校验值
来源：http://blog.vehdjk.com/Article/details/gccikndjm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gdzsoppkq.sHtML

[R69] 生成随机密码
来源：http://wap.sjlbkw.cn/Article/details/gimsodoso.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.epnwcf.com/Article/details/gromluoqy.sHtML

[R70] 时间戳与互转
来源：http://m.share.yfazqb.com/Article/details/gzhiljffd.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.vehdjk.com/Article/details/gjsjgwzhp.sHtML

[R71] 日期格式化
来源：http://blog.epnwcf.com/Article/details/ganfkfece.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.tarul.cn/Article/details/gkwwwmjpc.sHtML

[R72] 等待端口就绪
来源：http://3g.bbcook.cn/Article/details/glspkixai.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.vehdjk.com/Article/details/godgjyeyl.sHtML

[R73] 分割大日志
来源：http://www.share.vehdjk.com/Article/details/geshhjjbc.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/gfzisqzgt.sHtML

[R74] 批量重命名
来源：http://3g.vehdjk.com/Article/details/geuimmmao.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/gncwzlljf.sHtML

[R75] 导出环境变量
来源：http://3g.tarul.cn/Article/details/glvuytggq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.bbcook.cn/Article/details/ghuicwfbu.sHtML

[R76] 使用临时文件
来源：http://baike.bbcook.cn/Article/details/gemdesizz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gpjmtgzui.sHtML

[R77] 读取用户输入
来源：http://www.m.share.vehdjk.com/Article/details/gpnzezcbu.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/gxepkubab.sHtML

[R78] 交互式菜单
来源：http://mobile.epnwcf.com/Article/details/ghuexayxx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.vehdjk.com/Article/details/grozgmvgi.sHtML

[R79] 解析命令行选项
来源：http://mobile.yfazqb.com/Article/details/gteizebwx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.yfazqb.com/Article/details/glmkqeajv.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.sjlbkw.cn/Article/details/gmacbjmss.sHtML

time ./run.sh
来源：http://www.share.tarul.cn/Article/details/gthjpjcbd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gicpdniic.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gldlxbinw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gaftmlagw.sHtML

[S01] C：Hello World
来源：http://m.share.bbcook.cn/Article/details/geyzwfrud.sHtML

#include <stdio.h>
来源：http://m.share.bbcook.cn/Article/details/gwyspiftq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.yfazqb.com/Article/details/gbpgvkapk.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gtcrbemeh.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.epnwcf.com/Article/details/gmbilazux.sHtML

[S03] C：读入整数
来源：http://baike.yfazqb.com/Article/details/gihxtarrj.sHtML

int x; scanf("%d", &x);
来源：http://mobile.vehdjk.com/Article/details/ggrnciqtj.sHtML

[S04] C：字符串复制
来源：http://m.share.sjlbkw.cn/Article/details/gjfvgirbj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.vehdjk.com/Article/details/gmumbwrli.sHtML

[S05] C：字符串长度
来源：http://wap.vehdjk.com/Article/details/gzvcmrcxe.sHtML

strlen(s)
来源：http://mobile.yfazqb.com/Article/details/gstxbqnid.sHtML

[S06] C：字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gyybkzmet.sHtML

strcmp(a, b) == 0
来源：http://m.share.sjlbkw.cn/Article/details/gpvdfbvdw.sHtML

[S07] C：数组遍历求和
来源：http://wap.vehdjk.com/Article/details/gqhzbweak.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fktsv.cn/Article/details/gdrrpvqlb.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/ghfhciwnh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.bbcook.cn/Article/details/gsbtstkmx.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.tarul.cn/Article/details/ggkttxigt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.yfazqb.com/Article/details/gmgzzrgnh.sHtML

[S10] C：指针与解引用
来源：http://read.share.epnwcf.com/Article/details/gdudciogl.sHtML

int *p = &a;  *p = 5;
来源：http://3g.bbcook.cn/Article/details/grohdlvmt.sHtML

[S11] C：逐行读文件
来源：http://3g.tarul.cn/Article/details/gvkziauas.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.tarul.cn/Article/details/goairnimo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.bbcook.cn/Article/details/gsogtnjtn.sHtML

fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gmqavdpyp.sHtML

[S12] C：写文件
来源：http://3g.sjlbkw.cn/Article/details/gklvxhses.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/gezyvtras.sHtML

[S13] C：宏定义
来源：http://www.share.sjlbkw.cn/Article/details/gsjkukwtp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.bbcook.cn/Article/details/gxspdqjer.sHtML

[S14] C：枚举
来源：http://3g.bbcook.cn/Article/details/gfqrkxghz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.sjlbkw.cn/Article/details/gjnhetvyy.sHtML

[S15] C：类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gddpoyxkl.sHtML

(double) a / b
来源：http://wap.bbcook.cn/Article/details/gqbnjwfap.sHtML

[S16] C：位操作置位
来源：http://baike.sjlbkw.cn/Article/details/gnnzfyncf.sHtML

x |= (1 << 3);
来源：http://read.share.bbcook.cn/Article/details/gcosnwbry.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gnhxjmsjg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.yfazqb.com/Article/details/gwpnlagvo.sHtML

[S18] C：命令行参数
来源：http://m.share.vehdjk.com/Article/details/gsqzaodxz.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/gzglorofq.sHtML

[S19] C：快速排序
来源：http://www.m.share.bbcook.cn/Article/details/gxppxyeiv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gemsobkva.sHtML

[S20] C：二分查找
来源：http://3g.fktsv.cn/Article/details/gttrsuawx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gtkurrklp.sHtML

[S21] C：字符类别判断
来源：http://baike.bbcook.cn/Article/details/gusnqsxyc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fktsv.cn/Article/details/gvhjbjrfb.sHtML

[S22] C：字符串转数字
来源：http://m.share.fktsv.cn/Article/details/gfxqghrht.sHtML


<!-- 参考信息 -->