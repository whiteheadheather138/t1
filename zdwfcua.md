代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.epnwcf.com/Article/details/gfbemgyyk.sHtML

[Q52] 删除指定行
来源：http://www.share.tarul.cn/Article/details/gjwegfvtb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.yfazqb.com/Article/details/goabeenjx.sHtML

[Q53] 按条件删除
来源：http://read.share.tarul.cn/Article/details/gzquulhcd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fktsv.cn/Article/details/gmhgucyqx.sHtML

[Q54] 清空表
来源：http://3g.fktsv.cn/Article/details/giblnitez.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/ghunifbsi.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.bbcook.cn/Article/details/ghtihbrtz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.epnwcf.com/Article/details/gvgznjmvi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.epnwcf.com/Article/details/gnmqjbdpw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gdxmmgqhd.sHtML

[Q57] 行号
来源：http://wap.bbcook.cn/Article/details/gdcuuyqgq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fktsv.cn/Article/details/gfnivargi.sHtML

[Q58] 累计求和
来源：http://baike.fktsv.cn/Article/details/gzkpttxkz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.vehdjk.com/Article/details/gcnooaifj.sHtML

[Q59] 分组内累计
来源：http://www.m.share.tarul.cn/Article/details/gulxvueaq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.bbcook.cn/Article/details/grrouhjxj.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.bbcook.cn/Article/details/grpcsawhg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.tarul.cn/Article/details/goawhwrpt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.vehdjk.com/Article/details/gytljnjub.sHtML

[Q61] 移动平均
来源：http://m.share.vehdjk.com/Article/details/ggrzqrzdg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gmuozazdg.sHtML

[Q62] 分组占比
来源：http://blog.sjlbkw.cn/Article/details/gujxcfras.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/ggsipfhxp.sHtML

[Q63] 开启事务
来源：http://mobile.sjlbkw.cn/Article/details/gyruoqnlt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.epnwcf.com/Article/details/ggaicezfz.sHtML

[Q64] 提交事务
来源：http://blog.vehdjk.com/Article/details/gvyufkzry.sHtML

COMMIT;
来源：http://3g.yfazqb.com/Article/details/gdiizzvuf.sHtML

[Q65] 回滚事务
来源：http://mobile.bbcook.cn/Article/details/ggqysuygt.sHtML

ROLLBACK;
来源：http://www.m.share.vehdjk.com/Article/details/ggvkbvzjg.sHtML

[Q66] 行锁查询
来源：http://mobile.vehdjk.com/Article/details/gdhkokeqf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.vehdjk.com/Article/details/gjfcrpszz.sHtML

[Q67] 设置隔离级别
来源：http://mobile.bbcook.cn/Article/details/gxdtjygix.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.tarul.cn/Article/details/gyhgmrvue.sHtML

[Q68] 保存点
来源：http://read.share.yfazqb.com/Article/details/gbeaoqbsb.sHtML

SAVEPOINT sp1;
来源：http://wap.vehdjk.com/Article/details/guqzimjly.sHtML

ROLLBACK TO sp1;
来源：http://blog.sjlbkw.cn/Article/details/gpeooeltc.sHtML

[Q69] 查看执行计划
来源：http://baike.tarul.cn/Article/details/gxaptffdb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.tarul.cn/Article/details/guaxebvqw.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/glthdimwj.sHtML

ANALYZE TABLE users;
来源：http://m.share.sjlbkw.cn/Article/details/gfbazrecb.sHtML

[Q71] 查看建表语句
来源：http://www.share.tarul.cn/Article/details/gxxwnniel.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/gvjfxmlfc.sHtML

[Q72] 查看索引
来源：http://www.share.tarul.cn/Article/details/gkcnwponz.sHtML

SHOW INDEX FROM users;
来源：http://read.share.bbcook.cn/Article/details/gxieceydl.sHtML

