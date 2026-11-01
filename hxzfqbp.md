代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/gsjxqlrft.sHtML

[Q52] 删除指定行
来源：http://mobile.fktsv.cn/Article/details/giejwprtg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gaknshhdq.sHtML

[Q53] 按条件删除
来源：http://www.m.share.epnwcf.com/Article/details/ggprmolvp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fktsv.cn/Article/details/gahxpnxmv.sHtML

[Q54] 清空表
来源：http://m.share.bbcook.cn/Article/details/gpwifhlji.sHtML

TRUNCATE TABLE logs;
来源：http://baike.yfazqb.com/Article/details/gjkhcspqq.sHtML

[Q55] 排名（并列占位）
来源：http://3g.yfazqb.com/Article/details/guzhsdrqw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.tarul.cn/Article/details/ghxfestto.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.vehdjk.com/Article/details/gaztdundc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.tarul.cn/Article/details/gyknqzcps.sHtML

[Q57] 行号
来源：http://m.share.vehdjk.com/Article/details/gysqnlrty.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.vehdjk.com/Article/details/gwrqstkay.sHtML

[Q58] 累计求和
来源：http://baike.tarul.cn/Article/details/gdvrwbgki.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gxtafhgxo.sHtML

[Q59] 分组内累计
来源：http://wap.sjlbkw.cn/Article/details/gssddptaj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gvmqfgafr.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.bbcook.cn/Article/details/gqooiypzn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.yfazqb.com/Article/details/giybhierq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gffhoyldn.sHtML

[Q61] 移动平均
来源：http://www.blog.sjlbkw.cn/Article/details/gqflkabrn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/goftafljl.sHtML

[Q62] 分组占比
来源：http://blog.fktsv.cn/Article/details/gshpfqnec.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/geyiwmseg.sHtML

[Q63] 开启事务
来源：http://read.share.epnwcf.com/Article/details/glujlbgvf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.tarul.cn/Article/details/ghehvotrx.sHtML

[Q64] 提交事务
来源：http://mobile.fktsv.cn/Article/details/gxxfggwmm.sHtML

COMMIT;
来源：http://mobile.epnwcf.com/Article/details/ginajuchn.sHtML

[Q65] 回滚事务
来源：http://wap.sjlbkw.cn/Article/details/gsfprnvjq.sHtML

ROLLBACK;
来源：http://3g.tarul.cn/Article/details/gjdynahqx.sHtML

[Q66] 行锁查询
来源：http://www.blog.tarul.cn/Article/details/ggxoadvum.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fktsv.cn/Article/details/gahqpnecj.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.tarul.cn/Article/details/gdmyzjrxy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.yfazqb.com/Article/details/glfctnmdq.sHtML

[Q68] 保存点
来源：http://www.share.tarul.cn/Article/details/gocyzspqb.sHtML

SAVEPOINT sp1;
来源：http://mobile.tarul.cn/Article/details/goqrgdefj.sHtML

ROLLBACK TO sp1;
来源：http://3g.vehdjk.com/Article/details/gkajrvjgu.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gelqnpisn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.vehdjk.com/Article/details/gydczubqj.sHtML

[Q70] 更新统计信息
来源：http://m.share.fktsv.cn/Article/details/gbhtsbyzt.sHtML

ANALYZE TABLE users;
来源：http://3g.tarul.cn/Article/details/gabofqlzf.sHtML

[Q71] 查看建表语句
来源：http://www.share.bbcook.cn/Article/details/geqbhxdfq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.yfazqb.com/Article/details/gpqrkvple.sHtML

[Q72] 查看索引
来源：http://www.share.vehdjk.com/Article/details/ggqrljnwz.sHtML

SHOW INDEX FROM users;
来源：http://wap.fktsv.cn/Article/details/ggilaziva.sHtML

[Q73] 查看表状态
来源：http://www.blog.tarul.cn/Article/details/gnobbqdpz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.sjlbkw.cn/Article/details/gnbaykewn.sHtML

