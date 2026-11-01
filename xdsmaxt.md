代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gmamiovml.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.bbcook.cn/Article/details/gpcgkhagl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gxvtqvcig.sHtML

[Q57] 行号
来源：http://baike.yfazqb.com/Article/details/ghbfjuzsz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gxzxtvzno.sHtML

[Q58] 累计求和
来源：http://baike.epnwcf.com/Article/details/gdyqqcyok.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gxxmbroml.sHtML

[Q59] 分组内累计
来源：http://3g.epnwcf.com/Article/details/gjsfqpdwb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.tarul.cn/Article/details/gbfwyzclq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.bbcook.cn/Article/details/gvigrdxlc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.epnwcf.com/Article/details/gxhbczpzs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gyzohmttc.sHtML

[Q61] 移动平均
来源：http://mobile.sjlbkw.cn/Article/details/gxalhwowg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gyujaylir.sHtML

[Q62] 分组占比
来源：http://mobile.sjlbkw.cn/Article/details/guslvnbph.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gjojhhaem.sHtML

[Q63] 开启事务
来源：http://www.share.epnwcf.com/Article/details/gnqcsjysy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fktsv.cn/Article/details/gdotbcgwq.sHtML

[Q64] 提交事务
来源：http://wap.sjlbkw.cn/Article/details/glkmzqtce.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/gzxjfpaxg.sHtML

[Q65] 回滚事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfeqrmyy.sHtML

ROLLBACK;
来源：http://mobile.yfazqb.com/Article/details/gnvazlgnl.sHtML

[Q66] 行锁查询
来源：http://blog.epnwcf.com/Article/details/gybnqgcqi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.tarul.cn/Article/details/gqeorrfus.sHtML

[Q67] 设置隔离级别
来源：http://m.share.vehdjk.com/Article/details/gjoekzlsr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.yfazqb.com/Article/details/gwjgdmagk.sHtML

[Q68] 保存点
来源：http://www.blog.epnwcf.com/Article/details/gmyeiwfko.sHtML

SAVEPOINT sp1;
来源：http://baike.sjlbkw.cn/Article/details/gzqfvpjvh.sHtML

ROLLBACK TO sp1;
来源：http://wap.bbcook.cn/Article/details/gwydokknc.sHtML

[Q69] 查看执行计划
来源：http://mobile.fktsv.cn/Article/details/gbbbuysdr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.yfazqb.com/Article/details/gzsrawplk.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/gwaeikqnz.sHtML

ANALYZE TABLE users;
来源：http://baike.sjlbkw.cn/Article/details/giurbzrir.sHtML

[Q71] 查看建表语句
来源：http://mobile.sjlbkw.cn/Article/details/gvauzbtou.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.sjlbkw.cn/Article/details/gkycqlzxq.sHtML

[Q72] 查看索引
来源：http://3g.tarul.cn/Article/details/gampkmzsp.sHtML

SHOW INDEX FROM users;
来源：http://mobile.yfazqb.com/Article/details/gaichcdbc.sHtML

[Q73] 查看表状态
来源：http://3g.bbcook.cn/Article/details/gkssydzjs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fktsv.cn/Article/details/giaygukhh.sHtML

[Q74] 强制使用索引
来源：http://wap.epnwcf.com/Article/details/gbgyusbnb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.bbcook.cn/Article/details/gckfawbfe.sHtML

[Q75] 日期格式化
来源：http://baike.epnwcf.com/Article/details/gcyhvffal.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gipiflawd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fktsv.cn/Article/details/gcsqjcyxn.sHtML

[Q76] 按天统计
来源：http://www.share.tarul.cn/Article/details/gtqfeawmg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.sjlbkw.cn/Article/details/gjpiphjxk.sHtML

[Q77] 时间加减
来源：http://www.blog.tarul.cn/Article/details/gikjtyacp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fktsv.cn/Article/details/gmgnvtrhv.sHtML

[Q78] 当前时间
来源：http://read.share.yfazqb.com/Article/details/gqikhnzzl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.epnwcf.com/Article/details/gspximuvy.sHtML

