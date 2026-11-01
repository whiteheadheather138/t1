代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.epnwcf.com/Article/details/gtqikpyrm.sHtML

[Q54] 清空表
来源：http://blog.fktsv.cn/Article/details/gewsletlv.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.bbcook.cn/Article/details/gnzikbvlv.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.vehdjk.com/Article/details/gjavbyipv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gxespkkdb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.epnwcf.com/Article/details/glaifkqwl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.yfazqb.com/Article/details/gdonooobn.sHtML

[Q57] 行号
来源：http://www.m.share.yfazqb.com/Article/details/gurywnnkh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.tarul.cn/Article/details/gkrmijbfv.sHtML

[Q58] 累计求和
来源：http://www.blog.epnwcf.com/Article/details/gxrdyhzxx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.tarul.cn/Article/details/gcuyryvwb.sHtML

[Q59] 分组内累计
来源：http://mobile.sjlbkw.cn/Article/details/getwgyxwk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gjygvlucn.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fktsv.cn/Article/details/gdzghofve.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.epnwcf.com/Article/details/gnupfoeti.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gjlrecric.sHtML

[Q61] 移动平均
来源：http://www.blog.vehdjk.com/Article/details/gmwejdqqa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gjphgxpme.sHtML

[Q62] 分组占比
来源：http://baike.epnwcf.com/Article/details/gzowbxyec.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/ggefizmnq.sHtML

[Q63] 开启事务
来源：http://3g.sjlbkw.cn/Article/details/gziredlxx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.vehdjk.com/Article/details/gnhjaemye.sHtML

[Q64] 提交事务
来源：http://baike.sjlbkw.cn/Article/details/gohbkwmhk.sHtML

COMMIT;
来源：http://3g.sjlbkw.cn/Article/details/gbrcyobmi.sHtML

[Q65] 回滚事务
来源：http://m.share.yfazqb.com/Article/details/gdcxwaugp.sHtML

ROLLBACK;
来源：http://m.share.bbcook.cn/Article/details/gyolzlhbn.sHtML

[Q66] 行锁查询
来源：http://blog.sjlbkw.cn/Article/details/geruxbakf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fktsv.cn/Article/details/gupkgmbej.sHtML

[Q67] 设置隔离级别
来源：http://read.share.vehdjk.com/Article/details/gkriurfhl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.tarul.cn/Article/details/gzqgrtkqw.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/gulsxwjio.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.bbcook.cn/Article/details/gezsdwfmg.sHtML

ROLLBACK TO sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gzwwjvwtu.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/gjgiqavdy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fktsv.cn/Article/details/gufhznntc.sHtML

[Q70] 更新统计信息
来源：http://wap.fktsv.cn/Article/details/gquaxzmkr.sHtML

ANALYZE TABLE users;
来源：http://3g.yfazqb.com/Article/details/gqdktnwix.sHtML

[Q71] 查看建表语句
来源：http://mobile.epnwcf.com/Article/details/gdkrglvuz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.bbcook.cn/Article/details/gsqhffyac.sHtML

[Q72] 查看索引
来源：http://www.m.share.tarul.cn/Article/details/giydnljqj.sHtML

SHOW INDEX FROM users;
来源：http://wap.tarul.cn/Article/details/ghlkxkzot.sHtML

[Q73] 查看表状态
来源：http://blog.yfazqb.com/Article/details/gsbawwiat.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gobnnzjkx.sHtML

[Q74] 强制使用索引
来源：http://baike.epnwcf.com/Article/details/gtactxbcb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.epnwcf.com/Article/details/gsmpxfajx.sHtML

[Q75] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gqqyycerr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.vehdjk.com/Article/details/giogvcfto.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.epnwcf.com/Article/details/ghxxbdhjx.sHtML

[Q76] 按天统计
来源：http://www.blog.vehdjk.com/Article/details/gpqnquepv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.sjlbkw.cn/Article/details/gxrrawvnk.sHtML

