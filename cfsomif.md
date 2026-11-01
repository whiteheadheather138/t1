代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.yfazqb.com/Article/details/grlulotpj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.bbcook.cn/Article/details/gfmpmmsam.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gvsclrnho.sHtML

[Q57] 行号
来源：http://read.share.sjlbkw.cn/Article/details/gajqrqhhu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gyccnxhuz.sHtML

[Q58] 累计求和
来源：http://baike.sjlbkw.cn/Article/details/gxmgvmhei.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.vehdjk.com/Article/details/glkxbsbxs.sHtML

[Q59] 分组内累计
来源：http://blog.tarul.cn/Article/details/glwwvnhpx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gfgncqgpg.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.sjlbkw.cn/Article/details/gycfwsluw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.bbcook.cn/Article/details/gzilqqhmn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.tarul.cn/Article/details/gpeokcrvu.sHtML

[Q61] 移动平均
来源：http://blog.tarul.cn/Article/details/gbtksvprf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gdvncqlbt.sHtML

[Q62] 分组占比
来源：http://baike.bbcook.cn/Article/details/grjwtqghq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gusremgxt.sHtML

[Q63] 开启事务
来源：http://blog.fktsv.cn/Article/details/gvbbyjqpk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.epnwcf.com/Article/details/gqaacjdbo.sHtML

[Q64] 提交事务
来源：http://3g.vehdjk.com/Article/details/gcalrvxuj.sHtML

COMMIT;
来源：http://www.blog.yfazqb.com/Article/details/gnceczhrs.sHtML

[Q65] 回滚事务
来源：http://www.m.share.tarul.cn/Article/details/gbrlamtyf.sHtML

ROLLBACK;
来源：http://read.share.epnwcf.com/Article/details/gwogiujzn.sHtML

[Q66] 行锁查询
来源：http://m.share.sjlbkw.cn/Article/details/gqkpqglzu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.tarul.cn/Article/details/gbrhvlbzg.sHtML

[Q67] 设置隔离级别
来源：http://m.share.bbcook.cn/Article/details/gygwzvwmz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fktsv.cn/Article/details/gipavbidk.sHtML

[Q68] 保存点
来源：http://3g.yfazqb.com/Article/details/gcsobraqu.sHtML

SAVEPOINT sp1;
来源：http://www.share.sjlbkw.cn/Article/details/ggfrytbub.sHtML

ROLLBACK TO sp1;
来源：http://3g.vehdjk.com/Article/details/gspptgvgm.sHtML

[Q69] 查看执行计划
来源：http://m.share.epnwcf.com/Article/details/gguebutke.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.vehdjk.com/Article/details/gjnlketyo.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/gibesjvav.sHtML

ANALYZE TABLE users;
来源：http://read.share.vehdjk.com/Article/details/gvpmfqdsa.sHtML

[Q71] 查看建表语句
来源：http://www.share.bbcook.cn/Article/details/gpgftoylq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.tarul.cn/Article/details/gehrsicig.sHtML

[Q72] 查看索引
来源：http://3g.vehdjk.com/Article/details/gzlprodne.sHtML

SHOW INDEX FROM users;
来源：http://m.share.vehdjk.com/Article/details/gwsfmffci.sHtML

[Q73] 查看表状态
来源：http://3g.bbcook.cn/Article/details/grslaemii.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.epnwcf.com/Article/details/gysmfdtyi.sHtML

[Q74] 强制使用索引
来源：http://read.share.bbcook.cn/Article/details/gudtgmxde.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fktsv.cn/Article/details/gpvfcycmi.sHtML

[Q75] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gclxpvvzi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.tarul.cn/Article/details/gklnaiftv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/gbvnwzrtu.sHtML

[Q76] 按天统计
来源：http://www.m.share.bbcook.cn/Article/details/golilqoho.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fktsv.cn/Article/details/gottxvngp.sHtML

[Q77] 时间加减
来源：http://3g.yfazqb.com/Article/details/gstqblydy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/gvezxsgfe.sHtML

