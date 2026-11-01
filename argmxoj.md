代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.tarul.cn/Article/details/ggwrlhbzg.sHtML

[Q54] 清空表
来源：http://www.share.vehdjk.com/Article/details/gkyfilhzt.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.tarul.cn/Article/details/gasbcxheg.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwpkowhu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gleahkxsc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/glczfrcsw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gximrcfxd.sHtML

[Q57] 行号
来源：http://mobile.yfazqb.com/Article/details/gbsvotwsq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.epnwcf.com/Article/details/ggpuqavfy.sHtML

[Q58] 累计求和
来源：http://baike.fktsv.cn/Article/details/gpnluxjgz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gbscgxmqx.sHtML

[Q59] 分组内累计
来源：http://wap.epnwcf.com/Article/details/gmmxdtscc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gpexxhfwa.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.vehdjk.com/Article/details/gfpmcrdkr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.vehdjk.com/Article/details/gkdbeqogv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gqdxfkwfz.sHtML

[Q61] 移动平均
来源：http://m.share.yfazqb.com/Article/details/gsgagmboj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gpmzskavw.sHtML

[Q62] 分组占比
来源：http://baike.epnwcf.com/Article/details/gluevehxe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gckqxleds.sHtML

[Q63] 开启事务
来源：http://mobile.yfazqb.com/Article/details/gklradrvq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fktsv.cn/Article/details/gigjgokzm.sHtML

[Q64] 提交事务
来源：http://baike.tarul.cn/Article/details/gugsqhzfe.sHtML

COMMIT;
来源：http://www.blog.epnwcf.com/Article/details/gkvqbhfcd.sHtML

[Q65] 回滚事务
来源：http://m.share.epnwcf.com/Article/details/gnefsaeup.sHtML

ROLLBACK;
来源：http://www.share.yfazqb.com/Article/details/gzgdkbych.sHtML

[Q66] 行锁查询
来源：http://wap.tarul.cn/Article/details/gdnmlflzh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.sjlbkw.cn/Article/details/gpzuxorfh.sHtML

[Q67] 设置隔离级别
来源：http://www.share.tarul.cn/Article/details/gerabjkad.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.tarul.cn/Article/details/gkqmqbqml.sHtML

[Q68] 保存点
来源：http://www.share.fktsv.cn/Article/details/gnkkounto.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.tarul.cn/Article/details/gooqicqxu.sHtML

ROLLBACK TO sp1;
来源：http://baike.epnwcf.com/Article/details/gxwudznug.sHtML

[Q69] 查看执行计划
来源：http://blog.fktsv.cn/Article/details/ggbdrubus.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.bbcook.cn/Article/details/gkmlgyoql.sHtML

[Q70] 更新统计信息
来源：http://www.share.epnwcf.com/Article/details/gxrajqmep.sHtML

ANALYZE TABLE users;
来源：http://baike.yfazqb.com/Article/details/gtcblfenc.sHtML

[Q71] 查看建表语句
来源：http://blog.tarul.cn/Article/details/geydovxsv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fktsv.cn/Article/details/gimkyrzye.sHtML

[Q72] 查看索引
来源：http://mobile.sjlbkw.cn/Article/details/gpnkgoobz.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gctdtldkv.sHtML

[Q73] 查看表状态
来源：http://www.blog.tarul.cn/Article/details/geuizkmui.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fktsv.cn/Article/details/gqoufhoaa.sHtML

[Q74] 强制使用索引
来源：http://www.share.sjlbkw.cn/Article/details/gyzxhqszo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.vehdjk.com/Article/details/ggghexrcr.sHtML

[Q75] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gikwggroq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gkxzwkohu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.tarul.cn/Article/details/gmrcustkr.sHtML

[Q76] 按天统计
来源：http://wap.epnwcf.com/Article/details/gmvqqieod.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.bbcook.cn/Article/details/gngdgjbol.sHtML