[Q77] 时间加减
来源：http://wap.fktsv.cn/Article/details/gnoqfbhbo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.tarul.cn/Article/details/gyvvmnsbn.sHtML

[Q78] 当前时间
来源：http://www.m.share.yfazqb.com/Article/details/gmbztysot.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fktsv.cn/Article/details/gvgzsrbps.sHtML

[Q79] 字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/gzytvfset.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxfobofg.sHtML

[Q80] 字符串截取
来源：http://mobile.sjlbkw.cn/Article/details/gybnxmthv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.yfazqb.com/Article/details/guypkkner.sHtML

[Q81] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gbmwbylrt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.yfazqb.com/Article/details/glqxyzvrt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.tarul.cn/Article/details/gcirpqxef.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gghwodizv.sHtML

[Q83] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gzezwuwdm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gqnfqwebi.sHtML

[Q84] 去除首尾空格
来源：http://baike.fktsv.cn/Article/details/gnxvxcfhv.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gyjzkkmda.sHtML

[Q85] 数值取整
来源：http://www.share.yfazqb.com/Article/details/gmcadtlal.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.epnwcf.com/Article/details/gmbpjlqgx.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.sjlbkw.cn/Article/details/grhdpgefu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fktsv.cn/Article/details/ggmnxowjy.sHtML

[Q87] JSON 字段做条件
来源：http://blog.sjlbkw.cn/Article/details/gtaywndhu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fktsv.cn/Article/details/gonstqzwl.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.bbcook.cn/Article/details/gwcamrsmw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.yfazqb.com/Article/details/gmpktjofx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gybxqkmwu.sHtML

[Q89] 判断表是否存在
来源：http://baike.epnwcf.com/Article/details/gicbueosc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.sjlbkw.cn/Article/details/gffmvomra.sHtML

[Q90] 生成序号列
来源：http://3g.epnwcf.com/Article/details/gbpbsools.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fktsv.cn/Article/details/gxqkqeghl.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/grrnanbyj.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/gzfhfocoo.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gazgkiung.sHtML

[R01] shebang 与严格模式
来源：http://wap.fktsv.cn/Article/details/ganrglsih.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.yfazqb.com/Article/details/gcdkurncv.sHtML

set -euo pipefail
来源：http://read.share.sjlbkw.cn/Article/details/gbhvmnbzw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.bbcook.cn/Article/details/gyxymxrtg.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.yfazqb.com/Article/details/gubipknps.sHtML

[R03] 只读变量
来源：http://www.share.sjlbkw.cn/Article/details/gugkbcjal.sHtML

readonly PI=3.14
来源：http://m.share.vehdjk.com/Article/details/gehlfdmos.sHtML

[R04] 位置参数
来源：http://mobile.fktsv.cn/Article/details/gbwnwqsbn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.yfazqb.com/Article/details/gfxdaynqf.sHtML

[R05] 参数默认值
来源：http://mobile.epnwcf.com/Article/details/goydwbxue.sHtML

name="${1:-default}"
来源：http://m.share.sjlbkw.cn/Article/details/gycghcnvy.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrgzysrl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/gpmtxjdcx.sHtML

[R07] if 判断文件
来源：http://blog.sjlbkw.cn/Article/details/gpjrndlua.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gdjglmpow.sHtML

[R08] 数值比较
来源：http://baike.vehdjk.com/Article/details/gdcmkvajz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.bbcook.cn/Article/details/guhderpqy.sHtML

[R09] 字符串比较
来源：http://3g.fktsv.cn/Article/details/gdegjbdjq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.yfazqb.com/Article/details/gfcoftxyd.sHtML

[R10] 正则匹配
来源：http://3g.sjlbkw.cn/Article/details/ggfvrwaws.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.epnwcf.com/Article/details/gmjtxhwjy.sHtML

