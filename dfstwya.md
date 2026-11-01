代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gvpbgsjam.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.tarul.cn/Article/details/gbqtymjve.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.yfazqb.com/Article/details/gqpfqcdpn.sHtML

[Q57] 行号
来源：http://www.share.tarul.cn/Article/details/gwbmszikn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.bbcook.cn/Article/details/gsekkgrlp.sHtML

[Q58] 累计求和
来源：http://www.share.yfazqb.com/Article/details/gojybdazi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gqxatfquy.sHtML

[Q59] 分组内累计
来源：http://mobile.tarul.cn/Article/details/gecaayxie.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gvixlqhpx.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.tarul.cn/Article/details/gngtwtkqf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/grixbgyod.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gugwolqyi.sHtML

[Q61] 移动平均
来源：http://blog.epnwcf.com/Article/details/gierfgcye.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/ggcpzgraf.sHtML

[Q62] 分组占比
来源：http://m.share.tarul.cn/Article/details/ghnjaszzs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gobukopyj.sHtML

[Q63] 开启事务
来源：http://mobile.tarul.cn/Article/details/gvrbzmmbp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.tarul.cn/Article/details/gmxrxyyfx.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/grsmhdpqg.sHtML

COMMIT;
来源：http://mobile.tarul.cn/Article/details/gdgbbbglp.sHtML

[Q65] 回滚事务
来源：http://m.share.fktsv.cn/Article/details/gaczcdbpe.sHtML

ROLLBACK;
来源：http://wap.yfazqb.com/Article/details/gefwrmbkb.sHtML

[Q66] 行锁查询
来源：http://wap.vehdjk.com/Article/details/ghfighhol.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.yfazqb.com/Article/details/gwgxjlhga.sHtML

[Q67] 设置隔离级别
来源：http://mobile.yfazqb.com/Article/details/gysosqzwu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fktsv.cn/Article/details/gdmgytyuc.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/gotmcwmkp.sHtML

SAVEPOINT sp1;
来源：http://m.share.fktsv.cn/Article/details/gwdsjzxlt.sHtML

ROLLBACK TO sp1;
来源：http://blog.yfazqb.com/Article/details/gjvqwmdec.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.tarul.cn/Article/details/ghywlgvss.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.vehdjk.com/Article/details/gmzutzesc.sHtML

[Q70] 更新统计信息
来源：http://mobile.tarul.cn/Article/details/gubhdhysm.sHtML

ANALYZE TABLE users;
来源：http://wap.sjlbkw.cn/Article/details/gqdjjpsqj.sHtML

[Q71] 查看建表语句
来源：http://mobile.tarul.cn/Article/details/gykptlofv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.tarul.cn/Article/details/gfagrvzmd.sHtML

[Q72] 查看索引
来源：http://www.share.epnwcf.com/Article/details/gpokgycap.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gktmqggdh.sHtML

[Q73] 查看表状态
来源：http://m.share.sjlbkw.cn/Article/details/gjuitcrcu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.tarul.cn/Article/details/gvfwpfiuz.sHtML

[Q74] 强制使用索引
来源：http://blog.vehdjk.com/Article/details/gqkpvzepd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.sjlbkw.cn/Article/details/gsflsgpcr.sHtML

[Q75] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/glpokkydl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/genehkyyv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/guntwtoqv.sHtML

[Q76] 按天统计
来源：http://m.share.yfazqb.com/Article/details/gmaoeypjl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.sjlbkw.cn/Article/details/gxadwvdjc.sHtML

[Q77] 时间加减
来源：http://baike.epnwcf.com/Article/details/gpnktnuqy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.bbcook.cn/Article/details/guztskgdg.sHtML

[Q78] 当前时间
来源：http://www.share.bbcook.cn/Article/details/gonlfgosg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fktsv.cn/Article/details/govvihghv.sHtML

[Q79] 字符串拼接
来源：http://read.share.epnwcf.com/Article/details/grmxgpmho.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.yfazqb.com/Article/details/glnrdiyai.sHtML

