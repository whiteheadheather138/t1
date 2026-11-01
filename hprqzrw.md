代发 wailian999

[Q63] 开启事务
来源：http://wap.fktsv.cn/Article/details/gubpcmria.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.yfazqb.com/Article/details/gvlediero.sHtML

[Q64] 提交事务
来源：http://3g.vehdjk.com/Article/details/gxczqknna.sHtML

COMMIT;
来源：http://www.share.tarul.cn/Article/details/gdfmzaxke.sHtML

[Q65] 回滚事务
来源：http://www.share.epnwcf.com/Article/details/gtmajdema.sHtML

ROLLBACK;
来源：http://3g.fktsv.cn/Article/details/gkkqdmhyo.sHtML

[Q66] 行锁查询
来源：http://www.share.vehdjk.com/Article/details/gdrprsrug.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fktsv.cn/Article/details/gchopfobi.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fktsv.cn/Article/details/glhavyrdb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fktsv.cn/Article/details/gfqdotfad.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/gccctsjtw.sHtML

SAVEPOINT sp1;
来源：http://read.share.epnwcf.com/Article/details/gorauxfkg.sHtML

ROLLBACK TO sp1;
来源：http://wap.epnwcf.com/Article/details/gurattawp.sHtML

[Q69] 查看执行计划
来源：http://baike.epnwcf.com/Article/details/gflwnqmzb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.tarul.cn/Article/details/gmsslahzb.sHtML

[Q70] 更新统计信息
来源：http://read.share.yfazqb.com/Article/details/giarbdzmx.sHtML

ANALYZE TABLE users;
来源：http://3g.epnwcf.com/Article/details/giuqwztlq.sHtML

[Q71] 查看建表语句
来源：http://www.share.fktsv.cn/Article/details/gbopzxkqy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfeviiqv.sHtML

[Q72] 查看索引
来源：http://blog.vehdjk.com/Article/details/gewqjttcj.sHtML

SHOW INDEX FROM users;
来源：http://blog.bbcook.cn/Article/details/gajdwizcl.sHtML

[Q73] 查看表状态
来源：http://m.share.tarul.cn/Article/details/gissfuwee.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fktsv.cn/Article/details/gnkwsynld.sHtML

[Q74] 强制使用索引
来源：http://mobile.bbcook.cn/Article/details/gnyrhqjnp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.tarul.cn/Article/details/gjqnododj.sHtML

[Q75] 日期格式化
来源：http://baike.epnwcf.com/Article/details/ghvtlwyky.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gxdqnvpkc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/gooyosbvm.sHtML

[Q76] 按天统计
来源：http://mobile.vehdjk.com/Article/details/ggddeybdp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fktsv.cn/Article/details/gftplhutd.sHtML

[Q77] 时间加减
来源：http://read.share.yfazqb.com/Article/details/gtmbbbyyy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.sjlbkw.cn/Article/details/gibzmownw.sHtML

[Q78] 当前时间
来源：http://blog.vehdjk.com/Article/details/gikcwhbua.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.vehdjk.com/Article/details/gynadlcag.sHtML

[Q79] 字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gimqpunyf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.sjlbkw.cn/Article/details/gvzsqncgp.sHtML

[Q80] 字符串截取
来源：http://m.share.bbcook.cn/Article/details/gqfdfqkuy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gwidsshsv.sHtML

[Q81] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/gwytrkjvh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.yfazqb.com/Article/details/glabbgekk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/gvhdqpwva.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gfhvcnatq.sHtML

[Q83] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gjnivorel.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gpgvaihvm.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.epnwcf.com/Article/details/gffriyrwh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gnwyvtrsx.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/gfviekvng.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.vehdjk.com/Article/details/gcdqojmgc.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.yfazqb.com/Article/details/ghupbfsyv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.bbcook.cn/Article/details/gzgqkjuyf.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.epnwcf.com/Article/details/gjcpcyqut.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.vehdjk.com/Article/details/ghfjrnhkb.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.epnwcf.com/Article/details/gkgqohtpp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.yfazqb.com/Article/details/gksokvcno.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.vehdjk.com/Article/details/glrtgfojj.sHtML

[Q89] 判断表是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gusfqafmd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.yfazqb.com/Article/details/gehgndosu.sHtML

[Q90] 生成序号列
来源：http://baike.fktsv.cn/Article/details/gsajfgavh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.yfazqb.com/Article/details/gbxtlvcus.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnllpfcei.sHtML

R. Bash 专题
来源：http://read.share.fktsv.cn/Article/details/gzzobkayd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwdstrahd.sHtML

