代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fktsv.cn/Article/details/gjacycqve.sHtML

[Q58] 累计求和
来源：http://blog.epnwcf.com/Article/details/gqlhdwszv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.yfazqb.com/Article/details/gcqdtwbjo.sHtML

[Q59] 分组内累计
来源：http://www.share.yfazqb.com/Article/details/gnxusidbz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gkoqnbpwc.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.tarul.cn/Article/details/gyrojbpdv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.vehdjk.com/Article/details/gbqhqjwbn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.tarul.cn/Article/details/gtsgeporg.sHtML

[Q61] 移动平均
来源：http://read.share.epnwcf.com/Article/details/gwtvflyip.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/guqmfufyr.sHtML

[Q62] 分组占比
来源：http://wap.vehdjk.com/Article/details/gegotfyin.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gfwflwpny.sHtML

[Q63] 开启事务
来源：http://www.m.share.yfazqb.com/Article/details/gnknkgavx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.vehdjk.com/Article/details/gvvplvnny.sHtML

[Q64] 提交事务
来源：http://www.share.sjlbkw.cn/Article/details/gwesgbwsj.sHtML

COMMIT;
来源：http://www.m.share.yfazqb.com/Article/details/geiguxdjz.sHtML

[Q65] 回滚事务
来源：http://read.share.tarul.cn/Article/details/gugaaslpc.sHtML

ROLLBACK;
来源：http://m.share.epnwcf.com/Article/details/gipdbhgsg.sHtML

[Q66] 行锁查询
来源：http://m.share.vehdjk.com/Article/details/geydvdkgj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.yfazqb.com/Article/details/ghabshvhj.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.epnwcf.com/Article/details/gltiueqew.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.vehdjk.com/Article/details/giyxitfmi.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/gwzlcgcki.sHtML

SAVEPOINT sp1;
来源：http://blog.epnwcf.com/Article/details/gcxzqirkd.sHtML

ROLLBACK TO sp1;
来源：http://blog.yfazqb.com/Article/details/gcpwqfrvi.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.yfazqb.com/Article/details/gzzzrwpct.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.vehdjk.com/Article/details/ghdbulege.sHtML

[Q70] 更新统计信息
来源：http://wap.epnwcf.com/Article/details/gncjwyhqi.sHtML

ANALYZE TABLE users;
来源：http://www.blog.tarul.cn/Article/details/gdxarlxxi.sHtML

[Q71] 查看建表语句
来源：http://read.share.bbcook.cn/Article/details/gopwhljin.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.tarul.cn/Article/details/giytdzslv.sHtML

[Q72] 查看索引
来源：http://3g.fktsv.cn/Article/details/gjwwzlzmo.sHtML

SHOW INDEX FROM users;
来源：http://baike.fktsv.cn/Article/details/gnxuukmqt.sHtML

[Q73] 查看表状态
来源：http://blog.yfazqb.com/Article/details/giqsoesbo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.sjlbkw.cn/Article/details/gzqtxrqjw.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/gghsaggsx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.epnwcf.com/Article/details/gxdogxner.sHtML

[Q75] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gkzgljroz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.epnwcf.com/Article/details/ghbywxycr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fktsv.cn/Article/details/gwyomgsli.sHtML

[Q76] 按天统计
来源：http://baike.bbcook.cn/Article/details/gvsozlsnm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.vehdjk.com/Article/details/gjnusizku.sHtML

[Q77] 时间加减
来源：http://3g.bbcook.cn/Article/details/gewcgeoqt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.sjlbkw.cn/Article/details/gqitqalcv.sHtML

[Q78] 当前时间
来源：http://baike.yfazqb.com/Article/details/gjuercyln.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.vehdjk.com/Article/details/gnfbpmehp.sHtML

[Q79] 字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gesnwyqid.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.tarul.cn/Article/details/gwwxagxks.sHtML

