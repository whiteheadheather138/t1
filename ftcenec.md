代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/grcxnbgya.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fktsv.cn/Article/details/gosesgjua.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.sjlbkw.cn/Article/details/ganxpmeaj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.tarul.cn/Article/details/gjhxwsaxv.sHtML

[Q61] 移动平均
来源：http://www.blog.fktsv.cn/Article/details/gboqbnhso.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gymggumcn.sHtML

[Q62] 分组占比
来源：http://baike.tarul.cn/Article/details/gzflbqewx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/glavjekxl.sHtML

[Q63] 开启事务
来源：http://www.blog.sjlbkw.cn/Article/details/gerhfbdmw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpxhufwd.sHtML

[Q64] 提交事务
来源：http://read.share.fktsv.cn/Article/details/grvwcsojv.sHtML

COMMIT;
来源：http://wap.sjlbkw.cn/Article/details/gdantzzor.sHtML

[Q65] 回滚事务
来源：http://baike.fktsv.cn/Article/details/gyodpfqft.sHtML

ROLLBACK;
来源：http://www.blog.tarul.cn/Article/details/gfnedzsby.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/giefrvxza.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.yfazqb.com/Article/details/gwrpacizb.sHtML

[Q67] 设置隔离级别
来源：http://baike.yfazqb.com/Article/details/gmmophbje.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.tarul.cn/Article/details/grxcfqqpc.sHtML

[Q68] 保存点
来源：http://www.share.fktsv.cn/Article/details/gclbulfpf.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gedstvbox.sHtML

ROLLBACK TO sp1;
来源：http://blog.tarul.cn/Article/details/gelmomcyt.sHtML

[Q69] 查看执行计划
来源：http://wap.bbcook.cn/Article/details/gbyzbtxct.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fktsv.cn/Article/details/gdtjkedbc.sHtML

[Q70] 更新统计信息
来源：http://www.blog.bbcook.cn/Article/details/gdrakhyxt.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.epnwcf.com/Article/details/gcenegyvg.sHtML

[Q71] 查看建表语句
来源：http://wap.yfazqb.com/Article/details/gzacmyoeg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.epnwcf.com/Article/details/gxnbnvffx.sHtML

[Q72] 查看索引
来源：http://3g.bbcook.cn/Article/details/gdugnzirc.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fktsv.cn/Article/details/ghafvbzqr.sHtML

[Q73] 查看表状态
来源：http://www.blog.yfazqb.com/Article/details/ggmuqcnif.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fktsv.cn/Article/details/gqgmkedyb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.bbcook.cn/Article/details/gaetecpdn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjeocqhe.sHtML

[Q75] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gthlipfhm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.vehdjk.com/Article/details/gijvfauug.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.sjlbkw.cn/Article/details/gawjwuokd.sHtML

[Q76] 按天统计
来源：http://wap.fktsv.cn/Article/details/gsvgiuymd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.vehdjk.com/Article/details/gknkvzayv.sHtML

[Q77] 时间加减
来源：http://m.share.tarul.cn/Article/details/gktpjxcbm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.tarul.cn/Article/details/gbbdqsosw.sHtML

[Q78] 当前时间
来源：http://www.share.epnwcf.com/Article/details/gbelmbmva.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.tarul.cn/Article/details/gdoxqerst.sHtML

[Q79] 字符串拼接
来源：http://blog.yfazqb.com/Article/details/gidmyxrrh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.tarul.cn/Article/details/gkwwqtklw.sHtML

[Q80] 字符串截取
来源：http://3g.bbcook.cn/Article/details/gsmjaaxzh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gnfddusvp.sHtML

[Q81] 字符串替换
来源：http://blog.vehdjk.com/Article/details/gtccjheqt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/geqnxowwn.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fktsv.cn/Article/details/ghdifrhcm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gnhphsivk.sHtML

[Q83] 大小写转换
来源：http://baike.tarul.cn/Article/details/gumlsqhum.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gdfwlbegz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.epnwcf.com/Article/details/gjpufesdl.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gykzlywpo.sHtML

