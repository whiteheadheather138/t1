代发 wailian999

[Q65] 回滚事务
来源：http://www.blog.sjlbkw.cn/Article/details/grrqhbepv.sHtML

ROLLBACK;
来源：http://3g.sjlbkw.cn/Article/details/gsgozoorp.sHtML

[Q66] 行锁查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqnfzcka.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fktsv.cn/Article/details/gbncadjmb.sHtML

[Q67] 设置隔离级别
来源：http://read.share.vehdjk.com/Article/details/gzajsvmab.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.sjlbkw.cn/Article/details/gjcwwooau.sHtML

[Q68] 保存点
来源：http://m.share.fktsv.cn/Article/details/gqctqqcvl.sHtML

SAVEPOINT sp1;
来源：http://www.blog.vehdjk.com/Article/details/gswgcpiae.sHtML

ROLLBACK TO sp1;
来源：http://wap.fktsv.cn/Article/details/gymowapdb.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gpojreuke.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.yfazqb.com/Article/details/gqkrwpsdw.sHtML

[Q70] 更新统计信息
来源：http://www.share.epnwcf.com/Article/details/gsuzlpqvm.sHtML

ANALYZE TABLE users;
来源：http://read.share.epnwcf.com/Article/details/gqnidmwfx.sHtML

[Q71] 查看建表语句
来源：http://www.blog.yfazqb.com/Article/details/geieuomaq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.sjlbkw.cn/Article/details/gygflmafy.sHtML

[Q72] 查看索引
来源：http://3g.bbcook.cn/Article/details/gyhafrrde.sHtML

SHOW INDEX FROM users;
来源：http://mobile.epnwcf.com/Article/details/gyaqtdvdn.sHtML

[Q73] 查看表状态
来源：http://m.share.bbcook.cn/Article/details/gdzqmtxpp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.sjlbkw.cn/Article/details/gunvilypz.sHtML

[Q74] 强制使用索引
来源：http://www.share.epnwcf.com/Article/details/gsaatrdyg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.yfazqb.com/Article/details/gtuumjccm.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gwfiofert.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.yfazqb.com/Article/details/gpshkqdyt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/gapfnpgbh.sHtML

[Q76] 按天统计
来源：http://read.share.epnwcf.com/Article/details/gxpeeenpu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.tarul.cn/Article/details/ghyyxexsw.sHtML

[Q77] 时间加减
来源：http://read.share.vehdjk.com/Article/details/gratowqiv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.bbcook.cn/Article/details/goqbqmlom.sHtML

[Q78] 当前时间
来源：http://baike.bbcook.cn/Article/details/ggkceirht.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.yfazqb.com/Article/details/gijnesjvx.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gdrqwomww.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.bbcook.cn/Article/details/gqkenmnym.sHtML

[Q80] 字符串截取
来源：http://wap.bbcook.cn/Article/details/gnecuuigt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.tarul.cn/Article/details/ghqyjtczn.sHtML

[Q81] 字符串替换
来源：http://3g.fktsv.cn/Article/details/ggvqgpftp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.epnwcf.com/Article/details/gwjquhubz.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.sjlbkw.cn/Article/details/gwdpxnuhb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gwoyysjto.sHtML

[Q83] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gwloqawni.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gyzddpnwb.sHtML

[Q84] 去除首尾空格
来源：http://read.share.yfazqb.com/Article/details/glskockcf.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gzxfqwtdv.sHtML

[Q85] 数值取整
来源：http://www.m.share.yfazqb.com/Article/details/ghbgsuvta.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.bbcook.cn/Article/details/gaszssotw.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.bbcook.cn/Article/details/griijmnee.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.yfazqb.com/Article/details/ghiwbulzt.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fktsv.cn/Article/details/ggeugegqc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/gaqolzuxu.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fktsv.cn/Article/details/gvewderew.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.vehdjk.com/Article/details/ghbawppey.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.epnwcf.com/Article/details/gojimgprp.sHtML

