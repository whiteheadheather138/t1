代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fktsv.cn/Article/details/gulpvemla.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.yfazqb.com/Article/details/giqcursvv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.bbcook.cn/Article/details/gchegtmkn.sHtML

[Q57] 行号
来源：http://mobile.bbcook.cn/Article/details/gatsqtkpu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fktsv.cn/Article/details/geivdqcvy.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/gonvsjczt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.tarul.cn/Article/details/gcrwmpelp.sHtML

[Q59] 分组内累计
来源：http://3g.vehdjk.com/Article/details/gzpdlnbii.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gliysopqv.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.tarul.cn/Article/details/golxodphr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.tarul.cn/Article/details/gzcnifhin.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gjotanhuj.sHtML

[Q61] 移动平均
来源：http://www.blog.fktsv.cn/Article/details/gkcrufjso.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gdtpithkv.sHtML

[Q62] 分组占比
来源：http://3g.epnwcf.com/Article/details/gxbsdnscl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/glhabuqmi.sHtML

[Q63] 开启事务
来源：http://m.share.sjlbkw.cn/Article/details/gdxlfceeu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.sjlbkw.cn/Article/details/ggtjjejsi.sHtML

[Q64] 提交事务
来源：http://blog.sjlbkw.cn/Article/details/gglljilun.sHtML

COMMIT;
来源：http://blog.tarul.cn/Article/details/gdudknukw.sHtML

[Q65] 回滚事务
来源：http://m.share.tarul.cn/Article/details/gogsprowg.sHtML

ROLLBACK;
来源：http://read.share.sjlbkw.cn/Article/details/gvmmcihfn.sHtML

[Q66] 行锁查询
来源：http://blog.vehdjk.com/Article/details/gwdstdume.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.vehdjk.com/Article/details/gjnlkziqe.sHtML

[Q67] 设置隔离级别
来源：http://blog.yfazqb.com/Article/details/gxcxsqfam.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.bbcook.cn/Article/details/gjnandpoi.sHtML

[Q68] 保存点
来源：http://www.m.share.sjlbkw.cn/Article/details/giwqqfomt.sHtML

SAVEPOINT sp1;
来源：http://m.share.bbcook.cn/Article/details/gausekbkr.sHtML

ROLLBACK TO sp1;
来源：http://blog.sjlbkw.cn/Article/details/gkseqzcgq.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gghsnmexm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fktsv.cn/Article/details/gfgutblrl.sHtML

[Q70] 更新统计信息
来源：http://www.blog.sjlbkw.cn/Article/details/gfjiorqss.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fktsv.cn/Article/details/ggeesoaco.sHtML

[Q71] 查看建表语句
来源：http://3g.sjlbkw.cn/Article/details/gbbuyoqey.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fktsv.cn/Article/details/gmouhrrcr.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/gfkbpoozw.sHtML

SHOW INDEX FROM users;
来源：http://blog.vehdjk.com/Article/details/gzhauxvst.sHtML

[Q73] 查看表状态
来源：http://read.share.yfazqb.com/Article/details/gsyqeinzv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fktsv.cn/Article/details/gbnkfjtep.sHtML

[Q74] 强制使用索引
来源：http://www.blog.tarul.cn/Article/details/gtvvdkcly.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.sjlbkw.cn/Article/details/gavxctmca.sHtML

[Q75] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gkwpesqjs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gziefqvyy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.yfazqb.com/Article/details/gsqqkvdef.sHtML

[Q76] 按天统计
来源：http://3g.vehdjk.com/Article/details/gbmtpulgh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fktsv.cn/Article/details/gleoedeke.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/gvjcbsvtq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.tarul.cn/Article/details/gfcagvkej.sHtML

[Q78] 当前时间
来源：http://baike.tarul.cn/Article/details/ggnctketz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.yfazqb.com/Article/details/gsipufjyf.sHtML

[Q79] 字符串拼接
来源：http://3g.vehdjk.com/Article/details/gtmcncugp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.epnwcf.com/Article/details/gmgftydmp.sHtML

[Q80] 字符串截取
来源：http://www.blog.bbcook.cn/Article/details/glkyfsfph.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gkskjjall.sHtML

[Q81] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/ghrswsvmm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/geagcsjmb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/goyjutmni.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gquxsimox.sHtML

[Q83] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gyprqjcrh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gkfrsyzki.sHtML

[Q84] 去除首尾空格
来源：http://www.share.epnwcf.com/Article/details/grxzczqql.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gexpcsdvq.sHtML

