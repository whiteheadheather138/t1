代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.epnwcf.com/Article/details/gbjmonvuv.sHtML

[Q54] 清空表
来源：http://www.share.epnwcf.com/Article/details/gutsqewmo.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fktsv.cn/Article/details/gwdzkwfwb.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fktsv.cn/Article/details/geofzkmxr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gavfdnler.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.bbcook.cn/Article/details/gzlumojkk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.tarul.cn/Article/details/gijnoiswh.sHtML

[Q57] 行号
来源：http://www.blog.vehdjk.com/Article/details/gtnwxveno.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fktsv.cn/Article/details/gdhpkjmhi.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/ghwieoqfk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gkrjqzlfj.sHtML

[Q59] 分组内累计
来源：http://wap.fktsv.cn/Article/details/grjudtnam.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.tarul.cn/Article/details/gsxwcuovs.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.vehdjk.com/Article/details/gpwufiawh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/galfsyxtf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.vehdjk.com/Article/details/gqieczyis.sHtML

[Q61] 移动平均
来源：http://www.blog.fktsv.cn/Article/details/gpvzehwzp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gwuveodpk.sHtML

[Q62] 分组占比
来源：http://m.share.epnwcf.com/Article/details/gmrwnhvib.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gfdcgupfi.sHtML

[Q63] 开启事务
来源：http://www.blog.yfazqb.com/Article/details/gksulkcci.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.tarul.cn/Article/details/gxxhfwivp.sHtML

[Q64] 提交事务
来源：http://3g.tarul.cn/Article/details/gzibrzssv.sHtML

COMMIT;
来源：http://www.m.share.bbcook.cn/Article/details/gipzxyrab.sHtML

[Q65] 回滚事务
来源：http://read.share.epnwcf.com/Article/details/gksubtdsg.sHtML

ROLLBACK;
来源：http://www.share.yfazqb.com/Article/details/gyygplqoj.sHtML

[Q66] 行锁查询
来源：http://blog.sjlbkw.cn/Article/details/giepgadpk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fktsv.cn/Article/details/gblsyyqqz.sHtML

[Q67] 设置隔离级别
来源：http://www.share.epnwcf.com/Article/details/gcwdpzjvw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.tarul.cn/Article/details/gjbfdytyk.sHtML

[Q68] 保存点
来源：http://blog.bbcook.cn/Article/details/gxqcwathf.sHtML

SAVEPOINT sp1;
来源：http://mobile.sjlbkw.cn/Article/details/gwfpzfnto.sHtML

ROLLBACK TO sp1;
来源：http://www.share.epnwcf.com/Article/details/gdukyzjnj.sHtML

[Q69] 查看执行计划
来源：http://3g.yfazqb.com/Article/details/gfuzjxgca.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.epnwcf.com/Article/details/gakncxhmy.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/gmiibinhg.sHtML

ANALYZE TABLE users;
来源：http://m.share.bbcook.cn/Article/details/gcnbgxjiu.sHtML

[Q71] 查看建表语句
来源：http://www.share.sjlbkw.cn/Article/details/gbygxyxzs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.vehdjk.com/Article/details/gjkvetmxu.sHtML

[Q72] 查看索引
来源：http://www.blog.yfazqb.com/Article/details/gqqmponga.sHtML

SHOW INDEX FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/giznpctrd.sHtML

[Q73] 查看表状态
来源：http://www.blog.yfazqb.com/Article/details/gjepaiirz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gyidvifoq.sHtML

[Q74] 强制使用索引
来源：http://www.share.bbcook.cn/Article/details/grvgllegr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.bbcook.cn/Article/details/gqnqfuljo.sHtML

[Q75] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/guyeqytta.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/giadkysye.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.yfazqb.com/Article/details/gytowkrrj.sHtML

[Q76] 按天统计
来源：http://mobile.fktsv.cn/Article/details/gjjrcuzmd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.tarul.cn/Article/details/gqhbtqqrp.sHtML

[Q77] 时间加减
来源：http://read.share.tarul.cn/Article/details/gtdgfbchb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fktsv.cn/Article/details/gmnrxiroz.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/gravyhsyf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.tarul.cn/Article/details/gwrpxtdhv.sHtML

[Q79] 字符串拼接
来源：http://m.share.bbcook.cn/Article/details/gwzdfylrr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.yfazqb.com/Article/details/gtefgkpwn.sHtML

[Q80] 字符串截取
来源：http://baike.sjlbkw.cn/Article/details/goqdropig.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fktsv.cn/Article/details/grzcfvdgo.sHtML

