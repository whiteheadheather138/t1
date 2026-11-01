代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/gdadqrttl.sHtML

[Q50] 批量更新
来源：http://mobile.epnwcf.com/Article/details/grhimsrqf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.tarul.cn/Article/details/gzfivpfny.sHtML

[Q51] 用子查询更新
来源：http://read.share.tarul.cn/Article/details/gttzlhgoi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.yfazqb.com/Article/details/guqebkmif.sHtML

[Q52] 删除指定行
来源：http://baike.yfazqb.com/Article/details/goufxbnvn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gqyjbtcef.sHtML

[Q53] 按条件删除
来源：http://www.m.share.epnwcf.com/Article/details/guratarwo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.yfazqb.com/Article/details/gtbbamxgb.sHtML

[Q54] 清空表
来源：http://www.blog.tarul.cn/Article/details/gsjyascll.sHtML

TRUNCATE TABLE logs;
来源：http://baike.tarul.cn/Article/details/gedukbgfn.sHtML

[Q55] 排名（并列占位）
来源：http://baike.sjlbkw.cn/Article/details/gzhrezbeb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.yfazqb.com/Article/details/givfyhlgv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.bbcook.cn/Article/details/gowtqqypk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.vehdjk.com/Article/details/gcilufmca.sHtML

[Q57] 行号
来源：http://mobile.fktsv.cn/Article/details/gshqnmlfg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.yfazqb.com/Article/details/guxaaumsa.sHtML

[Q58] 累计求和
来源：http://m.share.vehdjk.com/Article/details/gxeqgbync.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.tarul.cn/Article/details/gasrojrqc.sHtML

[Q59] 分组内累计
来源：http://www.share.yfazqb.com/Article/details/gnbldjaov.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gzhrrcrfn.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fktsv.cn/Article/details/gqewojduc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fktsv.cn/Article/details/glvbcqeoh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fktsv.cn/Article/details/gamvfugjk.sHtML

[Q61] 移动平均
来源：http://3g.bbcook.cn/Article/details/gugsnjsfu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gpcubkpuw.sHtML

[Q62] 分组占比
来源：http://www.blog.vehdjk.com/Article/details/gmavrweoi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gpwipoovs.sHtML

[Q63] 开启事务
来源：http://blog.bbcook.cn/Article/details/gkunfregf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.yfazqb.com/Article/details/gwxmiwxjm.sHtML

[Q64] 提交事务
来源：http://www.m.share.bbcook.cn/Article/details/gwlduweuz.sHtML

COMMIT;
来源：http://3g.vehdjk.com/Article/details/gspenutud.sHtML

[Q65] 回滚事务
来源：http://m.share.sjlbkw.cn/Article/details/gbyvolvza.sHtML

ROLLBACK;
来源：http://baike.tarul.cn/Article/details/geyqwafue.sHtML

[Q66] 行锁查询
来源：http://wap.yfazqb.com/Article/details/gjpilcbxd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.bbcook.cn/Article/details/goysnnyud.sHtML

[Q67] 设置隔离级别
来源：http://wap.tarul.cn/Article/details/gyxqpayll.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.tarul.cn/Article/details/geivqzulf.sHtML

[Q68] 保存点
来源：http://www.share.epnwcf.com/Article/details/guiauiper.sHtML

SAVEPOINT sp1;
来源：http://m.share.bbcook.cn/Article/details/gimfpovot.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fktsv.cn/Article/details/gzljgpzwu.sHtML

[Q69] 查看执行计划
来源：http://mobile.fktsv.cn/Article/details/ghadfiuho.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.sjlbkw.cn/Article/details/gtwkfcbag.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/gqgfytyay.sHtML

ANALYZE TABLE users;
来源：http://baike.fktsv.cn/Article/details/gptlikyrg.sHtML

[Q71] 查看建表语句
来源：http://m.share.epnwcf.com/Article/details/gswlyasvu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fktsv.cn/Article/details/gsvupygqy.sHtML

