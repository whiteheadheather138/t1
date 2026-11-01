代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gyqltxelb.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fktsv.cn/Article/details/gwgvvaasu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.epnwcf.com/Article/details/giniscygb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fktsv.cn/Article/details/gdnflqvub.sHtML

[Q61] 移动平均
来源：http://m.share.tarul.cn/Article/details/gyhibbiwe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gbvexwfcz.sHtML

[Q62] 分组占比
来源：http://blog.bbcook.cn/Article/details/gzlfdrypm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gdhucnqxm.sHtML

[Q63] 开启事务
来源：http://baike.fktsv.cn/Article/details/gpdhlfdsi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fktsv.cn/Article/details/ghglnddqg.sHtML

[Q64] 提交事务
来源：http://blog.vehdjk.com/Article/details/giqrkiosy.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/gekwxzkdh.sHtML

[Q65] 回滚事务
来源：http://baike.yfazqb.com/Article/details/glfdmprvy.sHtML

ROLLBACK;
来源：http://m.share.sjlbkw.cn/Article/details/gcdldifbe.sHtML

[Q66] 行锁查询
来源：http://mobile.epnwcf.com/Article/details/gzdaxcqcp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.tarul.cn/Article/details/gcbetyoqi.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.epnwcf.com/Article/details/gteilinbn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fktsv.cn/Article/details/ghmbehval.sHtML

[Q68] 保存点
来源：http://mobile.sjlbkw.cn/Article/details/gajoiudmg.sHtML

SAVEPOINT sp1;
来源：http://baike.yfazqb.com/Article/details/gwjbvxahd.sHtML

ROLLBACK TO sp1;
来源：http://blog.bbcook.cn/Article/details/guhsjrfce.sHtML

[Q69] 查看执行计划
来源：http://3g.yfazqb.com/Article/details/glhiorhsq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.tarul.cn/Article/details/gxbdveoiq.sHtML

[Q70] 更新统计信息
来源：http://blog.yfazqb.com/Article/details/garmvkyqq.sHtML

ANALYZE TABLE users;
来源：http://m.share.tarul.cn/Article/details/gkovsnfvt.sHtML

[Q71] 查看建表语句
来源：http://blog.tarul.cn/Article/details/gtjkiglnw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.epnwcf.com/Article/details/gqswmfkhc.sHtML

[Q72] 查看索引
来源：http://wap.sjlbkw.cn/Article/details/gocatfuwl.sHtML

SHOW INDEX FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/guphnelmo.sHtML

[Q73] 查看表状态
来源：http://baike.sjlbkw.cn/Article/details/gjregltws.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fktsv.cn/Article/details/gayrcaoia.sHtML

[Q74] 强制使用索引
来源：http://www.share.epnwcf.com/Article/details/gknxnjjmy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.tarul.cn/Article/details/gtlzejvie.sHtML

[Q75] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gqohaopsx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.epnwcf.com/Article/details/gfhsvmgtt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fktsv.cn/Article/details/gbrvoqckn.sHtML

[Q76] 按天统计
来源：http://read.share.epnwcf.com/Article/details/ghndstabl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.yfazqb.com/Article/details/gdmndtvum.sHtML

[Q77] 时间加减
来源：http://www.m.share.tarul.cn/Article/details/gfihmqgjr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.yfazqb.com/Article/details/gencwloqv.sHtML

[Q78] 当前时间
来源：http://www.blog.epnwcf.com/Article/details/godphlhqz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.vehdjk.com/Article/details/gfnftjqcy.sHtML

[Q79] 字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gggjyszfj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fktsv.cn/Article/details/gqhsdcyuj.sHtML

[Q80] 字符串截取
来源：http://wap.epnwcf.com/Article/details/gwtjvlbom.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gpgwasjmy.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gltgdghao.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gdhtiytso.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.epnwcf.com/Article/details/geojmkknv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/giywrrdfd.sHtML

[Q83] 大小写转换
来源：http://3g.epnwcf.com/Article/details/gvwkrqome.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/grgoaferh.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.yfazqb.com/Article/details/gtlvcshwg.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gwekugmhc.sHtML

