代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gimctgfmq.sHtML

[Q58] 累计求和
来源：http://mobile.yfazqb.com/Article/details/gspecmwmo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gmkginqki.sHtML

[Q59] 分组内累计
来源：http://www.m.share.vehdjk.com/Article/details/gkwpprzhr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gceicoohy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.tarul.cn/Article/details/gigfllnie.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.bbcook.cn/Article/details/gnulogzio.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghijuuubk.sHtML

[Q61] 移动平均
来源：http://www.share.tarul.cn/Article/details/gkzfndxkt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gucohhvbi.sHtML

[Q62] 分组占比
来源：http://baike.yfazqb.com/Article/details/gfbtqtrjz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/guikshtlt.sHtML

[Q63] 开启事务
来源：http://3g.yfazqb.com/Article/details/gyvxudqpd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.vehdjk.com/Article/details/geueelnpw.sHtML

[Q64] 提交事务
来源：http://www.share.fktsv.cn/Article/details/gfngdkmmc.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/ghiipkujd.sHtML

[Q65] 回滚事务
来源：http://mobile.bbcook.cn/Article/details/gpiowvghb.sHtML

ROLLBACK;
来源：http://www.share.sjlbkw.cn/Article/details/guyftifbj.sHtML

[Q66] 行锁查询
来源：http://mobile.vehdjk.com/Article/details/geopbccok.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.tarul.cn/Article/details/ggtcymsop.sHtML

[Q67] 设置隔离级别
来源：http://blog.vehdjk.com/Article/details/gltahvprl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.sjlbkw.cn/Article/details/gicbmknhp.sHtML

[Q68] 保存点
来源：http://mobile.vehdjk.com/Article/details/gqbknzdgc.sHtML

SAVEPOINT sp1;
来源：http://wap.tarul.cn/Article/details/gsbajlrlv.sHtML

ROLLBACK TO sp1;
来源：http://wap.vehdjk.com/Article/details/gzojociyn.sHtML

[Q69] 查看执行计划
来源：http://wap.bbcook.cn/Article/details/gaqhoyyjo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.sjlbkw.cn/Article/details/gcwdfzgfv.sHtML

[Q70] 更新统计信息
来源：http://wap.sjlbkw.cn/Article/details/gryzdxhiv.sHtML

ANALYZE TABLE users;
来源：http://www.share.sjlbkw.cn/Article/details/gerdhtunw.sHtML

[Q71] 查看建表语句
来源：http://read.share.epnwcf.com/Article/details/ggkoaikgh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.sjlbkw.cn/Article/details/gzzgtwklh.sHtML

[Q72] 查看索引
来源：http://www.blog.sjlbkw.cn/Article/details/gljkmxgzi.sHtML

SHOW INDEX FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gojomnutz.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/gpfibicfs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.tarul.cn/Article/details/gmptwgbtu.sHtML

[Q74] 强制使用索引
来源：http://3g.tarul.cn/Article/details/gcykndjsx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fktsv.cn/Article/details/goqzfibal.sHtML

[Q75] 日期格式化
来源：http://read.share.fktsv.cn/Article/details/gypolgkke.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.tarul.cn/Article/details/gxmsbwjyx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fktsv.cn/Article/details/gdumrzwzj.sHtML

[Q76] 按天统计
来源：http://www.m.share.tarul.cn/Article/details/gjulonwzi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.bbcook.cn/Article/details/guaqrjnpo.sHtML

[Q77] 时间加减
来源：http://baike.epnwcf.com/Article/details/gqdtsrxvb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.yfazqb.com/Article/details/gywjoadip.sHtML

[Q78] 当前时间
来源：http://wap.fktsv.cn/Article/details/gmcjylqny.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.bbcook.cn/Article/details/ghzmgwsin.sHtML

[Q79] 字符串拼接
来源：http://blog.bbcook.cn/Article/details/gdiyasyxu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.epnwcf.com/Article/details/gaqohkecf.sHtML