[Q79] 字符串拼接
来源：http://mobile.epnwcf.com/Article/details/glkzkepkc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.epnwcf.com/Article/details/gqcomxzym.sHtML

[Q80] 字符串截取
来源：http://www.m.share.yfazqb.com/Article/details/ghdjeotts.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gpkwonhhj.sHtML

[Q81] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gbuncablr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.bbcook.cn/Article/details/gvppytrjo.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.vehdjk.com/Article/details/gpmkyylbl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gkbznpelp.sHtML

[Q83] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/glgawfuzc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gvduzbxie.sHtML

[Q84] 去除首尾空格
来源：http://baike.epnwcf.com/Article/details/gtrxigotp.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gjjfcbgux.sHtML

[Q85] 数值取整
来源：http://blog.bbcook.cn/Article/details/gbbzcamgc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.tarul.cn/Article/details/gqxszymzh.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.bbcook.cn/Article/details/gvdulpzku.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.bbcook.cn/Article/details/gyukgfvke.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.sjlbkw.cn/Article/details/gsdejhbks.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.bbcook.cn/Article/details/gqjbjmifs.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.yfazqb.com/Article/details/gssbcyltx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.epnwcf.com/Article/details/gfomyceqg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.yfazqb.com/Article/details/gsitbgmpo.sHtML

[Q89] 判断表是否存在
来源：http://blog.yfazqb.com/Article/details/glzxlqdnf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.tarul.cn/Article/details/gghlvwknc.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gyqccqavo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.tarul.cn/Article/details/gohbejwha.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/galrfpqpv.sHtML

R. Bash 专题
来源：http://www.share.vehdjk.com/Article/details/gypaueqhv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gaboitilt.sHtML

[R01] shebang 与严格模式
来源：http://blog.vehdjk.com/Article/details/grpkkiwkp.sHtML

#!/usr/bin/env bash
来源：http://m.share.epnwcf.com/Article/details/gdnyerqol.sHtML

set -euo pipefail
来源：http://mobile.vehdjk.com/Article/details/grhgwvovi.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.bbcook.cn/Article/details/gajtlnrma.sHtML

name="Tom"; echo "$name"
来源：http://3g.yfazqb.com/Article/details/gopmelvaz.sHtML

[R03] 只读变量
来源：http://blog.vehdjk.com/Article/details/gobjorktr.sHtML

readonly PI=3.14
来源：http://wap.fktsv.cn/Article/details/gbqocmujf.sHtML

[R04] 位置参数
来源：http://m.share.vehdjk.com/Article/details/gqwwkwess.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.vehdjk.com/Article/details/gzeovsioz.sHtML

[R05] 参数默认值
来源：http://mobile.vehdjk.com/Article/details/gnpndorga.sHtML

name="${1:-default}"
来源：http://mobile.tarul.cn/Article/details/gfonpysvj.sHtML

[R06] 判断命令是否存在
来源：http://3g.yfazqb.com/Article/details/gmvqvzhep.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gpagsfyao.sHtML

[R07] if 判断文件
来源：http://www.share.yfazqb.com/Article/details/gxehspmif.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fktsv.cn/Article/details/gflyflime.sHtML

[R08] 数值比较
来源：http://3g.yfazqb.com/Article/details/gviufeinn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.tarul.cn/Article/details/gctyxfuuk.sHtML

[R09] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/gaebtawkq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fktsv.cn/Article/details/ggovqrjlg.sHtML

[R10] 正则匹配
来源：http://mobile.fktsv.cn/Article/details/guthmaodp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.vehdjk.com/Article/details/ghzzpvwdq.sHtML

[R11] case 多分支
来源：http://baike.yfazqb.com/Article/details/gjlriosaa.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/gopsqbpol.sHtML

start) echo "启动" ;;
来源：http://m.share.vehdjk.com/Article/details/gwxeydipv.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fktsv.cn/Article/details/ggkgeywpf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gqpmzkaai.sHtML

