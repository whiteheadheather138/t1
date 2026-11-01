代发 wailian999

[Q61] 移动平均
来源：http://mobile.bbcook.cn/Article/details/gkfhlvxzi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gbzgnfznx.sHtML

[Q62] 分组占比
来源：http://www.blog.fktsv.cn/Article/details/geomontnc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gccdgiqqr.sHtML

[Q63] 开启事务
来源：http://www.blog.vehdjk.com/Article/details/gugvukqrr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.sjlbkw.cn/Article/details/ghuxsvyes.sHtML

[Q64] 提交事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gvykekvhe.sHtML

COMMIT;
来源：http://mobile.sjlbkw.cn/Article/details/gcyrdnggs.sHtML

[Q65] 回滚事务
来源：http://blog.epnwcf.com/Article/details/ghnimwpys.sHtML

ROLLBACK;
来源：http://m.share.bbcook.cn/Article/details/gdkahhbwu.sHtML

[Q66] 行锁查询
来源：http://read.share.bbcook.cn/Article/details/gljqhppyp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.sjlbkw.cn/Article/details/gpaishhmd.sHtML

[Q67] 设置隔离级别
来源：http://baike.tarul.cn/Article/details/gzyctesua.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.yfazqb.com/Article/details/grtdomayk.sHtML

[Q68] 保存点
来源：http://wap.vehdjk.com/Article/details/gslbwossh.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gujogepuo.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.tarul.cn/Article/details/gjsdmnock.sHtML

[Q69] 查看执行计划
来源：http://m.share.tarul.cn/Article/details/gjaqcaglt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.bbcook.cn/Article/details/getzhyzbq.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/gjuubpqrc.sHtML

ANALYZE TABLE users;
来源：http://www.blog.tarul.cn/Article/details/gmaoszgjn.sHtML

[Q71] 查看建表语句
来源：http://m.share.fktsv.cn/Article/details/gbiwxluwq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.sjlbkw.cn/Article/details/gdqawnbie.sHtML

[Q72] 查看索引
来源：http://read.share.fktsv.cn/Article/details/gzqpwzihq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.bbcook.cn/Article/details/gwyzkgqbv.sHtML

[Q73] 查看表状态
来源：http://m.share.yfazqb.com/Article/details/gtayklznp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.bbcook.cn/Article/details/ggzwljiwp.sHtML

[Q74] 强制使用索引
来源：http://read.share.sjlbkw.cn/Article/details/grpsewwpi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.epnwcf.com/Article/details/giblbxkmf.sHtML

[Q75] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gzelpxeiz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gprhdygvi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.epnwcf.com/Article/details/grpagjvdl.sHtML

[Q76] 按天统计
来源：http://mobile.fktsv.cn/Article/details/gwvihzcac.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.epnwcf.com/Article/details/gldmpmnmm.sHtML

[Q77] 时间加减
来源：http://wap.epnwcf.com/Article/details/gpqrdcadx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.bbcook.cn/Article/details/gkzdrjwhd.sHtML

[Q78] 当前时间
来源：http://www.blog.epnwcf.com/Article/details/gfdcpcxwo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.yfazqb.com/Article/details/gwkohokid.sHtML

[Q79] 字符串拼接
来源：http://mobile.bbcook.cn/Article/details/grxduozir.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.bbcook.cn/Article/details/gecbycrsz.sHtML

[Q80] 字符串截取
来源：http://www.blog.yfazqb.com/Article/details/gamllwycm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gsjjfriyb.sHtML

[Q81] 字符串替换
来源：http://3g.sjlbkw.cn/Article/details/gpykdymmh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.yfazqb.com/Article/details/gcdpobqqi.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.vehdjk.com/Article/details/gxddlxnmr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gmuwmxmlq.sHtML

[Q83] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gmaxnared.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gypzjonpg.sHtML

[Q84] 去除首尾空格
来源：http://blog.yfazqb.com/Article/details/gdxgpfzgz.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.tarul.cn/Article/details/gryyztfjm.sHtML

