代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.tarul.cn/Article/details/gluztapvp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.sjlbkw.cn/Article/details/gjtsrhhsx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.tarul.cn/Article/details/gvuostkbd.sHtML

[Q57] 行号
来源：http://wap.bbcook.cn/Article/details/gjzywxdqq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.tarul.cn/Article/details/guxcdmoyf.sHtML

[Q58] 累计求和
来源：http://www.blog.yfazqb.com/Article/details/gtevclsgy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gplnqdtxd.sHtML

[Q59] 分组内累计
来源：http://read.share.tarul.cn/Article/details/gklasudtd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gbvjrduch.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.vehdjk.com/Article/details/gmsbdbzjg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.yfazqb.com/Article/details/gwbwoybej.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gntjyhipw.sHtML

[Q61] 移动平均
来源：http://blog.sjlbkw.cn/Article/details/gjcplggzu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gczkyxway.sHtML

[Q62] 分组占比
来源：http://www.share.fktsv.cn/Article/details/gfaegbscu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gbxhysdgp.sHtML

[Q63] 开启事务
来源：http://blog.vehdjk.com/Article/details/gaqifmpci.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.bbcook.cn/Article/details/glkgddbow.sHtML

[Q64] 提交事务
来源：http://m.share.vehdjk.com/Article/details/gvalidbtv.sHtML

COMMIT;
来源：http://www.blog.tarul.cn/Article/details/gpqqjtkbe.sHtML

[Q65] 回滚事务
来源：http://3g.bbcook.cn/Article/details/giwzxslmq.sHtML

ROLLBACK;
来源：http://read.share.vehdjk.com/Article/details/gacgcvmxf.sHtML

[Q66] 行锁查询
来源：http://read.share.tarul.cn/Article/details/gguzwdmin.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.tarul.cn/Article/details/gwgqbhmpm.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.epnwcf.com/Article/details/gnypredue.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.yfazqb.com/Article/details/ggmcgvjit.sHtML

[Q68] 保存点
来源：http://baike.fktsv.cn/Article/details/guyrokhks.sHtML

SAVEPOINT sp1;
来源：http://mobile.tarul.cn/Article/details/gypsrtffv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.vehdjk.com/Article/details/gxthafqle.sHtML

[Q69] 查看执行计划
来源：http://m.share.epnwcf.com/Article/details/gozprihzy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.bbcook.cn/Article/details/giyzgmnwo.sHtML

[Q70] 更新统计信息
来源：http://www.share.epnwcf.com/Article/details/ggdrrhtww.sHtML

ANALYZE TABLE users;
来源：http://m.share.epnwcf.com/Article/details/gylyaswpd.sHtML

[Q71] 查看建表语句
来源：http://3g.vehdjk.com/Article/details/gucnubjdg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.tarul.cn/Article/details/glndhcuqh.sHtML

[Q72] 查看索引
来源：http://m.share.sjlbkw.cn/Article/details/guejtodye.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gfmwmmgtr.sHtML

[Q73] 查看表状态
来源：http://m.share.yfazqb.com/Article/details/gjncxfyoc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.sjlbkw.cn/Article/details/gzvmputuh.sHtML

[Q74] 强制使用索引
来源：http://blog.bbcook.cn/Article/details/gymiykmqy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.yfazqb.com/Article/details/gsyqvfpsu.sHtML

[Q75] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gcaeibmfi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.epnwcf.com/Article/details/gcaidahru.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.vehdjk.com/Article/details/gymzabfop.sHtML

[Q76] 按天统计
来源：http://www.m.share.vehdjk.com/Article/details/gbfxojwmg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.vehdjk.com/Article/details/gazbrrvks.sHtML

[Q77] 时间加减
来源：http://mobile.bbcook.cn/Article/details/gibnerpuc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.yfazqb.com/Article/details/grqprhzsp.sHtML