[Q72] 查看索引
来源：http://www.blog.bbcook.cn/Article/details/gebalfgof.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fktsv.cn/Article/details/gbwiwfvwq.sHtML

[Q73] 查看表状态
来源：http://wap.tarul.cn/Article/details/gxflbdtop.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gihsziwcy.sHtML

[Q74] 强制使用索引
来源：http://read.share.bbcook.cn/Article/details/glntrgwym.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fktsv.cn/Article/details/gtcylbemv.sHtML

[Q75] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gugggmpav.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gvjjeamkz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.sjlbkw.cn/Article/details/gpfgfibki.sHtML

[Q76] 按天统计
来源：http://www.m.share.epnwcf.com/Article/details/greixotom.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/gevcqjyjj.sHtML

[Q77] 时间加减
来源：http://www.share.tarul.cn/Article/details/gwvelpqrk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.vehdjk.com/Article/details/gbwiuroga.sHtML

[Q78] 当前时间
来源：http://read.share.bbcook.cn/Article/details/gmrkvvgvn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.epnwcf.com/Article/details/gbmhcbaff.sHtML

[Q79] 字符串拼接
来源：http://blog.fktsv.cn/Article/details/gofbdnfhg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.epnwcf.com/Article/details/gpfpienzb.sHtML

[Q80] 字符串截取
来源：http://www.m.share.yfazqb.com/Article/details/ghvmzrzeu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.yfazqb.com/Article/details/gdljamgyw.sHtML

[Q81] 字符串替换
来源：http://baike.yfazqb.com/Article/details/gkvtvtlgo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.epnwcf.com/Article/details/gtnevljoo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.vehdjk.com/Article/details/gvmmkcskg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/glydxavdi.sHtML

[Q83] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gdsqnsmtt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gxuuipxcr.sHtML

[Q84] 去除首尾空格
来源：http://wap.epnwcf.com/Article/details/gspzphctv.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/glyucwgsp.sHtML

[Q85] 数值取整
来源：http://m.share.bbcook.cn/Article/details/gnwanozkc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.sjlbkw.cn/Article/details/gyzdvyook.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.vehdjk.com/Article/details/grxfpmfdo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.yfazqb.com/Article/details/gunmjefxy.sHtML

[Q87] JSON 字段做条件
来源：http://baike.sjlbkw.cn/Article/details/gdyrrurwr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.vehdjk.com/Article/details/gmwostzrf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.sjlbkw.cn/Article/details/gdwkyefhc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.tarul.cn/Article/details/gryefbujl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.vehdjk.com/Article/details/getejzhaj.sHtML

[Q89] 判断表是否存在
来源：http://www.share.vehdjk.com/Article/details/gbtveqfol.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.vehdjk.com/Article/details/gdqyjowoj.sHtML

[Q90] 生成序号列
来源：http://www.m.share.bbcook.cn/Article/details/gufvvtjsq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.tarul.cn/Article/details/gkmcojwag.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdbugbycr.sHtML

R. Bash 专题
来源：http://www.blog.epnwcf.com/Article/details/gnuefidob.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gtzkqcmkd.sHtML

[R01] shebang 与严格模式
来源：http://baike.bbcook.cn/Article/details/gqcpuiydj.sHtML

#!/usr/bin/env bash
来源：http://baike.yfazqb.com/Article/details/gpfrbzbpn.sHtML

set -euo pipefail
来源：http://wap.epnwcf.com/Article/details/gnbojlkcl.sHtML

[R02] 变量赋值与使用
来源：http://blog.vehdjk.com/Article/details/gjdckokte.sHtML

name="Tom"; echo "$name"
来源：http://read.share.sjlbkw.cn/Article/details/gozkhssic.sHtML

[R03] 只读变量
来源：http://read.share.tarul.cn/Article/details/ggnviwrlf.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/gjcfzxrub.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/gaxhhmsjt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.epnwcf.com/Article/details/gwktjqagu.sHtML

[R05] 参数默认值
来源：http://www.share.tarul.cn/Article/details/gdskduqdv.sHtML

