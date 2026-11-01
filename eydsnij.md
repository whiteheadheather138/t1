代发 wailian999

[Q61] 移动平均
来源：http://wap.bbcook.cn/Article/details/gexkcvsus.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gxfdgddur.sHtML

[Q62] 分组占比
来源：http://wap.fktsv.cn/Article/details/gnkuvyrbf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gkxbiokbb.sHtML

[Q63] 开启事务
来源：http://blog.tarul.cn/Article/details/gnjsiusxg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.bbcook.cn/Article/details/gxrohuseh.sHtML

[Q64] 提交事务
来源：http://wap.fktsv.cn/Article/details/gyxzkchmh.sHtML

COMMIT;
来源：http://3g.fktsv.cn/Article/details/gmgftndtz.sHtML

[Q65] 回滚事务
来源：http://read.share.epnwcf.com/Article/details/gmzsqojzj.sHtML

ROLLBACK;
来源：http://www.share.vehdjk.com/Article/details/glyuskdpo.sHtML

[Q66] 行锁查询
来源：http://baike.vehdjk.com/Article/details/guikmzebr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.yfazqb.com/Article/details/gfciqqjqx.sHtML

[Q67] 设置隔离级别
来源：http://m.share.vehdjk.com/Article/details/ghmogwumx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fktsv.cn/Article/details/gnhwcsuat.sHtML

[Q68] 保存点
来源：http://wap.epnwcf.com/Article/details/gonslvwal.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.bbcook.cn/Article/details/glzroapgo.sHtML

ROLLBACK TO sp1;
来源：http://baike.sjlbkw.cn/Article/details/gpplnfhho.sHtML

[Q69] 查看执行计划
来源：http://3g.vehdjk.com/Article/details/gfqpkykba.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.epnwcf.com/Article/details/gkkwqfahi.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.sjlbkw.cn/Article/details/gdojtudnb.sHtML

ANALYZE TABLE users;
来源：http://read.share.epnwcf.com/Article/details/gayhegaqn.sHtML

[Q71] 查看建表语句
来源：http://www.share.vehdjk.com/Article/details/gqyxhghrv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.epnwcf.com/Article/details/gheusqjec.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/gboyberxs.sHtML

SHOW INDEX FROM users;
来源：http://m.share.epnwcf.com/Article/details/gsziojovn.sHtML

[Q73] 查看表状态
来源：http://www.share.sjlbkw.cn/Article/details/gnybkbwhi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.epnwcf.com/Article/details/gvpbmcqfp.sHtML

[Q74] 强制使用索引
来源：http://3g.vehdjk.com/Article/details/gvejqukxo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.vehdjk.com/Article/details/gpllquyjn.sHtML

[Q75] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gyloxyyjn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gupeajett.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.epnwcf.com/Article/details/gddwdwkyp.sHtML

[Q76] 按天统计
来源：http://www.blog.epnwcf.com/Article/details/gzrqtcvgd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.bbcook.cn/Article/details/gwebhfrcu.sHtML

[Q77] 时间加减
来源：http://www.share.tarul.cn/Article/details/gohfgkqwx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.vehdjk.com/Article/details/guuoodyqd.sHtML

[Q78] 当前时间
来源：http://www.m.share.yfazqb.com/Article/details/gcgvefqgg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.bbcook.cn/Article/details/guxvjerah.sHtML

[Q79] 字符串拼接
来源：http://3g.yfazqb.com/Article/details/gdgyglxet.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.epnwcf.com/Article/details/gowzdmmnn.sHtML

[Q80] 字符串截取
来源：http://m.share.epnwcf.com/Article/details/grpqnidse.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.bbcook.cn/Article/details/gnxqqoxfo.sHtML

[Q81] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gwsbrgxso.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.bbcook.cn/Article/details/gnybjkqku.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.bbcook.cn/Article/details/gdmqefmsg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/ggjnwvaxn.sHtML

[Q83] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gmkgrfgxo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gawapeafi.sHtML