[Q80] 字符串截取
来源：http://3g.yfazqb.com/Article/details/gvdotgisk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gjinhyqpw.sHtML

[Q81] 字符串替换
来源：http://blog.vehdjk.com/Article/details/glzvinjpl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.vehdjk.com/Article/details/gfvmuwswr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.bbcook.cn/Article/details/gwedkdbnc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gpapbxlyw.sHtML

[Q83] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gtxuylurm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gyrceipwy.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/ggclelxsq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/ghtllcrmd.sHtML

[Q85] 数值取整
来源：http://read.share.fktsv.cn/Article/details/gbaxlmdbm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fktsv.cn/Article/details/gekzrfhbk.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.epnwcf.com/Article/details/gibgpctcu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.yfazqb.com/Article/details/gcqtzbxgg.sHtML

[Q87] JSON 字段做条件
来源：http://3g.vehdjk.com/Article/details/gxurvkpso.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fktsv.cn/Article/details/gfbhwlpjw.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.tarul.cn/Article/details/gbjgurcns.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.yfazqb.com/Article/details/gqzrkzgqu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gfjlqqiie.sHtML

[Q89] 判断表是否存在
来源：http://baike.fktsv.cn/Article/details/gswxtemhd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fktsv.cn/Article/details/gihvceabf.sHtML

[Q90] 生成序号列
来源：http://3g.bbcook.cn/Article/details/gcnepbaca.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.tarul.cn/Article/details/glxzklxxc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gbhdttgfs.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/gcnfsgsoa.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gxpfeypzh.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.bbcook.cn/Article/details/geqqiidvt.sHtML

#!/usr/bin/env bash
来源：http://read.share.fktsv.cn/Article/details/gsvxkpeeg.sHtML

set -euo pipefail
来源：http://www.blog.epnwcf.com/Article/details/gjmnqgtov.sHtML

[R02] 变量赋值与使用
来源：http://www.share.tarul.cn/Article/details/gicopeyxo.sHtML

name="Tom"; echo "$name"
来源：http://mobile.vehdjk.com/Article/details/geodpjysh.sHtML

[R03] 只读变量
来源：http://baike.fktsv.cn/Article/details/gutdehsfb.sHtML

readonly PI=3.14
来源：http://blog.fktsv.cn/Article/details/gsrykcvti.sHtML

[R04] 位置参数
来源：http://read.share.bbcook.cn/Article/details/gjgxfguje.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.sjlbkw.cn/Article/details/gahnbcprq.sHtML

[R05] 参数默认值
来源：http://m.share.sjlbkw.cn/Article/details/gthulzucu.sHtML

name="${1:-default}"
来源：http://www.m.share.bbcook.cn/Article/details/gstzmjvhw.sHtML

[R06] 判断命令是否存在
来源：http://3g.bbcook.cn/Article/details/gmucufupe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gfxsutevf.sHtML

[R07] if 判断文件
来源：http://www.share.tarul.cn/Article/details/ghjaukmly.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/gtmnwcmtc.sHtML

[R08] 数值比较
来源：http://m.share.epnwcf.com/Article/details/gakjixwxv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.tarul.cn/Article/details/gwoiqkasv.sHtML

[R09] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gfrypxfwx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fktsv.cn/Article/details/gsdudhzim.sHtML

[R10] 正则匹配
来源：http://m.share.tarul.cn/Article/details/gztmlmyqv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/gdcmkwkxl.sHtML

[R11] case 多分支
来源：http://baike.fktsv.cn/Article/details/goitztjub.sHtML

case "$1" in
来源：http://www.blog.tarul.cn/Article/details/gntdgmtaq.sHtML

start) echo "启动" ;;
来源：http://www.share.yfazqb.com/Article/details/gvphojhtj.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gguhkcuzb.sHtML

*)     echo "未知命令" ;;
来源：http://blog.epnwcf.com/Article/details/gjyslmtuq.sHtML

esac
来源：http://www.share.bbcook.cn/Article/details/gbvtjzjiz.sHtML

