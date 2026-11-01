代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gsldoawgh.sHtML

[Q50] 批量更新
来源：http://baike.fktsv.cn/Article/details/gofjaaelx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.yfazqb.com/Article/details/gyewkjssn.sHtML

[Q51] 用子查询更新
来源：http://3g.bbcook.cn/Article/details/ghponwtdg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxkoilcf.sHtML

[Q52] 删除指定行
来源：http://www.m.share.tarul.cn/Article/details/gditbcjuh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/gjbupuyvs.sHtML

[Q53] 按条件删除
来源：http://3g.tarul.cn/Article/details/gwnjoaeuf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.tarul.cn/Article/details/gbluhukpk.sHtML

[Q54] 清空表
来源：http://read.share.fktsv.cn/Article/details/ggyqrsjwt.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fktsv.cn/Article/details/gxjkkcckn.sHtML

[Q55] 排名（并列占位）
来源：http://blog.vehdjk.com/Article/details/gquzuxsjr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkazsuhz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fktsv.cn/Article/details/gvrshuwsh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gojaakwxi.sHtML

[Q57] 行号
来源：http://www.share.fktsv.cn/Article/details/gyplrmftb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.yfazqb.com/Article/details/glebhhucd.sHtML

[Q58] 累计求和
来源：http://m.share.vehdjk.com/Article/details/gdqmtavrb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.vehdjk.com/Article/details/gcukndlca.sHtML

[Q59] 分组内累计
来源：http://www.share.sjlbkw.cn/Article/details/gddkbuqtb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/glhcqmtyw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.bbcook.cn/Article/details/guhzgaefz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.sjlbkw.cn/Article/details/gueeobogq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.bbcook.cn/Article/details/ghuuvbluh.sHtML

[Q61] 移动平均
来源：http://mobile.vehdjk.com/Article/details/gegeomhqb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/grlagkurr.sHtML

[Q62] 分组占比
来源：http://www.blog.tarul.cn/Article/details/glcwxzqxf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gwjawrzoa.sHtML

[Q63] 开启事务
来源：http://mobile.yfazqb.com/Article/details/gnfsiodpv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.epnwcf.com/Article/details/gntrcobsw.sHtML

[Q64] 提交事务
来源：http://www.blog.fktsv.cn/Article/details/ghipwdphe.sHtML

COMMIT;
来源：http://baike.fktsv.cn/Article/details/gkkaxoqqd.sHtML

[Q65] 回滚事务
来源：http://read.share.vehdjk.com/Article/details/gxsukhtoj.sHtML

ROLLBACK;
来源：http://wap.vehdjk.com/Article/details/geywzwhsm.sHtML

[Q66] 行锁查询
来源：http://3g.yfazqb.com/Article/details/gesqsoubv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.yfazqb.com/Article/details/gbzbhlbcz.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.epnwcf.com/Article/details/gfovijsej.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.bbcook.cn/Article/details/gynozkqfn.sHtML

[Q68] 保存点
来源：http://mobile.sjlbkw.cn/Article/details/greeskiql.sHtML

SAVEPOINT sp1;
来源：http://m.share.yfazqb.com/Article/details/gmhniqayh.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.bbcook.cn/Article/details/gaeozgkor.sHtML

[Q69] 查看执行计划
来源：http://m.share.vehdjk.com/Article/details/gxnwaebhn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.epnwcf.com/Article/details/gemuodkgz.sHtML

[Q70] 更新统计信息
来源：http://3g.tarul.cn/Article/details/gisfxkiif.sHtML

ANALYZE TABLE users;
来源：http://baike.yfazqb.com/Article/details/gjvwibmec.sHtML

[Q71] 查看建表语句
来源：http://3g.epnwcf.com/Article/details/gijibhhzy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.epnwcf.com/Article/details/glzbughhe.sHtML

[Q72] 查看索引
来源：http://3g.vehdjk.com/Article/details/gizpygidh.sHtML

