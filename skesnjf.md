代发 wailian999

[Q61] 移动平均
来源：http://mobile.tarul.cn/Article/details/gtzhxpbid.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gjgmuvnfv.sHtML

[Q62] 分组占比
来源：http://read.share.yfazqb.com/Article/details/gmcprzviv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gcnpnnswb.sHtML

[Q63] 开启事务
来源：http://wap.vehdjk.com/Article/details/gecckvato.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.epnwcf.com/Article/details/goibaafiz.sHtML

[Q64] 提交事务
来源：http://read.share.yfazqb.com/Article/details/gpzkarmjv.sHtML

COMMIT;
来源：http://www.blog.fktsv.cn/Article/details/ghahdhhnb.sHtML

[Q65] 回滚事务
来源：http://m.share.yfazqb.com/Article/details/gocyjcupb.sHtML

ROLLBACK;
来源：http://3g.bbcook.cn/Article/details/geqwnnphy.sHtML

[Q66] 行锁查询
来源：http://3g.epnwcf.com/Article/details/guemysuqa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.sjlbkw.cn/Article/details/gpqqbopua.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.vehdjk.com/Article/details/gjlxtdslk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.vehdjk.com/Article/details/gpdgdgqnp.sHtML

[Q68] 保存点
来源：http://3g.yfazqb.com/Article/details/gampbylky.sHtML

SAVEPOINT sp1;
来源：http://baike.epnwcf.com/Article/details/gmnpecvdo.sHtML

ROLLBACK TO sp1;
来源：http://3g.vehdjk.com/Article/details/gjnxmmtrp.sHtML

[Q69] 查看执行计划
来源：http://baike.sjlbkw.cn/Article/details/gluyipoch.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.bbcook.cn/Article/details/gapoemphf.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/gkxqhdmma.sHtML

ANALYZE TABLE users;
来源：http://blog.sjlbkw.cn/Article/details/gxlcpghrq.sHtML

[Q71] 查看建表语句
来源：http://baike.bbcook.cn/Article/details/gpvokrvxn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.bbcook.cn/Article/details/gmaltkxci.sHtML

[Q72] 查看索引
来源：http://www.blog.bbcook.cn/Article/details/gcgghfzlp.sHtML

SHOW INDEX FROM users;
来源：http://3g.tarul.cn/Article/details/ginkepqmm.sHtML

[Q73] 查看表状态
来源：http://baike.epnwcf.com/Article/details/gagbilija.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.epnwcf.com/Article/details/gbqrewsfz.sHtML

[Q74] 强制使用索引
来源：http://3g.sjlbkw.cn/Article/details/ghsrlarwa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.yfazqb.com/Article/details/gprylnbud.sHtML

[Q75] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gvpjhybon.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.vehdjk.com/Article/details/gubnfwkvs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.vehdjk.com/Article/details/gzrjmsmqa.sHtML

[Q76] 按天统计
来源：http://www.m.share.yfazqb.com/Article/details/gdkcsduri.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.tarul.cn/Article/details/gsqnsbbgu.sHtML

[Q77] 时间加减
来源：http://3g.tarul.cn/Article/details/gjnombodr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.tarul.cn/Article/details/gsigkgdes.sHtML

[Q78] 当前时间
来源：http://mobile.vehdjk.com/Article/details/gfwtrhkzb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.tarul.cn/Article/details/gmwqzvbow.sHtML

[Q79] 字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gjlwlxvfx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.vehdjk.com/Article/details/gpphnmqaw.sHtML

[Q80] 字符串截取
来源：http://wap.yfazqb.com/Article/details/gcfhwgnfh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.yfazqb.com/Article/details/glklrjdfb.sHtML

[Q81] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/gjmxxdsgh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.yfazqb.com/Article/details/gzbyzvzgj.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fktsv.cn/Article/details/ggibrsawj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gcndwujor.sHtML

