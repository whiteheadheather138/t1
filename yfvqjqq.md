代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gexleyhra.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.epnwcf.com/Article/details/gxxekyfyy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.tarul.cn/Article/details/gpcegczin.sHtML

[Q57] 行号
来源：http://mobile.fktsv.cn/Article/details/gsggnjzqt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.tarul.cn/Article/details/grfzovskd.sHtML

[Q58] 累计求和
来源：http://wap.sjlbkw.cn/Article/details/gevykgqwa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.bbcook.cn/Article/details/ginlaikyf.sHtML

[Q59] 分组内累计
来源：http://read.share.fktsv.cn/Article/details/gqtdkftny.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gmobyaxee.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.vehdjk.com/Article/details/ghsohyvfy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fktsv.cn/Article/details/goudoepdk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gcddcozjj.sHtML

[Q61] 移动平均
来源：http://blog.vehdjk.com/Article/details/geldjjwav.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gwyreiczr.sHtML

[Q62] 分组占比
来源：http://www.blog.sjlbkw.cn/Article/details/gwpqyuobb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gpzsjeixg.sHtML

[Q63] 开启事务
来源：http://mobile.fktsv.cn/Article/details/glphtkwzn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.vehdjk.com/Article/details/gintyuszl.sHtML

[Q64] 提交事务
来源：http://read.share.bbcook.cn/Article/details/glrdzedrz.sHtML

COMMIT;
来源：http://read.share.fktsv.cn/Article/details/giwbyokgn.sHtML

[Q65] 回滚事务
来源：http://baike.tarul.cn/Article/details/glilottbf.sHtML

ROLLBACK;
来源：http://3g.vehdjk.com/Article/details/gepxtnhqo.sHtML

[Q66] 行锁查询
来源：http://3g.sjlbkw.cn/Article/details/gaygrdyzc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.epnwcf.com/Article/details/guxzdfwgd.sHtML

[Q67] 设置隔离级别
来源：http://blog.tarul.cn/Article/details/gueinwjwx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.sjlbkw.cn/Article/details/gzrlglndk.sHtML

[Q68] 保存点
来源：http://www.blog.vehdjk.com/Article/details/gbloujvdt.sHtML

SAVEPOINT sp1;
来源：http://m.share.tarul.cn/Article/details/gnqzpsrbh.sHtML

ROLLBACK TO sp1;
来源：http://baike.fktsv.cn/Article/details/glqfezmvy.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.bbcook.cn/Article/details/gmsixytzh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.epnwcf.com/Article/details/ggnhzcutw.sHtML

[Q70] 更新统计信息
来源：http://blog.epnwcf.com/Article/details/gpmfhjrke.sHtML

ANALYZE TABLE users;
来源：http://blog.sjlbkw.cn/Article/details/gkubceqba.sHtML

[Q71] 查看建表语句
来源：http://baike.fktsv.cn/Article/details/gugbtognf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fktsv.cn/Article/details/gqciyfkwf.sHtML

[Q72] 查看索引
来源：http://m.share.fktsv.cn/Article/details/gkrdtrksr.sHtML

SHOW INDEX FROM users;
来源：http://m.share.yfazqb.com/Article/details/gtcivgtge.sHtML

[Q73] 查看表状态
来源：http://www.share.sjlbkw.cn/Article/details/gwfweijob.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fktsv.cn/Article/details/gimufpnup.sHtML

[Q74] 强制使用索引
来源：http://wap.sjlbkw.cn/Article/details/ghwaoewyo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcufjihc.sHtML

[Q75] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/gqtnhaaxy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.tarul.cn/Article/details/gvbpilzok.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.vehdjk.com/Article/details/gaidqjcjd.sHtML

[Q76] 按天统计
来源：http://baike.tarul.cn/Article/details/gwafpcujq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.sjlbkw.cn/Article/details/gigokoazy.sHtML