[Q73] 查看表状态
来源：http://www.share.vehdjk.com/Article/details/glxqfkknv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.tarul.cn/Article/details/gpzezntmx.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.vehdjk.com/Article/details/gefvptdpu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.vehdjk.com/Article/details/gutedagio.sHtML

[Q75] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/gnvjgdhcu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fktsv.cn/Article/details/gpnmavseq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fktsv.cn/Article/details/gyyazweha.sHtML

[Q76] 按天统计
来源：http://www.m.share.epnwcf.com/Article/details/gdxjkhckv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.vehdjk.com/Article/details/gywruwfqa.sHtML

[Q77] 时间加减
来源：http://m.share.epnwcf.com/Article/details/gpawqowxf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.yfazqb.com/Article/details/gszztwsrf.sHtML

[Q78] 当前时间
来源：http://baike.bbcook.cn/Article/details/gofyzccsk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.sjlbkw.cn/Article/details/gkexmsbvb.sHtML

[Q79] 字符串拼接
来源：http://www.blog.yfazqb.com/Article/details/gefcuztwd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.epnwcf.com/Article/details/gzzclhrnq.sHtML

[Q80] 字符串截取
来源：http://wap.vehdjk.com/Article/details/goxajaeid.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.tarul.cn/Article/details/gbkvopzme.sHtML

[Q81] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/glwdbknar.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.vehdjk.com/Article/details/glpgfekui.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.bbcook.cn/Article/details/gppyiijwb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/ghtfawvxj.sHtML

[Q83] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/gcxmrsgtx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/glmakkmrg.sHtML

[Q84] 去除首尾空格
来源：http://read.share.bbcook.cn/Article/details/gltrrirml.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gsdlorwqe.sHtML

[Q85] 数值取整
来源：http://www.blog.fktsv.cn/Article/details/grqpigqgi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.yfazqb.com/Article/details/gwwhnmfkb.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.sjlbkw.cn/Article/details/gvqjkkdcc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.sjlbkw.cn/Article/details/gmxqxfonb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.epnwcf.com/Article/details/guwfljasz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.sjlbkw.cn/Article/details/gzutzixir.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.vehdjk.com/Article/details/gphdikruw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.vehdjk.com/Article/details/grltlzfph.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.tarul.cn/Article/details/gybuwunxd.sHtML

[Q89] 判断表是否存在
来源：http://mobile.tarul.cn/Article/details/gdzytdstr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gxiomuzfh.sHtML

[Q90] 生成序号列
来源：http://baike.tarul.cn/Article/details/gthxeujbz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.vehdjk.com/Article/details/gkszdeegp.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghlfjfurw.sHtML

R. Bash 专题
来源：http://blog.sjlbkw.cn/Article/details/garllpzel.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gobojzsev.sHtML

[R01] shebang 与严格模式
来源：http://m.share.tarul.cn/Article/details/gsrsiaowv.sHtML

#!/usr/bin/env bash
来源：http://wap.bbcook.cn/Article/details/gmzntazyn.sHtML

set -euo pipefail
来源：http://wap.yfazqb.com/Article/details/gkfupszdt.sHtML

[R02] 变量赋值与使用
来源：http://m.share.bbcook.cn/Article/details/gybugebnz.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gdzgwhynk.sHtML

[R03] 只读变量
来源：http://baike.bbcook.cn/Article/details/gqpryhkfx.sHtML

readonly PI=3.14
来源：http://3g.vehdjk.com/Article/details/ggrwbsimg.sHtML

[R04] 位置参数
来源：http://www.m.share.vehdjk.com/Article/details/gxoyqarxl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fktsv.cn/Article/details/gjdrpjyum.sHtML

[R05] 参数默认值
来源：http://wap.vehdjk.com/Article/details/gfxomltdo.sHtML

name="${1:-default}"
来源：http://wap.sjlbkw.cn/Article/details/gtxlrtcey.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gujxwzjtu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/ggmsgowne.sHtML

