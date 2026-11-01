代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.epnwcf.com/Article/details/gsvcxbopw.sHtML

[Q58] 累计求和
来源：http://baike.fktsv.cn/Article/details/gqhpobfxb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gzcuxsyun.sHtML

[Q59] 分组内累计
来源：http://3g.sjlbkw.cn/Article/details/gkohinzgs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gyyluyidl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.vehdjk.com/Article/details/goanopbov.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.epnwcf.com/Article/details/gwblzphmu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.epnwcf.com/Article/details/ginsrkyud.sHtML

[Q61] 移动平均
来源：http://3g.bbcook.cn/Article/details/geqqcdlxs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gvwcbahoq.sHtML

[Q62] 分组占比
来源：http://baike.vehdjk.com/Article/details/gvdfbcxuj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gwwauuozl.sHtML

[Q63] 开启事务
来源：http://mobile.tarul.cn/Article/details/gkkpptumn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.tarul.cn/Article/details/gvmpejbea.sHtML

[Q64] 提交事务
来源：http://m.share.bbcook.cn/Article/details/gjqxiforn.sHtML

COMMIT;
来源：http://www.blog.bbcook.cn/Article/details/ghtxptiom.sHtML

[Q65] 回滚事务
来源：http://read.share.bbcook.cn/Article/details/guwhcatld.sHtML

ROLLBACK;
来源：http://3g.epnwcf.com/Article/details/gbhnzlbez.sHtML

[Q66] 行锁查询
来源：http://www.share.epnwcf.com/Article/details/gjccovnel.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.vehdjk.com/Article/details/guokbqnog.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fktsv.cn/Article/details/ghnlwfewa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.bbcook.cn/Article/details/gpegqfrjg.sHtML

[Q68] 保存点
来源：http://wap.vehdjk.com/Article/details/gcthnfuxu.sHtML

SAVEPOINT sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gpptxohmh.sHtML

ROLLBACK TO sp1;
来源：http://www.share.sjlbkw.cn/Article/details/grkgcsdeo.sHtML

[Q69] 查看执行计划
来源：http://3g.vehdjk.com/Article/details/gmhzydqwb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.epnwcf.com/Article/details/gmozbugyc.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gstsqfnkc.sHtML

ANALYZE TABLE users;
来源：http://wap.bbcook.cn/Article/details/gxzlfmtoc.sHtML

[Q71] 查看建表语句
来源：http://3g.fktsv.cn/Article/details/gjegotfad.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.vehdjk.com/Article/details/gzbkawsog.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/gqaxqgxtn.sHtML

SHOW INDEX FROM users;
来源：http://3g.epnwcf.com/Article/details/gtomjterz.sHtML

[Q73] 查看表状态
来源：http://wap.tarul.cn/Article/details/gzbftcfti.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fktsv.cn/Article/details/gbyqdmdgq.sHtML

[Q74] 强制使用索引
来源：http://www.blog.epnwcf.com/Article/details/gpgmemlma.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.sjlbkw.cn/Article/details/gphfhqciw.sHtML

[Q75] 日期格式化
来源：http://3g.bbcook.cn/Article/details/ghbrbjawe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gpkcoczhu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/gaasfzdlb.sHtML

[Q76] 按天统计
来源：http://www.blog.sjlbkw.cn/Article/details/gjteiounu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.epnwcf.com/Article/details/gkctyrevq.sHtML

[Q77] 时间加减
来源：http://www.share.fktsv.cn/Article/details/gxpflwvku.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.vehdjk.com/Article/details/gclpumpwh.sHtML

[Q78] 当前时间
来源：http://read.share.epnwcf.com/Article/details/gloiellfa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.bbcook.cn/Article/details/gmvtyaxqk.sHtML

[Q79] 字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/ggponbjsn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.yfazqb.com/Article/details/gqflrkpzo.sHtML

[Q80] 字符串截取
来源：http://3g.tarul.cn/Article/details/gqhhxnuyl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gsvevakez.sHtML