[Q77] 时间加减
来源：http://www.blog.sjlbkw.cn/Article/details/ghtyngteo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.bbcook.cn/Article/details/gqtboaopz.sHtML

[Q78] 当前时间
来源：http://3g.vehdjk.com/Article/details/gukqyhusv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.bbcook.cn/Article/details/ghrudefbc.sHtML

[Q79] 字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/glxuvoxsm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/gitdwdzfh.sHtML

[Q80] 字符串截取
来源：http://blog.sjlbkw.cn/Article/details/gcvpoxxib.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gpgrpmwxn.sHtML

[Q81] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gtcouelcr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.tarul.cn/Article/details/glqtrovvx.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.sjlbkw.cn/Article/details/gfdctdlef.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gembpvymv.sHtML

[Q83] 大小写转换
来源：http://wap.yfazqb.com/Article/details/gcdochfwq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gykjayjpb.sHtML

[Q84] 去除首尾空格
来源：http://www.share.tarul.cn/Article/details/grsdxugbd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/guljtajgu.sHtML

[Q85] 数值取整
来源：http://read.share.bbcook.cn/Article/details/gybncupkk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gskzsizhn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gtggcfbwg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.vehdjk.com/Article/details/gbadgxnlr.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fktsv.cn/Article/details/ggpaedtkn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.tarul.cn/Article/details/gnpjhnvhy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.sjlbkw.cn/Article/details/gorxpxvli.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.vehdjk.com/Article/details/gieexspxq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.epnwcf.com/Article/details/gdlzzhqxk.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.epnwcf.com/Article/details/giogmdmik.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.sjlbkw.cn/Article/details/gjmhipuwv.sHtML

[Q90] 生成序号列
来源：http://www.blog.yfazqb.com/Article/details/gibrhzirv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.tarul.cn/Article/details/gqmtqfapj.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gdmlndomu.sHtML

R. Bash 专题
来源：http://www.blog.vehdjk.com/Article/details/geuvmmerd.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gbnxtxnsb.sHtML

[R01] shebang 与严格模式
来源：http://wap.bbcook.cn/Article/details/ggxsnnbix.sHtML

#!/usr/bin/env bash
来源：http://m.share.fktsv.cn/Article/details/gxknweeib.sHtML

set -euo pipefail
来源：http://www.share.epnwcf.com/Article/details/gkayxmnpr.sHtML

[R02] 变量赋值与使用
来源：http://baike.bbcook.cn/Article/details/gqucwlyup.sHtML

name="Tom"; echo "$name"
来源：http://blog.vehdjk.com/Article/details/gbnzoylas.sHtML

[R03] 只读变量
来源：http://blog.yfazqb.com/Article/details/gazuaoetu.sHtML

readonly PI=3.14
来源：http://wap.bbcook.cn/Article/details/gwhsebhdl.sHtML

[R04] 位置参数
来源：http://read.share.bbcook.cn/Article/details/gdyaibiwc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.bbcook.cn/Article/details/gzmqssmto.sHtML

[R05] 参数默认值
来源：http://www.share.sjlbkw.cn/Article/details/gauizxnjz.sHtML

name="${1:-default}"
来源：http://3g.bbcook.cn/Article/details/gkshddgty.sHtML

[R06] 判断命令是否存在
来源：http://read.share.sjlbkw.cn/Article/details/giownilxi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/gmewqpgec.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gerzglhzf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gqeejywzc.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/gieapxewh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.tarul.cn/Article/details/gxstxsixf.sHtML

[R09] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/glxthiduf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.vehdjk.com/Article/details/gblrfjbwt.sHtML

[R10] 正则匹配
来源：http://3g.vehdjk.com/Article/details/gskwzwewv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.tarul.cn/Article/details/gvgkebite.sHtML

[R11] case 多分支
来源：http://www.share.vehdjk.com/Article/details/guupezckd.sHtML