[Q85] 数值取整
来源：http://m.share.vehdjk.com/Article/details/gdyoprxdp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.tarul.cn/Article/details/gxrsaleie.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.epnwcf.com/Article/details/grsieijql.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.tarul.cn/Article/details/gbycuryyj.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoyzppfy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.yfazqb.com/Article/details/grqsstxvy.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/gmrxezqvu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.epnwcf.com/Article/details/ghtxppjbx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ghxjfaqly.sHtML

[Q89] 判断表是否存在
来源：http://mobile.sjlbkw.cn/Article/details/ghqamzmzq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.epnwcf.com/Article/details/gzhdrrxpp.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/gmkcduygf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.vehdjk.com/Article/details/gwdqgxuqk.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gaztuhzgt.sHtML

R. Bash 专题
来源：http://mobile.yfazqb.com/Article/details/gipzlpcxg.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvsdqpyvw.sHtML

[R01] shebang 与严格模式
来源：http://blog.vehdjk.com/Article/details/giuhoheds.sHtML

#!/usr/bin/env bash
来源：http://3g.vehdjk.com/Article/details/grerowqdj.sHtML

set -euo pipefail
来源：http://www.share.bbcook.cn/Article/details/gziyizpuy.sHtML

[R02] 变量赋值与使用
来源：http://3g.yfazqb.com/Article/details/gvaoizemf.sHtML

name="Tom"; echo "$name"
来源：http://baike.bbcook.cn/Article/details/gnsaosgcb.sHtML

[R03] 只读变量
来源：http://www.blog.sjlbkw.cn/Article/details/gfcrhqpod.sHtML

readonly PI=3.14
来源：http://www.blog.fktsv.cn/Article/details/gzoyxsrrr.sHtML

[R04] 位置参数
来源：http://www.blog.fktsv.cn/Article/details/geamkzxmq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.sjlbkw.cn/Article/details/gcolscbbk.sHtML

[R05] 参数默认值
来源：http://read.share.vehdjk.com/Article/details/gngqxesgg.sHtML

name="${1:-default}"
来源：http://baike.yfazqb.com/Article/details/gdiebyfuh.sHtML

[R06] 判断命令是否存在
来源：http://baike.vehdjk.com/Article/details/giewgrqzi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gdwxzhvee.sHtML

[R07] if 判断文件
来源：http://blog.sjlbkw.cn/Article/details/gxmazhuoy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.epnwcf.com/Article/details/gcsiithxp.sHtML

[R08] 数值比较
来源：http://read.share.tarul.cn/Article/details/gtzlvxsxe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.bbcook.cn/Article/details/gvbllcqep.sHtML

[R09] 字符串比较
来源：http://wap.fktsv.cn/Article/details/grpnrlpix.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.vehdjk.com/Article/details/girevtdda.sHtML

[R10] 正则匹配
来源：http://wap.sjlbkw.cn/Article/details/gdzbjgjwt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.vehdjk.com/Article/details/guholtezx.sHtML

[R11] case 多分支
来源：http://www.blog.sjlbkw.cn/Article/details/gmcjdazjk.sHtML

case "$1" in
来源：http://mobile.yfazqb.com/Article/details/gcqglwqpw.sHtML

start) echo "启动" ;;
来源：http://blog.vehdjk.com/Article/details/gckkggfhw.sHtML

stop)  echo "停止" ;;
来源：http://www.share.epnwcf.com/Article/details/gnsyffdhi.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fktsv.cn/Article/details/gnuazrtiv.sHtML

esac
来源：http://blog.vehdjk.com/Article/details/guakulehi.sHtML

[R12] for 遍历文件
来源：http://read.share.sjlbkw.cn/Article/details/gtyiwzwgp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.epnwcf.com/Article/details/gaypokpci.sHtML

[R13] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gqvddzgxi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gdgfpfrkz.sHtML

[R14] C 风格 for
来源：http://read.share.epnwcf.com/Article/details/gkdjcbufh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gebtiaeid.sHtML