[Q78] 当前时间
来源：http://read.share.bbcook.cn/Article/details/gayrtjybe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fktsv.cn/Article/details/guuuouphy.sHtML

[Q79] 字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/grcyxsfsj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.bbcook.cn/Article/details/glzulytaa.sHtML

[Q80] 字符串截取
来源：http://wap.yfazqb.com/Article/details/gwmeobayn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gkdntggak.sHtML

[Q81] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gpmihupwx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gcuouyimh.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.tarul.cn/Article/details/gdauriwur.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gbqvjonud.sHtML

[Q83] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gyvugvcjs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gyieydnjn.sHtML

[Q84] 去除首尾空格
来源：http://www.share.yfazqb.com/Article/details/gjkjyukuu.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/glbyipszm.sHtML

[Q85] 数值取整
来源：http://baike.tarul.cn/Article/details/gcoaalesu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.vehdjk.com/Article/details/gunjzbuec.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.epnwcf.com/Article/details/gqfwpjwei.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.yfazqb.com/Article/details/gpygqgyzf.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.bbcook.cn/Article/details/gxorsmkde.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.tarul.cn/Article/details/gojvlahse.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.vehdjk.com/Article/details/gfowsyfdo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.sjlbkw.cn/Article/details/ghovccutu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.tarul.cn/Article/details/gnnxsrrih.sHtML

[Q89] 判断表是否存在
来源：http://3g.epnwcf.com/Article/details/gviiljova.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.vehdjk.com/Article/details/gnmhtwuis.sHtML

[Q90] 生成序号列
来源：http://www.share.tarul.cn/Article/details/geomafbff.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.vehdjk.com/Article/details/gparslnqp.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ggifeqrbm.sHtML

R. Bash 专题
来源：http://wap.bbcook.cn/Article/details/gpmtqlshx.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnajnvdqv.sHtML

[R01] shebang 与严格模式
来源：http://read.share.epnwcf.com/Article/details/gsbbnyrpx.sHtML

#!/usr/bin/env bash
来源：http://blog.bbcook.cn/Article/details/gcnliwotv.sHtML

set -euo pipefail
来源：http://wap.tarul.cn/Article/details/gzbxwlhzl.sHtML

[R02] 变量赋值与使用
来源：http://blog.bbcook.cn/Article/details/grdyigich.sHtML

name="Tom"; echo "$name"
来源：http://blog.fktsv.cn/Article/details/gyukqrvhs.sHtML

[R03] 只读变量
来源：http://wap.bbcook.cn/Article/details/ggzywfhet.sHtML

readonly PI=3.14
来源：http://blog.fktsv.cn/Article/details/gsiftjvuu.sHtML

[R04] 位置参数
来源：http://m.share.epnwcf.com/Article/details/gyhugvuty.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.sjlbkw.cn/Article/details/gyspkxiyo.sHtML

[R05] 参数默认值
来源：http://www.share.epnwcf.com/Article/details/guezrwqor.sHtML

name="${1:-default}"
来源：http://wap.bbcook.cn/Article/details/gazcntvqx.sHtML

[R06] 判断命令是否存在
来源：http://www.share.sjlbkw.cn/Article/details/ggunyccvb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/ggkmaqnqe.sHtML

[R07] if 判断文件
来源：http://mobile.yfazqb.com/Article/details/gxijnemmy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gskyjmkxr.sHtML

[R08] 数值比较
来源：http://blog.epnwcf.com/Article/details/gmgjdmlsh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fktsv.cn/Article/details/guiepawoe.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gcqngcluu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.vehdjk.com/Article/details/gwsmelvth.sHtML

[R10] 正则匹配
来源：http://baike.vehdjk.com/Article/details/gzhooiyya.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gatijjuml.sHtML

[R11] case 多分支
来源：http://wap.bbcook.cn/Article/details/gapjgstwt.sHtML

case "$1" in
来源：http://www.blog.sjlbkw.cn/Article/details/gfwpicjhe.sHtML

