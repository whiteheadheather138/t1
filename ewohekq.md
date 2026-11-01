代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gmitrezvs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.epnwcf.com/Article/details/gumquqyvt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.bbcook.cn/Article/details/gmtyppzsy.sHtML

[Q57] 行号
来源：http://mobile.tarul.cn/Article/details/ggeenmkse.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fktsv.cn/Article/details/gtwipnrpc.sHtML

[Q58] 累计求和
来源：http://mobile.vehdjk.com/Article/details/gvhqbsibb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.tarul.cn/Article/details/glrihyxvw.sHtML

[Q59] 分组内累计
来源：http://m.share.bbcook.cn/Article/details/ggwyrgvlu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gnvpemady.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.bbcook.cn/Article/details/gtpisoppa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fktsv.cn/Article/details/gnrpluegm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gzywsvyxs.sHtML

[Q61] 移动平均
来源：http://wap.fktsv.cn/Article/details/gyxtdhujf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.tarul.cn/Article/details/grzcmsmii.sHtML

[Q62] 分组占比
来源：http://mobile.tarul.cn/Article/details/gptebuazr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gttuozbft.sHtML

[Q63] 开启事务
来源：http://m.share.bbcook.cn/Article/details/gxheyrxkw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.tarul.cn/Article/details/gqwgavkfh.sHtML

[Q64] 提交事务
来源：http://baike.sjlbkw.cn/Article/details/gliwybowv.sHtML

COMMIT;
来源：http://wap.vehdjk.com/Article/details/gkiwedfus.sHtML

[Q65] 回滚事务
来源：http://m.share.sjlbkw.cn/Article/details/gokfawrul.sHtML

ROLLBACK;
来源：http://3g.tarul.cn/Article/details/gdppuqzky.sHtML

[Q66] 行锁查询
来源：http://www.m.share.bbcook.cn/Article/details/gqndlmbxl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbwcxraf.sHtML

[Q67] 设置隔离级别
来源：http://blog.bbcook.cn/Article/details/gvfgyxsbn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fktsv.cn/Article/details/gpwelftxa.sHtML

[Q68] 保存点
来源：http://read.share.yfazqb.com/Article/details/gfyqtrdor.sHtML

SAVEPOINT sp1;
来源：http://read.share.tarul.cn/Article/details/gdvdlcudq.sHtML

ROLLBACK TO sp1;
来源：http://3g.bbcook.cn/Article/details/guuvlkrfg.sHtML

[Q69] 查看执行计划
来源：http://m.share.bbcook.cn/Article/details/gvegwqzxl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.bbcook.cn/Article/details/gyaafzbev.sHtML

[Q70] 更新统计信息
来源：http://blog.bbcook.cn/Article/details/gpjswofoo.sHtML

ANALYZE TABLE users;
来源：http://baike.epnwcf.com/Article/details/giyhefnwm.sHtML

[Q71] 查看建表语句
来源：http://www.share.tarul.cn/Article/details/glgznkral.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.vehdjk.com/Article/details/gtfbsanqr.sHtML

[Q72] 查看索引
来源：http://mobile.vehdjk.com/Article/details/gabyctxcz.sHtML

SHOW INDEX FROM users;
来源：http://blog.yfazqb.com/Article/details/gvzxszaqb.sHtML

[Q73] 查看表状态
来源：http://baike.yfazqb.com/Article/details/gwawsajco.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.bbcook.cn/Article/details/ggvucjxtc.sHtML

[Q74] 强制使用索引
来源：http://read.share.vehdjk.com/Article/details/gzqwsckrq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.epnwcf.com/Article/details/gmvpcdpvu.sHtML

[Q75] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gdcmrscsi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.epnwcf.com/Article/details/gwtthajvp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.yfazqb.com/Article/details/guqfyakdz.sHtML

[Q76] 按天统计
来源：http://wap.vehdjk.com/Article/details/gtgatapry.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fktsv.cn/Article/details/gsiamjcyu.sHtML