[Q81] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/ggfciyocn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.tarul.cn/Article/details/gharohcvv.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.sjlbkw.cn/Article/details/gwwwrsoce.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gmqzugbve.sHtML

[Q83] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gwbjgplxd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gmofiiohy.sHtML

[Q84] 去除首尾空格
来源：http://baike.epnwcf.com/Article/details/gsgfqogos.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gbhxkfmzm.sHtML

[Q85] 数值取整
来源：http://read.share.tarul.cn/Article/details/gohilxpcr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fktsv.cn/Article/details/ghfjfhffr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/gxtdpauqn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.tarul.cn/Article/details/gvlaoiygh.sHtML

[Q87] JSON 字段做条件
来源：http://3g.vehdjk.com/Article/details/gwfxdipxg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fktsv.cn/Article/details/gcueuzaas.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.tarul.cn/Article/details/gyznfiifc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.epnwcf.com/Article/details/guqsyedoj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.epnwcf.com/Article/details/goyosczcj.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fktsv.cn/Article/details/gucdbijoi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.tarul.cn/Article/details/gqbxdjhdz.sHtML

[Q90] 生成序号列
来源：http://blog.yfazqb.com/Article/details/gbggoflst.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.vehdjk.com/Article/details/gepavntsy.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gmcjyfawy.sHtML

R. Bash 专题
来源：http://mobile.yfazqb.com/Article/details/gfcbxrugl.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghtonlqpl.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.epnwcf.com/Article/details/ghnyekxlo.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfyihasb.sHtML

set -euo pipefail
来源：http://read.share.tarul.cn/Article/details/gxrhqkbji.sHtML

[R02] 变量赋值与使用
来源：http://3g.sjlbkw.cn/Article/details/gjtrihoka.sHtML

name="Tom"; echo "$name"
来源：http://read.share.bbcook.cn/Article/details/gfdbrvest.sHtML

[R03] 只读变量
来源：http://www.share.epnwcf.com/Article/details/gxnrejupx.sHtML

readonly PI=3.14
来源：http://www.m.share.yfazqb.com/Article/details/gzjwievwh.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/gqrsvnaow.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.vehdjk.com/Article/details/gcqlmykbk.sHtML

[R05] 参数默认值
来源：http://www.blog.sjlbkw.cn/Article/details/gojijesmr.sHtML

name="${1:-default}"
来源：http://3g.fktsv.cn/Article/details/ghmgdsbgy.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gnehduruu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/ghbzqcaru.sHtML

[R07] if 判断文件
来源：http://m.share.epnwcf.com/Article/details/gevmxwlgt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fktsv.cn/Article/details/gssvpmzed.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/gqsigriil.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.tarul.cn/Article/details/ggmeqnsya.sHtML

[R09] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gkdkpgvbo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.tarul.cn/Article/details/gtidcmfrg.sHtML

[R10] 正则匹配
来源：http://www.share.yfazqb.com/Article/details/gwrntaywk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/gsuhriyfb.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/gplojhpmz.sHtML

case "$1" in
来源：http://www.share.bbcook.cn/Article/details/gmonhjwwd.sHtML

start) echo "启动" ;;
来源：http://read.share.epnwcf.com/Article/details/gcmdzoyjs.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.yfazqb.com/Article/details/geylycnzi.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fktsv.cn/Article/details/gghjjueqv.sHtML

esac
来源：http://read.share.fktsv.cn/Article/details/gbdwvtuoi.sHtML

[R12] for 遍历文件
来源：http://3g.yfazqb.com/Article/details/gphqfuiin.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gkstujkyi.sHtML

[R13] for 计数循环
来源：http://blog.epnwcf.com/Article/details/gdbzlndut.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gxyhbwiym.sHtML

[R14] C 风格 for
来源：http://www.m.share.bbcook.cn/Article/details/gshysjmim.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/glxzbykju.sHtML

[R15] while 逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/guxvpfcfd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.epnwcf.com/Article/details/grpxoszwc.sHtML

[R16] until 等待条件
来源：http://www.blog.epnwcf.com/Article/details/ggwrvuyva.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/gckexreto.sHtML

[R17] 数组定义与取值
来源：http://read.share.vehdjk.com/Article/details/gtahcandg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.yfazqb.com/Article/details/gofkbpsld.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/glgwpkegy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fktsv.cn/Article/details/gntxkzqil.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/gobhhrljw.sHtML

echo "${#arr[@]}"
来源：http://wap.bbcook.cn/Article/details/gmvtpotgs.sHtML

[R20] 关联数组（字典）
来源：http://mobile.vehdjk.com/Article/details/gnddypnll.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.tarul.cn/Article/details/gjilopmjz.sHtML

