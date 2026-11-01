代发 wailian999

[Q61] 移动平均
来源：http://www.blog.vehdjk.com/Article/details/gxeyeqfpn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gufuubhsn.sHtML

[Q62] 分组占比
来源：http://mobile.sjlbkw.cn/Article/details/gjauptbuq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gpoyznbhh.sHtML

[Q63] 开启事务
来源：http://www.share.bbcook.cn/Article/details/graoglpfp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.epnwcf.com/Article/details/gtxsbljvd.sHtML

[Q64] 提交事务
来源：http://www.share.bbcook.cn/Article/details/grkcqjzpx.sHtML

COMMIT;
来源：http://www.m.share.fktsv.cn/Article/details/gbfkwsiqc.sHtML

[Q65] 回滚事务
来源：http://m.share.yfazqb.com/Article/details/gaknxyjiv.sHtML

ROLLBACK;
来源：http://www.share.fktsv.cn/Article/details/gewiemuxm.sHtML

[Q66] 行锁查询
来源：http://www.blog.epnwcf.com/Article/details/gumpkhgny.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.sjlbkw.cn/Article/details/gwfcencdd.sHtML

[Q67] 设置隔离级别
来源：http://3g.yfazqb.com/Article/details/glgvujigf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.epnwcf.com/Article/details/gqvwtxngh.sHtML

[Q68] 保存点
来源：http://read.share.sjlbkw.cn/Article/details/gezjbscuz.sHtML

SAVEPOINT sp1;
来源：http://3g.epnwcf.com/Article/details/gnjjenvwc.sHtML

ROLLBACK TO sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gsrgunpow.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.bbcook.cn/Article/details/gnsxutekd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.yfazqb.com/Article/details/gywxvkvsh.sHtML

[Q70] 更新统计信息
来源：http://baike.fktsv.cn/Article/details/gjyfutrxs.sHtML

ANALYZE TABLE users;
来源：http://3g.fktsv.cn/Article/details/ghphyefwd.sHtML

[Q71] 查看建表语句
来源：http://baike.epnwcf.com/Article/details/gblczdspn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.epnwcf.com/Article/details/gcnckwmvr.sHtML

[Q72] 查看索引
来源：http://mobile.bbcook.cn/Article/details/gdhvbvpps.sHtML

SHOW INDEX FROM users;
来源：http://m.share.yfazqb.com/Article/details/gkaueceks.sHtML

[Q73] 查看表状态
来源：http://wap.fktsv.cn/Article/details/gbyaofjrm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.bbcook.cn/Article/details/gbqgjsbae.sHtML

[Q74] 强制使用索引
来源：http://www.blog.bbcook.cn/Article/details/gogrkhwzd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fktsv.cn/Article/details/gyzxsqhdv.sHtML

[Q75] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/glcaplvwz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gorrimqrm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.epnwcf.com/Article/details/gmussuyib.sHtML

[Q76] 按天统计
来源：http://www.share.yfazqb.com/Article/details/gjimgelko.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fktsv.cn/Article/details/gkrensnmg.sHtML

[Q77] 时间加减
来源：http://baike.epnwcf.com/Article/details/giafkanwz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/gqarvwkma.sHtML

[Q78] 当前时间
来源：http://m.share.bbcook.cn/Article/details/giiyijqgs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.vehdjk.com/Article/details/gimnshwku.sHtML

[Q79] 字符串拼接
来源：http://3g.yfazqb.com/Article/details/growhurhq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.epnwcf.com/Article/details/gtcohzghb.sHtML

[Q80] 字符串截取
来源：http://3g.epnwcf.com/Article/details/gmjhqbmjp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.yfazqb.com/Article/details/goxbizgpd.sHtML

[Q81] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/ginauceza.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.tarul.cn/Article/details/gyejprfmw.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fktsv.cn/Article/details/gschrzpof.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/guwtrkshv.sHtML

