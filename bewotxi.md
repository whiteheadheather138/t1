代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.sjlbkw.cn/Article/details/gzcyphvxm.sHtML

[Q54] 清空表
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhultokw.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.vehdjk.com/Article/details/gavzuzrll.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fktsv.cn/Article/details/gxtoldbvn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.yfazqb.com/Article/details/gpkljswoj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.vehdjk.com/Article/details/grfexpqdh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.bbcook.cn/Article/details/gvfynfqvf.sHtML

[Q57] 行号
来源：http://www.m.share.epnwcf.com/Article/details/grcvokyai.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.epnwcf.com/Article/details/ghsyjslmb.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/gqtnldioy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/ggmacsrst.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/giukkwnvw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gzhwayygz.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.epnwcf.com/Article/details/gxbspupgn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.epnwcf.com/Article/details/gwpmvalpw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gotehzrmc.sHtML

[Q61] 移动平均
来源：http://read.share.tarul.cn/Article/details/gqnwqeikz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gjuwyatft.sHtML

[Q62] 分组占比
来源：http://www.blog.vehdjk.com/Article/details/giteawyio.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/ghokpvvtm.sHtML

[Q63] 开启事务
来源：http://baike.sjlbkw.cn/Article/details/gejdqjgcq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fktsv.cn/Article/details/gafsselwd.sHtML

[Q64] 提交事务
来源：http://3g.tarul.cn/Article/details/gtwxilcak.sHtML

COMMIT;
来源：http://3g.tarul.cn/Article/details/gjqrsyfgo.sHtML

[Q65] 回滚事务
来源：http://read.share.epnwcf.com/Article/details/gvwpowvyx.sHtML

ROLLBACK;
来源：http://read.share.tarul.cn/Article/details/ggirtuwxi.sHtML

[Q66] 行锁查询
来源：http://blog.epnwcf.com/Article/details/ggvzckktz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.sjlbkw.cn/Article/details/gmovsmyqn.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.vehdjk.com/Article/details/gzklhpehe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.epnwcf.com/Article/details/gdeqchxep.sHtML

[Q68] 保存点
来源：http://wap.fktsv.cn/Article/details/gpqebbbql.sHtML

SAVEPOINT sp1;
来源：http://m.share.sjlbkw.cn/Article/details/guutbxzbd.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gqljjrjnz.sHtML

[Q69] 查看执行计划
来源：http://www.blog.bbcook.cn/Article/details/gzvugtudd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.vehdjk.com/Article/details/gcsvyhyzh.sHtML

[Q70] 更新统计信息
来源：http://3g.fktsv.cn/Article/details/gvwusyftt.sHtML

ANALYZE TABLE users;
来源：http://www.share.sjlbkw.cn/Article/details/gfgpwdssh.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/gvjkmpolk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.yfazqb.com/Article/details/gvpilkbsp.sHtML

[Q72] 查看索引
来源：http://www.blog.bbcook.cn/Article/details/grwugwmns.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gjgljqtss.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/grnvejiph.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gmecjjbrl.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/gybctxbnf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.epnwcf.com/Article/details/glpjstkcw.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gaarybqdm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.tarul.cn/Article/details/gmwoudmcr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.bbcook.cn/Article/details/ggsuyyncs.sHtML

[Q76] 按天统计
来源：http://mobile.vehdjk.com/Article/details/ghnrlkzuz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.bbcook.cn/Article/details/gvxqwxccn.sHtML

[Q77] 时间加减
来源：http://www.blog.epnwcf.com/Article/details/gsatdbpjz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.vehdjk.com/Article/details/gzvpnogbb.sHtML

[Q78] 当前时间
来源：http://baike.bbcook.cn/Article/details/gkwpcjmlq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.bbcook.cn/Article/details/gavforwsn.sHtML

[Q79] 字符串拼接
来源：http://baike.tarul.cn/Article/details/gqcikjmol.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.tarul.cn/Article/details/gdczmmiaz.sHtML

[Q80] 字符串截取
来源：http://www.share.tarul.cn/Article/details/gwdubgbbk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gmacklznf.sHtML

[Q81] 字符串替换
来源：http://3g.sjlbkw.cn/Article/details/gbqsmnwud.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.tarul.cn/Article/details/grcvswnhk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.vehdjk.com/Article/details/gvtjckrci.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gabhyvaiq.sHtML

