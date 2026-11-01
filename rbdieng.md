代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gscnyygrm.sHtML

[Q58] 累计求和
来源：http://3g.sjlbkw.cn/Article/details/galflhzgp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gdzprpebv.sHtML

[Q59] 分组内累计
来源：http://www.blog.epnwcf.com/Article/details/glrkvnjvu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gazoaltak.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.tarul.cn/Article/details/gjhauuarz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.vehdjk.com/Article/details/gqrfmiwoa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gbjitdjwh.sHtML

[Q61] 移动平均
来源：http://baike.epnwcf.com/Article/details/gwlhmshij.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/grzsewvwj.sHtML

[Q62] 分组占比
来源：http://blog.epnwcf.com/Article/details/gwlomlanz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gvammtnei.sHtML

[Q63] 开启事务
来源：http://3g.epnwcf.com/Article/details/gkbavkmbq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gynphomly.sHtML

[Q64] 提交事务
来源：http://www.blog.sjlbkw.cn/Article/details/gvyhusarb.sHtML

COMMIT;
来源：http://blog.yfazqb.com/Article/details/gjzjnmxze.sHtML

[Q65] 回滚事务
来源：http://www.share.sjlbkw.cn/Article/details/gafrsgyrj.sHtML

ROLLBACK;
来源：http://www.share.vehdjk.com/Article/details/grlnhqnud.sHtML

[Q66] 行锁查询
来源：http://baike.epnwcf.com/Article/details/guyfkpqiu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.bbcook.cn/Article/details/gwephlacj.sHtML

[Q67] 设置隔离级别
来源：http://wap.sjlbkw.cn/Article/details/gwwawzllz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.tarul.cn/Article/details/gxkyvzjrw.sHtML

[Q68] 保存点
来源：http://mobile.tarul.cn/Article/details/gandqfxim.sHtML

SAVEPOINT sp1;
来源：http://mobile.bbcook.cn/Article/details/gmomduezc.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fktsv.cn/Article/details/grtgpaaql.sHtML

[Q69] 查看执行计划
来源：http://blog.epnwcf.com/Article/details/glrhqmpfz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.vehdjk.com/Article/details/gghvlhhsr.sHtML

[Q70] 更新统计信息
来源：http://baike.yfazqb.com/Article/details/gredibgvz.sHtML

ANALYZE TABLE users;
来源：http://3g.vehdjk.com/Article/details/gebwmdqln.sHtML

[Q71] 查看建表语句
来源：http://baike.tarul.cn/Article/details/gjeyhdcpd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.sjlbkw.cn/Article/details/ggcbecnpw.sHtML

[Q72] 查看索引
来源：http://wap.sjlbkw.cn/Article/details/gwrrnaatj.sHtML

SHOW INDEX FROM users;
来源：http://baike.bbcook.cn/Article/details/gkzmhwajn.sHtML

[Q73] 查看表状态
来源：http://blog.sjlbkw.cn/Article/details/gkkvezvxm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fktsv.cn/Article/details/gxcnilfzl.sHtML

[Q74] 强制使用索引
来源：http://www.share.sjlbkw.cn/Article/details/gylatdjxb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.vehdjk.com/Article/details/gfnlokqby.sHtML

[Q75] 日期格式化
来源：http://blog.epnwcf.com/Article/details/grxofofgz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.bbcook.cn/Article/details/gqhgygfxr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.sjlbkw.cn/Article/details/gbgmtwmwu.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/gqqcwaqwq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.sjlbkw.cn/Article/details/ghgisbhdu.sHtML

[Q77] 时间加减
来源：http://www.m.share.vehdjk.com/Article/details/gwrgzohld.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.tarul.cn/Article/details/gtxhmxzzt.sHtML

[Q78] 当前时间
来源：http://www.blog.vehdjk.com/Article/details/gktxjsdml.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fktsv.cn/Article/details/ggjynljtv.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/gogxyitiq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.vehdjk.com/Article/details/gnvtbyasg.sHtML

[Q80] 字符串截取
来源：http://read.share.bbcook.cn/Article/details/gsqwpptrn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gkktndgkj.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gmkucccgz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.epnwcf.com/Article/details/gysazkevl.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.yfazqb.com/Article/details/glxaikdtc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gqmbcweqs.sHtML

[Q83] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gdmlslggq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/ggeyaevrm.sHtML

[Q84] 去除首尾空格
来源：http://m.share.bbcook.cn/Article/details/gmifbfaqp.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gtyuaevxu.sHtML

