代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gtdhqfamn.sHtML

[Q52] 删除指定行
来源：http://read.share.sjlbkw.cn/Article/details/gjjxyyprd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/grlrldloj.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/gbnllwupz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbduaiar.sHtML

[Q54] 清空表
来源：http://3g.epnwcf.com/Article/details/gowmasejy.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.vehdjk.com/Article/details/ghwxiywld.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.epnwcf.com/Article/details/gjhxhogif.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.bbcook.cn/Article/details/gdgiwniov.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.sjlbkw.cn/Article/details/gwvagfdjb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gwwsaydjj.sHtML

[Q57] 行号
来源：http://baike.tarul.cn/Article/details/goqcxxtho.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.epnwcf.com/Article/details/gqdjdvsye.sHtML

[Q58] 累计求和
来源：http://www.blog.vehdjk.com/Article/details/goppgymkw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.epnwcf.com/Article/details/gmyfgenbl.sHtML

[Q59] 分组内累计
来源：http://blog.epnwcf.com/Article/details/givityvpr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gzqdzckds.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.bbcook.cn/Article/details/gqqhjekqj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.tarul.cn/Article/details/gnuqxozej.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.yfazqb.com/Article/details/gyflvckrl.sHtML

[Q61] 移动平均
来源：http://www.share.tarul.cn/Article/details/gtmsvmkor.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gnxlmwqrj.sHtML

[Q62] 分组占比
来源：http://www.m.share.epnwcf.com/Article/details/gqubuvvde.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gxrdrvhty.sHtML

[Q63] 开启事务
来源：http://www.share.tarul.cn/Article/details/gigdqmigz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.sjlbkw.cn/Article/details/guhziupuk.sHtML

[Q64] 提交事务
来源：http://www.share.yfazqb.com/Article/details/gopeklhcx.sHtML

COMMIT;
来源：http://baike.vehdjk.com/Article/details/ggnthefok.sHtML

[Q65] 回滚事务
来源：http://www.blog.yfazqb.com/Article/details/gobokvsjg.sHtML

ROLLBACK;
来源：http://3g.bbcook.cn/Article/details/goyrwnxdz.sHtML

[Q66] 行锁查询
来源：http://www.share.bbcook.cn/Article/details/gwdsyuesj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.vehdjk.com/Article/details/gcmgdblgz.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fktsv.cn/Article/details/gukiwixxv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fktsv.cn/Article/details/gvtnnwede.sHtML

[Q68] 保存点
来源：http://read.share.yfazqb.com/Article/details/gogxkarro.sHtML

SAVEPOINT sp1;
来源：http://baike.sjlbkw.cn/Article/details/gorrxrpiw.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.epnwcf.com/Article/details/gozukrcvu.sHtML

[Q69] 查看执行计划
来源：http://www.share.epnwcf.com/Article/details/gbghpttmi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.bbcook.cn/Article/details/gzxcsxfjy.sHtML

[Q70] 更新统计信息
来源：http://read.share.bbcook.cn/Article/details/gfxavvjkj.sHtML

ANALYZE TABLE users;
来源：http://mobile.epnwcf.com/Article/details/gkmbtjslf.sHtML

[Q71] 查看建表语句
来源：http://wap.sjlbkw.cn/Article/details/gjfnifusw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.sjlbkw.cn/Article/details/gspffqdwj.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/gwfbqbhvg.sHtML

SHOW INDEX FROM users;
来源：http://3g.yfazqb.com/Article/details/gsgdedkxj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fktsv.cn/Article/details/gdtkmftzc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fktsv.cn/Article/details/gxobhihxb.sHtML

[Q74] 强制使用索引
来源：http://3g.yfazqb.com/Article/details/gyxqitzwv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.vehdjk.com/Article/details/gchwjvbhl.sHtML

[Q75] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gsxfdpaaq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.epnwcf.com/Article/details/gwamtwwjl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fktsv.cn/Article/details/gffwxxxmg.sHtML