[Q80] 字符串截取
来源：http://read.share.epnwcf.com/Article/details/gwrrchzod.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.yfazqb.com/Article/details/glxryfgzs.sHtML

[Q81] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gkidzkeaa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/gookxkazt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.sjlbkw.cn/Article/details/goguzikrd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/grvebghjc.sHtML

[Q83] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gndbohiep.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/goabmuyzj.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gcfgjhvgo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gvmcvgpot.sHtML

[Q85] 数值取整
来源：http://3g.bbcook.cn/Article/details/gsgbyyysz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.yfazqb.com/Article/details/grylpisan.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.vehdjk.com/Article/details/ggfoceywp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fktsv.cn/Article/details/gmumvxxqi.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.sjlbkw.cn/Article/details/gbzevkzup.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.vehdjk.com/Article/details/gsrmqwtwm.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fktsv.cn/Article/details/gyzralubo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.sjlbkw.cn/Article/details/gvekhgnus.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.bbcook.cn/Article/details/gpfibnlie.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gxquimtkl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.sjlbkw.cn/Article/details/gegfancgt.sHtML

[Q90] 生成序号列
来源：http://read.share.epnwcf.com/Article/details/ggfdhlerr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.yfazqb.com/Article/details/grunmsdxx.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtqrysflh.sHtML

R. Bash 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvbyqwkl.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gtrccdveg.sHtML

[R01] shebang 与严格模式
来源：http://baike.bbcook.cn/Article/details/ghuzhaqyq.sHtML

#!/usr/bin/env bash
来源：http://www.share.bbcook.cn/Article/details/gsxpvghnt.sHtML

set -euo pipefail
来源：http://www.share.tarul.cn/Article/details/gkwwusouq.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/ggkbjywme.sHtML

name="Tom"; echo "$name"
来源：http://read.share.epnwcf.com/Article/details/gjmongxid.sHtML

[R03] 只读变量
来源：http://m.share.yfazqb.com/Article/details/gsymnhpii.sHtML

readonly PI=3.14
来源：http://blog.sjlbkw.cn/Article/details/gdyzkobba.sHtML

[R04] 位置参数
来源：http://www.share.yfazqb.com/Article/details/gcjfrmret.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/gllndgwqz.sHtML

[R05] 参数默认值
来源：http://3g.bbcook.cn/Article/details/gurgdyyid.sHtML

name="${1:-default}"
来源：http://blog.fktsv.cn/Article/details/gmqjsaiel.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gldjfleor.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gyotqofsp.sHtML

[R07] if 判断文件
来源：http://blog.bbcook.cn/Article/details/gpbbzrjzr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gsjjybohw.sHtML

[R08] 数值比较
来源：http://mobile.vehdjk.com/Article/details/gqrgvprvc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.tarul.cn/Article/details/glvpffizz.sHtML

[R09] 字符串比较
来源：http://wap.epnwcf.com/Article/details/gjplxhojr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.epnwcf.com/Article/details/gzfyjzayh.sHtML

[R10] 正则匹配
来源：http://m.share.vehdjk.com/Article/details/gzqwrbovy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.epnwcf.com/Article/details/grzlpsxua.sHtML

[R11] case 多分支
来源：http://blog.yfazqb.com/Article/details/gdrheefuh.sHtML

case "$1" in
来源：http://baike.fktsv.cn/Article/details/goiyrurcn.sHtML

start) echo "启动" ;;
来源：http://mobile.epnwcf.com/Article/details/gscuezabz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gzhwgvkff.sHtML

*)     echo "未知命令" ;;
来源：http://3g.vehdjk.com/Article/details/gtnsogzsy.sHtML

esac
来源：http://www.share.fktsv.cn/Article/details/gjifggiov.sHtML

[R12] for 遍历文件
来源：http://read.share.yfazqb.com/Article/details/gnxvzrugr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.yfazqb.com/Article/details/gueglizey.sHtML