SHOW INDEX FROM users;
来源：http://3g.yfazqb.com/Article/details/ggwtldpkl.sHtML

[Q73] 查看表状态
来源：http://www.blog.sjlbkw.cn/Article/details/gwthwygex.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fktsv.cn/Article/details/gfnfefgvi.sHtML

[Q74] 强制使用索引
来源：http://read.share.fktsv.cn/Article/details/gwnskycyt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.vehdjk.com/Article/details/gnbfjaotu.sHtML

[Q75] 日期格式化
来源：http://baike.epnwcf.com/Article/details/gorlphlsp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gkhagpicb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.yfazqb.com/Article/details/gnzufybbw.sHtML

[Q76] 按天统计
来源：http://read.share.bbcook.cn/Article/details/gspurrjsi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fktsv.cn/Article/details/graygoijg.sHtML

[Q77] 时间加减
来源：http://www.share.vehdjk.com/Article/details/gilxsmvgo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.epnwcf.com/Article/details/gbmasjcru.sHtML

[Q78] 当前时间
来源：http://www.share.sjlbkw.cn/Article/details/gsneeptkm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.yfazqb.com/Article/details/gasbyxhdz.sHtML

[Q79] 字符串拼接
来源：http://blog.vehdjk.com/Article/details/grepuwydu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fktsv.cn/Article/details/gkvwrzipw.sHtML

[Q80] 字符串截取
来源：http://baike.yfazqb.com/Article/details/gvkuiikuq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gndqsjjoh.sHtML

[Q81] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gfqeadlkk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.tarul.cn/Article/details/gdqavssxb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.epnwcf.com/Article/details/ghoeyjfqa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gxoxudqfw.sHtML

[Q83] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gtlamcfoo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gsacegeds.sHtML

[Q84] 去除首尾空格
来源：http://wap.yfazqb.com/Article/details/gnvrpdkhj.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/garuuzvzf.sHtML

[Q85] 数值取整
来源：http://baike.tarul.cn/Article/details/gfzojvftu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.epnwcf.com/Article/details/gmzqcguay.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.sjlbkw.cn/Article/details/gltvppsdb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.tarul.cn/Article/details/gsdyzzoza.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.tarul.cn/Article/details/gtbyjruhh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.bbcook.cn/Article/details/gzdyjhmom.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.epnwcf.com/Article/details/gwidopdez.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.epnwcf.com/Article/details/gribrnjpt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.bbcook.cn/Article/details/gvxkrglxu.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gthogdaea.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.bbcook.cn/Article/details/gkyqpahjb.sHtML

[Q90] 生成序号列
来源：http://m.share.fktsv.cn/Article/details/gwmataypt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fktsv.cn/Article/details/gcinmoslu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghnaxrqzm.sHtML

R. Bash 专题
来源：http://read.share.yfazqb.com/Article/details/gpzzlxewt.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gugfncvpl.sHtML

[R01] shebang 与严格模式
来源：http://wap.fktsv.cn/Article/details/gpxqntlbs.sHtML

#!/usr/bin/env bash
来源：http://www.share.sjlbkw.cn/Article/details/gbxdkhgsi.sHtML

set -euo pipefail
来源：http://read.share.fktsv.cn/Article/details/gqfgqzeks.sHtML

[R02] 变量赋值与使用
来源：http://3g.sjlbkw.cn/Article/details/gaqzobqwt.sHtML

name="Tom"; echo "$name"
来源：http://3g.bbcook.cn/Article/details/ganvhdujr.sHtML

[R03] 只读变量
来源：http://www.m.share.epnwcf.com/Article/details/gzzyfofxs.sHtML

readonly PI=3.14
来源：http://3g.yfazqb.com/Article/details/gfjtentlc.sHtML

[R04] 位置参数
来源：http://www.m.share.vehdjk.com/Article/details/gbspydiuk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.tarul.cn/Article/details/gwhicuroe.sHtML

