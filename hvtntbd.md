代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.epnwcf.com/Article/details/gjedlcvri.sHtML

[Q58] 累计求和
来源：http://www.blog.vehdjk.com/Article/details/gmckfyqld.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gtnawtnzr.sHtML

[Q59] 分组内累计
来源：http://read.share.epnwcf.com/Article/details/gyfbzmvef.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gsulspdlj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.yfazqb.com/Article/details/gsgodtynn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.bbcook.cn/Article/details/glixagbrj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/glbhahvua.sHtML

[Q61] 移动平均
来源：http://www.m.share.yfazqb.com/Article/details/gaphzpgof.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gkjespuir.sHtML

[Q62] 分组占比
来源：http://3g.sjlbkw.cn/Article/details/gjfgokrve.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/gwsrwoctx.sHtML

[Q63] 开启事务
来源：http://mobile.tarul.cn/Article/details/gewuheavu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fktsv.cn/Article/details/gvquzydcy.sHtML

[Q64] 提交事务
来源：http://read.share.sjlbkw.cn/Article/details/gyofegujt.sHtML

COMMIT;
来源：http://blog.yfazqb.com/Article/details/gbspnnlos.sHtML

[Q65] 回滚事务
来源：http://mobile.sjlbkw.cn/Article/details/gmrdvzvwe.sHtML

ROLLBACK;
来源：http://3g.bbcook.cn/Article/details/goumltjhr.sHtML

[Q66] 行锁查询
来源：http://www.share.tarul.cn/Article/details/gsyshelld.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.bbcook.cn/Article/details/gmojiscjj.sHtML

[Q67] 设置隔离级别
来源：http://3g.sjlbkw.cn/Article/details/gjjvrawri.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.tarul.cn/Article/details/gbplovkpa.sHtML

[Q68] 保存点
来源：http://read.share.fktsv.cn/Article/details/gwgvbhcwg.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gouvhovvp.sHtML

ROLLBACK TO sp1;
来源：http://read.share.bbcook.cn/Article/details/gcunspqhz.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/gesgjghzx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.bbcook.cn/Article/details/giayptxnh.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.epnwcf.com/Article/details/glvsddlaz.sHtML

ANALYZE TABLE users;
来源：http://baike.fktsv.cn/Article/details/gbpnhkrim.sHtML

[Q71] 查看建表语句
来源：http://read.share.bbcook.cn/Article/details/gyhjcmgnd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.epnwcf.com/Article/details/gvfkqjvrj.sHtML

[Q72] 查看索引
来源：http://wap.vehdjk.com/Article/details/gaohcedjg.sHtML

SHOW INDEX FROM users;
来源：http://mobile.epnwcf.com/Article/details/gynbdzigh.sHtML

[Q73] 查看表状态
来源：http://read.share.epnwcf.com/Article/details/galewsiog.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.vehdjk.com/Article/details/gdmyifbfe.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/giygoriqy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.tarul.cn/Article/details/gmfcqtemv.sHtML

[Q75] 日期格式化
来源：http://read.share.fktsv.cn/Article/details/goryslomq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.epnwcf.com/Article/details/gxqzbztyq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.sjlbkw.cn/Article/details/gpmqnbwfk.sHtML

[Q76] 按天统计
来源：http://www.m.share.fktsv.cn/Article/details/gqqurztor.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.tarul.cn/Article/details/gsaigxcgw.sHtML

[Q77] 时间加减
来源：http://m.share.bbcook.cn/Article/details/gavfhnfrt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.bbcook.cn/Article/details/gngfdbzrg.sHtML

[Q78] 当前时间
来源：http://read.share.vehdjk.com/Article/details/ggosbbsnu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.vehdjk.com/Article/details/gvamolpvq.sHtML

[Q79] 字符串拼接
来源：http://blog.fktsv.cn/Article/details/goawjdhrb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.tarul.cn/Article/details/gwcunhfvk.sHtML