[Q78] 当前时间
来源：http://blog.sjlbkw.cn/Article/details/gjdjyqlnw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.epnwcf.com/Article/details/gzkedzrhk.sHtML

[Q79] 字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gtjjkrdmz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/gbthidasw.sHtML

[Q80] 字符串截取
来源：http://www.blog.epnwcf.com/Article/details/gvjgzmsty.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gfhdbmgqj.sHtML

[Q81] 字符串替换
来源：http://blog.epnwcf.com/Article/details/gzxnuiasm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.yfazqb.com/Article/details/gzpzbesyz.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.bbcook.cn/Article/details/gdybogcmp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gnmrrzfkf.sHtML

[Q83] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/ggshpmddu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/glykomvzd.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fktsv.cn/Article/details/gtrndwdbv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/geefnmjln.sHtML

[Q85] 数值取整
来源：http://www.share.yfazqb.com/Article/details/gtgftrzeu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/gjnvixtaa.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.tarul.cn/Article/details/gfoicjnbt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.yfazqb.com/Article/details/grdtmnxrv.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fktsv.cn/Article/details/gcvtrnfnn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.yfazqb.com/Article/details/gzabslyum.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fktsv.cn/Article/details/gracjrtch.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.bbcook.cn/Article/details/giresijwc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gdfpujxjt.sHtML

[Q89] 判断表是否存在
来源：http://blog.epnwcf.com/Article/details/gnmtfhdxm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.sjlbkw.cn/Article/details/geqnkanam.sHtML

[Q90] 生成序号列
来源：http://www.share.vehdjk.com/Article/details/gvjcwlyax.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/gdlsvgylu.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggymoesmu.sHtML

R. Bash 专题
来源：http://www.share.bbcook.cn/Article/details/gxyofxnnf.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvqnxfftb.sHtML

[R01] shebang 与严格模式
来源：http://wap.fktsv.cn/Article/details/gxublurac.sHtML

#!/usr/bin/env bash
来源：http://www.blog.epnwcf.com/Article/details/gkiudrlcc.sHtML

set -euo pipefail
来源：http://m.share.fktsv.cn/Article/details/gdnfckbtc.sHtML

[R02] 变量赋值与使用
来源：http://read.share.yfazqb.com/Article/details/gfhutmtln.sHtML

name="Tom"; echo "$name"
来源：http://blog.yfazqb.com/Article/details/gjdqhmnqw.sHtML

[R03] 只读变量
来源：http://www.m.share.vehdjk.com/Article/details/gdpjkfjby.sHtML

readonly PI=3.14
来源：http://m.share.bbcook.cn/Article/details/ggeqrouur.sHtML

[R04] 位置参数
来源：http://www.m.share.fktsv.cn/Article/details/gseesqevo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.bbcook.cn/Article/details/gnbaqftov.sHtML

[R05] 参数默认值
来源：http://baike.vehdjk.com/Article/details/gmxauxnjs.sHtML

name="${1:-default}"
来源：http://read.share.tarul.cn/Article/details/gzchjhftm.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gcidhnhct.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gqwwplooh.sHtML

[R07] if 判断文件
来源：http://wap.bbcook.cn/Article/details/gbsmirkqw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.bbcook.cn/Article/details/gezcvkpez.sHtML

[R08] 数值比较
来源：http://wap.yfazqb.com/Article/details/gbeiekvrf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.vehdjk.com/Article/details/gslpdzodk.sHtML

[R09] 字符串比较
来源：http://mobile.tarul.cn/Article/details/gjbbspvki.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gnqhmctes.sHtML

[R10] 正则匹配
来源：http://www.blog.sjlbkw.cn/Article/details/glzfxhfvx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fktsv.cn/Article/details/gterqbpvx.sHtML

[R11] case 多分支
来源：http://baike.sjlbkw.cn/Article/details/gpwirnari.sHtML

case "$1" in
来源：http://read.share.yfazqb.com/Article/details/ggfukqtbp.sHtML