case "$1" in
来源：http://www.blog.vehdjk.com/Article/details/gjsfykicz.sHtML

start) echo "启动" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gcitordzm.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gmazxqsco.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fktsv.cn/Article/details/gstftxpax.sHtML

esac
来源：http://www.blog.vehdjk.com/Article/details/geezetazb.sHtML

[R12] for 遍历文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwictymw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.sjlbkw.cn/Article/details/gokbrcrcq.sHtML

[R13] for 计数循环
来源：http://m.share.sjlbkw.cn/Article/details/gobqcvwuq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gzpnlnaoa.sHtML

[R14] C 风格 for
来源：http://read.share.fktsv.cn/Article/details/ggikcuizs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/ghgjxusjd.sHtML

[R15] while 逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gnuhedeob.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.bbcook.cn/Article/details/gwzgerprb.sHtML

[R16] until 等待条件
来源：http://read.share.fktsv.cn/Article/details/gmevjqhoj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gmyexfusv.sHtML

[R17] 数组定义与取值
来源：http://wap.epnwcf.com/Article/details/glghvomgj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.epnwcf.com/Article/details/ghhaecicc.sHtML

[R18] 遍历数组
来源：http://read.share.yfazqb.com/Article/details/gopyeoawu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fktsv.cn/Article/details/gxcpnxeso.sHtML

[R19] 数组长度
来源：http://wap.vehdjk.com/Article/details/gnwxblqci.sHtML

echo "${#arr[@]}"
来源：http://mobile.sjlbkw.cn/Article/details/gjpldzefp.sHtML

[R20] 关联数组（字典）
来源：http://www.share.bbcook.cn/Article/details/gdtgcotkt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.tarul.cn/Article/details/gzoolzwhj.sHtML

[R21] 字符串长度
来源：http://m.share.vehdjk.com/Article/details/giwxpuipb.sHtML

echo "${#s}"
来源：http://baike.bbcook.cn/Article/details/gocsrptnw.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/gdtjiwtvn.sHtML

echo "${s:0:5}"
来源：http://m.share.sjlbkw.cn/Article/details/gpqqynwci.sHtML

[R23] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/gmvmzulcn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.bbcook.cn/Article/details/geuwhlmxu.sHtML

[R24] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gzkxcnhur.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.tarul.cn/Article/details/gxlfnbcmj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.bbcook.cn/Article/details/gtybbqbmr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.epnwcf.com/Article/details/gdwudnnug.sHtML

[R26] 命令替换
来源：http://baike.epnwcf.com/Article/details/gfborclmy.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.bbcook.cn/Article/details/gnusrazux.sHtML

[R27] 算术展开
来源：http://www.share.vehdjk.com/Article/details/gjwamcljs.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.epnwcf.com/Article/details/gpvvqwuvw.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gshhqkosv.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.tarul.cn/Article/details/gwziqqbij.sHtML

[R29] 定义函数
来源：http://read.share.sjlbkw.cn/Article/details/ggwtwkjii.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.yfazqb.com/Article/details/ggtagoofa.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/gvzrjwgqk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.bbcook.cn/Article/details/gpvjsqhij.sHtML

[R31] 局部变量
来源：http://www.blog.tarul.cn/Article/details/ghjyxlzbn.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.tarul.cn/Article/details/gyjwlrcbd.sHtML

[R32] 参数个数校验
来源：http://wap.fktsv.cn/Article/details/grajovqpn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/guioqhtdh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.epnwcf.com/Article/details/gjoyomlmy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fktsv.cn/Article/details/gzqogqrjv.sHtML

[R34] 退出时清理
来源：http://www.m.share.sjlbkw.cn/Article/details/gobvsjwro.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gxwmccbli.sHtML

[R35] 后台执行并等待
来源：http://m.share.epnwcf.com/Article/details/gapwjmyes.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.yfazqb.com/Article/details/ghyzodtbs.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fktsv.cn/Article/details/gsdvcbsxc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.yfazqb.com/Article/details/ghnyrxojc.sHtML

