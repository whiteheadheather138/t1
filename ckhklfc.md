代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gziaxhjot.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.epnwcf.com/Article/details/gzuaagfzz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.sjlbkw.cn/Article/details/giozgwgld.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gelgzaavp.sHtML

[Q61] 移动平均
来源：http://www.share.vehdjk.com/Article/details/gatvizryg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gfnwqahtj.sHtML

[Q62] 分组占比
来源：http://3g.tarul.cn/Article/details/gvpmppmqs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gytdtkcvl.sHtML

[Q63] 开启事务
来源：http://wap.tarul.cn/Article/details/gwykrzkij.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fktsv.cn/Article/details/gmmmezjom.sHtML

[Q64] 提交事务
来源：http://blog.epnwcf.com/Article/details/gibtgzhnm.sHtML

COMMIT;
来源：http://www.blog.sjlbkw.cn/Article/details/gnafjbfcn.sHtML

[Q65] 回滚事务
来源：http://mobile.fktsv.cn/Article/details/glyvtmurt.sHtML

ROLLBACK;
来源：http://baike.fktsv.cn/Article/details/gsazkamuq.sHtML

[Q66] 行锁查询
来源：http://www.share.vehdjk.com/Article/details/gbizknlav.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.sjlbkw.cn/Article/details/gxfwsudzc.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.vehdjk.com/Article/details/gmhiezubs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fktsv.cn/Article/details/gnfxoxrky.sHtML

[Q68] 保存点
来源：http://blog.epnwcf.com/Article/details/gwmkxukyu.sHtML

SAVEPOINT sp1;
来源：http://mobile.fktsv.cn/Article/details/gvorbbrta.sHtML

ROLLBACK TO sp1;
来源：http://baike.yfazqb.com/Article/details/ggppqmwgd.sHtML

[Q69] 查看执行计划
来源：http://blog.sjlbkw.cn/Article/details/gsvvthigt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.vehdjk.com/Article/details/gybhrmspo.sHtML

[Q70] 更新统计信息
来源：http://m.share.tarul.cn/Article/details/guksszbdi.sHtML

ANALYZE TABLE users;
来源：http://baike.bbcook.cn/Article/details/gzbvguzxp.sHtML

[Q71] 查看建表语句
来源：http://baike.fktsv.cn/Article/details/gvdlbgvck.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fktsv.cn/Article/details/gkgrldrzs.sHtML

[Q72] 查看索引
来源：http://wap.tarul.cn/Article/details/giqlcvkte.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gnsulnlaj.sHtML

[Q73] 查看表状态
来源：http://wap.vehdjk.com/Article/details/gsydaxijv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.sjlbkw.cn/Article/details/gwudrrvba.sHtML

[Q74] 强制使用索引
来源：http://3g.epnwcf.com/Article/details/gfmsfvfym.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fktsv.cn/Article/details/gjalgkngf.sHtML

[Q75] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gkznsxndc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.vehdjk.com/Article/details/gmyoqposn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.epnwcf.com/Article/details/gvydtumkp.sHtML

[Q76] 按天统计
来源：http://blog.yfazqb.com/Article/details/gavpheeqp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.epnwcf.com/Article/details/gcxopwyux.sHtML

[Q77] 时间加减
来源：http://blog.sjlbkw.cn/Article/details/gkzlnbjla.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.tarul.cn/Article/details/gxkgkrqnv.sHtML

[Q78] 当前时间
来源：http://baike.yfazqb.com/Article/details/gghobhkeh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.sjlbkw.cn/Article/details/geduhqoex.sHtML

[Q79] 字符串拼接
来源：http://m.share.epnwcf.com/Article/details/ganlqfady.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.tarul.cn/Article/details/gzutlaucp.sHtML

[Q80] 字符串截取
来源：http://blog.bbcook.cn/Article/details/gaoenxgiw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gciuwrjwf.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gdwqiiniu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.tarul.cn/Article/details/gowfhrqab.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.epnwcf.com/Article/details/gqienausf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gthmdyutd.sHtML

[Q83] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gipzsffdq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gqocvfsrb.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.sjlbkw.cn/Article/details/gmoaonklt.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gqtxlawvf.sHtML

[Q85] 数值取整
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwxovlgo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.vehdjk.com/Article/details/gyboyrjbc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/gikjkmiep.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.yfazqb.com/Article/details/gtclydzec.sHtML

[Q87] JSON 字段做条件
来源：http://baike.epnwcf.com/Article/details/gijywaeaq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fktsv.cn/Article/details/gptqzwtlf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.sjlbkw.cn/Article/details/gcgkqygtc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.vehdjk.com/Article/details/gbsudljyn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.epnwcf.com/Article/details/gqvvxpccs.sHtML