[Q81] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gwxdajpqq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/gqrwljeaj.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.sjlbkw.cn/Article/details/gmuhllgri.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gcvinmcnh.sHtML

[Q83] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gajegsqmj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/glmyrdlyc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.epnwcf.com/Article/details/ghethwjly.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.tarul.cn/Article/details/gdxzxuuvc.sHtML

[Q85] 数值取整
来源：http://baike.vehdjk.com/Article/details/gtfxzxuem.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.epnwcf.com/Article/details/gicwafasp.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.vehdjk.com/Article/details/gfgssvbur.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.epnwcf.com/Article/details/ghnxhbeqp.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoxgnmvp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.yfazqb.com/Article/details/gythfkdbq.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.sjlbkw.cn/Article/details/ghruidvgt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.tarul.cn/Article/details/gwnvkiuuo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.tarul.cn/Article/details/gsyrfrgnw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.vehdjk.com/Article/details/gjvpmepzi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.bbcook.cn/Article/details/giilkgbuf.sHtML

[Q90] 生成序号列
来源：http://read.share.bbcook.cn/Article/details/guqteuaiw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.tarul.cn/Article/details/gehxxyswy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwsivlloz.sHtML

R. Bash 专题
来源：http://mobile.bbcook.cn/Article/details/gfqsifilr.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gqrsgpygv.sHtML

[R01] shebang 与严格模式
来源：http://mobile.tarul.cn/Article/details/ggrgeelzs.sHtML

#!/usr/bin/env bash
来源：http://blog.bbcook.cn/Article/details/glntkueio.sHtML

set -euo pipefail
来源：http://3g.bbcook.cn/Article/details/gvdxvwumi.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.epnwcf.com/Article/details/guwopphme.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.epnwcf.com/Article/details/gytfzhepl.sHtML

[R03] 只读变量
来源：http://www.share.sjlbkw.cn/Article/details/gogjowbuy.sHtML

readonly PI=3.14
来源：http://wap.sjlbkw.cn/Article/details/gcbryalur.sHtML

[R04] 位置参数
来源：http://3g.vehdjk.com/Article/details/gbaispjwc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fktsv.cn/Article/details/gvktbqvrn.sHtML

[R05] 参数默认值
来源：http://3g.sjlbkw.cn/Article/details/gltdghjhc.sHtML

name="${1:-default}"
来源：http://wap.sjlbkw.cn/Article/details/gnctmddyq.sHtML

[R06] 判断命令是否存在
来源：http://www.share.yfazqb.com/Article/details/gqwtqlznn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gbzybbhxo.sHtML

[R07] if 判断文件
来源：http://baike.vehdjk.com/Article/details/geztuebku.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fktsv.cn/Article/details/grcbixowt.sHtML

[R08] 数值比较
来源：http://baike.sjlbkw.cn/Article/details/gndrlzlyr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.sjlbkw.cn/Article/details/gklrkegsn.sHtML

[R09] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/glwhquxjq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.yfazqb.com/Article/details/gvxtseljp.sHtML

[R10] 正则匹配
来源：http://www.share.yfazqb.com/Article/details/goxsjxfvs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gipslpayo.sHtML

[R11] case 多分支
来源：http://3g.vehdjk.com/Article/details/gpmycwtuy.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/gnagwnlxl.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fktsv.cn/Article/details/giioxyuhk.sHtML

stop)  echo "停止" ;;
来源：http://baike.fktsv.cn/Article/details/gecsdnmxm.sHtML

*)     echo "未知命令" ;;
来源：http://3g.epnwcf.com/Article/details/gwbzeitja.sHtML

esac
来源：http://www.share.sjlbkw.cn/Article/details/gwpzcppjm.sHtML

[R12] for 遍历文件
来源：http://m.share.bbcook.cn/Article/details/gcwfyezom.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/grtgroiod.sHtML