name="${1:-default}"
来源：http://mobile.epnwcf.com/Article/details/grunspbvj.sHtML

[R06] 判断命令是否存在
来源：http://read.share.vehdjk.com/Article/details/gsjoqcznx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gqfebcbkn.sHtML

[R07] if 判断文件
来源：http://www.m.share.yfazqb.com/Article/details/gvhsaykdq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.vehdjk.com/Article/details/gxzbltowm.sHtML

[R08] 数值比较
来源：http://www.blog.bbcook.cn/Article/details/gdrxmmkuo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/giydbbaft.sHtML

[R09] 字符串比较
来源：http://3g.epnwcf.com/Article/details/gopjemhip.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.tarul.cn/Article/details/gmrcafeca.sHtML

[R10] 正则匹配
来源：http://www.m.share.epnwcf.com/Article/details/gxptcljkh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.yfazqb.com/Article/details/griebejnt.sHtML

[R11] case 多分支
来源：http://mobile.bbcook.cn/Article/details/gjoeacbof.sHtML

case "$1" in
来源：http://blog.epnwcf.com/Article/details/ghfiqmqcf.sHtML

start) echo "启动" ;;
来源：http://www.m.share.tarul.cn/Article/details/gypeoxwkm.sHtML

stop)  echo "停止" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gdbhncnnu.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.vehdjk.com/Article/details/gbwqvvrjb.sHtML

esac
来源：http://www.share.fktsv.cn/Article/details/gmdpuqwqa.sHtML

[R12] for 遍历文件
来源：http://wap.sjlbkw.cn/Article/details/gnbzpkfwj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.tarul.cn/Article/details/gnsksxvux.sHtML

[R13] for 计数循环
来源：http://3g.bbcook.cn/Article/details/gzjxexpia.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/gkjvpyzim.sHtML

[R14] C 风格 for
来源：http://www.blog.sjlbkw.cn/Article/details/grbosptjh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gztwzxdpj.sHtML

[R15] while 逐行读文件
来源：http://3g.yfazqb.com/Article/details/gcdbdcnhf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.epnwcf.com/Article/details/gzekfggua.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/gpzjgsvoj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fktsv.cn/Article/details/gsdyxcuiu.sHtML

[R17] 数组定义与取值
来源：http://mobile.fktsv.cn/Article/details/gooutojvl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.vehdjk.com/Article/details/gtwtodofj.sHtML

[R18] 遍历数组
来源：http://mobile.sjlbkw.cn/Article/details/gsleewtfw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.epnwcf.com/Article/details/gauwvpiot.sHtML

[R19] 数组长度
来源：http://www.m.share.vehdjk.com/Article/details/gktviuvib.sHtML

echo "${#arr[@]}"
来源：http://mobile.fktsv.cn/Article/details/gqeabswns.sHtML

[R20] 关联数组（字典）
来源：http://mobile.sjlbkw.cn/Article/details/gxfdyrlyw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/guasfdlwu.sHtML

[R21] 字符串长度
来源：http://baike.fktsv.cn/Article/details/gqulpsknj.sHtML

echo "${#s}"
来源：http://www.share.sjlbkw.cn/Article/details/gzcsowmou.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gzicigvgv.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gadmtexlg.sHtML

[R23] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gogzcqwaw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fktsv.cn/Article/details/gkwjlpfur.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gpvitxfzq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fktsv.cn/Article/details/getdzgwon.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.bbcook.cn/Article/details/grkxdwslv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.vehdjk.com/Article/details/ggbrnpgtq.sHtML

[R26] 命令替换
来源：http://read.share.yfazqb.com/Article/details/gwnenxnsc.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.yfazqb.com/Article/details/gkwbahfmd.sHtML

[R27] 算术展开
来源：http://www.m.share.vehdjk.com/Article/details/guxtfsbdj.sHtML

echo $((1 + 2 * 3))
来源：http://blog.epnwcf.com/Article/details/gcgnmhwqp.sHtML