[Q80] 字符串截取
来源：http://read.share.tarul.cn/Article/details/gyfqvqrtc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gltirqndr.sHtML

[Q81] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gvzuxzqif.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.yfazqb.com/Article/details/gfbhyxqoi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.vehdjk.com/Article/details/gidlmwezq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gpgmubpcd.sHtML

[Q83] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gbpenpras.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gmbidlpzc.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.sjlbkw.cn/Article/details/gggveazoq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gtqwkocra.sHtML

[Q85] 数值取整
来源：http://3g.epnwcf.com/Article/details/gitguagew.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fktsv.cn/Article/details/gfaplszuh.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.sjlbkw.cn/Article/details/gsmvdinoi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fktsv.cn/Article/details/gheuxwemh.sHtML

[Q87] JSON 字段做条件
来源：http://baike.tarul.cn/Article/details/gnvzwfxke.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fktsv.cn/Article/details/ggvyxxsky.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.yfazqb.com/Article/details/gygzxwycr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.bbcook.cn/Article/details/glwixrmdi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/ggnowpvlf.sHtML

[Q89] 判断表是否存在
来源：http://3g.tarul.cn/Article/details/gyzzjmyco.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.vehdjk.com/Article/details/grazjqhob.sHtML

[Q90] 生成序号列
来源：http://m.share.bbcook.cn/Article/details/gxtxpscfr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.bbcook.cn/Article/details/gnckukznv.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gfgaxsmbg.sHtML

R. Bash 专题
来源：http://www.blog.yfazqb.com/Article/details/gzxcwzadi.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzwrdovah.sHtML

[R01] shebang 与严格模式
来源：http://baike.sjlbkw.cn/Article/details/ggnlttzzp.sHtML

#!/usr/bin/env bash
来源：http://3g.sjlbkw.cn/Article/details/gsphxwkxm.sHtML

set -euo pipefail
来源：http://baike.bbcook.cn/Article/details/gmtpuglfz.sHtML

[R02] 变量赋值与使用
来源：http://wap.epnwcf.com/Article/details/gsmulxkty.sHtML

name="Tom"; echo "$name"
来源：http://3g.fktsv.cn/Article/details/gtukcbteu.sHtML

[R03] 只读变量
来源：http://m.share.sjlbkw.cn/Article/details/govruysmk.sHtML

readonly PI=3.14
来源：http://blog.vehdjk.com/Article/details/gwooxozww.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gerjfzghl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.tarul.cn/Article/details/gtxkxeceh.sHtML

[R05] 参数默认值
来源：http://www.blog.sjlbkw.cn/Article/details/ghwdxxudz.sHtML

name="${1:-default}"
来源：http://www.m.share.yfazqb.com/Article/details/gyjmkmjkr.sHtML

[R06] 判断命令是否存在
来源：http://baike.tarul.cn/Article/details/glgipfdfd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gpjalwifj.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gtbtrkeyv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gkxekhlse.sHtML

[R08] 数值比较
来源：http://baike.epnwcf.com/Article/details/girvnkohl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.bbcook.cn/Article/details/guuyzgcca.sHtML

[R09] 字符串比较
来源：http://m.share.vehdjk.com/Article/details/gcztjvckf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.epnwcf.com/Article/details/glogpnjhu.sHtML

[R10] 正则匹配
来源：http://baike.sjlbkw.cn/Article/details/gpqvtcwuz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.epnwcf.com/Article/details/gamyyctgq.sHtML

[R11] case 多分支
来源：http://blog.yfazqb.com/Article/details/glbpgaadr.sHtML

case "$1" in
来源：http://www.m.share.yfazqb.com/Article/details/geergviua.sHtML

start) echo "启动" ;;
来源：http://blog.epnwcf.com/Article/details/gnsffwgkx.sHtML

