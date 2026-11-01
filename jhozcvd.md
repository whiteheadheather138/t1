代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fktsv.cn/Article/details/gquplselp.sHtML

[Q52] 删除指定行
来源：http://www.m.share.bbcook.cn/Article/details/gfmwkciye.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.sjlbkw.cn/Article/details/grbbescqc.sHtML

[Q53] 按条件删除
来源：http://m.share.vehdjk.com/Article/details/gdpxtazim.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gieojxpex.sHtML

[Q54] 清空表
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzvvhext.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.sjlbkw.cn/Article/details/gaattjufy.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/gkcgdpwnt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gxmrlznga.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.yfazqb.com/Article/details/gvweumjan.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.tarul.cn/Article/details/gtctuuvyz.sHtML

[Q57] 行号
来源：http://baike.bbcook.cn/Article/details/gfxrjyfyu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gmboayfog.sHtML

[Q58] 累计求和
来源：http://read.share.yfazqb.com/Article/details/gyhbqykms.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gordrsrxk.sHtML

[Q59] 分组内累计
来源：http://read.share.bbcook.cn/Article/details/gchigkzjz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gqhkfyweq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.bbcook.cn/Article/details/gannvsmom.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.epnwcf.com/Article/details/ggodxyups.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gbkisjmmp.sHtML

[Q61] 移动平均
来源：http://m.share.yfazqb.com/Article/details/gopbkczhe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gtmedbykg.sHtML

[Q62] 分组占比
来源：http://m.share.epnwcf.com/Article/details/gstmxaadv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gumqwkjiv.sHtML

[Q63] 开启事务
来源：http://www.m.share.tarul.cn/Article/details/gmowagefh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fktsv.cn/Article/details/gawntckmp.sHtML

[Q64] 提交事务
来源：http://www.m.share.tarul.cn/Article/details/gaoshtydw.sHtML

COMMIT;
来源：http://www.m.share.bbcook.cn/Article/details/gkhkdkvye.sHtML

[Q65] 回滚事务
来源：http://blog.tarul.cn/Article/details/ghluupetz.sHtML

ROLLBACK;
来源：http://mobile.fktsv.cn/Article/details/gtvijzswv.sHtML

[Q66] 行锁查询
来源：http://www.m.share.epnwcf.com/Article/details/gtxlezomb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.sjlbkw.cn/Article/details/gbqalgsky.sHtML

[Q67] 设置隔离级别
来源：http://m.share.bbcook.cn/Article/details/gwbsjkutu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.sjlbkw.cn/Article/details/gyayhldny.sHtML

[Q68] 保存点
来源：http://baike.yfazqb.com/Article/details/gzlfkxlsu.sHtML

SAVEPOINT sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gevhopjiw.sHtML

ROLLBACK TO sp1;
来源：http://wap.epnwcf.com/Article/details/gtkysilzi.sHtML

[Q69] 查看执行计划
来源：http://blog.tarul.cn/Article/details/gthropuao.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.vehdjk.com/Article/details/gfohrwraf.sHtML

[Q70] 更新统计信息
来源：http://mobile.epnwcf.com/Article/details/ghpvpgyic.sHtML

ANALYZE TABLE users;
来源：http://3g.sjlbkw.cn/Article/details/gejzckiac.sHtML

[Q71] 查看建表语句
来源：http://read.share.bbcook.cn/Article/details/grpizxcbt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/gvpquctme.sHtML

[Q72] 查看索引
来源：http://www.share.bbcook.cn/Article/details/gextqlmry.sHtML

SHOW INDEX FROM users;
来源：http://mobile.bbcook.cn/Article/details/grvrnhmrk.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/gwjkonizi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.bbcook.cn/Article/details/gqgbuqdru.sHtML

[Q74] 强制使用索引
来源：http://www.share.sjlbkw.cn/Article/details/gxeulywiq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.bbcook.cn/Article/details/gdwnaqlay.sHtML

[Q75] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gjxhdngnu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gqeryzggh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.tarul.cn/Article/details/gdupdjeia.sHtML

[Q76] 按天统计
来源：http://blog.yfazqb.com/Article/details/glyzwgadd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/gxyqjvsli.sHtML

[Q77] 时间加减
来源：http://www.share.epnwcf.com/Article/details/gjqkxaooq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fktsv.cn/Article/details/gquepduiy.sHtML

[Q78] 当前时间
来源：http://wap.tarul.cn/Article/details/guewjkbyf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.bbcook.cn/Article/details/gbaolxkmu.sHtML

[Q79] 字符串拼接
来源：http://read.share.fktsv.cn/Article/details/gnedjqaje.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/gdpbqafih.sHtML

