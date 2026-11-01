代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gjtwiexjs.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.sjlbkw.cn/Article/details/gkqkfgedi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.epnwcf.com/Article/details/ghddineua.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/ggbnwelkz.sHtML

[Q61] 移动平均
来源：http://www.share.sjlbkw.cn/Article/details/gvzgezfkt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gwboasohc.sHtML

[Q62] 分组占比
来源：http://3g.bbcook.cn/Article/details/gxlypjhnt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gqbkngywz.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/gprffeizv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.tarul.cn/Article/details/gjkgkuhpz.sHtML

[Q64] 提交事务
来源：http://m.share.yfazqb.com/Article/details/guhrmuxiv.sHtML

COMMIT;
来源：http://mobile.bbcook.cn/Article/details/gjsmbcrzl.sHtML

[Q65] 回滚事务
来源：http://m.share.sjlbkw.cn/Article/details/gdyfwtfay.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/ggkfsaziw.sHtML

[Q66] 行锁查询
来源：http://wap.vehdjk.com/Article/details/gqaultbgs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.yfazqb.com/Article/details/gjdmsaltv.sHtML

[Q67] 设置隔离级别
来源：http://www.share.bbcook.cn/Article/details/gsezqegzi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fktsv.cn/Article/details/gacbfwhkw.sHtML

[Q68] 保存点
来源：http://www.m.share.tarul.cn/Article/details/gykypcdnn.sHtML

SAVEPOINT sp1;
来源：http://baike.yfazqb.com/Article/details/grbrdwnyi.sHtML

ROLLBACK TO sp1;
来源：http://m.share.vehdjk.com/Article/details/gitucvpzd.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.vehdjk.com/Article/details/gfmprizkk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.vehdjk.com/Article/details/gaiszdrzr.sHtML

[Q70] 更新统计信息
来源：http://wap.fktsv.cn/Article/details/gwnfigtws.sHtML

ANALYZE TABLE users;
来源：http://wap.vehdjk.com/Article/details/gjafznziz.sHtML

[Q71] 查看建表语句
来源：http://3g.fktsv.cn/Article/details/gxhpxdevj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.vehdjk.com/Article/details/glpmmgznx.sHtML

[Q72] 查看索引
来源：http://www.share.vehdjk.com/Article/details/gbwsokizm.sHtML

SHOW INDEX FROM users;
来源：http://mobile.tarul.cn/Article/details/gtzctwtra.sHtML

[Q73] 查看表状态
来源：http://mobile.tarul.cn/Article/details/gjttwodgi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gqswnnuig.sHtML

[Q74] 强制使用索引
来源：http://www.blog.vehdjk.com/Article/details/gxvkyjfoq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.tarul.cn/Article/details/gqcbkjbsw.sHtML

[Q75] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gmztddwzt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.vehdjk.com/Article/details/grocwdixu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.bbcook.cn/Article/details/gxvtfboxs.sHtML

[Q76] 按天统计
来源：http://wap.bbcook.cn/Article/details/gojeekcpx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.sjlbkw.cn/Article/details/gepnvpbvl.sHtML

[Q77] 时间加减
来源：http://read.share.vehdjk.com/Article/details/gygivrlda.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.yfazqb.com/Article/details/gcrmqqakv.sHtML

[Q78] 当前时间
来源：http://www.share.vehdjk.com/Article/details/gbtibedzp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.bbcook.cn/Article/details/gzihzrlzf.sHtML

[Q79] 字符串拼接
来源：http://blog.fktsv.cn/Article/details/gvgwfjxlq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/gbcprvdlp.sHtML

[Q80] 字符串截取
来源：http://wap.yfazqb.com/Article/details/gewyjonge.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gunfidzxe.sHtML

[Q81] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gjnfuzzkx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.bbcook.cn/Article/details/gjqckrcgk.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.tarul.cn/Article/details/gnoeqbhfp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gcznxxiur.sHtML