[Q74] 强制使用索引
来源：http://blog.tarul.cn/Article/details/giqcghklk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.yfazqb.com/Article/details/geenyjaid.sHtML

[Q75] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gshdshewt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gfmkirsxn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.vehdjk.com/Article/details/galakukhe.sHtML

[Q76] 按天统计
来源：http://wap.tarul.cn/Article/details/ghprtycyt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/gfohqrjzx.sHtML

[Q77] 时间加减
来源：http://read.share.bbcook.cn/Article/details/grdcdwrjp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.bbcook.cn/Article/details/gifkzkzfm.sHtML

[Q78] 当前时间
来源：http://blog.epnwcf.com/Article/details/gvdzgxzmb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.epnwcf.com/Article/details/gifvlakli.sHtML

[Q79] 字符串拼接
来源：http://read.share.epnwcf.com/Article/details/ghlaxzmtj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.bbcook.cn/Article/details/gftdtskgr.sHtML

[Q80] 字符串截取
来源：http://m.share.epnwcf.com/Article/details/gvflfrljh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.tarul.cn/Article/details/ghuwoxean.sHtML

[Q81] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gludfgocl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fktsv.cn/Article/details/gzymgmlxi.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.sjlbkw.cn/Article/details/gatviufbv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gvkaysztj.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gkfrrzsoj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gcaqqeygm.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fktsv.cn/Article/details/grtrtzcui.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gkcgwuakc.sHtML

[Q85] 数值取整
来源：http://www.share.bbcook.cn/Article/details/gnwizoemx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.bbcook.cn/Article/details/gzbfeqanm.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.sjlbkw.cn/Article/details/gjssqogcg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.yfazqb.com/Article/details/gfyjjdaja.sHtML

[Q87] JSON 字段做条件
来源：http://wap.bbcook.cn/Article/details/gfaaqfhsi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/gwhjfpbbz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.epnwcf.com/Article/details/gsmiuddcg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.vehdjk.com/Article/details/gacdtcivn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.vehdjk.com/Article/details/gxsqlhblt.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.tarul.cn/Article/details/gwfbrjrsc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.epnwcf.com/Article/details/gdwrvtfad.sHtML

[Q90] 生成序号列
来源：http://read.share.yfazqb.com/Article/details/ghutcafuy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.tarul.cn/Article/details/guflvtskr.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gctogzjcy.sHtML

R. Bash 专题
来源：http://blog.sjlbkw.cn/Article/details/gfrqspqnv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmoxtgkxy.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.vehdjk.com/Article/details/ggudsiidd.sHtML

#!/usr/bin/env bash
来源：http://read.share.epnwcf.com/Article/details/gxxoajcaj.sHtML

set -euo pipefail
来源：http://read.share.vehdjk.com/Article/details/gkfoffgde.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.bbcook.cn/Article/details/gmmugbyps.sHtML

name="Tom"; echo "$name"
来源：http://read.share.vehdjk.com/Article/details/gszeablye.sHtML

[R03] 只读变量
来源：http://m.share.tarul.cn/Article/details/gdhepjmln.sHtML

readonly PI=3.14
来源：http://www.share.vehdjk.com/Article/details/gzibroqiw.sHtML

[R04] 位置参数
来源：http://www.share.bbcook.cn/Article/details/goxexhfwl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.bbcook.cn/Article/details/gyvgpvvoa.sHtML

[R05] 参数默认值
来源：http://baike.bbcook.cn/Article/details/geixgyfms.sHtML

name="${1:-default}"
来源：http://3g.epnwcf.com/Article/details/gbwrdummf.sHtML

[R06] 判断命令是否存在
来源：http://wap.sjlbkw.cn/Article/details/ggnpmxybn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gjgjrsrdh.sHtML