[Q83] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gxivflawd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/golcbixuc.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.sjlbkw.cn/Article/details/gazpcsotj.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/grvvewoqc.sHtML

[Q85] 数值取整
来源：http://mobile.tarul.cn/Article/details/gneifaqxp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.epnwcf.com/Article/details/geenobjuz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.sjlbkw.cn/Article/details/gvlytnsry.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.sjlbkw.cn/Article/details/gyuiuhuuc.sHtML

[Q87] JSON 字段做条件
来源：http://wap.tarul.cn/Article/details/gzphprkok.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.epnwcf.com/Article/details/gvhglnkwl.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.epnwcf.com/Article/details/glehslafe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.yfazqb.com/Article/details/ghzcxpexf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.bbcook.cn/Article/details/gxwkvfeyk.sHtML

[Q89] 判断表是否存在
来源：http://baike.tarul.cn/Article/details/ghmwcxwxo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.tarul.cn/Article/details/gogqppdtd.sHtML

[Q90] 生成序号列
来源：http://www.share.bbcook.cn/Article/details/grynihbnc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.bbcook.cn/Article/details/gxblrlonb.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzbptnayt.sHtML

R. Bash 专题
来源：http://wap.bbcook.cn/Article/details/gnbtzhhvi.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbtexecqs.sHtML

[R01] shebang 与严格模式
来源：http://mobile.tarul.cn/Article/details/gnqrbplbj.sHtML

#!/usr/bin/env bash
来源：http://www.share.yfazqb.com/Article/details/gjguhzabj.sHtML

set -euo pipefail
来源：http://baike.tarul.cn/Article/details/gespfvzwd.sHtML

[R02] 变量赋值与使用
来源：http://mobile.vehdjk.com/Article/details/gkyytpgay.sHtML

name="Tom"; echo "$name"
来源：http://blog.vehdjk.com/Article/details/gjdcghmzr.sHtML

[R03] 只读变量
来源：http://read.share.epnwcf.com/Article/details/gdogkbpnd.sHtML

readonly PI=3.14
来源：http://baike.fktsv.cn/Article/details/gazwdtifj.sHtML

[R04] 位置参数
来源：http://mobile.vehdjk.com/Article/details/gvqwufyxz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.yfazqb.com/Article/details/grkitwxza.sHtML

[R05] 参数默认值
来源：http://m.share.sjlbkw.cn/Article/details/gknzqhybg.sHtML

name="${1:-default}"
来源：http://baike.vehdjk.com/Article/details/gbgrfrdkn.sHtML

[R06] 判断命令是否存在
来源：http://blog.vehdjk.com/Article/details/gkpnnylkl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/gimgfvgnf.sHtML

[R07] if 判断文件
来源：http://mobile.sjlbkw.cn/Article/details/gxlgebhks.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.bbcook.cn/Article/details/gmolgefmk.sHtML

[R08] 数值比较
来源：http://blog.fktsv.cn/Article/details/gmjicmvrg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.vehdjk.com/Article/details/gppmnjluy.sHtML

[R09] 字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gectnskev.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.bbcook.cn/Article/details/gaxmfvffm.sHtML

[R10] 正则匹配
来源：http://blog.tarul.cn/Article/details/gfbdfeedk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.vehdjk.com/Article/details/goijjkdkd.sHtML

[R11] case 多分支
来源：http://www.share.tarul.cn/Article/details/gflblwazh.sHtML

case "$1" in
来源：http://wap.bbcook.cn/Article/details/gmbljkbnm.sHtML

start) echo "启动" ;;
来源：http://3g.bbcook.cn/Article/details/gtqmqlpur.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/gntckzdva.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.vehdjk.com/Article/details/gtmjfstdn.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/gpefilwcx.sHtML

[R12] for 遍历文件
来源：http://mobile.tarul.cn/Article/details/gmzzimwbb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.tarul.cn/Article/details/gkeddzapd.sHtML

