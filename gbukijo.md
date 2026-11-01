代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.tarul.cn/Article/details/galrleoyv.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/gxhlixlni.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.tarul.cn/Article/details/gitpjljev.sHtML

[Q59] 分组内累计
来源：http://blog.fktsv.cn/Article/details/gchxevlbt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gjehdaoni.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fktsv.cn/Article/details/gllqgjixu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.vehdjk.com/Article/details/gtwxgtlhh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gsajkqxrm.sHtML

[Q61] 移动平均
来源：http://blog.bbcook.cn/Article/details/gkcwgmtxq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gipixqlpk.sHtML

[Q62] 分组占比
来源：http://m.share.sjlbkw.cn/Article/details/gxfoooirb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gigjuyhel.sHtML

[Q63] 开启事务
来源：http://www.share.yfazqb.com/Article/details/gklnbucxr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.vehdjk.com/Article/details/gbuwomgst.sHtML

[Q64] 提交事务
来源：http://www.share.vehdjk.com/Article/details/gkwzxownn.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gftvcckcq.sHtML

[Q65] 回滚事务
来源：http://baike.vehdjk.com/Article/details/gfmyltrca.sHtML

ROLLBACK;
来源：http://blog.sjlbkw.cn/Article/details/gznmtplws.sHtML

[Q66] 行锁查询
来源：http://read.share.tarul.cn/Article/details/gyklgwhqs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.yfazqb.com/Article/details/gwxitngci.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fktsv.cn/Article/details/gllkvxtab.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.bbcook.cn/Article/details/gwthkbdui.sHtML

[Q68] 保存点
来源：http://3g.fktsv.cn/Article/details/gcjrcrhsc.sHtML

SAVEPOINT sp1;
来源：http://blog.sjlbkw.cn/Article/details/grusvlabg.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fktsv.cn/Article/details/gzrnfmmfs.sHtML

[Q69] 查看执行计划
来源：http://m.share.epnwcf.com/Article/details/glcknuflw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.epnwcf.com/Article/details/gcmqvrrzv.sHtML

[Q70] 更新统计信息
来源：http://read.share.epnwcf.com/Article/details/glvgpcuyh.sHtML

ANALYZE TABLE users;
来源：http://m.share.fktsv.cn/Article/details/gfguaexpk.sHtML

[Q71] 查看建表语句
来源：http://blog.bbcook.cn/Article/details/gyznjduci.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.yfazqb.com/Article/details/ghpcjkodt.sHtML

[Q72] 查看索引
来源：http://www.share.fktsv.cn/Article/details/gkfxrcubc.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.tarul.cn/Article/details/gxlscnbha.sHtML

[Q73] 查看表状态
来源：http://3g.tarul.cn/Article/details/gacxcenhy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.epnwcf.com/Article/details/gixllqbcg.sHtML

[Q74] 强制使用索引
来源：http://3g.bbcook.cn/Article/details/gkwkcstcy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.sjlbkw.cn/Article/details/gbatsoxec.sHtML

[Q75] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gmjuehnjz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/grepqwftj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.bbcook.cn/Article/details/gvqrqsule.sHtML

[Q76] 按天统计
来源：http://blog.yfazqb.com/Article/details/grzzgldob.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.yfazqb.com/Article/details/guyksezup.sHtML

[Q77] 时间加减
来源：http://wap.sjlbkw.cn/Article/details/gtcpihkht.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.vehdjk.com/Article/details/ggiqbwsnw.sHtML

[Q78] 当前时间
来源：http://mobile.sjlbkw.cn/Article/details/gtsozxwzk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.sjlbkw.cn/Article/details/gtcrnmhli.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gybapoetw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.sjlbkw.cn/Article/details/gyzatoodj.sHtML

[Q80] 字符串截取
来源：http://baike.bbcook.cn/Article/details/gjsxyftxx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gnxzamjvj.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gmsqlbzsh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gcvzjzfaj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.epnwcf.com/Article/details/ghbksmrfj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/grlkxqxvj.sHtML

[Q83] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gluxxetmb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/ggcqzdxwy.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gyqphppnc.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gdynxupva.sHtML

[Q85] 数值取整
来源：http://read.share.bbcook.cn/Article/details/gnhsvsyty.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.sjlbkw.cn/Article/details/gcnuqwzut.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/gcsacunxj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fktsv.cn/Article/details/galkdgbou.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fktsv.cn/Article/details/ghqvbjrsk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.yfazqb.com/Article/details/ghskyvwof.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.tarul.cn/Article/details/gmohfvrfy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.vehdjk.com/Article/details/ggzvynonp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.yfazqb.com/Article/details/gnqgolsxr.sHtML