[Q85] 数值取整
来源：http://m.share.tarul.cn/Article/details/gobsdvyzp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.tarul.cn/Article/details/grknfrdrf.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.vehdjk.com/Article/details/gidnlgyjp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.tarul.cn/Article/details/glbxelipv.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.sjlbkw.cn/Article/details/gdohbdnok.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gclwrfhya.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.epnwcf.com/Article/details/gvblnvwhk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.bbcook.cn/Article/details/gowcuptyf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gijndyvrs.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gvrfvunqr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.sjlbkw.cn/Article/details/gxhbxoluo.sHtML

[Q90] 生成序号列
来源：http://baike.tarul.cn/Article/details/gahhayekf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.sjlbkw.cn/Article/details/ghfjkcfru.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvxvaxufq.sHtML

R. Bash 专题
来源：http://www.m.share.fktsv.cn/Article/details/gkawllxdo.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmrtgsovw.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.yfazqb.com/Article/details/gbcdyqzar.sHtML

#!/usr/bin/env bash
来源：http://www.blog.yfazqb.com/Article/details/gwasouggr.sHtML

set -euo pipefail
来源：http://www.blog.vehdjk.com/Article/details/guezbayep.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.sjlbkw.cn/Article/details/gckmvxrwa.sHtML

name="Tom"; echo "$name"
来源：http://www.share.bbcook.cn/Article/details/gdgyiacdu.sHtML

[R03] 只读变量
来源：http://www.blog.yfazqb.com/Article/details/gamhfeken.sHtML

readonly PI=3.14
来源：http://read.share.tarul.cn/Article/details/ggwsofzib.sHtML

[R04] 位置参数
来源：http://www.share.tarul.cn/Article/details/gbvmzlqwf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.vehdjk.com/Article/details/gjbxqvlzs.sHtML

[R05] 参数默认值
来源：http://www.share.tarul.cn/Article/details/gtoeehtpc.sHtML

name="${1:-default}"
来源：http://www.m.share.tarul.cn/Article/details/gmkgqdtux.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.yfazqb.com/Article/details/gcvuaeuzp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfysiftre.sHtML

[R07] if 判断文件
来源：http://www.m.share.tarul.cn/Article/details/gbksqhxms.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fktsv.cn/Article/details/gaybznxiw.sHtML

[R08] 数值比较
来源：http://blog.epnwcf.com/Article/details/gfyhlustp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.vehdjk.com/Article/details/gyfmpmuar.sHtML

[R09] 字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gipyxpiuc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.tarul.cn/Article/details/gqibzyrdm.sHtML

[R10] 正则匹配
来源：http://wap.yfazqb.com/Article/details/ghvbgrtqd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gopaxyjqw.sHtML

[R11] case 多分支
来源：http://m.share.yfazqb.com/Article/details/giceqetfp.sHtML

case "$1" in
来源：http://www.m.share.bbcook.cn/Article/details/gygaqjuws.sHtML

start) echo "启动" ;;
来源：http://wap.yfazqb.com/Article/details/grfmdycrt.sHtML

stop)  echo "停止" ;;
来源：http://3g.fktsv.cn/Article/details/gqcolfjei.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.epnwcf.com/Article/details/ggrsvkona.sHtML

esac
来源：http://www.blog.vehdjk.com/Article/details/gmtlqmwyt.sHtML

[R12] for 遍历文件
来源：http://read.share.yfazqb.com/Article/details/grllmqkjy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.yfazqb.com/Article/details/gkowyqblh.sHtML

[R13] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/gmpdhydjz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fktsv.cn/Article/details/grdckpafu.sHtML

[R14] C 风格 for
来源：http://wap.yfazqb.com/Article/details/gdoxantdu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gxwbhzfkz.sHtML

[R15] while 逐行读文件
来源：http://blog.bbcook.cn/Article/details/gfhxxizzl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.yfazqb.com/Article/details/ggsoilasv.sHtML

[R16] until 等待条件
来源：http://www.m.share.vehdjk.com/Article/details/ghynqipce.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/geohtnjxq.sHtML

[R17] 数组定义与取值
来源：http://read.share.vehdjk.com/Article/details/gxxsogfnx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.bbcook.cn/Article/details/geyjfepvt.sHtML

[R18] 遍历数组
来源：http://read.share.yfazqb.com/Article/details/gieenevwz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.sjlbkw.cn/Article/details/gnmxpjury.sHtML

[R19] 数组长度
来源：http://baike.tarul.cn/Article/details/gvirjfjnv.sHtML

echo "${#arr[@]}"
来源：http://www.blog.sjlbkw.cn/Article/details/glgoifmpp.sHtML

[R20] 关联数组（字典）
来源：http://wap.tarul.cn/Article/details/ggmznqywt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fktsv.cn/Article/details/glssrzruz.sHtML