[R11] case 多分支
来源：http://mobile.bbcook.cn/Article/details/gflominpp.sHtML

case "$1" in
来源：http://www.m.share.yfazqb.com/Article/details/gwdhfnntd.sHtML

start) echo "启动" ;;
来源：http://m.share.epnwcf.com/Article/details/grmijslwa.sHtML

stop)  echo "停止" ;;
来源：http://www.share.epnwcf.com/Article/details/gbujdgxji.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fktsv.cn/Article/details/ggjrofucd.sHtML

esac
来源：http://www.m.share.tarul.cn/Article/details/gicminslv.sHtML

[R12] for 遍历文件
来源：http://blog.bbcook.cn/Article/details/ggeltycho.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.epnwcf.com/Article/details/gqlsjrzue.sHtML

[R13] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gzmtoyasi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fktsv.cn/Article/details/gwflehgsg.sHtML

[R14] C 风格 for
来源：http://3g.vehdjk.com/Article/details/gtlicfber.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gmnafocwu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gsyfbjyvn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gfewcjryt.sHtML

[R16] until 等待条件
来源：http://3g.epnwcf.com/Article/details/ghfgbqsnv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gvxpyrool.sHtML

[R17] 数组定义与取值
来源：http://m.share.fktsv.cn/Article/details/grjqftoer.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.yfazqb.com/Article/details/ggjhdjytt.sHtML

[R18] 遍历数组
来源：http://wap.yfazqb.com/Article/details/guqasdffo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fktsv.cn/Article/details/gvxsrldrj.sHtML

[R19] 数组长度
来源：http://wap.epnwcf.com/Article/details/glpyyhtmm.sHtML

echo "${#arr[@]}"
来源：http://mobile.epnwcf.com/Article/details/gskbqvofp.sHtML

[R20] 关联数组（字典）
来源：http://read.share.epnwcf.com/Article/details/gdeyrqxmr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fktsv.cn/Article/details/geupgmshf.sHtML

[R21] 字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gjohquejr.sHtML

echo "${#s}"
来源：http://m.share.yfazqb.com/Article/details/gwcsiavpe.sHtML

[R22] 截取子串
来源：http://blog.yfazqb.com/Article/details/gnychyfgs.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/golhfcneu.sHtML

[R23] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/gkvsbaqqg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.sjlbkw.cn/Article/details/ghrslczfp.sHtML

[R24] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gblqudivs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.vehdjk.com/Article/details/gtbddethm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.epnwcf.com/Article/details/grvypdmxe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.vehdjk.com/Article/details/gpcwlriek.sHtML

[R26] 命令替换
来源：http://www.blog.epnwcf.com/Article/details/gqkfmxzvu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.sjlbkw.cn/Article/details/gmhuxazzs.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/gclroegqp.sHtML

echo $((1 + 2 * 3))
来源：http://baike.bbcook.cn/Article/details/gqmbmyipi.sHtML

[R28] 浮点运算
来源：http://www.blog.fktsv.cn/Article/details/gdeszbudi.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.tarul.cn/Article/details/gqabbjwri.sHtML

[R29] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gpibzgrzo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fktsv.cn/Article/details/ghsmuxdvt.sHtML

[R30] 函数返回状态码
来源：http://m.share.yfazqb.com/Article/details/gjkjbhpka.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.yfazqb.com/Article/details/glpwfvjpm.sHtML

[R31] 局部变量
来源：http://m.share.yfazqb.com/Article/details/gfblmyhta.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/ggaidlnys.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/gbbsvrzur.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.sjlbkw.cn/Article/details/gmtwrkixi.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fktsv.cn/Article/details/gjqijyrxb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.bbcook.cn/Article/details/gyohkoqhs.sHtML

[R34] 退出时清理
来源：http://wap.fktsv.cn/Article/details/gprsalonx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.tarul.cn/Article/details/gsfhdxtzd.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/gcbuvwkic.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.vehdjk.com/Article/details/gggfpskrq.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fktsv.cn/Article/details/gddeidevz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.bbcook.cn/Article/details/globejuho.sHtML