[R13] for 计数循环
来源：http://wap.fktsv.cn/Article/details/gwelbtjmq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gtoypemlj.sHtML

[R14] C 风格 for
来源：http://read.share.fktsv.cn/Article/details/gcibpufat.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gurxpnejp.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/gsxjowhax.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.vehdjk.com/Article/details/gdrwlrgsa.sHtML

[R16] until 等待条件
来源：http://baike.epnwcf.com/Article/details/gmicpmqlp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gcozpzrfg.sHtML

[R17] 数组定义与取值
来源：http://baike.vehdjk.com/Article/details/gsxriyibm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.bbcook.cn/Article/details/gsxfdvowi.sHtML

[R18] 遍历数组
来源：http://mobile.epnwcf.com/Article/details/ggoxxmeuz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.epnwcf.com/Article/details/gqsmejjcf.sHtML

[R19] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gosadpmtd.sHtML

echo "${#arr[@]}"
来源：http://www.blog.tarul.cn/Article/details/gfdmdxsbc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.vehdjk.com/Article/details/ggjgfhdcy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fktsv.cn/Article/details/gfvuahrgg.sHtML

[R21] 字符串长度
来源：http://www.share.vehdjk.com/Article/details/gmprjmfxw.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gazcjyryf.sHtML

[R22] 截取子串
来源：http://m.share.tarul.cn/Article/details/gbpvfnzxc.sHtML

echo "${s:0:5}"
来源：http://m.share.tarul.cn/Article/details/gfnbyzyjo.sHtML

[R23] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gqyynnqvb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fktsv.cn/Article/details/gajsjejoz.sHtML

[R24] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/gfsjftudg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.sjlbkw.cn/Article/details/gbjndjmie.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.vehdjk.com/Article/details/gxehqdcgh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.yfazqb.com/Article/details/gtzkuudva.sHtML

[R26] 命令替换
来源：http://m.share.sjlbkw.cn/Article/details/glkfyelby.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.bbcook.cn/Article/details/ghlxmoodo.sHtML

[R27] 算术展开
来源：http://www.blog.vehdjk.com/Article/details/gejcviknq.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.vehdjk.com/Article/details/gqihlcqhd.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/ggsycjnmr.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/ghiazbuem.sHtML

[R29] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/gcbphyskt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.epnwcf.com/Article/details/gxiczyuua.sHtML

[R30] 函数返回状态码
来源：http://mobile.sjlbkw.cn/Article/details/grqrogxfy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fktsv.cn/Article/details/gtogqshgy.sHtML

[R31] 局部变量
来源：http://baike.yfazqb.com/Article/details/ghtqvxzqz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/gavvzhqmt.sHtML

[R32] 参数个数校验
来源：http://www.m.share.tarul.cn/Article/details/gsisvscrz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/giauiaqba.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.vehdjk.com/Article/details/gtczlvims.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.vehdjk.com/Article/details/gnmunpfzn.sHtML

[R34] 退出时清理
来源：http://www.share.vehdjk.com/Article/details/gkowgsuby.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/ggcnvfjwj.sHtML

[R35] 后台执行并等待
来源：http://3g.tarul.cn/Article/details/gzlbmasbn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.epnwcf.com/Article/details/gpehsotez.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.epnwcf.com/Article/details/ggwnpyakc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.bbcook.cn/Article/details/glkqrrwhv.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.tarul.cn/Article/details/gqkqcjoxv.sHtML

files=$(ls -1)
来源：http://blog.sjlbkw.cn/Article/details/gfyhmowxp.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/grscefwyj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.bbcook.cn/Article/details/gvjdpsvmo.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.tarul.cn/Article/details/gvozgpxcb.sHtML

cmd > out.log 2>&1
来源：http://baike.vehdjk.com/Article/details/gemvejxgx.sHtML

[R40] 追加写日志
来源：http://www.blog.bbcook.cn/Article/details/gqlyvafsy.sHtML