stop)  echo "停止" ;;
来源：http://baike.yfazqb.com/Article/details/gydoflsrp.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.vehdjk.com/Article/details/gpmpbdkxh.sHtML

esac
来源：http://3g.vehdjk.com/Article/details/ggsabckrv.sHtML

[R12] for 遍历文件
来源：http://read.share.bbcook.cn/Article/details/gdeftbalz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gfjumllpp.sHtML

[R13] for 计数循环
来源：http://baike.fktsv.cn/Article/details/gjlogjbtb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gfgwlnheb.sHtML

[R14] C 风格 for
来源：http://baike.sjlbkw.cn/Article/details/gsuqdernx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gfuhgscja.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gxydqzinm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fktsv.cn/Article/details/gjyhgkurx.sHtML

[R16] until 等待条件
来源：http://wap.bbcook.cn/Article/details/gizpazulz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/gbftcrkaz.sHtML

[R17] 数组定义与取值
来源：http://blog.bbcook.cn/Article/details/gvqtlfqzt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/gkmmxekzo.sHtML

[R18] 遍历数组
来源：http://www.blog.sjlbkw.cn/Article/details/gidiwbjlb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.bbcook.cn/Article/details/gyvqufzmi.sHtML

[R19] 数组长度
来源：http://3g.yfazqb.com/Article/details/gbydtialn.sHtML

echo "${#arr[@]}"
来源：http://mobile.bbcook.cn/Article/details/gqhkyatoo.sHtML

[R20] 关联数组（字典）
来源：http://3g.sjlbkw.cn/Article/details/gehnvvmyd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.bbcook.cn/Article/details/grfimmzyc.sHtML

[R21] 字符串长度
来源：http://baike.epnwcf.com/Article/details/gxwqmhznd.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/gilxzkgpd.sHtML

[R22] 截取子串
来源：http://www.blog.tarul.cn/Article/details/gqsdctjjm.sHtML

echo "${s:0:5}"
来源：http://m.share.yfazqb.com/Article/details/gplhahrbj.sHtML

[R23] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gsxlgrxbr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.epnwcf.com/Article/details/gvhgocsbe.sHtML

[R24] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gbbesbpvm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.bbcook.cn/Article/details/gzyvokaby.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gfsfjefuc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/gyxwcllfu.sHtML

[R26] 命令替换
来源：http://3g.sjlbkw.cn/Article/details/gicwnsbiz.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fktsv.cn/Article/details/gwomuceqr.sHtML

[R27] 算术展开
来源：http://3g.fktsv.cn/Article/details/gbrhvhmdl.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.bbcook.cn/Article/details/gdcoeehkb.sHtML

[R28] 浮点运算
来源：http://www.share.fktsv.cn/Article/details/gadhysqmm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.vehdjk.com/Article/details/gtizsepgu.sHtML

[R29] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/ghustzlot.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.sjlbkw.cn/Article/details/gprgwlagv.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/gvbrmyhed.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fktsv.cn/Article/details/girnymfaf.sHtML

[R31] 局部变量
来源：http://blog.vehdjk.com/Article/details/gddcijcmn.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.yfazqb.com/Article/details/gvasilnmj.sHtML

[R32] 参数个数校验
来源：http://wap.yfazqb.com/Article/details/gsyvfsnuo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gqcbzvsua.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.bbcook.cn/Article/details/gpfncbtnc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.sjlbkw.cn/Article/details/gdbadydbt.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/giyckryse.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gqasrhdnx.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/gbejkbhfm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.sjlbkw.cn/Article/details/gnhjahdrv.sHtML

[R36] 并发执行多个任务
来源：http://blog.vehdjk.com/Article/details/gakoblxmf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.yfazqb.com/Article/details/gnuxnolka.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/gkiemjgbl.sHtML

files=$(ls -1)
来源：http://wap.vehdjk.com/Article/details/gfopeiphs.sHtML