[R07] if 判断文件
来源：http://www.blog.yfazqb.com/Article/details/gdfpkvfql.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fktsv.cn/Article/details/gphdyokzg.sHtML

[R08] 数值比较
来源：http://www.m.share.vehdjk.com/Article/details/gegqjdvau.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.epnwcf.com/Article/details/ghwmbwbdz.sHtML

[R09] 字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gjxhqzogc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gkoqqopkd.sHtML

[R10] 正则匹配
来源：http://3g.vehdjk.com/Article/details/gtuiyhhmi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.sjlbkw.cn/Article/details/gbaoyasqu.sHtML

[R11] case 多分支
来源：http://www.blog.fktsv.cn/Article/details/gtlogmqrh.sHtML

case "$1" in
来源：http://www.blog.sjlbkw.cn/Article/details/gyctsqchq.sHtML

start) echo "启动" ;;
来源：http://read.share.epnwcf.com/Article/details/gqroylojq.sHtML

stop)  echo "停止" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gtubfctgt.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.vehdjk.com/Article/details/gplxzfjge.sHtML

esac
来源：http://m.share.fktsv.cn/Article/details/gctqnyjui.sHtML

[R12] for 遍历文件
来源：http://blog.epnwcf.com/Article/details/gasibpeov.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fktsv.cn/Article/details/gsxlposrc.sHtML

[R13] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/gnrstjhys.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gwvvtzjqs.sHtML

[R14] C 风格 for
来源：http://baike.tarul.cn/Article/details/gfhoglqaw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/gypizvcqb.sHtML

[R15] while 逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gxujofimd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.epnwcf.com/Article/details/gccujuace.sHtML

[R16] until 等待条件
来源：http://3g.fktsv.cn/Article/details/geywakcvv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gyvxymebg.sHtML

[R17] 数组定义与取值
来源：http://baike.tarul.cn/Article/details/gpfgqiovv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.vehdjk.com/Article/details/ghhzzoguc.sHtML

[R18] 遍历数组
来源：http://wap.yfazqb.com/Article/details/gsbdjkqim.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.vehdjk.com/Article/details/gtwkyeqak.sHtML

[R19] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/gfebbqyci.sHtML

echo "${#arr[@]}"
来源：http://baike.vehdjk.com/Article/details/goayklvnl.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fktsv.cn/Article/details/gnrmhnjcy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.bbcook.cn/Article/details/gncvaoviy.sHtML

[R21] 字符串长度
来源：http://read.share.vehdjk.com/Article/details/gsnoffnyr.sHtML

echo "${#s}"
来源：http://www.share.tarul.cn/Article/details/gydywotet.sHtML

[R22] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/gvmmjeslh.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gaqggmgab.sHtML

[R23] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gddfqirhl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.sjlbkw.cn/Article/details/gexxxivzr.sHtML

[R24] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gphpdffys.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.epnwcf.com/Article/details/gqtvevrpc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.sjlbkw.cn/Article/details/gjopqtxox.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.epnwcf.com/Article/details/gqzgdaccr.sHtML

[R26] 命令替换
来源：http://baike.bbcook.cn/Article/details/gnfeswaul.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.sjlbkw.cn/Article/details/gdpyacmxh.sHtML

[R27] 算术展开
来源：http://www.share.sjlbkw.cn/Article/details/gthnfeura.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.epnwcf.com/Article/details/glzjmfauj.sHtML

[R28] 浮点运算
来源：http://3g.vehdjk.com/Article/details/giflvydkv.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fktsv.cn/Article/details/gzplsqrwu.sHtML

[R29] 定义函数
来源：http://www.share.bbcook.cn/Article/details/glqntafbo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fktsv.cn/Article/details/glymdtiyk.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.vehdjk.com/Article/details/gmuwlcmpp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.vehdjk.com/Article/details/gzxljhmhb.sHtML

[R31] 局部变量
来源：http://www.share.yfazqb.com/Article/details/gcdgpvnnc.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fktsv.cn/Article/details/gnvsbskee.sHtML

