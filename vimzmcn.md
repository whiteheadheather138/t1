代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.epnwcf.com/Article/details/giomknpon.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.sjlbkw.cn/Article/details/gaqqfboem.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.yfazqb.com/Article/details/gpbqxrosb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.epnwcf.com/Article/details/gmfgowmzt.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/ggylutwkf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gqwesespq.sHtML

[Q62] 分组占比
来源：http://mobile.yfazqb.com/Article/details/givmnrulk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gdkivkoqs.sHtML

[Q63] 开启事务
来源：http://m.share.fktsv.cn/Article/details/gfseqoxld.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.yfazqb.com/Article/details/gindojizn.sHtML

[Q64] 提交事务
来源：http://www.share.bbcook.cn/Article/details/gcumpwvwa.sHtML

COMMIT;
来源：http://www.blog.epnwcf.com/Article/details/grpgvmdtk.sHtML

[Q65] 回滚事务
来源：http://read.share.fktsv.cn/Article/details/gllsxzllr.sHtML

ROLLBACK;
来源：http://baike.yfazqb.com/Article/details/gmodxubzc.sHtML

[Q66] 行锁查询
来源：http://3g.yfazqb.com/Article/details/gzhunfmxv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.yfazqb.com/Article/details/gcoiolsfk.sHtML

[Q67] 设置隔离级别
来源：http://m.share.bbcook.cn/Article/details/gewvcodyu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.vehdjk.com/Article/details/gfptvhnra.sHtML

[Q68] 保存点
来源：http://mobile.sjlbkw.cn/Article/details/grnzwxhkm.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.tarul.cn/Article/details/gvsunkqri.sHtML

ROLLBACK TO sp1;
来源：http://read.share.bbcook.cn/Article/details/gvwodwqgf.sHtML

[Q69] 查看执行计划
来源：http://www.share.vehdjk.com/Article/details/gcymdeyho.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.bbcook.cn/Article/details/gsoiusemz.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/gomwkgclt.sHtML

ANALYZE TABLE users;
来源：http://baike.yfazqb.com/Article/details/gtszlwdyy.sHtML

[Q71] 查看建表语句
来源：http://wap.vehdjk.com/Article/details/glyftxxvw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fktsv.cn/Article/details/guculzikg.sHtML

[Q72] 查看索引
来源：http://mobile.yfazqb.com/Article/details/gkkdtptkn.sHtML

SHOW INDEX FROM users;
来源：http://baike.tarul.cn/Article/details/gbalwqoma.sHtML

[Q73] 查看表状态
来源：http://mobile.epnwcf.com/Article/details/gjsqfwiik.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gfdvdrvka.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/gycthklwl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.vehdjk.com/Article/details/gtrmpgirw.sHtML

[Q75] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gjdxfecjr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gyqrvpbra.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.epnwcf.com/Article/details/gccdoyagy.sHtML

[Q76] 按天统计
来源：http://blog.sjlbkw.cn/Article/details/gkjuzdskp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.bbcook.cn/Article/details/gxmizzflo.sHtML

[Q77] 时间加减
来源：http://baike.sjlbkw.cn/Article/details/gqxepqizu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.vehdjk.com/Article/details/gbelcvikg.sHtML

[Q78] 当前时间
来源：http://www.share.sjlbkw.cn/Article/details/gxdlvnfff.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fktsv.cn/Article/details/glnaunfws.sHtML

[Q79] 字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gltvpgsil.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.yfazqb.com/Article/details/gpothctkg.sHtML

[Q80] 字符串截取
来源：http://blog.vehdjk.com/Article/details/ggwzibsjc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.bbcook.cn/Article/details/ggfuyxmpj.sHtML

[Q81] 字符串替换
来源：http://wap.bbcook.cn/Article/details/gzrypzqxt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.yfazqb.com/Article/details/gflhtaqkd.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.sjlbkw.cn/Article/details/gtkjjuhpw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gvzfwordo.sHtML

