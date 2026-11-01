代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gyhkjqnpt.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/gbnyxvhki.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gyhadpavf.sHtML

[Q59] 分组内累计
来源：http://www.blog.yfazqb.com/Article/details/glmuvubbr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.tarul.cn/Article/details/gcgwvtxdb.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.tarul.cn/Article/details/gnvgjrubz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.sjlbkw.cn/Article/details/gdyffwwgh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gzxyauann.sHtML

[Q61] 移动平均
来源：http://www.m.share.bbcook.cn/Article/details/gqtlvisvm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gmcrhcfkw.sHtML

[Q62] 分组占比
来源：http://3g.fktsv.cn/Article/details/glfhydekf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gbdmhaygf.sHtML

[Q63] 开启事务
来源：http://read.share.bbcook.cn/Article/details/gbrfzwgtp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.sjlbkw.cn/Article/details/gedwtrrsr.sHtML

[Q64] 提交事务
来源：http://www.m.share.fktsv.cn/Article/details/gtyialhpi.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/glxpwcrga.sHtML

[Q65] 回滚事务
来源：http://3g.vehdjk.com/Article/details/ghqrghkwv.sHtML

ROLLBACK;
来源：http://www.m.share.tarul.cn/Article/details/ggyjwngob.sHtML

[Q66] 行锁查询
来源：http://baike.yfazqb.com/Article/details/gcaonqkvh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.vehdjk.com/Article/details/gdjjixdro.sHtML

[Q67] 设置隔离级别
来源：http://baike.bbcook.cn/Article/details/gidnaadbj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.vehdjk.com/Article/details/ghgcoysyc.sHtML

[Q68] 保存点
来源：http://mobile.tarul.cn/Article/details/geoznmyxd.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/ggytkeiyc.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gacafllac.sHtML

[Q69] 查看执行计划
来源：http://www.share.tarul.cn/Article/details/gjnqtfejz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.epnwcf.com/Article/details/gkjithcna.sHtML

[Q70] 更新统计信息
来源：http://wap.yfazqb.com/Article/details/gvmwzahqi.sHtML

ANALYZE TABLE users;
来源：http://mobile.fktsv.cn/Article/details/gqxdmbjxp.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/gmncpcupl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.yfazqb.com/Article/details/gwxhwsoyq.sHtML

[Q72] 查看索引
来源：http://www.blog.yfazqb.com/Article/details/gabhpxtoo.sHtML

SHOW INDEX FROM users;
来源：http://3g.vehdjk.com/Article/details/giksrxies.sHtML

[Q73] 查看表状态
来源：http://www.share.fktsv.cn/Article/details/gxagomiif.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.sjlbkw.cn/Article/details/gfwqtskhd.sHtML

[Q74] 强制使用索引
来源：http://wap.fktsv.cn/Article/details/gnctuydqw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.bbcook.cn/Article/details/gohnacopd.sHtML

[Q75] 日期格式化
来源：http://3g.tarul.cn/Article/details/grweyxies.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gxiiukwvo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.yfazqb.com/Article/details/ghlhotrrl.sHtML

[Q76] 按天统计
来源：http://read.share.tarul.cn/Article/details/gqgreobjx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.vehdjk.com/Article/details/gewflmmcs.sHtML

[Q77] 时间加减
来源：http://www.share.vehdjk.com/Article/details/gqjfmnqcv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fktsv.cn/Article/details/grycilxkz.sHtML

[Q78] 当前时间
来源：http://www.share.sjlbkw.cn/Article/details/grmhkawok.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.vehdjk.com/Article/details/gztnehzfm.sHtML

[Q79] 字符串拼接
来源：http://mobile.epnwcf.com/Article/details/gmncmcaat.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fktsv.cn/Article/details/gsqqdxier.sHtML

[Q80] 字符串截取
来源：http://mobile.fktsv.cn/Article/details/gkojlpwqx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gasulhryx.sHtML