echo "log" >> out.log
来源：http://wap.epnwcf.com/Article/details/gdiamvqun.sHtML

[R41] 丢弃输出
来源：http://www.share.epnwcf.com/Article/details/ggtwquyda.sHtML

cmd >/dev/null 2>&1
来源：http://blog.yfazqb.com/Article/details/gyocwbtpr.sHtML

[R42] 输入重定向
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrrdfkkc.sHtML

wc -l < a.txt
来源：http://read.share.yfazqb.com/Article/details/gwdzdboqx.sHtML

[R43] 按名字查找文件
来源：http://baike.fktsv.cn/Article/details/gkgqllnml.sHtML

find . -name "*.log" -type f
来源：http://3g.fktsv.cn/Article/details/ggsbnppzi.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.yfazqb.com/Article/details/gurorrrzv.sHtML

find . -mtime -7 -type f
来源：http://mobile.bbcook.cn/Article/details/gqatlvagg.sHtML

[R45] 批量删除
来源：http://baike.tarul.cn/Article/details/gmcxkzwrt.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/ggfggffys.sHtML

[R46] 递归替换文件内容
来源：http://read.share.sjlbkw.cn/Article/details/gkdsbhryd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.sjlbkw.cn/Article/details/giyawahjw.sHtML

[R47] sed 单行替换
来源：http://wap.sjlbkw.cn/Article/details/gbdqrnnws.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fktsv.cn/Article/details/gcbudncsp.sHtML

[R48] awk 取指定列
来源：http://www.blog.vehdjk.com/Article/details/gsnhhzgem.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gxoasdzrh.sHtML

[R49] awk 带条件
来源：http://www.share.fktsv.cn/Article/details/gydtyfcrr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.sjlbkw.cn/Article/details/gbampkadz.sHtML

[R50] awk 求和
来源：http://wap.vehdjk.com/Article/details/grcnpvywh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.tarul.cn/Article/details/gnoqgozwm.sHtML

[R51] 排序去重取前几
来源：http://wap.epnwcf.com/Article/details/goxvldwlp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.bbcook.cn/Article/details/giqzyicpe.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/gtpunnzzh.sHtML

wc -l a.txt
来源：http://www.share.epnwcf.com/Article/details/gihqbpilx.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.tarul.cn/Article/details/gckvbpesg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.yfazqb.com/Article/details/gxmmwxgvp.sHtML

[R54] 比较两个文件
来源：http://www.m.share.bbcook.cn/Article/details/gyasndkrh.sHtML

diff a.txt b.txt
来源：http://m.share.bbcook.cn/Article/details/gklqpxhuw.sHtML

[R55] 压缩与解压
来源：http://3g.sjlbkw.cn/Article/details/gsqawfekh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.tarul.cn/Article/details/gvrwwhezz.sHtML

[R56] 远程拷贝
来源：http://m.share.vehdjk.com/Article/details/gxyybvify.sHtML

scp file user@host:/path/
来源：http://mobile.sjlbkw.cn/Article/details/gwuiukhli.sHtML

[R57] 远程执行命令
来源：http://read.share.yfazqb.com/Article/details/gjfmwafgg.sHtML

ssh user@host 'uptime'
来源：http://mobile.fktsv.cn/Article/details/gxfoakqbh.sHtML

[R58] 下载文件
来源：http://wap.tarul.cn/Article/details/gokzpioee.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.vehdjk.com/Article/details/ghvcjpuyv.sHtML

[R59] 发 POST JSON
来源：http://baike.yfazqb.com/Article/details/gbuenopwz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.sjlbkw.cn/Article/details/gjltrdmvq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/gditndbqz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.sjlbkw.cn/Article/details/gtkjiwrmm.sHtML

[R61] 磁盘占用
来源：http://www.share.bbcook.cn/Article/details/gbmerqcsa.sHtML

df -h;  du -sh *
来源：http://mobile.epnwcf.com/Article/details/gmrrndvpm.sHtML