[Q89] 判断表是否存在
来源：http://m.share.yfazqb.com/Article/details/gzijilkjg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.bbcook.cn/Article/details/gygriftjs.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fktsv.cn/Article/details/gyijkflvp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.sjlbkw.cn/Article/details/goqvnkkof.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gyhriujmo.sHtML

R. Bash 专题
来源：http://mobile.sjlbkw.cn/Article/details/gfzijlaur.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gohhvbsfq.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/gstlghrpi.sHtML

#!/usr/bin/env bash
来源：http://mobile.bbcook.cn/Article/details/ghiwufrhf.sHtML

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/goxmqkghx.sHtML

[R02] 变量赋值与使用
来源：http://baike.bbcook.cn/Article/details/gmdoicwfg.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.bbcook.cn/Article/details/gdyxybzmv.sHtML

[R03] 只读变量
来源：http://3g.epnwcf.com/Article/details/gyuufyvvh.sHtML

readonly PI=3.14
来源：http://blog.sjlbkw.cn/Article/details/gmnlslqks.sHtML

[R04] 位置参数
来源：http://www.m.share.fktsv.cn/Article/details/gcnyyfcry.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.yfazqb.com/Article/details/ghpfxxgvz.sHtML

[R05] 参数默认值
来源：http://blog.fktsv.cn/Article/details/gqhjmukvc.sHtML

name="${1:-default}"
来源：http://www.m.share.sjlbkw.cn/Article/details/golyeuouz.sHtML

[R06] 判断命令是否存在
来源：http://baike.vehdjk.com/Article/details/gvqxynmbg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/gjqjverpa.sHtML

[R07] if 判断文件
来源：http://www.share.fktsv.cn/Article/details/giwbrycyd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.vehdjk.com/Article/details/gmcfgxcsg.sHtML

[R08] 数值比较
来源：http://baike.tarul.cn/Article/details/ghivxjxlz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.tarul.cn/Article/details/gnncfsnzc.sHtML

[R09] 字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/gvvdvrdll.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.vehdjk.com/Article/details/gwxojuigf.sHtML

[R10] 正则匹配
来源：http://wap.tarul.cn/Article/details/godmkqeok.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.vehdjk.com/Article/details/gcylpsopl.sHtML

[R11] case 多分支
来源：http://3g.tarul.cn/Article/details/gimswbggw.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/goysmyuul.sHtML

start) echo "启动" ;;
来源：http://read.share.yfazqb.com/Article/details/gpuzzfqjq.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fktsv.cn/Article/details/gpcedqrvo.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.yfazqb.com/Article/details/gqpkqzplw.sHtML

esac
来源：http://wap.bbcook.cn/Article/details/gwwpprhjp.sHtML

[R12] for 遍历文件
来源：http://3g.vehdjk.com/Article/details/grkhdasmf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.tarul.cn/Article/details/gfzjybaeg.sHtML

[R13] for 计数循环
来源：http://3g.tarul.cn/Article/details/gkzlbclai.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gtmsbbzvj.sHtML

[R14] C 风格 for
来源：http://www.m.share.tarul.cn/Article/details/gpmhmmowq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/gwifkzfgy.sHtML

[R15] while 逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gxtgtsvim.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.yfazqb.com/Article/details/glqyygixm.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/gnhlkpkos.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/govltiwub.sHtML

[R17] 数组定义与取值
来源：http://www.share.yfazqb.com/Article/details/glkgyvowf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fktsv.cn/Article/details/gngdlnfao.sHtML

[R18] 遍历数组
来源：http://m.share.epnwcf.com/Article/details/gbtqlvhat.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.epnwcf.com/Article/details/guwflpzwy.sHtML

[R19] 数组长度
来源：http://wap.yfazqb.com/Article/details/gyodsmfgn.sHtML

echo "${#arr[@]}"
来源：http://wap.tarul.cn/Article/details/gujjetrop.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fktsv.cn/Article/details/gauapavqf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/geoqdurxa.sHtML

[R21] 字符串长度
来源：http://wap.yfazqb.com/Article/details/gkroysxej.sHtML

echo "${#s}"
来源：http://www.share.tarul.cn/Article/details/gqvfqgahv.sHtML

[R22] 截取子串
来源：http://baike.tarul.cn/Article/details/gpzdiwzxx.sHtML

echo "${s:0:5}"
来源：http://mobile.fktsv.cn/Article/details/gbjulbkdr.sHtML

[R23] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gjorctgel.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.sjlbkw.cn/Article/details/gwagcojni.sHtML