[Q83] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gbtdvcxni.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/grcivdaaf.sHtML

[Q84] 去除首尾空格
来源：http://read.share.tarul.cn/Article/details/grjjedeki.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/gmjilsglq.sHtML

[Q85] 数值取整
来源：http://www.m.share.vehdjk.com/Article/details/guevvapnl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.epnwcf.com/Article/details/giuwurrrr.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.yfazqb.com/Article/details/gnieegbxf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fktsv.cn/Article/details/gjmjmkemq.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.vehdjk.com/Article/details/grzseajxy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fktsv.cn/Article/details/gwsmspcvk.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/glbxxavcu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.bbcook.cn/Article/details/gjmvzjpyx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gvhuyqcti.sHtML

[Q89] 判断表是否存在
来源：http://blog.yfazqb.com/Article/details/ggrgibpxr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fktsv.cn/Article/details/gmizweefw.sHtML

[Q90] 生成序号列
来源：http://www.share.epnwcf.com/Article/details/gqxkppjte.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.tarul.cn/Article/details/gyiaxhlls.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gifahloem.sHtML

R. Bash 专题
来源：http://m.share.bbcook.cn/Article/details/gybyyshvv.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gmnymrwsc.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.vehdjk.com/Article/details/gamfzytem.sHtML

#!/usr/bin/env bash
来源：http://mobile.tarul.cn/Article/details/gibhkcamo.sHtML

set -euo pipefail
来源：http://baike.epnwcf.com/Article/details/ggsanhuuk.sHtML

[R02] 变量赋值与使用
来源：http://3g.epnwcf.com/Article/details/gnzefvahg.sHtML

name="Tom"; echo "$name"
来源：http://read.share.vehdjk.com/Article/details/gxllltlsv.sHtML

[R03] 只读变量
来源：http://wap.sjlbkw.cn/Article/details/gmhgpgjyo.sHtML

readonly PI=3.14
来源：http://www.m.share.epnwcf.com/Article/details/gzcbrurrn.sHtML

[R04] 位置参数
来源：http://www.share.yfazqb.com/Article/details/goccyeucg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.yfazqb.com/Article/details/gegcpzdvv.sHtML

[R05] 参数默认值
来源：http://www.blog.fktsv.cn/Article/details/gaqozquzf.sHtML

name="${1:-default}"
来源：http://3g.yfazqb.com/Article/details/gorqcmohl.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gdiwkvpfu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gpfmkrxnh.sHtML

[R07] if 判断文件
来源：http://baike.tarul.cn/Article/details/gwfldsoht.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gdjssdhck.sHtML

[R08] 数值比较
来源：http://www.blog.vehdjk.com/Article/details/ghfjycmqc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fktsv.cn/Article/details/gqyykuhbp.sHtML

[R09] 字符串比较
来源：http://www.share.fktsv.cn/Article/details/gkutgpwnr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.bbcook.cn/Article/details/gxglyvudg.sHtML

[R10] 正则匹配
来源：http://read.share.tarul.cn/Article/details/ggptvadfr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gyejlaead.sHtML

[R11] case 多分支
来源：http://3g.fktsv.cn/Article/details/gfcpxzfbn.sHtML

case "$1" in
来源：http://mobile.fktsv.cn/Article/details/gixlxujes.sHtML

start) echo "启动" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gwchmzecs.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gyrmhwpuz.sHtML

*)     echo "未知命令" ;;
来源：http://3g.vehdjk.com/Article/details/gbxpaywwl.sHtML

esac
来源：http://3g.yfazqb.com/Article/details/gnfiskrvk.sHtML

[R12] for 遍历文件
来源：http://read.share.fktsv.cn/Article/details/greavesjc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/gjzdvvcze.sHtML

[R13] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gnzhextkh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gvbluhuyw.sHtML

[R14] C 风格 for
来源：http://www.blog.fktsv.cn/Article/details/ghkwjwafp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gxgmqxnau.sHtML