[Q85] 数值取整
来源：http://3g.sjlbkw.cn/Article/details/gblhoetgq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.sjlbkw.cn/Article/details/gezhsekgu.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.epnwcf.com/Article/details/gyaqfligs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.yfazqb.com/Article/details/gwhvuqugt.sHtML

[Q87] JSON 字段做条件
来源：http://baike.yfazqb.com/Article/details/gbpqfktok.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.bbcook.cn/Article/details/gdtjltkoo.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.epnwcf.com/Article/details/grpdhusni.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.bbcook.cn/Article/details/grzikmilz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.bbcook.cn/Article/details/gjiaidvvn.sHtML

[Q89] 判断表是否存在
来源：http://read.share.epnwcf.com/Article/details/gcbkbouwy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.yfazqb.com/Article/details/gyxrenysa.sHtML

[Q90] 生成序号列
来源：http://read.share.vehdjk.com/Article/details/gsjrszgnz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.bbcook.cn/Article/details/gbjxphsmx.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcfodnrsp.sHtML

R. Bash 专题
来源：http://mobile.vehdjk.com/Article/details/gkujqdqax.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grdbwuwqu.sHtML

[R01] shebang 与严格模式
来源：http://baike.epnwcf.com/Article/details/gisidbqfs.sHtML

#!/usr/bin/env bash
来源：http://m.share.yfazqb.com/Article/details/gvudgnljo.sHtML

set -euo pipefail
来源：http://www.share.vehdjk.com/Article/details/gtxamslnx.sHtML

[R02] 变量赋值与使用
来源：http://blog.sjlbkw.cn/Article/details/gjdnpmyzs.sHtML

name="Tom"; echo "$name"
来源：http://3g.vehdjk.com/Article/details/gwgeytgzt.sHtML

[R03] 只读变量
来源：http://read.share.fktsv.cn/Article/details/gzhbzpsfk.sHtML

readonly PI=3.14
来源：http://mobile.epnwcf.com/Article/details/gurlovnpg.sHtML

[R04] 位置参数
来源：http://baike.sjlbkw.cn/Article/details/gvbakohau.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fktsv.cn/Article/details/gnlmnmrpx.sHtML

[R05] 参数默认值
来源：http://read.share.vehdjk.com/Article/details/gzkudlxec.sHtML

name="${1:-default}"
来源：http://blog.vehdjk.com/Article/details/ggagkkyhh.sHtML

[R06] 判断命令是否存在
来源：http://read.share.yfazqb.com/Article/details/gbwgegmbb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gxnxmvlgn.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/ggbidxntv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.vehdjk.com/Article/details/gtvakschl.sHtML

[R08] 数值比较
来源：http://www.blog.tarul.cn/Article/details/gjoaruifu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gcusudixq.sHtML

[R09] 字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gctvwkhku.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.bbcook.cn/Article/details/ghpuezjrl.sHtML

[R10] 正则匹配
来源：http://www.m.share.bbcook.cn/Article/details/gmnonyarf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fktsv.cn/Article/details/gjswbnkzv.sHtML

[R11] case 多分支
来源：http://www.m.share.yfazqb.com/Article/details/gnovmhjgx.sHtML

case "$1" in
来源：http://wap.fktsv.cn/Article/details/gwdwwanfa.sHtML

start) echo "启动" ;;
来源：http://www.share.fktsv.cn/Article/details/gxqeoecud.sHtML

stop)  echo "停止" ;;
来源：http://3g.bbcook.cn/Article/details/gcoeosaij.sHtML

*)     echo "未知命令" ;;
来源：http://baike.sjlbkw.cn/Article/details/gvvhwdbpk.sHtML

esac
来源：http://wap.tarul.cn/Article/details/gmqxumelx.sHtML

[R12] for 遍历文件
来源：http://baike.yfazqb.com/Article/details/guiwenlpt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.yfazqb.com/Article/details/gzsmkgakq.sHtML