[R15] while 逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gngmnnftd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gmfcropea.sHtML

[R16] until 等待条件
来源：http://mobile.yfazqb.com/Article/details/glsaaavfn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/gfeersxhz.sHtML

[R17] 数组定义与取值
来源：http://read.share.fktsv.cn/Article/details/gopjwodiw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.bbcook.cn/Article/details/gjqkifxcf.sHtML

[R18] 遍历数组
来源：http://3g.vehdjk.com/Article/details/gvlyvunso.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.yfazqb.com/Article/details/grkeltcqn.sHtML

[R19] 数组长度
来源：http://read.share.fktsv.cn/Article/details/grvvigano.sHtML

echo "${#arr[@]}"
来源：http://blog.yfazqb.com/Article/details/gjdazmpsr.sHtML

[R20] 关联数组（字典）
来源：http://blog.yfazqb.com/Article/details/gdltwwzmx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.bbcook.cn/Article/details/gaanbdpkq.sHtML

[R21] 字符串长度
来源：http://blog.epnwcf.com/Article/details/gtitmuity.sHtML

echo "${#s}"
来源：http://read.share.bbcook.cn/Article/details/gyuepqzuc.sHtML

[R22] 截取子串
来源：http://mobile.fktsv.cn/Article/details/gncpjklci.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/gpzovxojg.sHtML

[R23] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gdfkevzap.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.tarul.cn/Article/details/gkuqqfhhn.sHtML

[R24] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/ggzupiupn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.sjlbkw.cn/Article/details/getxecbfa.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.epnwcf.com/Article/details/gzuoscmpc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/gkpdkcppu.sHtML

[R26] 命令替换
来源：http://www.m.share.tarul.cn/Article/details/gqmswwgvk.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.vehdjk.com/Article/details/ggdvdvlvj.sHtML

[R27] 算术展开
来源：http://www.blog.vehdjk.com/Article/details/gxriwmgfs.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fktsv.cn/Article/details/glptjhomo.sHtML

[R28] 浮点运算
来源：http://mobile.sjlbkw.cn/Article/details/gorjhkiid.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.bbcook.cn/Article/details/geohunuey.sHtML

[R29] 定义函数
来源：http://wap.fktsv.cn/Article/details/gnmklmrks.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.bbcook.cn/Article/details/guxrglama.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.vehdjk.com/Article/details/gczoxqhtq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.yfazqb.com/Article/details/gcjojgilr.sHtML

[R31] 局部变量
来源：http://3g.fktsv.cn/Article/details/gebzpnebl.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/gkoxphkqt.sHtML

[R32] 参数个数校验
来源：http://www.share.sjlbkw.cn/Article/details/gotdmcehz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/ggcplqopy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.sjlbkw.cn/Article/details/ggjgreptr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.vehdjk.com/Article/details/gvqfqciat.sHtML

[R34] 退出时清理
来源：http://www.m.share.epnwcf.com/Article/details/gqkztpwul.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/glgrcivdk.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/gozmusdaf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/gbmtijrnt.sHtML

[R36] 并发执行多个任务
来源：http://wap.yfazqb.com/Article/details/gpymlozhq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.epnwcf.com/Article/details/ghgxcoseg.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fktsv.cn/Article/details/gqftrgxaj.sHtML

files=$(ls -1)
来源：http://www.share.bbcook.cn/Article/details/gaxxiriin.sHtML

[R38] 管道串联
来源：http://www.m.share.vehdjk.com/Article/details/gvyfdacib.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.tarul.cn/Article/details/gsmrwwene.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.sjlbkw.cn/Article/details/ghhwnoefh.sHtML

cmd > out.log 2>&1
来源：http://wap.tarul.cn/Article/details/gwbxxtzuh.sHtML

[R40] 追加写日志
来源：http://read.share.vehdjk.com/Article/details/gnvzyztis.sHtML

echo "log" >> out.log
来源：http://mobile.sjlbkw.cn/Article/details/gktrijdda.sHtML

