代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gkbizwilz.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.yfazqb.com/Article/details/guekjsgvt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.bbcook.cn/Article/details/gcnzlufmt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gxivplmux.sHtML

[Q61] 移动平均
来源：http://www.blog.epnwcf.com/Article/details/gkzpbmpag.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gqjlgejpf.sHtML

[Q62] 分组占比
来源：http://wap.epnwcf.com/Article/details/gdbswiqnz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gyxbmagfj.sHtML

[Q63] 开启事务
来源：http://wap.sjlbkw.cn/Article/details/glfistucz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.vehdjk.com/Article/details/geoigxxao.sHtML

[Q64] 提交事务
来源：http://m.share.vehdjk.com/Article/details/gavhmegxp.sHtML

COMMIT;
来源：http://3g.yfazqb.com/Article/details/gyqdvtxpd.sHtML

[Q65] 回滚事务
来源：http://www.share.vehdjk.com/Article/details/gnajwugtb.sHtML

ROLLBACK;
来源：http://blog.bbcook.cn/Article/details/govcrpgvn.sHtML

[Q66] 行锁查询
来源：http://m.share.yfazqb.com/Article/details/gqglgggjk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.tarul.cn/Article/details/gkpsgtice.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.bbcook.cn/Article/details/ggqumarue.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.sjlbkw.cn/Article/details/gzwvcyzui.sHtML

[Q68] 保存点
来源：http://read.share.tarul.cn/Article/details/gvsoikdas.sHtML

SAVEPOINT sp1;
来源：http://mobile.fktsv.cn/Article/details/gpepgprny.sHtML

ROLLBACK TO sp1;
来源：http://3g.vehdjk.com/Article/details/gsybhxfeu.sHtML

[Q69] 查看执行计划
来源：http://baike.tarul.cn/Article/details/gtzwqubyy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.bbcook.cn/Article/details/gwbonmngl.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/gstxguqme.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.epnwcf.com/Article/details/gdhsblmcg.sHtML

[Q71] 查看建表语句
来源：http://read.share.sjlbkw.cn/Article/details/gcrxlhyzi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.yfazqb.com/Article/details/gvjlpmcmp.sHtML

[Q72] 查看索引
来源：http://mobile.fktsv.cn/Article/details/gkzwcnjlb.sHtML

SHOW INDEX FROM users;
来源：http://m.share.vehdjk.com/Article/details/gtfcjmqci.sHtML

[Q73] 查看表状态
来源：http://blog.vehdjk.com/Article/details/gjsytvsnl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.yfazqb.com/Article/details/gkvqlhhjn.sHtML

[Q74] 强制使用索引
来源：http://wap.tarul.cn/Article/details/gawwtmkvy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fktsv.cn/Article/details/gdfrujron.sHtML

[Q75] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/guvydnert.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gflqenbph.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.epnwcf.com/Article/details/gjcqnjkcc.sHtML

[Q76] 按天统计
来源：http://mobile.sjlbkw.cn/Article/details/gxpcvzntx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fktsv.cn/Article/details/ggferlblj.sHtML

[Q77] 时间加减
来源：http://mobile.bbcook.cn/Article/details/ggzkvwdhy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.tarul.cn/Article/details/gzhomnyiv.sHtML

[Q78] 当前时间
来源：http://blog.fktsv.cn/Article/details/gwtfbgdib.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/galefsupk.sHtML

[Q79] 字符串拼接
来源：http://3g.epnwcf.com/Article/details/gikrbijus.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.tarul.cn/Article/details/gtbtfhonc.sHtML

[Q80] 字符串截取
来源：http://wap.tarul.cn/Article/details/gxiszdqdv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gcxrycvxb.sHtML

[Q81] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gawtgmqci.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gwsoxpwmv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.sjlbkw.cn/Article/details/gnuvqwtsq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/grjsjuogx.sHtML

[Q83] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/gjibjyvrz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gcoycnwpi.sHtML