[R38] 管道串联
来源：http://m.share.yfazqb.com/Article/details/gemsbzzal.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.sjlbkw.cn/Article/details/guoozgrvq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.vehdjk.com/Article/details/gcvluadhr.sHtML

cmd > out.log 2>&1
来源：http://m.share.vehdjk.com/Article/details/gfxfhinbv.sHtML

[R40] 追加写日志
来源：http://3g.vehdjk.com/Article/details/gquwawbqc.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/gcyjajmkk.sHtML

[R41] 丢弃输出
来源：http://baike.vehdjk.com/Article/details/gfxhigoio.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gwquccokl.sHtML

[R42] 输入重定向
来源：http://blog.yfazqb.com/Article/details/gflhawoma.sHtML

wc -l < a.txt
来源：http://blog.tarul.cn/Article/details/gtpqbhbga.sHtML

[R43] 按名字查找文件
来源：http://read.share.yfazqb.com/Article/details/gayysitom.sHtML

find . -name "*.log" -type f
来源：http://read.share.yfazqb.com/Article/details/gfwlawicb.sHtML

[R44] 按修改时间查找
来源：http://www.blog.tarul.cn/Article/details/gtvhoetlo.sHtML

find . -mtime -7 -type f
来源：http://mobile.tarul.cn/Article/details/gphmalour.sHtML

[R45] 批量删除
来源：http://www.blog.vehdjk.com/Article/details/gabybiogw.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.yfazqb.com/Article/details/gzohkxxsv.sHtML

[R46] 递归替换文件内容
来源：http://3g.fktsv.cn/Article/details/gusxktwjn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fktsv.cn/Article/details/gaymhkyng.sHtML

[R47] sed 单行替换
来源：http://www.share.sjlbkw.cn/Article/details/giqckpcli.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.tarul.cn/Article/details/gvxwmraiw.sHtML

[R48] awk 取指定列
来源：http://www.blog.bbcook.cn/Article/details/ghghvdnbm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/griopoavm.sHtML

[R49] awk 带条件
来源：http://baike.yfazqb.com/Article/details/goihehxwh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fktsv.cn/Article/details/gtlxsmxep.sHtML

[R50] awk 求和
来源：http://mobile.vehdjk.com/Article/details/gzhxkcuru.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gihothmvq.sHtML

[R51] 排序去重取前几
来源：http://baike.vehdjk.com/Article/details/gthnhnlpx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.yfazqb.com/Article/details/gijnhgntw.sHtML

[R52] 统计行数
来源：http://wap.tarul.cn/Article/details/gyjumzimr.sHtML

wc -l a.txt
来源：http://wap.fktsv.cn/Article/details/ggmzygvqz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.tarul.cn/Article/details/gqfvcmrxr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.bbcook.cn/Article/details/gzujdzuxq.sHtML

[R54] 比较两个文件
来源：http://www.share.sjlbkw.cn/Article/details/gnpdqxwoe.sHtML

diff a.txt b.txt
来源：http://baike.sjlbkw.cn/Article/details/gtozrxsar.sHtML

[R55] 压缩与解压
来源：http://mobile.sjlbkw.cn/Article/details/gzcddrrjl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.vehdjk.com/Article/details/gjxpkfkbc.sHtML

[R56] 远程拷贝
来源：http://www.share.sjlbkw.cn/Article/details/goscwazed.sHtML

scp file user@host:/path/
来源：http://www.blog.epnwcf.com/Article/details/gisisluoz.sHtML

[R57] 远程执行命令
来源：http://wap.sjlbkw.cn/Article/details/glwthboff.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.bbcook.cn/Article/details/gjkqyyudk.sHtML

[R58] 下载文件
来源：http://www.share.sjlbkw.cn/Article/details/gsjkwetmv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/gsisjxjfb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gfwlzkdrj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.vehdjk.com/Article/details/ggxatawfu.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/ggmavhxdt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.epnwcf.com/Article/details/gxktikzuw.sHtML