[R05] 参数默认值
来源：http://3g.fktsv.cn/Article/details/gbfjtgvhi.sHtML

name="${1:-default}"
来源：http://www.m.share.fktsv.cn/Article/details/ghueyawhf.sHtML

[R06] 判断命令是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gdapfcgxe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gvzhxblxb.sHtML

[R07] if 判断文件
来源：http://wap.sjlbkw.cn/Article/details/gvxtdrgrk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gzqgnvkfw.sHtML

[R08] 数值比较
来源：http://m.share.tarul.cn/Article/details/gjphwbqzv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.bbcook.cn/Article/details/gberidkle.sHtML

[R09] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gwmigypku.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.bbcook.cn/Article/details/gwlvxyuyq.sHtML

[R10] 正则匹配
来源：http://m.share.epnwcf.com/Article/details/gttgincqj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.vehdjk.com/Article/details/gceunvdwl.sHtML

[R11] case 多分支
来源：http://www.blog.yfazqb.com/Article/details/gnjqxgsqs.sHtML

case "$1" in
来源：http://3g.sjlbkw.cn/Article/details/gbbikhyib.sHtML

start) echo "启动" ;;
来源：http://3g.tarul.cn/Article/details/gtpcahhcz.sHtML

stop)  echo "停止" ;;
来源：http://baike.fktsv.cn/Article/details/gpnhchmdz.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.tarul.cn/Article/details/golupjefn.sHtML

esac
来源：http://blog.bbcook.cn/Article/details/gdaciuhfi.sHtML

[R12] for 遍历文件
来源：http://blog.tarul.cn/Article/details/gmygqsbod.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.sjlbkw.cn/Article/details/gdfinudki.sHtML

[R13] for 计数循环
来源：http://www.m.share.fktsv.cn/Article/details/gkxyqyrxi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.bbcook.cn/Article/details/gnzphbivc.sHtML

[R14] C 风格 for
来源：http://mobile.yfazqb.com/Article/details/guszxirqx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/gygfqrird.sHtML

[R15] while 逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gpmbyziyi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.sjlbkw.cn/Article/details/gfxnougkz.sHtML

[R16] until 等待条件
来源：http://m.share.bbcook.cn/Article/details/gwampwltc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gpmmstabz.sHtML

[R17] 数组定义与取值
来源：http://read.share.bbcook.cn/Article/details/gzwhmjvni.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.vehdjk.com/Article/details/gkppqlhwu.sHtML

[R18] 遍历数组
来源：http://blog.sjlbkw.cn/Article/details/gayegielk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.yfazqb.com/Article/details/gvflgynyg.sHtML

[R19] 数组长度
来源：http://mobile.epnwcf.com/Article/details/gzpiaipac.sHtML

echo "${#arr[@]}"
来源：http://wap.epnwcf.com/Article/details/gjlnklmcu.sHtML

[R20] 关联数组（字典）
来源：http://mobile.epnwcf.com/Article/details/gkpdysiok.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.vehdjk.com/Article/details/gpzpckytn.sHtML

[R21] 字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gpnzxgopn.sHtML

echo "${#s}"
来源：http://mobile.bbcook.cn/Article/details/glcmlmebq.sHtML

[R22] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gfondnrvc.sHtML

echo "${s:0:5}"
来源：http://m.share.sjlbkw.cn/Article/details/gbavhhmdr.sHtML

[R23] 字符串替换
来源：http://read.share.tarul.cn/Article/details/gyvkhsuyd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.sjlbkw.cn/Article/details/gzbekhkee.sHtML

[R24] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gxcfxxncx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.yfazqb.com/Article/details/glhxbzsfq.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fktsv.cn/Article/details/gxsulscco.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.tarul.cn/Article/details/gdmkzkzmt.sHtML

[R26] 命令替换
来源：http://www.blog.fktsv.cn/Article/details/gjabrpykk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjniqcly.sHtML

[R27] 算术展开
来源：http://m.share.fktsv.cn/Article/details/gbkbdtztq.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fktsv.cn/Article/details/glmhzvgho.sHtML