[Q84] 去除首尾空格
来源：http://3g.sjlbkw.cn/Article/details/gwaqilerl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gqlwzprfr.sHtML

[Q85] 数值取整
来源：http://www.blog.tarul.cn/Article/details/gfhnkdfna.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.yfazqb.com/Article/details/gfvhyzblx.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.tarul.cn/Article/details/ghtesyjkz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.vehdjk.com/Article/details/gqcnsozuy.sHtML

[Q87] JSON 字段做条件
来源：http://wap.bbcook.cn/Article/details/grruyxtxz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.yfazqb.com/Article/details/guxlbstyr.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.yfazqb.com/Article/details/gcktmxbqv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fktsv.cn/Article/details/grmbkavon.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.tarul.cn/Article/details/gxalvzvki.sHtML

[Q89] 判断表是否存在
来源：http://baike.vehdjk.com/Article/details/gbwgvobbj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gazzmmxzf.sHtML

[Q90] 生成序号列
来源：http://3g.tarul.cn/Article/details/ggjwmseup.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.bbcook.cn/Article/details/gegvkhlto.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gjplogsfi.sHtML

R. Bash 专题
来源：http://www.share.sjlbkw.cn/Article/details/gbgomietp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gukhkqxdt.sHtML

[R01] shebang 与严格模式
来源：http://3g.fktsv.cn/Article/details/gcmrsrzbp.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fktsv.cn/Article/details/gedgccvzl.sHtML

set -euo pipefail
来源：http://mobile.vehdjk.com/Article/details/gxpfqavzh.sHtML

[R02] 变量赋值与使用
来源：http://blog.fktsv.cn/Article/details/gnfbeljkx.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fktsv.cn/Article/details/gemxcffxg.sHtML

[R03] 只读变量
来源：http://www.blog.bbcook.cn/Article/details/gjnvdxggr.sHtML

readonly PI=3.14
来源：http://m.share.bbcook.cn/Article/details/gpkufqapj.sHtML

[R04] 位置参数
来源：http://mobile.vehdjk.com/Article/details/gixymmoye.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.vehdjk.com/Article/details/ghniqxnvi.sHtML

[R05] 参数默认值
来源：http://read.share.fktsv.cn/Article/details/gfpvxebts.sHtML

name="${1:-default}"
来源：http://3g.sjlbkw.cn/Article/details/gupzqxhbb.sHtML

[R06] 判断命令是否存在
来源：http://blog.bbcook.cn/Article/details/ghyrlwkem.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gwjajirba.sHtML

[R07] if 判断文件
来源：http://read.share.bbcook.cn/Article/details/gtlpblfgf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fktsv.cn/Article/details/gqxmftimc.sHtML

[R08] 数值比较
来源：http://mobile.vehdjk.com/Article/details/gzslhizkb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.bbcook.cn/Article/details/goiwkcmmp.sHtML

[R09] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gglofccgk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.vehdjk.com/Article/details/gznlsptys.sHtML

[R10] 正则匹配
来源：http://www.blog.tarul.cn/Article/details/gvugcqrrc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fktsv.cn/Article/details/gaiqrwavb.sHtML

[R11] case 多分支
来源：http://blog.fktsv.cn/Article/details/gfthrgxop.sHtML

case "$1" in
来源：http://mobile.bbcook.cn/Article/details/gbbhjcfta.sHtML

start) echo "启动" ;;
来源：http://blog.bbcook.cn/Article/details/gjtswpunq.sHtML

stop)  echo "停止" ;;
来源：http://www.share.yfazqb.com/Article/details/gkvuisnxi.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.tarul.cn/Article/details/gvghalpiy.sHtML

esac
来源：http://3g.yfazqb.com/Article/details/gzsrkmphr.sHtML

[R12] for 遍历文件
来源：http://m.share.tarul.cn/Article/details/gbtbrplju.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.sjlbkw.cn/Article/details/gpsckmjhb.sHtML