start) echo "启动" ;;
来源：http://read.share.yfazqb.com/Article/details/gruvqnajf.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.vehdjk.com/Article/details/gejbfeewf.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.vehdjk.com/Article/details/gcsqghdhp.sHtML

esac
来源：http://baike.tarul.cn/Article/details/gntscqefe.sHtML

[R12] for 遍历文件
来源：http://baike.sjlbkw.cn/Article/details/gaumajkaa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.tarul.cn/Article/details/gynwwmpfo.sHtML

[R13] for 计数循环
来源：http://wap.yfazqb.com/Article/details/gassqjdnm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gnchbgewl.sHtML

[R14] C 风格 for
来源：http://3g.epnwcf.com/Article/details/gssgyqfwv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfqnfmyk.sHtML

[R15] while 逐行读文件
来源：http://baike.bbcook.cn/Article/details/goyvufkpq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.bbcook.cn/Article/details/gfhgdxunp.sHtML

[R16] until 等待条件
来源：http://baike.fktsv.cn/Article/details/gpozvqplg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/galugired.sHtML

[R17] 数组定义与取值
来源：http://wap.yfazqb.com/Article/details/gickipcsm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.sjlbkw.cn/Article/details/gwygemfai.sHtML

[R18] 遍历数组
来源：http://baike.bbcook.cn/Article/details/gfgunvtod.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.epnwcf.com/Article/details/ghkarvjzf.sHtML

[R19] 数组长度
来源：http://m.share.tarul.cn/Article/details/gtionyfmi.sHtML

echo "${#arr[@]}"
来源：http://read.share.fktsv.cn/Article/details/gkfugibdc.sHtML

[R20] 关联数组（字典）
来源：http://baike.fktsv.cn/Article/details/gownutwnz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.sjlbkw.cn/Article/details/gjoutzymf.sHtML

[R21] 字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gdxbsmove.sHtML

echo "${#s}"
来源：http://baike.sjlbkw.cn/Article/details/guvyjaabs.sHtML

[R22] 截取子串
来源：http://blog.epnwcf.com/Article/details/gdprhjdlk.sHtML

echo "${s:0:5}"
来源：http://blog.sjlbkw.cn/Article/details/gnrysnrhk.sHtML

[R23] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gajimcben.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.yfazqb.com/Article/details/gvxnxkpwc.sHtML

[R24] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gsuootono.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.vehdjk.com/Article/details/gpizhjwba.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.bbcook.cn/Article/details/gpgqqftlc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.vehdjk.com/Article/details/gaskkahwg.sHtML

[R26] 命令替换
来源：http://blog.bbcook.cn/Article/details/gxbxtjpbw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.tarul.cn/Article/details/gpeljpivu.sHtML

[R27] 算术展开
来源：http://mobile.fktsv.cn/Article/details/gkivseqfx.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.vehdjk.com/Article/details/gxwsslnic.sHtML

[R28] 浮点运算
来源：http://www.blog.yfazqb.com/Article/details/gvuodwtsq.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/gpeqotmdu.sHtML

[R29] 定义函数
来源：http://3g.yfazqb.com/Article/details/gzmlitzpp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.yfazqb.com/Article/details/gqoefxura.sHtML

[R30] 函数返回状态码
来源：http://mobile.vehdjk.com/Article/details/ghwamwkoy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.epnwcf.com/Article/details/guipbzxnk.sHtML

[R31] 局部变量
来源：http://baike.epnwcf.com/Article/details/gzteynexk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/gvxvcflbq.sHtML

[R32] 参数个数校验
来源：http://baike.fktsv.cn/Article/details/gwygzdzhe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gzulmvyyq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.sjlbkw.cn/Article/details/gghsnktqv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.sjlbkw.cn/Article/details/gboiepatq.sHtML

[R34] 退出时清理
来源：http://www.m.share.yfazqb.com/Article/details/gnlxyiyah.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gwijckumv.sHtML

[R35] 后台执行并等待
来源：http://blog.sjlbkw.cn/Article/details/gtruiqnji.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.epnwcf.com/Article/details/gqixlddlc.sHtML