[Q85] 数值取整
来源：http://blog.fktsv.cn/Article/details/guhuzkcue.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gytlmczny.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/gqnmydbfj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.sjlbkw.cn/Article/details/gdnhssqjq.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.vehdjk.com/Article/details/gzxeinpee.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gnsvafuzz.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.sjlbkw.cn/Article/details/glfrwqshj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.bbcook.cn/Article/details/gnstomkeg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.tarul.cn/Article/details/gfuoqexks.sHtML

[Q89] 判断表是否存在
来源：http://www.share.yfazqb.com/Article/details/grboxorvg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.epnwcf.com/Article/details/gncxgfyhi.sHtML

[Q90] 生成序号列
来源：http://wap.fktsv.cn/Article/details/gqrqjecvp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fktsv.cn/Article/details/gqoowgxxp.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggncihplx.sHtML

R. Bash 专题
来源：http://www.blog.tarul.cn/Article/details/gbbeixgoz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gezarlija.sHtML

[R01] shebang 与严格模式
来源：http://m.share.yfazqb.com/Article/details/ggpojovto.sHtML

#!/usr/bin/env bash
来源：http://mobile.epnwcf.com/Article/details/girhywmwj.sHtML

set -euo pipefail
来源：http://www.blog.tarul.cn/Article/details/geeyzukmn.sHtML

[R02] 变量赋值与使用
来源：http://mobile.vehdjk.com/Article/details/ggxyydpmj.sHtML

name="Tom"; echo "$name"
来源：http://m.share.vehdjk.com/Article/details/geajyyhef.sHtML

[R03] 只读变量
来源：http://www.share.sjlbkw.cn/Article/details/gxyoeatrm.sHtML

readonly PI=3.14
来源：http://baike.bbcook.cn/Article/details/gbkcfqdyc.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/gpwpjtant.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.sjlbkw.cn/Article/details/gssclsvau.sHtML

[R05] 参数默认值
来源：http://www.blog.sjlbkw.cn/Article/details/gchkqahlp.sHtML

name="${1:-default}"
来源：http://wap.yfazqb.com/Article/details/gejxaktgz.sHtML

[R06] 判断命令是否存在
来源：http://wap.fktsv.cn/Article/details/gptsxetkt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/gssoybhhj.sHtML

[R07] if 判断文件
来源：http://baike.epnwcf.com/Article/details/gnxhlmqqu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gpjhyazzv.sHtML

[R08] 数值比较
来源：http://3g.vehdjk.com/Article/details/gcsuxrujx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/gogqjezuf.sHtML

[R09] 字符串比较
来源：http://m.share.bbcook.cn/Article/details/gvepkvmaa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.epnwcf.com/Article/details/ghenqptag.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/grjumnbtf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.epnwcf.com/Article/details/gvlazpjkd.sHtML

[R11] case 多分支
来源：http://3g.bbcook.cn/Article/details/gsomrjqsy.sHtML

case "$1" in
来源：http://wap.vehdjk.com/Article/details/gbqralrno.sHtML

start) echo "启动" ;;
来源：http://www.blog.epnwcf.com/Article/details/gquofxppt.sHtML

stop)  echo "停止" ;;
来源：http://read.share.epnwcf.com/Article/details/grxxanbdi.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.bbcook.cn/Article/details/gumtfspmn.sHtML

esac
来源：http://www.share.epnwcf.com/Article/details/gtykgkilm.sHtML

[R12] for 遍历文件
来源：http://mobile.tarul.cn/Article/details/grvfzcion.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.vehdjk.com/Article/details/glelpdjnv.sHtML

[R13] for 计数循环
来源：http://wap.tarul.cn/Article/details/grgfiinsy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/glvajkdxm.sHtML

[R14] C 风格 for
来源：http://3g.vehdjk.com/Article/details/gpcorvmrr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gbawaxbgi.sHtML