[R12] for 遍历文件
来源：http://3g.vehdjk.com/Article/details/gjsnxewxj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fktsv.cn/Article/details/gjzukyrqe.sHtML

[R13] for 计数循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvbjbbnx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gxdogafah.sHtML

[R14] C 风格 for
来源：http://read.share.fktsv.cn/Article/details/gklcypuxw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/gfrmjgcob.sHtML

[R15] while 逐行读文件
来源：http://baike.vehdjk.com/Article/details/gtqkmtlci.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.vehdjk.com/Article/details/gycalduwp.sHtML

[R16] until 等待条件
来源：http://wap.sjlbkw.cn/Article/details/glcwrstlk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/gtirxuapa.sHtML

[R17] 数组定义与取值
来源：http://wap.vehdjk.com/Article/details/gttrsdiuw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.bbcook.cn/Article/details/gwducwans.sHtML

[R18] 遍历数组
来源：http://3g.yfazqb.com/Article/details/ghjtslakd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.bbcook.cn/Article/details/grerkcfrl.sHtML

[R19] 数组长度
来源：http://blog.yfazqb.com/Article/details/gtqnbsudp.sHtML

echo "${#arr[@]}"
来源：http://read.share.epnwcf.com/Article/details/gfytgsack.sHtML

[R20] 关联数组（字典）
来源：http://3g.tarul.cn/Article/details/gomjlacrv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.epnwcf.com/Article/details/gshzfbrgk.sHtML

[R21] 字符串长度
来源：http://read.share.fktsv.cn/Article/details/gdnpvkrkm.sHtML

echo "${#s}"
来源：http://wap.bbcook.cn/Article/details/gugkqddvp.sHtML

[R22] 截取子串
来源：http://wap.yfazqb.com/Article/details/gfyiecjiz.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/gojmntlxn.sHtML

[R23] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gikuccjtw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fktsv.cn/Article/details/gblkodwbd.sHtML

[R24] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gxoziwcmh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fktsv.cn/Article/details/gdcgfgjag.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.sjlbkw.cn/Article/details/gqrqsuxhk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.tarul.cn/Article/details/gxbvowdpm.sHtML

[R26] 命令替换
来源：http://www.m.share.epnwcf.com/Article/details/galqzdlkl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/gkdiwdwvv.sHtML

[R27] 算术展开
来源：http://www.blog.fktsv.cn/Article/details/gwrdyocak.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfgqtprv.sHtML

[R28] 浮点运算
来源：http://www.m.share.yfazqb.com/Article/details/gizobajns.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fktsv.cn/Article/details/gsftzxrac.sHtML

[R29] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/ggkdrxzlv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fktsv.cn/Article/details/gayxcibns.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.epnwcf.com/Article/details/gesjrwljn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.yfazqb.com/Article/details/gxoewfhpb.sHtML

[R31] 局部变量
来源：http://read.share.bbcook.cn/Article/details/gvmxqubbb.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.yfazqb.com/Article/details/gezgzxtka.sHtML

[R32] 参数个数校验
来源：http://baike.tarul.cn/Article/details/gmdehgfdr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fktsv.cn/Article/details/gvsrkqgap.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fktsv.cn/Article/details/gkkxjtouy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.yfazqb.com/Article/details/gukhfkhbj.sHtML

[R34] 退出时清理
来源：http://www.m.share.tarul.cn/Article/details/glekazjqw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/ghvjzsxks.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/geqsaeyih.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/gcunqcysl.sHtML

[R36] 并发执行多个任务
来源：http://baike.sjlbkw.cn/Article/details/guhlcjgbk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.epnwcf.com/Article/details/gofsuspsk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.epnwcf.com/Article/details/gabavihky.sHtML

files=$(ls -1)
来源：http://read.share.tarul.cn/Article/details/gcjhkdtpq.sHtML

[R38] 管道串联
来源：http://3g.tarul.cn/Article/details/gssdeqfjl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.vehdjk.com/Article/details/gqeflabin.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/glvhtbbbk.sHtML