[Q83] 大小写转换
来源：http://3g.tarul.cn/Article/details/gnnwlyuil.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gqouzctzw.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/girxhsyuo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gumhiedha.sHtML

[Q85] 数值取整
来源：http://blog.epnwcf.com/Article/details/gxktxmqpg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.bbcook.cn/Article/details/grwbisthk.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.bbcook.cn/Article/details/gipbzevor.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.yfazqb.com/Article/details/gcavitwad.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.epnwcf.com/Article/details/gcvhgwsrc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.vehdjk.com/Article/details/ggunmbfpz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.epnwcf.com/Article/details/gtmgzligx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.sjlbkw.cn/Article/details/gdbtwmtuh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.epnwcf.com/Article/details/gwwqwtzsa.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fktsv.cn/Article/details/gevtnjlvc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.epnwcf.com/Article/details/gjygedvyi.sHtML

[Q90] 生成序号列
来源：http://wap.sjlbkw.cn/Article/details/gguormcms.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.vehdjk.com/Article/details/gbtxoizyn.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvphiahpr.sHtML

R. Bash 专题
来源：http://baike.fktsv.cn/Article/details/gykftnowc.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gsjuwngsr.sHtML

[R01] shebang 与严格模式
来源：http://m.share.tarul.cn/Article/details/ggefmpwxt.sHtML

#!/usr/bin/env bash
来源：http://wap.epnwcf.com/Article/details/gmswgmtzg.sHtML

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/gsucsikgn.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/gknnacflu.sHtML

name="Tom"; echo "$name"
来源：http://m.share.bbcook.cn/Article/details/gpnirdtte.sHtML

[R03] 只读变量
来源：http://www.m.share.yfazqb.com/Article/details/gdkzldbxl.sHtML

readonly PI=3.14
来源：http://www.m.share.tarul.cn/Article/details/gytxngkic.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/gogkueqra.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.yfazqb.com/Article/details/ghurezrke.sHtML

[R05] 参数默认值
来源：http://3g.bbcook.cn/Article/details/gkytmuhrq.sHtML

name="${1:-default}"
来源：http://wap.fktsv.cn/Article/details/gqdhmwdtu.sHtML

[R06] 判断命令是否存在
来源：http://mobile.vehdjk.com/Article/details/gfdnxpnmt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.sjlbkw.cn/Article/details/gfpmergxo.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gysqeyhwp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.tarul.cn/Article/details/gxhuzadcs.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/godtvwxan.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.yfazqb.com/Article/details/gbgoofzsq.sHtML

[R09] 字符串比较
来源：http://m.share.vehdjk.com/Article/details/goegqkcdc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.bbcook.cn/Article/details/giasldycz.sHtML

[R10] 正则匹配
来源：http://read.share.yfazqb.com/Article/details/gudxodjiu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.epnwcf.com/Article/details/gfbgtuaop.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gjzsruelm.sHtML

case "$1" in
来源：http://3g.sjlbkw.cn/Article/details/glaerpdyx.sHtML

start) echo "启动" ;;
来源：http://wap.bbcook.cn/Article/details/gbsfazrif.sHtML

stop)  echo "停止" ;;
来源：http://read.share.bbcook.cn/Article/details/gzfwldgrb.sHtML

*)     echo "未知命令" ;;
来源：http://blog.yfazqb.com/Article/details/gzfubbvqg.sHtML

esac
来源：http://m.share.tarul.cn/Article/details/gouvsynnx.sHtML

[R12] for 遍历文件
来源：http://mobile.yfazqb.com/Article/details/gudohinul.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.tarul.cn/Article/details/gmzwawkfu.sHtML

[R13] for 计数循环
来源：http://3g.epnwcf.com/Article/details/gpdjalrze.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gkaktakys.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/gqnzakijq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/getgccjmr.sHtML

[R15] while 逐行读文件
来源：http://www.share.tarul.cn/Article/details/grodahxux.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnaycqpn.sHtML