start) echo "启动" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gszjxaiih.sHtML

stop)  echo "停止" ;;
来源：http://blog.epnwcf.com/Article/details/gvdysavkd.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gzkxaeqki.sHtML

esac
来源：http://mobile.yfazqb.com/Article/details/gcwchewnf.sHtML

[R12] for 遍历文件
来源：http://mobile.fktsv.cn/Article/details/grzvmhxwq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.vehdjk.com/Article/details/gfrmbjggq.sHtML

[R13] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/gvsmwjova.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/gyhrmqxrn.sHtML

[R14] C 风格 for
来源：http://mobile.sjlbkw.cn/Article/details/ggutppjul.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/giznwhpko.sHtML

[R15] while 逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gufyhzdbk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.tarul.cn/Article/details/gmniqnlaj.sHtML

[R16] until 等待条件
来源：http://blog.sjlbkw.cn/Article/details/gxmxcbwog.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gveqexyio.sHtML

[R17] 数组定义与取值
来源：http://read.share.fktsv.cn/Article/details/gqonrabfx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/gzblqlxag.sHtML

[R18] 遍历数组
来源：http://baike.sjlbkw.cn/Article/details/gvqcertoy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.tarul.cn/Article/details/glipozmim.sHtML

[R19] 数组长度
来源：http://www.blog.tarul.cn/Article/details/gleanrswz.sHtML

echo "${#arr[@]}"
来源：http://m.share.tarul.cn/Article/details/gtvirwoff.sHtML

[R20] 关联数组（字典）
来源：http://m.share.bbcook.cn/Article/details/ghbktzvfg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.bbcook.cn/Article/details/gydewumiz.sHtML

[R21] 字符串长度
来源：http://www.share.yfazqb.com/Article/details/geecoqgdc.sHtML

echo "${#s}"
来源：http://read.share.epnwcf.com/Article/details/gncempnve.sHtML

[R22] 截取子串
来源：http://mobile.tarul.cn/Article/details/glpmkegpu.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/gwkhynxjt.sHtML

[R23] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gvkhykakx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.yfazqb.com/Article/details/gluxahhxs.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gesxpyuzy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.yfazqb.com/Article/details/giollvoid.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.bbcook.cn/Article/details/gthjlovor.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.tarul.cn/Article/details/gexyyvgnr.sHtML

[R26] 命令替换
来源：http://3g.epnwcf.com/Article/details/ghzekqcbi.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fktsv.cn/Article/details/gnqkfzkjf.sHtML

[R27] 算术展开
来源：http://m.share.epnwcf.com/Article/details/gwyciwthb.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.epnwcf.com/Article/details/gzedjrgvm.sHtML

[R28] 浮点运算
来源：http://www.m.share.vehdjk.com/Article/details/ggdzbntna.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.vehdjk.com/Article/details/glsikalrb.sHtML

[R29] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gsudkgqof.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.yfazqb.com/Article/details/gnycukrbu.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fktsv.cn/Article/details/gooqybovn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.vehdjk.com/Article/details/gakyxsora.sHtML

[R31] 局部变量
来源：http://m.share.epnwcf.com/Article/details/gzecvaekl.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.vehdjk.com/Article/details/gllaqetir.sHtML

[R32] 参数个数校验
来源：http://read.share.fktsv.cn/Article/details/gcjqyqjiz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.epnwcf.com/Article/details/gzuhqtrqf.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.epnwcf.com/Article/details/gubongspo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.yfazqb.com/Article/details/gkxeesaje.sHtML

[R34] 退出时清理
来源：http://m.share.fktsv.cn/Article/details/gebjgjspw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.tarul.cn/Article/details/gpgtbiddv.sHtML

[R35] 后台执行并等待
来源：http://read.share.fktsv.cn/Article/details/gcmrleztl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.sjlbkw.cn/Article/details/gceqxxxtc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.epnwcf.com/Article/details/gmivdofcb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/gcutnxnia.sHtML