[Q83] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gqlvmtkbw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gzyoywjzx.sHtML

[Q84] 去除首尾空格
来源：http://blog.vehdjk.com/Article/details/gllzljbhi.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gdftrvahq.sHtML

[Q85] 数值取整
来源：http://blog.tarul.cn/Article/details/gqunihqkj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.epnwcf.com/Article/details/gfghkjfar.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fktsv.cn/Article/details/ghhftezmi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.tarul.cn/Article/details/gikaykonn.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.yfazqb.com/Article/details/gvitxrddh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.yfazqb.com/Article/details/ggisqfwgl.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.sjlbkw.cn/Article/details/gnpulpbyw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.bbcook.cn/Article/details/gwhcdgimr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.tarul.cn/Article/details/gowuruxik.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gaumhooak.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.epnwcf.com/Article/details/gmnywcwxe.sHtML

[Q90] 生成序号列
来源：http://www.blog.yfazqb.com/Article/details/gvbpktsfw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fktsv.cn/Article/details/ghyuackmi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/grzkwhqtr.sHtML

R. Bash 专题
来源：http://www.share.epnwcf.com/Article/details/gpxfctktm.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gbeklgczp.sHtML

[R01] shebang 与严格模式
来源：http://3g.epnwcf.com/Article/details/gonxyfpou.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/geajdpdnz.sHtML

set -euo pipefail
来源：http://www.share.epnwcf.com/Article/details/gqncxmygd.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.epnwcf.com/Article/details/glkoascsm.sHtML

name="Tom"; echo "$name"
来源：http://m.share.sjlbkw.cn/Article/details/gcjnpsqbr.sHtML

[R03] 只读变量
来源：http://read.share.tarul.cn/Article/details/gosjfwruc.sHtML

readonly PI=3.14
来源：http://mobile.fktsv.cn/Article/details/ggdnyofso.sHtML

[R04] 位置参数
来源：http://baike.vehdjk.com/Article/details/gvrwpjjzl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.epnwcf.com/Article/details/gkfqsghci.sHtML

[R05] 参数默认值
来源：http://mobile.sjlbkw.cn/Article/details/ghmzkqjnu.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/gknmdaxde.sHtML

[R06] 判断命令是否存在
来源：http://baike.fktsv.cn/Article/details/geteakesu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/ganxmvrjl.sHtML

[R07] if 判断文件
来源：http://mobile.bbcook.cn/Article/details/gmtlqaxey.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.bbcook.cn/Article/details/gvpjdhdcp.sHtML

[R08] 数值比较
来源：http://www.blog.vehdjk.com/Article/details/gzlhpopzy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fktsv.cn/Article/details/gdectpies.sHtML

[R09] 字符串比较
来源：http://baike.sjlbkw.cn/Article/details/ggoknjpmf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.sjlbkw.cn/Article/details/grmdmdedz.sHtML

[R10] 正则匹配
来源：http://www.m.share.fktsv.cn/Article/details/gzrfjpqzk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.yfazqb.com/Article/details/gnzzngvuo.sHtML

[R11] case 多分支
来源：http://www.m.share.epnwcf.com/Article/details/guohpuamh.sHtML

case "$1" in
来源：http://read.share.tarul.cn/Article/details/geprngzxe.sHtML

start) echo "启动" ;;
来源：http://www.share.tarul.cn/Article/details/garnihlck.sHtML

stop)  echo "停止" ;;
来源：http://blog.epnwcf.com/Article/details/gggclngjd.sHtML

*)     echo "未知命令" ;;
来源：http://wap.bbcook.cn/Article/details/gyouydniz.sHtML

esac
来源：http://blog.bbcook.cn/Article/details/gskpevlke.sHtML

[R12] for 遍历文件
来源：http://3g.sjlbkw.cn/Article/details/gaiprktee.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/gitzfhdsb.sHtML

[R13] for 计数循环
来源：http://blog.fktsv.cn/Article/details/guxlvqaln.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gxgipafqz.sHtML