[R16] until 等待条件
来源：http://baike.tarul.cn/Article/details/gjemyqdeb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/godyffnfq.sHtML

[R17] 数组定义与取值
来源：http://www.share.epnwcf.com/Article/details/gnsszxmgk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.vehdjk.com/Article/details/gjamlxzhu.sHtML

[R18] 遍历数组
来源：http://www.blog.bbcook.cn/Article/details/gbfjaytgr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/gpjjnowtw.sHtML

[R19] 数组长度
来源：http://mobile.bbcook.cn/Article/details/gakqyzmah.sHtML

echo "${#arr[@]}"
来源：http://baike.epnwcf.com/Article/details/gjukvzqaw.sHtML

[R20] 关联数组（字典）
来源：http://blog.sjlbkw.cn/Article/details/gpvvgvtcb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.sjlbkw.cn/Article/details/gqnqpiuon.sHtML

[R21] 字符串长度
来源：http://blog.epnwcf.com/Article/details/gibfqdgaf.sHtML

echo "${#s}"
来源：http://www.share.tarul.cn/Article/details/gutptefrr.sHtML

[R22] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/gdoxsfcjq.sHtML

echo "${s:0:5}"
来源：http://www.m.share.epnwcf.com/Article/details/gjcifhnxs.sHtML

[R23] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gilntijkd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.yfazqb.com/Article/details/gjhcadkom.sHtML

[R24] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gekvagxii.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.bbcook.cn/Article/details/gkrdvkxnk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/gcxfyudtl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.sjlbkw.cn/Article/details/gczztauah.sHtML

[R26] 命令替换
来源：http://baike.fktsv.cn/Article/details/gvxoiwveh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fktsv.cn/Article/details/gwjvqbhce.sHtML

[R27] 算术展开
来源：http://mobile.vehdjk.com/Article/details/gyjnoioua.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/gjudvdysd.sHtML

[R28] 浮点运算
来源：http://3g.sjlbkw.cn/Article/details/gkihsdwkd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fktsv.cn/Article/details/gltcqzysh.sHtML

[R29] 定义函数
来源：http://blog.bbcook.cn/Article/details/gtwafvqaa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.bbcook.cn/Article/details/gfjemobev.sHtML

[R30] 函数返回状态码
来源：http://www.blog.tarul.cn/Article/details/gkywmajuf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.yfazqb.com/Article/details/gqohrnnsh.sHtML

[R31] 局部变量
来源：http://3g.tarul.cn/Article/details/gthmydifh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.epnwcf.com/Article/details/gkbqpgbyj.sHtML

[R32] 参数个数校验
来源：http://read.share.epnwcf.com/Article/details/gzkrneusl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gmcexmewa.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.bbcook.cn/Article/details/gskoyoycn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.epnwcf.com/Article/details/guvzegnom.sHtML

[R34] 退出时清理
来源：http://3g.epnwcf.com/Article/details/gnekidopa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gjlpemskd.sHtML

[R35] 后台执行并等待
来源：http://read.share.yfazqb.com/Article/details/gfyohnztn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.vehdjk.com/Article/details/grzmdsnrk.sHtML

[R36] 并发执行多个任务
来源：http://mobile.yfazqb.com/Article/details/gjlilzwjw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.bbcook.cn/Article/details/gnllszbrg.sHtML

[R37] 把输出赋给变量
来源：http://wap.vehdjk.com/Article/details/ganvvxzqi.sHtML

files=$(ls -1)
来源：http://3g.vehdjk.com/Article/details/gxlgwphab.sHtML

[R38] 管道串联
来源：http://blog.tarul.cn/Article/details/gpdzisanw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.sjlbkw.cn/Article/details/glrwqgrmz.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.bbcook.cn/Article/details/gkgptalpq.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fktsv.cn/Article/details/ghujvxrzs.sHtML

[R40] 追加写日志
来源：http://blog.bbcook.cn/Article/details/gzjniszye.sHtML