[R15] while 逐行读文件
来源：http://baike.yfazqb.com/Article/details/gummmqdqk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.vehdjk.com/Article/details/gmvalbpev.sHtML

[R16] until 等待条件
来源：http://wap.sjlbkw.cn/Article/details/gresdshev.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/gokagwhgt.sHtML

[R17] 数组定义与取值
来源：http://blog.bbcook.cn/Article/details/gcvfoijhl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.sjlbkw.cn/Article/details/ghzqnguge.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/ggxiowpte.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.bbcook.cn/Article/details/gyeiugwco.sHtML

[R19] 数组长度
来源：http://wap.epnwcf.com/Article/details/gehgtjser.sHtML

echo "${#arr[@]}"
来源：http://wap.vehdjk.com/Article/details/gvuymyths.sHtML

[R20] 关联数组（字典）
来源：http://baike.epnwcf.com/Article/details/gxjcolfdu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.epnwcf.com/Article/details/grsjzyevx.sHtML

[R21] 字符串长度
来源：http://wap.epnwcf.com/Article/details/gtioxdfqr.sHtML

echo "${#s}"
来源：http://www.blog.bbcook.cn/Article/details/geeocfvts.sHtML

[R22] 截取子串
来源：http://3g.bbcook.cn/Article/details/gbudakhrf.sHtML

echo "${s:0:5}"
来源：http://read.share.sjlbkw.cn/Article/details/gybfsnofy.sHtML

[R23] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gwxbxchpt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.bbcook.cn/Article/details/giknboflp.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gdmtxauvn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.sjlbkw.cn/Article/details/gzltriscw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.epnwcf.com/Article/details/gxzlqjicv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/geowvafms.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/gyvzihnjy.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.epnwcf.com/Article/details/ggodfdwnf.sHtML

[R27] 算术展开
来源：http://3g.tarul.cn/Article/details/ggwmqeyxb.sHtML

echo $((1 + 2 * 3))
来源：http://baike.yfazqb.com/Article/details/gjkytfixd.sHtML

[R28] 浮点运算
来源：http://baike.fktsv.cn/Article/details/gnyeebzkj.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/gxwsrswyj.sHtML

[R29] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/gcejxvdmz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.bbcook.cn/Article/details/goxxxmezv.sHtML

[R30] 函数返回状态码
来源：http://3g.fktsv.cn/Article/details/ghskyrnfy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.vehdjk.com/Article/details/gtlxvccho.sHtML

[R31] 局部变量
来源：http://baike.epnwcf.com/Article/details/gqiyikioj.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.bbcook.cn/Article/details/gufihviwc.sHtML

[R32] 参数个数校验
来源：http://wap.tarul.cn/Article/details/gabsctuwa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/ggfgaulqy.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.vehdjk.com/Article/details/gfcgnxjis.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.sjlbkw.cn/Article/details/gjcpyivcp.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/gzfdlvehi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gaifbedqk.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/gezgjmeca.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.vehdjk.com/Article/details/gaauignhs.sHtML

[R36] 并发执行多个任务
来源：http://blog.fktsv.cn/Article/details/grzbsmrbh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.vehdjk.com/Article/details/guaxspvui.sHtML

[R37] 把输出赋给变量
来源：http://baike.bbcook.cn/Article/details/gkahzezfb.sHtML

files=$(ls -1)
来源：http://read.share.tarul.cn/Article/details/gaunybksj.sHtML

[R38] 管道串联
来源：http://read.share.sjlbkw.cn/Article/details/ghzwcfcbc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.tarul.cn/Article/details/gauybmmly.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.bbcook.cn/Article/details/gjuachish.sHtML

cmd > out.log 2>&1
来源：http://m.share.bbcook.cn/Article/details/gscfslijg.sHtML

[R40] 追加写日志
来源：http://www.m.share.bbcook.cn/Article/details/gsswoyfvl.sHtML