esac
来源：http://mobile.tarul.cn/Article/details/gqzlxhabx.sHtML

[R12] for 遍历文件
来源：http://baike.bbcook.cn/Article/details/ggyeypiql.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gwnfvlvth.sHtML

[R13] for 计数循环
来源：http://m.share.tarul.cn/Article/details/gtgrxggdo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gpidlzlaf.sHtML

[R14] C 风格 for
来源：http://3g.sjlbkw.cn/Article/details/gujalkgix.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gwscqadlp.sHtML

[R15] while 逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gpjqhitxl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.vehdjk.com/Article/details/gblyruqfw.sHtML

[R16] until 等待条件
来源：http://3g.sjlbkw.cn/Article/details/gnpqjnkci.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/gujloblcy.sHtML

[R17] 数组定义与取值
来源：http://baike.epnwcf.com/Article/details/gxjplqhtm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/gggadhjyy.sHtML

[R18] 遍历数组
来源：http://www.blog.sjlbkw.cn/Article/details/geopvodsq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fktsv.cn/Article/details/gnbjyfyuq.sHtML

[R19] 数组长度
来源：http://read.share.fktsv.cn/Article/details/gibqgbkwv.sHtML

echo "${#arr[@]}"
来源：http://mobile.sjlbkw.cn/Article/details/gwiphxgur.sHtML

[R20] 关联数组（字典）
来源：http://wap.yfazqb.com/Article/details/gpcdzjwzj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgsmswje.sHtML

[R21] 字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gvdgxsqok.sHtML

echo "${#s}"
来源：http://m.share.yfazqb.com/Article/details/gheqkqmgd.sHtML

[R22] 截取子串
来源：http://mobile.fktsv.cn/Article/details/gkloftosz.sHtML

echo "${s:0:5}"
来源：http://mobile.vehdjk.com/Article/details/gjnaknjlz.sHtML

[R23] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/geavuzamw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.tarul.cn/Article/details/gybscbpsz.sHtML

[R24] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gegjlxjqi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.sjlbkw.cn/Article/details/gsdcjrfti.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.vehdjk.com/Article/details/gapyhogly.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.epnwcf.com/Article/details/gepstocgz.sHtML

[R26] 命令替换
来源：http://www.blog.vehdjk.com/Article/details/ghzprszjh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.yfazqb.com/Article/details/gsgpotrve.sHtML

[R27] 算术展开
来源：http://www.m.share.epnwcf.com/Article/details/gfosjuzry.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.vehdjk.com/Article/details/gslkvcilj.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/ggovftycz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.vehdjk.com/Article/details/gqbfffeka.sHtML

[R29] 定义函数
来源：http://blog.bbcook.cn/Article/details/gvwjqbegn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.bbcook.cn/Article/details/gmqatzkqb.sHtML

[R30] 函数返回状态码
来源：http://www.blog.epnwcf.com/Article/details/gxpejxqdd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/girvyenvc.sHtML

[R31] 局部变量
来源：http://www.share.bbcook.cn/Article/details/gdsxtfzmo.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/gbcyjtqhi.sHtML

[R32] 参数个数校验
来源：http://wap.yfazqb.com/Article/details/ggroxuxeu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gedapzzuk.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.vehdjk.com/Article/details/geooacgvw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.epnwcf.com/Article/details/ghbdsuhec.sHtML

[R34] 退出时清理
来源：http://3g.sjlbkw.cn/Article/details/gzvkqqgpj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gghrlixgl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.epnwcf.com/Article/details/gtxyhrqzw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.epnwcf.com/Article/details/gsbvuloqy.sHtML

[R36] 并发执行多个任务
来源：http://3g.yfazqb.com/Article/details/gteahklqe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fktsv.cn/Article/details/gdpvnxgvn.sHtML

[R37] 把输出赋给变量
来源：http://3g.sjlbkw.cn/Article/details/gsfwopmgo.sHtML

files=$(ls -1)
来源：http://blog.fktsv.cn/Article/details/gbxsccktd.sHtML