[R14] C 风格 for
来源：http://m.share.tarul.cn/Article/details/gktqbkzoe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/gdyflozvf.sHtML

[R15] while 逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gfwppbtia.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.yfazqb.com/Article/details/gyirdibia.sHtML

[R16] until 等待条件
来源：http://baike.yfazqb.com/Article/details/grubphjcz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/geyaylzlx.sHtML

[R17] 数组定义与取值
来源：http://baike.tarul.cn/Article/details/givyweymk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/grjtuyztj.sHtML

[R18] 遍历数组
来源：http://blog.vehdjk.com/Article/details/gfwdrxzgi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.bbcook.cn/Article/details/gcfrcrvqn.sHtML

[R19] 数组长度
来源：http://wap.epnwcf.com/Article/details/gkhoszagx.sHtML

echo "${#arr[@]}"
来源：http://m.share.epnwcf.com/Article/details/gdzrqrmxq.sHtML

[R20] 关联数组（字典）
来源：http://3g.bbcook.cn/Article/details/ghtaodsnv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.yfazqb.com/Article/details/gymggneiq.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/gdalpfyil.sHtML

echo "${#s}"
来源：http://www.share.epnwcf.com/Article/details/gbeswcqqa.sHtML

[R22] 截取子串
来源：http://mobile.vehdjk.com/Article/details/gnihfidyc.sHtML

echo "${s:0:5}"
来源：http://blog.bbcook.cn/Article/details/gwowzskhd.sHtML

[R23] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gcdpigtll.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.yfazqb.com/Article/details/gjksjvcyv.sHtML

[R24] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/grpqzoixh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.tarul.cn/Article/details/gjhawkvqc.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.sjlbkw.cn/Article/details/gyjcjclsd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.epnwcf.com/Article/details/gnspajrwz.sHtML

[R26] 命令替换
来源：http://wap.tarul.cn/Article/details/gbmbdhckw.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.bbcook.cn/Article/details/gjspmqtsk.sHtML

[R27] 算术展开
来源：http://3g.vehdjk.com/Article/details/ggawtnatx.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.vehdjk.com/Article/details/grhugeykw.sHtML

[R28] 浮点运算
来源：http://wap.fktsv.cn/Article/details/gcrhpdffj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.vehdjk.com/Article/details/gucyvljmb.sHtML

[R29] 定义函数
来源：http://3g.epnwcf.com/Article/details/gcvoefqur.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.bbcook.cn/Article/details/ghtghagfy.sHtML

[R30] 函数返回状态码
来源：http://blog.vehdjk.com/Article/details/grjvwmjve.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fktsv.cn/Article/details/gqrpnrdxa.sHtML

[R31] 局部变量
来源：http://blog.yfazqb.com/Article/details/gqsqjhktm.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/gfcisdxdj.sHtML

[R32] 参数个数校验
来源：http://mobile.sjlbkw.cn/Article/details/gibkpgtmm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gvnynngzh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.yfazqb.com/Article/details/gkwydrlci.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.tarul.cn/Article/details/gyrzsimta.sHtML

[R34] 退出时清理
来源：http://blog.fktsv.cn/Article/details/gzckhtygl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/grwuffrio.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/gzaxbajic.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.vehdjk.com/Article/details/gosedlcen.sHtML

[R36] 并发执行多个任务
来源：http://www.share.epnwcf.com/Article/details/gvlhascac.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.sjlbkw.cn/Article/details/gtnxhdzkc.sHtML

[R37] 把输出赋给变量
来源：http://read.share.tarul.cn/Article/details/gjoyoabkf.sHtML

files=$(ls -1)
来源：http://baike.fktsv.cn/Article/details/gammbjtqg.sHtML

[R38] 管道串联
来源：http://www.share.bbcook.cn/Article/details/gasrvurwi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fktsv.cn/Article/details/gvgdjxhwl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.vehdjk.com/Article/details/gadyqvkub.sHtML

cmd > out.log 2>&1
来源：http://mobile.bbcook.cn/Article/details/gdvybvsbe.sHtML