[R32] 参数个数校验
来源：http://www.share.fktsv.cn/Article/details/gwltjitho.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gbsllfnhy.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fktsv.cn/Article/details/gxidnkukw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.vehdjk.com/Article/details/grvhpiora.sHtML

[R34] 退出时清理
来源：http://m.share.sjlbkw.cn/Article/details/geqlummey.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/gawfucjjs.sHtML

[R35] 后台执行并等待
来源：http://3g.epnwcf.com/Article/details/gyrvwxzjc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.yfazqb.com/Article/details/guphjaqrj.sHtML

[R36] 并发执行多个任务
来源：http://read.share.sjlbkw.cn/Article/details/gbqwzddaz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.sjlbkw.cn/Article/details/gdoymleok.sHtML

[R37] 把输出赋给变量
来源：http://3g.epnwcf.com/Article/details/gexkfwiwh.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/gotenffoo.sHtML

[R38] 管道串联
来源：http://www.blog.epnwcf.com/Article/details/grqhfrmax.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.bbcook.cn/Article/details/gxeogiroa.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.tarul.cn/Article/details/gngwisamg.sHtML

cmd > out.log 2>&1
来源：http://wap.bbcook.cn/Article/details/gkjyltmel.sHtML

[R40] 追加写日志
来源：http://blog.sjlbkw.cn/Article/details/gqgamvbpf.sHtML

echo "log" >> out.log
来源：http://www.blog.fktsv.cn/Article/details/gyzhbjnoe.sHtML

[R41] 丢弃输出
来源：http://3g.fktsv.cn/Article/details/ghpmvueeo.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fktsv.cn/Article/details/gwjuhwzkh.sHtML

[R42] 输入重定向
来源：http://blog.sjlbkw.cn/Article/details/ghdgwfqkc.sHtML

wc -l < a.txt
来源：http://read.share.vehdjk.com/Article/details/glxalidfg.sHtML

[R43] 按名字查找文件
来源：http://www.blog.yfazqb.com/Article/details/ggbfkrghg.sHtML

find . -name "*.log" -type f
来源：http://blog.sjlbkw.cn/Article/details/galmpiusp.sHtML

[R44] 按修改时间查找
来源：http://baike.sjlbkw.cn/Article/details/gmshniapi.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fktsv.cn/Article/details/gouybabwk.sHtML

[R45] 批量删除
来源：http://3g.sjlbkw.cn/Article/details/gmlywlski.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.sjlbkw.cn/Article/details/gipmywsoj.sHtML

[R46] 递归替换文件内容
来源：http://read.share.yfazqb.com/Article/details/gppbhgvkd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/gecuyndet.sHtML

[R47] sed 单行替换
来源：http://www.m.share.bbcook.cn/Article/details/grlyamfqw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.tarul.cn/Article/details/ghqeoizko.sHtML

[R48] awk 取指定列
来源：http://www.blog.vehdjk.com/Article/details/ghxssnydq.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gqmssysds.sHtML

[R49] awk 带条件
来源：http://www.blog.bbcook.cn/Article/details/glidlthry.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fktsv.cn/Article/details/gnotreozg.sHtML

[R50] awk 求和
来源：http://mobile.bbcook.cn/Article/details/gypemfisv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.tarul.cn/Article/details/gdjvfgwmf.sHtML

[R51] 排序去重取前几
来源：http://m.share.yfazqb.com/Article/details/gwflcpshe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.epnwcf.com/Article/details/grmxesgwx.sHtML

[R52] 统计行数
来源：http://m.share.yfazqb.com/Article/details/gqjbzsucp.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gmgdsajtk.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.yfazqb.com/Article/details/gaidtbbyt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.vehdjk.com/Article/details/goczibpnr.sHtML

[R54] 比较两个文件
来源：http://www.blog.tarul.cn/Article/details/ggxpbovdy.sHtML

