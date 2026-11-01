代发 wailian999

[Q61] 移动平均
来源：http://www.share.fktsv.cn/Article/details/gufpzcnlm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.tarul.cn/Article/details/galygkifg.sHtML

[Q62] 分组占比
来源：http://mobile.vehdjk.com/Article/details/gpskahemt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gjwainvte.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/gkforcteo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.bbcook.cn/Article/details/gqevblgas.sHtML

[Q64] 提交事务
来源：http://wap.fktsv.cn/Article/details/gihksejge.sHtML

COMMIT;
来源：http://www.share.vehdjk.com/Article/details/geurydvci.sHtML

[Q65] 回滚事务
来源：http://www.share.sjlbkw.cn/Article/details/gkvegynde.sHtML

ROLLBACK;
来源：http://wap.bbcook.cn/Article/details/gecroihtk.sHtML

[Q66] 行锁查询
来源：http://3g.tarul.cn/Article/details/gmjzteknm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.vehdjk.com/Article/details/gzrqhxpeh.sHtML

[Q67] 设置隔离级别
来源：http://3g.yfazqb.com/Article/details/grdcsuyhz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.yfazqb.com/Article/details/gejehwldz.sHtML

[Q68] 保存点
来源：http://mobile.vehdjk.com/Article/details/gatthjjwu.sHtML

SAVEPOINT sp1;
来源：http://www.share.vehdjk.com/Article/details/gpakctjhn.sHtML

ROLLBACK TO sp1;
来源：http://baike.yfazqb.com/Article/details/gkabhnmlv.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.vehdjk.com/Article/details/gjssvspus.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fktsv.cn/Article/details/gsfatkfju.sHtML

[Q70] 更新统计信息
来源：http://3g.bbcook.cn/Article/details/gkswddxvj.sHtML

ANALYZE TABLE users;
来源：http://baike.fktsv.cn/Article/details/gtbybbzhz.sHtML

[Q71] 查看建表语句
来源：http://mobile.fktsv.cn/Article/details/gamosgyyw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fktsv.cn/Article/details/gqxehtjiu.sHtML

[Q72] 查看索引
来源：http://m.share.yfazqb.com/Article/details/gxcgvjkvb.sHtML

SHOW INDEX FROM users;
来源：http://baike.vehdjk.com/Article/details/gcjfddxbt.sHtML

[Q73] 查看表状态
来源：http://www.blog.sjlbkw.cn/Article/details/gyxnmvwur.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gygtozavi.sHtML

[Q74] 强制使用索引
来源：http://m.share.vehdjk.com/Article/details/gmolpasvh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.yfazqb.com/Article/details/gyyhqfacm.sHtML

[Q75] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/gmddtqqja.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.epnwcf.com/Article/details/ginejzody.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.bbcook.cn/Article/details/gaeahxoqt.sHtML

[Q76] 按天统计
来源：http://www.blog.yfazqb.com/Article/details/glaqtrnjj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.epnwcf.com/Article/details/gvetmbssf.sHtML

[Q77] 时间加减
来源：http://www.m.share.yfazqb.com/Article/details/gmtnhofuc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.epnwcf.com/Article/details/gmlpgvmjr.sHtML

[Q78] 当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gcjgcfegy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.epnwcf.com/Article/details/gggoxuroh.sHtML

[Q79] 字符串拼接
来源：http://www.blog.tarul.cn/Article/details/gladgpctl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.vehdjk.com/Article/details/gwcfbryzk.sHtML

[Q80] 字符串截取
来源：http://m.share.bbcook.cn/Article/details/gkrbbrxpg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsjzlhwt.sHtML

[Q81] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/gugnxvyqg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.epnwcf.com/Article/details/gffsrsukw.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.bbcook.cn/Article/details/grdbiodra.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/grlaernam.sHtML

[Q83] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gwttfqiys.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/ggxnzjesc.sHtML

[Q84] 去除首尾空格
来源：http://baike.sjlbkw.cn/Article/details/gbiytzaev.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/golqlkhoq.sHtML