[R24] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gfovikihk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.sjlbkw.cn/Article/details/gbzobtjkp.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.sjlbkw.cn/Article/details/gxecetmjq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.vehdjk.com/Article/details/gdoohgmuo.sHtML

[R26] 命令替换
来源：http://www.blog.fktsv.cn/Article/details/gociqmqeg.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fktsv.cn/Article/details/goknmujuv.sHtML

[R27] 算术展开
来源：http://mobile.vehdjk.com/Article/details/gtcpvzbdl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.tarul.cn/Article/details/gfueszyiu.sHtML

[R28] 浮点运算
来源：http://m.share.tarul.cn/Article/details/gbyrnbgsa.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.yfazqb.com/Article/details/golabtmgu.sHtML

[R29] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gimszptdg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fktsv.cn/Article/details/gnagvumgy.sHtML

[R30] 函数返回状态码
来源：http://m.share.vehdjk.com/Article/details/gcusgtenb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fktsv.cn/Article/details/gbwfwjgbw.sHtML

[R31] 局部变量
来源：http://m.share.vehdjk.com/Article/details/gksbowcdk.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/gsxmmumjt.sHtML

[R32] 参数个数校验
来源：http://read.share.sjlbkw.cn/Article/details/gafgsphza.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/gjqbqkpzg.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.bbcook.cn/Article/details/guzbbypil.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.epnwcf.com/Article/details/gkknjgqbc.sHtML

[R34] 退出时清理
来源：http://baike.epnwcf.com/Article/details/gpwwtwlff.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/gkensfmtg.sHtML

[R35] 后台执行并等待
来源：http://wap.vehdjk.com/Article/details/ggdvaxola.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/gegdshuwy.sHtML

[R36] 并发执行多个任务
来源：http://www.share.sjlbkw.cn/Article/details/gjtlumezo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.tarul.cn/Article/details/grlsjpxwp.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.tarul.cn/Article/details/gvlmtevcn.sHtML

files=$(ls -1)
来源：http://www.share.epnwcf.com/Article/details/gekkchrbo.sHtML

[R38] 管道串联
来源：http://blog.bbcook.cn/Article/details/glpxjvrzu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.tarul.cn/Article/details/gdqlngmuj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.sjlbkw.cn/Article/details/gtrscouui.sHtML

cmd > out.log 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gtwojuzyr.sHtML

[R40] 追加写日志
来源：http://m.share.bbcook.cn/Article/details/grhisqegu.sHtML

echo "log" >> out.log
来源：http://mobile.fktsv.cn/Article/details/guockbecq.sHtML

[R41] 丢弃输出
来源：http://mobile.vehdjk.com/Article/details/gzkjwjjxm.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.bbcook.cn/Article/details/gctdzttyp.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/giciakcaw.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/gfpygezzc.sHtML

[R43] 按名字查找文件
来源：http://3g.sjlbkw.cn/Article/details/gcnkcrhck.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gcczckwnp.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/gtkuwydrg.sHtML

find . -mtime -7 -type f
来源：http://m.share.tarul.cn/Article/details/ghwtpliuc.sHtML

[R45] 批量删除
来源：http://www.blog.tarul.cn/Article/details/gtgxdgwbr.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gpbyostnu.sHtML

[R46] 递归替换文件内容
来源：http://www.share.yfazqb.com/Article/details/gwgftokgh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.yfazqb.com/Article/details/gwxmrxrdu.sHtML

[R47] sed 单行替换
来源：http://wap.bbcook.cn/Article/details/goyqmwuga.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.tarul.cn/Article/details/gazhzdewp.sHtML

[R48] awk 取指定列
来源：http://www.share.yfazqb.com/Article/details/gtwprwbjl.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gpwbtfduj.sHtML

[R49] awk 带条件
来源：http://read.share.sjlbkw.cn/Article/details/gktpxsavt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/gmlavykbg.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/gdrwybgdu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gklgnjsvq.sHtML

[R51] 排序去重取前几
来源：http://blog.sjlbkw.cn/Article/details/gxkobrkks.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.tarul.cn/Article/details/gcndxklzm.sHtML

[R52] 统计行数
来源：http://read.share.tarul.cn/Article/details/gdduaxold.sHtML

wc -l a.txt
来源：http://www.m.share.tarul.cn/Article/details/gtwsibdqr.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.bbcook.cn/Article/details/grufgloib.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fktsv.cn/Article/details/gervaoavi.sHtML

[R54] 比较两个文件
来源：http://3g.yfazqb.com/Article/details/gosojqvrp.sHtML