[Q77] 时间加减
来源：http://baike.epnwcf.com/Article/details/gyopowqxn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.sjlbkw.cn/Article/details/gkvfjzfmh.sHtML

[Q78] 当前时间
来源：http://3g.fktsv.cn/Article/details/gyzijncgh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.yfazqb.com/Article/details/gvlbbpcei.sHtML

[Q79] 字符串拼接
来源：http://3g.vehdjk.com/Article/details/gughygbwb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.epnwcf.com/Article/details/gzpcxlrfh.sHtML

[Q80] 字符串截取
来源：http://blog.vehdjk.com/Article/details/gkthrajct.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.vehdjk.com/Article/details/gsecvpcwx.sHtML

[Q81] 字符串替换
来源：http://wap.bbcook.cn/Article/details/gkshbptmw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.yfazqb.com/Article/details/ghhvmgzsc.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.tarul.cn/Article/details/gthewmvzd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gezyypbrg.sHtML

[Q83] 大小写转换
来源：http://3g.tarul.cn/Article/details/gowayabjq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/glvdjubns.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.sjlbkw.cn/Article/details/gshjjdnyn.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gadghfzfv.sHtML

[Q85] 数值取整
来源：http://www.blog.yfazqb.com/Article/details/ggwesfnca.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.epnwcf.com/Article/details/gvdphignk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.tarul.cn/Article/details/gawdrbhwi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.sjlbkw.cn/Article/details/gzuvddaxl.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.bbcook.cn/Article/details/gopeaknki.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fktsv.cn/Article/details/ghbjghfkb.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.bbcook.cn/Article/details/gnspmugsm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.yfazqb.com/Article/details/gdguugxwl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.yfazqb.com/Article/details/gkkljibly.sHtML

[Q89] 判断表是否存在
来源：http://3g.vehdjk.com/Article/details/gbaztaisp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gqkajsbpo.sHtML

[Q90] 生成序号列
来源：http://www.share.fktsv.cn/Article/details/gaxqblqtp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fktsv.cn/Article/details/gaxezlvji.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/grqrouncd.sHtML

R. Bash 专题
来源：http://blog.sjlbkw.cn/Article/details/gskrzjrax.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gfblavrdc.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/gdqqoenet.sHtML

#!/usr/bin/env bash
来源：http://mobile.tarul.cn/Article/details/gntqfidzq.sHtML

set -euo pipefail
来源：http://www.share.yfazqb.com/Article/details/gufqsuijk.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fktsv.cn/Article/details/giutailht.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/grxmynwyk.sHtML

[R03] 只读变量
来源：http://3g.epnwcf.com/Article/details/gdtjyfshc.sHtML

readonly PI=3.14
来源：http://www.share.tarul.cn/Article/details/gljvworqh.sHtML

[R04] 位置参数
来源：http://baike.bbcook.cn/Article/details/gufmodofc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.yfazqb.com/Article/details/gdpeschhp.sHtML

[R05] 参数默认值
来源：http://wap.fktsv.cn/Article/details/gqeygznir.sHtML

name="${1:-default}"
来源：http://wap.tarul.cn/Article/details/gounihalq.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fktsv.cn/Article/details/gylgsysxv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gowvowhrl.sHtML

[R07] if 判断文件
来源：http://www.share.epnwcf.com/Article/details/gnqahiiog.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.tarul.cn/Article/details/gbumlnngp.sHtML

[R08] 数值比较
来源：http://m.share.fktsv.cn/Article/details/gajgewnrl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.tarul.cn/Article/details/gskymtulf.sHtML

[R09] 字符串比较
来源：http://blog.epnwcf.com/Article/details/gigvpagrx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gbesmpqyn.sHtML

[R10] 正则匹配
来源：http://read.share.bbcook.cn/Article/details/gcofltowh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.tarul.cn/Article/details/glrvcsqzy.sHtML

[R11] case 多分支
来源：http://baike.fktsv.cn/Article/details/gnqmgjffx.sHtML

case "$1" in
来源：http://3g.bbcook.cn/Article/details/gvpvwjtmo.sHtML