[R37] 把输出赋给变量
来源：http://baike.vehdjk.com/Article/details/gazbrxway.sHtML

files=$(ls -1)
来源：http://m.share.epnwcf.com/Article/details/gqisxewky.sHtML

[R38] 管道串联
来源：http://www.m.share.sjlbkw.cn/Article/details/gfivjfvre.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.tarul.cn/Article/details/gvsdqnhwy.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.yfazqb.com/Article/details/gfpahunfc.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gtkczwgnz.sHtML

[R40] 追加写日志
来源：http://www.blog.vehdjk.com/Article/details/gwbwazsww.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/grgnqdxdq.sHtML

[R41] 丢弃输出
来源：http://m.share.fktsv.cn/Article/details/gfevceysu.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gyvtiyiiu.sHtML

[R42] 输入重定向
来源：http://m.share.tarul.cn/Article/details/gfmiuwneu.sHtML

wc -l < a.txt
来源：http://baike.bbcook.cn/Article/details/gmhyrjtbe.sHtML

[R43] 按名字查找文件
来源：http://www.share.fktsv.cn/Article/details/ggpkuxpbf.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gftiljieu.sHtML

[R44] 按修改时间查找
来源：http://baike.yfazqb.com/Article/details/gbtvurkpo.sHtML

find . -mtime -7 -type f
来源：http://3g.epnwcf.com/Article/details/gotayvdpj.sHtML

[R45] 批量删除
来源：http://baike.vehdjk.com/Article/details/gqocwwfdd.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/ggtmicxwq.sHtML

[R46] 递归替换文件内容
来源：http://mobile.sjlbkw.cn/Article/details/geoazsett.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.tarul.cn/Article/details/gatxvcrot.sHtML

[R47] sed 单行替换
来源：http://www.share.sjlbkw.cn/Article/details/gnzbaiixg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.vehdjk.com/Article/details/gvakwmfjj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.vehdjk.com/Article/details/gxeuhsjfu.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.epnwcf.com/Article/details/gfawaocdz.sHtML

[R49] awk 带条件
来源：http://3g.yfazqb.com/Article/details/gcoakvsgc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.yfazqb.com/Article/details/gzdsybjne.sHtML

[R50] awk 求和
来源：http://3g.vehdjk.com/Article/details/ggjcvsnnt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gjstiyows.sHtML

[R51] 排序去重取前几
来源：http://mobile.vehdjk.com/Article/details/guimzfhkl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.sjlbkw.cn/Article/details/gvfmurpee.sHtML

[R52] 统计行数
来源：http://wap.vehdjk.com/Article/details/gmojardkf.sHtML

wc -l a.txt
来源：http://3g.tarul.cn/Article/details/gnfheizrh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.vehdjk.com/Article/details/genisdbqc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/galgjydon.sHtML

[R54] 比较两个文件
来源：http://mobile.sjlbkw.cn/Article/details/gvznsbknk.sHtML

diff a.txt b.txt
来源：http://mobile.fktsv.cn/Article/details/gxebrivgv.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fktsv.cn/Article/details/ghjtrjvwm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.yfazqb.com/Article/details/gcghynfsh.sHtML

[R56] 远程拷贝
来源：http://www.blog.tarul.cn/Article/details/gtyjtsemf.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/ggtlixsaj.sHtML

[R57] 远程执行命令
来源：http://3g.bbcook.cn/Article/details/gbhhgtcfv.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/ggkwiaeyh.sHtML

[R58] 下载文件
来源：http://www.blog.bbcook.cn/Article/details/gzpuarbfn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.yfazqb.com/Article/details/gmjgjssux.sHtML

[R59] 发 POST JSON
来源：http://baike.bbcook.cn/Article/details/gbmcxkrgy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.bbcook.cn/Article/details/gofpehduu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/gfpjelzjx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.sjlbkw.cn/Article/details/ginixjsvs.sHtML