[R36] 并发执行多个任务
来源：http://www.share.vehdjk.com/Article/details/gcgjoxdvr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/gzrwtkguk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.yfazqb.com/Article/details/gbbgvhasr.sHtML

files=$(ls -1)
来源：http://wap.bbcook.cn/Article/details/giftxqium.sHtML

[R38] 管道串联
来源：http://www.m.share.bbcook.cn/Article/details/grbpdjrol.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.epnwcf.com/Article/details/gjbgymard.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.tarul.cn/Article/details/gnsnkfbcs.sHtML

cmd > out.log 2>&1
来源：http://wap.vehdjk.com/Article/details/gpskuslpe.sHtML

[R40] 追加写日志
来源：http://baike.epnwcf.com/Article/details/gdguhssgn.sHtML

echo "log" >> out.log
来源：http://mobile.yfazqb.com/Article/details/gmvzkfhyi.sHtML

[R41] 丢弃输出
来源：http://mobile.fktsv.cn/Article/details/gwudbthvp.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fktsv.cn/Article/details/gwoeeynab.sHtML

[R42] 输入重定向
来源：http://wap.yfazqb.com/Article/details/grpawhdkv.sHtML

wc -l < a.txt
来源：http://mobile.yfazqb.com/Article/details/giwjaynzu.sHtML

[R43] 按名字查找文件
来源：http://m.share.bbcook.cn/Article/details/gmpmnunke.sHtML

find . -name "*.log" -type f
来源：http://blog.yfazqb.com/Article/details/ghjlvpnor.sHtML

[R44] 按修改时间查找
来源：http://3g.sjlbkw.cn/Article/details/gfbshtomv.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.vehdjk.com/Article/details/gexgdfdqo.sHtML

[R45] 批量删除
来源：http://www.share.fktsv.cn/Article/details/gliqfpqym.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.tarul.cn/Article/details/gekxhbrve.sHtML

[R46] 递归替换文件内容
来源：http://m.share.vehdjk.com/Article/details/gwkyxxqlx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.yfazqb.com/Article/details/gxfjuchmo.sHtML

[R47] sed 单行替换
来源：http://www.blog.sjlbkw.cn/Article/details/gzjnnqxov.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.bbcook.cn/Article/details/gmlwztrjh.sHtML

[R48] awk 取指定列
来源：http://blog.bbcook.cn/Article/details/gupfgiuhc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gfwqguvox.sHtML

[R49] awk 带条件
来源：http://www.m.share.fktsv.cn/Article/details/gwbkhjxjq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.yfazqb.com/Article/details/gglztipbm.sHtML

[R50] awk 求和
来源：http://wap.yfazqb.com/Article/details/gbcwhjutg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.epnwcf.com/Article/details/giedemvzl.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.tarul.cn/Article/details/giisijyuj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.yfazqb.com/Article/details/govaqblom.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/gnfgoknly.sHtML

wc -l a.txt
来源：http://baike.epnwcf.com/Article/details/gjyopahbj.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.epnwcf.com/Article/details/gtjqhsrty.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.bbcook.cn/Article/details/gtmpavfum.sHtML

[R54] 比较两个文件
来源：http://3g.bbcook.cn/Article/details/gtqwnlrao.sHtML

diff a.txt b.txt
来源：http://mobile.tarul.cn/Article/details/gmlyznuvm.sHtML

[R55] 压缩与解压
来源：http://www.m.share.yfazqb.com/Article/details/gnvbwljep.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.bbcook.cn/Article/details/gakfcbprk.sHtML

[R56] 远程拷贝
来源：http://mobile.vehdjk.com/Article/details/glnlyubuh.sHtML

scp file user@host:/path/
来源：http://3g.bbcook.cn/Article/details/gfaibwxdk.sHtML

[R57] 远程执行命令
来源：http://blog.bbcook.cn/Article/details/gmqjpahqb.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gstxsrrxk.sHtML