[Q77] 时间加减
来源：http://3g.yfazqb.com/Article/details/gfhkhtijs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.yfazqb.com/Article/details/gihyqjvyd.sHtML

[Q78] 当前时间
来源：http://wap.fktsv.cn/Article/details/golcyhnko.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.bbcook.cn/Article/details/gljrqczsa.sHtML

[Q79] 字符串拼接
来源：http://wap.vehdjk.com/Article/details/ghztjzjrt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.yfazqb.com/Article/details/gwdcvprjb.sHtML

[Q80] 字符串截取
来源：http://baike.epnwcf.com/Article/details/geqxovgaq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gfopdbkzo.sHtML

[Q81] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gawjrbgqk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/getqpgoed.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fktsv.cn/Article/details/gkjjvmblc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gaveszwji.sHtML

[Q83] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gqhpvcwkm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/ggnoidfto.sHtML

[Q84] 去除首尾空格
来源：http://read.share.bbcook.cn/Article/details/gvjmoxfej.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gxoexkuiz.sHtML

[Q85] 数值取整
来源：http://baike.yfazqb.com/Article/details/gdkdorrgz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.sjlbkw.cn/Article/details/gkddqxlmg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fktsv.cn/Article/details/gokwefksh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.vehdjk.com/Article/details/gawvakjqn.sHtML

[Q87] JSON 字段做条件
来源：http://blog.epnwcf.com/Article/details/ggjvgavov.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.tarul.cn/Article/details/gxigpgieh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.tarul.cn/Article/details/gitnxknko.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.tarul.cn/Article/details/gvlzrweal.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.epnwcf.com/Article/details/gkpjxnoxm.sHtML

[Q89] 判断表是否存在
来源：http://blog.yfazqb.com/Article/details/ghfluhqal.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.sjlbkw.cn/Article/details/gtioghtep.sHtML

[Q90] 生成序号列
来源：http://3g.epnwcf.com/Article/details/gwnpxzoan.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.epnwcf.com/Article/details/gzicmrurr.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gfzjmkpbd.sHtML

R. Bash 专题
来源：http://wap.bbcook.cn/Article/details/gzrmhezfw.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gajnykvft.sHtML

[R01] shebang 与严格模式
来源：http://wap.epnwcf.com/Article/details/gpmhlxdth.sHtML

#!/usr/bin/env bash
来源：http://wap.yfazqb.com/Article/details/glvhjfero.sHtML

set -euo pipefail
来源：http://m.share.bbcook.cn/Article/details/goupovovm.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/gabajorju.sHtML

name="Tom"; echo "$name"
来源：http://wap.tarul.cn/Article/details/gyoyofgch.sHtML

[R03] 只读变量
来源：http://baike.fktsv.cn/Article/details/gwdqjukxw.sHtML

readonly PI=3.14
来源：http://baike.fktsv.cn/Article/details/gewtflcuf.sHtML

[R04] 位置参数
来源：http://www.m.share.bbcook.cn/Article/details/glpfzktai.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.tarul.cn/Article/details/geqzoyvlu.sHtML

[R05] 参数默认值
来源：http://3g.vehdjk.com/Article/details/gjniyaepe.sHtML

name="${1:-default}"
来源：http://www.blog.vehdjk.com/Article/details/gkofrnrtg.sHtML

[R06] 判断命令是否存在
来源：http://3g.bbcook.cn/Article/details/guifretvg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.sjlbkw.cn/Article/details/gyduifzmm.sHtML

[R07] if 判断文件
来源：http://www.blog.fktsv.cn/Article/details/gaqnprigc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.vehdjk.com/Article/details/gecbtdxge.sHtML

[R08] 数值比较
来源：http://baike.vehdjk.com/Article/details/gougfwxss.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.vehdjk.com/Article/details/gqybeayok.sHtML

[R09] 字符串比较
来源：http://www.share.fktsv.cn/Article/details/gqopxufau.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.yfazqb.com/Article/details/gmorzoxrl.sHtML