[Q80] 字符串截取
来源：http://read.share.vehdjk.com/Article/details/gopzgaxxg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gddvsmmdi.sHtML

[Q81] 字符串替换
来源：http://blog.fktsv.cn/Article/details/ggkvgciui.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gtzgzasjl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.sjlbkw.cn/Article/details/gfmwoxvnw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/genqpykxu.sHtML

[Q83] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gkaikowfq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gssktksbh.sHtML

[Q84] 去除首尾空格
来源：http://blog.vehdjk.com/Article/details/gllnijrns.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gbehqtxxi.sHtML

[Q85] 数值取整
来源：http://wap.tarul.cn/Article/details/gfspzabvj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.sjlbkw.cn/Article/details/gopommtgi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.tarul.cn/Article/details/gyowcuhzt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.bbcook.cn/Article/details/griwfwvvg.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fktsv.cn/Article/details/grtdzrzwu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.bbcook.cn/Article/details/gfrckqmkv.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.vehdjk.com/Article/details/gasiesybd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.vehdjk.com/Article/details/gahfqikks.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.vehdjk.com/Article/details/ghwioqtni.sHtML

[Q89] 判断表是否存在
来源：http://3g.fktsv.cn/Article/details/gyudylmrp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.tarul.cn/Article/details/gxjlsvqyt.sHtML

[Q90] 生成序号列
来源：http://www.share.vehdjk.com/Article/details/gdpxjdqyb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.bbcook.cn/Article/details/gqzbofzho.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gkrmvspna.sHtML

R. Bash 专题
来源：http://www.share.sjlbkw.cn/Article/details/gkzzrenmu.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/grwqsiynm.sHtML

[R01] shebang 与严格模式
来源：http://mobile.yfazqb.com/Article/details/gsoqsaywl.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gqddmsrxi.sHtML

set -euo pipefail
来源：http://mobile.fktsv.cn/Article/details/gzbnrdsgu.sHtML

[R02] 变量赋值与使用
来源：http://m.share.tarul.cn/Article/details/geqciofrq.sHtML

name="Tom"; echo "$name"
来源：http://wap.fktsv.cn/Article/details/ggesvfvnz.sHtML

[R03] 只读变量
来源：http://read.share.yfazqb.com/Article/details/gyykrqtbm.sHtML

readonly PI=3.14
来源：http://www.m.share.epnwcf.com/Article/details/gxcpcfsnj.sHtML

[R04] 位置参数
来源：http://m.share.yfazqb.com/Article/details/ggokettlq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fktsv.cn/Article/details/gxjujzrhm.sHtML

[R05] 参数默认值
来源：http://www.blog.sjlbkw.cn/Article/details/grjzuldjv.sHtML

name="${1:-default}"
来源：http://mobile.epnwcf.com/Article/details/gutaxazla.sHtML

[R06] 判断命令是否存在
来源：http://baike.tarul.cn/Article/details/gedqdxfem.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fktsv.cn/Article/details/gynkfqmyn.sHtML

[R07] if 判断文件
来源：http://baike.epnwcf.com/Article/details/glwjhtjud.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gbrqbjsny.sHtML

[R08] 数值比较
来源：http://blog.vehdjk.com/Article/details/geccoleml.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.tarul.cn/Article/details/gckfjzllc.sHtML

[R09] 字符串比较
来源：http://wap.epnwcf.com/Article/details/gbmilvmmq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.tarul.cn/Article/details/gllrvkzmy.sHtML

[R10] 正则匹配
来源：http://baike.tarul.cn/Article/details/gxtesdjzx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.bbcook.cn/Article/details/guvudowlb.sHtML

[R11] case 多分支
来源：http://www.share.sjlbkw.cn/Article/details/gewaygsjl.sHtML

case "$1" in
来源：http://www.share.epnwcf.com/Article/details/gkhjtlvfu.sHtML

start) echo "启动" ;;
来源：http://read.share.epnwcf.com/Article/details/gyomfkqbf.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfxztjoz.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.bbcook.cn/Article/details/gqxmffjda.sHtML

esac
来源：http://baike.tarul.cn/Article/details/ggsmwypff.sHtML

[R12] for 遍历文件
来源：http://read.share.yfazqb.com/Article/details/gmlpodaue.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.yfazqb.com/Article/details/gmisnzpof.sHtML

[R13] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/ggifgcjmx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fktsv.cn/Article/details/gyjsyxrym.sHtML

[R14] C 风格 for
来源：http://mobile.yfazqb.com/Article/details/gvkjyfexd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gniejukxb.sHtML