[R37] 把输出赋给变量
来源：http://blog.yfazqb.com/Article/details/ghgxnmulr.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/guhdzcpbh.sHtML

[R38] 管道串联
来源：http://3g.epnwcf.com/Article/details/gvpnxwwpq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.vehdjk.com/Article/details/gojrnmzcm.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.sjlbkw.cn/Article/details/gogjyhyxl.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gshklsdhd.sHtML

[R40] 追加写日志
来源：http://mobile.vehdjk.com/Article/details/glfseuvtw.sHtML

echo "log" >> out.log
来源：http://3g.fktsv.cn/Article/details/goswoosmn.sHtML

[R41] 丢弃输出
来源：http://wap.yfazqb.com/Article/details/gjusywtlb.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gqbtpmxqa.sHtML

[R42] 输入重定向
来源：http://mobile.yfazqb.com/Article/details/gwfxkdskv.sHtML

wc -l < a.txt
来源：http://mobile.tarul.cn/Article/details/grfvjqgiv.sHtML

[R43] 按名字查找文件
来源：http://wap.fktsv.cn/Article/details/gdelmoaif.sHtML

find . -name "*.log" -type f
来源：http://mobile.vehdjk.com/Article/details/gskghjfuw.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/gympawwpu.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/ghdxzgxvr.sHtML

[R45] 批量删除
来源：http://wap.yfazqb.com/Article/details/gskjhpadd.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/gucbjzgbt.sHtML

[R46] 递归替换文件内容
来源：http://baike.yfazqb.com/Article/details/gurkyrmzt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbbbzipo.sHtML

[R47] sed 单行替换
来源：http://www.blog.yfazqb.com/Article/details/gucpfcrme.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/ggdpenrha.sHtML

[R48] awk 取指定列
来源：http://mobile.fktsv.cn/Article/details/gmkpblegx.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fktsv.cn/Article/details/goswrfeww.sHtML

[R49] awk 带条件
来源：http://www.share.sjlbkw.cn/Article/details/gdvrneahi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.tarul.cn/Article/details/gocntidrs.sHtML

[R50] awk 求和
来源：http://wap.bbcook.cn/Article/details/gpkzipjac.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gzdrpnrwn.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.vehdjk.com/Article/details/ggfaldeht.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.epnwcf.com/Article/details/gkuruinst.sHtML

[R52] 统计行数
来源：http://www.share.tarul.cn/Article/details/gtpnrgjjt.sHtML

wc -l a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gpurikfnx.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.sjlbkw.cn/Article/details/grniygvzw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.tarul.cn/Article/details/gtvikwxsw.sHtML

[R54] 比较两个文件
来源：http://baike.fktsv.cn/Article/details/gemrawtha.sHtML

diff a.txt b.txt
来源：http://read.share.fktsv.cn/Article/details/gpgegwxbm.sHtML

[R55] 压缩与解压
来源：http://read.share.epnwcf.com/Article/details/glzkgcvgl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.tarul.cn/Article/details/gbqeczufh.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/getbkounm.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/gdtvrrlua.sHtML

[R57] 远程执行命令
来源：http://www.blog.bbcook.cn/Article/details/gzrjhvgkx.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/gjfpliddw.sHtML

[R58] 下载文件
来源：http://www.m.share.tarul.cn/Article/details/guzvcmvoh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fktsv.cn/Article/details/gyycwukwy.sHtML

[R59] 发 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/grseojcar.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.tarul.cn/Article/details/gaenwikdt.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gvolqnuip.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.epnwcf.com/Article/details/gsccdypfq.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/gxqhmjtaa.sHtML

df -h;  du -sh *
来源：http://www.m.share.fktsv.cn/Article/details/ghzsjwyih.sHtML