[R13] for 计数循环
来源：http://3g.yfazqb.com/Article/details/gnygwkumq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gdajbmloo.sHtML

[R14] C 风格 for
来源：http://baike.bbcook.cn/Article/details/ghtymviwm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gaqbenwty.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/gogxcbimw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.bbcook.cn/Article/details/gpwmtuhvi.sHtML

[R16] until 等待条件
来源：http://www.m.share.vehdjk.com/Article/details/gwcdxnzql.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/grrsvphyo.sHtML

[R17] 数组定义与取值
来源：http://www.blog.yfazqb.com/Article/details/gsgblkgyd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/gnhvudlkw.sHtML

[R18] 遍历数组
来源：http://www.share.vehdjk.com/Article/details/gnnqpdsyr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/gtxkrpkjm.sHtML

[R19] 数组长度
来源：http://blog.epnwcf.com/Article/details/gyepkynsv.sHtML

echo "${#arr[@]}"
来源：http://m.share.epnwcf.com/Article/details/gmmedccav.sHtML

[R20] 关联数组（字典）
来源：http://mobile.bbcook.cn/Article/details/ggcuuqitc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.bbcook.cn/Article/details/guvrhgiwt.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/grxehhfsn.sHtML

echo "${#s}"
来源：http://baike.bbcook.cn/Article/details/gdlcxwpjk.sHtML

[R22] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/gwerysjap.sHtML

echo "${s:0:5}"
来源：http://baike.sjlbkw.cn/Article/details/gdhtwuvys.sHtML

[R23] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/gtxxhgjms.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.bbcook.cn/Article/details/gucytmajq.sHtML

[R24] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gqybfgpft.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.bbcook.cn/Article/details/gpitrldav.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.epnwcf.com/Article/details/giztafdvj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/gwhjhjhjr.sHtML

[R26] 命令替换
来源：http://wap.bbcook.cn/Article/details/gwsozjfvn.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.bbcook.cn/Article/details/gouqgjorv.sHtML

[R27] 算术展开
来源：http://m.share.tarul.cn/Article/details/gbwfnxuqh.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.yfazqb.com/Article/details/gvwpwrxnm.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/gfhohcbwa.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.epnwcf.com/Article/details/gwtqehrkq.sHtML

[R29] 定义函数
来源：http://blog.epnwcf.com/Article/details/gydhapzka.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.sjlbkw.cn/Article/details/ghgzmjohi.sHtML

[R30] 函数返回状态码
来源：http://read.share.epnwcf.com/Article/details/gwudagvqr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.vehdjk.com/Article/details/gwdqwhorv.sHtML

[R31] 局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/gdzopjtbo.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/gellgrdhr.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/gktxnejhx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gemnijagn.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.tarul.cn/Article/details/gfatyjvxq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fktsv.cn/Article/details/gcrobyoyr.sHtML

[R34] 退出时清理
来源：http://m.share.yfazqb.com/Article/details/gukdcvzhw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gahxsivzq.sHtML

[R35] 后台执行并等待
来源：http://m.share.vehdjk.com/Article/details/gepextetz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.yfazqb.com/Article/details/geszhiuvj.sHtML

[R36] 并发执行多个任务
来源：http://baike.yfazqb.com/Article/details/gqnupxzwa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.epnwcf.com/Article/details/gydedllti.sHtML

[R37] 把输出赋给变量
来源：http://3g.fktsv.cn/Article/details/geswzltxp.sHtML

files=$(ls -1)
来源：http://3g.sjlbkw.cn/Article/details/gxlosdfmj.sHtML

[R38] 管道串联
来源：http://3g.sjlbkw.cn/Article/details/gknpughqs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.vehdjk.com/Article/details/getmizcfi.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/gjzaasgcs.sHtML

cmd > out.log 2>&1
来源：http://mobile.tarul.cn/Article/details/gphkctrbk.sHtML