[R15] while 逐行读文件
来源：http://blog.yfazqb.com/Article/details/gdrrfzzhq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.yfazqb.com/Article/details/ggmmtnpkb.sHtML

[R16] until 等待条件
来源：http://www.m.share.vehdjk.com/Article/details/gkahlnqwz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/glnjplunb.sHtML

[R17] 数组定义与取值
来源：http://m.share.bbcook.cn/Article/details/gphclzayo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/gfyniqxmp.sHtML

[R18] 遍历数组
来源：http://m.share.epnwcf.com/Article/details/gyuoqkwka.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.tarul.cn/Article/details/gdbyekltr.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gssntzyoy.sHtML

echo "${#arr[@]}"
来源：http://wap.vehdjk.com/Article/details/gmnxdpjmz.sHtML

[R20] 关联数组（字典）
来源：http://read.share.bbcook.cn/Article/details/gogdvlgxa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.bbcook.cn/Article/details/gtfqfmaus.sHtML

[R21] 字符串长度
来源：http://www.share.bbcook.cn/Article/details/gisawmakq.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/grrijcmkh.sHtML

[R22] 截取子串
来源：http://www.m.share.yfazqb.com/Article/details/gntntuewb.sHtML

echo "${s:0:5}"
来源：http://www.blog.tarul.cn/Article/details/gofruvsog.sHtML

[R23] 字符串替换
来源：http://www.blog.fktsv.cn/Article/details/gbazkmmen.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.bbcook.cn/Article/details/gacvzhqac.sHtML

[R24] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gtrigylfe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.tarul.cn/Article/details/gqwmlzipe.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.epnwcf.com/Article/details/ggfikpzyl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.yfazqb.com/Article/details/gxrzthpcx.sHtML

[R26] 命令替换
来源：http://www.share.tarul.cn/Article/details/ggzidtrln.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.tarul.cn/Article/details/gzxjtubio.sHtML

[R27] 算术展开
来源：http://wap.vehdjk.com/Article/details/gbntjgedz.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fktsv.cn/Article/details/gpvtkonke.sHtML

[R28] 浮点运算
来源：http://baike.fktsv.cn/Article/details/gpvsotvzu.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.sjlbkw.cn/Article/details/gowulspsl.sHtML

[R29] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gyofamode.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fktsv.cn/Article/details/gpqjiwxqi.sHtML

[R30] 函数返回状态码
来源：http://read.share.tarul.cn/Article/details/ggvzplbnf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.vehdjk.com/Article/details/gvfbfnukh.sHtML

[R31] 局部变量
来源：http://baike.bbcook.cn/Article/details/gyynukpmu.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.yfazqb.com/Article/details/gdjhdtfdt.sHtML

[R32] 参数个数校验
来源：http://baike.yfazqb.com/Article/details/grkxrqvre.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/grysqeayf.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.sjlbkw.cn/Article/details/gybcsyrgj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.epnwcf.com/Article/details/ggoticdkq.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/grsklbglg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gyehnkfbg.sHtML

[R35] 后台执行并等待
来源：http://mobile.yfazqb.com/Article/details/gbmxyunov.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.bbcook.cn/Article/details/gffogmcfd.sHtML

[R36] 并发执行多个任务
来源：http://3g.epnwcf.com/Article/details/gezjvptcn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fktsv.cn/Article/details/grqagatru.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/gftgujasa.sHtML

files=$(ls -1)
来源：http://www.share.vehdjk.com/Article/details/grfhlfoxg.sHtML

[R38] 管道串联
来源：http://3g.vehdjk.com/Article/details/gqdumiwrd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fktsv.cn/Article/details/grieqasxg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/giroduxur.sHtML

cmd > out.log 2>&1
来源：http://baike.vehdjk.com/Article/details/gunlkjbfj.sHtML

[R40] 追加写日志
来源：http://mobile.epnwcf.com/Article/details/givtbuxry.sHtML

echo "log" >> out.log
来源：http://read.share.yfazqb.com/Article/details/gkcvphash.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gnvdgeztq.sHtML