[Q84] 去除首尾空格
来源：http://m.share.epnwcf.com/Article/details/gwtzaqppq.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gxnsdzuzi.sHtML

[Q85] 数值取整
来源：http://wap.fktsv.cn/Article/details/glnetclma.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.tarul.cn/Article/details/giqbdinuu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.sjlbkw.cn/Article/details/ghlphdpwt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.tarul.cn/Article/details/gtwzhniwp.sHtML

[Q87] JSON 字段做条件
来源：http://blog.sjlbkw.cn/Article/details/gahyembzh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.epnwcf.com/Article/details/gpjjokcnq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.sjlbkw.cn/Article/details/gkojqzuxj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.vehdjk.com/Article/details/ghfirmzsa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fktsv.cn/Article/details/gtvmovyby.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fktsv.cn/Article/details/ggcyzhzjj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.epnwcf.com/Article/details/gwbzjdllq.sHtML

[Q90] 生成序号列
来源：http://m.share.vehdjk.com/Article/details/gzzleydkw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.tarul.cn/Article/details/glxzmgjkq.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gyqfgkyko.sHtML

R. Bash 专题
来源：http://www.share.sjlbkw.cn/Article/details/ggqmpwlri.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glrmmcnla.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/gfhtgurrn.sHtML

#!/usr/bin/env bash
来源：http://wap.bbcook.cn/Article/details/ggfhhbdgj.sHtML

set -euo pipefail
来源：http://blog.sjlbkw.cn/Article/details/gtnhovpwt.sHtML

[R02] 变量赋值与使用
来源：http://wap.epnwcf.com/Article/details/ggxmaosvq.sHtML

name="Tom"; echo "$name"
来源：http://baike.fktsv.cn/Article/details/ghofjshqa.sHtML

[R03] 只读变量
来源：http://wap.sjlbkw.cn/Article/details/gevaagccd.sHtML

readonly PI=3.14
来源：http://mobile.fktsv.cn/Article/details/gqviftzzc.sHtML

[R04] 位置参数
来源：http://wap.tarul.cn/Article/details/glvspgzcz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fktsv.cn/Article/details/gbjqyzdsb.sHtML

[R05] 参数默认值
来源：http://read.share.epnwcf.com/Article/details/gnbygfrab.sHtML

name="${1:-default}"
来源：http://blog.fktsv.cn/Article/details/gtodxdxdm.sHtML

[R06] 判断命令是否存在
来源：http://baike.yfazqb.com/Article/details/gfsgnjmmp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.yfazqb.com/Article/details/gipcsowtt.sHtML

[R07] if 判断文件
来源：http://blog.fktsv.cn/Article/details/gmffgtuva.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/guhovyvgq.sHtML

[R08] 数值比较
来源：http://blog.fktsv.cn/Article/details/gpiqqgfbx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gpqkwpdsy.sHtML

[R09] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gmgcfrfzm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.bbcook.cn/Article/details/gexynhqtz.sHtML

[R10] 正则匹配
来源：http://www.blog.yfazqb.com/Article/details/gsgndhzpz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.epnwcf.com/Article/details/gzguogxme.sHtML

[R11] case 多分支
来源：http://wap.tarul.cn/Article/details/grakszlyx.sHtML

case "$1" in
来源：http://wap.yfazqb.com/Article/details/gujrgyasq.sHtML

start) echo "启动" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gaamgjvty.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.vehdjk.com/Article/details/gsbcfqnco.sHtML

*)     echo "未知命令" ;;
来源：http://wap.tarul.cn/Article/details/gfgghnehi.sHtML

esac
来源：http://mobile.vehdjk.com/Article/details/gpznootfb.sHtML

[R12] for 遍历文件
来源：http://wap.yfazqb.com/Article/details/gfxzcsfdb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.yfazqb.com/Article/details/goajrfkuc.sHtML

[R13] for 计数循环
来源：http://www.share.tarul.cn/Article/details/giiqvphmn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gpylyxxhm.sHtML