[R62] 找最占空间的文件
来源：http://read.share.tarul.cn/Article/details/gvndxirbc.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fktsv.cn/Article/details/grndxddee.sHtML

[R63] 内存与进程
来源：http://www.m.share.fktsv.cn/Article/details/gxksikhyi.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.epnwcf.com/Article/details/gufcgnzxb.sHtML

[R64] 结束进程
来源：http://mobile.bbcook.cn/Article/details/gzbuxrfwc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/gradetwth.sHtML

[R65] 查看端口占用
来源：http://mobile.epnwcf.com/Article/details/gfggsfwwr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.sjlbkw.cn/Article/details/grayhlnlp.sHtML

[R66] 定时任务
来源：http://baike.yfazqb.com/Article/details/gzigmubjj.sHtML

crontab -e;  crontab -l
来源：http://mobile.vehdjk.com/Article/details/gmdirgiqa.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.vehdjk.com/Article/details/gacsxqwlc.sHtML

openssl rand -hex 16
来源：http://read.share.tarul.cn/Article/details/gjtgbibel.sHtML

[R68] 计算文件校验值
来源：http://baike.tarul.cn/Article/details/gvsjgkxoi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.tarul.cn/Article/details/goccznaln.sHtML

[R69] 生成随机密码
来源：http://read.share.fktsv.cn/Article/details/gajflaoic.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fktsv.cn/Article/details/gcmrnzine.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjygkqiv.sHtML

date +%s;  date -d @1700000000
来源：http://blog.tarul.cn/Article/details/gwabmzmrz.sHtML

[R71] 日期格式化
来源：http://read.share.fktsv.cn/Article/details/gomhzprld.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.epnwcf.com/Article/details/ghnksfsxc.sHtML

[R72] 等待端口就绪
来源：http://www.share.yfazqb.com/Article/details/gjbstwnnf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gomycmjvf.sHtML

[R73] 分割大日志
来源：http://www.share.vehdjk.com/Article/details/gjzzllziq.sHtML

split -l 1000 big.log part_
来源：http://blog.tarul.cn/Article/details/gouaivhbi.sHtML

[R74] 批量重命名
来源：http://blog.bbcook.cn/Article/details/gyqzwxrxl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gjtllahpd.sHtML

[R75] 导出环境变量
来源：http://wap.sjlbkw.cn/Article/details/giodlltjf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.bbcook.cn/Article/details/gvwzwomwu.sHtML

[R76] 使用临时文件
来源：http://3g.bbcook.cn/Article/details/gbaahbmrg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gqtswqyem.sHtML

[R77] 读取用户输入
来源：http://www.share.epnwcf.com/Article/details/gnxtvyjqr.sHtML

read -rp "请输入: " ans
来源：http://blog.tarul.cn/Article/details/gbqwteyvl.sHtML

[R78] 交互式菜单
来源：http://3g.fktsv.cn/Article/details/gzbnydcts.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.vehdjk.com/Article/details/gooltitdi.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fktsv.cn/Article/details/grrxdhegm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/gitwwnqed.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.vehdjk.com/Article/details/gpicedgyw.sHtML

time ./run.sh
来源：http://read.share.yfazqb.com/Article/details/geynkfxuv.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gzssjydmj.sHtML

S. C / C++ 专题
来源：http://blog.tarul.cn/Article/details/gidrmayvd.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gemdsezdr.sHtML

[S01] C：Hello World
来源：http://3g.yfazqb.com/Article/details/gltilgjai.sHtML

#include <stdio.h>
来源：http://wap.bbcook.cn/Article/details/gzhnwkcki.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.yfazqb.com/Article/details/gsvjgmjjw.sHtML

[S02] C：变量与格式化输出
来源：http://wap.tarul.cn/Article/details/gmhavsclq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.bbcook.cn/Article/details/gofyrvxon.sHtML