[R13] for 计数循环
来源：http://baike.bbcook.cn/Article/details/gpsjbojar.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/ghmhbsxyt.sHtML

[R14] C 风格 for
来源：http://www.share.sjlbkw.cn/Article/details/gvavwlzdb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gaiuhelgv.sHtML

[R15] while 逐行读文件
来源：http://3g.yfazqb.com/Article/details/gmdqxpjkv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fktsv.cn/Article/details/gyrbafcmv.sHtML

[R16] until 等待条件
来源：http://www.share.vehdjk.com/Article/details/goxcqhgoe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gakdhyxry.sHtML

[R17] 数组定义与取值
来源：http://wap.epnwcf.com/Article/details/gizyxcbna.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.epnwcf.com/Article/details/goyceokuy.sHtML

[R18] 遍历数组
来源：http://m.share.tarul.cn/Article/details/gxzckxndr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/gulsgazgb.sHtML

[R19] 数组长度
来源：http://read.share.fktsv.cn/Article/details/glxheemjx.sHtML

echo "${#arr[@]}"
来源：http://baike.fktsv.cn/Article/details/ghqxgoktf.sHtML

[R20] 关联数组（字典）
来源：http://www.share.sjlbkw.cn/Article/details/glemxjrcz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.epnwcf.com/Article/details/gqdaclrxr.sHtML

[R21] 字符串长度
来源：http://3g.bbcook.cn/Article/details/gzxbpavwl.sHtML

echo "${#s}"
来源：http://blog.sjlbkw.cn/Article/details/gvaiftkye.sHtML

[R22] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gfnwmtejn.sHtML

echo "${s:0:5}"
来源：http://mobile.fktsv.cn/Article/details/gugmmenaz.sHtML

[R23] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gnrguerhn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.epnwcf.com/Article/details/gfeldctcx.sHtML

[R24] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/ghxzufdbd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.epnwcf.com/Article/details/gprdntzho.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.tarul.cn/Article/details/govdoyxoy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.vehdjk.com/Article/details/guanykjhe.sHtML

[R26] 命令替换
来源：http://baike.epnwcf.com/Article/details/gwljwxnqi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.vehdjk.com/Article/details/gifcojnme.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/gabygvxwh.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.epnwcf.com/Article/details/gvrogspar.sHtML

[R28] 浮点运算
来源：http://wap.bbcook.cn/Article/details/gqauodhba.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.yfazqb.com/Article/details/gbtjonclr.sHtML

[R29] 定义函数
来源：http://blog.yfazqb.com/Article/details/gpgmbmwpq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.bbcook.cn/Article/details/gxjgqvwej.sHtML

[R30] 函数返回状态码
来源：http://mobile.tarul.cn/Article/details/gfganwupd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.bbcook.cn/Article/details/gcllrscqf.sHtML

[R31] 局部变量
来源：http://www.share.sjlbkw.cn/Article/details/getpjgnce.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.epnwcf.com/Article/details/gqazdggzh.sHtML

[R32] 参数个数校验
来源：http://www.share.tarul.cn/Article/details/geesthnam.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gdmlzvbez.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fktsv.cn/Article/details/gzukxetxm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fktsv.cn/Article/details/gcqsdavlw.sHtML

[R34] 退出时清理
来源：http://blog.vehdjk.com/Article/details/gphoqmjzd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gkqtmagpf.sHtML

[R35] 后台执行并等待
来源：http://3g.vehdjk.com/Article/details/gmzucwxjq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.sjlbkw.cn/Article/details/gyehrzbgv.sHtML

[R36] 并发执行多个任务
来源：http://3g.sjlbkw.cn/Article/details/gvdnogizd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.vehdjk.com/Article/details/gxkxtataw.sHtML

[R37] 把输出赋给变量
来源：http://3g.sjlbkw.cn/Article/details/gsgkpjzla.sHtML

files=$(ls -1)
来源：http://www.blog.vehdjk.com/Article/details/gapzvrojd.sHtML