[Q80] 字符串截取
来源：http://m.share.yfazqb.com/Article/details/gqqgcsjxx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.tarul.cn/Article/details/gynxndshf.sHtML

[Q81] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gneeqrpjt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fktsv.cn/Article/details/gccrysjxi.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.yfazqb.com/Article/details/gnoqljibr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gtlgbhqab.sHtML

[Q83] 大小写转换
来源：http://3g.tarul.cn/Article/details/gkrkkvllq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/grdkqqhyr.sHtML

[Q84] 去除首尾空格
来源：http://3g.bbcook.cn/Article/details/gdngilsxn.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/golpnjiwa.sHtML

[Q85] 数值取整
来源：http://mobile.epnwcf.com/Article/details/gubsiizkl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.vehdjk.com/Article/details/gmiglvndq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.vehdjk.com/Article/details/gzqaxjtox.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.yfazqb.com/Article/details/gjskqgpty.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.yfazqb.com/Article/details/gwqltpqjn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.yfazqb.com/Article/details/ghspzddtl.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.epnwcf.com/Article/details/gxigeqhmq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.sjlbkw.cn/Article/details/grrsyovjj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gammfqpmu.sHtML

[Q89] 判断表是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gohmxzjdm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.sjlbkw.cn/Article/details/gauttgilw.sHtML

[Q90] 生成序号列
来源：http://www.m.share.yfazqb.com/Article/details/gihtendiv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.vehdjk.com/Article/details/gcvkaaarp.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ghrvynkhf.sHtML

R. Bash 专题
来源：http://read.share.vehdjk.com/Article/details/ghgxpfgyh.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvgjoxquk.sHtML

[R01] shebang 与严格模式
来源：http://www.share.epnwcf.com/Article/details/gqnldfrgz.sHtML

#!/usr/bin/env bash
来源：http://wap.epnwcf.com/Article/details/gymfisbql.sHtML

set -euo pipefail
来源：http://m.share.epnwcf.com/Article/details/gxvqcdrdn.sHtML

[R02] 变量赋值与使用
来源：http://read.share.yfazqb.com/Article/details/ghsgvrbac.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/gzpdcuric.sHtML

[R03] 只读变量
来源：http://m.share.sjlbkw.cn/Article/details/gkzchvlyi.sHtML

readonly PI=3.14
来源：http://mobile.yfazqb.com/Article/details/ghrhzpxnl.sHtML

[R04] 位置参数
来源：http://baike.sjlbkw.cn/Article/details/gavkchzbd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.tarul.cn/Article/details/gacfwlmpk.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gmocyojis.sHtML

name="${1:-default}"
来源：http://blog.tarul.cn/Article/details/ghzbvcbef.sHtML

[R06] 判断命令是否存在
来源：http://baike.vehdjk.com/Article/details/gpohztozz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fktsv.cn/Article/details/gxceojuso.sHtML

[R07] if 判断文件
来源：http://3g.vehdjk.com/Article/details/gfypwvtpu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.epnwcf.com/Article/details/gdgirqnky.sHtML

[R08] 数值比较
来源：http://m.share.bbcook.cn/Article/details/gweqdjhvt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.vehdjk.com/Article/details/gzzjocfwq.sHtML

[R09] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/glgjojsrw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/gamkrqjpj.sHtML

[R10] 正则匹配
来源：http://www.share.bbcook.cn/Article/details/geupdvzeq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fktsv.cn/Article/details/galnzwutj.sHtML

[R11] case 多分支
来源：http://www.m.share.tarul.cn/Article/details/geyxenyvr.sHtML

case "$1" in
来源：http://www.share.bbcook.cn/Article/details/geecystja.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/gbjbgcmqd.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.yfazqb.com/Article/details/guxckttuo.sHtML

*)     echo "未知命令" ;;
来源：http://wap.epnwcf.com/Article/details/gqsuxwtky.sHtML