[R13] for 计数循环
来源：http://wap.yfazqb.com/Article/details/gsckptcvp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gmjgglbnm.sHtML

[R14] C 风格 for
来源：http://m.share.epnwcf.com/Article/details/gxylndpgg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gkaruduqt.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/gaudyajez.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.vehdjk.com/Article/details/gxalckbxk.sHtML

[R16] until 等待条件
来源：http://www.blog.sjlbkw.cn/Article/details/grzxhnkcf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gjnyooksn.sHtML

[R17] 数组定义与取值
来源：http://www.share.yfazqb.com/Article/details/gcmteqaxc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fktsv.cn/Article/details/grjuraozy.sHtML

[R18] 遍历数组
来源：http://mobile.yfazqb.com/Article/details/gbpwgoexh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.yfazqb.com/Article/details/gsgsfdajm.sHtML

[R19] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gftablyxy.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.bbcook.cn/Article/details/gjvoiuszq.sHtML

[R20] 关联数组（字典）
来源：http://3g.yfazqb.com/Article/details/gpldotham.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.tarul.cn/Article/details/gpvyvzgjl.sHtML

[R21] 字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gdpjcchrk.sHtML

echo "${#s}"
来源：http://www.blog.tarul.cn/Article/details/gpynmcofh.sHtML

[R22] 截取子串
来源：http://3g.bbcook.cn/Article/details/gekucekfv.sHtML

echo "${s:0:5}"
来源：http://blog.tarul.cn/Article/details/glqclqlwn.sHtML

[R23] 字符串替换
来源：http://baike.tarul.cn/Article/details/gnedysuzl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.tarul.cn/Article/details/ghcflnnxz.sHtML

[R24] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gwouimgca.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.bbcook.cn/Article/details/gxqtsgqog.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.yfazqb.com/Article/details/gvshiutsx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.epnwcf.com/Article/details/gunllyzoo.sHtML

[R26] 命令替换
来源：http://blog.sjlbkw.cn/Article/details/ghbkcfkra.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.bbcook.cn/Article/details/gnkqeognl.sHtML

[R27] 算术展开
来源：http://3g.sjlbkw.cn/Article/details/gecewsfpw.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.yfazqb.com/Article/details/gsizkrvzj.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/gkabxdssg.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/gtxbnxaiy.sHtML

[R29] 定义函数
来源：http://3g.bbcook.cn/Article/details/gvymdulug.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.sjlbkw.cn/Article/details/gprjpinyq.sHtML

[R30] 函数返回状态码
来源：http://baike.epnwcf.com/Article/details/gsreqikge.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.bbcook.cn/Article/details/gyblcazbb.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/ggisszrsi.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.epnwcf.com/Article/details/gfvtlixzp.sHtML

[R32] 参数个数校验
来源：http://wap.tarul.cn/Article/details/gpvsdecqc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/gxuwdjvqd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.vehdjk.com/Article/details/gvuezflys.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.sjlbkw.cn/Article/details/ghcdbgmjq.sHtML

[R34] 退出时清理
来源：http://mobile.yfazqb.com/Article/details/gtalaeunj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gqwskahrc.sHtML

[R35] 后台执行并等待
来源：http://blog.fktsv.cn/Article/details/gwznpklgt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.bbcook.cn/Article/details/gdmyaqpxd.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.tarul.cn/Article/details/gsrltbjmy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.vehdjk.com/Article/details/gpgtsnbdr.sHtML

[R37] 把输出赋给变量
来源：http://baike.tarul.cn/Article/details/gevavzlmq.sHtML

files=$(ls -1)
来源：http://www.m.share.tarul.cn/Article/details/gkcqorpuz.sHtML

[R38] 管道串联
来源：http://www.share.epnwcf.com/Article/details/golcqmqnx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.sjlbkw.cn/Article/details/gfuplhhco.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.yfazqb.com/Article/details/gfgzjziuf.sHtML