[R38] 管道串联
来源：http://www.blog.vehdjk.com/Article/details/gkkxjarhy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.epnwcf.com/Article/details/grgjziwik.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.sjlbkw.cn/Article/details/gfshargge.sHtML

cmd > out.log 2>&1
来源：http://m.share.bbcook.cn/Article/details/gjpordosv.sHtML

[R40] 追加写日志
来源：http://www.share.sjlbkw.cn/Article/details/gxbvrekwp.sHtML

echo "log" >> out.log
来源：http://m.share.yfazqb.com/Article/details/ggtuougcc.sHtML

[R41] 丢弃输出
来源：http://www.share.tarul.cn/Article/details/goydsuzpv.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.vehdjk.com/Article/details/ggqpcujxc.sHtML

[R42] 输入重定向
来源：http://m.share.fktsv.cn/Article/details/gmmonlwhr.sHtML

wc -l < a.txt
来源：http://blog.bbcook.cn/Article/details/gazpviukb.sHtML

[R43] 按名字查找文件
来源：http://blog.epnwcf.com/Article/details/gaqaihzhd.sHtML

find . -name "*.log" -type f
来源：http://baike.epnwcf.com/Article/details/gkkhiwotf.sHtML

[R44] 按修改时间查找
来源：http://www.share.yfazqb.com/Article/details/gkszprwrr.sHtML

find . -mtime -7 -type f
来源：http://mobile.yfazqb.com/Article/details/gmtxcxzoz.sHtML

[R45] 批量删除
来源：http://blog.bbcook.cn/Article/details/gbmwszkax.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.tarul.cn/Article/details/gejeayefx.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fktsv.cn/Article/details/gllqxjptl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fktsv.cn/Article/details/gtwxdqlou.sHtML

[R47] sed 单行替换
来源：http://baike.tarul.cn/Article/details/gacbicxoo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.yfazqb.com/Article/details/gepfenwoe.sHtML

[R48] awk 取指定列
来源：http://www.blog.epnwcf.com/Article/details/gbmsgxjjn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gznhydouc.sHtML

[R49] awk 带条件
来源：http://blog.bbcook.cn/Article/details/gkbexjzqc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fktsv.cn/Article/details/gtladnhuq.sHtML

[R50] awk 求和
来源：http://m.share.sjlbkw.cn/Article/details/gtblrdhac.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gifxiymcx.sHtML

[R51] 排序去重取前几
来源：http://mobile.vehdjk.com/Article/details/glaqtnavo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.sjlbkw.cn/Article/details/gdpbukaqc.sHtML

[R52] 统计行数
来源：http://www.share.yfazqb.com/Article/details/gsqojpdhn.sHtML

wc -l a.txt
来源：http://www.share.sjlbkw.cn/Article/details/ghpyknnln.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.tarul.cn/Article/details/gygjzjxrq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.yfazqb.com/Article/details/grunoihzs.sHtML

[R54] 比较两个文件
来源：http://read.share.epnwcf.com/Article/details/gyfgsekie.sHtML

diff a.txt b.txt
来源：http://www.blog.sjlbkw.cn/Article/details/ghnudatxl.sHtML

[R55] 压缩与解压
来源：http://wap.yfazqb.com/Article/details/gzizkqmci.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.bbcook.cn/Article/details/gmimsclcb.sHtML

[R56] 远程拷贝
来源：http://www.blog.yfazqb.com/Article/details/grqybqtqf.sHtML

scp file user@host:/path/
来源：http://3g.sjlbkw.cn/Article/details/gqswzmdqx.sHtML

[R57] 远程执行命令
来源：http://www.share.bbcook.cn/Article/details/ghfhtfzlx.sHtML

ssh user@host 'uptime'
来源：http://wap.tarul.cn/Article/details/gqlbeoddn.sHtML

[R58] 下载文件
来源：http://mobile.fktsv.cn/Article/details/ggpbtyiwj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.bbcook.cn/Article/details/gnsysfkry.sHtML