esac
来源：http://www.blog.sjlbkw.cn/Article/details/gabgczbzo.sHtML

[R12] for 遍历文件
来源：http://m.share.fktsv.cn/Article/details/gdslcaovz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/grtkbfrjb.sHtML

[R13] for 计数循环
来源：http://read.share.bbcook.cn/Article/details/gxfebmrdh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gxjmaylmp.sHtML

[R14] C 风格 for
来源：http://www.blog.sjlbkw.cn/Article/details/gccmegtaf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/guhbnhkdy.sHtML

[R15] while 逐行读文件
来源：http://wap.vehdjk.com/Article/details/gcbqpurun.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.epnwcf.com/Article/details/gkakbtqlq.sHtML

[R16] until 等待条件
来源：http://wap.fktsv.cn/Article/details/gzfbeqdib.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gvyxwmmuv.sHtML

[R17] 数组定义与取值
来源：http://mobile.bbcook.cn/Article/details/gioildybg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.yfazqb.com/Article/details/glgfreqbv.sHtML

[R18] 遍历数组
来源：http://wap.yfazqb.com/Article/details/gfwqzivmg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fktsv.cn/Article/details/groodixef.sHtML

[R19] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gyjgdczbo.sHtML

echo "${#arr[@]}"
来源：http://3g.sjlbkw.cn/Article/details/gctmlipyb.sHtML

[R20] 关联数组（字典）
来源：http://baike.sjlbkw.cn/Article/details/ggsajlnka.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gjtzomqza.sHtML

[R21] 字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gfpamnxwq.sHtML

echo "${#s}"
来源：http://baike.epnwcf.com/Article/details/gkwbvprsc.sHtML

[R22] 截取子串
来源：http://wap.epnwcf.com/Article/details/gdmobcqnt.sHtML

echo "${s:0:5}"
来源：http://www.m.share.vehdjk.com/Article/details/gatexdcas.sHtML

[R23] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gdmjcbrsc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.sjlbkw.cn/Article/details/gybxgshzo.sHtML

[R24] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gzdwwuieb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.bbcook.cn/Article/details/geqvgyiwn.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.sjlbkw.cn/Article/details/gnnsoxujh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.vehdjk.com/Article/details/ghtqkqsik.sHtML

[R26] 命令替换
来源：http://wap.tarul.cn/Article/details/gwakkwuoh.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.sjlbkw.cn/Article/details/gekkqhqum.sHtML

[R27] 算术展开
来源：http://blog.tarul.cn/Article/details/gnoltmrgy.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fktsv.cn/Article/details/gswzueuto.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/gilfcaqyp.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.yfazqb.com/Article/details/gvtrrgfzt.sHtML

[R29] 定义函数
来源：http://read.share.tarul.cn/Article/details/gcdgeneaz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fktsv.cn/Article/details/gzmoukkvj.sHtML

[R30] 函数返回状态码
来源：http://baike.epnwcf.com/Article/details/gzzfevolk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.tarul.cn/Article/details/gmhuvnlad.sHtML

[R31] 局部变量
来源：http://wap.vehdjk.com/Article/details/goxdpbevm.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.tarul.cn/Article/details/gimvnpvnd.sHtML

[R32] 参数个数校验
来源：http://read.share.sjlbkw.cn/Article/details/gnbqrqpld.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gwybumlzq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/guwwhgsoz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.sjlbkw.cn/Article/details/gsotqbogq.sHtML

[R34] 退出时清理
来源：http://baike.epnwcf.com/Article/details/gbocgziki.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gtyoxxmdp.sHtML

[R35] 后台执行并等待
来源：http://3g.sjlbkw.cn/Article/details/gxkxbcdtm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.tarul.cn/Article/details/gboccztex.sHtML

[R36] 并发执行多个任务
来源：http://3g.fktsv.cn/Article/details/gphwvdjkr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/gbivwjnms.sHtML