[Q89] 判断表是否存在
来源：http://blog.sjlbkw.cn/Article/details/gyqxfvwjq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fktsv.cn/Article/details/gpxdjiqmy.sHtML

[Q90] 生成序号列
来源：http://baike.sjlbkw.cn/Article/details/gogwizsyt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.tarul.cn/Article/details/gaxpduzlk.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gbxwrwpmk.sHtML

R. Bash 专题
来源：http://read.share.bbcook.cn/Article/details/gdghcpbfh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ghrpwiqmm.sHtML

[R01] shebang 与严格模式
来源：http://3g.sjlbkw.cn/Article/details/gmsgtduwj.sHtML

#!/usr/bin/env bash
来源：http://read.share.epnwcf.com/Article/details/gkevxbxhb.sHtML

set -euo pipefail
来源：http://mobile.epnwcf.com/Article/details/gfejesres.sHtML

[R02] 变量赋值与使用
来源：http://m.share.bbcook.cn/Article/details/gfwaxahfq.sHtML

name="Tom"; echo "$name"
来源：http://mobile.epnwcf.com/Article/details/gqguxxjsj.sHtML

[R03] 只读变量
来源：http://3g.fktsv.cn/Article/details/gqlbrqzqh.sHtML

readonly PI=3.14
来源：http://mobile.tarul.cn/Article/details/gehjlavfi.sHtML

[R04] 位置参数
来源：http://www.share.vehdjk.com/Article/details/gmejozfjy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjeiwxzpw.sHtML

[R05] 参数默认值
来源：http://read.share.bbcook.cn/Article/details/ghajpnbik.sHtML

name="${1:-default}"
来源：http://www.m.share.epnwcf.com/Article/details/glnmjktzk.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/gfyhyvvkx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gpezbgzcu.sHtML

[R07] if 判断文件
来源：http://read.share.fktsv.cn/Article/details/gygkredfp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.yfazqb.com/Article/details/gpsrfwqmt.sHtML

[R08] 数值比较
来源：http://wap.sjlbkw.cn/Article/details/gyvmavpon.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gfydmyhoo.sHtML

[R09] 字符串比较
来源：http://3g.tarul.cn/Article/details/geaudtzty.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.vehdjk.com/Article/details/gqcaarsus.sHtML

[R10] 正则匹配
来源：http://baike.sjlbkw.cn/Article/details/gdcwewbso.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.tarul.cn/Article/details/gerexsmuh.sHtML

[R11] case 多分支
来源：http://mobile.tarul.cn/Article/details/gedfbppka.sHtML

case "$1" in
来源：http://wap.bbcook.cn/Article/details/ghdobulgy.sHtML

start) echo "启动" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/goimtirrq.sHtML

stop)  echo "停止" ;;
来源：http://baike.fktsv.cn/Article/details/gcyeerfsg.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gzkethobv.sHtML

esac
来源：http://wap.sjlbkw.cn/Article/details/gmisxyokh.sHtML

[R12] for 遍历文件
来源：http://3g.epnwcf.com/Article/details/gozgfkuvp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.epnwcf.com/Article/details/gmoxqqjwa.sHtML

[R13] for 计数循环
来源：http://read.share.sjlbkw.cn/Article/details/gkoswnzln.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/gsbiwgxri.sHtML

[R14] C 风格 for
来源：http://baike.fktsv.cn/Article/details/ghdvohfez.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/gjvzfgeoq.sHtML

[R15] while 逐行读文件
来源：http://mobile.tarul.cn/Article/details/gepkodtwd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.epnwcf.com/Article/details/gbkuztecg.sHtML

[R16] until 等待条件
来源：http://blog.bbcook.cn/Article/details/gmetticob.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gwnxbncyj.sHtML

[R17] 数组定义与取值
来源：http://www.blog.yfazqb.com/Article/details/gqmgvwhih.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.vehdjk.com/Article/details/gxogtybkt.sHtML

[R18] 遍历数组
来源：http://wap.vehdjk.com/Article/details/ggovnmpyi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.bbcook.cn/Article/details/gmmfoycfq.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/gtffimzfg.sHtML