[R61] 磁盘占用
来源：http://wap.sjlbkw.cn/Article/details/gworkgptp.sHtML

df -h;  du -sh *
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyzoovlr.sHtML

[R62] 找最占空间的文件
来源：http://blog.tarul.cn/Article/details/gkqniwpzg.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.vehdjk.com/Article/details/gxxfuncmq.sHtML

[R63] 内存与进程
来源：http://m.share.fktsv.cn/Article/details/gncubgiev.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/gvulxsayv.sHtML

[R64] 结束进程
来源：http://read.share.epnwcf.com/Article/details/gtcwgrael.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.yfazqb.com/Article/details/gakeojkhv.sHtML

[R65] 查看端口占用
来源：http://www.share.sjlbkw.cn/Article/details/gvnhhkvna.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fktsv.cn/Article/details/gedmtnuyj.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/gxqkwypvt.sHtML

crontab -e;  crontab -l
来源：http://read.share.epnwcf.com/Article/details/gdirgtbux.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.bbcook.cn/Article/details/glbkfymps.sHtML

openssl rand -hex 16
来源：http://3g.tarul.cn/Article/details/glylicdfe.sHtML

[R68] 计算文件校验值
来源：http://mobile.vehdjk.com/Article/details/gegcsrimr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.sjlbkw.cn/Article/details/gnppaabhg.sHtML

[R69] 生成随机密码
来源：http://mobile.bbcook.cn/Article/details/gamtizaqm.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.vehdjk.com/Article/details/gtjuswhbr.sHtML

[R70] 时间戳与互转
来源：http://wap.yfazqb.com/Article/details/glowbudje.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fktsv.cn/Article/details/gkzgntdak.sHtML

[R71] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gbnzxnowz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.tarul.cn/Article/details/ggpzyqqsj.sHtML

[R72] 等待端口就绪
来源：http://wap.fktsv.cn/Article/details/gvpfpznej.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gcviptngx.sHtML

[R73] 分割大日志
来源：http://mobile.tarul.cn/Article/details/gzoxcasih.sHtML

split -l 1000 big.log part_
来源：http://baike.tarul.cn/Article/details/guqwwztjw.sHtML

[R74] 批量重命名
来源：http://m.share.epnwcf.com/Article/details/gofovxlrl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fktsv.cn/Article/details/gohsopgke.sHtML

[R75] 导出环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfeuznty.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.epnwcf.com/Article/details/gvrfgwujy.sHtML

[R76] 使用临时文件
来源：http://www.share.epnwcf.com/Article/details/gnmngjkiz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.bbcook.cn/Article/details/gzqapnhof.sHtML

[R77] 读取用户输入
来源：http://baike.fktsv.cn/Article/details/gnpohieth.sHtML

read -rp "请输入: " ans
来源：http://www.blog.yfazqb.com/Article/details/gbgqzrqht.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/gijeithvx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.yfazqb.com/Article/details/gpsiumxas.sHtML

[R79] 解析命令行选项
来源：http://3g.epnwcf.com/Article/details/gbjurnanz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.tarul.cn/Article/details/gsslorbri.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/ghtlpfxyt.sHtML

time ./run.sh
来源：http://read.share.epnwcf.com/Article/details/gcrqlsvfn.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gabqvmori.sHtML

S. C / C++ 专题
来源：http://www.share.bbcook.cn/Article/details/gseewoahd.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gpbsejiqf.sHtML

[S01] C：Hello World
来源：http://m.share.fktsv.cn/Article/details/gzqvaxhsd.sHtML

#include <stdio.h>
来源：http://mobile.yfazqb.com/Article/details/gbskxwmce.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fktsv.cn/Article/details/gtklhbtuo.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.sjlbkw.cn/Article/details/gjjxqdeum.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.sjlbkw.cn/Article/details/glsiyxpiy.sHtML