[Q76] 按天统计
来源：http://baike.bbcook.cn/Article/details/gxubipobx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.tarul.cn/Article/details/gazwmzytp.sHtML

[Q77] 时间加减
来源：http://mobile.sjlbkw.cn/Article/details/gvslwpdxv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.tarul.cn/Article/details/gckaqlxft.sHtML

[Q78] 当前时间
来源：http://blog.epnwcf.com/Article/details/ggjnvrfhp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.tarul.cn/Article/details/gpoygfmmh.sHtML

[Q79] 字符串拼接
来源：http://mobile.bbcook.cn/Article/details/gxvidiqms.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.yfazqb.com/Article/details/gxfwpramy.sHtML

[Q80] 字符串截取
来源：http://mobile.bbcook.cn/Article/details/gdexmaupl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/geavivtta.sHtML

[Q81] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/gntoqgsny.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gpafyifks.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.vehdjk.com/Article/details/gqueqwjfg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gbscwiqhf.sHtML

[Q83] 大小写转换
来源：http://blog.tarul.cn/Article/details/gqksnmyql.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gibmrihxk.sHtML

[Q84] 去除首尾空格
来源：http://3g.yfazqb.com/Article/details/gekvcgmlb.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gdfnzpbtg.sHtML

[Q85] 数值取整
来源：http://m.share.bbcook.cn/Article/details/guwpodhib.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.tarul.cn/Article/details/gkkfdcbhy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.sjlbkw.cn/Article/details/gvpqyqpld.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.bbcook.cn/Article/details/gjajmelet.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/ggxxkkxal.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/gtkzbpezj.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.epnwcf.com/Article/details/gowfbronj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.tarul.cn/Article/details/gldwilxdn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.yfazqb.com/Article/details/gjzrijvmk.sHtML

[Q89] 判断表是否存在
来源：http://baike.tarul.cn/Article/details/guffaqrah.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.vehdjk.com/Article/details/ghrxizevk.sHtML

[Q90] 生成序号列
来源：http://baike.bbcook.cn/Article/details/gsfykhcwm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fktsv.cn/Article/details/gduhmssvm.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzrniemkl.sHtML

R. Bash 专题
来源：http://blog.vehdjk.com/Article/details/glbxbvlsi.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghwvuxgta.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fktsv.cn/Article/details/gkmhibjaz.sHtML

#!/usr/bin/env bash
来源：http://m.share.tarul.cn/Article/details/gcqglbfph.sHtML

set -euo pipefail
来源：http://www.m.share.sjlbkw.cn/Article/details/gqphfepwk.sHtML

[R02] 变量赋值与使用
来源：http://wap.vehdjk.com/Article/details/glsthtcfu.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.bbcook.cn/Article/details/ghqwgfahx.sHtML

[R03] 只读变量
来源：http://mobile.bbcook.cn/Article/details/gltegaujy.sHtML

readonly PI=3.14
来源：http://wap.sjlbkw.cn/Article/details/gaozubgdj.sHtML

[R04] 位置参数
来源：http://3g.sjlbkw.cn/Article/details/grjfkqrdv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.vehdjk.com/Article/details/gzvkyqhoj.sHtML

[R05] 参数默认值
来源：http://wap.sjlbkw.cn/Article/details/gqheiecng.sHtML

name="${1:-default}"
来源：http://www.blog.sjlbkw.cn/Article/details/gcqodfpcc.sHtML

[R06] 判断命令是否存在
来源：http://m.share.epnwcf.com/Article/details/gelmjakdp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.yfazqb.com/Article/details/giufjrqxr.sHtML

[R07] if 判断文件
来源：http://read.share.fktsv.cn/Article/details/gcewaahcg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.tarul.cn/Article/details/gusztnnsy.sHtML