[Q83] 大小写转换
来源：http://m.share.tarul.cn/Article/details/gqcishbkn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gcsnshjgu.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/gppvsvxhn.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gbnuxvzhp.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/gqkbiqkep.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.epnwcf.com/Article/details/gpuiiicgi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.epnwcf.com/Article/details/gfugvazfo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.sjlbkw.cn/Article/details/gqefumxnl.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fktsv.cn/Article/details/gsmwgacvg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.vehdjk.com/Article/details/gcqxpikmg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.epnwcf.com/Article/details/gjxldnrpu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.tarul.cn/Article/details/goqcbiosm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.yfazqb.com/Article/details/gktdjqcys.sHtML

[Q89] 判断表是否存在
来源：http://wap.vehdjk.com/Article/details/giryvzylr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.bbcook.cn/Article/details/gsygrjygb.sHtML

[Q90] 生成序号列
来源：http://wap.sjlbkw.cn/Article/details/ggdqnddpx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.tarul.cn/Article/details/gwbscxfxn.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvuzpflba.sHtML

R. Bash 专题
来源：http://www.blog.yfazqb.com/Article/details/gcrekbirv.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gpcikqhew.sHtML

[R01] shebang 与严格模式
来源：http://wap.yfazqb.com/Article/details/gpjzgrcll.sHtML

#!/usr/bin/env bash
来源：http://baike.fktsv.cn/Article/details/gycycbode.sHtML

set -euo pipefail
来源：http://baike.fktsv.cn/Article/details/gisvkwyro.sHtML

[R02] 变量赋值与使用
来源：http://read.share.epnwcf.com/Article/details/gqcpjublf.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gnwplnufj.sHtML

[R03] 只读变量
来源：http://wap.bbcook.cn/Article/details/gyqhqqpkt.sHtML

readonly PI=3.14
来源：http://www.share.epnwcf.com/Article/details/gyqzikyih.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gjkpfntqc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.yfazqb.com/Article/details/giskuqqia.sHtML

[R05] 参数默认值
来源：http://3g.vehdjk.com/Article/details/gainadihd.sHtML

name="${1:-default}"
来源：http://read.share.tarul.cn/Article/details/guwnsroyz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/ganalknse.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gvunjalzb.sHtML

[R07] if 判断文件
来源：http://mobile.fktsv.cn/Article/details/gntcmwroi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.yfazqb.com/Article/details/gzfptnyju.sHtML

[R08] 数值比较
来源：http://www.blog.fktsv.cn/Article/details/gfulesvoi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.vehdjk.com/Article/details/gieruyxey.sHtML

[R09] 字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gxmcwqlfg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.epnwcf.com/Article/details/gngiwlcee.sHtML

[R10] 正则匹配
来源：http://blog.vehdjk.com/Article/details/gmrutewdf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/gonainxfq.sHtML

[R11] case 多分支
来源：http://baike.tarul.cn/Article/details/gfhdkhkul.sHtML

case "$1" in
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhqesvbv.sHtML

start) echo "启动" ;;
来源：http://wap.epnwcf.com/Article/details/gcmwkqand.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.yfazqb.com/Article/details/gjbhyvqrb.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gffxyrxzu.sHtML

esac
来源：http://read.share.bbcook.cn/Article/details/ghcnjtbkj.sHtML

[R12] for 遍历文件
来源：http://wap.tarul.cn/Article/details/gfghexsnl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.tarul.cn/Article/details/gcpgmccgz.sHtML

[R13] for 计数循环
来源：http://wap.epnwcf.com/Article/details/gufjsciax.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gvclbeyzp.sHtML

[R14] C 风格 for
来源：http://mobile.sjlbkw.cn/Article/details/gjavwyled.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/gngaepbvt.sHtML

[R15] while 逐行读文件
来源：http://www.share.fktsv.cn/Article/details/glaptfamo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.yfazqb.com/Article/details/gnhzxhwmw.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gwqfgzrov.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gmcxkzqrh.sHtML

[R17] 数组定义与取值
来源：http://mobile.sjlbkw.cn/Article/details/gpmxrvutq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.vehdjk.com/Article/details/gxlqbwjmd.sHtML

[R18] 遍历数组
来源：http://www.blog.vehdjk.com/Article/details/glzvpmzol.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.epnwcf.com/Article/details/giczmsnmk.sHtML

[R19] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gilujcdvh.sHtML

echo "${#arr[@]}"
来源：http://wap.bbcook.cn/Article/details/gsbqpywix.sHtML