echo "${#arr[@]}"
来源：http://blog.bbcook.cn/Article/details/gkivkjnog.sHtML

[R20] 关联数组（字典）
来源：http://3g.epnwcf.com/Article/details/gvdzfnjzp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.tarul.cn/Article/details/glkerjydy.sHtML

[R21] 字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gafryvsim.sHtML

echo "${#s}"
来源：http://m.share.bbcook.cn/Article/details/gjowybzhs.sHtML

[R22] 截取子串
来源：http://m.share.tarul.cn/Article/details/gpsasnfai.sHtML

echo "${s:0:5}"
来源：http://3g.tarul.cn/Article/details/gjsunksmx.sHtML

[R23] 字符串替换
来源：http://www.blog.fktsv.cn/Article/details/gmtgczdkl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.vehdjk.com/Article/details/galrjhhpp.sHtML

[R24] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/glhxdetkg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.epnwcf.com/Article/details/gjkjtvxsz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.epnwcf.com/Article/details/gxgbgaizp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.bbcook.cn/Article/details/gdozokxcp.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/gabdbohrd.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.bbcook.cn/Article/details/gmyaljoui.sHtML

[R27] 算术展开
来源：http://www.blog.epnwcf.com/Article/details/gctebuucz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.tarul.cn/Article/details/ggrlhquxg.sHtML

[R28] 浮点运算
来源：http://blog.yfazqb.com/Article/details/gxdljhqjd.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.vehdjk.com/Article/details/gcdqgbahf.sHtML

[R29] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gmpvrxqkc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/glodcyuor.sHtML

[R30] 函数返回状态码
来源：http://read.share.epnwcf.com/Article/details/gqjzynzxz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fktsv.cn/Article/details/gjvcxqzov.sHtML

[R31] 局部变量
来源：http://read.share.yfazqb.com/Article/details/gkjapiyov.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.epnwcf.com/Article/details/gpgjzugke.sHtML

[R32] 参数个数校验
来源：http://www.blog.bbcook.cn/Article/details/gosuzsgas.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gajtaeqmd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.yfazqb.com/Article/details/gqzgqvfte.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.epnwcf.com/Article/details/gbhjbcqgu.sHtML

[R34] 退出时清理
来源：http://www.share.vehdjk.com/Article/details/gekqlxyea.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/guvnubotk.sHtML

[R35] 后台执行并等待
来源：http://read.share.vehdjk.com/Article/details/gvfjyjjwh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.epnwcf.com/Article/details/gaigjnbjo.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fktsv.cn/Article/details/gatcfnxmo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.sjlbkw.cn/Article/details/goullmlzf.sHtML

[R37] 把输出赋给变量
来源：http://blog.tarul.cn/Article/details/gkxkjblrl.sHtML

files=$(ls -1)
来源：http://read.share.vehdjk.com/Article/details/guiedmiuw.sHtML

[R38] 管道串联
来源：http://blog.bbcook.cn/Article/details/gbwelspra.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.vehdjk.com/Article/details/gmozaokxt.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/gsxagruan.sHtML

cmd > out.log 2>&1
来源：http://m.share.yfazqb.com/Article/details/gjvjqfhkc.sHtML

[R40] 追加写日志
来源：http://www.share.sjlbkw.cn/Article/details/gpcwqkobo.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/gzhyxvigw.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/glupwszqe.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.vehdjk.com/Article/details/gavxgdgqd.sHtML

[R42] 输入重定向
来源：http://www.blog.epnwcf.com/Article/details/gpjjofcnw.sHtML

wc -l < a.txt
来源：http://3g.bbcook.cn/Article/details/gdanlmbls.sHtML

[R43] 按名字查找文件
来源：http://wap.tarul.cn/Article/details/gnnixqrww.sHtML

find . -name "*.log" -type f
来源：http://wap.epnwcf.com/Article/details/grthzqcfz.sHtML

[R44] 按修改时间查找
来源：http://baike.fktsv.cn/Article/details/gnoyluujw.sHtML