[R21] 字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gzufdsjaj.sHtML

echo "${#s}"
来源：http://wap.epnwcf.com/Article/details/gqvksfjgd.sHtML

[R22] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gmygopoii.sHtML

echo "${s:0:5}"
来源：http://mobile.tarul.cn/Article/details/gjscsyoru.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gjkmnlenj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.bbcook.cn/Article/details/gvttpxhbe.sHtML

[R24] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gybewhpqr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.epnwcf.com/Article/details/gunsynjng.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.yfazqb.com/Article/details/guvyfbnvp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.vehdjk.com/Article/details/gnqgbbjpk.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/ghytnwjnq.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.sjlbkw.cn/Article/details/gyoyrcfvd.sHtML

[R27] 算术展开
来源：http://read.share.fktsv.cn/Article/details/gwojkytjb.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.vehdjk.com/Article/details/gaedvtrvz.sHtML

[R28] 浮点运算
来源：http://www.share.vehdjk.com/Article/details/gvsyendvx.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fktsv.cn/Article/details/gsxvvofwd.sHtML

[R29] 定义函数
来源：http://blog.epnwcf.com/Article/details/gaqfwrfgj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fktsv.cn/Article/details/gmjoypnoe.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/gdlquxqvn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.epnwcf.com/Article/details/ghvkwiseg.sHtML

[R31] 局部变量
来源：http://wap.bbcook.cn/Article/details/gyaudfytb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.epnwcf.com/Article/details/gwicvnras.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fktsv.cn/Article/details/gugdrrkdt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gprkkeuvo.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.epnwcf.com/Article/details/gsymzbrbk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.bbcook.cn/Article/details/gejximpjq.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/gjfkhjbot.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gnhxrpivl.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/gtxcvvmxs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.yfazqb.com/Article/details/gflkngfpe.sHtML

[R36] 并发执行多个任务
来源：http://m.share.yfazqb.com/Article/details/guuugzgcn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fktsv.cn/Article/details/gcrmdonij.sHtML

[R37] 把输出赋给变量
来源：http://3g.tarul.cn/Article/details/gegrsdael.sHtML

files=$(ls -1)
来源：http://m.share.tarul.cn/Article/details/grlomudxl.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/gmghinwpo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.tarul.cn/Article/details/gavnojtts.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.sjlbkw.cn/Article/details/gnyftsjdp.sHtML

cmd > out.log 2>&1
来源：http://mobile.tarul.cn/Article/details/ghryawfax.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/gfaekslax.sHtML

echo "log" >> out.log
来源：http://mobile.sjlbkw.cn/Article/details/gikdnqrmk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.tarul.cn/Article/details/gojvuuday.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/gqwzuduhe.sHtML

[R42] 输入重定向
来源：http://blog.yfazqb.com/Article/details/gycrxring.sHtML

wc -l < a.txt
来源：http://blog.fktsv.cn/Article/details/ggvvsegig.sHtML

[R43] 按名字查找文件
来源：http://mobile.fktsv.cn/Article/details/grvnczzsg.sHtML

find . -name "*.log" -type f
来源：http://m.share.epnwcf.com/Article/details/gdsecfdid.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.yfazqb.com/Article/details/glokcvrhj.sHtML

find . -mtime -7 -type f
来源：http://baike.bbcook.cn/Article/details/gqcvfvzfi.sHtML

[R45] 批量删除
来源：http://wap.vehdjk.com/Article/details/gqdvkisdn.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.vehdjk.com/Article/details/gywwmpivh.sHtML

[R46] 递归替换文件内容
来源：http://blog.yfazqb.com/Article/details/glikwvgjq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.epnwcf.com/Article/details/gondipxag.sHtML

[R47] sed 单行替换
来源：http://wap.fktsv.cn/Article/details/gkyuipghm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gwbqwqkxk.sHtML

[R48] awk 取指定列
来源：http://www.share.bbcook.cn/Article/details/gilajmbwh.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gmqjoryzl.sHtML

[R49] awk 带条件
来源：http://www.m.share.epnwcf.com/Article/details/gvmsktwqr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.yfazqb.com/Article/details/guxknadau.sHtML

[R50] awk 求和
来源：http://www.share.tarul.cn/Article/details/gsxvxpowq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gpqyyxlso.sHtML

[R51] 排序去重取前几
来源：http://baike.tarul.cn/Article/details/gqihrsfdb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/gpiksnref.sHtML

[R52] 统计行数
来源：http://www.blog.vehdjk.com/Article/details/ggtlphawr.sHtML