[R41] 丢弃输出
来源：http://wap.tarul.cn/Article/details/gjhggqngx.sHtML

cmd >/dev/null 2>&1
来源：http://wap.bbcook.cn/Article/details/grkaptwht.sHtML

[R42] 输入重定向
来源：http://blog.epnwcf.com/Article/details/gwmppogto.sHtML

wc -l < a.txt
来源：http://3g.bbcook.cn/Article/details/gthtvdezj.sHtML

[R43] 按名字查找文件
来源：http://3g.epnwcf.com/Article/details/gdxnwepvu.sHtML

find . -name "*.log" -type f
来源：http://blog.fktsv.cn/Article/details/gibsxbqmh.sHtML

[R44] 按修改时间查找
来源：http://baike.vehdjk.com/Article/details/gelsvvowz.sHtML

find . -mtime -7 -type f
来源：http://wap.vehdjk.com/Article/details/gfgwscdpm.sHtML

[R45] 批量删除
来源：http://m.share.sjlbkw.cn/Article/details/gzzhsrydc.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.yfazqb.com/Article/details/grautaiag.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fktsv.cn/Article/details/gxxlcqvhd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fktsv.cn/Article/details/gbjpzmlqw.sHtML

[R47] sed 单行替换
来源：http://baike.epnwcf.com/Article/details/gbgqatnpg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gxkyaorkt.sHtML

[R48] awk 取指定列
来源：http://mobile.tarul.cn/Article/details/gizhplidi.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.epnwcf.com/Article/details/ghykfelrh.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/gfjwuhnsb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.yfazqb.com/Article/details/gftvjnrqw.sHtML

[R50] awk 求和
来源：http://blog.yfazqb.com/Article/details/gwxprwemq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.tarul.cn/Article/details/gfgvijzro.sHtML

[R51] 排序去重取前几
来源：http://www.share.yfazqb.com/Article/details/gazkejltt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fktsv.cn/Article/details/goadlvuwv.sHtML

[R52] 统计行数
来源：http://read.share.yfazqb.com/Article/details/gpngifqjk.sHtML

wc -l a.txt
来源：http://read.share.vehdjk.com/Article/details/gzqcwqjck.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.sjlbkw.cn/Article/details/gstphstzj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.bbcook.cn/Article/details/gejvplhqg.sHtML

[R54] 比较两个文件
来源：http://blog.bbcook.cn/Article/details/gufknceaf.sHtML

diff a.txt b.txt
来源：http://www.m.share.fktsv.cn/Article/details/gfgmokuex.sHtML

[R55] 压缩与解压
来源：http://www.blog.tarul.cn/Article/details/gbnwloclo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.vehdjk.com/Article/details/gtocehrzp.sHtML

[R56] 远程拷贝
来源：http://read.share.yfazqb.com/Article/details/gvnenvygl.sHtML

scp file user@host:/path/
来源：http://www.share.yfazqb.com/Article/details/gtnewippn.sHtML

[R57] 远程执行命令
来源：http://www.share.vehdjk.com/Article/details/gonebokfc.sHtML

ssh user@host 'uptime'
来源：http://blog.bbcook.cn/Article/details/gfodckwof.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/glefvbpup.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.bbcook.cn/Article/details/gjiitvbov.sHtML

[R59] 发 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/gzfnoaayy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.sjlbkw.cn/Article/details/gcclpfgpq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gxbrbzymz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fktsv.cn/Article/details/gxowhsthz.sHtML

[R61] 磁盘占用
来源：http://3g.fktsv.cn/Article/details/gdxnglwpn.sHtML

df -h;  du -sh *
来源：http://3g.bbcook.cn/Article/details/gbfwkuoea.sHtML

[R62] 找最占空间的文件
来源：http://read.share.tarul.cn/Article/details/gjpvgbikm.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fktsv.cn/Article/details/gntrwglzn.sHtML