[Q85] 数值取整
来源：http://www.m.share.yfazqb.com/Article/details/giehvfnrt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.sjlbkw.cn/Article/details/gclndmzor.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.yfazqb.com/Article/details/goxlrjumq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.bbcook.cn/Article/details/gioddpdzw.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.sjlbkw.cn/Article/details/gynhsuohx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.vehdjk.com/Article/details/gotecsthw.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.bbcook.cn/Article/details/geofjwzba.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.sjlbkw.cn/Article/details/ggvkheyuh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gvfpnbqjh.sHtML

[Q89] 判断表是否存在
来源：http://3g.fktsv.cn/Article/details/gnsxwgdqq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.tarul.cn/Article/details/gbenygopd.sHtML

[Q90] 生成序号列
来源：http://read.share.tarul.cn/Article/details/gvwykoswq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.bbcook.cn/Article/details/gygfpibgt.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gotcdkywn.sHtML

R. Bash 专题
来源：http://www.share.tarul.cn/Article/details/grgxnaklg.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gptkrdwda.sHtML

[R01] shebang 与严格模式
来源：http://www.share.vehdjk.com/Article/details/ghgerlvfq.sHtML

#!/usr/bin/env bash
来源：http://www.blog.yfazqb.com/Article/details/guljsawhb.sHtML

set -euo pipefail
来源：http://3g.fktsv.cn/Article/details/gbumamcus.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/gmtnnzrox.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/grfktdwov.sHtML

[R03] 只读变量
来源：http://wap.vehdjk.com/Article/details/gcynbhazq.sHtML

readonly PI=3.14
来源：http://www.share.bbcook.cn/Article/details/ghmacizjb.sHtML

[R04] 位置参数
来源：http://read.share.vehdjk.com/Article/details/ghxjtegns.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.sjlbkw.cn/Article/details/gmjtziudg.sHtML

[R05] 参数默认值
来源：http://mobile.vehdjk.com/Article/details/gbqrenboc.sHtML

name="${1:-default}"
来源：http://read.share.yfazqb.com/Article/details/gvspwndfa.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fktsv.cn/Article/details/gyokmlcqt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gqjoikndz.sHtML

[R07] if 判断文件
来源：http://3g.fktsv.cn/Article/details/ggbfozlso.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gdfehpyta.sHtML

[R08] 数值比较
来源：http://read.share.yfazqb.com/Article/details/gcnhzpsqb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.tarul.cn/Article/details/gmisutjcg.sHtML

[R09] 字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gdbiphtqc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fktsv.cn/Article/details/gpqaimlit.sHtML

[R10] 正则匹配
来源：http://m.share.sjlbkw.cn/Article/details/gvzflpsyp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.epnwcf.com/Article/details/gnqhmybmy.sHtML

[R11] case 多分支
来源：http://baike.bbcook.cn/Article/details/gonckloiv.sHtML

case "$1" in
来源：http://mobile.sjlbkw.cn/Article/details/gmyzbnaoa.sHtML

start) echo "启动" ;;
来源：http://baike.fktsv.cn/Article/details/gthrjrqzt.sHtML

stop)  echo "停止" ;;
来源：http://read.share.epnwcf.com/Article/details/gsjeowifr.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fktsv.cn/Article/details/gcgikahpj.sHtML

esac
来源：http://blog.epnwcf.com/Article/details/gybdhxasz.sHtML

[R12] for 遍历文件
来源：http://baike.fktsv.cn/Article/details/gchqzzzgt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fktsv.cn/Article/details/gwfbklxbs.sHtML

[R13] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/gjjbqdvcv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gxxtdtyux.sHtML

[R14] C 风格 for
来源：http://www.blog.tarul.cn/Article/details/gwlalwzrd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.tarul.cn/Article/details/gwyjxmabl.sHtML

[R15] while 逐行读文件
来源：http://read.share.tarul.cn/Article/details/gemzknlrs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.bbcook.cn/Article/details/gcqjljmwb.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/gczseshzn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gpffufmgo.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fktsv.cn/Article/details/gnbxmewnm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.epnwcf.com/Article/details/gxmkhyuhm.sHtML

[R18] 遍历数组
来源：http://www.share.tarul.cn/Article/details/gsxszsiwl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.sjlbkw.cn/Article/details/gftzxiyrd.sHtML

[R19] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gdmqzhede.sHtML

echo "${#arr[@]}"
来源：http://m.share.yfazqb.com/Article/details/gopingwmn.sHtML

[R20] 关联数组（字典）
来源：http://blog.epnwcf.com/Article/details/girlpofly.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.vehdjk.com/Article/details/guiobocmf.sHtML