find . -mtime -7 -type f
来源：http://baike.bbcook.cn/Article/details/gqsesutvq.sHtML

[R45] 批量删除
来源：http://blog.bbcook.cn/Article/details/gwjnehtid.sHtML

find . -name "*.tmp" -delete
来源：http://3g.yfazqb.com/Article/details/geaaphcvc.sHtML

[R46] 递归替换文件内容
来源：http://3g.yfazqb.com/Article/details/garzaahrm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.vehdjk.com/Article/details/gpyokrmwm.sHtML

[R47] sed 单行替换
来源：http://www.share.sjlbkw.cn/Article/details/glsgpfklx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.tarul.cn/Article/details/glpwjyvnv.sHtML

[R48] awk 取指定列
来源：http://3g.fktsv.cn/Article/details/gyiopcsjc.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.vehdjk.com/Article/details/gyxfdcqok.sHtML

[R49] awk 带条件
来源：http://blog.bbcook.cn/Article/details/gvabbffft.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.sjlbkw.cn/Article/details/gabeukiej.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/guqhhbkms.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.tarul.cn/Article/details/ghvulilxu.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/gvaoxobvt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fktsv.cn/Article/details/gjgmbrrkw.sHtML

[R52] 统计行数
来源：http://read.share.tarul.cn/Article/details/gslybuysk.sHtML

wc -l a.txt
来源：http://baike.fktsv.cn/Article/details/gduxszteu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.yfazqb.com/Article/details/guzxqiubb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fktsv.cn/Article/details/ggntisaer.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/gblilauwj.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/gnvdzvetk.sHtML

[R55] 压缩与解压
来源：http://3g.yfazqb.com/Article/details/gwftbgbrw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.tarul.cn/Article/details/ggevpycfv.sHtML

[R56] 远程拷贝
来源：http://baike.sjlbkw.cn/Article/details/geacixjxk.sHtML

scp file user@host:/path/
来源：http://blog.sjlbkw.cn/Article/details/gyoxokviy.sHtML

[R57] 远程执行命令
来源：http://mobile.sjlbkw.cn/Article/details/gdjudrmco.sHtML

ssh user@host 'uptime'
来源：http://www.share.fktsv.cn/Article/details/gwmhjnuwe.sHtML

[R58] 下载文件
来源：http://blog.bbcook.cn/Article/details/gdrndfaco.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/gqiedcvve.sHtML

[R59] 发 POST JSON
来源：http://baike.fktsv.cn/Article/details/gwhzgtbko.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.vehdjk.com/Article/details/gslvmrzgl.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/gvvhqnrcf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.tarul.cn/Article/details/gzyzppkvq.sHtML

[R61] 磁盘占用
来源：http://m.share.tarul.cn/Article/details/ghfnuborc.sHtML

df -h;  du -sh *
来源：http://read.share.sjlbkw.cn/Article/details/geccrqnhq.sHtML

[R62] 找最占空间的文件
来源：http://baike.epnwcf.com/Article/details/gefzubwvk.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.vehdjk.com/Article/details/gobyeqyph.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/gcuomysmr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.yfazqb.com/Article/details/ghnvnlocx.sHtML

[R64] 结束进程
来源：http://mobile.sjlbkw.cn/Article/details/gtqbydjjp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.epnwcf.com/Article/details/gqyzarltx.sHtML

[R65] 查看端口占用
来源：http://mobile.sjlbkw.cn/Article/details/gjzwenhdg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.epnwcf.com/Article/details/ggsuccpgj.sHtML

[R66] 定时任务
来源：http://baike.sjlbkw.cn/Article/details/gkypodcuh.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/gkpjrbsyy.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.sjlbkw.cn/Article/details/gondcqzab.sHtML

openssl rand -hex 16
来源：http://www.share.epnwcf.com/Article/details/gvtxmwrxg.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/gnksdpmgu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.bbcook.cn/Article/details/gygbkcvtp.sHtML