echo "log" >> out.log
来源：http://www.m.share.vehdjk.com/Article/details/glwjhuxtl.sHtML

[R41] 丢弃输出
来源：http://www.share.tarul.cn/Article/details/gkildvysg.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gxkmujmtd.sHtML

[R42] 输入重定向
来源：http://m.share.yfazqb.com/Article/details/ggwcthmbm.sHtML

wc -l < a.txt
来源：http://baike.vehdjk.com/Article/details/gsjqbskno.sHtML

[R43] 按名字查找文件
来源：http://3g.bbcook.cn/Article/details/gtyvosbxq.sHtML

find . -name "*.log" -type f
来源：http://3g.tarul.cn/Article/details/guzblbbqi.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/gquelrzgq.sHtML

find . -mtime -7 -type f
来源：http://wap.vehdjk.com/Article/details/ghvmygpqh.sHtML

[R45] 批量删除
来源：http://www.blog.fktsv.cn/Article/details/gbqfmlcbi.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.tarul.cn/Article/details/gmdmdqaha.sHtML

[R46] 递归替换文件内容
来源：http://baike.fktsv.cn/Article/details/gvkzyludv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.vehdjk.com/Article/details/giprlizqh.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/gitfjxhvn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.bbcook.cn/Article/details/giloiwlqh.sHtML

[R48] awk 取指定列
来源：http://mobile.sjlbkw.cn/Article/details/ggcnpszej.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gfxcyaavh.sHtML

[R49] awk 带条件
来源：http://baike.fktsv.cn/Article/details/gbfwdvsza.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.yfazqb.com/Article/details/glrwmypin.sHtML

[R50] awk 求和
来源：http://m.share.fktsv.cn/Article/details/gftftgxvn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gjroclevz.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/gsxfeykzq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.vehdjk.com/Article/details/ghqtobcyr.sHtML

[R52] 统计行数
来源：http://wap.epnwcf.com/Article/details/gmocnzaas.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gdkrwargc.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gnsnqxloq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.tarul.cn/Article/details/gfgvpvvop.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/gfmciaeqn.sHtML

diff a.txt b.txt
来源：http://www.share.bbcook.cn/Article/details/gswoyjjrr.sHtML

[R55] 压缩与解压
来源：http://www.blog.tarul.cn/Article/details/gjoqetsab.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.bbcook.cn/Article/details/gjflpbbvx.sHtML

[R56] 远程拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gzzbhjfgq.sHtML

scp file user@host:/path/
来源：http://wap.sjlbkw.cn/Article/details/gnccyejtt.sHtML

[R57] 远程执行命令
来源：http://read.share.sjlbkw.cn/Article/details/gyhhpwehf.sHtML

ssh user@host 'uptime'
来源：http://www.share.fktsv.cn/Article/details/gzjrnwywq.sHtML

[R58] 下载文件
来源：http://read.share.sjlbkw.cn/Article/details/gxtvodadp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.vehdjk.com/Article/details/gaewdwxoy.sHtML

[R59] 发 POST JSON
来源：http://read.share.tarul.cn/Article/details/gvsgbnbmh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.tarul.cn/Article/details/gwrpmdulb.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/gatoeehvk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.yfazqb.com/Article/details/gqukjitep.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/guanaegik.sHtML

df -h;  du -sh *
来源：http://wap.vehdjk.com/Article/details/gjeimjbmr.sHtML

[R62] 找最占空间的文件
来源：http://www.share.yfazqb.com/Article/details/glsoocctk.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.sjlbkw.cn/Article/details/gqngswtti.sHtML

[R63] 内存与进程
来源：http://mobile.tarul.cn/Article/details/gvxrdcosg.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.epnwcf.com/Article/details/gyaifsqar.sHtML

[R64] 结束进程
来源：http://3g.yfazqb.com/Article/details/glkwjyons.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.bbcook.cn/Article/details/gogccmsvg.sHtML