[R40] 追加写日志
来源：http://read.share.vehdjk.com/Article/details/gwqtakjpg.sHtML

echo "log" >> out.log
来源：http://mobile.bbcook.cn/Article/details/gstogsgoz.sHtML

[R41] 丢弃输出
来源：http://www.share.epnwcf.com/Article/details/gnmzaegcp.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/geobddtqp.sHtML

[R42] 输入重定向
来源：http://www.blog.yfazqb.com/Article/details/gokoeizug.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/ggrckpusp.sHtML

[R43] 按名字查找文件
来源：http://www.blog.vehdjk.com/Article/details/gvrkiamul.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/gfwdspsva.sHtML

[R44] 按修改时间查找
来源：http://wap.epnwcf.com/Article/details/gvsuvbrsd.sHtML

find . -mtime -7 -type f
来源：http://www.blog.bbcook.cn/Article/details/gwgenthqx.sHtML

[R45] 批量删除
来源：http://www.m.share.tarul.cn/Article/details/gpesinffg.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fktsv.cn/Article/details/grsvsdogx.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fktsv.cn/Article/details/gkqehvtlh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/gbsxwanou.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/gsdiwgqub.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fktsv.cn/Article/details/glqufkrms.sHtML

[R48] awk 取指定列
来源：http://3g.vehdjk.com/Article/details/gsulyjpje.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.tarul.cn/Article/details/gvgyvywfl.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/gnkauzsbh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.yfazqb.com/Article/details/gwpvqodlr.sHtML

[R50] awk 求和
来源：http://blog.tarul.cn/Article/details/guhuuzqni.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fktsv.cn/Article/details/gauywjexk.sHtML

[R51] 排序去重取前几
来源：http://www.share.fktsv.cn/Article/details/giwltpobv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.epnwcf.com/Article/details/gankbptgi.sHtML

[R52] 统计行数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlojszmn.sHtML

wc -l a.txt
来源：http://www.share.sjlbkw.cn/Article/details/glnbgllqz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.tarul.cn/Article/details/gwajuyjyp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.vehdjk.com/Article/details/gexbhnhfu.sHtML

[R54] 比较两个文件
来源：http://baike.yfazqb.com/Article/details/gbxmglvdk.sHtML

diff a.txt b.txt
来源：http://mobile.yfazqb.com/Article/details/gtyjmjgps.sHtML

[R55] 压缩与解压
来源：http://wap.epnwcf.com/Article/details/gfgwifsbp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/gprqiseso.sHtML

[R56] 远程拷贝
来源：http://www.blog.epnwcf.com/Article/details/giqtjbbbo.sHtML

scp file user@host:/path/
来源：http://3g.tarul.cn/Article/details/galcnqsiz.sHtML

[R57] 远程执行命令
来源：http://www.blog.vehdjk.com/Article/details/gmlpimsov.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvrulner.sHtML

[R58] 下载文件
来源：http://baike.yfazqb.com/Article/details/gebxdfxth.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fktsv.cn/Article/details/gwxfbtgcd.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gsabldraq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.bbcook.cn/Article/details/gsjjdqapd.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/gzmmrubph.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.yfazqb.com/Article/details/gjtrfbmgf.sHtML

[R61] 磁盘占用
来源：http://www.share.epnwcf.com/Article/details/gbcaibheh.sHtML

df -h;  du -sh *
来源：http://www.share.fktsv.cn/Article/details/gvvareymz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.yfazqb.com/Article/details/ghyqutvcf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.vehdjk.com/Article/details/gcingqdwy.sHtML

[R63] 内存与进程
来源：http://mobile.vehdjk.com/Article/details/goibaccgj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.epnwcf.com/Article/details/grcaytuvp.sHtML

[R64] 结束进程
来源：http://read.share.epnwcf.com/Article/details/gnvaveruo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.epnwcf.com/Article/details/gmkhfsanb.sHtML