[R69] 生成随机密码
来源：http://www.share.tarul.cn/Article/details/gambfhlfh.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.sjlbkw.cn/Article/details/groadeptw.sHtML

[R70] 时间戳与互转
来源：http://wap.bbcook.cn/Article/details/gakejpxkg.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.vehdjk.com/Article/details/gxmpfeted.sHtML

[R71] 日期格式化
来源：http://baike.vehdjk.com/Article/details/gqeciqwbr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqtojgge.sHtML

[R72] 等待端口就绪
来源：http://mobile.tarul.cn/Article/details/ghzcxkldb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gzrkqluyk.sHtML

[R73] 分割大日志
来源：http://wap.tarul.cn/Article/details/gqllsjxxs.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/gxwtbrnin.sHtML

[R74] 批量重命名
来源：http://m.share.fktsv.cn/Article/details/gblbylxfd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.bbcook.cn/Article/details/gpyuuneqs.sHtML

[R75] 导出环境变量
来源：http://www.blog.vehdjk.com/Article/details/gwldoeovq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.epnwcf.com/Article/details/ganfzhbvt.sHtML

[R76] 使用临时文件
来源：http://mobile.epnwcf.com/Article/details/gielcdwqc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gxqlmtves.sHtML

[R77] 读取用户输入
来源：http://m.share.vehdjk.com/Article/details/gkgtxgsea.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/gkgcmiamd.sHtML

[R78] 交互式菜单
来源：http://wap.sjlbkw.cn/Article/details/gwuirzygm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/ggzpiemlg.sHtML

[R79] 解析命令行选项
来源：http://blog.bbcook.cn/Article/details/gdqyitbqf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.sjlbkw.cn/Article/details/gbmgeyqgk.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.sjlbkw.cn/Article/details/gknsmvjwa.sHtML

time ./run.sh
来源：http://3g.fktsv.cn/Article/details/guezeqpfi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ghftzukxa.sHtML

S. C / C++ 专题
来源：http://blog.sjlbkw.cn/Article/details/gvcimuinm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gtpemvehz.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/glfcmpoxk.sHtML

#include <stdio.h>
来源：http://www.share.yfazqb.com/Article/details/gjlndypzc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.vehdjk.com/Article/details/gmwcjejbm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fktsv.cn/Article/details/gmtlfweks.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.epnwcf.com/Article/details/gklearqov.sHtML

[S03] C：读入整数
来源：http://wap.vehdjk.com/Article/details/geavuxhmj.sHtML

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/gwnpojeet.sHtML

[S04] C：字符串复制
来源：http://wap.sjlbkw.cn/Article/details/gboadogxu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.vehdjk.com/Article/details/gtvhabrfu.sHtML

[S05] C：字符串长度
来源：http://blog.epnwcf.com/Article/details/govotqkir.sHtML

strlen(s)
来源：http://3g.epnwcf.com/Article/details/gaxgvzyru.sHtML

[S06] C：字符串比较
来源：http://3g.bbcook.cn/Article/details/gysqzobnb.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/glxymdgsr.sHtML

[S07] C：数组遍历求和
来源：http://blog.sjlbkw.cn/Article/details/gxddovpli.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.epnwcf.com/Article/details/gunulkxzm.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.tarul.cn/Article/details/gbxgcxivo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.vehdjk.com/Article/details/ggpslmbsn.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.vehdjk.com/Article/details/geccndfev.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.tarul.cn/Article/details/gknvgtpxo.sHtML

[S10] C：指针与解引用
来源：http://m.share.yfazqb.com/Article/details/gwyijukze.sHtML

int *p = &a;  *p = 5;
来源：http://blog.bbcook.cn/Article/details/gwqohkqfg.sHtML

[S11] C：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gwiscjifx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.bbcook.cn/Article/details/gupyrrovx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.yfazqb.com/Article/details/gtoddsrbd.sHtML

fclose(f);
来源：http://3g.fktsv.cn/Article/details/gdvhxouno.sHtML