[S03] C：读入整数
来源：http://www.m.share.vehdjk.com/Article/details/gjbpolokh.sHtML

int x; scanf("%d", &x);
来源：http://read.share.sjlbkw.cn/Article/details/gyxggkqub.sHtML

[S04] C：字符串复制
来源：http://wap.bbcook.cn/Article/details/gtgxicmhx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fktsv.cn/Article/details/gokyvjanl.sHtML

[S05] C：字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gndduaylp.sHtML

strlen(s)
来源：http://www.m.share.fktsv.cn/Article/details/gcqjjqrjt.sHtML

[S06] C：字符串比较
来源：http://blog.epnwcf.com/Article/details/gvgsxyomb.sHtML

strcmp(a, b) == 0
来源：http://read.share.bbcook.cn/Article/details/gneedwqbs.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fktsv.cn/Article/details/govtlrkay.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.tarul.cn/Article/details/gcwoinrdo.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.yfazqb.com/Article/details/guwkfvtsq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.sjlbkw.cn/Article/details/gtursxykn.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.vehdjk.com/Article/details/gfvbcgpyt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gzsyuepio.sHtML

[S10] C：指针与解引用
来源：http://mobile.fktsv.cn/Article/details/gghjnixap.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.tarul.cn/Article/details/gueiszpeh.sHtML

[S11] C：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gzeuhthol.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.epnwcf.com/Article/details/grucylzro.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.epnwcf.com/Article/details/gccrleela.sHtML

fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdzepael.sHtML

[S12] C：写文件
来源：http://m.share.tarul.cn/Article/details/gxfegpqnx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.tarul.cn/Article/details/gammtjook.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/galnvdfoe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/gppufgxcr.sHtML

[S14] C：枚举
来源：http://m.share.yfazqb.com/Article/details/gejhxaxeu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.tarul.cn/Article/details/gkxikdqju.sHtML

[S15] C：类型转换
来源：http://baike.vehdjk.com/Article/details/glmljvwle.sHtML

(double) a / b
来源：http://blog.bbcook.cn/Article/details/gvvkiwjtq.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/gkaneukiy.sHtML

x |= (1 << 3);
来源：http://blog.bbcook.cn/Article/details/geoxwgbxr.sHtML

[S17] C：安全拼接字符串
来源：http://baike.epnwcf.com/Article/details/gwetlairm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/genyoqdkz.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gerpqcioc.sHtML

int main(int argc, char **argv)
来源：http://m.share.fktsv.cn/Article/details/grqdujjpp.sHtML

[S19] C：快速排序
来源：http://www.blog.tarul.cn/Article/details/gdnjahndz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/giomnqsrz.sHtML

[S20] C：二分查找
来源：http://www.blog.epnwcf.com/Article/details/gegonwaio.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcftwuovw.sHtML

[S21] C：字符类别判断
来源：http://wap.vehdjk.com/Article/details/gdczfpxfm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.yfazqb.com/Article/details/gfzvugobx.sHtML

[S22] C：字符串转数字
来源：http://www.blog.sjlbkw.cn/Article/details/gkzkpbxtv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/gfwhhbbdx.sHtML

[S23] C：随机数
来源：http://www.blog.tarul.cn/Article/details/gjfvgjdyr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.epnwcf.com/Article/details/guehxxbhp.sHtML

[S24] C：获取本地时间
来源：http://read.share.vehdjk.com/Article/details/gmqkzcqor.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.bbcook.cn/Article/details/grfcsxxoy.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gohgpcrzr.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gearqzonv.sHtML

[S26] C：内存清零
来源：http://www.blog.bbcook.cn/Article/details/gljdectub.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/gwxwwhieb.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/gzdlnrfgo.sHtML

const double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gagyaviiz.sHtML

[S28] C：静态变量
来源：http://m.share.bbcook.cn/Article/details/guemrumct.sHtML


<!-- 参考信息 -->