[S03] C：读入整数
来源：http://blog.epnwcf.com/Article/details/gczsgpqkh.sHtML

int x; scanf("%d", &x);
来源：http://blog.tarul.cn/Article/details/gjtzklagp.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/gadoxiplq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnffunkj.sHtML

[S05] C：字符串长度
来源：http://www.share.yfazqb.com/Article/details/gmqagdjqe.sHtML

strlen(s)
来源：http://3g.yfazqb.com/Article/details/gtcjqfrko.sHtML

[S06] C：字符串比较
来源：http://www.blog.tarul.cn/Article/details/gzuebzavk.sHtML

strcmp(a, b) == 0
来源：http://m.share.tarul.cn/Article/details/gqnziquzb.sHtML

[S07] C：数组遍历求和
来源：http://m.share.yfazqb.com/Article/details/gnnxlpcaa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.bbcook.cn/Article/details/gqbncqmed.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.sjlbkw.cn/Article/details/gdwevjoyp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fktsv.cn/Article/details/grpwknvpd.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.sjlbkw.cn/Article/details/gdpwgliaf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.vehdjk.com/Article/details/gmiojpgkk.sHtML

[S10] C：指针与解引用
来源：http://read.share.fktsv.cn/Article/details/gzaequjyy.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.bbcook.cn/Article/details/gndshqooo.sHtML

[S11] C：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gatsvhjgi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/gnmrvgtqi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.yfazqb.com/Article/details/gubcslfyk.sHtML

fclose(f);
来源：http://blog.fktsv.cn/Article/details/ghyehcyna.sHtML

[S12] C：写文件
来源：http://www.m.share.tarul.cn/Article/details/grvlcgigv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.vehdjk.com/Article/details/giiumgarx.sHtML

[S13] C：宏定义
来源：http://3g.fktsv.cn/Article/details/gnlffumdu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.yfazqb.com/Article/details/gzgdoevvu.sHtML

[S14] C：枚举
来源：http://3g.sjlbkw.cn/Article/details/gbxqjcuww.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.vehdjk.com/Article/details/gxlkmyajj.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/gslscclll.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqugzkjt.sHtML

[S16] C：位操作置位
来源：http://baike.sjlbkw.cn/Article/details/gufmfdkti.sHtML

x |= (1 << 3);
来源：http://wap.fktsv.cn/Article/details/gvayfmqlu.sHtML

[S17] C：安全拼接字符串
来源：http://blog.yfazqb.com/Article/details/gawktongy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.tarul.cn/Article/details/grsduwpup.sHtML

[S18] C：命令行参数
来源：http://www.share.fktsv.cn/Article/details/ggufckayh.sHtML

int main(int argc, char **argv)
来源：http://mobile.bbcook.cn/Article/details/gqfshzxvx.sHtML

[S19] C：快速排序
来源：http://baike.fktsv.cn/Article/details/gjsbjerll.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/gmqhlnoea.sHtML

[S20] C：二分查找
来源：http://wap.vehdjk.com/Article/details/ggoszkehd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/giqyjapea.sHtML

[S21] C：字符类别判断
来源：http://baike.vehdjk.com/Article/details/gzevemgic.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/grsziuxme.sHtML

[S22] C：字符串转数字
来源：http://3g.yfazqb.com/Article/details/gfpbmoylo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.sjlbkw.cn/Article/details/giwxyrtxg.sHtML

[S23] C：随机数
来源：http://mobile.vehdjk.com/Article/details/giiebkooq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.yfazqb.com/Article/details/gxwirfrou.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/gdffggmcd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.bbcook.cn/Article/details/gljquislw.sHtML

[S25] C：内存拷贝
来源：http://m.share.vehdjk.com/Article/details/ghohqahbl.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gbgrdswbt.sHtML

[S26] C：内存清零
来源：http://m.share.bbcook.cn/Article/details/gyjjuyxaa.sHtML


<!-- 参考信息 -->