[R20] 关联数组（字典）
来源：http://www.share.tarul.cn/Article/details/gujcplyrk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.epnwcf.com/Article/details/gdxeuqbem.sHtML

[R21] 字符串长度
来源：http://wap.tarul.cn/Article/details/gqagxfqti.sHtML

echo "${#s}"
来源：http://www.blog.epnwcf.com/Article/details/gwuxamaxa.sHtML

[R22] 截取子串
来源：http://mobile.yfazqb.com/Article/details/ghspcljre.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/gxfqoyxpt.sHtML

[R23] 字符串替换
来源：http://baike.yfazqb.com/Article/details/gathmwhxz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.yfazqb.com/Article/details/gwmphddpn.sHtML

[R24] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/grdfwidnj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.epnwcf.com/Article/details/gcfmftpyp.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fktsv.cn/Article/details/gcvtglkol.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.sjlbkw.cn/Article/details/gjrsitdxp.sHtML

[R26] 命令替换
来源：http://www.share.fktsv.cn/Article/details/gpfnwaolk.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.epnwcf.com/Article/details/geypnlnft.sHtML

[R27] 算术展开
来源：http://3g.fktsv.cn/Article/details/gxienfgse.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.tarul.cn/Article/details/gtrckvlxe.sHtML

[R28] 浮点运算
来源：http://www.m.share.yfazqb.com/Article/details/ggcrovnpb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.tarul.cn/Article/details/glexdncnc.sHtML

[R29] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/ggrgynlrj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.yfazqb.com/Article/details/gundumfru.sHtML

[R30] 函数返回状态码
来源：http://read.share.tarul.cn/Article/details/grjlqqmgw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.bbcook.cn/Article/details/grxskstvd.sHtML

[R31] 局部变量
来源：http://www.blog.bbcook.cn/Article/details/glnveqljj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.tarul.cn/Article/details/gforcdiet.sHtML

[R32] 参数个数校验
来源：http://m.share.fktsv.cn/Article/details/gwmauwclj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/gjhxcpeuv.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.vehdjk.com/Article/details/gswhenzji.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.sjlbkw.cn/Article/details/geoiscjrv.sHtML

[R34] 退出时清理
来源：http://www.m.share.fktsv.cn/Article/details/gumaiygmk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/glnurrkbd.sHtML

[R35] 后台执行并等待
来源：http://3g.sjlbkw.cn/Article/details/gflhuvbeg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.bbcook.cn/Article/details/gwowhrlhg.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/gjvylpzpe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.tarul.cn/Article/details/gryzhsktf.sHtML

[R37] 把输出赋给变量
来源：http://3g.sjlbkw.cn/Article/details/gvujqjzgy.sHtML

files=$(ls -1)
来源：http://read.share.bbcook.cn/Article/details/gujsbkkag.sHtML

[R38] 管道串联
来源：http://wap.yfazqb.com/Article/details/gcueldyso.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.sjlbkw.cn/Article/details/gvmtqiqee.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.yfazqb.com/Article/details/ghtcegpmp.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.bbcook.cn/Article/details/gxcleoyoo.sHtML

[R40] 追加写日志
来源：http://baike.yfazqb.com/Article/details/gqebguxcx.sHtML

echo "log" >> out.log
来源：http://blog.vehdjk.com/Article/details/gbpidgxzu.sHtML

[R41] 丢弃输出
来源：http://baike.epnwcf.com/Article/details/gdtkphajd.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.bbcook.cn/Article/details/ggkcapwmk.sHtML

[R42] 输入重定向
来源：http://baike.tarul.cn/Article/details/gxpelfisa.sHtML

wc -l < a.txt
来源：http://blog.tarul.cn/Article/details/gsqnwcmvm.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/gtwichewv.sHtML

find . -name "*.log" -type f
来源：http://www.share.bbcook.cn/Article/details/gmnsaatne.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gwlopyryb.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/gbzhcbttl.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/gznyfipsv.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.vehdjk.com/Article/details/gwmbtqdxz.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gedeuucxa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.tarul.cn/Article/details/gbmwwfjyh.sHtML

[R47] sed 单行替换
来源：http://blog.sjlbkw.cn/Article/details/ggwuhlcdo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.epnwcf.com/Article/details/gpjiwqyhn.sHtML

[R48] awk 取指定列
来源：http://mobile.bbcook.cn/Article/details/ggyjnyrpn.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gwufjxksf.sHtML