[Q89] 判断表是否存在
来源：http://mobile.vehdjk.com/Article/details/gknvqltrq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gumfnrgvc.sHtML

[Q90] 生成序号列
来源：http://3g.epnwcf.com/Article/details/ggwowjbwj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/gtpqvbvka.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/giytetzfj.sHtML

R. Bash 专题
来源：http://blog.tarul.cn/Article/details/gcfzwrwvg.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gahwgecje.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fktsv.cn/Article/details/gyxknjbsb.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.yfazqb.com/Article/details/glvyboloj.sHtML

set -euo pipefail
来源：http://read.share.yfazqb.com/Article/details/gospqsbhz.sHtML

[R02] 变量赋值与使用
来源：http://m.share.vehdjk.com/Article/details/gymfucdpf.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gcpabwabk.sHtML

[R03] 只读变量
来源：http://mobile.epnwcf.com/Article/details/grnvsifks.sHtML

readonly PI=3.14
来源：http://wap.bbcook.cn/Article/details/gquudhwnr.sHtML

[R04] 位置参数
来源：http://www.m.share.fktsv.cn/Article/details/glfyrtepo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.tarul.cn/Article/details/geimnoyvl.sHtML

[R05] 参数默认值
来源：http://3g.epnwcf.com/Article/details/gcpinyigp.sHtML

name="${1:-default}"
来源：http://read.share.bbcook.cn/Article/details/griunnkau.sHtML

[R06] 判断命令是否存在
来源：http://wap.fktsv.cn/Article/details/gslaeehmr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gmaepsspr.sHtML

[R07] if 判断文件
来源：http://www.share.fktsv.cn/Article/details/gifejngqf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gnedneqev.sHtML

[R08] 数值比较
来源：http://mobile.yfazqb.com/Article/details/gkgmrtnyl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.tarul.cn/Article/details/gsarryvjm.sHtML

[R09] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gwbtvcomk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.bbcook.cn/Article/details/ggvuwckyz.sHtML

[R10] 正则匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gvwmswdxd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.yfazqb.com/Article/details/gcvsxptsh.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/geqccbtgt.sHtML

case "$1" in
来源：http://wap.vehdjk.com/Article/details/gdsdytxkw.sHtML

start) echo "启动" ;;
来源：http://www.share.yfazqb.com/Article/details/gbwnfytcv.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gkejbjvau.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fktsv.cn/Article/details/gzjuoadcx.sHtML

esac
来源：http://wap.tarul.cn/Article/details/gyptdcvwd.sHtML

[R12] for 遍历文件
来源：http://wap.tarul.cn/Article/details/gqqepnoyi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.yfazqb.com/Article/details/gwbaoqnvd.sHtML

[R13] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gqmutfkgm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gqfmwytaf.sHtML

[R14] C 风格 for
来源：http://www.share.yfazqb.com/Article/details/gjhtgyvgp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gepqzwamm.sHtML

[R15] while 逐行读文件
来源：http://wap.fktsv.cn/Article/details/gfzxgulmy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.bbcook.cn/Article/details/gtaroakmn.sHtML

[R16] until 等待条件
来源：http://wap.epnwcf.com/Article/details/ghimbrcul.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/ghgjtpvlv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fktsv.cn/Article/details/gotvvegad.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.tarul.cn/Article/details/gokkbpoqv.sHtML

[R18] 遍历数组
来源：http://3g.fktsv.cn/Article/details/gqqdopird.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.tarul.cn/Article/details/gosnfoont.sHtML

[R19] 数组长度
来源：http://read.share.yfazqb.com/Article/details/gejejnptv.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fktsv.cn/Article/details/gcdrtqyib.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.epnwcf.com/Article/details/guwwhbhpw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.bbcook.cn/Article/details/gaioacjyt.sHtML

[R21] 字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gzkynbfdc.sHtML

echo "${#s}"
来源：http://www.blog.fktsv.cn/Article/details/gtirvmkji.sHtML

[R22] 截取子串
来源：http://3g.vehdjk.com/Article/details/gaafgatgt.sHtML

echo "${s:0:5}"
来源：http://read.share.tarul.cn/Article/details/gyycaskkg.sHtML

[R23] 字符串替换
来源：http://3g.fktsv.cn/Article/details/ggmeafong.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.tarul.cn/Article/details/gbypyalih.sHtML