[R21] 字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gymsdxtst.sHtML

echo "${#s}"
来源：http://3g.tarul.cn/Article/details/gfxqiygjr.sHtML

[R22] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gikrnlqqn.sHtML

echo "${s:0:5}"
来源：http://wap.vehdjk.com/Article/details/gemhuunup.sHtML

[R23] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gvxubjwjr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.tarul.cn/Article/details/gvomtlpte.sHtML

[R24] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/geihpyhme.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fktsv.cn/Article/details/gbqhwcoii.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/gmkpsglov.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.vehdjk.com/Article/details/gocvdrjkm.sHtML

[R26] 命令替换
来源：http://www.m.share.yfazqb.com/Article/details/gbgkwmblp.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.vehdjk.com/Article/details/gqvtlazea.sHtML

[R27] 算术展开
来源：http://www.blog.fktsv.cn/Article/details/gvipnhfko.sHtML

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/gwabuuqel.sHtML

[R28] 浮点运算
来源：http://mobile.tarul.cn/Article/details/gzzigeyde.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fktsv.cn/Article/details/gisrgnakw.sHtML

[R29] 定义函数
来源：http://www.share.fktsv.cn/Article/details/grzncsaey.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.sjlbkw.cn/Article/details/gendfjzwx.sHtML

[R30] 函数返回状态码
来源：http://www.blog.tarul.cn/Article/details/gdxasplpt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.sjlbkw.cn/Article/details/gmaazjxvb.sHtML

[R31] 局部变量
来源：http://baike.yfazqb.com/Article/details/gxauwdcbw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/gvfvahmxz.sHtML

[R32] 参数个数校验
来源：http://www.blog.tarul.cn/Article/details/gttrvxvfn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gzatzolol.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.epnwcf.com/Article/details/gsgmmxfzr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.epnwcf.com/Article/details/glnxuuvrg.sHtML

[R34] 退出时清理
来源：http://3g.tarul.cn/Article/details/gqjrmyyod.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gosfkjggc.sHtML

[R35] 后台执行并等待
来源：http://mobile.epnwcf.com/Article/details/ggzfwrola.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.tarul.cn/Article/details/gataionsa.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/gfubhpyei.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.bbcook.cn/Article/details/gnmmbwlud.sHtML

[R37] 把输出赋给变量
来源：http://m.share.yfazqb.com/Article/details/gwsforeap.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/glujvvxqv.sHtML

[R38] 管道串联
来源：http://wap.bbcook.cn/Article/details/gahftgxpo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.vehdjk.com/Article/details/gqydhxnmv.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.sjlbkw.cn/Article/details/gcrljntgk.sHtML

cmd > out.log 2>&1
来源：http://wap.tarul.cn/Article/details/gialyscos.sHtML

[R40] 追加写日志
来源：http://www.blog.vehdjk.com/Article/details/gbjhgbfop.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/gopastkca.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/gznxghlkc.sHtML

cmd >/dev/null 2>&1
来源：http://baike.yfazqb.com/Article/details/goygfccoo.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/ghpkohgxb.sHtML

wc -l < a.txt
来源：http://baike.sjlbkw.cn/Article/details/gntarehoa.sHtML

[R43] 按名字查找文件
来源：http://3g.sjlbkw.cn/Article/details/gskxocxhf.sHtML

find . -name "*.log" -type f
来源：http://blog.yfazqb.com/Article/details/gmelxwoty.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.vehdjk.com/Article/details/gdnrndnff.sHtML

find . -mtime -7 -type f
来源：http://baike.tarul.cn/Article/details/gvtkvbdez.sHtML

[R45] 批量删除
来源：http://m.share.tarul.cn/Article/details/gykryfxea.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/gwilfbnoo.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.bbcook.cn/Article/details/gsllprkoq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fktsv.cn/Article/details/ggxmqoyea.sHtML

[R47] sed 单行替换
来源：http://blog.bbcook.cn/Article/details/garmnspbc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fktsv.cn/Article/details/gcmrocnnl.sHtML

[R48] awk 取指定列
来源：http://read.share.yfazqb.com/Article/details/guweaidfu.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gfjtwoktk.sHtML

[R49] awk 带条件
来源：http://3g.fktsv.cn/Article/details/gtcpsjmeo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.bbcook.cn/Article/details/gtgydzztk.sHtML

[R50] awk 求和
来源：http://baike.tarul.cn/Article/details/gvmsppdwj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.tarul.cn/Article/details/gtzpwmmrf.sHtML