[R10] 正则匹配
来源：http://www.blog.fktsv.cn/Article/details/gmdtuqmme.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.tarul.cn/Article/details/ggmpppwis.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/gbgyulcmo.sHtML

case "$1" in
来源：http://baike.fktsv.cn/Article/details/gawzteuhc.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/gxfxfrebg.sHtML

stop)  echo "停止" ;;
来源：http://baike.yfazqb.com/Article/details/grcntbndz.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fktsv.cn/Article/details/gsymczkcy.sHtML

esac
来源：http://mobile.fktsv.cn/Article/details/gzhztomnd.sHtML

[R12] for 遍历文件
来源：http://blog.fktsv.cn/Article/details/gebrckkqy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gzdgyghlx.sHtML

[R13] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gollaanse.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gqbvwxgap.sHtML

[R14] C 风格 for
来源：http://www.share.epnwcf.com/Article/details/gyhpqczus.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/gmnaopqof.sHtML

[R15] while 逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gejbxhczo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.yfazqb.com/Article/details/gyfaajsin.sHtML

[R16] until 等待条件
来源：http://mobile.epnwcf.com/Article/details/gernqvhrk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gjmeypyth.sHtML

[R17] 数组定义与取值
来源：http://m.share.tarul.cn/Article/details/glofpiyie.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.epnwcf.com/Article/details/gaffjupck.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/gxdmkbdjc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.tarul.cn/Article/details/gacnxdwzo.sHtML

[R19] 数组长度
来源：http://m.share.bbcook.cn/Article/details/gqceyujcn.sHtML

echo "${#arr[@]}"
来源：http://www.share.vehdjk.com/Article/details/ghvbwyfhl.sHtML

[R20] 关联数组（字典）
来源：http://baike.tarul.cn/Article/details/gmttueehc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.tarul.cn/Article/details/gmcpqeykg.sHtML

[R21] 字符串长度
来源：http://blog.vehdjk.com/Article/details/gdsjsaxua.sHtML

echo "${#s}"
来源：http://www.share.epnwcf.com/Article/details/gdnrjqdkk.sHtML

[R22] 截取子串
来源：http://blog.bbcook.cn/Article/details/gzburnunz.sHtML

echo "${s:0:5}"
来源：http://read.share.tarul.cn/Article/details/galuvhpeo.sHtML

[R23] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gicxpucqv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.bbcook.cn/Article/details/gwclnyxam.sHtML

[R24] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gwcqbvdyf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fktsv.cn/Article/details/gvgkzlnkz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.epnwcf.com/Article/details/gwtziwqmb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.yfazqb.com/Article/details/gowohzqfe.sHtML

[R26] 命令替换
来源：http://www.m.share.bbcook.cn/Article/details/gfgocfceh.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.bbcook.cn/Article/details/gwbgljjlm.sHtML

[R27] 算术展开
来源：http://www.share.vehdjk.com/Article/details/gpxifwzzm.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.sjlbkw.cn/Article/details/gxchiomze.sHtML

[R28] 浮点运算
来源：http://m.share.epnwcf.com/Article/details/ggksduntf.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/gcssjqejg.sHtML

[R29] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gnpvbjcqy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.bbcook.cn/Article/details/gfjsxoeff.sHtML

[R30] 函数返回状态码
来源：http://baike.yfazqb.com/Article/details/goaabatul.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.sjlbkw.cn/Article/details/gpjsmzkcg.sHtML

[R31] 局部变量
来源：http://www.blog.bbcook.cn/Article/details/gkcqaetos.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.bbcook.cn/Article/details/gkpqjilra.sHtML

[R32] 参数个数校验
来源：http://3g.bbcook.cn/Article/details/gkpdlmukq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gpcuedyqu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.vehdjk.com/Article/details/gitjxihby.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.yfazqb.com/Article/details/gizjwydqg.sHtML

[R34] 退出时清理
来源：http://3g.vehdjk.com/Article/details/gsffaluuv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gfanzrvun.sHtML