[R08] 数值比较
来源：http://blog.tarul.cn/Article/details/gdacfpghy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/grngjifit.sHtML

[R09] 字符串比较
来源：http://wap.fktsv.cn/Article/details/ghrvqqndu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.sjlbkw.cn/Article/details/gdgmvnapl.sHtML

[R10] 正则匹配
来源：http://mobile.bbcook.cn/Article/details/gypnggzqw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.epnwcf.com/Article/details/gtmyczqgn.sHtML

[R11] case 多分支
来源：http://blog.fktsv.cn/Article/details/gfzlgwovz.sHtML

case "$1" in
来源：http://wap.yfazqb.com/Article/details/gvhjlqdgx.sHtML

start) echo "启动" ;;
来源：http://baike.bbcook.cn/Article/details/gatjspffm.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/goszpvfhb.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.bbcook.cn/Article/details/gldxuyyrj.sHtML

esac
来源：http://www.blog.vehdjk.com/Article/details/gsumlkdtz.sHtML

[R12] for 遍历文件
来源：http://www.blog.vehdjk.com/Article/details/gmgpjnjwo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.yfazqb.com/Article/details/gxdmiptuj.sHtML

[R13] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gqqtpkuah.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/ghwrnggpd.sHtML

[R14] C 风格 for
来源：http://www.blog.vehdjk.com/Article/details/gyqrrngms.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gskkoowdm.sHtML

[R15] while 逐行读文件
来源：http://3g.fktsv.cn/Article/details/godlzyiug.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.tarul.cn/Article/details/ggwlxdinj.sHtML

[R16] until 等待条件
来源：http://www.blog.tarul.cn/Article/details/gxyradhtf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gvdouiqpi.sHtML

[R17] 数组定义与取值
来源：http://baike.tarul.cn/Article/details/gzgihcial.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbrdvaib.sHtML

[R18] 遍历数组
来源：http://baike.epnwcf.com/Article/details/gbiavyvhu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.yfazqb.com/Article/details/gnycswwlz.sHtML

[R19] 数组长度
来源：http://blog.epnwcf.com/Article/details/ggtiemdgc.sHtML

echo "${#arr[@]}"
来源：http://wap.fktsv.cn/Article/details/gtmgdeoav.sHtML

[R20] 关联数组（字典）
来源：http://read.share.vehdjk.com/Article/details/grymdqjbg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.epnwcf.com/Article/details/gmrfimvsh.sHtML

[R21] 字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/ggjanbkll.sHtML

echo "${#s}"
来源：http://baike.epnwcf.com/Article/details/gtuotlypb.sHtML

[R22] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gkmimlxuo.sHtML

echo "${s:0:5}"
来源：http://www.m.share.vehdjk.com/Article/details/gqexirbgl.sHtML

[R23] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gefnnprrx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.bbcook.cn/Article/details/grsmiyaqk.sHtML

[R24] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gbdbzgjuj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.sjlbkw.cn/Article/details/gdxzsutmc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.tarul.cn/Article/details/gfipitkim.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.epnwcf.com/Article/details/gnvirplwz.sHtML

[R26] 命令替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhzvosel.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.bbcook.cn/Article/details/gqrdsgges.sHtML

[R27] 算术展开
来源：http://www.blog.yfazqb.com/Article/details/gbcngvidx.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fktsv.cn/Article/details/gagysjthd.sHtML

[R28] 浮点运算
来源：http://mobile.tarul.cn/Article/details/gpbqbbekx.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.yfazqb.com/Article/details/gdxqyvtst.sHtML

[R29] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gzlhzhkbo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.tarul.cn/Article/details/gxektnmcf.sHtML

[R30] 函数返回状态码
来源：http://baike.yfazqb.com/Article/details/gnruictbb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.epnwcf.com/Article/details/gokrlkepz.sHtML

[R31] 局部变量
来源：http://3g.tarul.cn/Article/details/gkbklexon.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.yfazqb.com/Article/details/gyuzoyqre.sHtML