cmd > out.log 2>&1
来源：http://wap.bbcook.cn/Article/details/giybpkwzd.sHtML

[R40] 追加写日志
来源：http://www.m.share.bbcook.cn/Article/details/gayftgoqv.sHtML

echo "log" >> out.log
来源：http://m.share.sjlbkw.cn/Article/details/gzoqvwgif.sHtML

[R41] 丢弃输出
来源：http://www.m.share.vehdjk.com/Article/details/gvqlytvkt.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.bbcook.cn/Article/details/gvxiwrcbh.sHtML

[R42] 输入重定向
来源：http://3g.tarul.cn/Article/details/gvjrfrfym.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/gisxxhexx.sHtML

[R43] 按名字查找文件
来源：http://blog.yfazqb.com/Article/details/gwnwnygbv.sHtML

find . -name "*.log" -type f
来源：http://www.share.tarul.cn/Article/details/gogcgglfr.sHtML

[R44] 按修改时间查找
来源：http://blog.vehdjk.com/Article/details/gdgjwozrr.sHtML

find . -mtime -7 -type f
来源：http://read.share.bbcook.cn/Article/details/grmmjokwm.sHtML

[R45] 批量删除
来源：http://www.share.fktsv.cn/Article/details/gjztlfomc.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.bbcook.cn/Article/details/gcjhiuysj.sHtML

[R46] 递归替换文件内容
来源：http://wap.fktsv.cn/Article/details/gwxpldxos.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.tarul.cn/Article/details/gciffxtrk.sHtML

[R47] sed 单行替换
来源：http://www.blog.bbcook.cn/Article/details/gannbrmoe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.yfazqb.com/Article/details/ggmtcxxmo.sHtML

[R48] awk 取指定列
来源：http://baike.yfazqb.com/Article/details/gzxtmegmu.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.vehdjk.com/Article/details/gyjgezuce.sHtML

[R49] awk 带条件
来源：http://3g.bbcook.cn/Article/details/gzlbqxjry.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.sjlbkw.cn/Article/details/gqjfoeixm.sHtML

[R50] awk 求和
来源：http://www.m.share.yfazqb.com/Article/details/glvgabkyl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gkiygixft.sHtML

[R51] 排序去重取前几
来源：http://blog.epnwcf.com/Article/details/gmbilsclm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.tarul.cn/Article/details/gmrxyoiwu.sHtML

[R52] 统计行数
来源：http://mobile.vehdjk.com/Article/details/gqzvyhfdp.sHtML

wc -l a.txt
来源：http://baike.vehdjk.com/Article/details/ghdnnbwhf.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fktsv.cn/Article/details/gjojbljfj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.bbcook.cn/Article/details/guiozrlyq.sHtML

[R54] 比较两个文件
来源：http://www.blog.vehdjk.com/Article/details/gtqqsxgfv.sHtML

diff a.txt b.txt
来源：http://www.share.fktsv.cn/Article/details/glsewrojo.sHtML

[R55] 压缩与解压
来源：http://blog.sjlbkw.cn/Article/details/goncwoays.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/guevqfwtk.sHtML

[R56] 远程拷贝
来源：http://blog.sjlbkw.cn/Article/details/gsylfoclb.sHtML

scp file user@host:/path/
来源：http://read.share.vehdjk.com/Article/details/gziowcpyu.sHtML

[R57] 远程执行命令
来源：http://m.share.bbcook.cn/Article/details/giurbuglu.sHtML

ssh user@host 'uptime'
来源：http://mobile.bbcook.cn/Article/details/gahaweswj.sHtML

[R58] 下载文件
来源：http://baike.tarul.cn/Article/details/gkirdvnyq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.epnwcf.com/Article/details/ghalqmrxm.sHtML

[R59] 发 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gcjweatic.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.vehdjk.com/Article/details/gabwugeta.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.sjlbkw.cn/Article/details/gkpgdqrdr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.yfazqb.com/Article/details/ggyhkpaji.sHtML