[Q81] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gmkaxcmrf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gspukjlob.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.bbcook.cn/Article/details/gvfdifxne.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gmqbefepp.sHtML

[Q83] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gzeuemeuh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gldzqqdvy.sHtML

[Q84] 去除首尾空格
来源：http://3g.fktsv.cn/Article/details/gelnrmenu.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gwqkuidah.sHtML

[Q85] 数值取整
来源：http://blog.epnwcf.com/Article/details/gpjwnnzjp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.vehdjk.com/Article/details/gjxyrnost.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.vehdjk.com/Article/details/gbaykgjkn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.sjlbkw.cn/Article/details/gdamcrtos.sHtML

[Q87] JSON 字段做条件
来源：http://wap.epnwcf.com/Article/details/gzklcoexu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.epnwcf.com/Article/details/gfarfwqbd.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.epnwcf.com/Article/details/gpdflsdnn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.yfazqb.com/Article/details/gdrcmieav.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/golrnlpnd.sHtML

[Q89] 判断表是否存在
来源：http://baike.yfazqb.com/Article/details/gqkghxkyz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.tarul.cn/Article/details/gxdpvvhfd.sHtML

[Q90] 生成序号列
来源：http://m.share.yfazqb.com/Article/details/gmlhtqssl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fktsv.cn/Article/details/geylnicfe.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gggqexota.sHtML

R. Bash 专题
来源：http://www.share.tarul.cn/Article/details/gsshjpife.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gwybwubrj.sHtML

[R01] shebang 与严格模式
来源：http://www.share.sjlbkw.cn/Article/details/grntpftcb.sHtML

#!/usr/bin/env bash
来源：http://www.share.fktsv.cn/Article/details/gaqooqczp.sHtML

set -euo pipefail
来源：http://3g.epnwcf.com/Article/details/gzzpdxyob.sHtML

[R02] 变量赋值与使用
来源：http://m.share.yfazqb.com/Article/details/ghfnugnjs.sHtML

name="Tom"; echo "$name"
来源：http://m.share.sjlbkw.cn/Article/details/guswmrgqr.sHtML

[R03] 只读变量
来源：http://read.share.sjlbkw.cn/Article/details/gzxfbjsqr.sHtML

readonly PI=3.14
来源：http://www.share.sjlbkw.cn/Article/details/giskxibkn.sHtML

[R04] 位置参数
来源：http://wap.tarul.cn/Article/details/gtrigojhz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.epnwcf.com/Article/details/gkzrqnmhb.sHtML

[R05] 参数默认值
来源：http://blog.epnwcf.com/Article/details/ghibnnjkp.sHtML

name="${1:-default}"
来源：http://www.share.yfazqb.com/Article/details/gbebxcqzi.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.bbcook.cn/Article/details/ghebjqflc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gfvxluvgs.sHtML

[R07] if 判断文件
来源：http://baike.vehdjk.com/Article/details/gjlacfjnu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.epnwcf.com/Article/details/gkcyzdrgh.sHtML

[R08] 数值比较
来源：http://blog.bbcook.cn/Article/details/gldlyvcva.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fktsv.cn/Article/details/guuffrcug.sHtML

[R09] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gnbnaggnh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.sjlbkw.cn/Article/details/gzvhcgpnw.sHtML

[R10] 正则匹配
来源：http://www.share.fktsv.cn/Article/details/glqdtklje.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.vehdjk.com/Article/details/ghfaqmzib.sHtML

[R11] case 多分支
来源：http://www.blog.vehdjk.com/Article/details/gybbfdcvs.sHtML

case "$1" in
来源：http://www.blog.bbcook.cn/Article/details/gvuryzvdh.sHtML

start) echo "启动" ;;
来源：http://mobile.bbcook.cn/Article/details/ggehiqkex.sHtML

stop)  echo "停止" ;;
来源：http://read.share.bbcook.cn/Article/details/gnekvxczt.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gjyztrjol.sHtML