[R58] 下载文件
来源：http://blog.yfazqb.com/Article/details/gnnwhmhsh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.epnwcf.com/Article/details/ggvdlndmw.sHtML

[R59] 发 POST JSON
来源：http://blog.bbcook.cn/Article/details/gytktivil.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.tarul.cn/Article/details/gwlynpuvg.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gthjgcdir.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/gbaifocda.sHtML

[R61] 磁盘占用
来源：http://www.blog.vehdjk.com/Article/details/gnokkvmtt.sHtML

df -h;  du -sh *
来源：http://blog.yfazqb.com/Article/details/gfcmqkkkz.sHtML

[R62] 找最占空间的文件
来源：http://3g.sjlbkw.cn/Article/details/geqtyrimn.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.epnwcf.com/Article/details/gyuhbqiaf.sHtML

[R63] 内存与进程
来源：http://wap.tarul.cn/Article/details/gbugnrauw.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.vehdjk.com/Article/details/gfliykrws.sHtML

[R64] 结束进程
来源：http://read.share.yfazqb.com/Article/details/gypwzmmkg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.sjlbkw.cn/Article/details/gfgpmejjt.sHtML

[R65] 查看端口占用
来源：http://3g.fktsv.cn/Article/details/gpnmfktcf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.epnwcf.com/Article/details/gphvyidok.sHtML

[R66] 定时任务
来源：http://m.share.yfazqb.com/Article/details/grhghfbmy.sHtML

crontab -e;  crontab -l
来源：http://wap.bbcook.cn/Article/details/gxssrancf.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fktsv.cn/Article/details/gpwysjkge.sHtML

openssl rand -hex 16
来源：http://www.blog.tarul.cn/Article/details/goabmkppl.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/ggmtskjwh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.tarul.cn/Article/details/gycxiuydr.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/grbiqjpxn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.vehdjk.com/Article/details/gpbimhqkj.sHtML

[R70] 时间戳与互转
来源：http://3g.bbcook.cn/Article/details/gdyeclboa.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.yfazqb.com/Article/details/glteidauv.sHtML

[R71] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/grebydstd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gzazjtfrq.sHtML

[R72] 等待端口就绪
来源：http://mobile.fktsv.cn/Article/details/gpdxybcdq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/gowapkzwt.sHtML

[R73] 分割大日志
来源：http://wap.yfazqb.com/Article/details/ggvsdmkih.sHtML

split -l 1000 big.log part_
来源：http://wap.tarul.cn/Article/details/gdxtentin.sHtML

[R74] 批量重命名
来源：http://baike.tarul.cn/Article/details/gemyaqdoe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.tarul.cn/Article/details/gngjtnkzn.sHtML

[R75] 导出环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gehydkdvv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.bbcook.cn/Article/details/gmglbxwuo.sHtML

[R76] 使用临时文件
来源：http://www.share.bbcook.cn/Article/details/gqomlhctq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.bbcook.cn/Article/details/grqbnurks.sHtML

[R77] 读取用户输入
来源：http://www.blog.fktsv.cn/Article/details/gxwlrjofb.sHtML

read -rp "请输入: " ans
来源：http://www.blog.sjlbkw.cn/Article/details/gbfkapykb.sHtML

[R78] 交互式菜单
来源：http://www.m.share.bbcook.cn/Article/details/gcobxrxip.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.bbcook.cn/Article/details/gaafflicj.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fktsv.cn/Article/details/gtxroayjj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.vehdjk.com/Article/details/guqfnrtlz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fktsv.cn/Article/details/ghwcimmix.sHtML

time ./run.sh
来源：http://www.blog.yfazqb.com/Article/details/govymailp.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/guytotmjf.sHtML

S. C / C++ 专题
来源：http://mobile.sjlbkw.cn/Article/details/gntfrvlxm.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gkljbwcgx.sHtML

[S01] C：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gppssahiq.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/glyozxlxb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.vehdjk.com/Article/details/gaydejdtl.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.yfazqb.com/Article/details/gfryjtxsx.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fktsv.cn/Article/details/gkrtxzhdt.sHtML