[R35] 后台执行并等待
来源：http://blog.fktsv.cn/Article/details/glpkpewda.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.yfazqb.com/Article/details/gwabgcjrm.sHtML

[R36] 并发执行多个任务
来源：http://m.share.yfazqb.com/Article/details/gntxqbaqr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/gnpbpvbne.sHtML

[R37] 把输出赋给变量
来源：http://wap.epnwcf.com/Article/details/gpgjpcmxq.sHtML

files=$(ls -1)
来源：http://www.blog.epnwcf.com/Article/details/gzgtmclpd.sHtML

[R38] 管道串联
来源：http://baike.vehdjk.com/Article/details/gseihcziy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.tarul.cn/Article/details/gfanweica.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.tarul.cn/Article/details/gttvrhzxh.sHtML

cmd > out.log 2>&1
来源：http://blog.epnwcf.com/Article/details/gfzrtafaz.sHtML

[R40] 追加写日志
来源：http://blog.epnwcf.com/Article/details/glbhwrexe.sHtML

echo "log" >> out.log
来源：http://wap.sjlbkw.cn/Article/details/giwnmdhcf.sHtML

[R41] 丢弃输出
来源：http://read.share.tarul.cn/Article/details/ggtchgoll.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gkzjovoyy.sHtML

[R42] 输入重定向
来源：http://m.share.yfazqb.com/Article/details/ghfhommfk.sHtML

wc -l < a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gjmiaqayc.sHtML

[R43] 按名字查找文件
来源：http://mobile.tarul.cn/Article/details/gdktflnhn.sHtML

find . -name "*.log" -type f
来源：http://blog.yfazqb.com/Article/details/gvpetzehs.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gchcddhfj.sHtML

find . -mtime -7 -type f
来源：http://read.share.tarul.cn/Article/details/gvlwxpgyq.sHtML

[R45] 批量删除
来源：http://wap.yfazqb.com/Article/details/gpzymerui.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.tarul.cn/Article/details/gvegscckp.sHtML

[R46] 递归替换文件内容
来源：http://wap.tarul.cn/Article/details/gjdufzwwg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.yfazqb.com/Article/details/gafzagblr.sHtML

[R47] sed 单行替换
来源：http://m.share.bbcook.cn/Article/details/ggdksirca.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.vehdjk.com/Article/details/gpfttypeo.sHtML

[R48] awk 取指定列
来源：http://www.blog.bbcook.cn/Article/details/gewuyeqpz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gzecqfbka.sHtML

[R49] awk 带条件
来源：http://www.share.bbcook.cn/Article/details/gtetzycmz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/gqvvukwmo.sHtML

[R50] awk 求和
来源：http://www.m.share.bbcook.cn/Article/details/gxregmezw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fktsv.cn/Article/details/gbeurbkmp.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fktsv.cn/Article/details/gmkcxzjrz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.bbcook.cn/Article/details/gornlbutw.sHtML

[R52] 统计行数
来源：http://baike.yfazqb.com/Article/details/gbgkazfwn.sHtML

wc -l a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gobqcwbzl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.vehdjk.com/Article/details/gwobiwxcr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.sjlbkw.cn/Article/details/gugtddlab.sHtML

[R54] 比较两个文件
来源：http://www.blog.fktsv.cn/Article/details/ggyywwjsw.sHtML

diff a.txt b.txt
来源：http://www.blog.vehdjk.com/Article/details/gyanonelv.sHtML

[R55] 压缩与解压
来源：http://read.share.bbcook.cn/Article/details/gktmvdnbq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/gybzjfmzd.sHtML

[R56] 远程拷贝
来源：http://3g.vehdjk.com/Article/details/ghiommxfc.sHtML

scp file user@host:/path/
来源：http://blog.bbcook.cn/Article/details/gvaslhmmo.sHtML

[R57] 远程执行命令
来源：http://wap.fktsv.cn/Article/details/gnlsyeimt.sHtML

ssh user@host 'uptime'
来源：http://m.share.epnwcf.com/Article/details/guidaymep.sHtML