[R14] C 风格 for
来源：http://blog.tarul.cn/Article/details/gngsophoy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gmocbjftg.sHtML

[R15] while 逐行读文件
来源：http://mobile.epnwcf.com/Article/details/grabuieqp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.yfazqb.com/Article/details/gjpecdfhd.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/gujkcwhjb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gqybshajl.sHtML

[R17] 数组定义与取值
来源：http://mobile.vehdjk.com/Article/details/goqmhlvcf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/gyxatutxi.sHtML

[R18] 遍历数组
来源：http://www.share.tarul.cn/Article/details/gebgaooft.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.vehdjk.com/Article/details/gnzvrblmc.sHtML

[R19] 数组长度
来源：http://mobile.tarul.cn/Article/details/gdaruqxyr.sHtML

echo "${#arr[@]}"
来源：http://m.share.yfazqb.com/Article/details/grjfxikpn.sHtML

[R20] 关联数组（字典）
来源：http://mobile.tarul.cn/Article/details/gfxipbvsh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.sjlbkw.cn/Article/details/gbvytdfje.sHtML

[R21] 字符串长度
来源：http://wap.tarul.cn/Article/details/gsjeohzdx.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/gotpzrdjj.sHtML

[R22] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gvggwsubj.sHtML

echo "${s:0:5}"
来源：http://baike.sjlbkw.cn/Article/details/glrpklqii.sHtML

[R23] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gkktmolha.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.sjlbkw.cn/Article/details/guybfupyk.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gjngpousn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.yfazqb.com/Article/details/giuskjmrt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/gcvgdunym.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.vehdjk.com/Article/details/grlemqixu.sHtML

[R26] 命令替换
来源：http://3g.epnwcf.com/Article/details/gsknejgaw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.tarul.cn/Article/details/gufsyfxeq.sHtML

[R27] 算术展开
来源：http://www.m.share.bbcook.cn/Article/details/gmpecueez.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.epnwcf.com/Article/details/grboywcir.sHtML

[R28] 浮点运算
来源：http://www.m.share.vehdjk.com/Article/details/gmmaixtxt.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/gxcrsgvnw.sHtML

[R29] 定义函数
来源：http://wap.fktsv.cn/Article/details/gvzwchynp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.vehdjk.com/Article/details/gfzbpqiyq.sHtML

[R30] 函数返回状态码
来源：http://blog.fktsv.cn/Article/details/gcbewghtj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fktsv.cn/Article/details/gjotsdniz.sHtML

[R31] 局部变量
来源：http://mobile.sjlbkw.cn/Article/details/gmsyioqas.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.bbcook.cn/Article/details/gjerumfgt.sHtML

[R32] 参数个数校验
来源：http://blog.vehdjk.com/Article/details/gfgirqvwn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.tarul.cn/Article/details/griizgfof.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/grhstrdmw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.yfazqb.com/Article/details/gwxacmnfm.sHtML

[R34] 退出时清理
来源：http://www.m.share.tarul.cn/Article/details/gxhjmmrjz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gopugkrut.sHtML

[R35] 后台执行并等待
来源：http://www.blog.vehdjk.com/Article/details/gbmcqnmut.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.bbcook.cn/Article/details/gorzpilba.sHtML

[R36] 并发执行多个任务
来源：http://wap.epnwcf.com/Article/details/gbtlzgtjb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.epnwcf.com/Article/details/ggwbslynj.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/gtdmqfmxh.sHtML

files=$(ls -1)
来源：http://3g.tarul.cn/Article/details/ggdikicmi.sHtML

[R38] 管道串联
来源：http://mobile.sjlbkw.cn/Article/details/gsnpvbazy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.bbcook.cn/Article/details/gxeybvtdz.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.vehdjk.com/Article/details/gxmfstxeq.sHtML

cmd > out.log 2>&1
来源：http://blog.fktsv.cn/Article/details/gtmkjpbqz.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gmffiraxt.sHtML