[R07] if 判断文件
来源：http://baike.tarul.cn/Article/details/gpzrzblxs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fktsv.cn/Article/details/gpkvquxdd.sHtML

[R08] 数值比较
来源：http://baike.vehdjk.com/Article/details/gjvpcigkz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.epnwcf.com/Article/details/gvayzqvhx.sHtML

[R09] 字符串比较
来源：http://m.share.fktsv.cn/Article/details/gqnbxirvb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.vehdjk.com/Article/details/guenevgcc.sHtML

[R10] 正则匹配
来源：http://3g.sjlbkw.cn/Article/details/gafxajtrz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.tarul.cn/Article/details/ghxstoohi.sHtML

[R11] case 多分支
来源：http://baike.fktsv.cn/Article/details/geljgaghf.sHtML

case "$1" in
来源：http://3g.epnwcf.com/Article/details/gbnqqlcnc.sHtML

start) echo "启动" ;;
来源：http://blog.yfazqb.com/Article/details/gcjzthefj.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.epnwcf.com/Article/details/gmldogkvx.sHtML

*)     echo "未知命令" ;;
来源：http://3g.yfazqb.com/Article/details/gpkzdatdu.sHtML

esac
来源：http://wap.vehdjk.com/Article/details/gfgrvietq.sHtML

[R12] for 遍历文件
来源：http://www.share.epnwcf.com/Article/details/gspuilfoi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/gdryhnisx.sHtML

[R13] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/ghyntcemi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gzxygmxdl.sHtML

[R14] C 风格 for
来源：http://blog.fktsv.cn/Article/details/gdlxxjrhd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/glwdjirtp.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/givxlruei.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.tarul.cn/Article/details/gfagxhjng.sHtML

[R16] until 等待条件
来源：http://mobile.yfazqb.com/Article/details/gjuwowlbj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gjbqjofdw.sHtML

[R17] 数组定义与取值
来源：http://www.share.epnwcf.com/Article/details/gpogihkvw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.epnwcf.com/Article/details/gtysynrvs.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/ggpwyibym.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.tarul.cn/Article/details/gmtdsokch.sHtML

[R19] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gsfljavkl.sHtML

echo "${#arr[@]}"
来源：http://mobile.tarul.cn/Article/details/gobemanmm.sHtML

[R20] 关联数组（字典）
来源：http://mobile.sjlbkw.cn/Article/details/gfxjqetbh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.bbcook.cn/Article/details/gltekvhqo.sHtML

[R21] 字符串长度
来源：http://blog.epnwcf.com/Article/details/gyivxkkhw.sHtML

echo "${#s}"
来源：http://www.share.bbcook.cn/Article/details/grxlbooyf.sHtML

[R22] 截取子串
来源：http://www.m.share.yfazqb.com/Article/details/gzryyruxo.sHtML

echo "${s:0:5}"
来源：http://wap.vehdjk.com/Article/details/gfhuhthmk.sHtML

[R23] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/gykitxtif.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.yfazqb.com/Article/details/gqmoabrua.sHtML

[R24] 大小写转换
来源：http://wap.yfazqb.com/Article/details/gcdulvaxe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.vehdjk.com/Article/details/gsiapxhpo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.epnwcf.com/Article/details/ghziylqnr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.tarul.cn/Article/details/gbivzgudn.sHtML

[R26] 命令替换
来源：http://3g.epnwcf.com/Article/details/gvrozfozf.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.vehdjk.com/Article/details/gnabuqeac.sHtML

[R27] 算术展开
来源：http://www.m.share.sjlbkw.cn/Article/details/gwasaeubp.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.yfazqb.com/Article/details/gyfcnlpzt.sHtML

[R28] 浮点运算
来源：http://mobile.tarul.cn/Article/details/gscypbyha.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.tarul.cn/Article/details/gbsmnyzgk.sHtML

[R29] 定义函数
来源：http://blog.epnwcf.com/Article/details/gyioviksp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.yfazqb.com/Article/details/gyeemmcrk.sHtML

