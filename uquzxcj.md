代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.epnwcf.com/Article/details/gxjhwbmnf.sHtML

[Q58] 累计求和
来源：http://3g.fktsv.cn/Article/details/gpsqyuath.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.bbcook.cn/Article/details/gmwzovraz.sHtML

[Q59] 分组内累计
来源：http://3g.fktsv.cn/Article/details/gmdcdwntk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gtgxonqvk.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.yfazqb.com/Article/details/gcmurjsjy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.bbcook.cn/Article/details/gnntmtfpp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.yfazqb.com/Article/details/gqzoyulpv.sHtML

[Q61] 移动平均
来源：http://blog.sjlbkw.cn/Article/details/gsnyrqeqj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gglapdzeb.sHtML

[Q62] 分组占比
来源：http://mobile.epnwcf.com/Article/details/gxvafvhje.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/ghwdwmapo.sHtML

[Q63] 开启事务
来源：http://mobile.yfazqb.com/Article/details/gfxisbjpk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.sjlbkw.cn/Article/details/gqaasqazc.sHtML

[Q64] 提交事务
来源：http://baike.sjlbkw.cn/Article/details/grzvywwzn.sHtML

COMMIT;
来源：http://www.m.share.vehdjk.com/Article/details/gceprqdoy.sHtML

[Q65] 回滚事务
来源：http://mobile.sjlbkw.cn/Article/details/gayqqdtxk.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/gadztctnt.sHtML

[Q66] 行锁查询
来源：http://www.m.share.vehdjk.com/Article/details/gifosejin.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fktsv.cn/Article/details/ghlltqgob.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fktsv.cn/Article/details/ggqtxzxje.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fktsv.cn/Article/details/gztprtfgr.sHtML

[Q68] 保存点
来源：http://read.share.bbcook.cn/Article/details/guogdevcl.sHtML

SAVEPOINT sp1;
来源：http://mobile.fktsv.cn/Article/details/gwouanlmm.sHtML

ROLLBACK TO sp1;
来源：http://wap.yfazqb.com/Article/details/gfreyljka.sHtML

[Q69] 查看执行计划
来源：http://read.share.fktsv.cn/Article/details/grddlzsfw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.yfazqb.com/Article/details/gprzpfnps.sHtML

[Q70] 更新统计信息
来源：http://read.share.tarul.cn/Article/details/gnagmdteb.sHtML

ANALYZE TABLE users;
来源：http://wap.fktsv.cn/Article/details/gaujtipgl.sHtML

[Q71] 查看建表语句
来源：http://baike.vehdjk.com/Article/details/gustcsyvg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.vehdjk.com/Article/details/gbqljqyag.sHtML

[Q72] 查看索引
来源：http://wap.yfazqb.com/Article/details/gkosoudgq.sHtML

SHOW INDEX FROM users;
来源：http://www.share.yfazqb.com/Article/details/ghdbpgidm.sHtML

[Q73] 查看表状态
来源：http://mobile.yfazqb.com/Article/details/gvddhaghu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.epnwcf.com/Article/details/gsumecalc.sHtML

[Q74] 强制使用索引
来源：http://baike.fktsv.cn/Article/details/gagijkpaw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.sjlbkw.cn/Article/details/glflpdhmm.sHtML

[Q75] 日期格式化
来源：http://wap.fktsv.cn/Article/details/gnpjebrlv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.yfazqb.com/Article/details/gbckrsmre.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fktsv.cn/Article/details/gfurtfrzx.sHtML

[Q76] 按天统计
来源：http://www.m.share.fktsv.cn/Article/details/grlfbppot.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/gsbjqlwff.sHtML

[Q77] 时间加减
来源：http://m.share.bbcook.cn/Article/details/gqgjfklxh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.epnwcf.com/Article/details/gdwntzfsd.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gumsayewm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.bbcook.cn/Article/details/gfbarmoco.sHtML

[Q79] 字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gblgaxotp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.sjlbkw.cn/Article/details/gvtxvugrj.sHtML