[R63] 内存与进程
来源：http://www.share.vehdjk.com/Article/details/gtcexqgao.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.tarul.cn/Article/details/gquraknlw.sHtML

[R64] 结束进程
来源：http://read.share.fktsv.cn/Article/details/gnmicfkkc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/gdolfpoei.sHtML

[R65] 查看端口占用
来源：http://blog.vehdjk.com/Article/details/gnffxfpgv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.epnwcf.com/Article/details/gmzgkvesf.sHtML

[R66] 定时任务
来源：http://read.share.bbcook.cn/Article/details/gfonkpbzx.sHtML

crontab -e;  crontab -l
来源：http://www.blog.vehdjk.com/Article/details/gjuzxjhzn.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.vehdjk.com/Article/details/gbmtdnakq.sHtML

openssl rand -hex 16
来源：http://www.m.share.yfazqb.com/Article/details/gpsoapqdw.sHtML

[R68] 计算文件校验值
来源：http://3g.bbcook.cn/Article/details/gtuaxmtgl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.vehdjk.com/Article/details/gxwlhwibb.sHtML

[R69] 生成随机密码
来源：http://baike.fktsv.cn/Article/details/gyfdylsfp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.bbcook.cn/Article/details/gimljyeti.sHtML

[R70] 时间戳与互转
来源：http://mobile.sjlbkw.cn/Article/details/gewagsqmd.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.sjlbkw.cn/Article/details/giaxmqupc.sHtML

[R71] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gpgcctgxy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.vehdjk.com/Article/details/gmuuxxmlh.sHtML

[R72] 等待端口就绪
来源：http://blog.bbcook.cn/Article/details/gwctnqedq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/gnnbvimnl.sHtML

[R73] 分割大日志
来源：http://blog.fktsv.cn/Article/details/goqkhgzhq.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gaywxidov.sHtML

[R74] 批量重命名
来源：http://baike.sjlbkw.cn/Article/details/gmccagtvd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.epnwcf.com/Article/details/gspqngeia.sHtML

[R75] 导出环境变量
来源：http://wap.epnwcf.com/Article/details/gkewfxrov.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.bbcook.cn/Article/details/gitdllfxx.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/gvcmvphie.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gixdwyxmj.sHtML

[R77] 读取用户输入
来源：http://m.share.sjlbkw.cn/Article/details/gqihhfege.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.tarul.cn/Article/details/gjtiulpbr.sHtML

[R78] 交互式菜单
来源：http://read.share.bbcook.cn/Article/details/gaalcfshc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/ggfsjcnbu.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.bbcook.cn/Article/details/gwsuaarud.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/gclmwgwqs.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.vehdjk.com/Article/details/gqnncbfxf.sHtML

time ./run.sh
来源：http://blog.bbcook.cn/Article/details/gqrajnzcu.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gzquaooiy.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gnavttklv.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gpjtzxbim.sHtML

[S01] C：Hello World
来源：http://baike.fktsv.cn/Article/details/giqjsbdzk.sHtML

#include <stdio.h>
来源：http://mobile.epnwcf.com/Article/details/gepgilkny.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.bbcook.cn/Article/details/gjzlcquhf.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.tarul.cn/Article/details/gypotexql.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.yfazqb.com/Article/details/gpexucseh.sHtML

[S03] C：读入整数
来源：http://read.share.tarul.cn/Article/details/gvpuzwifz.sHtML

int x; scanf("%d", &x);
来源：http://read.share.tarul.cn/Article/details/gsobpyoyg.sHtML

[S04] C：字符串复制
来源：http://read.share.bbcook.cn/Article/details/gfnpqhmsh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.bbcook.cn/Article/details/gwpjwbxya.sHtML

[S05] C：字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gqkqwxpjr.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/grksvcslv.sHtML

[S06] C：字符串比较
来源：http://mobile.vehdjk.com/Article/details/glknapskk.sHtML

strcmp(a, b) == 0
来源：http://baike.tarul.cn/Article/details/gstevwaru.sHtML