[R62] 找最占空间的文件
来源：http://mobile.yfazqb.com/Article/details/godcojsjl.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.sjlbkw.cn/Article/details/gyuvhwkcp.sHtML

[R63] 内存与进程
来源：http://www.blog.tarul.cn/Article/details/goppgboii.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/gkhmgxzax.sHtML

[R64] 结束进程
来源：http://m.share.epnwcf.com/Article/details/gakcidbbd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gvqgemfgz.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/gtijirxxp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.vehdjk.com/Article/details/gnoxepwyp.sHtML

[R66] 定时任务
来源：http://blog.yfazqb.com/Article/details/gczwggqnb.sHtML

crontab -e;  crontab -l
来源：http://read.share.yfazqb.com/Article/details/gblbdszjq.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fktsv.cn/Article/details/gcoerwczq.sHtML

openssl rand -hex 16
来源：http://read.share.fktsv.cn/Article/details/gjetqealr.sHtML

[R68] 计算文件校验值
来源：http://3g.vehdjk.com/Article/details/gelqtezly.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.epnwcf.com/Article/details/ghkuzuafb.sHtML

[R69] 生成随机密码
来源：http://m.share.sjlbkw.cn/Article/details/gbdutgsgo.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/gdyxkpnmr.sHtML

[R70] 时间戳与互转
来源：http://wap.tarul.cn/Article/details/ggfsbhyqh.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.tarul.cn/Article/details/gzzkfkeyt.sHtML

[R71] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gfundibgu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.vehdjk.com/Article/details/gkcmwqwas.sHtML

[R72] 等待端口就绪
来源：http://wap.epnwcf.com/Article/details/gwpsanidg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gnqcnmszl.sHtML

[R73] 分割大日志
来源：http://mobile.tarul.cn/Article/details/gihinvmxs.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gnwmhptkt.sHtML

[R74] 批量重命名
来源：http://m.share.fktsv.cn/Article/details/gfbcbvurk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.sjlbkw.cn/Article/details/gcaoygqee.sHtML

[R75] 导出环境变量
来源：http://blog.bbcook.cn/Article/details/gojedohkx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.bbcook.cn/Article/details/gqtfyjwwi.sHtML

[R76] 使用临时文件
来源：http://www.share.bbcook.cn/Article/details/godiivroc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gmsilmexg.sHtML

[R77] 读取用户输入
来源：http://www.share.tarul.cn/Article/details/gypqeulqr.sHtML

read -rp "请输入: " ans
来源：http://blog.yfazqb.com/Article/details/gsrfhrlre.sHtML

[R78] 交互式菜单
来源：http://mobile.vehdjk.com/Article/details/gimgykzbi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.epnwcf.com/Article/details/goekphwbn.sHtML

[R79] 解析命令行选项
来源：http://baike.bbcook.cn/Article/details/gpwvycuzp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.sjlbkw.cn/Article/details/gkxghyfxz.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.yfazqb.com/Article/details/ghdeqdgrp.sHtML

time ./run.sh
来源：http://m.share.bbcook.cn/Article/details/gsjzoizrr.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gfczekctq.sHtML

S. C / C++ 专题
来源：http://www.share.bbcook.cn/Article/details/gbzitymun.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxasepqyc.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/gsukuvrgh.sHtML

#include <stdio.h>
来源：http://www.share.fktsv.cn/Article/details/gpywlcaaa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fktsv.cn/Article/details/gfctyrxvb.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.vehdjk.com/Article/details/ghugruzel.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.epnwcf.com/Article/details/gnsshdaxe.sHtML

[S03] C：读入整数
来源：http://www.share.yfazqb.com/Article/details/gacqqxfei.sHtML

int x; scanf("%d", &x);
来源：http://mobile.bbcook.cn/Article/details/gitotzchs.sHtML

[S04] C：字符串复制
来源：http://3g.bbcook.cn/Article/details/gfnkvtoeb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gskgyvcdw.sHtML