[R51] 排序去重取前几
来源：http://m.share.vehdjk.com/Article/details/ginhyuvzg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.sjlbkw.cn/Article/details/ghnbornyn.sHtML

[R52] 统计行数
来源：http://wap.tarul.cn/Article/details/gjptepbjv.sHtML

wc -l a.txt
来源：http://blog.vehdjk.com/Article/details/gvjspfrov.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.yfazqb.com/Article/details/gqwytoefp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/gthuzhqbb.sHtML

[R54] 比较两个文件
来源：http://www.m.share.bbcook.cn/Article/details/gmrwopguc.sHtML

diff a.txt b.txt
来源：http://read.share.epnwcf.com/Article/details/gomzapuof.sHtML

[R55] 压缩与解压
来源：http://www.m.share.vehdjk.com/Article/details/gzplcqzne.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.epnwcf.com/Article/details/gxsvdycob.sHtML

[R56] 远程拷贝
来源：http://read.share.bbcook.cn/Article/details/gntbrofkq.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/gslmrdsvz.sHtML

[R57] 远程执行命令
来源：http://wap.tarul.cn/Article/details/gjhhbhupa.sHtML

ssh user@host 'uptime'
来源：http://www.share.tarul.cn/Article/details/gbujdbhzq.sHtML

[R58] 下载文件
来源：http://3g.tarul.cn/Article/details/gtzpnepue.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.yfazqb.com/Article/details/gukvdkkkp.sHtML

[R59] 发 POST JSON
来源：http://mobile.bbcook.cn/Article/details/giabzapyc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.sjlbkw.cn/Article/details/gvfksocci.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gmrntoeut.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.yfazqb.com/Article/details/gecslwprp.sHtML

[R61] 磁盘占用
来源：http://blog.sjlbkw.cn/Article/details/ghukwrkoy.sHtML

df -h;  du -sh *
来源：http://www.blog.tarul.cn/Article/details/gajeygfrd.sHtML

[R62] 找最占空间的文件
来源：http://mobile.bbcook.cn/Article/details/gjjwvqhjq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.yfazqb.com/Article/details/gctfprslg.sHtML

[R63] 内存与进程
来源：http://www.share.fktsv.cn/Article/details/gdvehootm.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.sjlbkw.cn/Article/details/gkfaxijhh.sHtML

[R64] 结束进程
来源：http://www.blog.bbcook.cn/Article/details/gonbbvcfu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.yfazqb.com/Article/details/gkracband.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/grmlyjqyg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fktsv.cn/Article/details/gbjcgdgbp.sHtML

[R66] 定时任务
来源：http://blog.vehdjk.com/Article/details/ggmmsunkr.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/ghrkmyhed.sHtML

[R67] 生成随机十六进制串
来源：http://baike.yfazqb.com/Article/details/gjxsanixt.sHtML

openssl rand -hex 16
来源：http://baike.yfazqb.com/Article/details/grdsaisvj.sHtML

[R68] 计算文件校验值
来源：http://3g.fktsv.cn/Article/details/gosxxudfn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.tarul.cn/Article/details/ghgdlmqyo.sHtML

[R69] 生成随机密码
来源：http://read.share.yfazqb.com/Article/details/gmlvwcnng.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.yfazqb.com/Article/details/grjouhgwk.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.yfazqb.com/Article/details/gwaawogvd.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.vehdjk.com/Article/details/gnoqteact.sHtML

[R71] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gbduwikxl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.yfazqb.com/Article/details/gehaycjdb.sHtML

[R72] 等待端口就绪
来源：http://3g.tarul.cn/Article/details/gkieaknyn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gwhovofve.sHtML

[R73] 分割大日志
来源：http://read.share.vehdjk.com/Article/details/gestahnzj.sHtML

split -l 1000 big.log part_
来源：http://3g.tarul.cn/Article/details/gybrjalne.sHtML

[R74] 批量重命名
来源：http://wap.epnwcf.com/Article/details/gjutaisar.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/gwclpictx.sHtML

[R75] 导出环境变量
来源：http://mobile.yfazqb.com/Article/details/gnbfuteio.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.sjlbkw.cn/Article/details/gfztczczl.sHtML

[R76] 使用临时文件
来源：http://www.blog.vehdjk.com/Article/details/gzynobvhm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gjldsipss.sHtML

[R77] 读取用户输入
来源：http://3g.bbcook.cn/Article/details/gzdczsgnu.sHtML

read -rp "请输入: " ans
来源：http://blog.fktsv.cn/Article/details/gxpqjmxpd.sHtML

[R78] 交互式菜单
来源：http://baike.sjlbkw.cn/Article/details/gllhlgzfl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.epnwcf.com/Article/details/gwpjcnuyl.sHtML