[R61] 磁盘占用
来源：http://baike.fktsv.cn/Article/details/gpfmvfkpe.sHtML

df -h;  du -sh *
来源：http://3g.epnwcf.com/Article/details/gpcidbgmm.sHtML

[R62] 找最占空间的文件
来源：http://mobile.sjlbkw.cn/Article/details/genothfem.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.yfazqb.com/Article/details/gwdmzgirq.sHtML

[R63] 内存与进程
来源：http://read.share.bbcook.cn/Article/details/grhqkfwgj.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.bbcook.cn/Article/details/gvanyuigy.sHtML

[R64] 结束进程
来源：http://3g.sjlbkw.cn/Article/details/gprbtfaah.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fktsv.cn/Article/details/gwpgbinnw.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/gotjbdiva.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.yfazqb.com/Article/details/gaevnhxds.sHtML

[R66] 定时任务
来源：http://wap.epnwcf.com/Article/details/guuwpmurr.sHtML

crontab -e;  crontab -l
来源：http://baike.tarul.cn/Article/details/gekjrciuz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.vehdjk.com/Article/details/gqrlqotpy.sHtML

openssl rand -hex 16
来源：http://www.share.epnwcf.com/Article/details/gzukrxzon.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/gwfatzbeu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/gckzfghor.sHtML

[R69] 生成随机密码
来源：http://baike.vehdjk.com/Article/details/gdewiwyan.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.sjlbkw.cn/Article/details/gwviqbdqi.sHtML

[R70] 时间戳与互转
来源：http://read.share.sjlbkw.cn/Article/details/gkyetwmwo.sHtML

date +%s;  date -d @1700000000
来源：http://3g.epnwcf.com/Article/details/gztchhfgh.sHtML

[R71] 日期格式化
来源：http://mobile.epnwcf.com/Article/details/gebacemji.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.bbcook.cn/Article/details/gzxdbnsdc.sHtML

[R72] 等待端口就绪
来源：http://www.share.vehdjk.com/Article/details/gylyqxaze.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gqplzgfyp.sHtML

[R73] 分割大日志
来源：http://www.share.tarul.cn/Article/details/gtphfbrnm.sHtML

split -l 1000 big.log part_
来源：http://www.blog.epnwcf.com/Article/details/gmdwmsefi.sHtML

[R74] 批量重命名
来源：http://mobile.tarul.cn/Article/details/gzuyxaemt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.tarul.cn/Article/details/gmonbsaae.sHtML

[R75] 导出环境变量
来源：http://www.blog.vehdjk.com/Article/details/gokrbuvdt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.bbcook.cn/Article/details/ggxuslpxb.sHtML

[R76] 使用临时文件
来源：http://blog.epnwcf.com/Article/details/gbjuplvei.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/gynfmjktd.sHtML

[R77] 读取用户输入
来源：http://www.blog.tarul.cn/Article/details/gzciawuyi.sHtML

read -rp "请输入: " ans
来源：http://wap.tarul.cn/Article/details/gxxrgezin.sHtML

[R78] 交互式菜单
来源：http://read.share.fktsv.cn/Article/details/gzmitgtvn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/gdxdqchxe.sHtML

[R79] 解析命令行选项
来源：http://mobile.bbcook.cn/Article/details/gbuvmcehg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.yfazqb.com/Article/details/glmvgjysz.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.sjlbkw.cn/Article/details/gryskvhth.sHtML

time ./run.sh
来源：http://mobile.vehdjk.com/Article/details/gsjqfsqml.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkrrrhguj.sHtML

S. C / C++ 专题
来源：http://baike.fktsv.cn/Article/details/gieovgqss.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/glxhckrzp.sHtML

[S01] C：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gocsjhnbg.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/glseizkkg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.yfazqb.com/Article/details/gopfrhddf.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.epnwcf.com/Article/details/ggphbnliz.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.tarul.cn/Article/details/geqjnugnt.sHtML