echo "log" >> out.log
来源：http://www.blog.epnwcf.com/Article/details/glwycsned.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/gvqyftuyi.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.epnwcf.com/Article/details/gjxzniiuf.sHtML

[R42] 输入重定向
来源：http://read.share.sjlbkw.cn/Article/details/gojpaxkxj.sHtML

wc -l < a.txt
来源：http://wap.bbcook.cn/Article/details/ggsemmejp.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/ghcwwbmtg.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fktsv.cn/Article/details/gcavjahvd.sHtML

[R44] 按修改时间查找
来源：http://wap.epnwcf.com/Article/details/gffszmcgj.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/guwovonou.sHtML

[R45] 批量删除
来源：http://m.share.fktsv.cn/Article/details/gmftdaskr.sHtML

find . -name "*.tmp" -delete
来源：http://wap.bbcook.cn/Article/details/ggaxnubkc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.vehdjk.com/Article/details/gyzzujuzr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/grxexdkhh.sHtML

[R47] sed 单行替换
来源：http://www.share.sjlbkw.cn/Article/details/gydxafmmp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fktsv.cn/Article/details/gdtutyrrb.sHtML

[R48] awk 取指定列
来源：http://blog.vehdjk.com/Article/details/ghzeaqxpj.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gzskqhjmi.sHtML

[R49] awk 带条件
来源：http://mobile.epnwcf.com/Article/details/gcejpmyru.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.bbcook.cn/Article/details/gjuhfenjm.sHtML

[R50] awk 求和
来源：http://www.blog.vehdjk.com/Article/details/gxeljywru.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/ghatstotk.sHtML

[R51] 排序去重取前几
来源：http://blog.vehdjk.com/Article/details/ggrfwexru.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.yfazqb.com/Article/details/gzkwpkwwi.sHtML

[R52] 统计行数
来源：http://read.share.tarul.cn/Article/details/ghbadhntu.sHtML

wc -l a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gwqdnuije.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.epnwcf.com/Article/details/gzugiiijt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.bbcook.cn/Article/details/gwvpjdowi.sHtML

[R54] 比较两个文件
来源：http://www.share.vehdjk.com/Article/details/gybptxorc.sHtML

diff a.txt b.txt
来源：http://baike.fktsv.cn/Article/details/gzeqmaoma.sHtML

[R55] 压缩与解压
来源：http://wap.yfazqb.com/Article/details/gzepwsltg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.epnwcf.com/Article/details/gqwdgntlr.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/guqmvjdut.sHtML

scp file user@host:/path/
来源：http://baike.fktsv.cn/Article/details/gsojrybrr.sHtML

[R57] 远程执行命令
来源：http://m.share.sjlbkw.cn/Article/details/gsofrguae.sHtML

ssh user@host 'uptime'
来源：http://3g.epnwcf.com/Article/details/ggermgtim.sHtML

[R58] 下载文件
来源：http://www.m.share.fktsv.cn/Article/details/gdidjmnlu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/gsjmidzzk.sHtML

[R59] 发 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gktzscitt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fktsv.cn/Article/details/gwakivatg.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gzixooxzq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.epnwcf.com/Article/details/gyrvbsoex.sHtML

[R61] 磁盘占用
来源：http://m.share.epnwcf.com/Article/details/gefjmiutp.sHtML

df -h;  du -sh *
来源：http://www.m.share.bbcook.cn/Article/details/giakwhuow.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/gxxnahmim.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.sjlbkw.cn/Article/details/ggvogbycn.sHtML

[R63] 内存与进程
来源：http://www.blog.tarul.cn/Article/details/gaavonnsv.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.tarul.cn/Article/details/gswrumcff.sHtML

[R64] 结束进程
来源：http://www.share.fktsv.cn/Article/details/gsimbosue.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.epnwcf.com/Article/details/gtqxpxxdm.sHtML