[R37] 把输出赋给变量
来源：http://read.share.tarul.cn/Article/details/gogfuecem.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/govbhjehq.sHtML

[R38] 管道串联
来源：http://wap.yfazqb.com/Article/details/gdzzbszjj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fktsv.cn/Article/details/gjvncvrbr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/gdcssrqtl.sHtML

cmd > out.log 2>&1
来源：http://3g.bbcook.cn/Article/details/gbocbuyff.sHtML

[R40] 追加写日志
来源：http://m.share.sjlbkw.cn/Article/details/grqalsegy.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/galugcevx.sHtML

[R41] 丢弃输出
来源：http://www.share.epnwcf.com/Article/details/guzplvmys.sHtML

cmd >/dev/null 2>&1
来源：http://blog.bbcook.cn/Article/details/gblmxfxam.sHtML

[R42] 输入重定向
来源：http://blog.epnwcf.com/Article/details/gnawbbeom.sHtML

wc -l < a.txt
来源：http://www.share.tarul.cn/Article/details/gvublnrzy.sHtML

[R43] 按名字查找文件
来源：http://read.share.tarul.cn/Article/details/gnvvqixwn.sHtML

find . -name "*.log" -type f
来源：http://www.share.vehdjk.com/Article/details/gxxitjtyz.sHtML

[R44] 按修改时间查找
来源：http://wap.yfazqb.com/Article/details/gphxeacwo.sHtML

find . -mtime -7 -type f
来源：http://read.share.tarul.cn/Article/details/ggybiwwdo.sHtML

[R45] 批量删除
来源：http://baike.vehdjk.com/Article/details/gcdzaiani.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fktsv.cn/Article/details/ghioqhxzn.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/gvnrcprex.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.yfazqb.com/Article/details/gpryvzlfa.sHtML

[R47] sed 单行替换
来源：http://www.blog.tarul.cn/Article/details/gaellxylk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fktsv.cn/Article/details/gnoztncfi.sHtML

[R48] awk 取指定列
来源：http://www.share.fktsv.cn/Article/details/gqhmmuijf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gzznrknef.sHtML

[R49] awk 带条件
来源：http://baike.epnwcf.com/Article/details/gqwjdreyh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.epnwcf.com/Article/details/ghfkqimdk.sHtML

[R50] awk 求和
来源：http://www.blog.epnwcf.com/Article/details/gdltgmchn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gqxgknhdc.sHtML

[R51] 排序去重取前几
来源：http://baike.fktsv.cn/Article/details/gboodfxnq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.sjlbkw.cn/Article/details/gsphxjwdw.sHtML

[R52] 统计行数
来源：http://wap.epnwcf.com/Article/details/giswqzbxx.sHtML

wc -l a.txt
来源：http://www.share.tarul.cn/Article/details/gnhtferwd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.epnwcf.com/Article/details/ghchmfrhx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fktsv.cn/Article/details/gmxfnrqok.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/gsbpixuje.sHtML

diff a.txt b.txt
来源：http://baike.sjlbkw.cn/Article/details/grkjixdwa.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/gtjvqpyqx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.bbcook.cn/Article/details/gmiopxtbl.sHtML

[R56] 远程拷贝
来源：http://m.share.bbcook.cn/Article/details/giktzkbjs.sHtML

scp file user@host:/path/
来源：http://3g.fktsv.cn/Article/details/gfxrkbhoa.sHtML

[R57] 远程执行命令
来源：http://baike.sjlbkw.cn/Article/details/gbdxzsfhz.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gakyfuvld.sHtML

[R58] 下载文件
来源：http://blog.epnwcf.com/Article/details/gxbvziofu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/gjmpatufv.sHtML