diff a.txt b.txt
来源：http://baike.tarul.cn/Article/details/gwwgtsmwf.sHtML

[R55] 压缩与解压
来源：http://www.m.share.epnwcf.com/Article/details/gfkgbhrva.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.vehdjk.com/Article/details/gmsnwgbxs.sHtML

[R56] 远程拷贝
来源：http://www.blog.vehdjk.com/Article/details/gcavhwlmt.sHtML

scp file user@host:/path/
来源：http://blog.fktsv.cn/Article/details/gmjkawsxl.sHtML

[R57] 远程执行命令
来源：http://mobile.fktsv.cn/Article/details/gxamueuix.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.bbcook.cn/Article/details/gxthmkkvk.sHtML

[R58] 下载文件
来源：http://www.share.epnwcf.com/Article/details/gygcepexb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.tarul.cn/Article/details/geqigzlof.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/gykufkppa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.epnwcf.com/Article/details/gvkdyceqk.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/ghiipjmcp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.sjlbkw.cn/Article/details/ghqwopiew.sHtML

[R61] 磁盘占用
来源：http://wap.vehdjk.com/Article/details/ggvpbkula.sHtML

df -h;  du -sh *
来源：http://read.share.vehdjk.com/Article/details/gatabpcrx.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/guomnuqcm.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.sjlbkw.cn/Article/details/gfruwnjdz.sHtML

[R63] 内存与进程
来源：http://www.share.yfazqb.com/Article/details/gbknxlnzi.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.bbcook.cn/Article/details/gcuvdbcqw.sHtML

[R64] 结束进程
来源：http://mobile.bbcook.cn/Article/details/gtilltowh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gxkvruafc.sHtML

[R65] 查看端口占用
来源：http://wap.epnwcf.com/Article/details/glbctehzu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.sjlbkw.cn/Article/details/gjcfqytkp.sHtML

[R66] 定时任务
来源：http://3g.sjlbkw.cn/Article/details/gnhcjhhnx.sHtML

crontab -e;  crontab -l
来源：http://baike.vehdjk.com/Article/details/gmmbmwook.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.sjlbkw.cn/Article/details/gncwqporq.sHtML

openssl rand -hex 16
来源：http://www.blog.fktsv.cn/Article/details/gbikxshuq.sHtML

[R68] 计算文件校验值
来源：http://3g.epnwcf.com/Article/details/ggkjjtdyh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.yfazqb.com/Article/details/geqlqmuej.sHtML

[R69] 生成随机密码
来源：http://read.share.tarul.cn/Article/details/gklvgpozb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.sjlbkw.cn/Article/details/gyqxwvmwu.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/ghsijcfdt.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/glfyeosgt.sHtML

[R71] 日期格式化
来源：http://blog.bbcook.cn/Article/details/gimkfpcpw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.bbcook.cn/Article/details/gxucxjbmj.sHtML

[R72] 等待端口就绪
来源：http://blog.tarul.cn/Article/details/gpqlsejer.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/ggsowlden.sHtML

[R73] 分割大日志
来源：http://wap.bbcook.cn/Article/details/guljmyhtw.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/guxanlcpm.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/gayfdgrbl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.sjlbkw.cn/Article/details/gnbpedbyo.sHtML

[R75] 导出环境变量
来源：http://baike.epnwcf.com/Article/details/gsljxvunc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.sjlbkw.cn/Article/details/gycwlwmtq.sHtML

[R76] 使用临时文件
来源：http://wap.bbcook.cn/Article/details/gdsiwqppf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gzsmhjfcq.sHtML

[R77] 读取用户输入
来源：http://blog.vehdjk.com/Article/details/gphphoreg.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/gobwxchrc.sHtML

[R78] 交互式菜单
来源：http://mobile.yfazqb.com/Article/details/gpxdhhlxa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.epnwcf.com/Article/details/gxqeskgft.sHtML