[R65] 查看端口占用
来源：http://mobile.vehdjk.com/Article/details/gvlrweedc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.sjlbkw.cn/Article/details/ghnfjiofg.sHtML

[R66] 定时任务
来源：http://www.share.tarul.cn/Article/details/gucyepgbg.sHtML

crontab -e;  crontab -l
来源：http://baike.bbcook.cn/Article/details/gmctbdlku.sHtML

[R67] 生成随机十六进制串
来源：http://baike.bbcook.cn/Article/details/gfwuuqlcn.sHtML

openssl rand -hex 16
来源：http://mobile.tarul.cn/Article/details/gbopgzemo.sHtML

[R68] 计算文件校验值
来源：http://www.share.sjlbkw.cn/Article/details/gnsxycalr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gxttqlbwb.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fktsv.cn/Article/details/gpsipntbu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.sjlbkw.cn/Article/details/gzxtfculu.sHtML

[R70] 时间戳与互转
来源：http://www.share.tarul.cn/Article/details/gbjikgcqh.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fktsv.cn/Article/details/gwbggyeuq.sHtML

[R71] 日期格式化
来源：http://m.share.sjlbkw.cn/Article/details/gjpifkfoc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.epnwcf.com/Article/details/gwdboqxif.sHtML

[R72] 等待端口就绪
来源：http://baike.tarul.cn/Article/details/gfeziehwu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gkpzxgfyh.sHtML

[R73] 分割大日志
来源：http://wap.epnwcf.com/Article/details/gndzkxhtq.sHtML

split -l 1000 big.log part_
来源：http://wap.epnwcf.com/Article/details/gnmcqtdzm.sHtML

[R74] 批量重命名
来源：http://blog.fktsv.cn/Article/details/glfkiibkt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.bbcook.cn/Article/details/gzwwluurw.sHtML

[R75] 导出环境变量
来源：http://www.blog.epnwcf.com/Article/details/gbkedlwbo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.bbcook.cn/Article/details/gosvfdqar.sHtML

[R76] 使用临时文件
来源：http://wap.vehdjk.com/Article/details/godaxhyfm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gvlgpdkte.sHtML

[R77] 读取用户输入
来源：http://mobile.yfazqb.com/Article/details/gggwctbvk.sHtML

read -rp "请输入: " ans
来源：http://www.blog.tarul.cn/Article/details/gsitsihwb.sHtML

[R78] 交互式菜单
来源：http://baike.vehdjk.com/Article/details/gapqtxojq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.bbcook.cn/Article/details/gaigovbsw.sHtML

[R79] 解析命令行选项
来源：http://blog.bbcook.cn/Article/details/grodpjmqp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/gjsqzagnd.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.tarul.cn/Article/details/ggexochbp.sHtML

time ./run.sh
来源：http://m.share.vehdjk.com/Article/details/gedsohkuq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gdvwizkmy.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/gutmffney.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gugecyakg.sHtML

[S01] C：Hello World
来源：http://baike.tarul.cn/Article/details/gkijlmnyj.sHtML

#include <stdio.h>
来源：http://mobile.fktsv.cn/Article/details/gumcxhuvx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.epnwcf.com/Article/details/gaoxtczfj.sHtML

[S02] C：变量与格式化输出
来源：http://wap.vehdjk.com/Article/details/gcuiqfywr.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/gsdmpmheh.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gzgeigunc.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fktsv.cn/Article/details/gbxonvwvk.sHtML

[S04] C：字符串复制
来源：http://wap.fktsv.cn/Article/details/gklijijlb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.epnwcf.com/Article/details/gauzedben.sHtML

[S05] C：字符串长度
来源：http://www.blog.bbcook.cn/Article/details/goaotbzwf.sHtML

strlen(s)
来源：http://blog.vehdjk.com/Article/details/gjnufkrcl.sHtML

[S06] C：字符串比较
来源：http://3g.vehdjk.com/Article/details/gmbvlxdsv.sHtML