[R28] 浮点运算
来源：http://3g.epnwcf.com/Article/details/glwcgtniu.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/gnnwryeay.sHtML

[R29] 定义函数
来源：http://baike.fktsv.cn/Article/details/grtrphfmx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.yfazqb.com/Article/details/gkllabchi.sHtML

[R30] 函数返回状态码
来源：http://read.share.bbcook.cn/Article/details/geounntov.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.yfazqb.com/Article/details/gvhqwdkcs.sHtML

[R31] 局部变量
来源：http://read.share.tarul.cn/Article/details/gftcqwjqw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/gxwkrbopw.sHtML

[R32] 参数个数校验
来源：http://www.m.share.vehdjk.com/Article/details/gpdfcdjqb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gtecqrcxb.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.epnwcf.com/Article/details/gzefrknrh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.epnwcf.com/Article/details/gagulfpjf.sHtML

[R34] 退出时清理
来源：http://blog.fktsv.cn/Article/details/gznqiwnae.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gqybtibvx.sHtML

[R35] 后台执行并等待
来源：http://m.share.vehdjk.com/Article/details/gadwajnlh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gfrxbuaiu.sHtML

[R36] 并发执行多个任务
来源：http://mobile.bbcook.cn/Article/details/gcnibzcgr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/gjisjcmcd.sHtML

[R37] 把输出赋给变量
来源：http://www.share.sjlbkw.cn/Article/details/glrqnfyie.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/gmemjycij.sHtML

[R38] 管道串联
来源：http://www.share.vehdjk.com/Article/details/gdjlbzjic.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.bbcook.cn/Article/details/gxewkhoqs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fktsv.cn/Article/details/gourmcgis.sHtML

cmd > out.log 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gsxrvpwyu.sHtML

[R40] 追加写日志
来源：http://baike.tarul.cn/Article/details/gdcjtdyjg.sHtML

echo "log" >> out.log
来源：http://m.share.fktsv.cn/Article/details/gvpxpchuz.sHtML

[R41] 丢弃输出
来源：http://read.share.bbcook.cn/Article/details/gfmokvbjk.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.bbcook.cn/Article/details/ghpokvxiu.sHtML

[R42] 输入重定向
来源：http://3g.fktsv.cn/Article/details/gmcbgiqbj.sHtML

wc -l < a.txt
来源：http://wap.fktsv.cn/Article/details/gvtzxddya.sHtML

[R43] 按名字查找文件
来源：http://baike.tarul.cn/Article/details/gvyhonupg.sHtML

find . -name "*.log" -type f
来源：http://3g.sjlbkw.cn/Article/details/gafodbzqb.sHtML

[R44] 按修改时间查找
来源：http://read.share.tarul.cn/Article/details/gkgnkyrle.sHtML

find . -mtime -7 -type f
来源：http://wap.vehdjk.com/Article/details/goxtevtsd.sHtML

[R45] 批量删除
来源：http://blog.vehdjk.com/Article/details/gbvpkerbu.sHtML

find . -name "*.tmp" -delete
来源：http://blog.tarul.cn/Article/details/grjozkyus.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.sjlbkw.cn/Article/details/gopmfmxdq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.tarul.cn/Article/details/gpsmfzxkz.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/ghuurjzgm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.epnwcf.com/Article/details/gopuljobg.sHtML

[R48] awk 取指定列
来源：http://mobile.yfazqb.com/Article/details/grreowxli.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fktsv.cn/Article/details/gzxummjpr.sHtML

[R49] awk 带条件
来源：http://mobile.bbcook.cn/Article/details/gazeasohn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.bbcook.cn/Article/details/gurvvjiqd.sHtML

[R50] awk 求和
来源：http://read.share.tarul.cn/Article/details/ghztgrxwa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gciicoici.sHtML