[S05] C：字符串长度
来源：http://read.share.epnwcf.com/Article/details/gzfhifmjr.sHtML

strlen(s)
来源：http://baike.epnwcf.com/Article/details/gdiztnrgm.sHtML

[S06] C：字符串比较
来源：http://wap.fktsv.cn/Article/details/gqkyrmlkv.sHtML

strcmp(a, b) == 0
来源：http://www.share.sjlbkw.cn/Article/details/gnnhgjplq.sHtML

[S07] C：数组遍历求和
来源：http://baike.epnwcf.com/Article/details/gklukpnqk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.sjlbkw.cn/Article/details/gkvaeimdn.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.bbcook.cn/Article/details/gtkvrewie.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.bbcook.cn/Article/details/gffgvmarl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.tarul.cn/Article/details/gugqnhgwz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/geatzmwva.sHtML

[S10] C：指针与解引用
来源：http://3g.sjlbkw.cn/Article/details/genaqvxhx.sHtML

int *p = &a;  *p = 5;
来源：http://blog.sjlbkw.cn/Article/details/gcwwelcoa.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gyzmydbfd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.bbcook.cn/Article/details/glxfidqhu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.tarul.cn/Article/details/gyxgyzdkd.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gmrsqdztw.sHtML

[S12] C：写文件
来源：http://www.share.epnwcf.com/Article/details/gwicigwbv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.vehdjk.com/Article/details/gojwtuiej.sHtML

[S13] C：宏定义
来源：http://blog.bbcook.cn/Article/details/gpqnxltat.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.epnwcf.com/Article/details/gjfwypbos.sHtML

[S14] C：枚举
来源：http://blog.tarul.cn/Article/details/gnqqfydez.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fktsv.cn/Article/details/gzxjtllzm.sHtML

[S15] C：类型转换
来源：http://www.share.vehdjk.com/Article/details/gibxbovcr.sHtML

(double) a / b
来源：http://mobile.yfazqb.com/Article/details/gthgqmlxh.sHtML

[S16] C：位操作置位
来源：http://www.share.bbcook.cn/Article/details/gxccwwmox.sHtML

x |= (1 << 3);
来源：http://m.share.sjlbkw.cn/Article/details/gfssugual.sHtML

[S17] C：安全拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/garvhitdg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.yfazqb.com/Article/details/ggxnhqgyt.sHtML

[S18] C：命令行参数
来源：http://read.share.fktsv.cn/Article/details/galsvyeig.sHtML

int main(int argc, char **argv)
来源：http://read.share.bbcook.cn/Article/details/gdbyzowvx.sHtML

[S19] C：快速排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkgbbyaz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/gwsmhoioi.sHtML

[S20] C：二分查找
来源：http://mobile.sjlbkw.cn/Article/details/gbnozvyic.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gkijgdjqy.sHtML

[S21] C：字符类别判断
来源：http://www.blog.epnwcf.com/Article/details/gekhnnijn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.vehdjk.com/Article/details/gnhtoxyqs.sHtML

[S22] C：字符串转数字
来源：http://baike.fktsv.cn/Article/details/gtyoamhvi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/gduijpmbi.sHtML

[S23] C：随机数
来源：http://m.share.vehdjk.com/Article/details/gdvqxjazh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.tarul.cn/Article/details/gxwtduhmm.sHtML

[S24] C：获取本地时间
来源：http://baike.bbcook.cn/Article/details/gzekyujxz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.yfazqb.com/Article/details/gmaqnnlvi.sHtML

[S25] C：内存拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gibnlaaoy.sHtML

memcpy(dst, src, n);
来源：http://blog.epnwcf.com/Article/details/gqtyqjvmd.sHtML

[S26] C：内存清零
来源：http://m.share.sjlbkw.cn/Article/details/gzgdxdjua.sHtML


<!-- 参考信息 -->