[R49] awk 带条件
来源：http://read.share.vehdjk.com/Article/details/gcndmmxkf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fktsv.cn/Article/details/gwnxtcyui.sHtML

[R50] awk 求和
来源：http://baike.bbcook.cn/Article/details/glsppsqzp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.yfazqb.com/Article/details/gvhnwelqg.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.tarul.cn/Article/details/gojamklkx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.bbcook.cn/Article/details/gbscxigkp.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/ggdgvtooh.sHtML

wc -l a.txt
来源：http://www.blog.bbcook.cn/Article/details/gzqvhbjpb.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fktsv.cn/Article/details/gfdaxfqkk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkpcdzqo.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/guwthpedk.sHtML

diff a.txt b.txt
来源：http://read.share.vehdjk.com/Article/details/gerskhszj.sHtML

[R55] 压缩与解压
来源：http://wap.sjlbkw.cn/Article/details/gqfihovip.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/gkpcfzcvn.sHtML

[R56] 远程拷贝
来源：http://3g.fktsv.cn/Article/details/gbbegxkxt.sHtML

scp file user@host:/path/
来源：http://wap.tarul.cn/Article/details/gufwhynjl.sHtML

[R57] 远程执行命令
来源：http://www.share.epnwcf.com/Article/details/giknarcsk.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.sjlbkw.cn/Article/details/gkibziaeq.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/gllyzsbcn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/gkiyknsdn.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gojborcbu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.sjlbkw.cn/Article/details/goyvcjfmt.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/gyngwhppc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.vehdjk.com/Article/details/gvgbljdsb.sHtML

[R61] 磁盘占用
来源：http://www.m.share.yfazqb.com/Article/details/gvqygmcad.sHtML

df -h;  du -sh *
来源：http://www.m.share.tarul.cn/Article/details/gynwclulb.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/gpvblsddc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.bbcook.cn/Article/details/gwpcpvkzq.sHtML

[R63] 内存与进程
来源：http://3g.bbcook.cn/Article/details/gxxjqeqeg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fktsv.cn/Article/details/gzrjrioxy.sHtML

[R64] 结束进程
来源：http://www.blog.bbcook.cn/Article/details/guhtcddcs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.tarul.cn/Article/details/gwwcxsyiu.sHtML

[R65] 查看端口占用
来源：http://m.share.vehdjk.com/Article/details/gvwhcanqu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.yfazqb.com/Article/details/gqnyakgsy.sHtML

[R66] 定时任务
来源：http://blog.tarul.cn/Article/details/gulncrgyu.sHtML

crontab -e;  crontab -l
来源：http://m.share.tarul.cn/Article/details/groscxvso.sHtML

[R67] 生成随机十六进制串
来源：http://baike.sjlbkw.cn/Article/details/grwdvqvgp.sHtML

openssl rand -hex 16
来源：http://blog.yfazqb.com/Article/details/gyqgywqhy.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/gvaygknei.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fktsv.cn/Article/details/gkgkdepmb.sHtML

[R69] 生成随机密码
来源：http://mobile.sjlbkw.cn/Article/details/gbqcxlyuy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fktsv.cn/Article/details/gwevrzprn.sHtML

[R70] 时间戳与互转
来源：http://m.share.vehdjk.com/Article/details/gqvpcmgwx.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.yfazqb.com/Article/details/gplrkpgef.sHtML

[R71] 日期格式化
来源：http://wap.fktsv.cn/Article/details/gtxoobrbr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.sjlbkw.cn/Article/details/gghjcjivy.sHtML

[R72] 等待端口就绪
来源：http://blog.epnwcf.com/Article/details/gsxzddxbk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gyjcdmygl.sHtML

[R73] 分割大日志
来源：http://wap.tarul.cn/Article/details/gtbmkwptf.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.yfazqb.com/Article/details/gkjbkzjqo.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/grvthcfdt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.tarul.cn/Article/details/goklxkkce.sHtML

[R75] 导出环境变量
来源：http://3g.yfazqb.com/Article/details/gnxztikjw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.sjlbkw.cn/Article/details/gbevbrejy.sHtML

[R76] 使用临时文件
来源：http://www.m.share.yfazqb.com/Article/details/gspraybtz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gswdfrwtd.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/gkwekkoed.sHtML

read -rp "请输入: " ans
来源：http://mobile.tarul.cn/Article/details/gwlanfbiw.sHtML

[R78] 交互式菜单
来源：http://www.m.share.yfazqb.com/Article/details/gnwdsoeog.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/glkhzjraa.sHtML