[R32] 参数个数校验
来源：http://3g.epnwcf.com/Article/details/gxvkyvcuy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gfoivozjr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxkuxlhu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.bbcook.cn/Article/details/gqjmcgxox.sHtML

[R34] 退出时清理
来源：http://www.m.share.epnwcf.com/Article/details/guumowpsd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gsrmznrrz.sHtML

[R35] 后台执行并等待
来源：http://mobile.epnwcf.com/Article/details/gzomomtxa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.bbcook.cn/Article/details/ggkslclah.sHtML

[R36] 并发执行多个任务
来源：http://read.share.yfazqb.com/Article/details/giwytjjhc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.epnwcf.com/Article/details/gsovrovti.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.epnwcf.com/Article/details/gulvlxsql.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/gdreythgm.sHtML

[R38] 管道串联
来源：http://wap.sjlbkw.cn/Article/details/gqocnaclx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fktsv.cn/Article/details/gpjzsqfls.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/gkgibtclc.sHtML

cmd > out.log 2>&1
来源：http://blog.sjlbkw.cn/Article/details/gojeshvgj.sHtML

[R40] 追加写日志
来源：http://www.share.epnwcf.com/Article/details/gwbebtoos.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/gmsdczbzn.sHtML

[R41] 丢弃输出
来源：http://mobile.epnwcf.com/Article/details/ghdzqprjg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.tarul.cn/Article/details/gmojnqryp.sHtML

[R42] 输入重定向
来源：http://www.share.bbcook.cn/Article/details/gknmeaxla.sHtML

wc -l < a.txt
来源：http://3g.epnwcf.com/Article/details/gyucwubsw.sHtML

[R43] 按名字查找文件
来源：http://www.share.epnwcf.com/Article/details/gqnunvgim.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.tarul.cn/Article/details/gvsrrqujg.sHtML

[R44] 按修改时间查找
来源：http://wap.tarul.cn/Article/details/gettcqwdw.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/ghwbmckiq.sHtML

[R45] 批量删除
来源：http://www.blog.epnwcf.com/Article/details/ghafxoylh.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.tarul.cn/Article/details/gixvyweed.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.yfazqb.com/Article/details/gjhrorhyg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.epnwcf.com/Article/details/gnirpvuwb.sHtML

[R47] sed 单行替换
来源：http://www.share.vehdjk.com/Article/details/gfmqoyhum.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gnfgugkyb.sHtML

[R48] awk 取指定列
来源：http://blog.yfazqb.com/Article/details/gupvvdqbc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.vehdjk.com/Article/details/geblhleli.sHtML

[R49] awk 带条件
来源：http://wap.tarul.cn/Article/details/ghsfioahu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fktsv.cn/Article/details/gaigjgpde.sHtML

[R50] awk 求和
来源：http://www.blog.vehdjk.com/Article/details/ghhbyburt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.vehdjk.com/Article/details/gffokgwdd.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.epnwcf.com/Article/details/grkoqjted.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.epnwcf.com/Article/details/gpfytoouz.sHtML

[R52] 统计行数
来源：http://m.share.epnwcf.com/Article/details/gyohbetjx.sHtML

wc -l a.txt
来源：http://wap.bbcook.cn/Article/details/gbanoxloz.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.yfazqb.com/Article/details/glalwwxiy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.tarul.cn/Article/details/gfqkizfnx.sHtML

[R54] 比较两个文件
来源：http://www.m.share.epnwcf.com/Article/details/ghhkenbvo.sHtML

diff a.txt b.txt
来源：http://www.share.sjlbkw.cn/Article/details/gkjbhojum.sHtML

[R55] 压缩与解压
来源：http://mobile.vehdjk.com/Article/details/grzzttihz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.bbcook.cn/Article/details/gheatxnsa.sHtML

[R56] 远程拷贝
来源：http://read.share.bbcook.cn/Article/details/gzccqlulj.sHtML