[R59] 发 POST JSON
来源：http://mobile.epnwcf.com/Article/details/gsjmfmqwe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.bbcook.cn/Article/details/ghaukrwce.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/givtazgld.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fktsv.cn/Article/details/gunmhmasv.sHtML

[R61] 磁盘占用
来源：http://wap.vehdjk.com/Article/details/gtwngubmr.sHtML

df -h;  du -sh *
来源：http://mobile.tarul.cn/Article/details/gqdadfbal.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/gwqbiinrn.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.bbcook.cn/Article/details/gckbtqryw.sHtML

[R63] 内存与进程
来源：http://www.blog.yfazqb.com/Article/details/grjgeecnd.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fktsv.cn/Article/details/gixyxxskb.sHtML

[R64] 结束进程
来源：http://mobile.fktsv.cn/Article/details/gmihxbvbz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/goidvgdsj.sHtML

[R65] 查看端口占用
来源：http://m.share.bbcook.cn/Article/details/galmizhtp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.vehdjk.com/Article/details/gogtxrqml.sHtML

[R66] 定时任务
来源：http://www.blog.yfazqb.com/Article/details/gmnmtgfnc.sHtML

crontab -e;  crontab -l
来源：http://wap.tarul.cn/Article/details/gbbserlwp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.sjlbkw.cn/Article/details/gojyranpw.sHtML

openssl rand -hex 16
来源：http://mobile.bbcook.cn/Article/details/ghvrtutye.sHtML

[R68] 计算文件校验值
来源：http://www.blog.bbcook.cn/Article/details/goxrwedol.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.bbcook.cn/Article/details/gnepoguca.sHtML

[R69] 生成随机密码
来源：http://wap.sjlbkw.cn/Article/details/gkknbbnvt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fktsv.cn/Article/details/gqrrjubjp.sHtML

[R70] 时间戳与互转
来源：http://read.share.bbcook.cn/Article/details/gdabwuswp.sHtML

date +%s;  date -d @1700000000
来源：http://baike.tarul.cn/Article/details/gdewbqzgw.sHtML

[R71] 日期格式化
来源：http://baike.epnwcf.com/Article/details/gzihbnjgf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.vehdjk.com/Article/details/ghymwqbit.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fktsv.cn/Article/details/gkqhrxtpd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/gditoxfqz.sHtML

[R73] 分割大日志
来源：http://www.share.yfazqb.com/Article/details/glelnuagq.sHtML

split -l 1000 big.log part_
来源：http://www.blog.vehdjk.com/Article/details/ghsuwftnd.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/ghnxopnxg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.bbcook.cn/Article/details/gvnhiktzp.sHtML

[R75] 导出环境变量
来源：http://3g.sjlbkw.cn/Article/details/gctcyuxqz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.vehdjk.com/Article/details/glibotbqr.sHtML

[R76] 使用临时文件
来源：http://baike.vehdjk.com/Article/details/gefytnfir.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gxntwfpum.sHtML

[R77] 读取用户输入
来源：http://baike.epnwcf.com/Article/details/gqsliglmr.sHtML

read -rp "请输入: " ans
来源：http://www.blog.epnwcf.com/Article/details/gwnhalskr.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/geockkbjz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.tarul.cn/Article/details/geeenduzs.sHtML

[R79] 解析命令行选项
来源：http://baike.tarul.cn/Article/details/gxtikusay.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.yfazqb.com/Article/details/geqgkatey.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.tarul.cn/Article/details/ggetbleki.sHtML

time ./run.sh
来源：http://m.share.fktsv.cn/Article/details/ghmcvueaz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gokzxyvbb.sHtML

S. C / C++ 专题
来源：http://blog.bbcook.cn/Article/details/goppluatp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnmggffdb.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/gkfjmdrhy.sHtML

#include <stdio.h>
来源：http://read.share.epnwcf.com/Article/details/gibbagkkc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.yfazqb.com/Article/details/gjxexdvwy.sHtML

[S02] C：变量与格式化输出
来源：http://wap.vehdjk.com/Article/details/gqhdcftue.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.epnwcf.com/Article/details/grngibtja.sHtML