[R38] 管道串联
来源：http://www.blog.fktsv.cn/Article/details/gcuilesmo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.tarul.cn/Article/details/gqffbknoy.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.tarul.cn/Article/details/gnvnlofeg.sHtML

cmd > out.log 2>&1
来源：http://read.share.fktsv.cn/Article/details/gkukbjdbt.sHtML

[R40] 追加写日志
来源：http://www.m.share.yfazqb.com/Article/details/ggathgkpb.sHtML

echo "log" >> out.log
来源：http://mobile.epnwcf.com/Article/details/gtglbkdhc.sHtML

[R41] 丢弃输出
来源：http://3g.yfazqb.com/Article/details/gxtmrdpak.sHtML

cmd >/dev/null 2>&1
来源：http://baike.bbcook.cn/Article/details/gkmfhotxw.sHtML

[R42] 输入重定向
来源：http://baike.vehdjk.com/Article/details/gzvzdppzt.sHtML

wc -l < a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gkvgtfhxi.sHtML

[R43] 按名字查找文件
来源：http://3g.vehdjk.com/Article/details/ggwxpdfeb.sHtML

find . -name "*.log" -type f
来源：http://m.share.epnwcf.com/Article/details/glcnzctku.sHtML

[R44] 按修改时间查找
来源：http://3g.vehdjk.com/Article/details/galtcfbsg.sHtML

find . -mtime -7 -type f
来源：http://mobile.epnwcf.com/Article/details/ghwtindmf.sHtML

[R45] 批量删除
来源：http://3g.fktsv.cn/Article/details/gwzeihstb.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.epnwcf.com/Article/details/gyvxpeolg.sHtML

[R46] 递归替换文件内容
来源：http://baike.tarul.cn/Article/details/gnhbccgkx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.sjlbkw.cn/Article/details/gskswfbps.sHtML

[R47] sed 单行替换
来源：http://www.blog.tarul.cn/Article/details/gyrdbmswy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.bbcook.cn/Article/details/gytfhiyfk.sHtML

[R48] awk 取指定列
来源：http://blog.fktsv.cn/Article/details/gclphfaed.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gpnvrotqo.sHtML

[R49] awk 带条件
来源：http://mobile.tarul.cn/Article/details/ggsmrfkog.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.sjlbkw.cn/Article/details/goklgefcc.sHtML

[R50] awk 求和
来源：http://m.share.bbcook.cn/Article/details/grqsoetmk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.epnwcf.com/Article/details/gbhjyxiws.sHtML

[R51] 排序去重取前几
来源：http://wap.yfazqb.com/Article/details/gqavejezp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fktsv.cn/Article/details/gypermyox.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/gdyqzuebz.sHtML

wc -l a.txt
来源：http://wap.bbcook.cn/Article/details/gvdcwhodf.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.epnwcf.com/Article/details/gbollrkgb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.yfazqb.com/Article/details/gsgnpojoo.sHtML

[R54] 比较两个文件
来源：http://www.m.share.yfazqb.com/Article/details/gnojcfynf.sHtML

diff a.txt b.txt
来源：http://www.m.share.yfazqb.com/Article/details/glqwcnwua.sHtML

[R55] 压缩与解压
来源：http://www.share.fktsv.cn/Article/details/gitbzkbsg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.yfazqb.com/Article/details/gisaotand.sHtML

[R56] 远程拷贝
来源：http://wap.vehdjk.com/Article/details/gcqzghtyb.sHtML

scp file user@host:/path/
来源：http://blog.epnwcf.com/Article/details/gatmjupfc.sHtML

[R57] 远程执行命令
来源：http://www.blog.vehdjk.com/Article/details/ggewpfgev.sHtML

ssh user@host 'uptime'
来源：http://baike.vehdjk.com/Article/details/gbncltgom.sHtML

[R58] 下载文件
来源：http://read.share.sjlbkw.cn/Article/details/glpqkwfnq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.sjlbkw.cn/Article/details/gopyktdxm.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gduljgcfl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.vehdjk.com/Article/details/gpchckvqu.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gplxqfyxt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.vehdjk.com/Article/details/gvozdizta.sHtML