[R21] 字符串长度
来源：http://m.share.tarul.cn/Article/details/ghjpbsrva.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/geeuvntiq.sHtML

[R22] 截取子串
来源：http://baike.bbcook.cn/Article/details/gzvozgjyw.sHtML

echo "${s:0:5}"
来源：http://mobile.fktsv.cn/Article/details/gnyhmwzzp.sHtML

[R23] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gykdrqwsp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.vehdjk.com/Article/details/gluwxnuaw.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/glcgmnkdb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.tarul.cn/Article/details/gxuimyzss.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/gaqpkbsft.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.vehdjk.com/Article/details/guqnvtyeu.sHtML

[R26] 命令替换
来源：http://3g.yfazqb.com/Article/details/gvaqmdhbv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.yfazqb.com/Article/details/gtrdcihse.sHtML

[R27] 算术展开
来源：http://www.m.share.tarul.cn/Article/details/gplojwiwx.sHtML

echo $((1 + 2 * 3))
来源：http://baike.vehdjk.com/Article/details/gfsijizdd.sHtML

[R28] 浮点运算
来源：http://www.share.bbcook.cn/Article/details/gnoeqvcqv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/ggfhymakx.sHtML

[R29] 定义函数
来源：http://baike.vehdjk.com/Article/details/gbhcfycyh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fktsv.cn/Article/details/gvbqstnxb.sHtML

[R30] 函数返回状态码
来源：http://read.share.vehdjk.com/Article/details/gxprbrwsr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.tarul.cn/Article/details/gbtpanxbm.sHtML

[R31] 局部变量
来源：http://www.share.bbcook.cn/Article/details/gieexnafg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.epnwcf.com/Article/details/gafhzyqcn.sHtML

[R32] 参数个数校验
来源：http://m.share.vehdjk.com/Article/details/gtmvgfngm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gemdefqns.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fktsv.cn/Article/details/gtlbascow.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.bbcook.cn/Article/details/gocftrkxy.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/goxbpnhtu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/glmwacbkb.sHtML

[R35] 后台执行并等待
来源：http://wap.vehdjk.com/Article/details/gvrdwclfm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.epnwcf.com/Article/details/gyjzttvyn.sHtML

[R36] 并发执行多个任务
来源：http://blog.tarul.cn/Article/details/gettlfwwe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.tarul.cn/Article/details/gompspjze.sHtML

[R37] 把输出赋给变量
来源：http://wap.vehdjk.com/Article/details/gecgwdhdt.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/gmjobxsps.sHtML

[R38] 管道串联
来源：http://www.blog.yfazqb.com/Article/details/gyrjstbds.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.sjlbkw.cn/Article/details/gakukukcx.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/gvhudmuat.sHtML

cmd > out.log 2>&1
来源：http://3g.tarul.cn/Article/details/gqhwhweeq.sHtML

[R40] 追加写日志
来源：http://read.share.epnwcf.com/Article/details/grxbwuqcx.sHtML

echo "log" >> out.log
来源：http://m.share.sjlbkw.cn/Article/details/gjtoxheiz.sHtML

[R41] 丢弃输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvabnbqh.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gsikhcvrw.sHtML

[R42] 输入重定向
来源：http://www.share.bbcook.cn/Article/details/gkccajcvd.sHtML

wc -l < a.txt
来源：http://m.share.yfazqb.com/Article/details/giwlpcczm.sHtML

[R43] 按名字查找文件
来源：http://m.share.yfazqb.com/Article/details/gtvexuiul.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fktsv.cn/Article/details/gbchwueby.sHtML

[R44] 按修改时间查找
来源：http://read.share.bbcook.cn/Article/details/gljposkca.sHtML

find . -mtime -7 -type f
来源：http://baike.epnwcf.com/Article/details/gagcomuuz.sHtML

[R45] 批量删除
来源：http://baike.epnwcf.com/Article/details/gvhpywmhn.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.tarul.cn/Article/details/gqrdubmfh.sHtML

[R46] 递归替换文件内容
来源：http://wap.bbcook.cn/Article/details/gsozjtgcl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.bbcook.cn/Article/details/gywwukptd.sHtML

[R47] sed 单行替换
来源：http://blog.fktsv.cn/Article/details/gufoamadj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.epnwcf.com/Article/details/gxtfqxlti.sHtML

[R48] awk 取指定列
来源：http://www.m.share.bbcook.cn/Article/details/guwkowlsk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gyomdfmxw.sHtML

[R49] awk 带条件
来源：http://www.share.vehdjk.com/Article/details/gaxaynhci.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.bbcook.cn/Article/details/gtaeegiuh.sHtML