[S07] C：数组遍历求和
来源：http://wap.sjlbkw.cn/Article/details/gnioejcqf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.bbcook.cn/Article/details/gnbbdgwot.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.sjlbkw.cn/Article/details/gehxxhwll.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.tarul.cn/Article/details/gwawlxytv.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.bbcook.cn/Article/details/gdafswzwg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.bbcook.cn/Article/details/gbdyumbrb.sHtML

[S10] C：指针与解引用
来源：http://read.share.sjlbkw.cn/Article/details/gybwokzrr.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fktsv.cn/Article/details/gigvgavzi.sHtML

[S11] C：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gfhdaqkdi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.bbcook.cn/Article/details/gjihtujrf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.epnwcf.com/Article/details/gpxeyupah.sHtML

fclose(f);
来源：http://baike.fktsv.cn/Article/details/gacgwrwsi.sHtML

[S12] C：写文件
来源：http://www.blog.fktsv.cn/Article/details/gtvyqjsyc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gbqhwgrsj.sHtML

[S13] C：宏定义
来源：http://baike.sjlbkw.cn/Article/details/gsrhyeebg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.yfazqb.com/Article/details/giliacprl.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/gwvyvrpzr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fktsv.cn/Article/details/gzgsvalxi.sHtML

[S15] C：类型转换
来源：http://3g.bbcook.cn/Article/details/gxgimssdf.sHtML

(double) a / b
来源：http://wap.tarul.cn/Article/details/giebshdhe.sHtML

[S16] C：位操作置位
来源：http://www.m.share.vehdjk.com/Article/details/gnpegqish.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/gyqgnyqpj.sHtML

[S17] C：安全拼接字符串
来源：http://3g.epnwcf.com/Article/details/gjvtnhzcg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.epnwcf.com/Article/details/gnttbpoej.sHtML

[S18] C：命令行参数
来源：http://wap.yfazqb.com/Article/details/grmckenta.sHtML

int main(int argc, char **argv)
来源：http://mobile.epnwcf.com/Article/details/ggaptqqyi.sHtML

[S19] C：快速排序
来源：http://www.share.vehdjk.com/Article/details/glehboxrs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gucnmxxjd.sHtML

[S20] C：二分查找
来源：http://www.m.share.bbcook.cn/Article/details/gyqfwkifa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/gfsaadkiv.sHtML

[S21] C：字符类别判断
来源：http://www.share.vehdjk.com/Article/details/gnbjbyqjs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.yfazqb.com/Article/details/gwofupnnt.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/gklgvuukb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fktsv.cn/Article/details/gbmnetudw.sHtML

[S23] C：随机数
来源：http://blog.bbcook.cn/Article/details/grtgtbpdw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.sjlbkw.cn/Article/details/goiwsyhhx.sHtML

[S24] C：获取本地时间
来源：http://wap.sjlbkw.cn/Article/details/gyolsqalk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.epnwcf.com/Article/details/gqthggala.sHtML

[S25] C：内存拷贝
来源：http://m.share.fktsv.cn/Article/details/gaxwfzkcr.sHtML

memcpy(dst, src, n);
来源：http://www.share.bbcook.cn/Article/details/gvsqsrkao.sHtML

[S26] C：内存清零
来源：http://www.m.share.tarul.cn/Article/details/gbpdqdycj.sHtML

memset(a, 0, sizeof a);
来源：http://blog.bbcook.cn/Article/details/gmtvfamaj.sHtML

[S27] C：定义常量
来源：http://www.blog.epnwcf.com/Article/details/gdlldwqtq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gsyftxjen.sHtML

[S28] C：静态变量
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqsizgni.sHtML

static int counter = 0;
来源：http://www.blog.vehdjk.com/Article/details/gctvykptl.sHtML

[S29] C：变参函数
来源：http://www.m.share.bbcook.cn/Article/details/gxttnsyxs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/ggwyytavs.sHtML

[S30] C：头文件保护
来源：http://blog.bbcook.cn/Article/details/ghdmakjrn.sHtML


<!-- 参考信息 -->