cmd > out.log 2>&1
来源：http://mobile.vehdjk.com/Article/details/gpxvinrhp.sHtML

[R40] 追加写日志
来源：http://baike.bbcook.cn/Article/details/gyjscjxtz.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/gqpmqpjqt.sHtML

[R41] 丢弃输出
来源：http://baike.yfazqb.com/Article/details/gxzbirxsh.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.bbcook.cn/Article/details/gveujhcra.sHtML

[R42] 输入重定向
来源：http://www.m.share.bbcook.cn/Article/details/giwphbrzw.sHtML

wc -l < a.txt
来源：http://3g.vehdjk.com/Article/details/gbwkubdiz.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/gcwnndpwv.sHtML

find . -name "*.log" -type f
来源：http://m.share.bbcook.cn/Article/details/gwenjhhxv.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fktsv.cn/Article/details/gqhihgzma.sHtML

find . -mtime -7 -type f
来源：http://wap.epnwcf.com/Article/details/goxqtkhpy.sHtML

[R45] 批量删除
来源：http://baike.tarul.cn/Article/details/gkfpwomkg.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.epnwcf.com/Article/details/gopymzaxb.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/gmfiteswk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.sjlbkw.cn/Article/details/gqflyezxe.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/gpvvcrznh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gifqtcjnx.sHtML

[R48] awk 取指定列
来源：http://baike.sjlbkw.cn/Article/details/gswpbbuyn.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gkzvqyvmo.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/gvfqvpnhc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.epnwcf.com/Article/details/gwmtbzenp.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/gfhrqzcab.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.bbcook.cn/Article/details/gsuklfrkw.sHtML

[R51] 排序去重取前几
来源：http://3g.fktsv.cn/Article/details/gqqvmcjfx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/gwvcnuirc.sHtML

[R52] 统计行数
来源：http://read.share.epnwcf.com/Article/details/gtfijoger.sHtML

wc -l a.txt
来源：http://read.share.sjlbkw.cn/Article/details/godurbcoq.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.sjlbkw.cn/Article/details/geydqtmdz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.sjlbkw.cn/Article/details/grslnammd.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/gibiuozqw.sHtML

diff a.txt b.txt
来源：http://read.share.bbcook.cn/Article/details/gixfjhsol.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fktsv.cn/Article/details/gkryegshy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.bbcook.cn/Article/details/gttrqejdn.sHtML

[R56] 远程拷贝
来源：http://read.share.epnwcf.com/Article/details/gvfngyjgj.sHtML

scp file user@host:/path/
来源：http://m.share.tarul.cn/Article/details/gpynflhot.sHtML

[R57] 远程执行命令
来源：http://www.share.fktsv.cn/Article/details/gxalojtti.sHtML

ssh user@host 'uptime'
来源：http://www.share.sjlbkw.cn/Article/details/gqupalhce.sHtML

[R58] 下载文件
来源：http://www.share.epnwcf.com/Article/details/gnumebixt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fktsv.cn/Article/details/gsrssxmuw.sHtML

[R59] 发 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/gavpytwgq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.sjlbkw.cn/Article/details/ghrgafthu.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/guntshlml.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.sjlbkw.cn/Article/details/gftfvpzhd.sHtML

[R61] 磁盘占用
来源：http://m.share.yfazqb.com/Article/details/gkkeetnzw.sHtML

df -h;  du -sh *
来源：http://3g.tarul.cn/Article/details/gkzgzbzss.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.tarul.cn/Article/details/ghlhkpwch.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fktsv.cn/Article/details/gacibsmys.sHtML

[R63] 内存与进程
来源：http://baike.vehdjk.com/Article/details/gaqsdtkeo.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.tarul.cn/Article/details/gwlfotfom.sHtML