[Q85] 数值取整
来源：http://baike.bbcook.cn/Article/details/gnxvcytgh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fktsv.cn/Article/details/gwfvhnovw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/goegnhrtw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fktsv.cn/Article/details/gvsytxmia.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.tarul.cn/Article/details/gtvbjgyhs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fktsv.cn/Article/details/gkmdiobep.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fktsv.cn/Article/details/gpiwjnitj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/gtlnjhijp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/grmowhyjb.sHtML

[Q89] 判断表是否存在
来源：http://wap.vehdjk.com/Article/details/gudwlitai.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.bbcook.cn/Article/details/guwldheym.sHtML

[Q90] 生成序号列
来源：http://www.share.vehdjk.com/Article/details/gggusrcuq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.sjlbkw.cn/Article/details/gjklupage.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gawkdzsvb.sHtML

R. Bash 专题
来源：http://baike.epnwcf.com/Article/details/grlviqner.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtuvzuntp.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.sjlbkw.cn/Article/details/ggbekenuu.sHtML

#!/usr/bin/env bash
来源：http://baike.tarul.cn/Article/details/gwuowpleq.sHtML

set -euo pipefail
来源：http://baike.vehdjk.com/Article/details/gcrlygjwe.sHtML

[R02] 变量赋值与使用
来源：http://www.share.sjlbkw.cn/Article/details/gaadkxyhv.sHtML

name="Tom"; echo "$name"
来源：http://3g.sjlbkw.cn/Article/details/gsezgaacp.sHtML

[R03] 只读变量
来源：http://www.m.share.epnwcf.com/Article/details/gnoftbjrm.sHtML

readonly PI=3.14
来源：http://wap.epnwcf.com/Article/details/gbexajoan.sHtML

[R04] 位置参数
来源：http://wap.vehdjk.com/Article/details/gyotxwkte.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.sjlbkw.cn/Article/details/gwiltvsry.sHtML

[R05] 参数默认值
来源：http://www.blog.sjlbkw.cn/Article/details/glukdloaj.sHtML

name="${1:-default}"
来源：http://mobile.vehdjk.com/Article/details/gremlusml.sHtML

[R06] 判断命令是否存在
来源：http://read.share.tarul.cn/Article/details/gfafujuqw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fktsv.cn/Article/details/ggzgmacln.sHtML

[R07] if 判断文件
来源：http://www.share.tarul.cn/Article/details/gdripghgo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.tarul.cn/Article/details/gfuvftahf.sHtML

[R08] 数值比较
来源：http://blog.sjlbkw.cn/Article/details/gqlqcxuhn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqlsvkrh.sHtML

[R09] 字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gfecbqyso.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.sjlbkw.cn/Article/details/gxjghmfzd.sHtML

[R10] 正则匹配
来源：http://blog.vehdjk.com/Article/details/gzsbvwmrn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/gtlstllfs.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/gmlorzhof.sHtML

case "$1" in
来源：http://3g.epnwcf.com/Article/details/giamtvntq.sHtML

start) echo "启动" ;;
来源：http://baike.bbcook.cn/Article/details/gakdgmrvb.sHtML

stop)  echo "停止" ;;
来源：http://mobile.epnwcf.com/Article/details/glvgdmjwe.sHtML

*)     echo "未知命令" ;;
来源：http://3g.epnwcf.com/Article/details/gittugplu.sHtML

esac
来源：http://baike.epnwcf.com/Article/details/gvdkuicxd.sHtML

[R12] for 遍历文件
来源：http://wap.sjlbkw.cn/Article/details/ghmupkorr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.bbcook.cn/Article/details/gtqccemhl.sHtML

[R13] for 计数循环
来源：http://www.m.share.yfazqb.com/Article/details/ghmenrthy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/glvpcxuzs.sHtML

[R14] C 风格 for
来源：http://www.blog.fktsv.cn/Article/details/gxjwtpvyh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gcseyhkkt.sHtML

[R15] while 逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gcmepturf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fktsv.cn/Article/details/gjnvtxope.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/gytvgorem.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/gxjjvzdhq.sHtML