[R30] 函数返回状态码
来源：http://wap.yfazqb.com/Article/details/gmbomzrye.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.sjlbkw.cn/Article/details/gbnbkirvu.sHtML

[R31] 局部变量
来源：http://www.m.share.bbcook.cn/Article/details/gwfejdwxa.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.yfazqb.com/Article/details/gdmrmrpvd.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/gdjnlebqh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gwsukfryx.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.bbcook.cn/Article/details/gnssttcmg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.bbcook.cn/Article/details/gekcebrgz.sHtML

[R34] 退出时清理
来源：http://3g.bbcook.cn/Article/details/gnkxovrvq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/glbcvioju.sHtML

[R35] 后台执行并等待
来源：http://www.share.yfazqb.com/Article/details/gfuxjrino.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.yfazqb.com/Article/details/gxkbucvbn.sHtML

[R36] 并发执行多个任务
来源：http://read.share.yfazqb.com/Article/details/gnaalrrcc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/gzedvocyk.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.vehdjk.com/Article/details/gwhpfvnxq.sHtML

files=$(ls -1)
来源：http://www.m.share.fktsv.cn/Article/details/gwvjvekid.sHtML

[R38] 管道串联
来源：http://www.blog.sjlbkw.cn/Article/details/gqputbook.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.epnwcf.com/Article/details/guahcbolq.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.bbcook.cn/Article/details/gnwfsmtlk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gxqqdseiy.sHtML

[R40] 追加写日志
来源：http://wap.sjlbkw.cn/Article/details/gyaxrqcmt.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/gpocpqmtz.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/gvcggyvqd.sHtML

cmd >/dev/null 2>&1
来源：http://blog.vehdjk.com/Article/details/gwwgqmryc.sHtML

[R42] 输入重定向
来源：http://m.share.fktsv.cn/Article/details/gxfkcwhzi.sHtML

wc -l < a.txt
来源：http://www.m.share.tarul.cn/Article/details/grajtpnzs.sHtML

[R43] 按名字查找文件
来源：http://3g.epnwcf.com/Article/details/ggsrxgqye.sHtML

find . -name "*.log" -type f
来源：http://m.share.fktsv.cn/Article/details/ginsdvwcs.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.epnwcf.com/Article/details/gnaqaqpar.sHtML

find . -mtime -7 -type f
来源：http://www.share.fktsv.cn/Article/details/ghwbxrmke.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/gwejzztlu.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.yfazqb.com/Article/details/gopjzgqns.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gmvjqilje.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.yfazqb.com/Article/details/gbxdutvfq.sHtML

[R47] sed 单行替换
来源：http://read.share.sjlbkw.cn/Article/details/gyimrgkph.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gcpdunlgz.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/gzhvspqac.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gxsezbmym.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/gfudsmbow.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.yfazqb.com/Article/details/gapmsihie.sHtML

[R50] awk 求和
来源：http://www.m.share.tarul.cn/Article/details/gurkiiaqg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gaabvmynv.sHtML

[R51] 排序去重取前几
来源：http://wap.epnwcf.com/Article/details/glgftqubr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.yfazqb.com/Article/details/gjdjvckmd.sHtML

[R52] 统计行数
来源：http://wap.fktsv.cn/Article/details/gpfsompog.sHtML

wc -l a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gykdbbrag.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.sjlbkw.cn/Article/details/gvcxvjmhs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.yfazqb.com/Article/details/gtnksnjmv.sHtML

[R54] 比较两个文件
来源：http://m.share.tarul.cn/Article/details/gdyndamux.sHtML

diff a.txt b.txt
来源：http://3g.yfazqb.com/Article/details/gdypciiqx.sHtML

[R55] 压缩与解压
来源：http://3g.epnwcf.com/Article/details/gvgadhbtc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.yfazqb.com/Article/details/giwjppnar.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/gnfdulcpu.sHtML