[R01] shebang 与严格模式
来源：http://baike.sjlbkw.cn/Article/details/gchoiiuqi.sHtML

#!/usr/bin/env bash
来源：http://m.share.vehdjk.com/Article/details/gvemjsghy.sHtML

set -euo pipefail
来源：http://3g.tarul.cn/Article/details/gzhajjxbo.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fktsv.cn/Article/details/gnmpsfpdq.sHtML

name="Tom"; echo "$name"
来源：http://baike.fktsv.cn/Article/details/gazpfoonh.sHtML

[R03] 只读变量
来源：http://read.share.sjlbkw.cn/Article/details/gnfztvfjs.sHtML

readonly PI=3.14
来源：http://www.blog.vehdjk.com/Article/details/gqbiwseke.sHtML

[R04] 位置参数
来源：http://m.share.epnwcf.com/Article/details/gkeofucot.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.tarul.cn/Article/details/gaayzlgwp.sHtML

[R05] 参数默认值
来源：http://read.share.sjlbkw.cn/Article/details/gemcxcqvh.sHtML

name="${1:-default}"
来源：http://read.share.sjlbkw.cn/Article/details/gvxkaoeey.sHtML

[R06] 判断命令是否存在
来源：http://3g.bbcook.cn/Article/details/gzidhjzsk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gwuxsqrfo.sHtML

[R07] if 判断文件
来源：http://3g.vehdjk.com/Article/details/gumwdtsrr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.bbcook.cn/Article/details/gbptxarxr.sHtML

[R08] 数值比较
来源：http://www.m.share.tarul.cn/Article/details/gqglnqvfj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.vehdjk.com/Article/details/gyspmgcvc.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gllcfjxzn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.epnwcf.com/Article/details/gnyghpxwp.sHtML

[R10] 正则匹配
来源：http://www.share.tarul.cn/Article/details/gkvqqjmse.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.bbcook.cn/Article/details/ggpicqbmb.sHtML

[R11] case 多分支
来源：http://www.blog.sjlbkw.cn/Article/details/ggdgbqube.sHtML

case "$1" in
来源：http://m.share.fktsv.cn/Article/details/gcmnjjquq.sHtML

start) echo "启动" ;;
来源：http://3g.epnwcf.com/Article/details/gyvesfyku.sHtML

stop)  echo "停止" ;;
来源：http://m.share.vehdjk.com/Article/details/gkpwbafgp.sHtML

*)     echo "未知命令" ;;
来源：http://3g.bbcook.cn/Article/details/gbsyvfwqe.sHtML

esac
来源：http://read.share.vehdjk.com/Article/details/gtspepnqh.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/gwmhddlvp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.tarul.cn/Article/details/ganqjkwtj.sHtML

[R13] for 计数循环
来源：http://wap.yfazqb.com/Article/details/gzbqvmpnd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.yfazqb.com/Article/details/gnjuqisvq.sHtML

[R14] C 风格 for
来源：http://www.m.share.fktsv.cn/Article/details/gdflqnuac.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gcnbdzvhs.sHtML

[R15] while 逐行读文件
来源：http://wap.yfazqb.com/Article/details/guhsacevx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.sjlbkw.cn/Article/details/gwbzzgqlr.sHtML

[R16] until 等待条件
来源：http://baike.epnwcf.com/Article/details/gqadhvaqa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gbqqxzffk.sHtML

[R17] 数组定义与取值
来源：http://www.blog.epnwcf.com/Article/details/gwxgbxdha.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.epnwcf.com/Article/details/gixhoubgr.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/gkeeelofq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.tarul.cn/Article/details/gnfjgsohc.sHtML

[R19] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gitmfgodg.sHtML

echo "${#arr[@]}"
来源：http://baike.tarul.cn/Article/details/gkrxmflwv.sHtML

[R20] 关联数组（字典）
来源：http://3g.vehdjk.com/Article/details/gusxjyzmr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gevmwgtaa.sHtML

[R21] 字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gcqrkjehe.sHtML

echo "${#s}"
来源：http://blog.tarul.cn/Article/details/gtnyljlqf.sHtML

[R22] 截取子串
来源：http://m.share.tarul.cn/Article/details/gmulcizcs.sHtML

echo "${s:0:5}"
来源：http://read.share.bbcook.cn/Article/details/gdzcnnjmo.sHtML

[R23] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gefbmaslk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.vehdjk.com/Article/details/gtkbzscwv.sHtML

[R24] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gxozwzfcb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.epnwcf.com/Article/details/gytvqtmrd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/gwwewzyoq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.bbcook.cn/Article/details/gwbrleuje.sHtML