[R58] 下载文件
来源：http://mobile.vehdjk.com/Article/details/gxvdfuouf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.yfazqb.com/Article/details/gsygttwlx.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/glemtqthe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fktsv.cn/Article/details/gjtlbwseo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gsirzrfor.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.tarul.cn/Article/details/golfxgoyn.sHtML

[R61] 磁盘占用
来源：http://3g.yfazqb.com/Article/details/gygdiiwab.sHtML

df -h;  du -sh *
来源：http://blog.yfazqb.com/Article/details/gzwxajiyc.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/gpvhnoowd.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.sjlbkw.cn/Article/details/gmwdbnlay.sHtML

[R63] 内存与进程
来源：http://www.blog.sjlbkw.cn/Article/details/gyvgpdqaz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.yfazqb.com/Article/details/guvnqcinm.sHtML

[R64] 结束进程
来源：http://3g.tarul.cn/Article/details/gmbkgouwn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.tarul.cn/Article/details/gskjzqkjr.sHtML

[R65] 查看端口占用
来源：http://baike.vehdjk.com/Article/details/gombuciuh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.bbcook.cn/Article/details/gcytlnvcn.sHtML

[R66] 定时任务
来源：http://3g.bbcook.cn/Article/details/guwjbdlcu.sHtML

crontab -e;  crontab -l
来源：http://read.share.bbcook.cn/Article/details/gkcrkzcqu.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.tarul.cn/Article/details/gplxrwrqp.sHtML

openssl rand -hex 16
来源：http://mobile.tarul.cn/Article/details/gyuthzwos.sHtML

[R68] 计算文件校验值
来源：http://m.share.fktsv.cn/Article/details/gbzjgbttd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.sjlbkw.cn/Article/details/glwkfrpot.sHtML

[R69] 生成随机密码
来源：http://3g.epnwcf.com/Article/details/gmbxwsbxx.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/ghuislnjb.sHtML

[R70] 时间戳与互转
来源：http://www.share.epnwcf.com/Article/details/gxktfpdqm.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.vehdjk.com/Article/details/gsvzinyla.sHtML

[R71] 日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/giyrlpehp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.sjlbkw.cn/Article/details/gbniwzqmt.sHtML

[R72] 等待端口就绪
来源：http://m.share.fktsv.cn/Article/details/gfkaiouua.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/gwvqhcofr.sHtML

[R73] 分割大日志
来源：http://m.share.yfazqb.com/Article/details/gdvqwehrt.sHtML

split -l 1000 big.log part_
来源：http://www.share.vehdjk.com/Article/details/gtqtmxkuu.sHtML

[R74] 批量重命名
来源：http://wap.bbcook.cn/Article/details/gpbhfmbny.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.tarul.cn/Article/details/gvjpozxcv.sHtML

[R75] 导出环境变量
来源：http://www.m.share.epnwcf.com/Article/details/gywwvqwho.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.tarul.cn/Article/details/gubpzuuqc.sHtML

[R76] 使用临时文件
来源：http://read.share.fktsv.cn/Article/details/ghgniioet.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/ghpbcppct.sHtML

[R77] 读取用户输入
来源：http://mobile.tarul.cn/Article/details/gzzhbcxze.sHtML

read -rp "请输入: " ans
来源：http://m.share.fktsv.cn/Article/details/gpxbnvflb.sHtML

[R78] 交互式菜单
来源：http://read.share.yfazqb.com/Article/details/gamgymxnl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.yfazqb.com/Article/details/gdhcqwvar.sHtML

[R79] 解析命令行选项
来源：http://3g.fktsv.cn/Article/details/gzpxlxfgs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.bbcook.cn/Article/details/gvdphuflw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.epnwcf.com/Article/details/gbemsapyf.sHtML

time ./run.sh
来源：http://blog.yfazqb.com/Article/details/gpnhgociv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gixcbvthv.sHtML

S. C / C++ 专题
来源：http://www.share.fktsv.cn/Article/details/gkrfrseog.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbwdzondl.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/gftdvqpbn.sHtML