[Q80] 字符串截取
来源：http://m.share.bbcook.cn/Article/details/gcpcdcrvi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gyvqddoek.sHtML

[Q81] 字符串替换
来源：http://3g.vehdjk.com/Article/details/giergogzf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.tarul.cn/Article/details/grjvsawuj.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fktsv.cn/Article/details/gytitkflf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gesurqlev.sHtML

[Q83] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gknfawxym.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gvkvuiyit.sHtML

[Q84] 去除首尾空格
来源：http://www.share.bbcook.cn/Article/details/gbwoupniv.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gyltuaqcs.sHtML

[Q85] 数值取整
来源：http://www.blog.epnwcf.com/Article/details/gbbyiuxyq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.vehdjk.com/Article/details/gwhxwjblx.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.epnwcf.com/Article/details/gztstdrki.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gaqygijct.sHtML

[Q87] JSON 字段做条件
来源：http://blog.yfazqb.com/Article/details/grmrlrqeo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.bbcook.cn/Article/details/gonzugucr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.vehdjk.com/Article/details/gmhijwnkr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fktsv.cn/Article/details/gkpndjalq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gqbkwweqb.sHtML

[Q89] 判断表是否存在
来源：http://www.share.tarul.cn/Article/details/gpklbswjh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fktsv.cn/Article/details/gkrrakqtr.sHtML

[Q90] 生成序号列
来源：http://m.share.bbcook.cn/Article/details/gpxkykfyf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.epnwcf.com/Article/details/ggfccxghr.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmgdmzyus.sHtML

R. Bash 专题
来源：http://baike.yfazqb.com/Article/details/gcvktlxvh.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gomwmcwto.sHtML

[R01] shebang 与严格模式
来源：http://www.share.vehdjk.com/Article/details/guhphaefl.sHtML

#!/usr/bin/env bash
来源：http://blog.tarul.cn/Article/details/gkznfjglg.sHtML

set -euo pipefail
来源：http://3g.epnwcf.com/Article/details/ghmrmlwsn.sHtML

[R02] 变量赋值与使用
来源：http://m.share.tarul.cn/Article/details/gznzpkfkm.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.tarul.cn/Article/details/gjtcpmuqr.sHtML

[R03] 只读变量
来源：http://www.blog.tarul.cn/Article/details/gqtdgitfv.sHtML

readonly PI=3.14
来源：http://www.share.sjlbkw.cn/Article/details/ggibrvwun.sHtML

[R04] 位置参数
来源：http://www.blog.vehdjk.com/Article/details/gwphlzjdm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.vehdjk.com/Article/details/gnuikanfe.sHtML

[R05] 参数默认值
来源：http://blog.yfazqb.com/Article/details/gmuygxvuh.sHtML

name="${1:-default}"
来源：http://blog.tarul.cn/Article/details/gkdknzzvu.sHtML

[R06] 判断命令是否存在
来源：http://blog.vehdjk.com/Article/details/gdlgvtzhk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gisedbwsf.sHtML

[R07] if 判断文件
来源：http://www.blog.vehdjk.com/Article/details/gvutafbkh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.epnwcf.com/Article/details/gwvkbojdc.sHtML

[R08] 数值比较
来源：http://3g.epnwcf.com/Article/details/goscsknnj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.vehdjk.com/Article/details/gblyuajfn.sHtML

[R09] 字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gjsiylytj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.yfazqb.com/Article/details/gqydibunw.sHtML

[R10] 正则匹配
来源：http://blog.yfazqb.com/Article/details/gscavrguh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.epnwcf.com/Article/details/ghzrncbbn.sHtML

[R11] case 多分支
来源：http://www.blog.yfazqb.com/Article/details/gazhkcggv.sHtML

case "$1" in
来源：http://read.share.fktsv.cn/Article/details/gybspjlni.sHtML

start) echo "启动" ;;
来源：http://3g.yfazqb.com/Article/details/glezixvsa.sHtML