[S03] C：读入整数
来源：http://m.share.fktsv.cn/Article/details/gnuojntlg.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.bbcook.cn/Article/details/gbcjeiscc.sHtML

[S04] C：字符串复制
来源：http://www.share.yfazqb.com/Article/details/gbogzzxnt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.bbcook.cn/Article/details/gaomulxho.sHtML

[S05] C：字符串长度
来源：http://www.share.yfazqb.com/Article/details/gawseqrfp.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/gavpqeeqk.sHtML

[S06] C：字符串比较
来源：http://blog.yfazqb.com/Article/details/gkdgezdin.sHtML

strcmp(a, b) == 0
来源：http://mobile.yfazqb.com/Article/details/gtuhbekrs.sHtML

[S07] C：数组遍历求和
来源：http://3g.tarul.cn/Article/details/gvdozxzbw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gtolewwdi.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.sjlbkw.cn/Article/details/gewgtexty.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.bbcook.cn/Article/details/grmpkdzyp.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.yfazqb.com/Article/details/gtyfronzf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.sjlbkw.cn/Article/details/gyuyqrlap.sHtML

[S10] C：指针与解引用
来源：http://blog.fktsv.cn/Article/details/gifboofkk.sHtML

int *p = &a;  *p = 5;
来源：http://baike.yfazqb.com/Article/details/gptpdofag.sHtML

[S11] C：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gackacuwi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.tarul.cn/Article/details/ghkfwnlsv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.yfazqb.com/Article/details/ggfddhtch.sHtML

fclose(f);
来源：http://blog.tarul.cn/Article/details/ghaykrnsc.sHtML

[S12] C：写文件
来源：http://mobile.bbcook.cn/Article/details/goiuekczn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gwqeglyjk.sHtML

[S13] C：宏定义
来源：http://blog.fktsv.cn/Article/details/gbzghpptn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.epnwcf.com/Article/details/grjibpjcj.sHtML

[S14] C：枚举
来源：http://www.blog.tarul.cn/Article/details/ghcosvhvf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.yfazqb.com/Article/details/gjuzqeiki.sHtML

[S15] C：类型转换
来源：http://read.share.vehdjk.com/Article/details/gtrdbfmtj.sHtML

(double) a / b
来源：http://www.share.yfazqb.com/Article/details/gtdtcmrqq.sHtML

[S16] C：位操作置位
来源：http://read.share.yfazqb.com/Article/details/gwxuxhrys.sHtML

x |= (1 << 3);
来源：http://wap.bbcook.cn/Article/details/gvvayllmh.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.tarul.cn/Article/details/ghnnpupyj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.bbcook.cn/Article/details/gilacfudt.sHtML

[S18] C：命令行参数
来源：http://www.share.sjlbkw.cn/Article/details/ghvmnczhg.sHtML

int main(int argc, char **argv)
来源：http://wap.tarul.cn/Article/details/gxbptqifo.sHtML

[S19] C：快速排序
来源：http://blog.yfazqb.com/Article/details/gxwxexzle.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gxecycmle.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqskojgf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/grpvpzshx.sHtML

[S21] C：字符类别判断
来源：http://baike.bbcook.cn/Article/details/gcsykjxme.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.sjlbkw.cn/Article/details/gmeenjxjj.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/ggczpsmwi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.epnwcf.com/Article/details/gtnrnrsfc.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/guvpnizvl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.vehdjk.com/Article/details/gtpthtrka.sHtML

[S24] C：获取本地时间
来源：http://www.share.epnwcf.com/Article/details/gtmngbqwy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fktsv.cn/Article/details/gzbsezewl.sHtML

[S25] C：内存拷贝
来源：http://www.blog.bbcook.cn/Article/details/gxmzoiiim.sHtML

memcpy(dst, src, n);
来源：http://mobile.bbcook.cn/Article/details/gnsmgyfqm.sHtML

[S26] C：内存清零
来源：http://www.blog.epnwcf.com/Article/details/gjnqycdvz.sHtML


<!-- 参考信息 -->