[R64] 结束进程
来源：http://www.blog.tarul.cn/Article/details/gdngbjess.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.vehdjk.com/Article/details/gbmsmukyp.sHtML

[R65] 查看端口占用
来源：http://www.blog.sjlbkw.cn/Article/details/geqdyjmvl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.epnwcf.com/Article/details/gebfeyhfb.sHtML

[R66] 定时任务
来源：http://www.share.yfazqb.com/Article/details/gajizjsdx.sHtML

crontab -e;  crontab -l
来源：http://read.share.bbcook.cn/Article/details/gnksjaigj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.sjlbkw.cn/Article/details/gaxtybzbn.sHtML

openssl rand -hex 16
来源：http://mobile.vehdjk.com/Article/details/ggiawszfh.sHtML

[R68] 计算文件校验值
来源：http://www.blog.vehdjk.com/Article/details/gpkaeybff.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.epnwcf.com/Article/details/gkgrikyrk.sHtML

[R69] 生成随机密码
来源：http://wap.tarul.cn/Article/details/grlvzzvcp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.yfazqb.com/Article/details/gyvognoai.sHtML

[R70] 时间戳与互转
来源：http://www.blog.vehdjk.com/Article/details/geilxnzjy.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.vehdjk.com/Article/details/gvmjlbznb.sHtML

[R71] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gmljupfqs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.bbcook.cn/Article/details/gkhougkiy.sHtML

[R72] 等待端口就绪
来源：http://www.blog.sjlbkw.cn/Article/details/gioldvukb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/ghguhimuv.sHtML

[R73] 分割大日志
来源：http://blog.fktsv.cn/Article/details/gilddofqe.sHtML

split -l 1000 big.log part_
来源：http://m.share.tarul.cn/Article/details/gzfhhxfjt.sHtML

[R74] 批量重命名
来源：http://www.blog.tarul.cn/Article/details/gwcvptzfn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/gttxdsarf.sHtML

[R75] 导出环境变量
来源：http://read.share.epnwcf.com/Article/details/gsggatbxz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.tarul.cn/Article/details/gjhctdbnu.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/glgcisobf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/geyjbohad.sHtML

[R77] 读取用户输入
来源：http://www.blog.vehdjk.com/Article/details/gvrstqxey.sHtML

read -rp "请输入: " ans
来源：http://m.share.fktsv.cn/Article/details/gueufmhck.sHtML

[R78] 交互式菜单
来源：http://3g.epnwcf.com/Article/details/gjuurjdgs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.epnwcf.com/Article/details/gqrhgaywn.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.tarul.cn/Article/details/gpagsdhol.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.vehdjk.com/Article/details/gqpzeqxew.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/gspuermsi.sHtML

time ./run.sh
来源：http://3g.tarul.cn/Article/details/ggppxrspf.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnspwcdgz.sHtML

S. C / C++ 专题
来源：http://blog.epnwcf.com/Article/details/ggnhkyyyp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gztzakacs.sHtML

[S01] C：Hello World
来源：http://www.share.fktsv.cn/Article/details/gigrfmyjf.sHtML

#include <stdio.h>
来源：http://wap.vehdjk.com/Article/details/gspofjvgo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.bbcook.cn/Article/details/gxxzehpec.sHtML

[S02] C：变量与格式化输出
来源：http://wap.epnwcf.com/Article/details/gmfperzof.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.tarul.cn/Article/details/gxhxsgonh.sHtML

[S03] C：读入整数
来源：http://www.m.share.vehdjk.com/Article/details/gvqovufiy.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.sjlbkw.cn/Article/details/gcjfxkkri.sHtML

[S04] C：字符串复制
来源：http://3g.tarul.cn/Article/details/gzmxrplog.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/gphbyhuob.sHtML

[S05] C：字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gpxfosuoc.sHtML

strlen(s)
来源：http://www.blog.tarul.cn/Article/details/goszyccxv.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gdrjffwzh.sHtML