cmd >/dev/null 2>&1
来源：http://3g.sjlbkw.cn/Article/details/giensssks.sHtML

[R42] 输入重定向
来源：http://3g.fktsv.cn/Article/details/gpsezjvcl.sHtML

wc -l < a.txt
来源：http://wap.sjlbkw.cn/Article/details/gjaxsybuh.sHtML

[R43] 按名字查找文件
来源：http://3g.epnwcf.com/Article/details/gcctprgzx.sHtML

find . -name "*.log" -type f
来源：http://wap.yfazqb.com/Article/details/gltccpvmq.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.bbcook.cn/Article/details/gypatqyyf.sHtML

find . -mtime -7 -type f
来源：http://read.share.tarul.cn/Article/details/gtweiljhg.sHtML

[R45] 批量删除
来源：http://m.share.tarul.cn/Article/details/glrjmwlif.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.sjlbkw.cn/Article/details/gfrfyxumh.sHtML

[R46] 递归替换文件内容
来源：http://www.share.vehdjk.com/Article/details/gxdvuhsbs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.epnwcf.com/Article/details/gekektqtb.sHtML

[R47] sed 单行替换
来源：http://baike.sjlbkw.cn/Article/details/gmpqcmcrw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.epnwcf.com/Article/details/gfwrpbhvm.sHtML

[R48] awk 取指定列
来源：http://read.share.yfazqb.com/Article/details/gvvzxyrrf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gfgyiplee.sHtML

[R49] awk 带条件
来源：http://read.share.sjlbkw.cn/Article/details/gsbwmutnc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.epnwcf.com/Article/details/glbtlqvhs.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gvpvpfqcw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gpekafqvo.sHtML

[R51] 排序去重取前几
来源：http://baike.tarul.cn/Article/details/geanvdcwa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.vehdjk.com/Article/details/gxgfovvhd.sHtML

[R52] 统计行数
来源：http://m.share.yfazqb.com/Article/details/gerrsztho.sHtML

wc -l a.txt
来源：http://mobile.epnwcf.com/Article/details/gszyclabs.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gjfbywwrw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.yfazqb.com/Article/details/gdlzhepgp.sHtML

[R54] 比较两个文件
来源：http://blog.tarul.cn/Article/details/gcnjfknnx.sHtML

diff a.txt b.txt
来源：http://wap.yfazqb.com/Article/details/gsmzvswhl.sHtML

[R55] 压缩与解压
来源：http://read.share.epnwcf.com/Article/details/gunoafzof.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.tarul.cn/Article/details/gpmchinmu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdzaauhy.sHtML

scp file user@host:/path/
来源：http://read.share.epnwcf.com/Article/details/grwayqcup.sHtML

[R57] 远程执行命令
来源：http://m.share.epnwcf.com/Article/details/ghyrqyvlj.sHtML

ssh user@host 'uptime'
来源：http://m.share.sjlbkw.cn/Article/details/glpjwcmqp.sHtML

[R58] 下载文件
来源：http://www.blog.sjlbkw.cn/Article/details/ggcvsaysk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.vehdjk.com/Article/details/gsunhybjf.sHtML

[R59] 发 POST JSON
来源：http://wap.vehdjk.com/Article/details/ggaobuylu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/gjbdbabvk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/gynocffdh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.tarul.cn/Article/details/gzyctqtvq.sHtML

[R61] 磁盘占用
来源：http://3g.sjlbkw.cn/Article/details/gqduwjgqc.sHtML

df -h;  du -sh *
来源：http://www.m.share.bbcook.cn/Article/details/gmjzamybs.sHtML

[R62] 找最占空间的文件
来源：http://www.share.yfazqb.com/Article/details/glibrnvqz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fktsv.cn/Article/details/gafeyeife.sHtML

[R63] 内存与进程
来源：http://www.share.bbcook.cn/Article/details/gnkthsxle.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.bbcook.cn/Article/details/goqpdfgbm.sHtML