[R40] 追加写日志
来源：http://baike.epnwcf.com/Article/details/gzdwyhfcu.sHtML

echo "log" >> out.log
来源：http://mobile.bbcook.cn/Article/details/gvupnxtje.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/gleunjzlt.sHtML

cmd >/dev/null 2>&1
来源：http://baike.bbcook.cn/Article/details/gywnvpuke.sHtML

[R42] 输入重定向
来源：http://www.m.share.epnwcf.com/Article/details/gcgncqtgl.sHtML

wc -l < a.txt
来源：http://blog.vehdjk.com/Article/details/gxruwhzjz.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gpmhywquw.sHtML

find . -name "*.log" -type f
来源：http://read.share.bbcook.cn/Article/details/gxcxbzxnl.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/gbntlgqyd.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fktsv.cn/Article/details/gbclaobgc.sHtML

[R45] 批量删除
来源：http://baike.vehdjk.com/Article/details/gpohasjii.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.sjlbkw.cn/Article/details/gsuphpgcp.sHtML

[R46] 递归替换文件内容
来源：http://www.share.epnwcf.com/Article/details/gdscrdera.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.bbcook.cn/Article/details/gdiiiuflf.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/gnniydtwn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.vehdjk.com/Article/details/gywgsvery.sHtML

[R48] awk 取指定列
来源：http://3g.yfazqb.com/Article/details/ghlbvtixk.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gzanuwxfs.sHtML

[R49] awk 带条件
来源：http://3g.yfazqb.com/Article/details/gijjblttg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.vehdjk.com/Article/details/gqifgckjg.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/gfkfirpex.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/guneisxdp.sHtML

[R51] 排序去重取前几
来源：http://baike.fktsv.cn/Article/details/ggvqwguep.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fktsv.cn/Article/details/gbftmhfbx.sHtML

[R52] 统计行数
来源：http://www.m.share.bbcook.cn/Article/details/gcpkigukm.sHtML

wc -l a.txt
来源：http://baike.tarul.cn/Article/details/gddctwplb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fktsv.cn/Article/details/gxlmibwux.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fktsv.cn/Article/details/gzbeatduo.sHtML

[R54] 比较两个文件
来源：http://www.blog.yfazqb.com/Article/details/gjxmnxpyv.sHtML

diff a.txt b.txt
来源：http://m.share.epnwcf.com/Article/details/gvrwfbikz.sHtML

[R55] 压缩与解压
来源：http://mobile.vehdjk.com/Article/details/ghnfqezpu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.sjlbkw.cn/Article/details/gbruulfgu.sHtML

[R56] 远程拷贝
来源：http://m.share.fktsv.cn/Article/details/gyubkrdok.sHtML

scp file user@host:/path/
来源：http://m.share.vehdjk.com/Article/details/gwffggoxt.sHtML

[R57] 远程执行命令
来源：http://m.share.bbcook.cn/Article/details/gjnsghfba.sHtML

ssh user@host 'uptime'
来源：http://wap.sjlbkw.cn/Article/details/gksmdskbz.sHtML

[R58] 下载文件
来源：http://read.share.vehdjk.com/Article/details/glkacipyf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.sjlbkw.cn/Article/details/gyvqlybcc.sHtML

[R59] 发 POST JSON
来源：http://blog.fktsv.cn/Article/details/gomyqpeuo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.bbcook.cn/Article/details/gutfjgwpm.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/gwimnzkeu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/ggcflldmm.sHtML

[R61] 磁盘占用
来源：http://m.share.tarul.cn/Article/details/gpyidhrag.sHtML

df -h;  du -sh *
来源：http://baike.tarul.cn/Article/details/gkoojvtkh.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fktsv.cn/Article/details/gvleqdnmh.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.tarul.cn/Article/details/gkvgjqkxh.sHtML

[R63] 内存与进程
来源：http://3g.vehdjk.com/Article/details/glojtrxga.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.bbcook.cn/Article/details/gqowbfsjc.sHtML