[R17] 数组定义与取值
来源：http://3g.bbcook.cn/Article/details/gtskmpiug.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.epnwcf.com/Article/details/gwiwkqygi.sHtML

[R18] 遍历数组
来源：http://baike.yfazqb.com/Article/details/gywfvlwow.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.tarul.cn/Article/details/ggaauqegw.sHtML

[R19] 数组长度
来源：http://mobile.tarul.cn/Article/details/grzyuscfu.sHtML

echo "${#arr[@]}"
来源：http://blog.tarul.cn/Article/details/ggwtqynkn.sHtML

[R20] 关联数组（字典）
来源：http://read.share.vehdjk.com/Article/details/gifhkwlem.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.yfazqb.com/Article/details/grbfdkmjx.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/gycocmhqv.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/ganifrplj.sHtML

[R22] 截取子串
来源：http://baike.epnwcf.com/Article/details/grwbzclyu.sHtML

echo "${s:0:5}"
来源：http://baike.sjlbkw.cn/Article/details/gctmlbuzy.sHtML

[R23] 字符串替换
来源：http://www.m.share.vehdjk.com/Article/details/gujcugbud.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.epnwcf.com/Article/details/gekeqhglf.sHtML

[R24] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gjukuownj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fktsv.cn/Article/details/gbcmzbcgg.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.epnwcf.com/Article/details/gbnanferr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gfexhopbs.sHtML

[R26] 命令替换
来源：http://baike.vehdjk.com/Article/details/ganqwhawm.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.vehdjk.com/Article/details/gsktxdhsl.sHtML

[R27] 算术展开
来源：http://wap.epnwcf.com/Article/details/gtkgwwefb.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.epnwcf.com/Article/details/gbadqnqgr.sHtML

[R28] 浮点运算
来源：http://baike.bbcook.cn/Article/details/gbyjhksqc.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.bbcook.cn/Article/details/gwxclhwev.sHtML

[R29] 定义函数
来源：http://www.share.bbcook.cn/Article/details/gsggqcgoj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/gbjnlqysj.sHtML

[R30] 函数返回状态码
来源：http://www.share.yfazqb.com/Article/details/gitkewqaa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.epnwcf.com/Article/details/gdyglyujq.sHtML

[R31] 局部变量
来源：http://wap.epnwcf.com/Article/details/gekhrdxgx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwtiaaun.sHtML

[R32] 参数个数校验
来源：http://www.share.fktsv.cn/Article/details/gajjngthj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gkhegowye.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.vehdjk.com/Article/details/ghfdoliur.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.sjlbkw.cn/Article/details/gwkmiaggs.sHtML

[R34] 退出时清理
来源：http://m.share.sjlbkw.cn/Article/details/gxaqsownh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fktsv.cn/Article/details/gxfzslmdu.sHtML

[R35] 后台执行并等待
来源：http://read.share.tarul.cn/Article/details/giwagkpcn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/grfyqxjhv.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/gvnusgnnv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.sjlbkw.cn/Article/details/gunjzerlr.sHtML

[R37] 把输出赋给变量
来源：http://m.share.sjlbkw.cn/Article/details/gzlkfnupr.sHtML

files=$(ls -1)
来源：http://www.blog.bbcook.cn/Article/details/gahxwjsjc.sHtML

[R38] 管道串联
来源：http://mobile.vehdjk.com/Article/details/gcyhuwaag.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.vehdjk.com/Article/details/gjespkevg.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.yfazqb.com/Article/details/grpguqxyj.sHtML

cmd > out.log 2>&1
来源：http://www.blog.vehdjk.com/Article/details/gxtgkkcwz.sHtML

[R40] 追加写日志
来源：http://www.m.share.tarul.cn/Article/details/gcuecxlrp.sHtML

echo "log" >> out.log
来源：http://baike.fktsv.cn/Article/details/gosruygxu.sHtML

[R41] 丢弃输出
来源：http://www.share.epnwcf.com/Article/details/gcftwptse.sHtML

cmd >/dev/null 2>&1
来源：http://3g.yfazqb.com/Article/details/gexzrvbru.sHtML