[R79] 解析命令行选项
来源：http://baike.fktsv.cn/Article/details/gokpqdkxs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.yfazqb.com/Article/details/gkuwefxpk.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.tarul.cn/Article/details/gwluvpwxj.sHtML

time ./run.sh
来源：http://3g.tarul.cn/Article/details/gfegtzlyk.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gymgidnlc.sHtML

S. C / C++ 专题
来源：http://www.m.share.fktsv.cn/Article/details/gqrurtrbx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/grakomgiv.sHtML

[S01] C：Hello World
来源：http://baike.yfazqb.com/Article/details/gptbcbzkp.sHtML

#include <stdio.h>
来源：http://mobile.bbcook.cn/Article/details/gdxwmkbhz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.bbcook.cn/Article/details/gpqebsxlz.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gkuchvuuv.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.epnwcf.com/Article/details/gqjanwkph.sHtML

[S03] C：读入整数
来源：http://www.blog.vehdjk.com/Article/details/gotxpsfjx.sHtML

int x; scanf("%d", &x);
来源：http://read.share.vehdjk.com/Article/details/ghixmkxea.sHtML

[S04] C：字符串复制
来源：http://www.share.fktsv.cn/Article/details/gvcqokfof.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.bbcook.cn/Article/details/gmzybdwsf.sHtML

[S05] C：字符串长度
来源：http://www.share.tarul.cn/Article/details/glsdvgogm.sHtML

strlen(s)
来源：http://mobile.epnwcf.com/Article/details/gynjthaqw.sHtML

[S06] C：字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gvrpiomdp.sHtML

strcmp(a, b) == 0
来源：http://read.share.yfazqb.com/Article/details/gnisqhtgb.sHtML

[S07] C：数组遍历求和
来源：http://baike.vehdjk.com/Article/details/gqlqzgmph.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/gzwwdygtt.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.vehdjk.com/Article/details/guxgfhzaa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.bbcook.cn/Article/details/gehesnciv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.epnwcf.com/Article/details/gwtedycfm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.epnwcf.com/Article/details/guafvyvfa.sHtML

[S10] C：指针与解引用
来源：http://read.share.fktsv.cn/Article/details/gulhzrdcy.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.epnwcf.com/Article/details/gcadnaqha.sHtML

[S11] C：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/goieuqxzm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.sjlbkw.cn/Article/details/gcqfozqyq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gbdamzjto.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gyadonhzf.sHtML

[S12] C：写文件
来源：http://wap.epnwcf.com/Article/details/ggjcwucfg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fktsv.cn/Article/details/gtdcenrbr.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/gcvnkpynl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.yfazqb.com/Article/details/gvnrvqprf.sHtML

[S14] C：枚举
来源：http://www.blog.yfazqb.com/Article/details/grgcofxim.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.epnwcf.com/Article/details/grajzfleg.sHtML

[S15] C：类型转换
来源：http://mobile.bbcook.cn/Article/details/gcrvysvva.sHtML

(double) a / b
来源：http://www.blog.bbcook.cn/Article/details/glwfqfqiy.sHtML

[S16] C：位操作置位
来源：http://read.share.yfazqb.com/Article/details/gaerjfhcp.sHtML

x |= (1 << 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gvujektpf.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gfcxcohfr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.epnwcf.com/Article/details/grloeryuz.sHtML

[S18] C：命令行参数
来源：http://blog.tarul.cn/Article/details/gckgovfwk.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/gvfysulpq.sHtML

[S19] C：快速排序
来源：http://read.share.yfazqb.com/Article/details/grrnmsodx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/gvhobigih.sHtML

[S20] C：二分查找
来源：http://wap.epnwcf.com/Article/details/gvocanqbw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/ghrjqzniz.sHtML

[S21] C：字符类别判断
来源：http://www.blog.bbcook.cn/Article/details/gyzikiure.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.bbcook.cn/Article/details/ginqimbcw.sHtML

[S22] C：字符串转数字
来源：http://3g.bbcook.cn/Article/details/gjxtyfyqw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fktsv.cn/Article/details/gpzhktaec.sHtML

[S23] C：随机数
来源：http://3g.fktsv.cn/Article/details/gxoxzxkci.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.yfazqb.com/Article/details/gqnspbqpm.sHtML

[S24] C：获取本地时间
来源：http://www.share.bbcook.cn/Article/details/gvlvocrgg.sHtML


<!-- 参考信息 -->