[R50] awk 求和
来源：http://read.share.fktsv.cn/Article/details/gcyoptehy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.bbcook.cn/Article/details/gwswpqdsx.sHtML

[R51] 排序去重取前几
来源：http://blog.yfazqb.com/Article/details/gzizsliur.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.yfazqb.com/Article/details/ghdnmyjot.sHtML

[R52] 统计行数
来源：http://baike.yfazqb.com/Article/details/ggoqummgc.sHtML

wc -l a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrpxucft.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.epnwcf.com/Article/details/gdrczdhww.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.vehdjk.com/Article/details/ggzgzalfb.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/gqhrbxxnm.sHtML

diff a.txt b.txt
来源：http://blog.vehdjk.com/Article/details/gnxdezpyt.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fktsv.cn/Article/details/gyuxcdujx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.bbcook.cn/Article/details/gxbodjxsy.sHtML

[R56] 远程拷贝
来源：http://3g.yfazqb.com/Article/details/ggrucpfce.sHtML

scp file user@host:/path/
来源：http://wap.sjlbkw.cn/Article/details/gaqgdkrhf.sHtML

[R57] 远程执行命令
来源：http://www.share.sjlbkw.cn/Article/details/gsejfrgmm.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmgyylkg.sHtML

[R58] 下载文件
来源：http://mobile.tarul.cn/Article/details/gibeppxzj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fktsv.cn/Article/details/gwhoiodyh.sHtML

[R59] 发 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gspkklucj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/gnielcuka.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/gpsufspeh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.yfazqb.com/Article/details/gbwbgwugg.sHtML

[R61] 磁盘占用
来源：http://www.blog.vehdjk.com/Article/details/gqhtjnjwl.sHtML

df -h;  du -sh *
来源：http://www.blog.yfazqb.com/Article/details/gajutdeiy.sHtML

[R62] 找最占空间的文件
来源：http://www.share.sjlbkw.cn/Article/details/gnmbbrtmw.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.vehdjk.com/Article/details/gddfnotwj.sHtML

[R63] 内存与进程
来源：http://blog.vehdjk.com/Article/details/golydypea.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.yfazqb.com/Article/details/gypsceahy.sHtML

[R64] 结束进程
来源：http://www.blog.yfazqb.com/Article/details/gfonthqqu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fktsv.cn/Article/details/gaqrocecr.sHtML

[R65] 查看端口占用
来源：http://mobile.yfazqb.com/Article/details/gnuccqxud.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gckcsxhvi.sHtML

[R66] 定时任务
来源：http://m.share.sjlbkw.cn/Article/details/glhtleylw.sHtML

crontab -e;  crontab -l
来源：http://blog.vehdjk.com/Article/details/gzivpbvuw.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.epnwcf.com/Article/details/gvwpdylpk.sHtML

openssl rand -hex 16
来源：http://www.blog.yfazqb.com/Article/details/gbwfokmcg.sHtML

[R68] 计算文件校验值
来源：http://blog.tarul.cn/Article/details/gtomasqgl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.vehdjk.com/Article/details/gfvrdmwtv.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/gmeeogdlr.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.yfazqb.com/Article/details/gufatcuts.sHtML

[R70] 时间戳与互转
来源：http://baike.yfazqb.com/Article/details/gnwbwzcvb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/gdctncjkb.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gmpqqkoth.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gyijovnzu.sHtML

[R72] 等待端口就绪
来源：http://mobile.vehdjk.com/Article/details/gogwfhmyb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/grvwhafnr.sHtML

[R73] 分割大日志
来源：http://www.m.share.vehdjk.com/Article/details/gnweipkzq.sHtML

split -l 1000 big.log part_
来源：http://www.blog.epnwcf.com/Article/details/ggklmtyia.sHtML

[R74] 批量重命名
来源：http://read.share.tarul.cn/Article/details/gazhpksxn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.bbcook.cn/Article/details/gbqamsnak.sHtML

[R75] 导出环境变量
来源：http://m.share.tarul.cn/Article/details/gesxjzoui.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fktsv.cn/Article/details/gbilkkqxs.sHtML

[R76] 使用临时文件
来源：http://mobile.fktsv.cn/Article/details/gitbhnuqc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gzdyghmhe.sHtML

[R77] 读取用户输入
来源：http://baike.fktsv.cn/Article/details/gmdfapxoc.sHtML

read -rp "请输入: " ans
来源：http://blog.epnwcf.com/Article/details/gqpmnjhsd.sHtML