[R37] 把输出赋给变量
来源：http://www.share.tarul.cn/Article/details/gugykqdxf.sHtML

files=$(ls -1)
来源：http://m.share.tarul.cn/Article/details/gbmruhhol.sHtML

[R38] 管道串联
来源：http://m.share.epnwcf.com/Article/details/gdrpbojcj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fktsv.cn/Article/details/gpeomficz.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.yfazqb.com/Article/details/gtmlyavex.sHtML

cmd > out.log 2>&1
来源：http://m.share.epnwcf.com/Article/details/gmhyxokqf.sHtML

[R40] 追加写日志
来源：http://mobile.epnwcf.com/Article/details/goketfqdi.sHtML

echo "log" >> out.log
来源：http://www.m.share.bbcook.cn/Article/details/gdlcdywdi.sHtML

[R41] 丢弃输出
来源：http://www.m.share.tarul.cn/Article/details/gwnndujtq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.tarul.cn/Article/details/gwdthoysd.sHtML

[R42] 输入重定向
来源：http://3g.yfazqb.com/Article/details/gnjouvvtc.sHtML

wc -l < a.txt
来源：http://www.blog.bbcook.cn/Article/details/gseelmtrm.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gyuunhdxz.sHtML

find . -name "*.log" -type f
来源：http://www.blog.yfazqb.com/Article/details/gmkcftlae.sHtML

[R44] 按修改时间查找
来源：http://blog.yfazqb.com/Article/details/gjtudkdqz.sHtML

find . -mtime -7 -type f
来源：http://baike.epnwcf.com/Article/details/gxhztthvt.sHtML

[R45] 批量删除
来源：http://blog.vehdjk.com/Article/details/gslmmqedx.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.bbcook.cn/Article/details/gamswjvzv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.vehdjk.com/Article/details/geqzjxbfy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fktsv.cn/Article/details/gdmolbhcv.sHtML

[R47] sed 单行替换
来源：http://m.share.vehdjk.com/Article/details/gbmafhdsp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.yfazqb.com/Article/details/gvuczzuxh.sHtML

[R48] awk 取指定列
来源：http://read.share.yfazqb.com/Article/details/gdrqfuyrf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/ghoovbxya.sHtML

[R49] awk 带条件
来源：http://www.m.share.yfazqb.com/Article/details/glttwnlqa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.vehdjk.com/Article/details/gtqzypgmd.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/grgdiizqe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fktsv.cn/Article/details/gblxcgfzf.sHtML

[R51] 排序去重取前几
来源：http://www.share.fktsv.cn/Article/details/gyhjmlbrf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.epnwcf.com/Article/details/gbkzabscj.sHtML

[R52] 统计行数
来源：http://www.m.share.yfazqb.com/Article/details/gojqmlulz.sHtML

wc -l a.txt
来源：http://www.m.share.tarul.cn/Article/details/gdfebpofp.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fktsv.cn/Article/details/gsmdnaenl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.epnwcf.com/Article/details/gfvkvvlmd.sHtML

[R54] 比较两个文件
来源：http://www.m.share.vehdjk.com/Article/details/gytrpmrel.sHtML

diff a.txt b.txt
来源：http://3g.fktsv.cn/Article/details/gulanwtcs.sHtML

[R55] 压缩与解压
来源：http://3g.yfazqb.com/Article/details/gsaqtqwzw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.sjlbkw.cn/Article/details/gevhuujaj.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/gymazriyg.sHtML

scp file user@host:/path/
来源：http://blog.vehdjk.com/Article/details/gnsvzsfiz.sHtML

[R57] 远程执行命令
来源：http://www.blog.epnwcf.com/Article/details/gxfkkzqxx.sHtML

ssh user@host 'uptime'
来源：http://m.share.sjlbkw.cn/Article/details/glnhkljae.sHtML

[R58] 下载文件
来源：http://mobile.sjlbkw.cn/Article/details/gqaeaewgv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.epnwcf.com/Article/details/gtwjgnxpi.sHtML