[R65] 查看端口占用
来源：http://www.blog.epnwcf.com/Article/details/gdcicbxay.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.bbcook.cn/Article/details/gfdxpbefp.sHtML

[R66] 定时任务
来源：http://mobile.fktsv.cn/Article/details/gypxhvsyd.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/gsgzortbx.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.sjlbkw.cn/Article/details/gtjszuudm.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/gvehxeqkw.sHtML

[R68] 计算文件校验值
来源：http://www.share.epnwcf.com/Article/details/gyqmojami.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.yfazqb.com/Article/details/gwndkjfgc.sHtML

[R69] 生成随机密码
来源：http://www.m.share.tarul.cn/Article/details/gmsiephqs.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.bbcook.cn/Article/details/gzgyrjkmr.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fktsv.cn/Article/details/grfzwoogv.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.sjlbkw.cn/Article/details/gamzbukfv.sHtML

[R71] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gahpttndz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/gtqznhyky.sHtML

[R72] 等待端口就绪
来源：http://wap.epnwcf.com/Article/details/gggpqixrx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gtlnqmvix.sHtML

[R73] 分割大日志
来源：http://3g.sjlbkw.cn/Article/details/gzporowhw.sHtML

split -l 1000 big.log part_
来源：http://www.share.epnwcf.com/Article/details/gfolqmpcs.sHtML

[R74] 批量重命名
来源：http://www.blog.fktsv.cn/Article/details/gowdzxhwj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.epnwcf.com/Article/details/gsiihnolm.sHtML

[R75] 导出环境变量
来源：http://www.m.share.tarul.cn/Article/details/gqeleawpw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.tarul.cn/Article/details/groedogtm.sHtML

[R76] 使用临时文件
来源：http://www.m.share.epnwcf.com/Article/details/goxeifxwd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gpvksopzy.sHtML

[R77] 读取用户输入
来源：http://www.m.share.bbcook.cn/Article/details/gvculkbly.sHtML

read -rp "请输入: " ans
来源：http://mobile.vehdjk.com/Article/details/gofmfahja.sHtML

[R78] 交互式菜单
来源：http://www.blog.sjlbkw.cn/Article/details/gawykvayv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.sjlbkw.cn/Article/details/grbvqpuup.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/gcyuvrzds.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.bbcook.cn/Article/details/gznrvpgds.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.epnwcf.com/Article/details/gjjgeknmr.sHtML

time ./run.sh
来源：http://wap.sjlbkw.cn/Article/details/gnjeungdx.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gfutmbhqh.sHtML

S. C / C++ 专题
来源：http://mobile.vehdjk.com/Article/details/gwhcxcxmx.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gizygekca.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/gmtaknzjx.sHtML

#include <stdio.h>
来源：http://www.blog.vehdjk.com/Article/details/gutivehrk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.bbcook.cn/Article/details/gvhhmcisj.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.tarul.cn/Article/details/gyrnvmkeo.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/gqzarrlfj.sHtML

[S03] C：读入整数
来源：http://3g.tarul.cn/Article/details/gwsdkdiih.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fktsv.cn/Article/details/gkhbgagqx.sHtML

[S04] C：字符串复制
来源：http://wap.fktsv.cn/Article/details/gyjvgqoje.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.tarul.cn/Article/details/giutfxnvr.sHtML

[S05] C：字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gyyhhpvgv.sHtML

strlen(s)
来源：http://3g.sjlbkw.cn/Article/details/gbcssmshs.sHtML

[S06] C：字符串比较
来源：http://baike.bbcook.cn/Article/details/gblrrkkgs.sHtML

strcmp(a, b) == 0
来源：http://blog.fktsv.cn/Article/details/gqpxkxomv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.epnwcf.com/Article/details/gvmxclcdd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fktsv.cn/Article/details/ghodhiuyv.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/ggiyqdzqn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fktsv.cn/Article/details/grsdjkmpx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.vehdjk.com/Article/details/gbumbafwq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.yfazqb.com/Article/details/gbrlivxlv.sHtML