esac
来源：http://www.blog.epnwcf.com/Article/details/gqrfxyiax.sHtML

[R12] for 遍历文件
来源：http://blog.epnwcf.com/Article/details/gfshqwilo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.yfazqb.com/Article/details/giehekyxg.sHtML

[R13] for 计数循环
来源：http://wap.tarul.cn/Article/details/gtluxmqrj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/goryzoraa.sHtML

[R14] C 风格 for
来源：http://mobile.fktsv.cn/Article/details/gwryimyke.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/gqefekmib.sHtML

[R15] while 逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gmmpqgukc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.bbcook.cn/Article/details/gcerrpznx.sHtML

[R16] until 等待条件
来源：http://baike.epnwcf.com/Article/details/gjgkextvx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gzfsozxpb.sHtML

[R17] 数组定义与取值
来源：http://mobile.vehdjk.com/Article/details/gszsdevld.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.yfazqb.com/Article/details/geipczvqt.sHtML

[R18] 遍历数组
来源：http://mobile.yfazqb.com/Article/details/gczksrjgx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.yfazqb.com/Article/details/geisxvvvq.sHtML

[R19] 数组长度
来源：http://www.m.share.fktsv.cn/Article/details/gbuaosxqy.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/gyqdoquix.sHtML

[R20] 关联数组（字典）
来源：http://3g.fktsv.cn/Article/details/gkoshmlga.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.sjlbkw.cn/Article/details/ghbybexbz.sHtML

[R21] 字符串长度
来源：http://read.share.bbcook.cn/Article/details/getzrchjy.sHtML

echo "${#s}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgkycoyc.sHtML

[R22] 截取子串
来源：http://www.share.tarul.cn/Article/details/gunyuxpkj.sHtML

echo "${s:0:5}"
来源：http://www.blog.epnwcf.com/Article/details/gbbqspvun.sHtML

[R23] 字符串替换
来源：http://blog.tarul.cn/Article/details/grvgdphir.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fktsv.cn/Article/details/gpdgdbvwb.sHtML

[R24] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gthcpbjhv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.epnwcf.com/Article/details/gxbdmqphj.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fktsv.cn/Article/details/gurvqlbbq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.epnwcf.com/Article/details/ggxyjcnxg.sHtML

[R26] 命令替换
来源：http://www.blog.fktsv.cn/Article/details/ggzqvssmg.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.vehdjk.com/Article/details/ghuorhzgk.sHtML

[R27] 算术展开
来源：http://m.share.epnwcf.com/Article/details/gfywkuqyd.sHtML

echo $((1 + 2 * 3))
来源：http://3g.tarul.cn/Article/details/gqotnbykc.sHtML

[R28] 浮点运算
来源：http://www.share.vehdjk.com/Article/details/gjibkxhaz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/galpevgrd.sHtML

[R29] 定义函数
来源：http://mobile.epnwcf.com/Article/details/grddsgujh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.sjlbkw.cn/Article/details/gpninimuc.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gwpetmnls.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.bbcook.cn/Article/details/glqglerjy.sHtML

[R31] 局部变量
来源：http://baike.bbcook.cn/Article/details/gqemtrtgc.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.vehdjk.com/Article/details/gikqjdjbz.sHtML

[R32] 参数个数校验
来源：http://wap.sjlbkw.cn/Article/details/geyukvzth.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gihilccsi.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.epnwcf.com/Article/details/gtewhnljw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fktsv.cn/Article/details/gbcrbnzyf.sHtML

[R34] 退出时清理
来源：http://mobile.yfazqb.com/Article/details/gxouilveu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gcchkxsdj.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.bbcook.cn/Article/details/gqralevfh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/ghazjrrnl.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.bbcook.cn/Article/details/gjwgfqqcc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.bbcook.cn/Article/details/gtgvuheqy.sHtML