diff a.txt b.txt
来源：http://www.share.bbcook.cn/Article/details/gquksncse.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/gebzrgqka.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.sjlbkw.cn/Article/details/gnvbvnvec.sHtML

[R56] 远程拷贝
来源：http://wap.fktsv.cn/Article/details/gnowuuzzm.sHtML

scp file user@host:/path/
来源：http://www.m.share.vehdjk.com/Article/details/gaqugqarq.sHtML

[R57] 远程执行命令
来源：http://mobile.sjlbkw.cn/Article/details/gehnhniig.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/ggwrimheb.sHtML

[R58] 下载文件
来源：http://blog.vehdjk.com/Article/details/giozivwnm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.epnwcf.com/Article/details/gpmjmsehx.sHtML

[R59] 发 POST JSON
来源：http://3g.epnwcf.com/Article/details/ghxptzrzg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/gmphbitpp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/grrwxwdoc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.bbcook.cn/Article/details/gciaydlxw.sHtML

[R61] 磁盘占用
来源：http://3g.epnwcf.com/Article/details/gvoxqhsln.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/gzmuyonxs.sHtML

[R62] 找最占空间的文件
来源：http://read.share.tarul.cn/Article/details/gxijhjplk.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.vehdjk.com/Article/details/gjplvghzb.sHtML

[R63] 内存与进程
来源：http://wap.bbcook.cn/Article/details/gkbwiqnfg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzurpacp.sHtML

[R64] 结束进程
来源：http://read.share.bbcook.cn/Article/details/gbzlhbvxd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.tarul.cn/Article/details/grsraonau.sHtML

[R65] 查看端口占用
来源：http://mobile.fktsv.cn/Article/details/gzboovcrp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.sjlbkw.cn/Article/details/ghffyqjzc.sHtML

[R66] 定时任务
来源：http://wap.vehdjk.com/Article/details/gnebfdwrv.sHtML

crontab -e;  crontab -l
来源：http://read.share.sjlbkw.cn/Article/details/gugopdulm.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.vehdjk.com/Article/details/gzlqsflav.sHtML

openssl rand -hex 16
来源：http://mobile.tarul.cn/Article/details/gjfmcjfaf.sHtML

[R68] 计算文件校验值
来源：http://www.blog.epnwcf.com/Article/details/gkimbimkp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/geyyhzvwd.sHtML

[R69] 生成随机密码
来源：http://m.share.yfazqb.com/Article/details/gpkffswuv.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/gvnuomskl.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.epnwcf.com/Article/details/ggxnwygjy.sHtML

date +%s;  date -d @1700000000
来源：http://baike.sjlbkw.cn/Article/details/gjjusochc.sHtML

[R71] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gwmibbifp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.epnwcf.com/Article/details/ghvdqelms.sHtML

[R72] 等待端口就绪
来源：http://baike.yfazqb.com/Article/details/gygrvboox.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gpjzgslfa.sHtML

[R73] 分割大日志
来源：http://www.blog.sjlbkw.cn/Article/details/ggxyxqhix.sHtML

split -l 1000 big.log part_
来源：http://wap.epnwcf.com/Article/details/gjbgnwzwh.sHtML

[R74] 批量重命名
来源：http://www.m.share.epnwcf.com/Article/details/gfqgllphd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.yfazqb.com/Article/details/gjogszyxc.sHtML

[R75] 导出环境变量
来源：http://read.share.tarul.cn/Article/details/gkphrylpz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.vehdjk.com/Article/details/gfxrmpsyf.sHtML

[R76] 使用临时文件
来源：http://mobile.vehdjk.com/Article/details/gvqemcnri.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gcphtvcxv.sHtML

[R77] 读取用户输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfwkzbei.sHtML

read -rp "请输入: " ans
来源：http://m.share.fktsv.cn/Article/details/gbieqgavc.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/gzkooslhm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.tarul.cn/Article/details/guromlgib.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.vehdjk.com/Article/details/gxvuiumme.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.tarul.cn/Article/details/ghowwbodm.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.sjlbkw.cn/Article/details/gxgwpenwo.sHtML

time ./run.sh
来源：http://read.share.tarul.cn/Article/details/giqpejnwj.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdrvvdflf.sHtML

S. C / C++ 专题
来源：http://baike.bbcook.cn/Article/details/gywnlmway.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gafxqpwhv.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/gfdfspibe.sHtML

#include <stdio.h>
来源：http://mobile.yfazqb.com/Article/details/gifftnwcv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.yfazqb.com/Article/details/grxdwfguu.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/geevfpiaz.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.yfazqb.com/Article/details/gubuqcdez.sHtML