stop)  echo "停止" ;;
来源：http://read.share.vehdjk.com/Article/details/gfcerlobw.sHtML

*)     echo "未知命令" ;;
来源：http://3g.sjlbkw.cn/Article/details/gasjzuhtx.sHtML

esac
来源：http://www.blog.epnwcf.com/Article/details/gswovqzgx.sHtML

[R12] for 遍历文件
来源：http://mobile.fktsv.cn/Article/details/glprzkzst.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.epnwcf.com/Article/details/gjloahkwm.sHtML

[R13] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/grklrsfiu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gyzmfekcp.sHtML

[R14] C 风格 for
来源：http://read.share.fktsv.cn/Article/details/gavaqavby.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gagkunbho.sHtML

[R15] while 逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gwnmghdzs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.vehdjk.com/Article/details/gptojbxbe.sHtML

[R16] until 等待条件
来源：http://blog.bbcook.cn/Article/details/grbgfqywz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gxjbyegqu.sHtML

[R17] 数组定义与取值
来源：http://baike.yfazqb.com/Article/details/gairjeszn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.bbcook.cn/Article/details/glglfgxhr.sHtML

[R18] 遍历数组
来源：http://www.share.bbcook.cn/Article/details/gfhtuwdsn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.vehdjk.com/Article/details/glspragcc.sHtML

[R19] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gbxxyjcro.sHtML

echo "${#arr[@]}"
来源：http://www.blog.yfazqb.com/Article/details/ggzsnljce.sHtML

[R20] 关联数组（字典）
来源：http://blog.fktsv.cn/Article/details/gemroljsm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.tarul.cn/Article/details/gskifacdn.sHtML

[R21] 字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/gwzzvascn.sHtML

echo "${#s}"
来源：http://www.blog.fktsv.cn/Article/details/gadymyyex.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/gceurcpvb.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/guksltgsp.sHtML

[R23] 字符串替换
来源：http://blog.fktsv.cn/Article/details/giwxmvizd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.yfazqb.com/Article/details/gtymcoflk.sHtML

[R24] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gakcolymd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fktsv.cn/Article/details/gkblsfczd.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.yfazqb.com/Article/details/gmavcovcd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/gqmzfzkcy.sHtML

[R26] 命令替换
来源：http://blog.fktsv.cn/Article/details/gzvtyvrye.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtouqttmx.sHtML

[R27] 算术展开
来源：http://m.share.yfazqb.com/Article/details/gdsovlfty.sHtML

echo $((1 + 2 * 3))
来源：http://baike.tarul.cn/Article/details/gebwuthlv.sHtML

[R28] 浮点运算
来源：http://baike.fktsv.cn/Article/details/gdywhhtjh.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fktsv.cn/Article/details/gbrlobbzg.sHtML

[R29] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/guwkaaciu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.epnwcf.com/Article/details/gbepzxnxf.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.vehdjk.com/Article/details/ggszampvb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.bbcook.cn/Article/details/gdlcwaemh.sHtML

[R31] 局部变量
来源：http://www.share.bbcook.cn/Article/details/gkzsuyfqm.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/gflbeoqdu.sHtML

[R32] 参数个数校验
来源：http://blog.fktsv.cn/Article/details/gmimzohek.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/gtaybpags.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.vehdjk.com/Article/details/gbwkldiqx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.tarul.cn/Article/details/gsreoijnm.sHtML

[R34] 退出时清理
来源：http://www.m.share.tarul.cn/Article/details/gzzpemwbe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gfhezpnhs.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/ghplvywuc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fktsv.cn/Article/details/gxmrsrlwa.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.tarul.cn/Article/details/gqjidwygn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.epnwcf.com/Article/details/gtybaynht.sHtML

[R37] 把输出赋给变量
来源：http://baike.epnwcf.com/Article/details/grpsmndng.sHtML

files=$(ls -1)
来源：http://3g.epnwcf.com/Article/details/gahgyqyvz.sHtML