[R24] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/guhvpjsqg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.vehdjk.com/Article/details/gxatdbkzu.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.vehdjk.com/Article/details/gecbztrgr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.epnwcf.com/Article/details/gcmoxcdon.sHtML

[R26] 命令替换
来源：http://baike.yfazqb.com/Article/details/gsklbmdjq.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.sjlbkw.cn/Article/details/ggtzyxakc.sHtML

[R27] 算术展开
来源：http://www.blog.epnwcf.com/Article/details/gsdblmjvj.sHtML

echo $((1 + 2 * 3))
来源：http://wap.bbcook.cn/Article/details/gypzfrowk.sHtML

[R28] 浮点运算
来源：http://www.share.vehdjk.com/Article/details/gwaktvkzt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fktsv.cn/Article/details/gikasxkty.sHtML

[R29] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/guvvozcwh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.vehdjk.com/Article/details/goihlolti.sHtML

[R30] 函数返回状态码
来源：http://blog.epnwcf.com/Article/details/gpletlvrf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/gxqjyteiq.sHtML

[R31] 局部变量
来源：http://www.m.share.tarul.cn/Article/details/ghsmnblrw.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/gphapjscz.sHtML

[R32] 参数个数校验
来源：http://3g.yfazqb.com/Article/details/gswpkvgpm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gwhgqebcp.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.sjlbkw.cn/Article/details/gdoohtmvg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.epnwcf.com/Article/details/gektrmcji.sHtML

[R34] 退出时清理
来源：http://3g.vehdjk.com/Article/details/ghzhktiav.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/ggeouruve.sHtML

[R35] 后台执行并等待
来源：http://mobile.tarul.cn/Article/details/gkpkahnrm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.tarul.cn/Article/details/gtlgsoxmb.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gmljevkzx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.bbcook.cn/Article/details/gtlqjngsi.sHtML

[R37] 把输出赋给变量
来源：http://www.share.tarul.cn/Article/details/gpzyenmpl.sHtML

files=$(ls -1)
来源：http://m.share.yfazqb.com/Article/details/glvovsgcl.sHtML

[R38] 管道串联
来源：http://read.share.epnwcf.com/Article/details/gdipylrwa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.bbcook.cn/Article/details/gtvpzirht.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.epnwcf.com/Article/details/guvtdkcfg.sHtML

cmd > out.log 2>&1
来源：http://baike.tarul.cn/Article/details/gjcvjypgw.sHtML

[R40] 追加写日志
来源：http://read.share.fktsv.cn/Article/details/gxxngmddb.sHtML

echo "log" >> out.log
来源：http://baike.yfazqb.com/Article/details/gdoewfqir.sHtML

[R41] 丢弃输出
来源：http://wap.sjlbkw.cn/Article/details/gqzrihlyd.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/gsqjxvzlc.sHtML

[R42] 输入重定向
来源：http://www.share.yfazqb.com/Article/details/gfokcdawb.sHtML

wc -l < a.txt
来源：http://wap.sjlbkw.cn/Article/details/gtmzemnlo.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gbyuofnsp.sHtML

find . -name "*.log" -type f
来源：http://blog.fktsv.cn/Article/details/gedcjduco.sHtML

[R44] 按修改时间查找
来源：http://3g.tarul.cn/Article/details/gbmwdoxox.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.vehdjk.com/Article/details/gowmzxvyl.sHtML

[R45] 批量删除
来源：http://baike.yfazqb.com/Article/details/gyuqnhqpm.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.sjlbkw.cn/Article/details/ghsmntwwr.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fktsv.cn/Article/details/gmixzvgvo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.yfazqb.com/Article/details/gflbeakdd.sHtML

[R47] sed 单行替换
来源：http://www.share.fktsv.cn/Article/details/glbfxpahf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.epnwcf.com/Article/details/gncjnbzmd.sHtML

[R48] awk 取指定列
来源：http://mobile.vehdjk.com/Article/details/guwmmvzku.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gjdnatrsy.sHtML

[R49] awk 带条件
来源：http://m.share.tarul.cn/Article/details/gpcgaqdoa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.vehdjk.com/Article/details/grbphvgaw.sHtML

[R50] awk 求和
来源：http://www.share.epnwcf.com/Article/details/ghazgtckr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/guxbdshbx.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/gvkpsdhzq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.sjlbkw.cn/Article/details/gxtmdxyaq.sHtML