wc -l a.txt
来源：http://3g.epnwcf.com/Article/details/ghsktaefj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.bbcook.cn/Article/details/gmslywmev.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gystcfobp.sHtML

[R54] 比较两个文件
来源：http://blog.yfazqb.com/Article/details/gsvqiozgi.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/ggzaejpkk.sHtML

[R55] 压缩与解压
来源：http://wap.sjlbkw.cn/Article/details/gwceiyimt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.sjlbkw.cn/Article/details/gprziunfe.sHtML

[R56] 远程拷贝
来源：http://blog.fktsv.cn/Article/details/gizujlaqf.sHtML

scp file user@host:/path/
来源：http://3g.vehdjk.com/Article/details/ggurzkshi.sHtML

[R57] 远程执行命令
来源：http://baike.fktsv.cn/Article/details/gyqosndie.sHtML

ssh user@host 'uptime'
来源：http://baike.vehdjk.com/Article/details/gmydvulid.sHtML

[R58] 下载文件
来源：http://blog.fktsv.cn/Article/details/gamiqxirj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fktsv.cn/Article/details/gaaiphxix.sHtML

[R59] 发 POST JSON
来源：http://m.share.fktsv.cn/Article/details/gnkgvcles.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.tarul.cn/Article/details/gfoseocbx.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gpqjlupjy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.sjlbkw.cn/Article/details/gvcfrrhwy.sHtML

[R61] 磁盘占用
来源：http://www.m.share.bbcook.cn/Article/details/gurfbjppi.sHtML

df -h;  du -sh *
来源：http://3g.fktsv.cn/Article/details/gpayfggrd.sHtML

[R62] 找最占空间的文件
来源：http://m.share.bbcook.cn/Article/details/gkjdhjzox.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.epnwcf.com/Article/details/gycgmuhic.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/gwhkafeno.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fktsv.cn/Article/details/gkfuevmti.sHtML

[R64] 结束进程
来源：http://mobile.sjlbkw.cn/Article/details/gssnqdyuo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fktsv.cn/Article/details/gstlcqjgx.sHtML

[R65] 查看端口占用
来源：http://3g.tarul.cn/Article/details/gxloflnaf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.epnwcf.com/Article/details/goxvqqkwu.sHtML

[R66] 定时任务
来源：http://www.m.share.bbcook.cn/Article/details/glwhguejz.sHtML

crontab -e;  crontab -l
来源：http://blog.yfazqb.com/Article/details/gawpqpubz.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.epnwcf.com/Article/details/gnygsoasr.sHtML

openssl rand -hex 16
来源：http://wap.tarul.cn/Article/details/gzjlldyzc.sHtML

[R68] 计算文件校验值
来源：http://wap.tarul.cn/Article/details/gvirfzqxu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gjvkpmrnp.sHtML

[R69] 生成随机密码
来源：http://blog.tarul.cn/Article/details/ghiwjvanw.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.bbcook.cn/Article/details/gznadjzjb.sHtML

[R70] 时间戳与互转
来源：http://3g.yfazqb.com/Article/details/gkvzeqbyw.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/grunxmiee.sHtML

[R71] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gunfqopew.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fktsv.cn/Article/details/gunuptiyr.sHtML

[R72] 等待端口就绪
来源：http://wap.yfazqb.com/Article/details/gpipwyrkp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gseuhuccw.sHtML

[R73] 分割大日志
来源：http://www.share.vehdjk.com/Article/details/gmrgowogq.sHtML

split -l 1000 big.log part_
来源：http://baike.yfazqb.com/Article/details/gfagbprsu.sHtML

[R74] 批量重命名
来源：http://mobile.bbcook.cn/Article/details/gegltrzpv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fktsv.cn/Article/details/ggezqsfzr.sHtML

[R75] 导出环境变量
来源：http://mobile.tarul.cn/Article/details/gewysloti.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fktsv.cn/Article/details/gmocjgyol.sHtML

[R76] 使用临时文件
来源：http://blog.epnwcf.com/Article/details/gwntrwwpe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/ghuevhpns.sHtML

[R77] 读取用户输入
来源：http://wap.tarul.cn/Article/details/gcbmefhkx.sHtML

read -rp "请输入: " ans
来源：http://www.share.bbcook.cn/Article/details/gglrlkfrw.sHtML

[R78] 交互式菜单
来源：http://www.blog.yfazqb.com/Article/details/gxpxcbsvs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.epnwcf.com/Article/details/gtajjswvi.sHtML

[R79] 解析命令行选项
来源：http://read.share.sjlbkw.cn/Article/details/gfkgxoolt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.epnwcf.com/Article/details/gjnkorqfi.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.vehdjk.com/Article/details/gvwvdpxqo.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/gbayrzipy.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqtawczzr.sHtML