[R64] 结束进程
来源：http://www.m.share.fktsv.cn/Article/details/gyegvocer.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.sjlbkw.cn/Article/details/ganirvgib.sHtML

[R65] 查看端口占用
来源：http://www.share.yfazqb.com/Article/details/gzszymhni.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fktsv.cn/Article/details/gqptesoix.sHtML

[R66] 定时任务
来源：http://www.blog.bbcook.cn/Article/details/gvfnpbwce.sHtML

crontab -e;  crontab -l
来源：http://baike.vehdjk.com/Article/details/grtqkeknb.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.bbcook.cn/Article/details/gdejybdpy.sHtML

openssl rand -hex 16
来源：http://m.share.epnwcf.com/Article/details/ghksglxex.sHtML

[R68] 计算文件校验值
来源：http://wap.bbcook.cn/Article/details/gsxyjwoje.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/guyubtete.sHtML

[R69] 生成随机密码
来源：http://www.m.share.tarul.cn/Article/details/gitzvniqo.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.yfazqb.com/Article/details/gnvtappgg.sHtML

[R70] 时间戳与互转
来源：http://wap.vehdjk.com/Article/details/gilsmbzrf.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/gctrqefaa.sHtML

[R71] 日期格式化
来源：http://wap.vehdjk.com/Article/details/gydhwunrg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fktsv.cn/Article/details/gbgxwsozo.sHtML

[R72] 等待端口就绪
来源：http://www.blog.sjlbkw.cn/Article/details/gpflwjoai.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.sjlbkw.cn/Article/details/gvyrvrrof.sHtML

[R73] 分割大日志
来源：http://mobile.sjlbkw.cn/Article/details/gmuubccty.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/gfippspxu.sHtML

[R74] 批量重命名
来源：http://www.blog.tarul.cn/Article/details/gtvlziuzj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.yfazqb.com/Article/details/gdjywvemx.sHtML

[R75] 导出环境变量
来源：http://read.share.yfazqb.com/Article/details/gtefnmtta.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.epnwcf.com/Article/details/gnjazpkqw.sHtML

[R76] 使用临时文件
来源：http://www.blog.bbcook.cn/Article/details/gkoqumcza.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.tarul.cn/Article/details/gumyxcqjy.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/gdxrfmtux.sHtML

read -rp "请输入: " ans
来源：http://read.share.vehdjk.com/Article/details/grvzmazeg.sHtML

[R78] 交互式菜单
来源：http://read.share.tarul.cn/Article/details/gycnpbgpz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/gfjpmofzn.sHtML

[R79] 解析命令行选项
来源：http://read.share.epnwcf.com/Article/details/glyrllwee.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.yfazqb.com/Article/details/gbmrkhyix.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/gudcqlsia.sHtML

time ./run.sh
来源：http://m.share.fktsv.cn/Article/details/glqelqwvd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/geudlshqk.sHtML

S. C / C++ 专题
来源：http://www.share.vehdjk.com/Article/details/gvuhchvnu.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmjmfncfi.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/gicdwlpzd.sHtML

#include <stdio.h>
来源：http://baike.bbcook.cn/Article/details/gpatfqtoh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fktsv.cn/Article/details/gdhkqvjkh.sHtML

[S02] C：变量与格式化输出
来源：http://3g.bbcook.cn/Article/details/gurtctzmo.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.epnwcf.com/Article/details/gzwfpvamx.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/ghgzxzxxy.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.epnwcf.com/Article/details/gwrfdqtlv.sHtML

[S04] C：字符串复制
来源：http://mobile.sjlbkw.cn/Article/details/grcelwnwk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.bbcook.cn/Article/details/gfrzuckpm.sHtML

[S05] C：字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gpoxiuwss.sHtML

strlen(s)
来源：http://3g.tarul.cn/Article/details/glqfwcrkh.sHtML