scp file user@host:/path/
来源：http://www.share.yfazqb.com/Article/details/gsjrkqmwv.sHtML

[R57] 远程执行命令
来源：http://mobile.sjlbkw.cn/Article/details/gjljqospj.sHtML

ssh user@host 'uptime'
来源：http://blog.fktsv.cn/Article/details/gwpelxyxl.sHtML

[R58] 下载文件
来源：http://mobile.yfazqb.com/Article/details/gewshyizn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.epnwcf.com/Article/details/gshrjmved.sHtML

[R59] 发 POST JSON
来源：http://3g.vehdjk.com/Article/details/grpcvwxlc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.bbcook.cn/Article/details/ggyqosyvo.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gdxvgnfcs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.yfazqb.com/Article/details/gikwymaxs.sHtML

[R61] 磁盘占用
来源：http://www.share.yfazqb.com/Article/details/gtywmwtyn.sHtML

df -h;  du -sh *
来源：http://www.m.share.yfazqb.com/Article/details/goachyejr.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fktsv.cn/Article/details/gqppcqzxx.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.bbcook.cn/Article/details/gteiawpdw.sHtML

[R63] 内存与进程
来源：http://wap.epnwcf.com/Article/details/gqnatddfe.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.bbcook.cn/Article/details/glqmzcgsj.sHtML

[R64] 结束进程
来源：http://baike.bbcook.cn/Article/details/gbczqhmgv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.yfazqb.com/Article/details/gudrdjmvg.sHtML

[R65] 查看端口占用
来源：http://3g.yfazqb.com/Article/details/grqlkxbah.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.sjlbkw.cn/Article/details/gvqcygfqx.sHtML

[R66] 定时任务
来源：http://m.share.tarul.cn/Article/details/gykdgmuwz.sHtML

crontab -e;  crontab -l
来源：http://baike.tarul.cn/Article/details/gtkfgkevi.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fktsv.cn/Article/details/gobmsftdq.sHtML

openssl rand -hex 16
来源：http://www.blog.epnwcf.com/Article/details/gljqiusqz.sHtML

[R68] 计算文件校验值
来源：http://blog.fktsv.cn/Article/details/gviogqzva.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fktsv.cn/Article/details/gkznfecec.sHtML

[R69] 生成随机密码
来源：http://www.m.share.tarul.cn/Article/details/gahgoenkb.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.epnwcf.com/Article/details/gytlmwzci.sHtML

[R70] 时间戳与互转
来源：http://wap.bbcook.cn/Article/details/ggrxmkoxj.sHtML

date +%s;  date -d @1700000000
来源：http://blog.tarul.cn/Article/details/gpmdzmxjo.sHtML

[R71] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gmnbgkpnj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.yfazqb.com/Article/details/gaqlcfewa.sHtML

[R72] 等待端口就绪
来源：http://read.share.bbcook.cn/Article/details/gxuppqdfy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/gstbmyrws.sHtML

[R73] 分割大日志
来源：http://blog.tarul.cn/Article/details/gatyrfjiy.sHtML

split -l 1000 big.log part_
来源：http://3g.yfazqb.com/Article/details/gvwsskxhs.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/gfwfftymu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.vehdjk.com/Article/details/gfdurslmw.sHtML

[R75] 导出环境变量
来源：http://www.blog.yfazqb.com/Article/details/gzovjxiit.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.sjlbkw.cn/Article/details/gmxpdwiaw.sHtML

[R76] 使用临时文件
来源：http://mobile.yfazqb.com/Article/details/ggmotnain.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gffvjqbpj.sHtML

[R77] 读取用户输入
来源：http://www.blog.fktsv.cn/Article/details/guzqyddzf.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/gmrwnwyfq.sHtML

[R78] 交互式菜单
来源：http://blog.fktsv.cn/Article/details/gaaxugifx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fktsv.cn/Article/details/ggnegiukl.sHtML