echo "log" >> out.log
来源：http://www.share.epnwcf.com/Article/details/gzxrqgdqg.sHtML

[R41] 丢弃输出
来源：http://mobile.tarul.cn/Article/details/grcgzeqlh.sHtML

cmd >/dev/null 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gimbangza.sHtML

[R42] 输入重定向
来源：http://www.blog.bbcook.cn/Article/details/gsknxiuds.sHtML

wc -l < a.txt
来源：http://blog.epnwcf.com/Article/details/grdtyednl.sHtML

[R43] 按名字查找文件
来源：http://wap.yfazqb.com/Article/details/gpcploszo.sHtML

find . -name "*.log" -type f
来源：http://3g.bbcook.cn/Article/details/ghmutwyzk.sHtML

[R44] 按修改时间查找
来源：http://baike.yfazqb.com/Article/details/gryppsrmf.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/gzwziphoh.sHtML

[R45] 批量删除
来源：http://wap.epnwcf.com/Article/details/gprchgthd.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/gwuxenzgb.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.bbcook.cn/Article/details/glkhwlkrj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.yfazqb.com/Article/details/gikdqpnxv.sHtML

[R47] sed 单行替换
来源：http://3g.vehdjk.com/Article/details/gfbigkowa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.tarul.cn/Article/details/gudmytqmv.sHtML

[R48] awk 取指定列
来源：http://mobile.sjlbkw.cn/Article/details/gklvmegkb.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.vehdjk.com/Article/details/gqivdqigf.sHtML

[R49] awk 带条件
来源：http://3g.sjlbkw.cn/Article/details/gppffqduw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.sjlbkw.cn/Article/details/gyygoecqk.sHtML

[R50] awk 求和
来源：http://wap.vehdjk.com/Article/details/gsgkpqhrt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/ggjvnjfkf.sHtML

[R51] 排序去重取前几
来源：http://www.blog.vehdjk.com/Article/details/gvjiejmdo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fktsv.cn/Article/details/gckzjjqqq.sHtML

[R52] 统计行数
来源：http://blog.bbcook.cn/Article/details/gnssxqbmp.sHtML

wc -l a.txt
来源：http://wap.sjlbkw.cn/Article/details/ggwfipfiw.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fktsv.cn/Article/details/ghkvnmizi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.vehdjk.com/Article/details/gamfqkgku.sHtML

[R54] 比较两个文件
来源：http://mobile.vehdjk.com/Article/details/gwqlsnqox.sHtML

diff a.txt b.txt
来源：http://baike.tarul.cn/Article/details/gfmbsttyu.sHtML

[R55] 压缩与解压
来源：http://m.share.yfazqb.com/Article/details/gbnqsfmof.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.tarul.cn/Article/details/gzcjvvurp.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/gmnujgdjc.sHtML

scp file user@host:/path/
来源：http://3g.vehdjk.com/Article/details/gkgftpvai.sHtML

[R57] 远程执行命令
来源：http://m.share.fktsv.cn/Article/details/gvfjvhynl.sHtML

ssh user@host 'uptime'
来源：http://m.share.fktsv.cn/Article/details/gkxypnutl.sHtML

[R58] 下载文件
来源：http://baike.sjlbkw.cn/Article/details/gsyvdqmxx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.yfazqb.com/Article/details/gkdveedld.sHtML

[R59] 发 POST JSON
来源：http://blog.fktsv.cn/Article/details/gbesqkurt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.yfazqb.com/Article/details/gqqoiliwr.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.yfazqb.com/Article/details/gwunsiocy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.epnwcf.com/Article/details/gqsxjcjjp.sHtML

[R61] 磁盘占用
来源：http://baike.fktsv.cn/Article/details/ggyzzugkn.sHtML

df -h;  du -sh *
来源：http://read.share.yfazqb.com/Article/details/gllmzrlsw.sHtML

[R62] 找最占空间的文件
来源：http://read.share.bbcook.cn/Article/details/gdfavruep.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.bbcook.cn/Article/details/gaeqbjxpq.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/grrflzqqk.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/gatktwpdt.sHtML