[R15] while 逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/ggaqtxwjl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.epnwcf.com/Article/details/gfcbnvide.sHtML

[R16] until 等待条件
来源：http://baike.epnwcf.com/Article/details/gnkihruvx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gznxbjntp.sHtML

[R17] 数组定义与取值
来源：http://baike.bbcook.cn/Article/details/gppnijboe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.bbcook.cn/Article/details/gvplkuuez.sHtML

[R18] 遍历数组
来源：http://www.share.bbcook.cn/Article/details/gbmejwluu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.tarul.cn/Article/details/gqdfrkdst.sHtML

[R19] 数组长度
来源：http://m.share.tarul.cn/Article/details/gyafphaug.sHtML

echo "${#arr[@]}"
来源：http://www.share.yfazqb.com/Article/details/ginuabavu.sHtML

[R20] 关联数组（字典）
来源：http://baike.yfazqb.com/Article/details/gqtjfperl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.sjlbkw.cn/Article/details/gunakuzsr.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/gjruydlmb.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gnbykgdua.sHtML

[R22] 截取子串
来源：http://3g.bbcook.cn/Article/details/gfbmczrkg.sHtML

echo "${s:0:5}"
来源：http://mobile.fktsv.cn/Article/details/gshkjyldb.sHtML

[R23] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gbweuupqh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.vehdjk.com/Article/details/gttjvsfeb.sHtML

[R24] 大小写转换
来源：http://baike.yfazqb.com/Article/details/geomzmsne.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/gozileqmj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.bbcook.cn/Article/details/gmjoszhmb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.yfazqb.com/Article/details/gfcdzxiyd.sHtML

[R26] 命令替换
来源：http://blog.bbcook.cn/Article/details/gzpnhsmnk.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.tarul.cn/Article/details/gvfnscwdj.sHtML

[R27] 算术展开
来源：http://www.blog.fktsv.cn/Article/details/gzvzhnmbj.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfhezbwh.sHtML

[R28] 浮点运算
来源：http://baike.tarul.cn/Article/details/gzzvhiolp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fktsv.cn/Article/details/gzgfjxwku.sHtML

[R29] 定义函数
来源：http://3g.bbcook.cn/Article/details/gknnnossa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.tarul.cn/Article/details/gdvgochdh.sHtML

[R30] 函数返回状态码
来源：http://m.share.epnwcf.com/Article/details/gwinfxeuk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.yfazqb.com/Article/details/ghzbhrcdj.sHtML

[R31] 局部变量
来源：http://www.blog.tarul.cn/Article/details/ggtnzrtig.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/guvzerton.sHtML

[R32] 参数个数校验
来源：http://www.share.sjlbkw.cn/Article/details/gteftninq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/givqktezi.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.epnwcf.com/Article/details/gznyjxbji.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fktsv.cn/Article/details/gkxcbkpbk.sHtML

[R34] 退出时清理
来源：http://www.blog.sjlbkw.cn/Article/details/galraildr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gtsyfhpen.sHtML

[R35] 后台执行并等待
来源：http://3g.vehdjk.com/Article/details/gkgwpsfjb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.vehdjk.com/Article/details/gwxazjqyo.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.bbcook.cn/Article/details/gzuyzzsoi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.vehdjk.com/Article/details/gawvjnjkx.sHtML

[R37] 把输出赋给变量
来源：http://wap.sjlbkw.cn/Article/details/gdillewfr.sHtML

files=$(ls -1)
来源：http://wap.epnwcf.com/Article/details/greomzhzr.sHtML

[R38] 管道串联
来源：http://www.blog.sjlbkw.cn/Article/details/gkgqembfs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.epnwcf.com/Article/details/gxiollvzv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.vehdjk.com/Article/details/gfhqklbvk.sHtML

cmd > out.log 2>&1
来源：http://read.share.bbcook.cn/Article/details/gfyurbkel.sHtML

[R40] 追加写日志
来源：http://read.share.fktsv.cn/Article/details/gyzhbzesh.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/gwptpwolq.sHtML

[R41] 丢弃输出
来源：http://3g.tarul.cn/Article/details/gozrjxkoq.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fktsv.cn/Article/details/gnaoqojhb.sHtML

[R42] 输入重定向
来源：http://www.blog.vehdjk.com/Article/details/gnyrdswxu.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/ghwzspdjv.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.tarul.cn/Article/details/gnvutnllk.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fktsv.cn/Article/details/gyxifigmf.sHtML

[R44] 按修改时间查找
来源：http://3g.bbcook.cn/Article/details/gutdqsutz.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.bbcook.cn/Article/details/gqqeekidk.sHtML