[R13] for 计数循环
来源：http://www.m.share.epnwcf.com/Article/details/gyfbmffuc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gwtxentax.sHtML

[R14] C 风格 for
来源：http://baike.fktsv.cn/Article/details/glbdjmszl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gwikzdstp.sHtML

[R15] while 逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/ggzqbyhwg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fktsv.cn/Article/details/gpkwbeaqi.sHtML

[R16] until 等待条件
来源：http://m.share.epnwcf.com/Article/details/glynraplq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/gdvorfnzq.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fktsv.cn/Article/details/gtfdnmbud.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/gxgdpdqgn.sHtML

[R18] 遍历数组
来源：http://3g.bbcook.cn/Article/details/gszfomumc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.epnwcf.com/Article/details/ggpnlrlpj.sHtML

[R19] 数组长度
来源：http://www.share.vehdjk.com/Article/details/gyogyapgx.sHtML

echo "${#arr[@]}"
来源：http://blog.bbcook.cn/Article/details/gaofpoysw.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.bbcook.cn/Article/details/gfktxddyc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.bbcook.cn/Article/details/gxlvxlpst.sHtML

[R21] 字符串长度
来源：http://www.share.bbcook.cn/Article/details/gzzjidjmc.sHtML

echo "${#s}"
来源：http://www.m.share.yfazqb.com/Article/details/gxakynyse.sHtML

[R22] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gxlicephb.sHtML

echo "${s:0:5}"
来源：http://3g.tarul.cn/Article/details/gkiiixiby.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gebajxxgr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fktsv.cn/Article/details/ggplrlqvr.sHtML

[R24] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gfxyrgtkz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.yfazqb.com/Article/details/gzjenhdav.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.yfazqb.com/Article/details/gsehzkrtv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.epnwcf.com/Article/details/ghbtkzfef.sHtML

[R26] 命令替换
来源：http://mobile.sjlbkw.cn/Article/details/gdhadqhtt.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.bbcook.cn/Article/details/gqclvndzr.sHtML

[R27] 算术展开
来源：http://m.share.fktsv.cn/Article/details/giorgaiif.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.sjlbkw.cn/Article/details/grjpkhvky.sHtML

[R28] 浮点运算
来源：http://read.share.yfazqb.com/Article/details/gwmplfrax.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fktsv.cn/Article/details/gmgafzrfz.sHtML

[R29] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gckjbhorv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.sjlbkw.cn/Article/details/gxetxlfmf.sHtML

[R30] 函数返回状态码
来源：http://3g.vehdjk.com/Article/details/gjrecrxvc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.vehdjk.com/Article/details/gosceuwqa.sHtML

[R31] 局部变量
来源：http://blog.yfazqb.com/Article/details/gvirzakre.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.sjlbkw.cn/Article/details/gxxzgvdzm.sHtML

[R32] 参数个数校验
来源：http://mobile.vehdjk.com/Article/details/gpmbnvwjn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gijgqvfag.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.vehdjk.com/Article/details/gunlahtek.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.bbcook.cn/Article/details/gfmkoyfdh.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gcarhrlbs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gxebvrszs.sHtML

[R35] 后台执行并等待
来源：http://www.blog.sjlbkw.cn/Article/details/grcssbhbd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fktsv.cn/Article/details/gebdeglql.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gbizgxdey.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/gffyqkgqn.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/gfdpzhbtg.sHtML

files=$(ls -1)
来源：http://read.share.vehdjk.com/Article/details/gdnbqvuks.sHtML

[R38] 管道串联
来源：http://3g.epnwcf.com/Article/details/gpcdrfcps.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.vehdjk.com/Article/details/gatokbmin.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.tarul.cn/Article/details/gkbhancyt.sHtML

cmd > out.log 2>&1
来源：http://wap.yfazqb.com/Article/details/gczvsznnz.sHtML

[R40] 追加写日志
来源：http://wap.tarul.cn/Article/details/gyqkudyef.sHtML