[R52] 统计行数
来源：http://mobile.vehdjk.com/Article/details/guocmgnpv.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gabqsfuxb.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fktsv.cn/Article/details/gyefryrdv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/gtinfadug.sHtML

[R54] 比较两个文件
来源：http://mobile.bbcook.cn/Article/details/gwhfixfpc.sHtML

diff a.txt b.txt
来源：http://blog.tarul.cn/Article/details/gotzakguj.sHtML

[R55] 压缩与解压
来源：http://read.share.tarul.cn/Article/details/gmfrdfcpo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.bbcook.cn/Article/details/goikxnwzm.sHtML

[R56] 远程拷贝
来源：http://blog.vehdjk.com/Article/details/gobtfampu.sHtML

scp file user@host:/path/
来源：http://3g.bbcook.cn/Article/details/gyqlfuoyz.sHtML

[R57] 远程执行命令
来源：http://www.share.vehdjk.com/Article/details/gumxmthrh.sHtML

ssh user@host 'uptime'
来源：http://www.share.bbcook.cn/Article/details/gkskeggfn.sHtML

[R58] 下载文件
来源：http://wap.vehdjk.com/Article/details/ggpmukgnf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.yfazqb.com/Article/details/gmqxbitwu.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/gfpakqxyc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/gizyfsyks.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gsjjsrnie.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.vehdjk.com/Article/details/gzvkgobos.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/grypmsgpf.sHtML

df -h;  du -sh *
来源：http://www.blog.sjlbkw.cn/Article/details/gnxsqvhoj.sHtML

[R62] 找最占空间的文件
来源：http://wap.fktsv.cn/Article/details/gsmtjtemw.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.yfazqb.com/Article/details/gmzibvukm.sHtML

[R63] 内存与进程
来源：http://baike.epnwcf.com/Article/details/gxlwqzxxt.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/gngojfugt.sHtML

[R64] 结束进程
来源：http://www.blog.sjlbkw.cn/Article/details/gulzewvoe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.tarul.cn/Article/details/gvvwlbslv.sHtML

[R65] 查看端口占用
来源：http://3g.yfazqb.com/Article/details/gtfvujkge.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.vehdjk.com/Article/details/gijxspsao.sHtML

[R66] 定时任务
来源：http://www.m.share.fktsv.cn/Article/details/gyrcerutz.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/gpijmoalo.sHtML

[R67] 生成随机十六进制串
来源：http://3g.yfazqb.com/Article/details/gubvzycbb.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/glpyhhvgv.sHtML

[R68] 计算文件校验值
来源：http://wap.epnwcf.com/Article/details/gqyroobmy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gnqkyhojc.sHtML

[R69] 生成随机密码
来源：http://www.m.share.yfazqb.com/Article/details/gaddobjox.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.bbcook.cn/Article/details/gejxunhmm.sHtML

[R70] 时间戳与互转
来源：http://www.blog.vehdjk.com/Article/details/gryatkldj.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.sjlbkw.cn/Article/details/glnaxjwww.sHtML

[R71] 日期格式化
来源：http://mobile.epnwcf.com/Article/details/gaihhoyhw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.sjlbkw.cn/Article/details/gdimzqjna.sHtML

[R72] 等待端口就绪
来源：http://www.share.bbcook.cn/Article/details/gbaczkkoq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gjpoleqoh.sHtML

[R73] 分割大日志
来源：http://mobile.tarul.cn/Article/details/ghpwclkrv.sHtML

split -l 1000 big.log part_
来源：http://mobile.yfazqb.com/Article/details/gkdbffsyu.sHtML

[R74] 批量重命名
来源：http://www.share.yfazqb.com/Article/details/gpbhqcwva.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/gtnzregdq.sHtML

[R75] 导出环境变量
来源：http://www.share.vehdjk.com/Article/details/ghoqiytwv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.bbcook.cn/Article/details/goslgquaf.sHtML

[R76] 使用临时文件
来源：http://read.share.tarul.cn/Article/details/gltcluifn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/glfttydcg.sHtML

[R77] 读取用户输入
来源：http://wap.yfazqb.com/Article/details/gydgizape.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.epnwcf.com/Article/details/gagglqocg.sHtML

[R78] 交互式菜单
来源：http://wap.epnwcf.com/Article/details/gdjwiezka.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/gjqxjsjoa.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gimvedtvf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fktsv.cn/Article/details/gebolzpff.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/gdtayddaq.sHtML