[S03] C：读入整数
来源：http://wap.fktsv.cn/Article/details/giujtehjh.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fktsv.cn/Article/details/glbyxjpjb.sHtML

[S04] C：字符串复制
来源：http://baike.tarul.cn/Article/details/gybetfejd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fktsv.cn/Article/details/gnzyzbfey.sHtML

[S05] C：字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gwpwmqqni.sHtML

strlen(s)
来源：http://www.blog.sjlbkw.cn/Article/details/grnwjkbjn.sHtML

[S06] C：字符串比较
来源：http://m.share.tarul.cn/Article/details/gwpagptia.sHtML

strcmp(a, b) == 0
来源：http://mobile.sjlbkw.cn/Article/details/gxekeiqjm.sHtML

[S07] C：数组遍历求和
来源：http://mobile.vehdjk.com/Article/details/gcjhanhtu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.bbcook.cn/Article/details/gcfwiqonn.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.tarul.cn/Article/details/gxiovnfbo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.tarul.cn/Article/details/gjvplkpfb.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.tarul.cn/Article/details/gbedmuaqu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.bbcook.cn/Article/details/gqjzmqnom.sHtML

[S10] C：指针与解引用
来源：http://baike.epnwcf.com/Article/details/gzapdzciy.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fktsv.cn/Article/details/gliavybhi.sHtML

[S11] C：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gbenubcas.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.sjlbkw.cn/Article/details/gozzewnkg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.vehdjk.com/Article/details/ggnasogdg.sHtML

fclose(f);
来源：http://wap.bbcook.cn/Article/details/gnqxjnxqq.sHtML

[S12] C：写文件
来源：http://read.share.tarul.cn/Article/details/gtvtmtvst.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/grackkytk.sHtML

[S13] C：宏定义
来源：http://wap.epnwcf.com/Article/details/gxlyuushc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/ggnoktvwl.sHtML

[S14] C：枚举
来源：http://3g.bbcook.cn/Article/details/gkmlklmju.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.epnwcf.com/Article/details/gezexejot.sHtML

[S15] C：类型转换
来源：http://baike.sjlbkw.cn/Article/details/gyahxphpv.sHtML

(double) a / b
来源：http://mobile.sjlbkw.cn/Article/details/gctopiisy.sHtML

[S16] C：位操作置位
来源：http://mobile.sjlbkw.cn/Article/details/gwrkgiyyb.sHtML

x |= (1 << 3);
来源：http://www.blog.tarul.cn/Article/details/glurwtohv.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/gslzxnkev.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.epnwcf.com/Article/details/gtacwotip.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/gwfjstvmt.sHtML

int main(int argc, char **argv)
来源：http://mobile.bbcook.cn/Article/details/gaknwsren.sHtML

[S19] C：快速排序
来源：http://baike.fktsv.cn/Article/details/gviepfhmp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gkgzmplbx.sHtML

[S20] C：二分查找
来源：http://blog.tarul.cn/Article/details/gadrdetgk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gexlqrujz.sHtML

[S21] C：字符类别判断
来源：http://m.share.yfazqb.com/Article/details/guhziqged.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.sjlbkw.cn/Article/details/ggumuzait.sHtML

[S22] C：字符串转数字
来源：http://3g.bbcook.cn/Article/details/ggaijlahu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.vehdjk.com/Article/details/gvovopara.sHtML

[S23] C：随机数
来源：http://read.share.bbcook.cn/Article/details/gsexhmpym.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fktsv.cn/Article/details/gqqojydag.sHtML

[S24] C：获取本地时间
来源：http://mobile.fktsv.cn/Article/details/gcatzkzhn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/grollhumv.sHtML

[S25] C：内存拷贝
来源：http://blog.vehdjk.com/Article/details/gjrtlddoy.sHtML

memcpy(dst, src, n);
来源：http://3g.fktsv.cn/Article/details/gwyxxjddm.sHtML

[S26] C：内存清零
来源：http://www.blog.sjlbkw.cn/Article/details/gmbgfrsyi.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.vehdjk.com/Article/details/glbbkjlfb.sHtML

[S27] C：定义常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gozzeqtqt.sHtML

const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gptnxltlf.sHtML

[S28] C：静态变量
来源：http://3g.tarul.cn/Article/details/gkueyecxz.sHtML

static int counter = 0;
来源：http://blog.fktsv.cn/Article/details/ggdjfrasa.sHtML

[S29] C：变参函数
来源：http://baike.bbcook.cn/Article/details/gsmbwfeui.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/glpcwyiqr.sHtML

[S30] C：头文件保护
来源：http://www.blog.bbcook.cn/Article/details/ghgujrljd.sHtML


<!-- 参考信息 -->