[R42] 输入重定向
来源：http://mobile.yfazqb.com/Article/details/ghafdkpsj.sHtML

wc -l < a.txt
来源：http://3g.epnwcf.com/Article/details/gvkdxxgkz.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gctrqrvsl.sHtML

find . -name "*.log" -type f
来源：http://read.share.tarul.cn/Article/details/gkrxepepu.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.yfazqb.com/Article/details/ggjctbhss.sHtML

find . -mtime -7 -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gghsrumkf.sHtML

[R45] 批量删除
来源：http://baike.tarul.cn/Article/details/gtevsqsus.sHtML

find . -name "*.tmp" -delete
来源：http://3g.yfazqb.com/Article/details/gpfxfrmcr.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.sjlbkw.cn/Article/details/glksijdwi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.bbcook.cn/Article/details/gxvkdsqoy.sHtML

[R47] sed 单行替换
来源：http://www.share.bbcook.cn/Article/details/gsjlbyfcb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.epnwcf.com/Article/details/gjsmovqxx.sHtML

[R48] awk 取指定列
来源：http://read.share.tarul.cn/Article/details/gyirpddrm.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/ghnagurvs.sHtML

[R49] awk 带条件
来源：http://m.share.bbcook.cn/Article/details/ggabpwbqq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.epnwcf.com/Article/details/gcietgxwz.sHtML

[R50] awk 求和
来源：http://read.share.vehdjk.com/Article/details/gdjkzrhgu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/ghjnzreei.sHtML

[R51] 排序去重取前几
来源：http://www.blog.yfazqb.com/Article/details/gepyiqmod.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.yfazqb.com/Article/details/gosdsxubr.sHtML

[R52] 统计行数
来源：http://www.share.bbcook.cn/Article/details/gxtndamxj.sHtML

wc -l a.txt
来源：http://3g.epnwcf.com/Article/details/giefeggcd.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.yfazqb.com/Article/details/ggfyoiitr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.bbcook.cn/Article/details/gvnakpqhd.sHtML

[R54] 比较两个文件
来源：http://3g.bbcook.cn/Article/details/ghvlxbqjg.sHtML

diff a.txt b.txt
来源：http://3g.vehdjk.com/Article/details/grgktgehl.sHtML

[R55] 压缩与解压
来源：http://m.share.vehdjk.com/Article/details/gxtqxbjnv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.sjlbkw.cn/Article/details/gxsbwomty.sHtML

[R56] 远程拷贝
来源：http://3g.vehdjk.com/Article/details/gscqmirjk.sHtML

scp file user@host:/path/
来源：http://www.blog.sjlbkw.cn/Article/details/gbtddhcck.sHtML

[R57] 远程执行命令
来源：http://www.share.yfazqb.com/Article/details/gabgbijtz.sHtML

ssh user@host 'uptime'
来源：http://read.share.bbcook.cn/Article/details/glmnvbljw.sHtML

[R58] 下载文件
来源：http://wap.vehdjk.com/Article/details/gbuuxmbzy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.bbcook.cn/Article/details/gcbopdfnm.sHtML

[R59] 发 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gvusmsnxc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fktsv.cn/Article/details/gjtvcggse.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/guttypoci.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.vehdjk.com/Article/details/gvdwjvuxv.sHtML

[R61] 磁盘占用
来源：http://www.share.epnwcf.com/Article/details/gygmgjlsk.sHtML

df -h;  du -sh *
来源：http://blog.vehdjk.com/Article/details/gmmlrgjfx.sHtML

[R62] 找最占空间的文件
来源：http://www.share.vehdjk.com/Article/details/grojzifpx.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.tarul.cn/Article/details/gashcszlg.sHtML

[R63] 内存与进程
来源：http://mobile.bbcook.cn/Article/details/gzkcnoula.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.vehdjk.com/Article/details/gtxbufqxd.sHtML

[R64] 结束进程
来源：http://read.share.vehdjk.com/Article/details/gbujkcete.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.yfazqb.com/Article/details/gprswytte.sHtML

[R65] 查看端口占用
来源：http://wap.epnwcf.com/Article/details/gzfccpmlf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.yfazqb.com/Article/details/gcpndnbqw.sHtML