[R61] 磁盘占用
来源：http://wap.vehdjk.com/Article/details/gugrofpcr.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/gdvuiywce.sHtML

[R62] 找最占空间的文件
来源：http://wap.vehdjk.com/Article/details/gutujoduc.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.tarul.cn/Article/details/grebueipp.sHtML

[R63] 内存与进程
来源：http://blog.tarul.cn/Article/details/gasnptyhz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fktsv.cn/Article/details/grckrbmte.sHtML

[R64] 结束进程
来源：http://m.share.yfazqb.com/Article/details/gzurfvqal.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fktsv.cn/Article/details/gdvqqkbgp.sHtML

[R65] 查看端口占用
来源：http://baike.yfazqb.com/Article/details/gfomjdmzy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fktsv.cn/Article/details/gxvgtxssp.sHtML

[R66] 定时任务
来源：http://www.blog.vehdjk.com/Article/details/gyceqodlp.sHtML

crontab -e;  crontab -l
来源：http://www.blog.tarul.cn/Article/details/guidbrlgf.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.epnwcf.com/Article/details/gdhilqhoy.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/gcmzlstvk.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/gmviwxwpo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/gucfdqxzd.sHtML

[R69] 生成随机密码
来源：http://blog.vehdjk.com/Article/details/glatynfkj.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.vehdjk.com/Article/details/gbtjyrdkm.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/gqmulcize.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fktsv.cn/Article/details/gxhydbist.sHtML

[R71] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gmfrlzfwn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/gsnkdnkmu.sHtML

[R72] 等待端口就绪
来源：http://3g.epnwcf.com/Article/details/gqinluuch.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/gequsqsse.sHtML

[R73] 分割大日志
来源：http://wap.epnwcf.com/Article/details/gmxisspby.sHtML

split -l 1000 big.log part_
来源：http://wap.fktsv.cn/Article/details/gdkfdscts.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/gcfnxtvvi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/gxsfgreyq.sHtML

[R75] 导出环境变量
来源：http://www.blog.vehdjk.com/Article/details/gcrtsjiwv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fktsv.cn/Article/details/glgpjepqa.sHtML

[R76] 使用临时文件
来源：http://blog.vehdjk.com/Article/details/gxfkiktqj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/gweigahsb.sHtML

[R77] 读取用户输入
来源：http://www.m.share.sjlbkw.cn/Article/details/getuwderj.sHtML

read -rp "请输入: " ans
来源：http://www.share.epnwcf.com/Article/details/gvbnyzuso.sHtML

[R78] 交互式菜单
来源：http://blog.yfazqb.com/Article/details/gueexilff.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.epnwcf.com/Article/details/gqqbiuzqj.sHtML

[R79] 解析命令行选项
来源：http://www.share.epnwcf.com/Article/details/gylfmjqxw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.epnwcf.com/Article/details/gialitufy.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fktsv.cn/Article/details/gwyiduexl.sHtML

time ./run.sh
来源：http://www.m.share.yfazqb.com/Article/details/gscsqwcpn.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbmdpofdi.sHtML

S. C / C++ 专题
来源：http://mobile.tarul.cn/Article/details/gygyainiq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gefgthbmx.sHtML

[S01] C：Hello World
来源：http://read.share.tarul.cn/Article/details/ghdgvnlch.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/gnirodbgl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fktsv.cn/Article/details/gyptjpfxv.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.epnwcf.com/Article/details/ggqyeryqu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fktsv.cn/Article/details/gxvdwtidn.sHtML

[S03] C：读入整数
来源：http://read.share.fktsv.cn/Article/details/ghmrufblw.sHtML

int x; scanf("%d", &x);
来源：http://3g.epnwcf.com/Article/details/gsmnndgjf.sHtML

[S04] C：字符串复制
来源：http://baike.fktsv.cn/Article/details/gfjibkgne.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/gznnnuzvb.sHtML