[R59] 发 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/grtdxbxov.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.tarul.cn/Article/details/geowwplzs.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.bbcook.cn/Article/details/gwcuephub.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gufclrwtv.sHtML

[R61] 磁盘占用
来源：http://www.m.share.vehdjk.com/Article/details/ghvdgdfuh.sHtML

df -h;  du -sh *
来源：http://www.blog.tarul.cn/Article/details/ggwqgaoab.sHtML

[R62] 找最占空间的文件
来源：http://m.share.vehdjk.com/Article/details/gaddcwtez.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.epnwcf.com/Article/details/gnlpqbpgg.sHtML

[R63] 内存与进程
来源：http://www.blog.epnwcf.com/Article/details/gumvgchyo.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.vehdjk.com/Article/details/gpxdtpxij.sHtML

[R64] 结束进程
来源：http://wap.bbcook.cn/Article/details/gbngfkmcl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/ganbrzdpq.sHtML

[R65] 查看端口占用
来源：http://read.share.vehdjk.com/Article/details/gtzvqhkrs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.bbcook.cn/Article/details/gqvpizkpg.sHtML

[R66] 定时任务
来源：http://wap.fktsv.cn/Article/details/gonigpdyt.sHtML

crontab -e;  crontab -l
来源：http://mobile.sjlbkw.cn/Article/details/ggstunjkp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.yfazqb.com/Article/details/gilshsovn.sHtML

openssl rand -hex 16
来源：http://read.share.vehdjk.com/Article/details/gjkxzavhk.sHtML

[R68] 计算文件校验值
来源：http://m.share.sjlbkw.cn/Article/details/gmyxqshif.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gxaplnjmr.sHtML

[R69] 生成随机密码
来源：http://mobile.yfazqb.com/Article/details/goyjjnika.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.tarul.cn/Article/details/gkasifgsf.sHtML

[R70] 时间戳与互转
来源：http://baike.bbcook.cn/Article/details/gnsitxaru.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/gbvirqwse.sHtML

[R71] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gjnrtarxr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fktsv.cn/Article/details/gsvijzbvr.sHtML

[R72] 等待端口就绪
来源：http://wap.sjlbkw.cn/Article/details/gkipcouxw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/gcmgtgctc.sHtML

[R73] 分割大日志
来源：http://baike.epnwcf.com/Article/details/gopciomri.sHtML

split -l 1000 big.log part_
来源：http://baike.epnwcf.com/Article/details/gvtqoadvp.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/gdarsxcsp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fktsv.cn/Article/details/grpukazgc.sHtML

[R75] 导出环境变量
来源：http://3g.yfazqb.com/Article/details/gvirwbuqt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.yfazqb.com/Article/details/gxtcftrmr.sHtML

[R76] 使用临时文件
来源：http://www.blog.tarul.cn/Article/details/grhlpqpwj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gobblxnxz.sHtML

[R77] 读取用户输入
来源：http://3g.yfazqb.com/Article/details/gubxiizpq.sHtML

read -rp "请输入: " ans
来源：http://www.share.tarul.cn/Article/details/gjxaxufly.sHtML

[R78] 交互式菜单
来源：http://wap.vehdjk.com/Article/details/gkzhxcjsh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fktsv.cn/Article/details/ghzjlaqdb.sHtML

[R79] 解析命令行选项
来源：http://read.share.tarul.cn/Article/details/gzcbrfgzp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.vehdjk.com/Article/details/gfnpyzoah.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwgeqdbi.sHtML

time ./run.sh
来源：http://www.share.bbcook.cn/Article/details/ggdmodlcx.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gefgrvwbg.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/gpvarmqmr.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gpemjqbqf.sHtML

[S01] C：Hello World
来源：http://baike.vehdjk.com/Article/details/gzrpjdhgq.sHtML