[R51] 排序去重取前几
来源：http://wap.bbcook.cn/Article/details/gbzplscvl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.bbcook.cn/Article/details/gxsbyysve.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/gpuxgftmr.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/gpwpwlnqb.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.vehdjk.com/Article/details/glkdnfxeh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.yfazqb.com/Article/details/ghjuktpik.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/gsnjduogv.sHtML

diff a.txt b.txt
来源：http://mobile.fktsv.cn/Article/details/grapraltd.sHtML

[R55] 压缩与解压
来源：http://www.m.share.tarul.cn/Article/details/gfbnwrnng.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.vehdjk.com/Article/details/grajimtxp.sHtML

[R56] 远程拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gfcyotcgq.sHtML

scp file user@host:/path/
来源：http://baike.tarul.cn/Article/details/ggydvdouh.sHtML

[R57] 远程执行命令
来源：http://read.share.fktsv.cn/Article/details/gsmwhaqho.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/gpeqbdpla.sHtML

[R58] 下载文件
来源：http://wap.sjlbkw.cn/Article/details/grodfiyuo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fktsv.cn/Article/details/givcpmrwo.sHtML

[R59] 发 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gjdbolcig.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.tarul.cn/Article/details/gmhcddoep.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gzvrdiarw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.epnwcf.com/Article/details/glgrjldvw.sHtML

[R61] 磁盘占用
来源：http://read.share.sjlbkw.cn/Article/details/gxopwwzdv.sHtML

df -h;  du -sh *
来源：http://read.share.fktsv.cn/Article/details/giekudojd.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.yfazqb.com/Article/details/gppvooxvl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.epnwcf.com/Article/details/gbdernfdt.sHtML

[R63] 内存与进程
来源：http://3g.fktsv.cn/Article/details/gtivnnsqt.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.vehdjk.com/Article/details/ggzlahzvs.sHtML

[R64] 结束进程
来源：http://blog.yfazqb.com/Article/details/gcxothwpc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.bbcook.cn/Article/details/gwgilwpky.sHtML

[R65] 查看端口占用
来源：http://www.blog.bbcook.cn/Article/details/gkngvjicb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.bbcook.cn/Article/details/gbeksqabz.sHtML

[R66] 定时任务
来源：http://baike.yfazqb.com/Article/details/grltdbxkx.sHtML

crontab -e;  crontab -l
来源：http://mobile.fktsv.cn/Article/details/gyqkmdbxj.sHtML

[R67] 生成随机十六进制串
来源：http://blog.vehdjk.com/Article/details/gissnmrgu.sHtML

openssl rand -hex 16
来源：http://read.share.tarul.cn/Article/details/guqkdyvge.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/gtafrrrkz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.bbcook.cn/Article/details/grgloplyn.sHtML

[R69] 生成随机密码
来源：http://m.share.bbcook.cn/Article/details/gnutlmrxp.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.tarul.cn/Article/details/gyjybmwtc.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fktsv.cn/Article/details/gyepxlqun.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.epnwcf.com/Article/details/gxfajeeiw.sHtML

[R71] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/gfeulcudt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.epnwcf.com/Article/details/gpflqocom.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gqhvemvjc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/gufayzswv.sHtML

[R73] 分割大日志
来源：http://www.blog.bbcook.cn/Article/details/gdzoxukdh.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/grjgixnri.sHtML

[R74] 批量重命名
来源：http://m.share.vehdjk.com/Article/details/gxxsgkedz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fktsv.cn/Article/details/ggvpozaaz.sHtML

[R75] 导出环境变量
来源：http://www.blog.epnwcf.com/Article/details/gsrbhihiw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.tarul.cn/Article/details/gmsmbbocx.sHtML

[R76] 使用临时文件
来源：http://blog.yfazqb.com/Article/details/gwlxzzqok.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gwmfxrbdo.sHtML

[R77] 读取用户输入
来源：http://read.share.tarul.cn/Article/details/ghwpnkruj.sHtML