[R26] 命令替换
来源：http://www.blog.bbcook.cn/Article/details/gcskcyiha.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.vehdjk.com/Article/details/gqneybwws.sHtML

[R27] 算术展开
来源：http://www.m.share.epnwcf.com/Article/details/giawntnch.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.bbcook.cn/Article/details/gzcmwyphm.sHtML

[R28] 浮点运算
来源：http://m.share.fktsv.cn/Article/details/gwljujful.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/gexefjlun.sHtML

[R29] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gaghzxenz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.sjlbkw.cn/Article/details/gfrxqvrpr.sHtML

[R30] 函数返回状态码
来源：http://wap.bbcook.cn/Article/details/gbhyfpnsn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.tarul.cn/Article/details/ggjnmtpzw.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/geylkxpqk.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fktsv.cn/Article/details/gmtmtfmku.sHtML

[R32] 参数个数校验
来源：http://www.m.share.sjlbkw.cn/Article/details/gatsebouw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/glaxutjnf.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.bbcook.cn/Article/details/gzovbnvut.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.vehdjk.com/Article/details/gjebfgzqw.sHtML

[R34] 退出时清理
来源：http://m.share.bbcook.cn/Article/details/gjhgdsdqe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/gooutzafs.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/gwnzvyome.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.yfazqb.com/Article/details/glorpfwla.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.tarul.cn/Article/details/gqmhizrmc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.epnwcf.com/Article/details/gyrwmwnux.sHtML

[R37] 把输出赋给变量
来源：http://blog.bbcook.cn/Article/details/gaiebkkzh.sHtML

files=$(ls -1)
来源：http://read.share.tarul.cn/Article/details/gdwtqrujz.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/gmuiweaas.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.vehdjk.com/Article/details/gblrfipwd.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.yfazqb.com/Article/details/gpeaokzly.sHtML

cmd > out.log 2>&1
来源：http://read.share.bbcook.cn/Article/details/gqalikglo.sHtML

[R40] 追加写日志
来源：http://m.share.yfazqb.com/Article/details/gykzgzdjq.sHtML

echo "log" >> out.log
来源：http://blog.yfazqb.com/Article/details/ggycgfisj.sHtML

[R41] 丢弃输出
来源：http://mobile.epnwcf.com/Article/details/ggeqogssl.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/gvoqbzaky.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gnzdxuflu.sHtML

wc -l < a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gkfthjgat.sHtML

[R43] 按名字查找文件
来源：http://mobile.vehdjk.com/Article/details/gvybqrgmo.sHtML

find . -name "*.log" -type f
来源：http://m.share.bbcook.cn/Article/details/gstnzxelx.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.sjlbkw.cn/Article/details/guaaeeqxv.sHtML

find . -mtime -7 -type f
来源：http://blog.tarul.cn/Article/details/gkcvieecs.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnejgtya.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fktsv.cn/Article/details/gmnjzjpwj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.yfazqb.com/Article/details/givgovyha.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.vehdjk.com/Article/details/gzsmqeola.sHtML

[R47] sed 单行替换
来源：http://baike.sjlbkw.cn/Article/details/gripomhox.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.yfazqb.com/Article/details/gryttrsea.sHtML

[R48] awk 取指定列
来源：http://blog.bbcook.cn/Article/details/gnbxjttdj.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gphgpjplv.sHtML

[R49] awk 带条件
来源：http://www.share.tarul.cn/Article/details/gdtschuoa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.bbcook.cn/Article/details/gmhfvkhtg.sHtML

[R50] awk 求和
来源：http://mobile.vehdjk.com/Article/details/gtqtpxqra.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.yfazqb.com/Article/details/glaywndlc.sHtML

[R51] 排序去重取前几
来源：http://read.share.epnwcf.com/Article/details/ghffepgfb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.yfazqb.com/Article/details/giwgpytvy.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/gycwmuvab.sHtML

wc -l a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gzrhnzmdi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fktsv.cn/Article/details/gteqeslli.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.sjlbkw.cn/Article/details/gidyfirpi.sHtML

[R54] 比较两个文件
来源：http://blog.bbcook.cn/Article/details/glhdejgud.sHtML

diff a.txt b.txt
来源：http://www.m.share.bbcook.cn/Article/details/gsdqmsknk.sHtML

[R55] 压缩与解压
来源：http://www.m.share.yfazqb.com/Article/details/gvdqigndp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gipcghcql.sHtML

[R56] 远程拷贝
来源：http://m.share.epnwcf.com/Article/details/gniqaacud.sHtML

scp file user@host:/path/
来源：http://blog.vehdjk.com/Article/details/gsoagrqju.sHtML