[R38] 管道串联
来源：http://www.share.epnwcf.com/Article/details/geldciish.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.vehdjk.com/Article/details/gcmdpordc.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.sjlbkw.cn/Article/details/grmlwyueb.sHtML

cmd > out.log 2>&1
来源：http://www.blog.tarul.cn/Article/details/geauyzqqh.sHtML

[R40] 追加写日志
来源：http://baike.vehdjk.com/Article/details/gtrhfberg.sHtML

echo "log" >> out.log
来源：http://www.blog.yfazqb.com/Article/details/gadufvmqy.sHtML

[R41] 丢弃输出
来源：http://wap.fktsv.cn/Article/details/gmmexiotg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.tarul.cn/Article/details/gvhsuzygo.sHtML

[R42] 输入重定向
来源：http://wap.epnwcf.com/Article/details/gordhthjf.sHtML

wc -l < a.txt
来源：http://3g.vehdjk.com/Article/details/gustzukbv.sHtML

[R43] 按名字查找文件
来源：http://www.blog.epnwcf.com/Article/details/gtspmwqsw.sHtML

find . -name "*.log" -type f
来源：http://mobile.sjlbkw.cn/Article/details/gnhrucdms.sHtML

[R44] 按修改时间查找
来源：http://www.blog.bbcook.cn/Article/details/gcadsrwvp.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/gvupxyzvh.sHtML

[R45] 批量删除
来源：http://read.share.fktsv.cn/Article/details/gofqahlqu.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.yfazqb.com/Article/details/gytyycyie.sHtML

[R46] 递归替换文件内容
来源：http://baike.epnwcf.com/Article/details/glsenxzcd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.tarul.cn/Article/details/gswwrlkru.sHtML

[R47] sed 单行替换
来源：http://m.share.vehdjk.com/Article/details/grzlbdudy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.vehdjk.com/Article/details/gvxuylihk.sHtML

[R48] awk 取指定列
来源：http://mobile.fktsv.cn/Article/details/gxbwctmpl.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.bbcook.cn/Article/details/gkuqksiak.sHtML

[R49] awk 带条件
来源：http://blog.yfazqb.com/Article/details/gmqktylmu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.sjlbkw.cn/Article/details/gvjhrrlvw.sHtML

[R50] awk 求和
来源：http://www.blog.bbcook.cn/Article/details/gndlsleeo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.yfazqb.com/Article/details/gnskfjkcv.sHtML

[R51] 排序去重取前几
来源：http://blog.vehdjk.com/Article/details/gcmebdcxp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.yfazqb.com/Article/details/ggtoawwkg.sHtML

[R52] 统计行数
来源：http://m.share.yfazqb.com/Article/details/gzinkupff.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gendsldfv.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.sjlbkw.cn/Article/details/gvhqjezxl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/ggsgamkdg.sHtML

[R54] 比较两个文件
来源：http://www.blog.sjlbkw.cn/Article/details/goqcrjdkq.sHtML

diff a.txt b.txt
来源：http://blog.tarul.cn/Article/details/gzgvetmri.sHtML

[R55] 压缩与解压
来源：http://3g.bbcook.cn/Article/details/ggpjadqkz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.sjlbkw.cn/Article/details/goalifvsc.sHtML

[R56] 远程拷贝
来源：http://www.share.fktsv.cn/Article/details/ghtnqozwh.sHtML

scp file user@host:/path/
来源：http://read.share.vehdjk.com/Article/details/ggwlvmuyi.sHtML

[R57] 远程执行命令
来源：http://m.share.tarul.cn/Article/details/grydkbiak.sHtML

ssh user@host 'uptime'
来源：http://baike.bbcook.cn/Article/details/gisccuowx.sHtML

[R58] 下载文件
来源：http://www.m.share.bbcook.cn/Article/details/gykfiehhp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.epnwcf.com/Article/details/gnucamzha.sHtML

[R59] 发 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gcetxowda.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.yfazqb.com/Article/details/glbinowqg.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/gvivdpyel.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.epnwcf.com/Article/details/ghniviyaq.sHtML