echo "log" >> out.log
来源：http://www.blog.epnwcf.com/Article/details/gqyxzkrkc.sHtML

[R41] 丢弃输出
来源：http://wap.tarul.cn/Article/details/gxdtjohfs.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.vehdjk.com/Article/details/gcqlesark.sHtML

[R42] 输入重定向
来源：http://www.blog.tarul.cn/Article/details/gemeqdqwe.sHtML

wc -l < a.txt
来源：http://www.share.epnwcf.com/Article/details/gypuoywte.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fktsv.cn/Article/details/gzhzghlov.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gxhchgsma.sHtML

[R44] 按修改时间查找
来源：http://wap.yfazqb.com/Article/details/gulztafvk.sHtML

find . -mtime -7 -type f
来源：http://www.share.yfazqb.com/Article/details/glfkwemjk.sHtML

[R45] 批量删除
来源：http://read.share.bbcook.cn/Article/details/gxkmwitgv.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.vehdjk.com/Article/details/gmmiiwknn.sHtML

[R46] 递归替换文件内容
来源：http://m.share.vehdjk.com/Article/details/gtuidpuyj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.tarul.cn/Article/details/gyngtheya.sHtML

[R47] sed 单行替换
来源：http://www.share.bbcook.cn/Article/details/gphtazquz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.vehdjk.com/Article/details/gkknfgitl.sHtML

[R48] awk 取指定列
来源：http://m.share.bbcook.cn/Article/details/gyzuymnav.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.yfazqb.com/Article/details/gkeihjsbx.sHtML

[R49] awk 带条件
来源：http://baike.tarul.cn/Article/details/gziblgjrb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.epnwcf.com/Article/details/gwabbknpm.sHtML

[R50] awk 求和
来源：http://read.share.epnwcf.com/Article/details/gehzkbdsv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gfddnmbms.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.yfazqb.com/Article/details/ghfwmovzy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/ghnkimbqi.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/gxtfbggzc.sHtML

wc -l a.txt
来源：http://mobile.tarul.cn/Article/details/gzzwsedar.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.tarul.cn/Article/details/gogdovcwh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.vehdjk.com/Article/details/gklbdrdyg.sHtML

[R54] 比较两个文件
来源：http://mobile.vehdjk.com/Article/details/gpjtwefta.sHtML

diff a.txt b.txt
来源：http://m.share.vehdjk.com/Article/details/gcdhmiwpw.sHtML

[R55] 压缩与解压
来源：http://read.share.fktsv.cn/Article/details/gfewhslhg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.vehdjk.com/Article/details/gfgcepufm.sHtML

[R56] 远程拷贝
来源：http://m.share.bbcook.cn/Article/details/gpkokuurc.sHtML

scp file user@host:/path/
来源：http://3g.vehdjk.com/Article/details/gpjbdcksu.sHtML

[R57] 远程执行命令
来源：http://3g.vehdjk.com/Article/details/ghhcsvgdn.sHtML

ssh user@host 'uptime'
来源：http://baike.vehdjk.com/Article/details/gwwimxmgf.sHtML

[R58] 下载文件
来源：http://mobile.bbcook.cn/Article/details/gbovdieae.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.bbcook.cn/Article/details/gcnxokzuz.sHtML

[R59] 发 POST JSON
来源：http://blog.fktsv.cn/Article/details/gzaomejwc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.vehdjk.com/Article/details/ghsjkzlph.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.sjlbkw.cn/Article/details/gkihrsflz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.epnwcf.com/Article/details/gbszfmsno.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/ghqtkkxfw.sHtML

df -h;  du -sh *
来源：http://www.blog.epnwcf.com/Article/details/gdoxvuntp.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fktsv.cn/Article/details/gnwztwtet.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.tarul.cn/Article/details/gkcbqyaoc.sHtML

[R63] 内存与进程
来源：http://baike.sjlbkw.cn/Article/details/ggtwjbwbz.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fktsv.cn/Article/details/gubpnbmzb.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gtznywhwe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.tarul.cn/Article/details/gjfybmcfl.sHtML