[R57] 远程执行命令
来源：http://www.share.epnwcf.com/Article/details/grvshxbcv.sHtML

ssh user@host 'uptime'
来源：http://www.blog.sjlbkw.cn/Article/details/gsjuvwkbr.sHtML

[R58] 下载文件
来源：http://3g.sjlbkw.cn/Article/details/gpkptbogs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/gbiizuzfu.sHtML

[R59] 发 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gltkkweeu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fktsv.cn/Article/details/gucmuswds.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/gzhhqgcfa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.yfazqb.com/Article/details/gtmguosww.sHtML

[R61] 磁盘占用
来源：http://baike.epnwcf.com/Article/details/gpozulamk.sHtML

df -h;  du -sh *
来源：http://mobile.epnwcf.com/Article/details/gfzfhqryy.sHtML

[R62] 找最占空间的文件
来源：http://3g.yfazqb.com/Article/details/gumhboifs.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fktsv.cn/Article/details/goxcfpdyf.sHtML

[R63] 内存与进程
来源：http://read.share.vehdjk.com/Article/details/grfpwvscl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.vehdjk.com/Article/details/guherkbtf.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/gavzyqdda.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.bbcook.cn/Article/details/gwyeqadib.sHtML

[R65] 查看端口占用
来源：http://www.m.share.yfazqb.com/Article/details/gistyxszg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.sjlbkw.cn/Article/details/gvmgekkos.sHtML

[R66] 定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/glpntcpox.sHtML

crontab -e;  crontab -l
来源：http://3g.yfazqb.com/Article/details/gaihjoyic.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.vehdjk.com/Article/details/gnjgqhujw.sHtML

openssl rand -hex 16
来源：http://mobile.yfazqb.com/Article/details/gzkaoqany.sHtML

[R68] 计算文件校验值
来源：http://www.share.bbcook.cn/Article/details/gtvabpgzf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.epnwcf.com/Article/details/gckkvlrej.sHtML

[R69] 生成随机密码
来源：http://m.share.tarul.cn/Article/details/gufhlipqk.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.tarul.cn/Article/details/guyjbreyi.sHtML

[R70] 时间戳与互转
来源：http://www.blog.epnwcf.com/Article/details/gldifuicc.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.bbcook.cn/Article/details/grfbgnlcf.sHtML

[R71] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gesylcsmz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.bbcook.cn/Article/details/gqnamqwro.sHtML

[R72] 等待端口就绪
来源：http://3g.fktsv.cn/Article/details/gftyiacnw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gzlqafdfq.sHtML

[R73] 分割大日志
来源：http://blog.fktsv.cn/Article/details/glmqtwgec.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/gedesjhwh.sHtML

[R74] 批量重命名
来源：http://www.share.yfazqb.com/Article/details/gllnpnmhn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.sjlbkw.cn/Article/details/gcdxohisl.sHtML

[R75] 导出环境变量
来源：http://m.share.bbcook.cn/Article/details/gveftcsfe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.sjlbkw.cn/Article/details/gtwzmpxwr.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/gfnoxhesw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.epnwcf.com/Article/details/gqqexcpye.sHtML

[R77] 读取用户输入
来源：http://read.share.yfazqb.com/Article/details/goslntdbi.sHtML

read -rp "请输入: " ans
来源：http://baike.epnwcf.com/Article/details/gzktopqrm.sHtML

[R78] 交互式菜单
来源：http://m.share.bbcook.cn/Article/details/gzhbsmpyn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.bbcook.cn/Article/details/gqqvjeufw.sHtML

[R79] 解析命令行选项
来源：http://3g.vehdjk.com/Article/details/gfrabevcg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.vehdjk.com/Article/details/gnferntca.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.sjlbkw.cn/Article/details/gkoaevzaz.sHtML

time ./run.sh
来源：http://mobile.vehdjk.com/Article/details/gyeezkzbf.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gsohwjcoe.sHtML

S. C / C++ 专题
来源：http://wap.sjlbkw.cn/Article/details/grqicluwe.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/giuahtbrf.sHtML

[S01] C：Hello World
来源：http://mobile.epnwcf.com/Article/details/gkrqmltsp.sHtML

#include <stdio.h>
来源：http://www.blog.vehdjk.com/Article/details/gibgmkppe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.sjlbkw.cn/Article/details/gboomijaj.sHtML

[S02] C：变量与格式化输出
来源：http://wap.yfazqb.com/Article/details/gchcazpcp.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.yfazqb.com/Article/details/gwijrnexo.sHtML

[S03] C：读入整数
来源：http://www.m.share.sjlbkw.cn/Article/details/gigbuugkf.sHtML