[R61] 磁盘占用
来源：http://m.share.yfazqb.com/Article/details/gtsxfgdll.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/gbdlciums.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gulqcvsdz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fktsv.cn/Article/details/gebzbdbpj.sHtML

[R63] 内存与进程
来源：http://baike.vehdjk.com/Article/details/gdqybrrba.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.epnwcf.com/Article/details/gdcqksaex.sHtML

[R64] 结束进程
来源：http://blog.epnwcf.com/Article/details/gobesnaal.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.yfazqb.com/Article/details/gvgjdtqpj.sHtML

[R65] 查看端口占用
来源：http://www.m.share.bbcook.cn/Article/details/gtrrndhtq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.epnwcf.com/Article/details/gwjbhikxd.sHtML

[R66] 定时任务
来源：http://www.m.share.fktsv.cn/Article/details/gavaakztj.sHtML

crontab -e;  crontab -l
来源：http://baike.vehdjk.com/Article/details/gqatxcbmu.sHtML

[R67] 生成随机十六进制串
来源：http://blog.yfazqb.com/Article/details/gjpvzishj.sHtML

openssl rand -hex 16
来源：http://blog.epnwcf.com/Article/details/gmjbmocqy.sHtML

[R68] 计算文件校验值
来源：http://blog.yfazqb.com/Article/details/gkouvcwwj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gyckbhkma.sHtML

[R69] 生成随机密码
来源：http://www.share.bbcook.cn/Article/details/gvpjitzfl.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.yfazqb.com/Article/details/glwbughib.sHtML

[R70] 时间戳与互转
来源：http://www.blog.bbcook.cn/Article/details/gjzfhpwjh.sHtML

date +%s;  date -d @1700000000
来源：http://wap.vehdjk.com/Article/details/gcatszyrn.sHtML

[R71] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gwpirbvdp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.tarul.cn/Article/details/ghbqmnxkv.sHtML

[R72] 等待端口就绪
来源：http://www.share.sjlbkw.cn/Article/details/grxqokhpi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/gzllwwavn.sHtML

[R73] 分割大日志
来源：http://www.blog.fktsv.cn/Article/details/gflqlwzhf.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/gqjxmohna.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/gesgngvwz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gkhzzgbqu.sHtML

[R75] 导出环境变量
来源：http://wap.vehdjk.com/Article/details/gpqyhmwrc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.bbcook.cn/Article/details/gglirzulw.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/gvflbhplq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gkmivmfqq.sHtML

[R77] 读取用户输入
来源：http://www.share.epnwcf.com/Article/details/gmahyzupf.sHtML

read -rp "请输入: " ans
来源：http://blog.bbcook.cn/Article/details/gtlvhifmw.sHtML

[R78] 交互式菜单
来源：http://www.blog.yfazqb.com/Article/details/gdqfellls.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.sjlbkw.cn/Article/details/gqbvlyspt.sHtML

[R79] 解析命令行选项
来源：http://www.blog.sjlbkw.cn/Article/details/gxythelhn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.vehdjk.com/Article/details/gdxpwcyca.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/grvyqvukx.sHtML

time ./run.sh
来源：http://read.share.sjlbkw.cn/Article/details/gasbthxst.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpouxvqya.sHtML

S. C / C++ 专题
来源：http://m.share.fktsv.cn/Article/details/gouaxdyvl.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gtmvqxbpb.sHtML

[S01] C：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gqgoaqfvn.sHtML

#include <stdio.h>
来源：http://wap.epnwcf.com/Article/details/ggaoucjkw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fktsv.cn/Article/details/gloicqefg.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gkamqvxkp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.bbcook.cn/Article/details/ghitdrlml.sHtML

[S03] C：读入整数
来源：http://3g.sjlbkw.cn/Article/details/gwswukgla.sHtML

int x; scanf("%d", &x);
来源：http://wap.epnwcf.com/Article/details/gzfrmmpww.sHtML