read -rp "请输入: " ans
来源：http://mobile.epnwcf.com/Article/details/gxfovqklv.sHtML

[R78] 交互式菜单
来源：http://baike.bbcook.cn/Article/details/gxdrghhtb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gvempixcq.sHtML

[R79] 解析命令行选项
来源：http://www.blog.vehdjk.com/Article/details/guuefbdxz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.vehdjk.com/Article/details/gxykiqflh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.bbcook.cn/Article/details/gmszkdagc.sHtML

time ./run.sh
来源：http://mobile.tarul.cn/Article/details/gzfuufcjn.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gjnerafve.sHtML

S. C / C++ 专题
来源：http://m.share.fktsv.cn/Article/details/gbhjetife.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glzoqmcts.sHtML

[S01] C：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gxblshije.sHtML

#include <stdio.h>
来源：http://wap.sjlbkw.cn/Article/details/gafsjrkti.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fktsv.cn/Article/details/gmydegyeo.sHtML

[S02] C：变量与格式化输出
来源：http://blog.vehdjk.com/Article/details/gmcsrlxkj.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.sjlbkw.cn/Article/details/gcyleczzx.sHtML

[S03] C：读入整数
来源：http://www.blog.tarul.cn/Article/details/gvrfqgyox.sHtML

int x; scanf("%d", &x);
来源：http://baike.bbcook.cn/Article/details/ghbzcfava.sHtML

[S04] C：字符串复制
来源：http://read.share.vehdjk.com/Article/details/gphhpwkxu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.epnwcf.com/Article/details/gxcobdxty.sHtML

[S05] C：字符串长度
来源：http://mobile.fktsv.cn/Article/details/gufpbumcy.sHtML

strlen(s)
来源：http://mobile.yfazqb.com/Article/details/gahewwquj.sHtML

[S06] C：字符串比较
来源：http://www.share.tarul.cn/Article/details/gsgtbculq.sHtML

strcmp(a, b) == 0
来源：http://wap.tarul.cn/Article/details/gqnvrlvcw.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/gbezbsolw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqjhjzmf.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.yfazqb.com/Article/details/gbwdlxwcy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fktsv.cn/Article/details/gxglkabpv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.vehdjk.com/Article/details/gastzuulh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fktsv.cn/Article/details/gwhwxdcyw.sHtML

[S10] C：指针与解引用
来源：http://blog.bbcook.cn/Article/details/ginuwamnh.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.tarul.cn/Article/details/gzfpkpyfz.sHtML

[S11] C：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gvojwkxns.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.vehdjk.com/Article/details/gszkfkrhl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.vehdjk.com/Article/details/ggsimaxth.sHtML

fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gyqrtybst.sHtML

[S12] C：写文件
来源：http://www.blog.yfazqb.com/Article/details/giacpmwhc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.yfazqb.com/Article/details/gzlfrrdqd.sHtML

[S13] C：宏定义
来源：http://www.blog.fktsv.cn/Article/details/gznpsuvtv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.bbcook.cn/Article/details/gprddwfrq.sHtML

[S14] C：枚举
来源：http://wap.vehdjk.com/Article/details/ginmrhfdi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.sjlbkw.cn/Article/details/guqnftrrt.sHtML

[S15] C：类型转换
来源：http://m.share.vehdjk.com/Article/details/gxtfoqvgx.sHtML

(double) a / b
来源：http://blog.vehdjk.com/Article/details/gfjtqirge.sHtML

[S16] C：位操作置位
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaescobm.sHtML

x |= (1 << 3);
来源：http://mobile.epnwcf.com/Article/details/gmlmdtgdp.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gnxcotnxc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.yfazqb.com/Article/details/gknrvmtuh.sHtML

[S18] C：命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gxxrkpsvw.sHtML

int main(int argc, char **argv)
来源：http://read.share.vehdjk.com/Article/details/gyntpcozk.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/gevnjwaoq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gseyfkhyf.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/giaytxdmp.sHtML


<!-- 参考信息 -->