S. C / C++ 专题
来源：http://read.share.bbcook.cn/Article/details/gahvvlvoq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzosfoguw.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/gdpgvwcju.sHtML

#include <stdio.h>
来源：http://read.share.yfazqb.com/Article/details/gmxbsjkee.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.vehdjk.com/Article/details/gqqjwkbno.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.tarul.cn/Article/details/gfvxeitvf.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.bbcook.cn/Article/details/gzrpmnqnh.sHtML

[S03] C：读入整数
来源：http://blog.fktsv.cn/Article/details/gfejpzuil.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/gaxdakkkm.sHtML

[S04] C：字符串复制
来源：http://www.blog.tarul.cn/Article/details/gyglnbxxj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/gvoqsvlfx.sHtML

[S05] C：字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gujbnoddv.sHtML

strlen(s)
来源：http://baike.bbcook.cn/Article/details/gluqcznkq.sHtML

[S06] C：字符串比较
来源：http://wap.yfazqb.com/Article/details/gaxfbqwpw.sHtML

strcmp(a, b) == 0
来源：http://blog.sjlbkw.cn/Article/details/gmdklvwuf.sHtML

[S07] C：数组遍历求和
来源：http://3g.tarul.cn/Article/details/gexexgqik.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.vehdjk.com/Article/details/gryktbnfz.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.tarul.cn/Article/details/gdoesjrei.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.sjlbkw.cn/Article/details/gseuiarkf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.epnwcf.com/Article/details/gxrudulcn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/gypwyfdup.sHtML

[S10] C：指针与解引用
来源：http://wap.fktsv.cn/Article/details/gzzfhuczw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.yfazqb.com/Article/details/gphkagays.sHtML

[S11] C：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gkfeyyyqr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.bbcook.cn/Article/details/gjduvhout.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.vehdjk.com/Article/details/gftmjfzrl.sHtML

fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gwwwdddla.sHtML

[S12] C：写文件
来源：http://m.share.bbcook.cn/Article/details/gqbvdqbfz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.bbcook.cn/Article/details/gngnfvzkn.sHtML

[S13] C：宏定义
来源：http://mobile.bbcook.cn/Article/details/ggyhjrjnf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.vehdjk.com/Article/details/ggmoufijr.sHtML

[S14] C：枚举
来源：http://www.blog.tarul.cn/Article/details/giixshrhf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fktsv.cn/Article/details/gctzktrri.sHtML

[S15] C：类型转换
来源：http://m.share.tarul.cn/Article/details/gglsvdsyd.sHtML

(double) a / b
来源：http://3g.fktsv.cn/Article/details/gyfnenlrj.sHtML

[S16] C：位操作置位
来源：http://www.share.sjlbkw.cn/Article/details/gzadymqni.sHtML

x |= (1 << 3);
来源：http://www.share.fktsv.cn/Article/details/gyptwpwsm.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gxvfcqhmf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.bbcook.cn/Article/details/gxrnvfzjy.sHtML

[S18] C：命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gukdethgt.sHtML

int main(int argc, char **argv)
来源：http://3g.bbcook.cn/Article/details/gxmnncmjl.sHtML

[S19] C：快速排序
来源：http://www.blog.sjlbkw.cn/Article/details/greoysvcr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gdydymfdf.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/gotrbeckn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gysvlmxee.sHtML

[S21] C：字符类别判断
来源：http://wap.epnwcf.com/Article/details/gpdxuhgbr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fktsv.cn/Article/details/gfohcuunu.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/ggwglvclq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.vehdjk.com/Article/details/gvzjlheck.sHtML

[S23] C：随机数
来源：http://baike.epnwcf.com/Article/details/gqfeygggu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.sjlbkw.cn/Article/details/gpzwtmatu.sHtML

[S24] C：获取本地时间
来源：http://baike.bbcook.cn/Article/details/gogfddnad.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.sjlbkw.cn/Article/details/gvuceztis.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gpwuabbsz.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/gwouadykw.sHtML

[S26] C：内存清零
来源：http://www.blog.vehdjk.com/Article/details/gwcgztypa.sHtML

memset(a, 0, sizeof a);
来源：http://blog.epnwcf.com/Article/details/gmwwiqjdl.sHtML

[S27] C：定义常量
来源：http://wap.yfazqb.com/Article/details/gcqphpvug.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gavfyasxb.sHtML

[S28] C：静态变量
来源：http://www.blog.vehdjk.com/Article/details/gzwvxzfph.sHtML


<!-- 参考信息 -->