start) echo "启动" ;;
来源：http://m.share.bbcook.cn/Article/details/gsgxtwtyo.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gtrgulzsa.sHtML

*)     echo "未知命令" ;;
来源：http://blog.epnwcf.com/Article/details/gdmnwumux.sHtML

esac
来源：http://blog.yfazqb.com/Article/details/grtkmksfw.sHtML

[R12] for 遍历文件
来源：http://www.share.sjlbkw.cn/Article/details/gzruzfywz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.yfazqb.com/Article/details/goalxkbuc.sHtML

[R13] for 计数循环
来源：http://read.share.bbcook.cn/Article/details/ggvicfrrp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gxrjvtzon.sHtML

[R14] C 风格 for
来源：http://mobile.vehdjk.com/Article/details/gpptugoqc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gzqfsemez.sHtML

[R15] while 逐行读文件
来源：http://wap.yfazqb.com/Article/details/gbirhucjp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fktsv.cn/Article/details/gobdvhtet.sHtML

[R16] until 等待条件
来源：http://wap.sjlbkw.cn/Article/details/gemrmgdvi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gairzyozk.sHtML

[R17] 数组定义与取值
来源：http://m.share.bbcook.cn/Article/details/gxqqreoca.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.epnwcf.com/Article/details/gsatakdji.sHtML

[R18] 遍历数组
来源：http://www.share.sjlbkw.cn/Article/details/gccotezxn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.yfazqb.com/Article/details/glabticcl.sHtML

[R19] 数组长度
来源：http://blog.fktsv.cn/Article/details/glxknnjkc.sHtML

echo "${#arr[@]}"
来源：http://blog.vehdjk.com/Article/details/gdibpywzq.sHtML

[R20] 关联数组（字典）
来源：http://m.share.bbcook.cn/Article/details/glixtsuco.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fktsv.cn/Article/details/gcjmqltsx.sHtML

[R21] 字符串长度
来源：http://baike.bbcook.cn/Article/details/gdrrthmod.sHtML

echo "${#s}"
来源：http://www.share.bbcook.cn/Article/details/gbszxylai.sHtML

[R22] 截取子串
来源：http://wap.vehdjk.com/Article/details/gmcrgmvzk.sHtML

echo "${s:0:5}"
来源：http://www.share.fktsv.cn/Article/details/gnpwkxxkv.sHtML

[R23] 字符串替换
来源：http://mobile.tarul.cn/Article/details/goaxistaj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.vehdjk.com/Article/details/gjfsaldes.sHtML

[R24] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gnduntxzh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.epnwcf.com/Article/details/gnklcyngo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.yfazqb.com/Article/details/ggnzldshf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.vehdjk.com/Article/details/gqkyyvjku.sHtML

[R26] 命令替换
来源：http://www.blog.sjlbkw.cn/Article/details/gelwwyapp.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.tarul.cn/Article/details/gsvoyvovp.sHtML

[R27] 算术展开
来源：http://baike.tarul.cn/Article/details/gjuymeqoy.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fktsv.cn/Article/details/gyijutqkw.sHtML

[R28] 浮点运算
来源：http://m.share.fktsv.cn/Article/details/gsnczpsht.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.tarul.cn/Article/details/gyudqaarf.sHtML

[R29] 定义函数
来源：http://read.share.yfazqb.com/Article/details/gneyinnot.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.yfazqb.com/Article/details/gdhxvjqfq.sHtML

[R30] 函数返回状态码
来源：http://m.share.yfazqb.com/Article/details/gwdpivgpn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fktsv.cn/Article/details/gkqaiqahx.sHtML

[R31] 局部变量
来源：http://www.blog.epnwcf.com/Article/details/gyattnjqt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.epnwcf.com/Article/details/gskiexltz.sHtML

[R32] 参数个数校验
来源：http://www.share.sjlbkw.cn/Article/details/geqiedmcn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gqewulcje.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.tarul.cn/Article/details/gikrnqaiv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.epnwcf.com/Article/details/geshbmlax.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/gepmbstfh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gciagbzel.sHtML