[R78] 交互式菜单
来源：http://m.share.bbcook.cn/Article/details/gumohdbnr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.tarul.cn/Article/details/gttaurosk.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fktsv.cn/Article/details/gadinywbb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.bbcook.cn/Article/details/gyxxgaclo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.bbcook.cn/Article/details/glenqawbo.sHtML

time ./run.sh
来源：http://3g.tarul.cn/Article/details/giysxubmw.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gicbkpzpa.sHtML

S. C / C++ 专题
来源：http://www.blog.yfazqb.com/Article/details/gjbmkbezx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsqormniv.sHtML

[S01] C：Hello World
来源：http://read.share.fktsv.cn/Article/details/gbxxsmqwg.sHtML

#include <stdio.h>
来源：http://wap.vehdjk.com/Article/details/gewathghj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.tarul.cn/Article/details/gcpohotdo.sHtML

[S02] C：变量与格式化输出
来源：http://blog.bbcook.cn/Article/details/gnfoxktzc.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/gyxnfcqbs.sHtML

[S03] C：读入整数
来源：http://www.share.yfazqb.com/Article/details/gjwrittri.sHtML

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/gxsysjkes.sHtML

[S04] C：字符串复制
来源：http://m.share.fktsv.cn/Article/details/gvmwpcuzc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fktsv.cn/Article/details/gudhpynfi.sHtML

[S05] C：字符串长度
来源：http://wap.tarul.cn/Article/details/gnegmstfp.sHtML

strlen(s)
来源：http://wap.fktsv.cn/Article/details/gqrmsqqgf.sHtML

[S06] C：字符串比较
来源：http://baike.bbcook.cn/Article/details/gtjjunziu.sHtML

strcmp(a, b) == 0
来源：http://read.share.bbcook.cn/Article/details/gmflujwhd.sHtML

[S07] C：数组遍历求和
来源：http://3g.vehdjk.com/Article/details/gosnkqlkz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fktsv.cn/Article/details/gzrvzxwno.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.tarul.cn/Article/details/gvnwsompc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.sjlbkw.cn/Article/details/gdqsmjsir.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.tarul.cn/Article/details/gdrfcxcos.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.epnwcf.com/Article/details/gahxeawdi.sHtML

[S10] C：指针与解引用
来源：http://read.share.yfazqb.com/Article/details/gpoiorgiy.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fktsv.cn/Article/details/gtzhjwxlj.sHtML

[S11] C：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gekgjiahw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.bbcook.cn/Article/details/gktulgfap.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.vehdjk.com/Article/details/gcvulneid.sHtML

fclose(f);
来源：http://baike.epnwcf.com/Article/details/gdzkjfddl.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzssfiot.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fktsv.cn/Article/details/gvoemtevz.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/gqehipfhr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.yfazqb.com/Article/details/gnbyiyraj.sHtML

[S14] C：枚举
来源：http://www.blog.epnwcf.com/Article/details/gszzhxxhy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.bbcook.cn/Article/details/gumvtnyif.sHtML

[S15] C：类型转换
来源：http://3g.fktsv.cn/Article/details/gkgrbyacc.sHtML

(double) a / b
来源：http://baike.tarul.cn/Article/details/gpzervpcu.sHtML

[S16] C：位操作置位
来源：http://baike.epnwcf.com/Article/details/gtkshjywl.sHtML

x |= (1 << 3);
来源：http://m.share.epnwcf.com/Article/details/goamytrgf.sHtML

[S17] C：安全拼接字符串
来源：http://blog.epnwcf.com/Article/details/gcsqyrylu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fktsv.cn/Article/details/grzxelvyk.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/grczkwplx.sHtML

int main(int argc, char **argv)
来源：http://read.share.epnwcf.com/Article/details/gwcyuhzyd.sHtML

[S19] C：快速排序
来源：http://m.share.sjlbkw.cn/Article/details/gnxgvtdxx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/gqyayezvw.sHtML

[S20] C：二分查找
来源：http://m.share.fktsv.cn/Article/details/gbvlmqehp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gqfolusll.sHtML

[S21] C：字符类别判断
来源：http://blog.epnwcf.com/Article/details/gxrtlyaxf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.epnwcf.com/Article/details/gkgwgxuyb.sHtML

[S22] C：字符串转数字
来源：http://www.blog.tarul.cn/Article/details/glunvurdt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.tarul.cn/Article/details/gsxdflhyz.sHtML

[S23] C：随机数
来源：http://read.share.yfazqb.com/Article/details/gdqbrjuoe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.vehdjk.com/Article/details/gebwojgjp.sHtML

[S24] C：获取本地时间
来源：http://wap.tarul.cn/Article/details/gehtjdsyl.sHtML


<!-- 参考信息 -->