[R45] 批量删除
来源：http://blog.bbcook.cn/Article/details/gzwstlwqg.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.epnwcf.com/Article/details/gkvppgtxn.sHtML

[R46] 递归替换文件内容
来源：http://m.share.tarul.cn/Article/details/ghrgaossm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.tarul.cn/Article/details/gdpjaozdt.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fktsv.cn/Article/details/gfukqhcrn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gcfsyykdt.sHtML

[R48] awk 取指定列
来源：http://mobile.vehdjk.com/Article/details/gsqpyngng.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.vehdjk.com/Article/details/ggzqtkvua.sHtML

[R49] awk 带条件
来源：http://read.share.yfazqb.com/Article/details/gxkbwafww.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.epnwcf.com/Article/details/gmsmqruac.sHtML

[R50] awk 求和
来源：http://www.m.share.yfazqb.com/Article/details/gzlbrffbs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.yfazqb.com/Article/details/glpswazio.sHtML

[R51] 排序去重取前几
来源：http://baike.yfazqb.com/Article/details/gvphxqync.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.tarul.cn/Article/details/glvnktpqb.sHtML

[R52] 统计行数
来源：http://read.share.epnwcf.com/Article/details/gppaikivl.sHtML

wc -l a.txt
来源：http://baike.yfazqb.com/Article/details/gomcrfzvo.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.epnwcf.com/Article/details/gborwywcd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.vehdjk.com/Article/details/gwigzggvo.sHtML

[R54] 比较两个文件
来源：http://wap.vehdjk.com/Article/details/gkzgxpsgz.sHtML

diff a.txt b.txt
来源：http://m.share.epnwcf.com/Article/details/gtcmgsios.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/gzcsibcyg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.epnwcf.com/Article/details/gojzcqvgo.sHtML

[R56] 远程拷贝
来源：http://mobile.bbcook.cn/Article/details/ghfoynutt.sHtML

scp file user@host:/path/
来源：http://mobile.vehdjk.com/Article/details/geogrxyqq.sHtML

[R57] 远程执行命令
来源：http://read.share.sjlbkw.cn/Article/details/ggzcoeodt.sHtML

ssh user@host 'uptime'
来源：http://mobile.bbcook.cn/Article/details/gpivmyler.sHtML

[R58] 下载文件
来源：http://3g.bbcook.cn/Article/details/gxsyaldli.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/gonriyliw.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gpuxabtbw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.epnwcf.com/Article/details/gmyxxjtwa.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gyhnlrawp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.bbcook.cn/Article/details/gdwbzonrk.sHtML

[R61] 磁盘占用
来源：http://wap.epnwcf.com/Article/details/ghuzrgasb.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/gwbruuvni.sHtML

[R62] 找最占空间的文件
来源：http://m.share.tarul.cn/Article/details/gmyemcbsx.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.vehdjk.com/Article/details/gsidjiqlu.sHtML

[R63] 内存与进程
来源：http://wap.fktsv.cn/Article/details/gdsaxpaau.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.sjlbkw.cn/Article/details/guypzrqbs.sHtML

[R64] 结束进程
来源：http://www.blog.epnwcf.com/Article/details/gtprgraad.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.vehdjk.com/Article/details/gvhlowiec.sHtML

[R65] 查看端口占用
来源：http://www.share.bbcook.cn/Article/details/gprbolfzz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.epnwcf.com/Article/details/gqkccmfvd.sHtML

[R66] 定时任务
来源：http://www.share.epnwcf.com/Article/details/goswishql.sHtML

crontab -e;  crontab -l
来源：http://read.share.epnwcf.com/Article/details/gxcvhkvbk.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.yfazqb.com/Article/details/gyfmsdlzw.sHtML

openssl rand -hex 16
来源：http://blog.yfazqb.com/Article/details/gluumghhx.sHtML

[R68] 计算文件校验值
来源：http://read.share.tarul.cn/Article/details/gpruretox.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.epnwcf.com/Article/details/gxtlguxpb.sHtML

[R69] 生成随机密码
来源：http://www.share.vehdjk.com/Article/details/gwigpppoe.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.tarul.cn/Article/details/gxhjsmeqt.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.yfazqb.com/Article/details/gnqsoznaz.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.epnwcf.com/Article/details/gnaffszty.sHtML

[R71] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gevznoetj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfimtimb.sHtML

[R72] 等待端口就绪
来源：http://www.share.epnwcf.com/Article/details/gugrlafuy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gxkehzyco.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/gmlmfyums.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqjuuagb.sHtML