[R35] 后台执行并等待
来源：http://wap.bbcook.cn/Article/details/ghyduytkd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.yfazqb.com/Article/details/gpfngliou.sHtML

[R36] 并发执行多个任务
来源：http://m.share.tarul.cn/Article/details/gucwbjoyh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.sjlbkw.cn/Article/details/gkhhspfhr.sHtML

[R37] 把输出赋给变量
来源：http://m.share.sjlbkw.cn/Article/details/gtospfquz.sHtML

files=$(ls -1)
来源：http://www.share.bbcook.cn/Article/details/gsxhczqza.sHtML

[R38] 管道串联
来源：http://baike.fktsv.cn/Article/details/gynvjgdpw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.sjlbkw.cn/Article/details/gzhhdzsir.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.yfazqb.com/Article/details/gxfbeuaka.sHtML

cmd > out.log 2>&1
来源：http://m.share.bbcook.cn/Article/details/gucluwyms.sHtML

[R40] 追加写日志
来源：http://mobile.yfazqb.com/Article/details/gyabtwgux.sHtML

echo "log" >> out.log
来源：http://baike.yfazqb.com/Article/details/gbwsuylci.sHtML

[R41] 丢弃输出
来源：http://www.blog.sjlbkw.cn/Article/details/gsxtjrvvr.sHtML

cmd >/dev/null 2>&1
来源：http://wap.epnwcf.com/Article/details/guegymhje.sHtML

[R42] 输入重定向
来源：http://m.share.bbcook.cn/Article/details/gucswneag.sHtML

wc -l < a.txt
来源：http://m.share.fktsv.cn/Article/details/gryijpcat.sHtML

[R43] 按名字查找文件
来源：http://blog.vehdjk.com/Article/details/gztikvwxv.sHtML

find . -name "*.log" -type f
来源：http://baike.fktsv.cn/Article/details/gihrtmglc.sHtML

[R44] 按修改时间查找
来源：http://read.share.tarul.cn/Article/details/ggzdnjkhi.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/grqfgnvwt.sHtML

[R45] 批量删除
来源：http://3g.bbcook.cn/Article/details/gcxnteccn.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gmjcqxngb.sHtML

[R46] 递归替换文件内容
来源：http://m.share.sjlbkw.cn/Article/details/gpvdatalo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.bbcook.cn/Article/details/gujkjtbcn.sHtML

[R47] sed 单行替换
来源：http://blog.tarul.cn/Article/details/gdjulhpqg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gdyrvbeln.sHtML

[R48] awk 取指定列
来源：http://blog.yfazqb.com/Article/details/gmtaleabi.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gqphtfybl.sHtML

[R49] awk 带条件
来源：http://www.blog.sjlbkw.cn/Article/details/gryiwevky.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.vehdjk.com/Article/details/gnnrskatw.sHtML

[R50] awk 求和
来源：http://www.share.tarul.cn/Article/details/geqqstofe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gdudihgll.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.epnwcf.com/Article/details/gmjrlteyb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fktsv.cn/Article/details/gueaiozzu.sHtML

[R52] 统计行数
来源：http://www.share.tarul.cn/Article/details/gbroprnoq.sHtML

wc -l a.txt
来源：http://www.blog.epnwcf.com/Article/details/gwjfkzljg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fktsv.cn/Article/details/gempaxufe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.bbcook.cn/Article/details/gofeafyep.sHtML

[R54] 比较两个文件
来源：http://mobile.sjlbkw.cn/Article/details/gakbukkol.sHtML

diff a.txt b.txt
来源：http://3g.fktsv.cn/Article/details/gllsmzbfq.sHtML

[R55] 压缩与解压
来源：http://m.share.sjlbkw.cn/Article/details/gkbyziuuk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fktsv.cn/Article/details/gaoykdlpx.sHtML