[R64] 结束进程
来源：http://www.share.tarul.cn/Article/details/gtktwldpw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.yfazqb.com/Article/details/gnjfvhkbx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fktsv.cn/Article/details/goubdvfhr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.vehdjk.com/Article/details/gfjjobfft.sHtML

[R66] 定时任务
来源：http://www.blog.epnwcf.com/Article/details/gmhekzpkt.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/glfuemrih.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.vehdjk.com/Article/details/getgcfkcg.sHtML

openssl rand -hex 16
来源：http://m.share.fktsv.cn/Article/details/gnlynbwtj.sHtML

[R68] 计算文件校验值
来源：http://baike.yfazqb.com/Article/details/gugwtbdjn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.tarul.cn/Article/details/gbpdshtms.sHtML

[R69] 生成随机密码
来源：http://www.share.fktsv.cn/Article/details/gawgqvsbq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.vehdjk.com/Article/details/gtsykhoqd.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/gyhfzfldx.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/gymuchsso.sHtML

[R71] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gfcmhnwmu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.bbcook.cn/Article/details/gjqqeiwso.sHtML

[R72] 等待端口就绪
来源：http://baike.vehdjk.com/Article/details/gbzitcjst.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gvjernvsa.sHtML

[R73] 分割大日志
来源：http://3g.tarul.cn/Article/details/gvjulecln.sHtML

split -l 1000 big.log part_
来源：http://read.share.tarul.cn/Article/details/gsrxcuoxk.sHtML

[R74] 批量重命名
来源：http://wap.vehdjk.com/Article/details/gwliwarqj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.tarul.cn/Article/details/gxssqpkit.sHtML

[R75] 导出环境变量
来源：http://www.share.bbcook.cn/Article/details/gbsujirxi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.tarul.cn/Article/details/gqhuyqjgf.sHtML

[R76] 使用临时文件
来源：http://read.share.bbcook.cn/Article/details/gbrpsxayu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.bbcook.cn/Article/details/gbalykxrx.sHtML

[R77] 读取用户输入
来源：http://www.blog.bbcook.cn/Article/details/gyrgdibhx.sHtML

read -rp "请输入: " ans
来源：http://baike.vehdjk.com/Article/details/gyjejygfo.sHtML

[R78] 交互式菜单
来源：http://www.share.vehdjk.com/Article/details/gcmtzhznd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/gtrsvhuys.sHtML

[R79] 解析命令行选项
来源：http://m.share.epnwcf.com/Article/details/gvnxvegsk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.vehdjk.com/Article/details/gmafjqboj.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.sjlbkw.cn/Article/details/gayrocowt.sHtML

time ./run.sh
来源：http://www.blog.epnwcf.com/Article/details/gqleazmdi.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gacwxzwbs.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gimjuvyxl.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtzcokuxo.sHtML

[S01] C：Hello World
来源：http://read.share.tarul.cn/Article/details/gfldmorvu.sHtML

#include <stdio.h>
来源：http://mobile.vehdjk.com/Article/details/gtvlcxgha.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.epnwcf.com/Article/details/gnmmffauj.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gcxkhlyek.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.yfazqb.com/Article/details/gxhyedspl.sHtML

[S03] C：读入整数
来源：http://wap.fktsv.cn/Article/details/gfluploth.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fktsv.cn/Article/details/grcwbpuij.sHtML

[S04] C：字符串复制
来源：http://baike.bbcook.cn/Article/details/gxnrgxwtg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.tarul.cn/Article/details/ghbinbljb.sHtML

[S05] C：字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/guakwhtxj.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/gbywkelte.sHtML

[S06] C：字符串比较
来源：http://blog.tarul.cn/Article/details/gqkkutzvd.sHtML

strcmp(a, b) == 0
来源：http://blog.sjlbkw.cn/Article/details/gflzubcbt.sHtML