[R59] 发 POST JSON
来源：http://read.share.tarul.cn/Article/details/gleipklkt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/gstdpvwlt.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/gjlnjefej.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.tarul.cn/Article/details/gahemtvgs.sHtML

[R61] 磁盘占用
来源：http://mobile.sjlbkw.cn/Article/details/gguzgvsgq.sHtML

df -h;  du -sh *
来源：http://www.share.fktsv.cn/Article/details/gwdvgmekw.sHtML

[R62] 找最占空间的文件
来源：http://read.share.vehdjk.com/Article/details/gzlyqbuak.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.epnwcf.com/Article/details/gnfbwhyma.sHtML

[R63] 内存与进程
来源：http://www.blog.yfazqb.com/Article/details/gvgdefepu.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.epnwcf.com/Article/details/gluqcpnaj.sHtML

[R64] 结束进程
来源：http://mobile.tarul.cn/Article/details/gljbcnkvc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.tarul.cn/Article/details/gxbrdrnyt.sHtML

[R65] 查看端口占用
来源：http://www.share.bbcook.cn/Article/details/gxgatktuv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.bbcook.cn/Article/details/gcuokadjw.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gizbkjgsp.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/gisskxlno.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.yfazqb.com/Article/details/gwhosnlwb.sHtML

openssl rand -hex 16
来源：http://www.share.sjlbkw.cn/Article/details/gkkvlbcuv.sHtML

[R68] 计算文件校验值
来源：http://www.share.yfazqb.com/Article/details/geyhjplgj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.tarul.cn/Article/details/glsyigrkq.sHtML

[R69] 生成随机密码
来源：http://wap.bbcook.cn/Article/details/gjlfcchoe.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.yfazqb.com/Article/details/genhwwzle.sHtML

[R70] 时间戳与互转
来源：http://m.share.vehdjk.com/Article/details/gsvldmymi.sHtML

date +%s;  date -d @1700000000
来源：http://blog.bbcook.cn/Article/details/gcmxbknuf.sHtML

[R71] 日期格式化
来源：http://baike.epnwcf.com/Article/details/gsgyylljx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/gbaurosng.sHtML

[R72] 等待端口就绪
来源：http://m.share.tarul.cn/Article/details/gyzqijbyu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gaefsslia.sHtML

[R73] 分割大日志
来源：http://m.share.vehdjk.com/Article/details/gqiyzzbqb.sHtML

split -l 1000 big.log part_
来源：http://www.share.tarul.cn/Article/details/gpnpsfvmu.sHtML

[R74] 批量重命名
来源：http://www.share.tarul.cn/Article/details/gutcphjaa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.bbcook.cn/Article/details/gufcxckbm.sHtML

[R75] 导出环境变量
来源：http://www.blog.vehdjk.com/Article/details/grptjtvzg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.yfazqb.com/Article/details/gynalglwp.sHtML

[R76] 使用临时文件
来源：http://www.blog.vehdjk.com/Article/details/gfumncxyy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.yfazqb.com/Article/details/gwjskybro.sHtML

[R77] 读取用户输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvvzxrfg.sHtML

read -rp "请输入: " ans
来源：http://mobile.epnwcf.com/Article/details/geobhkycq.sHtML

[R78] 交互式菜单
来源：http://www.share.fktsv.cn/Article/details/gbrlldslg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.yfazqb.com/Article/details/greggknul.sHtML

[R79] 解析命令行选项
来源：http://read.share.epnwcf.com/Article/details/gzqegurnc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/gvffbkjaw.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.sjlbkw.cn/Article/details/gdwxebbnh.sHtML

time ./run.sh
来源：http://read.share.bbcook.cn/Article/details/gentgbxbp.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gkcqknyph.sHtML

S. C / C++ 专题
来源：http://www.m.share.yfazqb.com/Article/details/gzfxnlgpz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmrsvhxvq.sHtML