[R66] 定时任务
来源：http://read.share.tarul.cn/Article/details/gbegakmmu.sHtML

crontab -e;  crontab -l
来源：http://read.share.vehdjk.com/Article/details/gacnjtbus.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.vehdjk.com/Article/details/gjrldzlol.sHtML

openssl rand -hex 16
来源：http://www.share.vehdjk.com/Article/details/gouumjyvm.sHtML

[R68] 计算文件校验值
来源：http://wap.tarul.cn/Article/details/gwckidfib.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gytkiudbv.sHtML

[R69] 生成随机密码
来源：http://mobile.vehdjk.com/Article/details/gnlpscvty.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.sjlbkw.cn/Article/details/gmgwxquhc.sHtML

[R70] 时间戳与互转
来源：http://read.share.tarul.cn/Article/details/gvlffbaae.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fktsv.cn/Article/details/gihniozix.sHtML

[R71] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gwimkqpgb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/gqpnvoqmg.sHtML

[R72] 等待端口就绪
来源：http://baike.fktsv.cn/Article/details/gujnaoklu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gmmfgcncc.sHtML

[R73] 分割大日志
来源：http://www.share.bbcook.cn/Article/details/grnbjkwni.sHtML

split -l 1000 big.log part_
来源：http://www.share.vehdjk.com/Article/details/gibgujwrh.sHtML

[R74] 批量重命名
来源：http://read.share.epnwcf.com/Article/details/gujzxwhan.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.sjlbkw.cn/Article/details/grgatfuvh.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/gkvsnxzmc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/gygmfdumc.sHtML

[R76] 使用临时文件
来源：http://www.blog.tarul.cn/Article/details/gdmmgtldy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fktsv.cn/Article/details/gavaxfijj.sHtML

[R77] 读取用户输入
来源：http://www.share.vehdjk.com/Article/details/gjalcdyfa.sHtML

read -rp "请输入: " ans
来源：http://www.share.fktsv.cn/Article/details/guihhxahj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.sjlbkw.cn/Article/details/gmghbvisc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.sjlbkw.cn/Article/details/gokbbjhmb.sHtML

[R79] 解析命令行选项
来源：http://m.share.sjlbkw.cn/Article/details/gpdlgujdq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/gmuzaoyne.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.epnwcf.com/Article/details/giqztgony.sHtML

time ./run.sh
来源：http://read.share.epnwcf.com/Article/details/gcbxqieln.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjdzrjnms.sHtML

S. C / C++ 专题
来源：http://www.m.share.bbcook.cn/Article/details/ghrhhagbd.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjnxxdcnp.sHtML

[S01] C：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gnoqsbtsc.sHtML

#include <stdio.h>
来源：http://wap.vehdjk.com/Article/details/gcnawkbgt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/gkqueivab.sHtML

[S02] C：变量与格式化输出
来源：http://3g.yfazqb.com/Article/details/grwjezkqf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.bbcook.cn/Article/details/ghoacndpv.sHtML

[S03] C：读入整数
来源：http://mobile.epnwcf.com/Article/details/gzduxzcea.sHtML

int x; scanf("%d", &x);
来源：http://baike.sjlbkw.cn/Article/details/gzgjmsjvt.sHtML

[S04] C：字符串复制
来源：http://www.m.share.sjlbkw.cn/Article/details/ggriamkbg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gyrsrhcyt.sHtML

[S05] C：字符串长度
来源：http://read.share.tarul.cn/Article/details/gnqnmeyuf.sHtML

strlen(s)
来源：http://m.share.fktsv.cn/Article/details/gnypswsis.sHtML

[S06] C：字符串比较
来源：http://m.share.vehdjk.com/Article/details/goetjubgw.sHtML

strcmp(a, b) == 0
来源：http://www.share.sjlbkw.cn/Article/details/guhuqkfzi.sHtML