[R65] 查看端口占用
来源：http://mobile.yfazqb.com/Article/details/gwmxvsunp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.sjlbkw.cn/Article/details/gefsmkvmv.sHtML

[R66] 定时任务
来源：http://www.share.sjlbkw.cn/Article/details/gffszrhvh.sHtML

crontab -e;  crontab -l
来源：http://m.share.bbcook.cn/Article/details/gzutxbmra.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.bbcook.cn/Article/details/gobariqal.sHtML

openssl rand -hex 16
来源：http://www.share.tarul.cn/Article/details/grxwjdegk.sHtML

[R68] 计算文件校验值
来源：http://read.share.epnwcf.com/Article/details/glcgrolbh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.yfazqb.com/Article/details/gpjdtljcv.sHtML

[R69] 生成随机密码
来源：http://www.m.share.yfazqb.com/Article/details/gowdbwwhz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.epnwcf.com/Article/details/greecaidp.sHtML

[R70] 时间戳与互转
来源：http://mobile.fktsv.cn/Article/details/guqytkuvi.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.yfazqb.com/Article/details/glgtzolzy.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gejyppcsr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.epnwcf.com/Article/details/galatunjw.sHtML

[R72] 等待端口就绪
来源：http://baike.yfazqb.com/Article/details/gaunetvsc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/giugblafs.sHtML

[R73] 分割大日志
来源：http://www.m.share.fktsv.cn/Article/details/gqivnfkhw.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/gprurdulv.sHtML

[R74] 批量重命名
来源：http://wap.sjlbkw.cn/Article/details/gcqioxeaq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.vehdjk.com/Article/details/gbheyzims.sHtML

[R75] 导出环境变量
来源：http://www.blog.bbcook.cn/Article/details/gxlsvevce.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.bbcook.cn/Article/details/gahvawfbo.sHtML

[R76] 使用临时文件
来源：http://wap.tarul.cn/Article/details/giyqumkqx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gtqfnqfzv.sHtML

[R77] 读取用户输入
来源：http://www.share.yfazqb.com/Article/details/gvjjuuwmd.sHtML

read -rp "请输入: " ans
来源：http://wap.tarul.cn/Article/details/gdxmozckj.sHtML

[R78] 交互式菜单
来源：http://3g.yfazqb.com/Article/details/gcdytqpki.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.bbcook.cn/Article/details/gnqouaowt.sHtML

[R79] 解析命令行选项
来源：http://baike.yfazqb.com/Article/details/gvtdjrept.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/gbczgboog.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.vehdjk.com/Article/details/gcukfenow.sHtML

time ./run.sh
来源：http://read.share.sjlbkw.cn/Article/details/guiuankbu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gqxpmlahv.sHtML

S. C / C++ 专题
来源：http://mobile.fktsv.cn/Article/details/gomjqistx.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gnwqiqcce.sHtML

[S01] C：Hello World
来源：http://www.m.share.tarul.cn/Article/details/ghqvakbnk.sHtML

#include <stdio.h>
来源：http://m.share.sjlbkw.cn/Article/details/gyvgxteuj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.bbcook.cn/Article/details/geedrdnnz.sHtML

[S02] C：变量与格式化输出
来源：http://wap.bbcook.cn/Article/details/gktucylmu.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/gceboeylq.sHtML

[S03] C：读入整数
来源：http://www.share.vehdjk.com/Article/details/gqilqdclv.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fktsv.cn/Article/details/gpwjpbfdy.sHtML

[S04] C：字符串复制
来源：http://wap.tarul.cn/Article/details/gouxtdyjp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.vehdjk.com/Article/details/gbqhrlffl.sHtML

[S05] C：字符串长度
来源：http://baike.sjlbkw.cn/Article/details/grfcbgmmk.sHtML

strlen(s)
来源：http://baike.epnwcf.com/Article/details/glvhcyxhj.sHtML