[S12] C：写文件
来源：http://blog.yfazqb.com/Article/details/gizoebvog.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.yfazqb.com/Article/details/gbpwfaycb.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gpijpayxl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.tarul.cn/Article/details/gsbmxvjzt.sHtML

[S14] C：枚举
来源：http://wap.sjlbkw.cn/Article/details/gypdbwbed.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fktsv.cn/Article/details/gnewefoyb.sHtML

[S15] C：类型转换
来源：http://wap.fktsv.cn/Article/details/gisnaqyeb.sHtML

(double) a / b
来源：http://wap.yfazqb.com/Article/details/gsbejnnuu.sHtML

[S16] C：位操作置位
来源：http://3g.sjlbkw.cn/Article/details/glnaibcjl.sHtML

x |= (1 << 3);
来源：http://www.m.share.vehdjk.com/Article/details/geflnykxj.sHtML

[S17] C：安全拼接字符串
来源：http://wap.bbcook.cn/Article/details/gufylfijf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.sjlbkw.cn/Article/details/gayikvqvu.sHtML

[S18] C：命令行参数
来源：http://www.share.yfazqb.com/Article/details/gtykmvphr.sHtML

int main(int argc, char **argv)
来源：http://blog.sjlbkw.cn/Article/details/gordrrveg.sHtML

[S19] C：快速排序
来源：http://3g.yfazqb.com/Article/details/gzojxsfks.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/ghysmrsaw.sHtML

[S20] C：二分查找
来源：http://baike.sjlbkw.cn/Article/details/gnlvlxxvu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/gzmibgzwl.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.bbcook.cn/Article/details/gyulgwebb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.epnwcf.com/Article/details/gxttzlfse.sHtML

[S22] C：字符串转数字
来源：http://m.share.vehdjk.com/Article/details/gacemhnwc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/gutnwgvtu.sHtML

[S23] C：随机数
来源：http://www.share.yfazqb.com/Article/details/gokywdtxf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fktsv.cn/Article/details/goieiatxj.sHtML

[S24] C：获取本地时间
来源：http://blog.tarul.cn/Article/details/gzgbddkbc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.bbcook.cn/Article/details/grrlmdpyy.sHtML

[S25] C：内存拷贝
来源：http://www.share.vehdjk.com/Article/details/gnnnpqikw.sHtML

memcpy(dst, src, n);
来源：http://blog.yfazqb.com/Article/details/gutfjumon.sHtML

[S26] C：内存清零
来源：http://wap.sjlbkw.cn/Article/details/glpbxsdro.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fktsv.cn/Article/details/gbynbwsgm.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/gqpgdllol.sHtML

const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/ghrnigpoc.sHtML

[S28] C：静态变量
来源：http://3g.fktsv.cn/Article/details/gjmocvabl.sHtML

static int counter = 0;
来源：http://mobile.tarul.cn/Article/details/gnxayvdof.sHtML

[S29] C：变参函数
来源：http://www.blog.bbcook.cn/Article/details/gxbtqxohz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.sjlbkw.cn/Article/details/gfdghyhtp.sHtML

[S30] C：头文件保护
来源：http://www.share.sjlbkw.cn/Article/details/gpmzxwzev.sHtML

#ifndef X_H
来源：http://blog.vehdjk.com/Article/details/gqikkzvcc.sHtML

#define X_H
来源：http://www.m.share.yfazqb.com/Article/details/gfzjeapmo.sHtML

#endif
来源：http://read.share.bbcook.cn/Article/details/gucahyfzu.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/ggfitxmhc.sHtML

#include <iostream>
来源：http://www.blog.bbcook.cn/Article/details/gjnlujwfg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.bbcook.cn/Article/details/gwftqxpxq.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gxtfxebmx.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fktsv.cn/Article/details/gbmqehlhu.sHtML

[S33] C++：vector 增删
来源：http://read.share.yfazqb.com/Article/details/gndjodsjh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.vehdjk.com/Article/details/gsrlqbjjq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fktsv.cn/Article/details/gdeznvrdr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fktsv.cn/Article/details/giyxtppjh.sHtML


<!-- 参考信息 -->