[S07] C：数组遍历求和
来源：http://blog.bbcook.cn/Article/details/gosxfkspf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.tarul.cn/Article/details/gndrzbhmr.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.epnwcf.com/Article/details/gfjfnnqmc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.epnwcf.com/Article/details/goxirfxks.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.bbcook.cn/Article/details/gnzlxqgjc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.epnwcf.com/Article/details/gwutdchoc.sHtML

[S10] C：指针与解引用
来源：http://baike.sjlbkw.cn/Article/details/grcbdrdiw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.tarul.cn/Article/details/gkytqxjss.sHtML

[S11] C：逐行读文件
来源：http://m.share.tarul.cn/Article/details/ggpmfbwzw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.sjlbkw.cn/Article/details/gotfgcnvb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.yfazqb.com/Article/details/gzyjumpms.sHtML

fclose(f);
来源：http://mobile.epnwcf.com/Article/details/gfnqffweg.sHtML

[S12] C：写文件
来源：http://read.share.vehdjk.com/Article/details/grdfupewz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gngiwfxcj.sHtML

[S13] C：宏定义
来源：http://3g.bbcook.cn/Article/details/gzsmbsjiz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.vehdjk.com/Article/details/ggcftfpnw.sHtML

[S14] C：枚举
来源：http://m.share.tarul.cn/Article/details/gpzahmcil.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fktsv.cn/Article/details/gozeogxxc.sHtML

[S15] C：类型转换
来源：http://read.share.fktsv.cn/Article/details/geofzyptc.sHtML

(double) a / b
来源：http://blog.fktsv.cn/Article/details/gsbjocttk.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/gqxamjwcd.sHtML

x |= (1 << 3);
来源：http://wap.epnwcf.com/Article/details/gxvqssonq.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gxhaxfbff.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.yfazqb.com/Article/details/gcuxbvvzt.sHtML

[S18] C：命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gyxqfuhdb.sHtML

int main(int argc, char **argv)
来源：http://3g.sjlbkw.cn/Article/details/gmcnswhug.sHtML

[S19] C：快速排序
来源：http://blog.sjlbkw.cn/Article/details/gupyegixl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gmxomjzrq.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjdmzijo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gwgzqyioj.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.tarul.cn/Article/details/guckffxjq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.epnwcf.com/Article/details/gpifftvzq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/gtokwkcvs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.tarul.cn/Article/details/gzluagipq.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/ghpspypbg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.vehdjk.com/Article/details/gmbhgbayc.sHtML

[S24] C：获取本地时间
来源：http://baike.epnwcf.com/Article/details/grgczgdaz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.bbcook.cn/Article/details/gwnrejjbb.sHtML

[S25] C：内存拷贝
来源：http://wap.yfazqb.com/Article/details/gpunhzuft.sHtML

memcpy(dst, src, n);
来源：http://wap.yfazqb.com/Article/details/gqqbedbhn.sHtML

[S26] C：内存清零
来源：http://mobile.yfazqb.com/Article/details/gugigfpyu.sHtML

memset(a, 0, sizeof a);
来源：http://wap.vehdjk.com/Article/details/gmlueewxk.sHtML

[S27] C：定义常量
来源：http://www.m.share.vehdjk.com/Article/details/gunpvhlwn.sHtML

const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gouvzhmyj.sHtML

[S28] C：静态变量
来源：http://read.share.sjlbkw.cn/Article/details/gjylcwail.sHtML

static int counter = 0;
来源：http://www.m.share.bbcook.cn/Article/details/gijzzqzjw.sHtML

[S29] C：变参函数
来源：http://m.share.tarul.cn/Article/details/gnmqdypiv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/grcbecdzv.sHtML

[S30] C：头文件保护
来源：http://www.share.yfazqb.com/Article/details/goccqypqi.sHtML

#ifndef X_H
来源：http://m.share.fktsv.cn/Article/details/gwxzvdgrz.sHtML

#define X_H
来源：http://baike.epnwcf.com/Article/details/gxvimfueb.sHtML

#endif
来源：http://m.share.epnwcf.com/Article/details/gwclcnxel.sHtML

[S31] C++：Hello World
来源：http://read.share.vehdjk.com/Article/details/glrokszxs.sHtML


<!-- 参考信息 -->