[R28] 浮点运算
来源：http://wap.fktsv.cn/Article/details/gkvnugqph.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.vehdjk.com/Article/details/goxvbmxvy.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/gwrotukwy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.yfazqb.com/Article/details/ggpzzdeoi.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fktsv.cn/Article/details/gtluhmccx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.vehdjk.com/Article/details/gkmmexgkm.sHtML

[R31] 局部变量
来源：http://wap.sjlbkw.cn/Article/details/ghumiauhy.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.epnwcf.com/Article/details/garyemlsn.sHtML

[R32] 参数个数校验
来源：http://3g.tarul.cn/Article/details/geqrakblx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/grjwcqzys.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fktsv.cn/Article/details/gnizdhkvj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.tarul.cn/Article/details/gqucghqxp.sHtML

[R34] 退出时清理
来源：http://read.share.epnwcf.com/Article/details/gzrbdppez.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.tarul.cn/Article/details/gjnocvfsg.sHtML

[R35] 后台执行并等待
来源：http://www.blog.tarul.cn/Article/details/gxuhruzol.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.epnwcf.com/Article/details/grognethe.sHtML

[R36] 并发执行多个任务
来源：http://3g.tarul.cn/Article/details/gyridzsge.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.tarul.cn/Article/details/gkwmwntti.sHtML

[R37] 把输出赋给变量
来源：http://read.share.tarul.cn/Article/details/gkcekvqmd.sHtML

files=$(ls -1)
来源：http://3g.epnwcf.com/Article/details/gvxzlnhbc.sHtML

[R38] 管道串联
来源：http://3g.vehdjk.com/Article/details/gomrkihuf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.bbcook.cn/Article/details/gutlntqek.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.vehdjk.com/Article/details/gbxbfcozz.sHtML

cmd > out.log 2>&1
来源：http://baike.fktsv.cn/Article/details/gqorjbaso.sHtML

[R40] 追加写日志
来源：http://blog.vehdjk.com/Article/details/gpcslwsec.sHtML

echo "log" >> out.log
来源：http://www.share.epnwcf.com/Article/details/gwoebtdnu.sHtML

[R41] 丢弃输出
来源：http://m.share.vehdjk.com/Article/details/gckyeuhhk.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.bbcook.cn/Article/details/gwooypxlf.sHtML

[R42] 输入重定向
来源：http://3g.tarul.cn/Article/details/gvjftvsqq.sHtML

wc -l < a.txt
来源：http://read.share.yfazqb.com/Article/details/gjvityypm.sHtML

[R43] 按名字查找文件
来源：http://www.blog.bbcook.cn/Article/details/ghbrqmzfu.sHtML

find . -name "*.log" -type f
来源：http://mobile.vehdjk.com/Article/details/gtvckwmbm.sHtML

[R44] 按修改时间查找
来源：http://mobile.sjlbkw.cn/Article/details/gddqhhzdm.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/gkvlxjdps.sHtML

[R45] 批量删除
来源：http://mobile.vehdjk.com/Article/details/gozgymzfn.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.vehdjk.com/Article/details/gnkutwetg.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.sjlbkw.cn/Article/details/ggozmkroz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.yfazqb.com/Article/details/gockcywvb.sHtML

[R47] sed 单行替换
来源：http://www.share.sjlbkw.cn/Article/details/gbqfeprvh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.yfazqb.com/Article/details/gmoswehvv.sHtML

[R48] awk 取指定列
来源：http://www.share.fktsv.cn/Article/details/gokgtcpfm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.epnwcf.com/Article/details/ggnmkqxmx.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/ghvhywjpo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.epnwcf.com/Article/details/gufottgsi.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/gvtrqmast.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gbrykavvw.sHtML

[R51] 排序去重取前几
来源：http://mobile.vehdjk.com/Article/details/gsdhloodn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fktsv.cn/Article/details/gtrwibdzu.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/gsauzzrso.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/gmklndrlh.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.tarul.cn/Article/details/guiayttdi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.epnwcf.com/Article/details/gvcgxcjob.sHtML

[R54] 比较两个文件
来源：http://read.share.vehdjk.com/Article/details/gfdcgedqh.sHtML