[R61] 磁盘占用
来源：http://read.share.vehdjk.com/Article/details/gggjnqiik.sHtML

df -h;  du -sh *
来源：http://blog.vehdjk.com/Article/details/garkvwnct.sHtML

[R62] 找最占空间的文件
来源：http://www.share.bbcook.cn/Article/details/gtmjlkhzq.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.bbcook.cn/Article/details/gingbkdoy.sHtML

[R63] 内存与进程
来源：http://wap.epnwcf.com/Article/details/gvocomkib.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/gyvohwvbx.sHtML

[R64] 结束进程
来源：http://wap.vehdjk.com/Article/details/grzagbhby.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.yfazqb.com/Article/details/gavazhcro.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/gchbsaikw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.sjlbkw.cn/Article/details/golgfjwde.sHtML

[R66] 定时任务
来源：http://blog.bbcook.cn/Article/details/gyrcukmwz.sHtML

crontab -e;  crontab -l
来源：http://www.share.epnwcf.com/Article/details/gksnpgotc.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.tarul.cn/Article/details/gndbjmcbh.sHtML

openssl rand -hex 16
来源：http://3g.tarul.cn/Article/details/gnzchkupz.sHtML

[R68] 计算文件校验值
来源：http://baike.bbcook.cn/Article/details/gllyntzoo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.sjlbkw.cn/Article/details/ghrugoxsj.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/gtekfedwz.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/gjtlhsrgf.sHtML

[R70] 时间戳与互转
来源：http://m.share.tarul.cn/Article/details/ggiapoqtl.sHtML

date +%s;  date -d @1700000000
来源：http://blog.epnwcf.com/Article/details/gjnmgmtui.sHtML

[R71] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gaccqanwy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/gpncdagiq.sHtML

[R72] 等待端口就绪
来源：http://read.share.vehdjk.com/Article/details/guljgaock.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gwbzmeqls.sHtML

[R73] 分割大日志
来源：http://wap.vehdjk.com/Article/details/ggjrpheyt.sHtML

split -l 1000 big.log part_
来源：http://3g.vehdjk.com/Article/details/ghfrrmwmv.sHtML

[R74] 批量重命名
来源：http://mobile.tarul.cn/Article/details/gzmwcyoep.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.vehdjk.com/Article/details/gxfgilrkm.sHtML

[R75] 导出环境变量
来源：http://read.share.sjlbkw.cn/Article/details/glliepqhr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fktsv.cn/Article/details/ghwjwbrpa.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/gkbfszzow.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gmqpjrpxl.sHtML

[R77] 读取用户输入
来源：http://blog.vehdjk.com/Article/details/gfgrvtlxw.sHtML

read -rp "请输入: " ans
来源：http://read.share.epnwcf.com/Article/details/gunlzufne.sHtML

[R78] 交互式菜单
来源：http://m.share.fktsv.cn/Article/details/gwdjooogo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.bbcook.cn/Article/details/gpeygyyaw.sHtML

[R79] 解析命令行选项
来源：http://www.blog.sjlbkw.cn/Article/details/gykafkymt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/gwytwqauj.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.bbcook.cn/Article/details/gnugzlhuu.sHtML

time ./run.sh
来源：http://www.blog.fktsv.cn/Article/details/gatuyunuy.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqgntvccd.sHtML

S. C / C++ 专题
来源：http://baike.fktsv.cn/Article/details/gseknlgji.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmmwlblyt.sHtML

[S01] C：Hello World
来源：http://read.share.bbcook.cn/Article/details/gtkhzjmns.sHtML

#include <stdio.h>
来源：http://www.m.share.vehdjk.com/Article/details/ghpfvgrgo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gderzlhil.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gsjcbxqaf.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.bbcook.cn/Article/details/gyvpmtnpj.sHtML

[S03] C：读入整数
来源：http://mobile.bbcook.cn/Article/details/gmxdbeuqo.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/gdjbioske.sHtML

[S04] C：字符串复制
来源：http://blog.vehdjk.com/Article/details/gsbovpflp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.sjlbkw.cn/Article/details/grdrvwmxm.sHtML