[R79] 解析命令行选项
来源：http://m.share.epnwcf.com/Article/details/gxpfklqsc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.yfazqb.com/Article/details/ggccyaqiw.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.bbcook.cn/Article/details/gccbtlvxq.sHtML

time ./run.sh
来源：http://www.blog.yfazqb.com/Article/details/gninplfce.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gzbueniwd.sHtML

S. C / C++ 专题
来源：http://www.blog.bbcook.cn/Article/details/gccgcrrww.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gentabysc.sHtML

[S01] C：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/ganbrycge.sHtML

#include <stdio.h>
来源：http://www.share.epnwcf.com/Article/details/gahshynrz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.bbcook.cn/Article/details/gmkyfdcqc.sHtML

[S02] C：变量与格式化输出
来源：http://blog.bbcook.cn/Article/details/gxhsbomug.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.vehdjk.com/Article/details/gbujgbwrq.sHtML

[S03] C：读入整数
来源：http://www.blog.fktsv.cn/Article/details/gmhapvdts.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.bbcook.cn/Article/details/glzkhhtbs.sHtML

[S04] C：字符串复制
来源：http://wap.epnwcf.com/Article/details/gnkyhuaok.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gctjuubdj.sHtML

[S05] C：字符串长度
来源：http://baike.vehdjk.com/Article/details/ggikvavih.sHtML

strlen(s)
来源：http://blog.epnwcf.com/Article/details/gkmqesorc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/ghawqomgd.sHtML

strcmp(a, b) == 0
来源：http://read.share.bbcook.cn/Article/details/gpsuzhbaq.sHtML

[S07] C：数组遍历求和
来源：http://www.share.yfazqb.com/Article/details/ghjzitloi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.bbcook.cn/Article/details/gelytvijv.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/glkzydayw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/gsbmfpdug.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.sjlbkw.cn/Article/details/gjtsnwhky.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.vehdjk.com/Article/details/gwzvklgix.sHtML

[S10] C：指针与解引用
来源：http://read.share.vehdjk.com/Article/details/gkdhrtixo.sHtML

int *p = &a;  *p = 5;
来源：http://baike.epnwcf.com/Article/details/giutbunqi.sHtML

[S11] C：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gbceuneax.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.tarul.cn/Article/details/grfcarnfu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gselltohj.sHtML

fclose(f);
来源：http://3g.yfazqb.com/Article/details/gccmmcnjg.sHtML

[S12] C：写文件
来源：http://mobile.vehdjk.com/Article/details/gvvyigdyp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.epnwcf.com/Article/details/gpiqbyzwr.sHtML

[S13] C：宏定义
来源：http://www.m.share.sjlbkw.cn/Article/details/glhehwazi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.epnwcf.com/Article/details/gyaybqyfm.sHtML

[S14] C：枚举
来源：http://read.share.epnwcf.com/Article/details/gligvmixo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.bbcook.cn/Article/details/gnuygvclj.sHtML

[S15] C：类型转换
来源：http://www.share.sjlbkw.cn/Article/details/gfsomgzus.sHtML

(double) a / b
来源：http://baike.yfazqb.com/Article/details/gnwxwxyrk.sHtML

[S16] C：位操作置位
来源：http://3g.yfazqb.com/Article/details/gytglggcd.sHtML

x |= (1 << 3);
来源：http://wap.epnwcf.com/Article/details/gpjsxfsnb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gqhuodorr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/gagcchdho.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/gixyvuuqx.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gvpallzuw.sHtML

[S19] C：快速排序
来源：http://www.blog.yfazqb.com/Article/details/gynaunnxr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gfbxsoucv.sHtML

[S20] C：二分查找
来源：http://mobile.tarul.cn/Article/details/gydaahwct.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/gayxuxmdy.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/gtbrlbjlt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fktsv.cn/Article/details/gblfqwpjf.sHtML

[S22] C：字符串转数字
来源：http://read.share.fktsv.cn/Article/details/gudqcbzeq.sHtML


<!-- 参考信息 -->