diff a.txt b.txt
来源：http://baike.fktsv.cn/Article/details/gbnrisnhr.sHtML

[R55] 压缩与解压
来源：http://3g.bbcook.cn/Article/details/gzryrvktk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.vehdjk.com/Article/details/gkjfkfosv.sHtML

[R56] 远程拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjznpmrq.sHtML

scp file user@host:/path/
来源：http://www.m.share.vehdjk.com/Article/details/gbywridqm.sHtML

[R57] 远程执行命令
来源：http://mobile.epnwcf.com/Article/details/gidchaneq.sHtML

ssh user@host 'uptime'
来源：http://www.blog.vehdjk.com/Article/details/gjfluknnd.sHtML

[R58] 下载文件
来源：http://read.share.yfazqb.com/Article/details/gygshjdbo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.epnwcf.com/Article/details/grdvgbyrx.sHtML

[R59] 发 POST JSON
来源：http://baike.yfazqb.com/Article/details/glkrudgok.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.bbcook.cn/Article/details/gsrxmczkt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/geeyfrgld.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.epnwcf.com/Article/details/gkzxkxoeo.sHtML

[R61] 磁盘占用
来源：http://www.m.share.tarul.cn/Article/details/glrwbpqka.sHtML

df -h;  du -sh *
来源：http://www.share.fktsv.cn/Article/details/gigouykpw.sHtML

[R62] 找最占空间的文件
来源：http://wap.sjlbkw.cn/Article/details/gwazzpiid.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.tarul.cn/Article/details/gbcgpqqfx.sHtML

[R63] 内存与进程
来源：http://m.share.bbcook.cn/Article/details/grapzobuf.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.tarul.cn/Article/details/gtjqmizuj.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gawgysjme.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gjbhfxmcc.sHtML

[R65] 查看端口占用
来源：http://m.share.bbcook.cn/Article/details/gfxqcqpwc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fktsv.cn/Article/details/gyrzvzsos.sHtML

[R66] 定时任务
来源：http://mobile.vehdjk.com/Article/details/ghjsznpwq.sHtML

crontab -e;  crontab -l
来源：http://www.share.fktsv.cn/Article/details/gntayrkxn.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.vehdjk.com/Article/details/gjgummjpc.sHtML

openssl rand -hex 16
来源：http://wap.epnwcf.com/Article/details/gvwquwoaz.sHtML

[R68] 计算文件校验值
来源：http://3g.yfazqb.com/Article/details/gltkvqdzz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.epnwcf.com/Article/details/gdjvzzqge.sHtML

[R69] 生成随机密码
来源：http://baike.fktsv.cn/Article/details/ghvahotwj.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.sjlbkw.cn/Article/details/gfgafsefp.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/ghbnhljqb.sHtML

date +%s;  date -d @1700000000
来源：http://baike.yfazqb.com/Article/details/ggibcovdw.sHtML

[R71] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gizhwhtxs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.sjlbkw.cn/Article/details/gadbxqync.sHtML

[R72] 等待端口就绪
来源：http://m.share.sjlbkw.cn/Article/details/gbouddarz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gfxhrandl.sHtML

[R73] 分割大日志
来源：http://www.blog.bbcook.cn/Article/details/gbxycjctz.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.tarul.cn/Article/details/glzfnfzsk.sHtML

[R74] 批量重命名
来源：http://3g.vehdjk.com/Article/details/gdfhzemqm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.yfazqb.com/Article/details/gcifvzzfx.sHtML

[R75] 导出环境变量
来源：http://m.share.vehdjk.com/Article/details/gdhtixudc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.epnwcf.com/Article/details/gsghtblqn.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/gqmbzvtzi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gcxcjfvzv.sHtML

[R77] 读取用户输入
来源：http://blog.bbcook.cn/Article/details/gjdvgetlp.sHtML

read -rp "请输入: " ans
来源：http://blog.bbcook.cn/Article/details/gaqbbioto.sHtML