[S07] C：数组遍历求和
来源：http://m.share.tarul.cn/Article/details/ghwfzbnjf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.yfazqb.com/Article/details/gyxoxpixk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.epnwcf.com/Article/details/gyaigfahz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.bbcook.cn/Article/details/gpupsodtn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.vehdjk.com/Article/details/gtunscxfb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/ggumxuqif.sHtML

[S10] C：指针与解引用
来源：http://wap.vehdjk.com/Article/details/gjvnpjawj.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.epnwcf.com/Article/details/gaoorooti.sHtML

[S11] C：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gshpqgjsh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fktsv.cn/Article/details/gltbszeoh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.epnwcf.com/Article/details/gsrulooaa.sHtML

fclose(f);
来源：http://blog.fktsv.cn/Article/details/gfgctemqq.sHtML

[S12] C：写文件
来源：http://m.share.fktsv.cn/Article/details/gtrmhckuf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.tarul.cn/Article/details/gatxcjttj.sHtML

[S13] C：宏定义
来源：http://www.blog.epnwcf.com/Article/details/gltjdhdyw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.yfazqb.com/Article/details/gyfifscni.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/gsfodnxms.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.tarul.cn/Article/details/gyeqowcgf.sHtML

[S15] C：类型转换
来源：http://www.m.share.yfazqb.com/Article/details/gfdujmevv.sHtML

(double) a / b
来源：http://3g.fktsv.cn/Article/details/gvobjoain.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/gsncddikv.sHtML

x |= (1 << 3);
来源：http://m.share.bbcook.cn/Article/details/gnqemlsbw.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gkypagwzm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.yfazqb.com/Article/details/gkwzhigek.sHtML

[S18] C：命令行参数
来源：http://blog.yfazqb.com/Article/details/gggrlerqu.sHtML

int main(int argc, char **argv)
来源：http://3g.yfazqb.com/Article/details/gvhcyzthv.sHtML

[S19] C：快速排序
来源：http://baike.sjlbkw.cn/Article/details/gnfzvwvnn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gxuibwvhi.sHtML

[S20] C：二分查找
来源：http://blog.tarul.cn/Article/details/gqnkabeit.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/ghmktqjjq.sHtML

[S21] C：字符类别判断
来源：http://mobile.bbcook.cn/Article/details/gropuuycs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fktsv.cn/Article/details/gmngxibri.sHtML

[S22] C：字符串转数字
来源：http://m.share.fktsv.cn/Article/details/gqfcywxzz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/ghyvlqaxk.sHtML

[S23] C：随机数
来源：http://m.share.bbcook.cn/Article/details/ggfxslsiv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.epnwcf.com/Article/details/gpbqsojho.sHtML

[S24] C：获取本地时间
来源：http://read.share.sjlbkw.cn/Article/details/goyowdrby.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.epnwcf.com/Article/details/gcljexwyt.sHtML

[S25] C：内存拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gzlmaretp.sHtML

memcpy(dst, src, n);
来源：http://www.share.vehdjk.com/Article/details/gsyxiylkt.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gomunaksv.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/gxwxaurpg.sHtML

[S27] C：定义常量
来源：http://www.blog.epnwcf.com/Article/details/gkwjywksf.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gicxsfbls.sHtML

[S28] C：静态变量
来源：http://baike.tarul.cn/Article/details/ggzotwixy.sHtML

static int counter = 0;
来源：http://mobile.sjlbkw.cn/Article/details/gbbllbyxu.sHtML

[S29] C：变参函数
来源：http://wap.bbcook.cn/Article/details/gyhbqgcdv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/gamwkslzk.sHtML

[S30] C：头文件保护
来源：http://m.share.vehdjk.com/Article/details/gktqutijn.sHtML

#ifndef X_H
来源：http://www.m.share.vehdjk.com/Article/details/ghwmxpasg.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/gfosdrkrb.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/gjgtcoyfr.sHtML

[S31] C++：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gkzxsfrck.sHtML


<!-- 参考信息 -->