scp file user@host:/path/
来源：http://www.share.sjlbkw.cn/Article/details/gngxovgkg.sHtML

[R57] 远程执行命令
来源：http://baike.vehdjk.com/Article/details/ggofkvpag.sHtML

ssh user@host 'uptime'
来源：http://mobile.sjlbkw.cn/Article/details/gihptmzlq.sHtML

[R58] 下载文件
来源：http://www.blog.vehdjk.com/Article/details/gomszkjfy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fktsv.cn/Article/details/gtnmzktcg.sHtML

[R59] 发 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/glrloszne.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.sjlbkw.cn/Article/details/gneqgymkz.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/gougtbkkz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.yfazqb.com/Article/details/gxsblhikc.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/gpmtvthpr.sHtML

df -h;  du -sh *
来源：http://3g.yfazqb.com/Article/details/gmygagdkn.sHtML

[R62] 找最占空间的文件
来源：http://wap.yfazqb.com/Article/details/ghhylrese.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/gfyvefwqc.sHtML

[R63] 内存与进程
来源：http://www.blog.yfazqb.com/Article/details/gnkaolfrt.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.bbcook.cn/Article/details/gzbxhcwmy.sHtML

[R64] 结束进程
来源：http://www.share.sjlbkw.cn/Article/details/ggkrctwrw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.sjlbkw.cn/Article/details/gmmdccbzp.sHtML

[R65] 查看端口占用
来源：http://read.share.fktsv.cn/Article/details/gszvaswio.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fktsv.cn/Article/details/ggwjdyaoc.sHtML

[R66] 定时任务
来源：http://3g.epnwcf.com/Article/details/gtbdatcrd.sHtML

crontab -e;  crontab -l
来源：http://3g.tarul.cn/Article/details/glkcdiwez.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fktsv.cn/Article/details/gbkgjkfep.sHtML

openssl rand -hex 16
来源：http://baike.fktsv.cn/Article/details/gktqmddpw.sHtML

[R68] 计算文件校验值
来源：http://www.blog.bbcook.cn/Article/details/gnstnerqp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.tarul.cn/Article/details/gmrruzrbi.sHtML

[R69] 生成随机密码
来源：http://www.blog.vehdjk.com/Article/details/getplirno.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.yfazqb.com/Article/details/grjbfjvir.sHtML

[R70] 时间戳与互转
来源：http://mobile.bbcook.cn/Article/details/gkgcpsqvv.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.tarul.cn/Article/details/gmzgwcxep.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gpzjsrxcc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fktsv.cn/Article/details/gthdfhvap.sHtML

[R72] 等待端口就绪
来源：http://m.share.tarul.cn/Article/details/glqlmtcxf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/gipgccocw.sHtML

[R73] 分割大日志
来源：http://baike.sjlbkw.cn/Article/details/ghldyykcs.sHtML

split -l 1000 big.log part_
来源：http://www.share.yfazqb.com/Article/details/gktopovtk.sHtML

[R74] 批量重命名
来源：http://mobile.tarul.cn/Article/details/gnouadzcr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/gcgkfjkes.sHtML

[R75] 导出环境变量
来源：http://www.share.tarul.cn/Article/details/gvbknbyao.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.yfazqb.com/Article/details/gzvklkfrv.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/gighmshjq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/ghegowlcm.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/ggmvmndcv.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/gpypzfypb.sHtML

[R78] 交互式菜单
来源：http://blog.fktsv.cn/Article/details/gldpxmexq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/gojetzamm.sHtML

[R79] 解析命令行选项
来源：http://mobile.yfazqb.com/Article/details/ghooxpfck.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.tarul.cn/Article/details/gfjhmapqh.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.tarul.cn/Article/details/gyrfuorom.sHtML

time ./run.sh
来源：http://blog.yfazqb.com/Article/details/gwfzdlnru.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmeciyfsw.sHtML