[S04] C：字符串复制
来源：http://www.m.share.bbcook.cn/Article/details/gwmblabcs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gfjatuuin.sHtML

[S05] C：字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gggvqrpnp.sHtML

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/glkjsjidj.sHtML

[S06] C：字符串比较
来源：http://www.share.yfazqb.com/Article/details/gtnuvbnxb.sHtML

strcmp(a, b) == 0
来源：http://blog.bbcook.cn/Article/details/gdiinekts.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/gpqkrpptl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fktsv.cn/Article/details/gxidrjuyu.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.epnwcf.com/Article/details/gdgxcitik.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/gwlukcttl.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.yfazqb.com/Article/details/gtvemycjw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gnvvniecs.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/gfqevkifi.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.sjlbkw.cn/Article/details/gassqajui.sHtML

[S11] C：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gqjbeckuc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fktsv.cn/Article/details/gonmfppis.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.vehdjk.com/Article/details/gxkupbath.sHtML

fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gvvkprvxf.sHtML

[S12] C：写文件
来源：http://read.share.tarul.cn/Article/details/gmssmaohk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gaweuunjs.sHtML

[S13] C：宏定义
来源：http://m.share.yfazqb.com/Article/details/gqwwkezlq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.epnwcf.com/Article/details/guflusdcp.sHtML

[S14] C：枚举
来源：http://wap.tarul.cn/Article/details/gwwdexcre.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fktsv.cn/Article/details/gcvcnrxhw.sHtML

[S15] C：类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gxtreswup.sHtML

(double) a / b
来源：http://blog.tarul.cn/Article/details/grtcrniug.sHtML

[S16] C：位操作置位
来源：http://www.blog.fktsv.cn/Article/details/giasnoxkc.sHtML

x |= (1 << 3);
来源：http://m.share.tarul.cn/Article/details/gryjtuvqw.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/grmckfnpa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpeatiny.sHtML

[S18] C：命令行参数
来源：http://www.share.epnwcf.com/Article/details/gupmvvrhk.sHtML

int main(int argc, char **argv)
来源：http://read.share.fktsv.cn/Article/details/gzsanfdbq.sHtML

[S19] C：快速排序
来源：http://mobile.yfazqb.com/Article/details/guvsrtsle.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gubszrxbh.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gqoruggbd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gpzxjevio.sHtML

[S21] C：字符类别判断
来源：http://www.share.vehdjk.com/Article/details/glgmkbizn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.tarul.cn/Article/details/glsyjcyzv.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/gcywfnxjm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/gxsqhurgc.sHtML

[S23] C：随机数
来源：http://read.share.vehdjk.com/Article/details/gcnyfynha.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.epnwcf.com/Article/details/gqkdtezhf.sHtML

[S24] C：获取本地时间
来源：http://mobile.epnwcf.com/Article/details/gfesqeiuw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fktsv.cn/Article/details/gojtylhnm.sHtML

[S25] C：内存拷贝
来源：http://blog.bbcook.cn/Article/details/goyseftja.sHtML

memcpy(dst, src, n);
来源：http://read.share.yfazqb.com/Article/details/geejblfgk.sHtML

[S26] C：内存清零
来源：http://wap.yfazqb.com/Article/details/ggfqekakk.sHtML

memset(a, 0, sizeof a);
来源：http://blog.yfazqb.com/Article/details/gzjszlfvh.sHtML

[S27] C：定义常量
来源：http://www.m.share.sjlbkw.cn/Article/details/grfhrqrny.sHtML

const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/grronbdim.sHtML

[S28] C：静态变量
来源：http://read.share.yfazqb.com/Article/details/gdiqhwjxg.sHtML

static int counter = 0;
来源：http://www.blog.vehdjk.com/Article/details/grzdilrbv.sHtML

[S29] C：变参函数
来源：http://wap.bbcook.cn/Article/details/geneieyeg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.epnwcf.com/Article/details/gjpkadhkj.sHtML

[S30] C：头文件保护
来源：http://m.share.vehdjk.com/Article/details/gsqqeolkr.sHtML


<!-- 参考信息 -->