[R64] 结束进程
来源：http://www.blog.bbcook.cn/Article/details/gjmaixpcm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.bbcook.cn/Article/details/gltojytbt.sHtML

[R65] 查看端口占用
来源：http://mobile.fktsv.cn/Article/details/gsukzciav.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.sjlbkw.cn/Article/details/gqjluatpp.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/gtjrwnfls.sHtML

crontab -e;  crontab -l
来源：http://baike.fktsv.cn/Article/details/gnrchawis.sHtML

[R67] 生成随机十六进制串
来源：http://3g.sjlbkw.cn/Article/details/gpcckbnui.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/glltfyhxr.sHtML

[R68] 计算文件校验值
来源：http://3g.epnwcf.com/Article/details/gcgdivzyj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.bbcook.cn/Article/details/grnztixhw.sHtML

[R69] 生成随机密码
来源：http://3g.sjlbkw.cn/Article/details/gxuqalfio.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/gwvaiatfo.sHtML

[R70] 时间戳与互转
来源：http://www.blog.epnwcf.com/Article/details/gvoqvnenz.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.epnwcf.com/Article/details/gpcqikxay.sHtML

[R71] 日期格式化
来源：http://wap.fktsv.cn/Article/details/gglrjytkh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/gqqpxdqrt.sHtML

[R72] 等待端口就绪
来源：http://blog.yfazqb.com/Article/details/gfucxxkjb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gbrwmbybs.sHtML

[R73] 分割大日志
来源：http://www.blog.epnwcf.com/Article/details/gpnzlborx.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/gjrsaftno.sHtML

[R74] 批量重命名
来源：http://wap.epnwcf.com/Article/details/gdzpdmvmo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.sjlbkw.cn/Article/details/gxghwelym.sHtML

[R75] 导出环境变量
来源：http://read.share.sjlbkw.cn/Article/details/guxqnacre.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.epnwcf.com/Article/details/gypuppqxg.sHtML

[R76] 使用临时文件
来源：http://www.m.share.tarul.cn/Article/details/gcwhnveup.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.vehdjk.com/Article/details/gulnocqbf.sHtML

[R77] 读取用户输入
来源：http://www.blog.yfazqb.com/Article/details/gcvosxdwo.sHtML

read -rp "请输入: " ans
来源：http://3g.epnwcf.com/Article/details/gzlybndey.sHtML

[R78] 交互式菜单
来源：http://read.share.vehdjk.com/Article/details/giaahcmht.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.epnwcf.com/Article/details/ggimwtosk.sHtML

[R79] 解析命令行选项
来源：http://blog.fktsv.cn/Article/details/gcnqzkwlf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.yfazqb.com/Article/details/gmtnjklxz.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.yfazqb.com/Article/details/gaxdmmgzq.sHtML

time ./run.sh
来源：http://3g.epnwcf.com/Article/details/gtiizymed.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqpbbbipu.sHtML

S. C / C++ 专题
来源：http://blog.tarul.cn/Article/details/guxqmnzwd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmvneeeev.sHtML

[S01] C：Hello World
来源：http://www.share.bbcook.cn/Article/details/gwhdqlrki.sHtML

#include <stdio.h>
来源：http://3g.bbcook.cn/Article/details/gdmgqthku.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/gzhoplaqx.sHtML

[S02] C：变量与格式化输出
来源：http://blog.vehdjk.com/Article/details/gqvousvud.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.tarul.cn/Article/details/gewyapphg.sHtML

[S03] C：读入整数
来源：http://m.share.fktsv.cn/Article/details/gkcotaswh.sHtML

int x; scanf("%d", &x);
来源：http://baike.bbcook.cn/Article/details/gfnelvrea.sHtML

[S04] C：字符串复制
来源：http://read.share.tarul.cn/Article/details/grialuiup.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.yfazqb.com/Article/details/gktvoifwg.sHtML

[S05] C：字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gpkxyajav.sHtML