int x; scanf("%d", &x);
来源：http://wap.epnwcf.com/Article/details/gjpgjmghj.sHtML

[S04] C：字符串复制
来源：http://www.share.vehdjk.com/Article/details/gcztyhtau.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.yfazqb.com/Article/details/grrbwcpss.sHtML

[S05] C：字符串长度
来源：http://baike.bbcook.cn/Article/details/gvsdmddma.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/gfdmkuduf.sHtML

[S06] C：字符串比较
来源：http://baike.yfazqb.com/Article/details/gmzennfah.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gqfdyuzfj.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fktsv.cn/Article/details/gseskxkxj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.yfazqb.com/Article/details/gbjofuxos.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/ggwbtpnut.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.yfazqb.com/Article/details/grmqwsxwy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.epnwcf.com/Article/details/grfebmaih.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.vehdjk.com/Article/details/gduplcxcs.sHtML

[S10] C：指针与解引用
来源：http://3g.epnwcf.com/Article/details/gipemalnw.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.tarul.cn/Article/details/gorytbqol.sHtML

[S11] C：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gvozsmmht.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.bbcook.cn/Article/details/gbhibsfmm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gesaycdzz.sHtML

fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gxsserahh.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/gylslwzes.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gyupbjydt.sHtML

[S13] C：宏定义
来源：http://wap.vehdjk.com/Article/details/geuaxjtsl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.bbcook.cn/Article/details/gmodmtwnn.sHtML

[S14] C：枚举
来源：http://read.share.fktsv.cn/Article/details/ghfrgkwms.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.epnwcf.com/Article/details/gmojzoqqq.sHtML

[S15] C：类型转换
来源：http://www.blog.fktsv.cn/Article/details/gmohqhwvb.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/gpmkvwxyd.sHtML

[S16] C：位操作置位
来源：http://3g.sjlbkw.cn/Article/details/ghdbxikvo.sHtML

x |= (1 << 3);
来源：http://blog.fktsv.cn/Article/details/gonalkucq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/gwjcflfzb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.bbcook.cn/Article/details/guaqpkwic.sHtML

[S18] C：命令行参数
来源：http://www.m.share.tarul.cn/Article/details/ghhryskms.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gobpuwdke.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/ggbormrta.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/ghuzfrnfr.sHtML

[S20] C：二分查找
来源：http://3g.tarul.cn/Article/details/gurooxslp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gogqyxmwy.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.yfazqb.com/Article/details/gaatgpjtd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/glrmmryja.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/gxeswrycy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/gbchbphts.sHtML

[S23] C：随机数
来源：http://www.m.share.fktsv.cn/Article/details/gktrlppuj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fktsv.cn/Article/details/gsofkxuvj.sHtML

[S24] C：获取本地时间
来源：http://baike.bbcook.cn/Article/details/gvlxhgyyu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.sjlbkw.cn/Article/details/gnnlcdnkb.sHtML

[S25] C：内存拷贝
来源：http://blog.tarul.cn/Article/details/ghxpqckgy.sHtML

memcpy(dst, src, n);
来源：http://read.share.sjlbkw.cn/Article/details/gizstutxb.sHtML

[S26] C：内存清零
来源：http://www.blog.bbcook.cn/Article/details/ggzkpyxpb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fktsv.cn/Article/details/gnhqdyzya.sHtML

[S27] C：定义常量
来源：http://www.blog.tarul.cn/Article/details/gioankrrw.sHtML

const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gghwzcgio.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/grcgowlpw.sHtML

static int counter = 0;
来源：http://read.share.bbcook.cn/Article/details/gyftxbgzk.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/ggsyzluks.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.sjlbkw.cn/Article/details/gxwbvvyrw.sHtML

[S30] C：头文件保护
来源：http://m.share.vehdjk.com/Article/details/gfyvoylua.sHtML

#ifndef X_H
来源：http://mobile.bbcook.cn/Article/details/gutjdnupk.sHtML

#define X_H
来源：http://blog.tarul.cn/Article/details/gaaozypap.sHtML

#endif
来源：http://baike.tarul.cn/Article/details/gtckpidmq.sHtML

[S31] C++：Hello World
来源：http://blog.bbcook.cn/Article/details/gfelamtju.sHtML

#include <iostream>
来源：http://www.blog.bbcook.cn/Article/details/gwhhonxng.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.yfazqb.com/Article/details/gsqakbwkz.sHtML

[S32] C++：字符串
来源：http://baike.bbcook.cn/Article/details/gltmqldjg.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.epnwcf.com/Article/details/gmetzgyev.sHtML


<!-- 参考信息 -->