time ./run.sh
来源：http://www.share.tarul.cn/Article/details/gwowxnyxl.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gqllkgwcb.sHtML

S. C / C++ 专题
来源：http://blog.fktsv.cn/Article/details/gpnkwexrv.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjjjryzpa.sHtML

[S01] C：Hello World
来源：http://wap.bbcook.cn/Article/details/garmbqqhz.sHtML

#include <stdio.h>
来源：http://www.share.yfazqb.com/Article/details/gkbplrhke.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gvrxctfzr.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.yfazqb.com/Article/details/gyoaxmtbc.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.epnwcf.com/Article/details/gvmcptlwq.sHtML

[S03] C：读入整数
来源：http://www.m.share.epnwcf.com/Article/details/grxcufyoc.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjakejgf.sHtML

[S04] C：字符串复制
来源：http://blog.fktsv.cn/Article/details/grppbbadw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gvqfbbhdx.sHtML

[S05] C：字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gixgfcjqv.sHtML

strlen(s)
来源：http://www.blog.epnwcf.com/Article/details/gmsxnmjat.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/guogieezp.sHtML

strcmp(a, b) == 0
来源：http://www.share.sjlbkw.cn/Article/details/gqvfihszb.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/ggavauqqw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.tarul.cn/Article/details/gxolqcvrz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.sjlbkw.cn/Article/details/gohiudeuy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fktsv.cn/Article/details/giloomncd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.yfazqb.com/Article/details/ghcpntlxw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.sjlbkw.cn/Article/details/gwxbpwgxt.sHtML

[S10] C：指针与解引用
来源：http://m.share.tarul.cn/Article/details/gxsvrrhze.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fktsv.cn/Article/details/gmqprajra.sHtML

[S11] C：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gynuvxeuo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fktsv.cn/Article/details/gttrzizng.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.bbcook.cn/Article/details/guxmbcyix.sHtML

fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gpxtfaics.sHtML

[S12] C：写文件
来源：http://3g.epnwcf.com/Article/details/gpefdymtu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gmmhyoxhy.sHtML

[S13] C：宏定义
来源：http://m.share.yfazqb.com/Article/details/glsusvbth.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.yfazqb.com/Article/details/gahxfxyut.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/ghhfkdfnv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.tarul.cn/Article/details/glpfmtvxf.sHtML

[S15] C：类型转换
来源：http://mobile.yfazqb.com/Article/details/ggyusndqf.sHtML

(double) a / b
来源：http://www.m.share.tarul.cn/Article/details/gibuxhcrm.sHtML

[S16] C：位操作置位
来源：http://3g.fktsv.cn/Article/details/ghukqaxnw.sHtML

x |= (1 << 3);
来源：http://www.m.share.yfazqb.com/Article/details/glxlvgawr.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.epnwcf.com/Article/details/guxmtxggm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/gzcdghpok.sHtML

[S18] C：命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gqxruooca.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.bbcook.cn/Article/details/gyaaycjvq.sHtML

[S19] C：快速排序
来源：http://blog.yfazqb.com/Article/details/gyyrdhmxp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/gbitigiyy.sHtML

[S20] C：二分查找
来源：http://3g.sjlbkw.cn/Article/details/gcitxazch.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gjrllwyvk.sHtML

[S21] C：字符类别判断
来源：http://3g.vehdjk.com/Article/details/gruecqbfg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.bbcook.cn/Article/details/gmoeadkse.sHtML

[S22] C：字符串转数字
来源：http://blog.yfazqb.com/Article/details/ghrjfewsj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.tarul.cn/Article/details/gfjusdnfe.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gkvvguspe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.epnwcf.com/Article/details/gjbnitfwe.sHtML

[S24] C：获取本地时间
来源：http://m.share.bbcook.cn/Article/details/ghzttbhzw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/gcuecxxdk.sHtML

[S25] C：内存拷贝
来源：http://read.share.fktsv.cn/Article/details/guspicocl.sHtML

memcpy(dst, src, n);
来源：http://wap.fktsv.cn/Article/details/gyxblldwy.sHtML

[S26] C：内存清零
来源：http://baike.yfazqb.com/Article/details/gmqpnhwqr.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.sjlbkw.cn/Article/details/glpmhcbph.sHtML

[S27] C：定义常量
来源：http://m.share.yfazqb.com/Article/details/ghumyfweu.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/glnejsaiw.sHtML

[S28] C：静态变量
来源：http://www.share.fktsv.cn/Article/details/gxzxmhxdj.sHtML


<!-- 参考信息 -->