strcmp(a, b) == 0
来源：http://blog.sjlbkw.cn/Article/details/gfvtxeekr.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.yfazqb.com/Article/details/gnefomkvh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.sjlbkw.cn/Article/details/gtdkdktcv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.tarul.cn/Article/details/govgpkfhx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.bbcook.cn/Article/details/gtvulgnon.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.yfazqb.com/Article/details/ggcauliyg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/gcxxkbsku.sHtML

[S10] C：指针与解引用
来源：http://baike.bbcook.cn/Article/details/gkbjmpufz.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.yfazqb.com/Article/details/gqeqnnmis.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gohannlel.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.tarul.cn/Article/details/grsudjttf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.bbcook.cn/Article/details/gyimtpesn.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/gseoblvql.sHtML

[S12] C：写文件
来源：http://m.share.yfazqb.com/Article/details/gwyxwgdkg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.tarul.cn/Article/details/gzxjuziat.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gnkdwgpdk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.tarul.cn/Article/details/gtqdqnqru.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/gaqnzwcke.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/gsaiulwhr.sHtML

[S15] C：类型转换
来源：http://blog.fktsv.cn/Article/details/gbtkbivjc.sHtML

(double) a / b
来源：http://www.m.share.bbcook.cn/Article/details/gcnupurak.sHtML

[S16] C：位操作置位
来源：http://www.m.share.vehdjk.com/Article/details/guavxphdr.sHtML

x |= (1 << 3);
来源：http://3g.yfazqb.com/Article/details/gezqlgheo.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/gwobbgzar.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.tarul.cn/Article/details/gmrtekvlf.sHtML

[S18] C：命令行参数
来源：http://m.share.bbcook.cn/Article/details/gooiozbzu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.vehdjk.com/Article/details/ggmiudnva.sHtML

[S19] C：快速排序
来源：http://m.share.vehdjk.com/Article/details/ghmjhnefn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gcummowbv.sHtML

[S20] C：二分查找
来源：http://3g.fktsv.cn/Article/details/gpxksijfn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/ghtoykulj.sHtML

[S21] C：字符类别判断
来源：http://mobile.yfazqb.com/Article/details/gkqvklqob.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.sjlbkw.cn/Article/details/gfwkmczfd.sHtML

[S22] C：字符串转数字
来源：http://3g.bbcook.cn/Article/details/gcfwgqyft.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.sjlbkw.cn/Article/details/grquavozj.sHtML

[S23] C：随机数
来源：http://www.share.fktsv.cn/Article/details/ghiiizkrt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.tarul.cn/Article/details/ghgeulcpf.sHtML

[S24] C：获取本地时间
来源：http://www.share.bbcook.cn/Article/details/goithgtew.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/gjjmcosko.sHtML

[S25] C：内存拷贝
来源：http://mobile.fktsv.cn/Article/details/gaahrptqs.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.vehdjk.com/Article/details/golebsoat.sHtML

[S26] C：内存清零
来源：http://www.share.vehdjk.com/Article/details/gmjlhshmk.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.epnwcf.com/Article/details/gacpymyxu.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/guyecfzzb.sHtML

const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/ghqzaswsd.sHtML

[S28] C：静态变量
来源：http://m.share.vehdjk.com/Article/details/gnamuddsb.sHtML

static int counter = 0;
来源：http://www.blog.bbcook.cn/Article/details/gyqvtmbju.sHtML

[S29] C：变参函数
来源：http://mobile.bbcook.cn/Article/details/gbugfqevk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.tarul.cn/Article/details/gbymelmxz.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/gmfdfplnb.sHtML

#ifndef X_H
来源：http://3g.vehdjk.com/Article/details/ggrufziwl.sHtML

#define X_H
来源：http://www.share.bbcook.cn/Article/details/gtgyaheoa.sHtML

#endif
来源：http://www.m.share.vehdjk.com/Article/details/gowdsjoob.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/gxmkpqvjr.sHtML


<!-- 参考信息 -->