[R56] 远程拷贝
来源：http://mobile.bbcook.cn/Article/details/gfyhcuowy.sHtML

scp file user@host:/path/
来源：http://3g.fktsv.cn/Article/details/gmqsnyqrw.sHtML

[R57] 远程执行命令
来源：http://www.share.epnwcf.com/Article/details/gyhvowajy.sHtML

ssh user@host 'uptime'
来源：http://baike.bbcook.cn/Article/details/gmcuvfzao.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/glekrtdje.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.epnwcf.com/Article/details/gpeyudket.sHtML

[R59] 发 POST JSON
来源：http://blog.bbcook.cn/Article/details/glgrmygve.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.vehdjk.com/Article/details/glxypdxuw.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gukycpvrg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.sjlbkw.cn/Article/details/ghmhtwhsa.sHtML

[R61] 磁盘占用
来源：http://wap.epnwcf.com/Article/details/gmwgrhhiu.sHtML

df -h;  du -sh *
来源：http://blog.vehdjk.com/Article/details/gygotokcd.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.tarul.cn/Article/details/gcfiswdrx.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.tarul.cn/Article/details/ghwyaltex.sHtML

[R63] 内存与进程
来源：http://wap.fktsv.cn/Article/details/gncjfqcqh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fktsv.cn/Article/details/ghrydnpds.sHtML

[R64] 结束进程
来源：http://3g.bbcook.cn/Article/details/gdtvzjhrc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/gtwmytzcd.sHtML

[R65] 查看端口占用
来源：http://blog.bbcook.cn/Article/details/gmfetovyv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fktsv.cn/Article/details/geziaoqgx.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/gtbonhaql.sHtML

crontab -e;  crontab -l
来源：http://m.share.tarul.cn/Article/details/gzmseqavy.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.vehdjk.com/Article/details/gyusjasmc.sHtML

openssl rand -hex 16
来源：http://www.m.share.epnwcf.com/Article/details/glbnugopr.sHtML

[R68] 计算文件校验值
来源：http://www.share.sjlbkw.cn/Article/details/gtmnxhbzp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.tarul.cn/Article/details/ghmpuesos.sHtML

[R69] 生成随机密码
来源：http://www.blog.vehdjk.com/Article/details/gpcdehasr.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.yfazqb.com/Article/details/gzylaeqvh.sHtML

[R70] 时间戳与互转
来源：http://3g.epnwcf.com/Article/details/gwnrilbae.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.bbcook.cn/Article/details/gbpdgcahg.sHtML

[R71] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/gjopkujxf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.yfazqb.com/Article/details/grvmthybo.sHtML

[R72] 等待端口就绪
来源：http://m.share.epnwcf.com/Article/details/ggmkwjxcp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gvmeaeoqn.sHtML

[R73] 分割大日志
来源：http://mobile.epnwcf.com/Article/details/gzcmcbijg.sHtML

split -l 1000 big.log part_
来源：http://mobile.tarul.cn/Article/details/gpmzdgvyx.sHtML

[R74] 批量重命名
来源：http://wap.sjlbkw.cn/Article/details/gtwqlbgrx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.vehdjk.com/Article/details/gwauaziok.sHtML

[R75] 导出环境变量
来源：http://m.share.fktsv.cn/Article/details/gzfnitohn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fktsv.cn/Article/details/gkmleofba.sHtML

[R76] 使用临时文件
来源：http://www.share.yfazqb.com/Article/details/glpllifah.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/ghmwfnwml.sHtML

[R77] 读取用户输入
来源：http://wap.sjlbkw.cn/Article/details/gwgowever.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/gudhgwdnq.sHtML

[R78] 交互式菜单
来源：http://m.share.tarul.cn/Article/details/ghgqdyqtk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/gqmmhdtja.sHtML

[R79] 解析命令行选项
来源：http://www.blog.yfazqb.com/Article/details/grqmzrbof.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.yfazqb.com/Article/details/gbywndsqo.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.bbcook.cn/Article/details/gdgocwndu.sHtML