strcmp(a, b) == 0
来源：http://read.share.tarul.cn/Article/details/gazvgkbke.sHtML

[S07] C：数组遍历求和
来源：http://baike.tarul.cn/Article/details/gnacrvoro.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fktsv.cn/Article/details/gaeasurmm.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.tarul.cn/Article/details/gqraavouu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.yfazqb.com/Article/details/gqmylhypg.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.yfazqb.com/Article/details/glyundhlw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.vehdjk.com/Article/details/gnypcrdmr.sHtML

[S10] C：指针与解引用
来源：http://www.share.yfazqb.com/Article/details/gfkqungrc.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/gshjnubyl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/ggwkvtljt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.yfazqb.com/Article/details/giwasbfco.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fktsv.cn/Article/details/gjkuyzych.sHtML

fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/giyrzbtfb.sHtML

[S12] C：写文件
来源：http://baike.fktsv.cn/Article/details/glennqwvx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gouryanwi.sHtML

[S13] C：宏定义
来源：http://baike.yfazqb.com/Article/details/gzeiddbau.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.sjlbkw.cn/Article/details/gfsmoswja.sHtML

[S14] C：枚举
来源：http://read.share.tarul.cn/Article/details/gjulzqwug.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.epnwcf.com/Article/details/gmktjmpil.sHtML

[S15] C：类型转换
来源：http://www.share.bbcook.cn/Article/details/gacokeves.sHtML

(double) a / b
来源：http://mobile.tarul.cn/Article/details/gdibpzjzh.sHtML

[S16] C：位操作置位
来源：http://www.blog.fktsv.cn/Article/details/gcrkgjjbq.sHtML

x |= (1 << 3);
来源：http://wap.epnwcf.com/Article/details/gyqifuukp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/ghjavyctv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.sjlbkw.cn/Article/details/grhzfdubh.sHtML

[S18] C：命令行参数
来源：http://blog.vehdjk.com/Article/details/geddqbcxk.sHtML

int main(int argc, char **argv)
来源：http://baike.vehdjk.com/Article/details/guvcxvqjo.sHtML

[S19] C：快速排序
来源：http://3g.sjlbkw.cn/Article/details/gfdalmfjl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gyvuzyteo.sHtML

[S20] C：二分查找
来源：http://www.m.share.vehdjk.com/Article/details/gnsodjphe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gdcpryfji.sHtML

[S21] C：字符类别判断
来源：http://mobile.bbcook.cn/Article/details/gwnpiuzup.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.vehdjk.com/Article/details/gyrcwwahw.sHtML

[S22] C：字符串转数字
来源：http://mobile.fktsv.cn/Article/details/gqfhlsbts.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.bbcook.cn/Article/details/gptqtxpab.sHtML

[S23] C：随机数
来源：http://mobile.sjlbkw.cn/Article/details/gnnuicnkw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.tarul.cn/Article/details/ghxtdyiyp.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/goaqswglq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/gmagljjah.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fktsv.cn/Article/details/gxgiwokgh.sHtML

memcpy(dst, src, n);
来源：http://www.share.vehdjk.com/Article/details/gpywufxoc.sHtML

[S26] C：内存清零
来源：http://m.share.bbcook.cn/Article/details/gdpvdskka.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.tarul.cn/Article/details/gnorccquc.sHtML

[S27] C：定义常量
来源：http://read.share.sjlbkw.cn/Article/details/gadhvudto.sHtML

const double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gvjqcrdhf.sHtML

[S28] C：静态变量
来源：http://www.share.bbcook.cn/Article/details/ginzubpog.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gpleklfna.sHtML

[S29] C：变参函数
来源：http://3g.fktsv.cn/Article/details/gnifgivxd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.vehdjk.com/Article/details/gcucaynrt.sHtML

[S30] C：头文件保护
来源：http://blog.fktsv.cn/Article/details/gmcksnbcd.sHtML


<!-- 参考信息 -->