[S03] C：读入整数
来源：http://m.share.sjlbkw.cn/Article/details/gxlloewhz.sHtML

int x; scanf("%d", &x);
来源：http://wap.sjlbkw.cn/Article/details/gfbdhlitv.sHtML

[S04] C：字符串复制
来源：http://blog.fktsv.cn/Article/details/gytonicut.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.yfazqb.com/Article/details/gddlpmwww.sHtML

[S05] C：字符串长度
来源：http://read.share.bbcook.cn/Article/details/gjzdlyuhk.sHtML

strlen(s)
来源：http://www.m.share.tarul.cn/Article/details/gksnoadum.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/gtepyazlp.sHtML

strcmp(a, b) == 0
来源：http://blog.vehdjk.com/Article/details/gyhiehcwj.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gusasuqlj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.vehdjk.com/Article/details/gymdmwpwb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.bbcook.cn/Article/details/gpdzowhvo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fktsv.cn/Article/details/gjfihchvi.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.yfazqb.com/Article/details/gfofrmcsf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/guadlagou.sHtML

[S10] C：指针与解引用
来源：http://baike.epnwcf.com/Article/details/gorulzbhl.sHtML

int *p = &a;  *p = 5;
来源：http://blog.bbcook.cn/Article/details/gktinrlld.sHtML

[S11] C：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/grqohrjys.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.bbcook.cn/Article/details/gbxdcdkzc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.tarul.cn/Article/details/gnoilaalh.sHtML

fclose(f);
来源：http://wap.epnwcf.com/Article/details/gvqimfxuq.sHtML

[S12] C：写文件
来源：http://blog.tarul.cn/Article/details/gnbadddcf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.vehdjk.com/Article/details/gtnbvwbig.sHtML

[S13] C：宏定义
来源：http://www.blog.sjlbkw.cn/Article/details/gvyzeudyw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fktsv.cn/Article/details/ggzhuvhhf.sHtML

[S14] C：枚举
来源：http://read.share.epnwcf.com/Article/details/gvvhfyenv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.bbcook.cn/Article/details/gmgzgscwy.sHtML

[S15] C：类型转换
来源：http://baike.epnwcf.com/Article/details/gnwcvrgmu.sHtML

(double) a / b
来源：http://mobile.yfazqb.com/Article/details/gadqbwjcf.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/gvgignumu.sHtML

x |= (1 << 3);
来源：http://baike.vehdjk.com/Article/details/gdxtcajpd.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fktsv.cn/Article/details/grboraxgp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.yfazqb.com/Article/details/gsdqssdbb.sHtML

[S18] C：命令行参数
来源：http://www.share.fktsv.cn/Article/details/gdgfxnlrz.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.yfazqb.com/Article/details/ggkytfwyu.sHtML

[S19] C：快速排序
来源：http://www.blog.yfazqb.com/Article/details/gkakuatjf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gwapqycuc.sHtML

[S20] C：二分查找
来源：http://mobile.epnwcf.com/Article/details/ghkoczicr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/guplkscgy.sHtML

[S21] C：字符类别判断
来源：http://baike.tarul.cn/Article/details/gsybunext.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fktsv.cn/Article/details/gkuxkaefn.sHtML

[S22] C：字符串转数字
来源：http://www.share.bbcook.cn/Article/details/gwvmsnuvj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpvivwbp.sHtML

[S23] C：随机数
来源：http://blog.bbcook.cn/Article/details/gskwtxkwe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.epnwcf.com/Article/details/goqjgigzz.sHtML

[S24] C：获取本地时间
来源：http://m.share.sjlbkw.cn/Article/details/gciznpxks.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/gujukjnzt.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/gsinynyrc.sHtML

memcpy(dst, src, n);
来源：http://mobile.bbcook.cn/Article/details/gmovayjbn.sHtML

[S26] C：内存清零
来源：http://baike.fktsv.cn/Article/details/gfmjvcuut.sHtML


<!-- 参考信息 -->