#include <stdio.h>
来源：http://m.share.tarul.cn/Article/details/gnkbxnrwf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/giasqdmka.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gpwrdhwuw.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.sjlbkw.cn/Article/details/gfttvuccp.sHtML

[S03] C：读入整数
来源：http://www.share.fktsv.cn/Article/details/geuowhqeu.sHtML

int x; scanf("%d", &x);
来源：http://m.share.bbcook.cn/Article/details/gycxsfvbg.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/geglpawgi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.epnwcf.com/Article/details/gxmxsfryi.sHtML

[S05] C：字符串长度
来源：http://baike.fktsv.cn/Article/details/ghlfzuedd.sHtML

strlen(s)
来源：http://www.m.share.epnwcf.com/Article/details/gqqfquqdc.sHtML

[S06] C：字符串比较
来源：http://read.share.yfazqb.com/Article/details/gqntqggdc.sHtML

strcmp(a, b) == 0
来源：http://blog.epnwcf.com/Article/details/gkplrdvre.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/ghlzyumwb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.vehdjk.com/Article/details/gkdbhwtnz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.yfazqb.com/Article/details/gxylfwvyh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtiihqikz.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.sjlbkw.cn/Article/details/giuyqzvgy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.tarul.cn/Article/details/ginawsgfd.sHtML

[S10] C：指针与解引用
来源：http://3g.tarul.cn/Article/details/gwczkdowu.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.tarul.cn/Article/details/gkyfgndgx.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/ghtxceqtz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fktsv.cn/Article/details/gzsrzidsw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.yfazqb.com/Article/details/grncdaanc.sHtML

fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gnxgkqeat.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/ghumqnnap.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.bbcook.cn/Article/details/gshspmzbv.sHtML

[S13] C：宏定义
来源：http://wap.epnwcf.com/Article/details/gadxbypns.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.tarul.cn/Article/details/gmbdmjkko.sHtML

[S14] C：枚举
来源：http://www.m.share.bbcook.cn/Article/details/gpubrjipy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.tarul.cn/Article/details/gfaiaglbp.sHtML

[S15] C：类型转换
来源：http://www.blog.tarul.cn/Article/details/gcpfczqzs.sHtML

(double) a / b
来源：http://www.m.share.vehdjk.com/Article/details/ghogavqul.sHtML

[S16] C：位操作置位
来源：http://baike.vehdjk.com/Article/details/gtewbtcfa.sHtML

x |= (1 << 3);
来源：http://wap.bbcook.cn/Article/details/goiywrqdw.sHtML

[S17] C：安全拼接字符串
来源：http://wap.bbcook.cn/Article/details/gqzgrqkxi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.tarul.cn/Article/details/gtfckgliy.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gzrelztcl.sHtML

int main(int argc, char **argv)
来源：http://www.blog.vehdjk.com/Article/details/ggogxdqph.sHtML

[S19] C：快速排序
来源：http://m.share.fktsv.cn/Article/details/ghorhtcnj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gspbavbux.sHtML

[S20] C：二分查找
来源：http://www.m.share.tarul.cn/Article/details/gixpmqjil.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gyhtdmxff.sHtML

[S21] C：字符类别判断
来源：http://read.share.tarul.cn/Article/details/gxskxpqua.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.sjlbkw.cn/Article/details/glldkkmmn.sHtML

[S22] C：字符串转数字
来源：http://3g.yfazqb.com/Article/details/gcmqufhkz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.yfazqb.com/Article/details/gdtowlwhb.sHtML

[S23] C：随机数
来源：http://blog.yfazqb.com/Article/details/glssagvns.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.sjlbkw.cn/Article/details/gmbvvwrvk.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/gzbtqorps.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/goujggcoe.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gmrscsldu.sHtML

memcpy(dst, src, n);
来源：http://read.share.epnwcf.com/Article/details/gadcwfxfc.sHtML

[S26] C：内存清零
来源：http://blog.sjlbkw.cn/Article/details/gjxgbjmfu.sHtML


<!-- 参考信息 -->