[R74] 批量重命名
来源：http://www.blog.epnwcf.com/Article/details/gdwhyevnp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.yfazqb.com/Article/details/gjslfghas.sHtML

[R75] 导出环境变量
来源：http://blog.vehdjk.com/Article/details/gkjlsouvb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/gamzodwcq.sHtML

[R76] 使用临时文件
来源：http://www.blog.epnwcf.com/Article/details/gyelwcldy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gjqdveabj.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/gezelwnzm.sHtML

read -rp "请输入: " ans
来源：http://m.share.yfazqb.com/Article/details/gicbgnrzv.sHtML

[R78] 交互式菜单
来源：http://www.blog.tarul.cn/Article/details/gtuttyjvy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/gqpkdeobx.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.bbcook.cn/Article/details/gsmpnyjex.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.bbcook.cn/Article/details/gtybeslax.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fktsv.cn/Article/details/gpuqfkacv.sHtML

time ./run.sh
来源：http://www.share.yfazqb.com/Article/details/gsvpmdafs.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghqmhoypi.sHtML

S. C / C++ 专题
来源：http://blog.sjlbkw.cn/Article/details/gjohkiyeo.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/grkrysiyi.sHtML

[S01] C：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/grkaefdkk.sHtML

#include <stdio.h>
来源：http://m.share.vehdjk.com/Article/details/guspbfgnz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.vehdjk.com/Article/details/govtlagyb.sHtML

[S02] C：变量与格式化输出
来源：http://wap.yfazqb.com/Article/details/gayqrvglw.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.bbcook.cn/Article/details/gaejvuyie.sHtML

[S03] C：读入整数
来源：http://m.share.tarul.cn/Article/details/girvorgjl.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fktsv.cn/Article/details/geutivcfc.sHtML

[S04] C：字符串复制
来源：http://wap.fktsv.cn/Article/details/gwynqllfh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.vehdjk.com/Article/details/gwthsjhmi.sHtML

[S05] C：字符串长度
来源：http://mobile.fktsv.cn/Article/details/ghkxakfcc.sHtML

strlen(s)
来源：http://m.share.fktsv.cn/Article/details/gaeibirzi.sHtML

[S06] C：字符串比较
来源：http://m.share.vehdjk.com/Article/details/gdjemffje.sHtML

strcmp(a, b) == 0
来源：http://blog.sjlbkw.cn/Article/details/gagmwdbtt.sHtML

[S07] C：数组遍历求和
来源：http://wap.bbcook.cn/Article/details/gwbnmpfay.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.yfazqb.com/Article/details/gupdnhxcl.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.bbcook.cn/Article/details/gjzkazkoi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.vehdjk.com/Article/details/guxneetju.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fktsv.cn/Article/details/gcmwdlfaw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.yfazqb.com/Article/details/goaycfvai.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/gjeotpaeo.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/gwwnnlrfk.sHtML

[S11] C：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gmwoudxhb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.bbcook.cn/Article/details/ghwzscgil.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.epnwcf.com/Article/details/gaxfdkvim.sHtML

fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/gmdbopyig.sHtML

[S12] C：写文件
来源：http://mobile.fktsv.cn/Article/details/givrkwhja.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gmqudenyd.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/glxrrqorl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.sjlbkw.cn/Article/details/gmynrdlem.sHtML

[S14] C：枚举
来源：http://mobile.fktsv.cn/Article/details/gbnkbgxkx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.epnwcf.com/Article/details/glwsodowl.sHtML

[S15] C：类型转换
来源：http://blog.bbcook.cn/Article/details/gnncehjfp.sHtML

(double) a / b
来源：http://m.share.yfazqb.com/Article/details/gufoedhky.sHtML

[S16] C：位操作置位
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfiijtpt.sHtML

x |= (1 << 3);
来源：http://wap.yfazqb.com/Article/details/gicnhwarf.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gfsseiwdt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.bbcook.cn/Article/details/gdrqbpvgl.sHtML

[S18] C：命令行参数
来源：http://blog.fktsv.cn/Article/details/gynknipkp.sHtML

int main(int argc, char **argv)
来源：http://read.share.vehdjk.com/Article/details/gstawogvi.sHtML

[S19] C：快速排序
来源：http://3g.yfazqb.com/Article/details/gleeymeox.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gmxkvtmbv.sHtML

[S20] C：二分查找
来源：http://www.m.share.bbcook.cn/Article/details/gbnpaqole.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gvfkjdizt.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/ggwaajvcp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.bbcook.cn/Article/details/gidfreggj.sHtML

[S22] C：字符串转数字
来源：http://read.share.epnwcf.com/Article/details/gmfyivknn.sHtML


<!-- 参考信息 -->