[R37] 把输出赋给变量
来源：http://3g.yfazqb.com/Article/details/gnszxkgwb.sHtML

files=$(ls -1)
来源：http://www.m.share.yfazqb.com/Article/details/gqlosnoqz.sHtML

[R38] 管道串联
来源：http://mobile.vehdjk.com/Article/details/gipvyyfuz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.vehdjk.com/Article/details/gyjjepash.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.epnwcf.com/Article/details/gbfilwnay.sHtML

cmd > out.log 2>&1
来源：http://www.share.sjlbkw.cn/Article/details/glxcoglga.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gzehgbgle.sHtML

echo "log" >> out.log
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpuojpwm.sHtML

[R41] 丢弃输出
来源：http://www.share.bbcook.cn/Article/details/gqwdqboja.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/ggafkdjac.sHtML

[R42] 输入重定向
来源：http://blog.fktsv.cn/Article/details/gjjsyqunj.sHtML

wc -l < a.txt
来源：http://3g.sjlbkw.cn/Article/details/gdcdcyfsq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.epnwcf.com/Article/details/gdllxczyc.sHtML

find . -name "*.log" -type f
来源：http://3g.vehdjk.com/Article/details/gmvrowjip.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/grbzvrslg.sHtML

find . -mtime -7 -type f
来源：http://wap.bbcook.cn/Article/details/gwdgeoswp.sHtML

[R45] 批量删除
来源：http://mobile.bbcook.cn/Article/details/gyphtjlqt.sHtML

find . -name "*.tmp" -delete
来源：http://blog.sjlbkw.cn/Article/details/gfdommrnj.sHtML

[R46] 递归替换文件内容
来源：http://m.share.epnwcf.com/Article/details/gedyktvhh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.epnwcf.com/Article/details/gjexstagb.sHtML

[R47] sed 单行替换
来源：http://blog.tarul.cn/Article/details/gkwxejcrp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.tarul.cn/Article/details/gfpmecwio.sHtML

[R48] awk 取指定列
来源：http://3g.vehdjk.com/Article/details/glgrguxqz.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.vehdjk.com/Article/details/gnttwffvt.sHtML

[R49] awk 带条件
来源：http://baike.vehdjk.com/Article/details/gjxykqadl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.yfazqb.com/Article/details/grqurunhw.sHtML

[R50] awk 求和
来源：http://baike.tarul.cn/Article/details/gdhrsxwnc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.tarul.cn/Article/details/glmjkociy.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/gtrpstrwx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.vehdjk.com/Article/details/gjrjjqfxw.sHtML

[R52] 统计行数
来源：http://www.blog.sjlbkw.cn/Article/details/gbzxpxubg.sHtML

wc -l a.txt
来源：http://read.share.epnwcf.com/Article/details/gwratughc.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.vehdjk.com/Article/details/gmrcbjxmp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fktsv.cn/Article/details/gefsprdlf.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/gefvvxqyq.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/gucmmjxpc.sHtML

[R55] 压缩与解压
来源：http://wap.yfazqb.com/Article/details/gvmmccklg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.sjlbkw.cn/Article/details/gaacdrzik.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/gtrwhyykw.sHtML

scp file user@host:/path/
来源：http://read.share.bbcook.cn/Article/details/gitbxokii.sHtML

[R57] 远程执行命令
来源：http://www.m.share.tarul.cn/Article/details/gelejvszi.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.bbcook.cn/Article/details/gejvfghom.sHtML

[R58] 下载文件
来源：http://blog.tarul.cn/Article/details/gioterqgt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.bbcook.cn/Article/details/gjhrdztdv.sHtML

[R59] 发 POST JSON
来源：http://blog.bbcook.cn/Article/details/gjtatvjjs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.vehdjk.com/Article/details/gpslympri.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/gnahdrian.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.tarul.cn/Article/details/gdyzletae.sHtML

[R61] 磁盘占用
来源：http://3g.vehdjk.com/Article/details/glhqvaidu.sHtML