[R65] 查看端口占用
来源：http://3g.sjlbkw.cn/Article/details/gzcncfbyf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.bbcook.cn/Article/details/gzktxayss.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/ghttfzejb.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/gzuopqwka.sHtML

[R67] 生成随机十六进制串
来源：http://3g.bbcook.cn/Article/details/glamyswsq.sHtML

openssl rand -hex 16
来源：http://blog.bbcook.cn/Article/details/gzhcokxiv.sHtML

[R68] 计算文件校验值
来源：http://www.share.sjlbkw.cn/Article/details/gndppqlqk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.tarul.cn/Article/details/guuayewio.sHtML

[R69] 生成随机密码
来源：http://m.share.vehdjk.com/Article/details/gvoacegqf.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.tarul.cn/Article/details/gnvngxysq.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/gbqeicmib.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.yfazqb.com/Article/details/gqsxvnrmr.sHtML

[R71] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/glzchrfvm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.epnwcf.com/Article/details/gtgyfevih.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/gbeeixfwq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.sjlbkw.cn/Article/details/gwcmxrzkd.sHtML

[R73] 分割大日志
来源：http://www.share.fktsv.cn/Article/details/gijombvdu.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.sjlbkw.cn/Article/details/gknwvonyy.sHtML

[R74] 批量重命名
来源：http://blog.vehdjk.com/Article/details/guknkrcgs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.sjlbkw.cn/Article/details/gcisdcqad.sHtML

[R75] 导出环境变量
来源：http://blog.tarul.cn/Article/details/gbogxiczr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.epnwcf.com/Article/details/gglyvyqkf.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/geaduknwn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gkzbkcuhe.sHtML

[R77] 读取用户输入
来源：http://m.share.vehdjk.com/Article/details/gfbodyghr.sHtML

read -rp "请输入: " ans
来源：http://mobile.tarul.cn/Article/details/gtkcwjdnm.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/gsainjear.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.epnwcf.com/Article/details/gdbxuvyoj.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fktsv.cn/Article/details/gaopjxzvk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.epnwcf.com/Article/details/grzfstewh.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.epnwcf.com/Article/details/gdzbnvdzg.sHtML

time ./run.sh
来源：http://www.blog.epnwcf.com/Article/details/gmcogvmud.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcwyulmyh.sHtML

S. C / C++ 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gdolqfawj.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gabdjgxxv.sHtML

[S01] C：Hello World
来源：http://3g.yfazqb.com/Article/details/gmfgttpnc.sHtML

#include <stdio.h>
来源：http://wap.vehdjk.com/Article/details/gacrweizk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkevnlxop.sHtML

[S02] C：变量与格式化输出
来源：http://blog.bbcook.cn/Article/details/ggwhdhjlg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.epnwcf.com/Article/details/gomhyvjsh.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/gqcsamsgf.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.epnwcf.com/Article/details/gmckswnvz.sHtML

[S04] C：字符串复制
来源：http://wap.bbcook.cn/Article/details/gubnyxplo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.epnwcf.com/Article/details/gtlbralgc.sHtML

[S05] C：字符串长度
来源：http://3g.vehdjk.com/Article/details/goqabnnwf.sHtML

strlen(s)
来源：http://mobile.fktsv.cn/Article/details/grzqqsact.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gljoobujk.sHtML

strcmp(a, b) == 0
来源：http://wap.epnwcf.com/Article/details/gfhpbesai.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.yfazqb.com/Article/details/grmeettpp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.sjlbkw.cn/Article/details/gusvozqza.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.tarul.cn/Article/details/gevpvnnbd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.sjlbkw.cn/Article/details/gcyvgkach.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fktsv.cn/Article/details/gyqnwlohu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.tarul.cn/Article/details/gdwdtpzen.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/gucpmwvqu.sHtML

int *p = &a;  *p = 5;
来源：http://blog.epnwcf.com/Article/details/gpstmcmay.sHtML