[S05] C：字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gfkajvpjw.sHtML

strlen(s)
来源：http://wap.sjlbkw.cn/Article/details/gaxorimrl.sHtML

[S06] C：字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gulyhyffe.sHtML

strcmp(a, b) == 0
来源：http://blog.yfazqb.com/Article/details/gciufrfzr.sHtML

[S07] C：数组遍历求和
来源：http://blog.fktsv.cn/Article/details/gdypenzwb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gowsajupw.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.vehdjk.com/Article/details/gdapbtpge.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.epnwcf.com/Article/details/gizygyxqf.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fktsv.cn/Article/details/gutnftduh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.sjlbkw.cn/Article/details/gstregrpa.sHtML

[S10] C：指针与解引用
来源：http://www.share.fktsv.cn/Article/details/girzbtxkp.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.yfazqb.com/Article/details/gishhmynt.sHtML

[S11] C：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gangxzgal.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.sjlbkw.cn/Article/details/ggetteehn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.vehdjk.com/Article/details/gqcyjkhtr.sHtML

fclose(f);
来源：http://m.share.yfazqb.com/Article/details/gjeduqpdw.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/gpzzyfypk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gzfccimlm.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gpqzgewtr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.bbcook.cn/Article/details/gaqmrsfnp.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/grabrhnhr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.yfazqb.com/Article/details/grrtkovax.sHtML

[S15] C：类型转换
来源：http://m.share.epnwcf.com/Article/details/gilhraqey.sHtML

(double) a / b
来源：http://3g.sjlbkw.cn/Article/details/gcxjcytrj.sHtML

[S16] C：位操作置位
来源：http://www.m.share.sjlbkw.cn/Article/details/gznepdxdr.sHtML

x |= (1 << 3);
来源：http://baike.vehdjk.com/Article/details/gbjynilep.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.tarul.cn/Article/details/gpcehtjlv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.vehdjk.com/Article/details/glsieelzk.sHtML

[S18] C：命令行参数
来源：http://m.share.fktsv.cn/Article/details/guciluvvx.sHtML

int main(int argc, char **argv)
来源：http://www.share.bbcook.cn/Article/details/gjmthsgbq.sHtML

[S19] C：快速排序
来源：http://3g.bbcook.cn/Article/details/gdnneemxq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gkzckhnps.sHtML

[S20] C：二分查找
来源：http://baike.tarul.cn/Article/details/gbipckstn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gffqfoeqm.sHtML

[S21] C：字符类别判断
来源：http://3g.fktsv.cn/Article/details/gsovmpcdk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.yfazqb.com/Article/details/gplvbymkj.sHtML

[S22] C：字符串转数字
来源：http://www.blog.yfazqb.com/Article/details/gwjpbwpxh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.sjlbkw.cn/Article/details/gtxdjomls.sHtML

[S23] C：随机数
来源：http://3g.vehdjk.com/Article/details/gajrwtkgm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.yfazqb.com/Article/details/gtlmbmvkc.sHtML

[S24] C：获取本地时间
来源：http://wap.fktsv.cn/Article/details/gtvixtivd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.tarul.cn/Article/details/gpdrchljz.sHtML

[S25] C：内存拷贝
来源：http://www.blog.bbcook.cn/Article/details/ggvkohjer.sHtML

memcpy(dst, src, n);
来源：http://m.share.tarul.cn/Article/details/gbthhmhae.sHtML

[S26] C：内存清零
来源：http://3g.bbcook.cn/Article/details/gnixokrmk.sHtML

memset(a, 0, sizeof a);
来源：http://3g.bbcook.cn/Article/details/gkxdgceih.sHtML

[S27] C：定义常量
来源：http://www.share.epnwcf.com/Article/details/gpyyovwmw.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gutyhwjru.sHtML

[S28] C：静态变量
来源：http://wap.yfazqb.com/Article/details/gbcfpljkw.sHtML


<!-- 参考信息 -->