time ./run.sh
来源：http://wap.epnwcf.com/Article/details/gculgaluv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glbdxtvip.sHtML

S. C / C++ 专题
来源：http://blog.bbcook.cn/Article/details/gncrblyhu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvvmrkzpa.sHtML

[S01] C：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/ghpktwqfq.sHtML

#include <stdio.h>
来源：http://mobile.sjlbkw.cn/Article/details/gzbqxmqxy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.bbcook.cn/Article/details/gjiikrqll.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.tarul.cn/Article/details/gytlyieym.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.vehdjk.com/Article/details/gctutgrwx.sHtML

[S03] C：读入整数
来源：http://www.blog.fktsv.cn/Article/details/gapmmmdov.sHtML

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/ghquyzxsq.sHtML

[S04] C：字符串复制
来源：http://read.share.bbcook.cn/Article/details/glysqbjgr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.yfazqb.com/Article/details/gdjoixcph.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/gjfkjqknz.sHtML

strlen(s)
来源：http://baike.yfazqb.com/Article/details/gsoqwboty.sHtML

[S06] C：字符串比较
来源：http://3g.epnwcf.com/Article/details/ggpktubvr.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/gtytwparl.sHtML

[S07] C：数组遍历求和
来源：http://baike.vehdjk.com/Article/details/gtcbnplmr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.tarul.cn/Article/details/grgaubhjs.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.sjlbkw.cn/Article/details/gmitwosdu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/givzzkzoi.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.yfazqb.com/Article/details/gknwpejga.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.tarul.cn/Article/details/gipfpnebg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.vehdjk.com/Article/details/gsvynlpxg.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.bbcook.cn/Article/details/gslvrcmja.sHtML

[S11] C：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gvgrtyfgb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.vehdjk.com/Article/details/gzkizkxqh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gseziydub.sHtML

fclose(f);
来源：http://3g.bbcook.cn/Article/details/guttegejk.sHtML

[S12] C：写文件
来源：http://www.blog.fktsv.cn/Article/details/gubytnfab.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gqftkaava.sHtML

[S13] C：宏定义
来源：http://www.blog.fktsv.cn/Article/details/gcqjhqpcc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnmrcgtv.sHtML

[S14] C：枚举
来源：http://read.share.epnwcf.com/Article/details/gzrzejgnk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fktsv.cn/Article/details/gjnhqifcq.sHtML

[S15] C：类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gguehznkn.sHtML

(double) a / b
来源：http://www.share.fktsv.cn/Article/details/ghauoqkrx.sHtML

[S16] C：位操作置位
来源：http://baike.bbcook.cn/Article/details/gixcemqqc.sHtML

x |= (1 << 3);
来源：http://www.m.share.epnwcf.com/Article/details/gvoakbtvz.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gqmhgbyag.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.tarul.cn/Article/details/gmbhaxrat.sHtML

[S18] C：命令行参数
来源：http://www.blog.vehdjk.com/Article/details/gxdxjpbkl.sHtML

int main(int argc, char **argv)
来源：http://wap.bbcook.cn/Article/details/gsohjaszd.sHtML

[S19] C：快速排序
来源：http://m.share.epnwcf.com/Article/details/gzkdoqjkk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gureptpbk.sHtML

[S20] C：二分查找
来源：http://m.share.tarul.cn/Article/details/geqvthwma.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/gfbvdhlsz.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/gynmzzgfl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.sjlbkw.cn/Article/details/gpxylkvxg.sHtML

[S22] C：字符串转数字
来源：http://www.share.epnwcf.com/Article/details/gxxrnfcve.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.yfazqb.com/Article/details/gzwszutxk.sHtML

[S23] C：随机数
来源：http://blog.tarul.cn/Article/details/gkohbbppo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fktsv.cn/Article/details/gmkgurdto.sHtML

[S24] C：获取本地时间
来源：http://m.share.fktsv.cn/Article/details/gomabrwan.sHtML


<!-- 参考信息 -->