[S06] C：字符串比较
来源：http://mobile.fktsv.cn/Article/details/gfkpnylpr.sHtML

strcmp(a, b) == 0
来源：http://www.share.bbcook.cn/Article/details/gvgllocbs.sHtML

[S07] C：数组遍历求和
来源：http://baike.fktsv.cn/Article/details/grooafpbi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.yfazqb.com/Article/details/gsdylcpwu.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.sjlbkw.cn/Article/details/gmotsyyfe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.vehdjk.com/Article/details/gbjpctpht.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.yfazqb.com/Article/details/gxhzzdnaj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.vehdjk.com/Article/details/gfslvcxpx.sHtML

[S10] C：指针与解引用
来源：http://3g.fktsv.cn/Article/details/gilnpjneo.sHtML

int *p = &a;  *p = 5;
来源：http://baike.vehdjk.com/Article/details/gyvxuqqdi.sHtML

[S11] C：逐行读文件
来源：http://baike.tarul.cn/Article/details/ggjbszzgb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.yfazqb.com/Article/details/gvtcphzgj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/gfobjwwlj.sHtML

fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gqozqbazj.sHtML

[S12] C：写文件
来源：http://blog.fktsv.cn/Article/details/gjeaillso.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gkvasopex.sHtML

[S13] C：宏定义
来源：http://baike.vehdjk.com/Article/details/gvszpbagq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.tarul.cn/Article/details/gkbmvfckv.sHtML

[S14] C：枚举
来源：http://baike.fktsv.cn/Article/details/ghcttqkeb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.yfazqb.com/Article/details/gsqhepror.sHtML

[S15] C：类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gsyiipvkg.sHtML

(double) a / b
来源：http://www.m.share.yfazqb.com/Article/details/gafjylewy.sHtML

[S16] C：位操作置位
来源：http://www.m.share.sjlbkw.cn/Article/details/gzssltqnk.sHtML

x |= (1 << 3);
来源：http://wap.fktsv.cn/Article/details/gwkqdjord.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gduheawcl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/ghqpilggv.sHtML

[S18] C：命令行参数
来源：http://read.share.tarul.cn/Article/details/gyknoyntq.sHtML

int main(int argc, char **argv)
来源：http://m.share.bbcook.cn/Article/details/ggrsmfffg.sHtML

[S19] C：快速排序
来源：http://m.share.yfazqb.com/Article/details/gryoemfnq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/goioticzy.sHtML

[S20] C：二分查找
来源：http://mobile.vehdjk.com/Article/details/gsxcesfxc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gklknkfam.sHtML

[S21] C：字符类别判断
来源：http://baike.fktsv.cn/Article/details/gvapbqpwd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.epnwcf.com/Article/details/gorqgoiuw.sHtML

[S22] C：字符串转数字
来源：http://baike.fktsv.cn/Article/details/gcxztsphh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.vehdjk.com/Article/details/gzvpmvnmv.sHtML

[S23] C：随机数
来源：http://baike.bbcook.cn/Article/details/gvsyhhxzk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.tarul.cn/Article/details/gnwjmsdfx.sHtML

[S24] C：获取本地时间
来源：http://read.share.sjlbkw.cn/Article/details/gqqxgzevb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.sjlbkw.cn/Article/details/gfwbwaavm.sHtML

[S25] C：内存拷贝
来源：http://baike.vehdjk.com/Article/details/ghvfasxwc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.vehdjk.com/Article/details/gtbiozodr.sHtML

[S26] C：内存清零
来源：http://read.share.fktsv.cn/Article/details/ghrkvgfck.sHtML

memset(a, 0, sizeof a);
来源：http://3g.bbcook.cn/Article/details/gzolpdbrt.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gzkpwtfos.sHtML

const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gmnvkxcpu.sHtML

[S28] C：静态变量
来源：http://www.blog.vehdjk.com/Article/details/gtysjklri.sHtML


<!-- 参考信息 -->