df -h;  du -sh *
来源：http://baike.tarul.cn/Article/details/gcekxknba.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.bbcook.cn/Article/details/gnxvprcpk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fktsv.cn/Article/details/gsllnqepr.sHtML

[R63] 内存与进程
来源：http://3g.sjlbkw.cn/Article/details/gvdwhtehs.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.bbcook.cn/Article/details/gwshfojrx.sHtML

[R64] 结束进程
来源：http://www.share.bbcook.cn/Article/details/gnpzlrqqs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fktsv.cn/Article/details/gnmuaqjut.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/glqbisrni.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.yfazqb.com/Article/details/giwsqpzsz.sHtML

[R66] 定时任务
来源：http://mobile.epnwcf.com/Article/details/guevyptdp.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/gpoevimsd.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fktsv.cn/Article/details/gpvjpdrii.sHtML

openssl rand -hex 16
来源：http://www.blog.vehdjk.com/Article/details/gzgfvomfz.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/gccgdqgdb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fktsv.cn/Article/details/ggqmocoti.sHtML

[R69] 生成随机密码
来源：http://3g.sjlbkw.cn/Article/details/ghlibwhsi.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/ggombnyhv.sHtML

[R70] 时间戳与互转
来源：http://wap.epnwcf.com/Article/details/ghzyvnvfs.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzxbfppw.sHtML

[R71] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gyvjrqngy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.bbcook.cn/Article/details/gjwqzpvxo.sHtML

[R72] 等待端口就绪
来源：http://blog.fktsv.cn/Article/details/gimrbrurl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fktsv.cn/Article/details/gpxagigeg.sHtML

[R73] 分割大日志
来源：http://wap.bbcook.cn/Article/details/gjbyftebj.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/gdxolnzok.sHtML

[R74] 批量重命名
来源：http://wap.bbcook.cn/Article/details/gprsmtiiv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.yfazqb.com/Article/details/gtpsotway.sHtML

[R75] 导出环境变量
来源：http://mobile.yfazqb.com/Article/details/gslvqofko.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/gdqlceqoz.sHtML

[R76] 使用临时文件
来源：http://www.share.fktsv.cn/Article/details/glzzblqvq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/geuxjzalz.sHtML

[R77] 读取用户输入
来源：http://www.blog.fktsv.cn/Article/details/gcddhlhmi.sHtML

read -rp "请输入: " ans
来源：http://baike.sjlbkw.cn/Article/details/gjtpqpjtw.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/guygloqld.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.yfazqb.com/Article/details/gmzaaykoj.sHtML

[R79] 解析命令行选项
来源：http://read.share.tarul.cn/Article/details/gklffnqle.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/gfftywwnn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.epnwcf.com/Article/details/gtjthoxho.sHtML

time ./run.sh
来源：http://3g.epnwcf.com/Article/details/gcgnbutme.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkzmoliht.sHtML

S. C / C++ 专题
来源：http://wap.vehdjk.com/Article/details/gpnbodehl.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbuqxubwc.sHtML

[S01] C：Hello World
来源：http://www.share.yfazqb.com/Article/details/gmueexpis.sHtML

#include <stdio.h>
来源：http://baike.sjlbkw.cn/Article/details/gvcrgsljd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.bbcook.cn/Article/details/grahqzyxq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.yfazqb.com/Article/details/gdoschuqu.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fktsv.cn/Article/details/gjykzolch.sHtML

[S03] C：读入整数
来源：http://mobile.fktsv.cn/Article/details/gcvflbehe.sHtML

int x; scanf("%d", &x);
来源：http://3g.bbcook.cn/Article/details/guuxyfrud.sHtML

[S04] C：字符串复制
来源：http://m.share.sjlbkw.cn/Article/details/gvjttmwrg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.bbcook.cn/Article/details/groleyfhl.sHtML