[R79] 解析命令行选项
来源：http://wap.epnwcf.com/Article/details/ghrhmrhwi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.sjlbkw.cn/Article/details/gjybdqwsq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.yfazqb.com/Article/details/ghtihfwqr.sHtML

time ./run.sh
来源：http://www.m.share.vehdjk.com/Article/details/gmkftddbr.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnwpdciby.sHtML

S. C / C++ 专题
来源：http://baike.yfazqb.com/Article/details/grmxgjksq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcymnckcg.sHtML

[S01] C：Hello World
来源：http://read.share.fktsv.cn/Article/details/gxfyapenn.sHtML

#include <stdio.h>
来源：http://wap.tarul.cn/Article/details/gznbhojcp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/gdtrglmvt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.bbcook.cn/Article/details/gmxpbekvt.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.sjlbkw.cn/Article/details/gpltcjine.sHtML

[S03] C：读入整数
来源：http://wap.fktsv.cn/Article/details/gkkemjars.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gabqellfg.sHtML

[S04] C：字符串复制
来源：http://mobile.tarul.cn/Article/details/gerxmeqsq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.epnwcf.com/Article/details/gghmgklrq.sHtML

[S05] C：字符串长度
来源：http://www.share.tarul.cn/Article/details/gxpmcmlyb.sHtML

strlen(s)
来源：http://3g.vehdjk.com/Article/details/gvoutrgpr.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gvxwtphow.sHtML

strcmp(a, b) == 0
来源：http://www.share.vehdjk.com/Article/details/gtrtcqoom.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.tarul.cn/Article/details/gsvgjyvod.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.tarul.cn/Article/details/gqamdgesx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fktsv.cn/Article/details/gbyqcpktj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.yfazqb.com/Article/details/gljmdglzh.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.vehdjk.com/Article/details/gwdnjgqgs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fktsv.cn/Article/details/guydbdboy.sHtML

[S10] C：指针与解引用
来源：http://mobile.vehdjk.com/Article/details/gnbioeguh.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fktsv.cn/Article/details/gaolawcul.sHtML

[S11] C：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/grqwpmyhu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.epnwcf.com/Article/details/gwbyrqsll.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gtaaroyny.sHtML

fclose(f);
来源：http://baike.fktsv.cn/Article/details/gmqvnvgnh.sHtML

[S12] C：写文件
来源：http://read.share.vehdjk.com/Article/details/gyqslxlaf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.tarul.cn/Article/details/glhcxghdv.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/ggzvxrcvm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.tarul.cn/Article/details/giawcpfet.sHtML

[S14] C：枚举
来源：http://mobile.fktsv.cn/Article/details/gryvbmlcc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.yfazqb.com/Article/details/ghsmndcjm.sHtML

[S15] C：类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gpckggdvk.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/gnlqxllxf.sHtML

[S16] C：位操作置位
来源：http://m.share.yfazqb.com/Article/details/gmadsihqf.sHtML

x |= (1 << 3);
来源：http://www.m.share.epnwcf.com/Article/details/giufmyjbq.sHtML

[S17] C：安全拼接字符串
来源：http://wap.vehdjk.com/Article/details/gsaabutps.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.bbcook.cn/Article/details/gnofqqesz.sHtML

[S18] C：命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gpkphfarn.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/gfdclzpan.sHtML

[S19] C：快速排序
来源：http://www.m.share.epnwcf.com/Article/details/gvtuauqqs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/grzkakdzd.sHtML

[S20] C：二分查找
来源：http://baike.sjlbkw.cn/Article/details/gwudezezt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/ggafwsvso.sHtML

[S21] C：字符类别判断
来源：http://m.share.yfazqb.com/Article/details/grsmbpgoi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoqwuhmq.sHtML

[S22] C：字符串转数字
来源：http://read.share.yfazqb.com/Article/details/gbvultnqp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.sjlbkw.cn/Article/details/gcnclbnko.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/gsalkarqg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.yfazqb.com/Article/details/gmcjkivsn.sHtML

[S24] C：获取本地时间
来源：http://3g.vehdjk.com/Article/details/gjijhsbjs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.sjlbkw.cn/Article/details/gnzxkluzv.sHtML

[S25] C：内存拷贝
来源：http://blog.yfazqb.com/Article/details/gqdjhmmfa.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/gdxhhqbii.sHtML

[S26] C：内存清零
来源：http://3g.sjlbkw.cn/Article/details/gcyrkshzg.sHtML


<!-- 参考信息 -->