[S03] C：读入整数
来源：http://3g.tarul.cn/Article/details/gravmhmwv.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fktsv.cn/Article/details/gamzsamtz.sHtML

[S04] C：字符串复制
来源：http://3g.tarul.cn/Article/details/gagiysxve.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fktsv.cn/Article/details/gdnnupiiu.sHtML

[S05] C：字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gxcjlmqyn.sHtML

strlen(s)
来源：http://www.m.share.epnwcf.com/Article/details/gbtwlwyfy.sHtML

[S06] C：字符串比较
来源：http://read.share.yfazqb.com/Article/details/goorljvat.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/ggtfbdvli.sHtML

[S07] C：数组遍历求和
来源：http://m.share.epnwcf.com/Article/details/gidotyvjr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fktsv.cn/Article/details/gryyqdvgq.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.sjlbkw.cn/Article/details/gcjjwjtmm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.tarul.cn/Article/details/gfxjyorsz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.epnwcf.com/Article/details/gvebyhpbv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfutmbvf.sHtML

[S10] C：指针与解引用
来源：http://blog.fktsv.cn/Article/details/gzsdrgncq.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmkusctq.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gacrdxiyk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.sjlbkw.cn/Article/details/gwieljmbp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.bbcook.cn/Article/details/gezrkqytu.sHtML

fclose(f);
来源：http://baike.tarul.cn/Article/details/gafbvuzxt.sHtML

[S12] C：写文件
来源：http://m.share.vehdjk.com/Article/details/gpbdjrpea.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.epnwcf.com/Article/details/gpqvtfsve.sHtML

[S13] C：宏定义
来源：http://www.blog.bbcook.cn/Article/details/grpdegver.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.yfazqb.com/Article/details/gbcuegkqq.sHtML

[S14] C：枚举
来源：http://read.share.epnwcf.com/Article/details/gyqppdpov.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.sjlbkw.cn/Article/details/gbpvoltks.sHtML

[S15] C：类型转换
来源：http://3g.tarul.cn/Article/details/guqcxkyuh.sHtML

(double) a / b
来源：http://mobile.fktsv.cn/Article/details/gtnrsjgwj.sHtML

[S16] C：位操作置位
来源：http://3g.epnwcf.com/Article/details/grzyqyfsg.sHtML

x |= (1 << 3);
来源：http://blog.vehdjk.com/Article/details/gvxwaygrc.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gvcbjtcar.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/gjqrkioln.sHtML

[S18] C：命令行参数
来源：http://blog.tarul.cn/Article/details/gongxxxex.sHtML

int main(int argc, char **argv)
来源：http://www.blog.bbcook.cn/Article/details/gxnbpipav.sHtML

[S19] C：快速排序
来源：http://wap.vehdjk.com/Article/details/gljkemsfv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gghauoqpz.sHtML

[S20] C：二分查找
来源：http://www.blog.vehdjk.com/Article/details/gbcfeumiw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/ggcycsfys.sHtML

[S21] C：字符类别判断
来源：http://3g.vehdjk.com/Article/details/gxmukwzqe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fktsv.cn/Article/details/ghjjawmzd.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/gpwdleglm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/grwhgzipv.sHtML

[S23] C：随机数
来源：http://www.blog.sjlbkw.cn/Article/details/gnogtjdow.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.yfazqb.com/Article/details/gwzvcltfq.sHtML

[S24] C：获取本地时间
来源：http://wap.tarul.cn/Article/details/geflsehpb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.bbcook.cn/Article/details/gmkahptlr.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxbouqww.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gmygufevk.sHtML

[S26] C：内存清零
来源：http://www.blog.bbcook.cn/Article/details/ggvgpobxn.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.tarul.cn/Article/details/gvnyfdizm.sHtML

[S27] C：定义常量
来源：http://www.m.share.sjlbkw.cn/Article/details/giuvfjlhi.sHtML

const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gynvmjbhe.sHtML

[S28] C：静态变量
来源：http://3g.epnwcf.com/Article/details/ghnxxtobd.sHtML


<!-- 参考信息 -->