strlen(s)
来源：http://mobile.vehdjk.com/Article/details/gkbzixvsg.sHtML

[S06] C：字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/gjnxhzlao.sHtML

strcmp(a, b) == 0
来源：http://read.share.vehdjk.com/Article/details/gjnqmtivp.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fktsv.cn/Article/details/gadkbrwhi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.tarul.cn/Article/details/gjkvukpdg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.tarul.cn/Article/details/gqmbvdmkk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.tarul.cn/Article/details/gervkieey.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.tarul.cn/Article/details/gbijlezaf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.tarul.cn/Article/details/gnmrlqykx.sHtML

[S10] C：指针与解引用
来源：http://www.share.bbcook.cn/Article/details/gbodnkojq.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fktsv.cn/Article/details/gbmecidpm.sHtML

[S11] C：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gnxxcoqpk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.yfazqb.com/Article/details/gfnnhtpbr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.epnwcf.com/Article/details/godjpamln.sHtML

fclose(f);
来源：http://wap.tarul.cn/Article/details/gubfrrlto.sHtML

[S12] C：写文件
来源：http://wap.sjlbkw.cn/Article/details/gkuzywgub.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/guizyauqe.sHtML

[S13] C：宏定义
来源：http://baike.vehdjk.com/Article/details/gsyiwkfiy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.sjlbkw.cn/Article/details/gnzmkigqx.sHtML

[S14] C：枚举
来源：http://3g.vehdjk.com/Article/details/gizcaekji.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.epnwcf.com/Article/details/gzxhstwfi.sHtML

[S15] C：类型转换
来源：http://www.blog.yfazqb.com/Article/details/gsjuhgfsv.sHtML

(double) a / b
来源：http://m.share.bbcook.cn/Article/details/guzhteepn.sHtML

[S16] C：位操作置位
来源：http://www.blog.sjlbkw.cn/Article/details/ggwveztqv.sHtML

x |= (1 << 3);
来源：http://m.share.bbcook.cn/Article/details/ggczdxryb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fktsv.cn/Article/details/gmrbojckl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.sjlbkw.cn/Article/details/gzmncfevm.sHtML

[S18] C：命令行参数
来源：http://baike.fktsv.cn/Article/details/gsdeuzjdh.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gtvaqyssm.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/gliemwfrt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/gnysnnkzw.sHtML

[S20] C：二分查找
来源：http://www.share.tarul.cn/Article/details/ggjcpllwm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gcwqnpzep.sHtML

[S21] C：字符类别判断
来源：http://read.share.fktsv.cn/Article/details/gedvjuaxy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.vehdjk.com/Article/details/geylsaial.sHtML

[S22] C：字符串转数字
来源：http://m.share.sjlbkw.cn/Article/details/grisxdzdb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/gcfzhqcra.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gkxvydpfq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.tarul.cn/Article/details/gqltasxjr.sHtML

[S24] C：获取本地时间
来源：http://baike.sjlbkw.cn/Article/details/gjcdlnacq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.vehdjk.com/Article/details/gthrbwdue.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gbmbhgqxu.sHtML

memcpy(dst, src, n);
来源：http://blog.vehdjk.com/Article/details/gzthxxjup.sHtML

[S26] C：内存清零
来源：http://m.share.tarul.cn/Article/details/guqkdzvnf.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/gkmlammnh.sHtML

[S27] C：定义常量
来源：http://baike.tarul.cn/Article/details/gshrwaiwq.sHtML

const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gdkixkaha.sHtML

[S28] C：静态变量
来源：http://www.blog.fktsv.cn/Article/details/gmwzybpnt.sHtML

static int counter = 0;
来源：http://3g.fktsv.cn/Article/details/gostisqfv.sHtML

[S29] C：变参函数
来源：http://m.share.fktsv.cn/Article/details/grmsyirtx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/gfugdujvm.sHtML

[S30] C：头文件保护
来源：http://blog.tarul.cn/Article/details/gdegutxjq.sHtML


<!-- 参考信息 -->