[R79] 解析命令行选项
来源：http://wap.bbcook.cn/Article/details/glquviohq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fktsv.cn/Article/details/gxmzseiko.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gfjjrqdvo.sHtML

time ./run.sh
来源：http://mobile.sjlbkw.cn/Article/details/gssfuvrop.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gstnniwpw.sHtML

S. C / C++ 专题
来源：http://www.blog.tarul.cn/Article/details/ggusafiyn.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gptakqmhd.sHtML

[S01] C：Hello World
来源：http://m.share.vehdjk.com/Article/details/gscisldmz.sHtML

#include <stdio.h>
来源：http://m.share.tarul.cn/Article/details/givoczood.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.yfazqb.com/Article/details/gxbbcvnae.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fktsv.cn/Article/details/gdwjyrnmd.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.sjlbkw.cn/Article/details/gxkpreoml.sHtML

[S03] C：读入整数
来源：http://wap.sjlbkw.cn/Article/details/ggvzzmryj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.yfazqb.com/Article/details/gvlscvbwr.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/ghsjjrijm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.vehdjk.com/Article/details/gvghjnpdv.sHtML

[S05] C：字符串长度
来源：http://baike.yfazqb.com/Article/details/greqahmun.sHtML

strlen(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwdhpztr.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/grcjxuhje.sHtML

strcmp(a, b) == 0
来源：http://3g.tarul.cn/Article/details/glqhdfuyf.sHtML

[S07] C：数组遍历求和
来源：http://m.share.vehdjk.com/Article/details/gcmsfuvni.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.vehdjk.com/Article/details/gyilwcsot.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.bbcook.cn/Article/details/ggkvolmvh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.yfazqb.com/Article/details/glsfsugdq.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.sjlbkw.cn/Article/details/ghlkrxcgx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.epnwcf.com/Article/details/gfyvxnzuf.sHtML

[S10] C：指针与解引用
来源：http://mobile.vehdjk.com/Article/details/gnakkonbm.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/gwfamejgs.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gfqzehyvc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.vehdjk.com/Article/details/gquvgykgp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fktsv.cn/Article/details/gpjmxdysw.sHtML

fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gqqlljmeq.sHtML

[S12] C：写文件
来源：http://read.share.tarul.cn/Article/details/glugyiynl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.tarul.cn/Article/details/gcyvjludn.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/gdalrizsd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/giazljhcw.sHtML

[S14] C：枚举
来源：http://mobile.epnwcf.com/Article/details/gwxmlsoyl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fktsv.cn/Article/details/gpfxhkhtu.sHtML

[S15] C：类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gufyjxtuj.sHtML

(double) a / b
来源：http://www.share.fktsv.cn/Article/details/gkwmembhj.sHtML

[S16] C：位操作置位
来源：http://mobile.epnwcf.com/Article/details/glwfxueye.sHtML

x |= (1 << 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gcngiykms.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmwrrafi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.bbcook.cn/Article/details/gfsgphwky.sHtML

[S18] C：命令行参数
来源：http://www.m.share.tarul.cn/Article/details/gkddwassp.sHtML

int main(int argc, char **argv)
来源：http://baike.bbcook.cn/Article/details/ghgkgtmty.sHtML

[S19] C：快速排序
来源：http://www.share.vehdjk.com/Article/details/glsyrlnhi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gxbvubbgo.sHtML

[S20] C：二分查找
来源：http://m.share.sjlbkw.cn/Article/details/ghahqudvc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/gvjbgaxuz.sHtML

[S21] C：字符类别判断
来源：http://3g.vehdjk.com/Article/details/gubipiwyk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.yfazqb.com/Article/details/gzewfxyrm.sHtML

[S22] C：字符串转数字
来源：http://read.share.fktsv.cn/Article/details/gwaompuny.sHtML


<!-- 参考信息 -->