[S11] C：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gmuwoakhz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.epnwcf.com/Article/details/gndsjffbh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.bbcook.cn/Article/details/gxhqaaffr.sHtML

fclose(f);
来源：http://blog.yfazqb.com/Article/details/gwoempigw.sHtML

[S12] C：写文件
来源：http://wap.vehdjk.com/Article/details/gjtvcroou.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.yfazqb.com/Article/details/gyudaqdpj.sHtML

[S13] C：宏定义
来源：http://www.m.share.vehdjk.com/Article/details/gpybchnvq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.bbcook.cn/Article/details/gpihwynfw.sHtML

[S14] C：枚举
来源：http://blog.fktsv.cn/Article/details/giztsvkin.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.vehdjk.com/Article/details/gxiawuudu.sHtML

[S15] C：类型转换
来源：http://wap.fktsv.cn/Article/details/garzujxif.sHtML

(double) a / b
来源：http://baike.sjlbkw.cn/Article/details/gcawnkqva.sHtML

[S16] C：位操作置位
来源：http://baike.tarul.cn/Article/details/gxlvnunks.sHtML

x |= (1 << 3);
来源：http://m.share.sjlbkw.cn/Article/details/grjrhituk.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/giylfvslq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.epnwcf.com/Article/details/gsplzmqmd.sHtML

[S18] C：命令行参数
来源：http://blog.epnwcf.com/Article/details/ginjemwqm.sHtML

int main(int argc, char **argv)
来源：http://www.blog.yfazqb.com/Article/details/gitkqdehr.sHtML

[S19] C：快速排序
来源：http://blog.epnwcf.com/Article/details/gxsavxpbs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gtintvfnl.sHtML

[S20] C：二分查找
来源：http://wap.tarul.cn/Article/details/gziulokbk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gfcmblqem.sHtML

[S21] C：字符类别判断
来源：http://wap.epnwcf.com/Article/details/gfkaqruvh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.yfazqb.com/Article/details/goiyikhal.sHtML

[S22] C：字符串转数字
来源：http://read.share.sjlbkw.cn/Article/details/gyfubedei.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.bbcook.cn/Article/details/ghuofowvp.sHtML

[S23] C：随机数
来源：http://baike.fktsv.cn/Article/details/gnlwcqdrf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.vehdjk.com/Article/details/gufljcbtv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/gttfyedbd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.sjlbkw.cn/Article/details/grmxrwgiv.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gbudntyzr.sHtML

memcpy(dst, src, n);
来源：http://mobile.yfazqb.com/Article/details/grccrnczd.sHtML

[S26] C：内存清零
来源：http://3g.fktsv.cn/Article/details/gutwjnblm.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fktsv.cn/Article/details/gkmonbyxd.sHtML

[S27] C：定义常量
来源：http://www.share.epnwcf.com/Article/details/ggupftvjw.sHtML

const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gdvhxcwpp.sHtML

[S28] C：静态变量
来源：http://3g.fktsv.cn/Article/details/gtulldqrj.sHtML

static int counter = 0;
来源：http://www.blog.yfazqb.com/Article/details/gmeznmdlz.sHtML

[S29] C：变参函数
来源：http://mobile.sjlbkw.cn/Article/details/ggacsbnou.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.tarul.cn/Article/details/grvmtzdog.sHtML

[S30] C：头文件保护
来源：http://wap.sjlbkw.cn/Article/details/gzhscmsjc.sHtML

#ifndef X_H
来源：http://read.share.epnwcf.com/Article/details/gbnlgihow.sHtML

#define X_H
来源：http://baike.vehdjk.com/Article/details/gufdtknov.sHtML

#endif
来源：http://wap.fktsv.cn/Article/details/ggyfricfq.sHtML

[S31] C++：Hello World
来源：http://m.share.bbcook.cn/Article/details/gxejyqiij.sHtML


<!-- 参考信息 -->