[S01] C：Hello World
来源：http://blog.vehdjk.com/Article/details/gxrwasowj.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/glxyxsmyb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.vehdjk.com/Article/details/gmocabyqw.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.bbcook.cn/Article/details/gdbpevqoz.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.yfazqb.com/Article/details/ghgssxlxm.sHtML

[S03] C：读入整数
来源：http://baike.sjlbkw.cn/Article/details/garkplwyo.sHtML

int x; scanf("%d", &x);
来源：http://3g.bbcook.cn/Article/details/gvwuenpyw.sHtML

[S04] C：字符串复制
来源：http://read.share.yfazqb.com/Article/details/gfywgwvwm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fktsv.cn/Article/details/gzszlfbpn.sHtML

[S05] C：字符串长度
来源：http://baike.yfazqb.com/Article/details/govtezgxo.sHtML

strlen(s)
来源：http://mobile.epnwcf.com/Article/details/gbfmrgjjz.sHtML

[S06] C：字符串比较
来源：http://www.blog.bbcook.cn/Article/details/grcchvlyy.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.yfazqb.com/Article/details/gyxpkbiin.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fktsv.cn/Article/details/gnmwddfdt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fktsv.cn/Article/details/gqagrgqzj.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.sjlbkw.cn/Article/details/gtqiotmhh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fktsv.cn/Article/details/gzpthbmel.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.tarul.cn/Article/details/gjaihmaij.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.epnwcf.com/Article/details/gueqjpqtq.sHtML

[S10] C：指针与解引用
来源：http://read.share.tarul.cn/Article/details/gfdfvmmbp.sHtML

int *p = &a;  *p = 5;
来源：http://baike.yfazqb.com/Article/details/gefrdvndn.sHtML

[S11] C：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gerqauwtl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.tarul.cn/Article/details/gyzwobdce.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.bbcook.cn/Article/details/gqguwkyuh.sHtML

fclose(f);
来源：http://www.blog.tarul.cn/Article/details/guaqpofmq.sHtML

[S12] C：写文件
来源：http://www.share.yfazqb.com/Article/details/gxvudhkot.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gmoedflwn.sHtML

[S13] C：宏定义
来源：http://wap.bbcook.cn/Article/details/glmefczfk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/gfsfmaxjx.sHtML

[S14] C：枚举
来源：http://m.share.vehdjk.com/Article/details/gsffbktwh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fktsv.cn/Article/details/gfhtoywrr.sHtML

[S15] C：类型转换
来源：http://blog.epnwcf.com/Article/details/gxztoupgz.sHtML

(double) a / b
来源：http://mobile.sjlbkw.cn/Article/details/gzbnroxfw.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/gyncttepm.sHtML

x |= (1 << 3);
来源：http://read.share.sjlbkw.cn/Article/details/ghgvuumuy.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.yfazqb.com/Article/details/ghgnykxya.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/ggidqybld.sHtML

[S18] C：命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gdjualkyk.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fktsv.cn/Article/details/giiylitjf.sHtML

[S19] C：快速排序
来源：http://wap.bbcook.cn/Article/details/gfgxvchex.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gtdqjuizx.sHtML

[S20] C：二分查找
来源：http://wap.epnwcf.com/Article/details/gnyuqcayw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/ghrmnwlsi.sHtML

[S21] C：字符类别判断
来源：http://3g.vehdjk.com/Article/details/ggtbwrstj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.bbcook.cn/Article/details/gdsakppxj.sHtML

[S22] C：字符串转数字
来源：http://wap.tarul.cn/Article/details/gtlisfotj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.bbcook.cn/Article/details/gqphvjaxp.sHtML

[S23] C：随机数
来源：http://blog.fktsv.cn/Article/details/gjuadslxd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.vehdjk.com/Article/details/gyvtsfnpx.sHtML

[S24] C：获取本地时间
来源：http://mobile.tarul.cn/Article/details/gbvxvkhbm.sHtML


<!-- 参考信息 -->