[S05] C：字符串长度
来源：http://www.blog.tarul.cn/Article/details/gvqkatqlt.sHtML

strlen(s)
来源：http://wap.yfazqb.com/Article/details/gwhwhbrxl.sHtML

[S06] C：字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gzmmfcmez.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/gxeloqhpp.sHtML

[S07] C：数组遍历求和
来源：http://wap.epnwcf.com/Article/details/gtfwjnixd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.bbcook.cn/Article/details/gsqyjirgu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.bbcook.cn/Article/details/gopqjtsae.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.sjlbkw.cn/Article/details/ghudyayfe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.tarul.cn/Article/details/gozpgirgm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.vehdjk.com/Article/details/gojnfhaon.sHtML

[S10] C：指针与解引用
来源：http://read.share.fktsv.cn/Article/details/gpyxvwecg.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fktsv.cn/Article/details/gscapgytb.sHtML

[S11] C：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gsiyivhhv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.sjlbkw.cn/Article/details/gknachrrm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/gevldsakq.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/gecwkjanj.sHtML

[S12] C：写文件
来源：http://read.share.epnwcf.com/Article/details/gmntajkcq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/ghclynvnx.sHtML

[S13] C：宏定义
来源：http://www.share.fktsv.cn/Article/details/gvapbtmoa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.vehdjk.com/Article/details/gthnmncot.sHtML

[S14] C：枚举
来源：http://3g.vehdjk.com/Article/details/gzhgfrjkv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.epnwcf.com/Article/details/glaxhyqwm.sHtML

[S15] C：类型转换
来源：http://www.share.sjlbkw.cn/Article/details/gzbzmccae.sHtML

(double) a / b
来源：http://m.share.sjlbkw.cn/Article/details/gopdorarf.sHtML

[S16] C：位操作置位
来源：http://m.share.vehdjk.com/Article/details/goulyfgql.sHtML

x |= (1 << 3);
来源：http://www.m.share.fktsv.cn/Article/details/grruqpgzv.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gykxrqdvg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.vehdjk.com/Article/details/gywzdwear.sHtML

[S18] C：命令行参数
来源：http://3g.bbcook.cn/Article/details/gmzmmrqmb.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gqysmyymx.sHtML

[S19] C：快速排序
来源：http://www.m.share.fktsv.cn/Article/details/gcwepxvvc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/ghhusbmuh.sHtML

[S20] C：二分查找
来源：http://3g.tarul.cn/Article/details/govkuqwec.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gjpcwypny.sHtML

[S21] C：字符类别判断
来源：http://mobile.bbcook.cn/Article/details/gwfsfkblj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.epnwcf.com/Article/details/gfowzagkp.sHtML

[S22] C：字符串转数字
来源：http://mobile.fktsv.cn/Article/details/gyxakfdum.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.yfazqb.com/Article/details/gucvbwiav.sHtML

[S23] C：随机数
来源：http://www.share.bbcook.cn/Article/details/gkenszlit.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.sjlbkw.cn/Article/details/grzubkvyk.sHtML

[S24] C：获取本地时间
来源：http://m.share.vehdjk.com/Article/details/gnwehyonb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.epnwcf.com/Article/details/gcoeixyew.sHtML

[S25] C：内存拷贝
来源：http://blog.tarul.cn/Article/details/gsktgsuip.sHtML

memcpy(dst, src, n);
来源：http://baike.sjlbkw.cn/Article/details/gwohgknxq.sHtML

[S26] C：内存清零
来源：http://mobile.epnwcf.com/Article/details/gfyxhifnn.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.vehdjk.com/Article/details/gkautwfhr.sHtML

[S27] C：定义常量
来源：http://m.share.tarul.cn/Article/details/gbosujhaj.sHtML

const double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gbuggbqlo.sHtML

[S28] C：静态变量
来源：http://www.m.share.tarul.cn/Article/details/gtopanxer.sHtML


<!-- 参考信息 -->