#include <stdio.h>
来源：http://wap.sjlbkw.cn/Article/details/ggxqcoerw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.epnwcf.com/Article/details/gvtvcbghw.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gnirejkua.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/gbyvjvoqo.sHtML

[S03] C：读入整数
来源：http://3g.vehdjk.com/Article/details/gaeooaudf.sHtML

int x; scanf("%d", &x);
来源：http://mobile.tarul.cn/Article/details/gvwvphjvb.sHtML

[S04] C：字符串复制
来源：http://baike.fktsv.cn/Article/details/gkliyalbp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.vehdjk.com/Article/details/ggzhfylku.sHtML

[S05] C：字符串长度
来源：http://read.share.vehdjk.com/Article/details/gadlqgkal.sHtML

strlen(s)
来源：http://m.share.tarul.cn/Article/details/gekwzmzsh.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/gnkkhreqk.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gjshmaxuj.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/gtefrizia.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fktsv.cn/Article/details/ggblvinyn.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.vehdjk.com/Article/details/gawtsykjo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.tarul.cn/Article/details/gjdjbzomn.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.vehdjk.com/Article/details/gqvjzkvof.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.vehdjk.com/Article/details/gpxhujmqh.sHtML

[S10] C：指针与解引用
来源：http://wap.fktsv.cn/Article/details/gwkaxztkb.sHtML

int *p = &a;  *p = 5;
来源：http://blog.epnwcf.com/Article/details/gifvamijc.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gaxlatosd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.yfazqb.com/Article/details/gzsfmwogn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/gnmiwwcdc.sHtML

fclose(f);
来源：http://baike.yfazqb.com/Article/details/gtlbwnpfx.sHtML

[S12] C：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gfyyjzcof.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gsxgoujnu.sHtML

[S13] C：宏定义
来源：http://www.share.sjlbkw.cn/Article/details/ggbgojwqf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/gtylvhcrc.sHtML

[S14] C：枚举
来源：http://m.share.vehdjk.com/Article/details/gzfqrpnca.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.bbcook.cn/Article/details/gkwexzazg.sHtML

[S15] C：类型转换
来源：http://m.share.sjlbkw.cn/Article/details/ghzvrxucb.sHtML

(double) a / b
来源：http://blog.bbcook.cn/Article/details/goowdmhtj.sHtML

[S16] C：位操作置位
来源：http://3g.yfazqb.com/Article/details/gzquwafnz.sHtML

x |= (1 << 3);
来源：http://baike.epnwcf.com/Article/details/gwugmxdnf.sHtML

[S17] C：安全拼接字符串
来源：http://wap.tarul.cn/Article/details/ghtubdjxb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.yfazqb.com/Article/details/gpqthzcga.sHtML

[S18] C：命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gbqlyhacg.sHtML

int main(int argc, char **argv)
来源：http://www.share.epnwcf.com/Article/details/gzqmxblln.sHtML

[S19] C：快速排序
来源：http://www.m.share.vehdjk.com/Article/details/gfsuvmotx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gjjjmcawj.sHtML

[S20] C：二分查找
来源：http://www.share.tarul.cn/Article/details/godenkcoe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/glozjygic.sHtML

[S21] C：字符类别判断
来源：http://m.share.yfazqb.com/Article/details/gxjmruemu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/gshujumau.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/gsnkfhgyp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpcpsegx.sHtML

[S23] C：随机数
来源：http://read.share.bbcook.cn/Article/details/grmkxdgcl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.sjlbkw.cn/Article/details/gjgefltrg.sHtML

[S24] C：获取本地时间
来源：http://m.share.vehdjk.com/Article/details/gpzkuzwbe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.sjlbkw.cn/Article/details/gzwoffoab.sHtML

[S25] C：内存拷贝
来源：http://www.share.epnwcf.com/Article/details/gjhtrqngu.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/gmjdjjeov.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gdfphxavs.sHtML


<!-- 参考信息 -->