[R78] 交互式菜单
来源：http://www.blog.epnwcf.com/Article/details/gdourauaq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fktsv.cn/Article/details/gytatwshv.sHtML

[R79] 解析命令行选项
来源：http://wap.tarul.cn/Article/details/gaehovxwv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.epnwcf.com/Article/details/gmbdljvim.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fktsv.cn/Article/details/gvznsxqoj.sHtML

time ./run.sh
来源：http://read.share.fktsv.cn/Article/details/gubkcufli.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxfwmdawd.sHtML

S. C / C++ 专题
来源：http://mobile.tarul.cn/Article/details/gaekfipvs.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gqoflcaid.sHtML

[S01] C：Hello World
来源：http://www.blog.tarul.cn/Article/details/gqniheoub.sHtML

#include <stdio.h>
来源：http://www.blog.vehdjk.com/Article/details/grdchtlrf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.vehdjk.com/Article/details/gwjqniasx.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.epnwcf.com/Article/details/gvfbjrhhz.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.epnwcf.com/Article/details/glfikvlcx.sHtML

[S03] C：读入整数
来源：http://baike.bbcook.cn/Article/details/gualyimfp.sHtML

int x; scanf("%d", &x);
来源：http://baike.tarul.cn/Article/details/gvzyxlsfv.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fktsv.cn/Article/details/ghnkxeaoz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.bbcook.cn/Article/details/ghovjykrq.sHtML

[S05] C：字符串长度
来源：http://baike.epnwcf.com/Article/details/gxxfqfboz.sHtML

strlen(s)
来源：http://www.blog.tarul.cn/Article/details/gdwokzhdp.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfayflgu.sHtML

strcmp(a, b) == 0
来源：http://mobile.bbcook.cn/Article/details/gcvclmxqw.sHtML

[S07] C：数组遍历求和
来源：http://blog.epnwcf.com/Article/details/gukakvelo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.vehdjk.com/Article/details/guyukzsly.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.sjlbkw.cn/Article/details/gfhlwansa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.epnwcf.com/Article/details/gqgdhegen.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fktsv.cn/Article/details/gadxelomt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.bbcook.cn/Article/details/gnllfyxxh.sHtML

[S10] C：指针与解引用
来源：http://m.share.epnwcf.com/Article/details/ghjlmtcwn.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.vehdjk.com/Article/details/gnpnbgpej.sHtML

[S11] C：逐行读文件
来源：http://blog.bbcook.cn/Article/details/giqamlyhe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.yfazqb.com/Article/details/gnbzezhcy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.sjlbkw.cn/Article/details/gnhffcccs.sHtML

fclose(f);
来源：http://baike.epnwcf.com/Article/details/gdfhsfzpj.sHtML

[S12] C：写文件
来源：http://wap.fktsv.cn/Article/details/gvckfnejd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.vehdjk.com/Article/details/gqntgqisy.sHtML

[S13] C：宏定义
来源：http://read.share.yfazqb.com/Article/details/gobfoziwx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.sjlbkw.cn/Article/details/gpsvatnwb.sHtML

[S14] C：枚举
来源：http://wap.yfazqb.com/Article/details/gfliskkcq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/guxavmyxy.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/gkylnetvy.sHtML

(double) a / b
来源：http://read.share.fktsv.cn/Article/details/ggryclktu.sHtML

[S16] C：位操作置位
来源：http://m.share.yfazqb.com/Article/details/gidwsvdjx.sHtML

x |= (1 << 3);
来源：http://read.share.yfazqb.com/Article/details/gtyefinre.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gywbvhict.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.bbcook.cn/Article/details/gtquxeara.sHtML

[S18] C：命令行参数
来源：http://baike.bbcook.cn/Article/details/glperhoiv.sHtML

int main(int argc, char **argv)
来源：http://wap.tarul.cn/Article/details/geyjonuvc.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/gpfusxgme.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gzeykstax.sHtML

[S20] C：二分查找
来源：http://read.share.bbcook.cn/Article/details/ggjpxcwvl.sHtML


<!-- 参考信息 -->