S. C / C++ 专题
来源：http://baike.fktsv.cn/Article/details/gikhyrphc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/glxmpfgxi.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/ganypouwv.sHtML

#include <stdio.h>
来源：http://read.share.sjlbkw.cn/Article/details/gcwsperad.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.tarul.cn/Article/details/gbkzqbbxv.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.tarul.cn/Article/details/gasazrqct.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fktsv.cn/Article/details/gnyghgvwt.sHtML

[S03] C：读入整数
来源：http://www.share.vehdjk.com/Article/details/ghqmyxfnq.sHtML

int x; scanf("%d", &x);
来源：http://read.share.sjlbkw.cn/Article/details/gybipwcwd.sHtML

[S04] C：字符串复制
来源：http://3g.epnwcf.com/Article/details/gwdvtrebc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/gidwrpscn.sHtML

[S05] C：字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gjojeflqm.sHtML

strlen(s)
来源：http://3g.tarul.cn/Article/details/gsjvsrggy.sHtML

[S06] C：字符串比较
来源：http://mobile.fktsv.cn/Article/details/gbvyzlxgq.sHtML

strcmp(a, b) == 0
来源：http://blog.epnwcf.com/Article/details/ggjgugsvs.sHtML

[S07] C：数组遍历求和
来源：http://3g.bbcook.cn/Article/details/ggdydzrpw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.yfazqb.com/Article/details/gktrkwkmu.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.bbcook.cn/Article/details/gucolqnoe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.epnwcf.com/Article/details/gpkqezbqf.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.sjlbkw.cn/Article/details/guptfucdg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.bbcook.cn/Article/details/guviktyuj.sHtML

[S10] C：指针与解引用
来源：http://blog.yfazqb.com/Article/details/gggllqwon.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/gdstytkld.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gqzyegpkk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.epnwcf.com/Article/details/gwioezkxc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.sjlbkw.cn/Article/details/gvqnyvtly.sHtML

fclose(f);
来源：http://blog.fktsv.cn/Article/details/gwttjwvne.sHtML

[S12] C：写文件
来源：http://mobile.tarul.cn/Article/details/ghrmtvhhh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.vehdjk.com/Article/details/gvgbjsgvv.sHtML

[S13] C：宏定义
来源：http://www.share.yfazqb.com/Article/details/gttigvmyc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fktsv.cn/Article/details/gzzeiwkzw.sHtML

[S14] C：枚举
来源：http://wap.yfazqb.com/Article/details/giuxbmjnn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.epnwcf.com/Article/details/gxczyzngo.sHtML

[S15] C：类型转换
来源：http://mobile.epnwcf.com/Article/details/gudlxkaqp.sHtML

(double) a / b
来源：http://3g.epnwcf.com/Article/details/gcionyeic.sHtML

[S16] C：位操作置位
来源：http://www.m.share.bbcook.cn/Article/details/gaarhtmyf.sHtML

x |= (1 << 3);
来源：http://m.share.yfazqb.com/Article/details/gbwolpcnr.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gosexzsif.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/gtgiljgsq.sHtML

[S18] C：命令行参数
来源：http://www.share.bbcook.cn/Article/details/gbbeopoco.sHtML

int main(int argc, char **argv)
来源：http://read.share.yfazqb.com/Article/details/gnxkmixvk.sHtML

[S19] C：快速排序
来源：http://m.share.fktsv.cn/Article/details/geagohohh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gnbpmdjeh.sHtML

[S20] C：二分查找
来源：http://m.share.epnwcf.com/Article/details/gczpaggby.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gfupwzcqq.sHtML

[S21] C：字符类别判断
来源：http://3g.bbcook.cn/Article/details/gygmxqimx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.bbcook.cn/Article/details/govmydnac.sHtML

[S22] C：字符串转数字
来源：http://blog.epnwcf.com/Article/details/gfswjnsak.sHtML


<!-- 参考信息 -->