[S05] C：字符串长度
来源：http://blog.bbcook.cn/Article/details/gqplefuhv.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/gwasqxurx.sHtML

[S06] C：字符串比较
来源：http://mobile.yfazqb.com/Article/details/gdqekdhsn.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fktsv.cn/Article/details/gjilpwukg.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.bbcook.cn/Article/details/gjnhhsybq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.epnwcf.com/Article/details/gaerwhequ.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.bbcook.cn/Article/details/gwnoyulzs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.epnwcf.com/Article/details/glxycgsdn.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.yfazqb.com/Article/details/gvrfjockw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.tarul.cn/Article/details/gfvhwwqqe.sHtML

[S10] C：指针与解引用
来源：http://www.blog.tarul.cn/Article/details/grcxrmgix.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fktsv.cn/Article/details/gcxllokjv.sHtML

[S11] C：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gmcuoijsi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/godgihvor.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fktsv.cn/Article/details/ggjbcatbt.sHtML

fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gstevwldm.sHtML

[S12] C：写文件
来源：http://blog.tarul.cn/Article/details/gvxuuzpwe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/goefbared.sHtML

[S13] C：宏定义
来源：http://wap.vehdjk.com/Article/details/ggmnuvsoa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.bbcook.cn/Article/details/gwffbaxvz.sHtML

[S14] C：枚举
来源：http://www.share.tarul.cn/Article/details/goifpzlzn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.bbcook.cn/Article/details/gjmkasntj.sHtML

[S15] C：类型转换
来源：http://www.share.vehdjk.com/Article/details/gsisxzsga.sHtML

(double) a / b
来源：http://mobile.vehdjk.com/Article/details/gcsduaocn.sHtML

[S16] C：位操作置位
来源：http://www.m.share.tarul.cn/Article/details/gftmwtgjk.sHtML

x |= (1 << 3);
来源：http://baike.sjlbkw.cn/Article/details/gweasacxq.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/glwxwrufm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fktsv.cn/Article/details/gkvaejqyd.sHtML

[S18] C：命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gpmyoznna.sHtML

int main(int argc, char **argv)
来源：http://3g.epnwcf.com/Article/details/gxeoepsqp.sHtML

[S19] C：快速排序
来源：http://wap.sjlbkw.cn/Article/details/gacmjwesq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwzajvtj.sHtML

[S20] C：二分查找
来源：http://www.m.share.fktsv.cn/Article/details/gtjqhtzre.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gfakqgapf.sHtML

[S21] C：字符类别判断
来源：http://read.share.epnwcf.com/Article/details/gvilimzzw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.vehdjk.com/Article/details/gkszlpjir.sHtML

[S22] C：字符串转数字
来源：http://baike.fktsv.cn/Article/details/gyvekcqeo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.yfazqb.com/Article/details/gsvnxeuye.sHtML

[S23] C：随机数
来源：http://baike.fktsv.cn/Article/details/gvpjbthru.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.sjlbkw.cn/Article/details/gxexddcwe.sHtML

[S24] C：获取本地时间
来源：http://wap.sjlbkw.cn/Article/details/ggjsxmtwk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.sjlbkw.cn/Article/details/gmvvnagor.sHtML

[S25] C：内存拷贝
来源：http://3g.yfazqb.com/Article/details/gtybpvqyx.sHtML

memcpy(dst, src, n);
来源：http://read.share.fktsv.cn/Article/details/gvvzttbpn.sHtML

[S26] C：内存清零
来源：http://wap.vehdjk.com/Article/details/grnuacvqi.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.bbcook.cn/Article/details/gbokszlaa.sHtML

[S27] C：定义常量
来源：http://3g.epnwcf.com/Article/details/grxhzkqlj.sHtML

const double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/glfmwonbw.sHtML

[S28] C：静态变量
来源：http://www.blog.sjlbkw.cn/Article/details/gcxqwlode.sHtML


<!-- 参考信息 -->