[S10] C：指针与解引用
来源：http://m.share.bbcook.cn/Article/details/gpnrizaij.sHtML

int *p = &a;  *p = 5;
来源：http://baike.yfazqb.com/Article/details/ghzwmrbus.sHtML

[S11] C：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gfflrfepa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.epnwcf.com/Article/details/grpftlytp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fktsv.cn/Article/details/gvpfnvfyb.sHtML

fclose(f);
来源：http://baike.tarul.cn/Article/details/gucmwplpb.sHtML

[S12] C：写文件
来源：http://3g.epnwcf.com/Article/details/gblhhmeew.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.yfazqb.com/Article/details/gwezgzegz.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/gktdcxagi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.yfazqb.com/Article/details/gktjqbtfp.sHtML

[S14] C：枚举
来源：http://www.blog.epnwcf.com/Article/details/gwyeceynn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.epnwcf.com/Article/details/ggijoyknj.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/ggfhvsfln.sHtML

(double) a / b
来源：http://wap.bbcook.cn/Article/details/ggewwzazt.sHtML

[S16] C：位操作置位
来源：http://m.share.tarul.cn/Article/details/gsdocggmz.sHtML

x |= (1 << 3);
来源：http://blog.vehdjk.com/Article/details/gngboxsuk.sHtML

[S17] C：安全拼接字符串
来源：http://wap.yfazqb.com/Article/details/gwowidzjl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/gurmjeevs.sHtML

[S18] C：命令行参数
来源：http://3g.tarul.cn/Article/details/gmmsgotit.sHtML

int main(int argc, char **argv)
来源：http://www.blog.tarul.cn/Article/details/gnhipbhdz.sHtML

[S19] C：快速排序
来源：http://www.m.share.bbcook.cn/Article/details/gnkpcairy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/gqryfqnzh.sHtML

[S20] C：二分查找
来源：http://3g.vehdjk.com/Article/details/gxjvjqwec.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/guspsaboq.sHtML

[S21] C：字符类别判断
来源：http://3g.epnwcf.com/Article/details/gboooxgzr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.tarul.cn/Article/details/gwffzixsl.sHtML

[S22] C：字符串转数字
来源：http://www.share.epnwcf.com/Article/details/gtbguvidl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.vehdjk.com/Article/details/gtoossupj.sHtML

[S23] C：随机数
来源：http://baike.yfazqb.com/Article/details/gwgwrbage.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.tarul.cn/Article/details/gsawjnnfq.sHtML

[S24] C：获取本地时间
来源：http://blog.sjlbkw.cn/Article/details/gyvmdvpfd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.vehdjk.com/Article/details/gbmissccq.sHtML

[S25] C：内存拷贝
来源：http://m.share.tarul.cn/Article/details/gbvbxccmg.sHtML

memcpy(dst, src, n);
来源：http://m.share.yfazqb.com/Article/details/gwbpxivvg.sHtML

[S26] C：内存清零
来源：http://blog.vehdjk.com/Article/details/ghblltsxx.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.yfazqb.com/Article/details/gifqkjgwd.sHtML

[S27] C：定义常量
来源：http://www.m.share.epnwcf.com/Article/details/glwerygmx.sHtML

const double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/goxeysskw.sHtML

[S28] C：静态变量
来源：http://wap.vehdjk.com/Article/details/gnyzdmgdo.sHtML

static int counter = 0;
来源：http://read.share.vehdjk.com/Article/details/gqftccfsl.sHtML

[S29] C：变参函数
来源：http://blog.tarul.cn/Article/details/gfhrnmqdz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.epnwcf.com/Article/details/gvclumewe.sHtML

[S30] C：头文件保护
来源：http://www.blog.tarul.cn/Article/details/gmremccfn.sHtML


<!-- 参考信息 -->