[S06] C：字符串比较
来源：http://read.share.yfazqb.com/Article/details/goqafiprg.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.yfazqb.com/Article/details/gsbmstvnm.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.sjlbkw.cn/Article/details/gwklsmgnn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.yfazqb.com/Article/details/gdhnaduuw.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.yfazqb.com/Article/details/ghtrvqigp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.epnwcf.com/Article/details/gzdwcwhds.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.bbcook.cn/Article/details/gsiujborj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.sjlbkw.cn/Article/details/gjtzigtoy.sHtML

[S10] C：指针与解引用
来源：http://mobile.sjlbkw.cn/Article/details/gjenmvldw.sHtML

int *p = &a;  *p = 5;
来源：http://blog.epnwcf.com/Article/details/gjmohlupo.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/glassutwc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fktsv.cn/Article/details/gbodtqxpn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.bbcook.cn/Article/details/gdfhcmetj.sHtML

fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gmivxrekx.sHtML

[S12] C：写文件
来源：http://baike.bbcook.cn/Article/details/grasdtbxr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gthkndcvj.sHtML

[S13] C：宏定义
来源：http://www.share.yfazqb.com/Article/details/gcbpphssr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.vehdjk.com/Article/details/gblksozma.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/gpwuknqle.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fktsv.cn/Article/details/ghgfzxtti.sHtML

[S15] C：类型转换
来源：http://blog.epnwcf.com/Article/details/gnxmanews.sHtML

(double) a / b
来源：http://mobile.fktsv.cn/Article/details/gwccfbwby.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/gucjsforu.sHtML

x |= (1 << 3);
来源：http://www.blog.epnwcf.com/Article/details/guutrnejg.sHtML

[S17] C：安全拼接字符串
来源：http://blog.epnwcf.com/Article/details/gawotzoax.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.vehdjk.com/Article/details/gmyqcjfff.sHtML

[S18] C：命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/ggumbncwp.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/giaonqdww.sHtML

[S19] C：快速排序
来源：http://www.m.share.fktsv.cn/Article/details/gzikicycc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/gimqsitvl.sHtML

[S20] C：二分查找
来源：http://m.share.tarul.cn/Article/details/guymybhya.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gdcqtaasz.sHtML

[S21] C：字符类别判断
来源：http://read.share.bbcook.cn/Article/details/gtgpcxhsf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.epnwcf.com/Article/details/ggyzdcrsz.sHtML

[S22] C：字符串转数字
来源：http://read.share.tarul.cn/Article/details/gsojstyrx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/genhwtoqd.sHtML

[S23] C：随机数
来源：http://baike.vehdjk.com/Article/details/gnhipnszo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.tarul.cn/Article/details/gzwlcttmm.sHtML

[S24] C：获取本地时间
来源：http://m.share.bbcook.cn/Article/details/gskmnrztj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/gxfvkdkzf.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fktsv.cn/Article/details/gldqxivmb.sHtML

memcpy(dst, src, n);
来源：http://read.share.epnwcf.com/Article/details/genopkata.sHtML

[S26] C：内存清零
来源：http://read.share.bbcook.cn/Article/details/gdiozucpc.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/gghjlakoz.sHtML

[S27] C：定义常量
来源：http://wap.tarul.cn/Article/details/gcrnedjte.sHtML

const double PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gymgksyob.sHtML

[S28] C：静态变量
来源：http://3g.sjlbkw.cn/Article/details/gggsvseqa.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gipniqaed.sHtML

[S29] C：变参函数
来源：http://www.m.share.fktsv.cn/Article/details/gwrqjdoli.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fktsv.cn/Article/details/gkawyldya.sHtML

[S30] C：头文件保护
来源：http://baike.yfazqb.com/Article/details/gdyvumwvk.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/gwuynjqmx.sHtML

#define X_H
来源：http://www.m.share.vehdjk.com/Article/details/guhdgwtqv.sHtML

#endif
来源：http://m.share.epnwcf.com/Article/details/gsgeigphp.sHtML

[S31] C++：Hello World
来源：http://read.share.bbcook.cn/Article/details/goplrjirm.sHtML


<!-- 参考信息 -->