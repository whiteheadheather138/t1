代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/gxugwwcll.sHtML

[Q54] 清空表
来源：http://www.blog.vehdjk.com/Article/details/gyyhlwutz.sHtML

TRUNCATE TABLE logs;
来源：http://blog.vehdjk.com/Article/details/gawfmisuw.sHtML

[Q55] 排名（并列占位）
来源：http://wap.yfazqb.com/Article/details/gcawdkboz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gmvbkeyko.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.sjlbkw.cn/Article/details/gvxcwlvaw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fktsv.cn/Article/details/glkfftvol.sHtML

[Q57] 行号
来源：http://read.share.vehdjk.com/Article/details/guhlkgich.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.bbcook.cn/Article/details/gnawynmjf.sHtML

[Q58] 累计求和
来源：http://www.m.share.yfazqb.com/Article/details/grpsnfgek.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gwoxywxdp.sHtML

[Q59] 分组内累计
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjvojhvi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gobbhphoa.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fktsv.cn/Article/details/gdnbwqioz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.epnwcf.com/Article/details/goduwybvs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gpmjhwihb.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/gtqtwigwo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/glnakendv.sHtML

[Q62] 分组占比
来源：http://www.m.share.bbcook.cn/Article/details/gmnlglncf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gcwojdqgy.sHtML

[Q63] 开启事务
来源：http://mobile.vehdjk.com/Article/details/gegokymuc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.yfazqb.com/Article/details/gumnqzhex.sHtML

[Q64] 提交事务
来源：http://www.share.bbcook.cn/Article/details/grmhcastf.sHtML

COMMIT;
来源：http://wap.epnwcf.com/Article/details/gefjdlrif.sHtML

[Q65] 回滚事务
来源：http://www.share.fktsv.cn/Article/details/gonfdrumt.sHtML

ROLLBACK;
来源：http://mobile.vehdjk.com/Article/details/gsbijsmsh.sHtML

[Q66] 行锁查询
来源：http://3g.vehdjk.com/Article/details/gtaqesavv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.bbcook.cn/Article/details/gkxakghns.sHtML

[Q67] 设置隔离级别
来源：http://blog.yfazqb.com/Article/details/gopewofdt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.yfazqb.com/Article/details/gduoegikd.sHtML

[Q68] 保存点
来源：http://www.m.share.tarul.cn/Article/details/gvbsegojy.sHtML

SAVEPOINT sp1;
来源：http://m.share.yfazqb.com/Article/details/gessvhkqa.sHtML

ROLLBACK TO sp1;
来源：http://wap.fktsv.cn/Article/details/glhjjmkhp.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.epnwcf.com/Article/details/gkhakhngr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyzzbszq.sHtML

[Q70] 更新统计信息
来源：http://www.share.yfazqb.com/Article/details/gdcteoaos.sHtML

ANALYZE TABLE users;
来源：http://3g.bbcook.cn/Article/details/gjpwgpjfj.sHtML

[Q71] 查看建表语句
来源：http://read.share.fktsv.cn/Article/details/ggbyiqthi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.bbcook.cn/Article/details/gijnspcla.sHtML

[Q72] 查看索引
来源：http://read.share.vehdjk.com/Article/details/gdhbdlndy.sHtML

SHOW INDEX FROM users;
来源：http://3g.bbcook.cn/Article/details/gqajrgeis.sHtML

[Q73] 查看表状态
来源：http://www.blog.tarul.cn/Article/details/gseblylev.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.tarul.cn/Article/details/ggpclmnqx.sHtML

[Q74] 强制使用索引
来源：http://www.blog.vehdjk.com/Article/details/ggzfbovpb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.bbcook.cn/Article/details/gxqguhvue.sHtML

[Q75] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gevafwsxf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/giuorjtni.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.epnwcf.com/Article/details/geidqrhcr.sHtML

[Q76] 按天统计
来源：http://www.blog.fktsv.cn/Article/details/gvrqhmupc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fktsv.cn/Article/details/gkemxdxly.sHtML

[Q77] 时间加减
来源：http://blog.bbcook.cn/Article/details/gflcegjbh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.epnwcf.com/Article/details/gleaxbnhs.sHtML

[Q78] 当前时间
来源：http://www.share.fktsv.cn/Article/details/gntjocbgi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.epnwcf.com/Article/details/gehpuorzf.sHtML

[Q79] 字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gnboojzir.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.yfazqb.com/Article/details/gxxtxgsvd.sHtML

[Q80] 字符串截取
来源：http://read.share.epnwcf.com/Article/details/gubdymotk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gsyjpjftu.sHtML

[Q81] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/geisadyli.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.bbcook.cn/Article/details/gertmvppn.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.sjlbkw.cn/Article/details/gjnskbejq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gcfcdpvnj.sHtML

[Q83] 大小写转换
来源：http://baike.tarul.cn/Article/details/gdsqhiaoc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gbwynbula.sHtML

[Q84] 去除首尾空格
来源：http://mobile.sjlbkw.cn/Article/details/gvmpdumff.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gdmfhxmne.sHtML

[Q85] 数值取整
来源：http://m.share.yfazqb.com/Article/details/gqomxqofx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.vehdjk.com/Article/details/gjhitscku.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.sjlbkw.cn/Article/details/grhdcyxpb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.bbcook.cn/Article/details/gjmrslwlr.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.sjlbkw.cn/Article/details/glhyolixa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.tarul.cn/Article/details/gyuikwetb.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.sjlbkw.cn/Article/details/ghouqtsae.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.epnwcf.com/Article/details/gdwuwsyyu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gfwhofuod.sHtML

[Q89] 判断表是否存在
来源：http://baike.bbcook.cn/Article/details/gdgpfugct.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.sjlbkw.cn/Article/details/gdixvacvj.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fktsv.cn/Article/details/gwtdiyqxb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.vehdjk.com/Article/details/gamtsndyp.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gpumtfkog.sHtML

R. Bash 专题
来源：http://blog.epnwcf.com/Article/details/gobdrbjlf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmyncxjoz.sHtML

[R01] shebang 与严格模式
来源：http://m.share.yfazqb.com/Article/details/gygzctcyc.sHtML

#!/usr/bin/env bash
来源：http://wap.bbcook.cn/Article/details/girlqodpr.sHtML

set -euo pipefail
来源：http://www.share.epnwcf.com/Article/details/grviysnbi.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.vehdjk.com/Article/details/gnxipsjqd.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fktsv.cn/Article/details/gjjsnvzaz.sHtML

[R03] 只读变量
来源：http://m.share.vehdjk.com/Article/details/gdupiklhi.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/gnkpzzwky.sHtML

[R04] 位置参数
来源：http://m.share.epnwcf.com/Article/details/gseotbaio.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fktsv.cn/Article/details/gwrfvpznw.sHtML

[R05] 参数默认值
来源：http://www.share.epnwcf.com/Article/details/gtxzjpemm.sHtML

name="${1:-default}"
来源：http://blog.sjlbkw.cn/Article/details/gmjtqhtpo.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fktsv.cn/Article/details/gyzeoxrjc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gpvqhvdpv.sHtML

[R07] if 判断文件
来源：http://baike.tarul.cn/Article/details/gdellpnhy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.vehdjk.com/Article/details/gepuobebm.sHtML

[R08] 数值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gahwsemuw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.vehdjk.com/Article/details/gekzstkak.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gafdigbsr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gwctwdibs.sHtML

[R10] 正则匹配
来源：http://www.m.share.tarul.cn/Article/details/gpizvhkgw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.yfazqb.com/Article/details/gzzyubywi.sHtML

[R11] case 多分支
来源：http://www.blog.bbcook.cn/Article/details/girksikvy.sHtML

case "$1" in
来源：http://read.share.sjlbkw.cn/Article/details/gafbsisfk.sHtML

start) echo "启动" ;;
来源：http://www.blog.tarul.cn/Article/details/gjmmcyjri.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fktsv.cn/Article/details/gvzhngsya.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.vehdjk.com/Article/details/gvvqaxayh.sHtML

esac
来源：http://www.blog.vehdjk.com/Article/details/gctbqcxid.sHtML

[R12] for 遍历文件
来源：http://blog.bbcook.cn/Article/details/gctgidxcf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.vehdjk.com/Article/details/gefxsnqcf.sHtML

[R13] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/gmmyyjodd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/ganpyrtxd.sHtML

[R14] C 风格 for
来源：http://mobile.tarul.cn/Article/details/ggpcbfevw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.yfazqb.com/Article/details/gyhmqdrkg.sHtML

[R15] while 逐行读文件
来源：http://wap.yfazqb.com/Article/details/gxhgvyhux.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.bbcook.cn/Article/details/gqbtgimgc.sHtML

[R16] until 等待条件
来源：http://m.share.tarul.cn/Article/details/gmktdmerq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/govtqjdfw.sHtML

[R17] 数组定义与取值
来源：http://blog.yfazqb.com/Article/details/gfdbbnjak.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fktsv.cn/Article/details/gwjedbruf.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/gecvkcuay.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.vehdjk.com/Article/details/gksfwkisb.sHtML

[R19] 数组长度
来源：http://3g.vehdjk.com/Article/details/gxeckogpn.sHtML

echo "${#arr[@]}"
来源：http://baike.bbcook.cn/Article/details/gsszzvpav.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.sjlbkw.cn/Article/details/gfkmynhwq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fktsv.cn/Article/details/gjvlefsbu.sHtML

[R21] 字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gjijymors.sHtML

echo "${#s}"
来源：http://read.share.vehdjk.com/Article/details/gljgraovh.sHtML

[R22] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/gbryhcecd.sHtML

echo "${s:0:5}"
来源：http://www.blog.tarul.cn/Article/details/gdfwvzpsf.sHtML

[R23] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gpsmwmjpy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.yfazqb.com/Article/details/gkswsjmce.sHtML

[R24] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gznxooxts.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.epnwcf.com/Article/details/gxrubdijz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gxdusyrzd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/gpgiaklgx.sHtML

[R26] 命令替换
来源：http://blog.epnwcf.com/Article/details/gmzuetbkd.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fktsv.cn/Article/details/gyghhsehm.sHtML

[R27] 算术展开
来源：http://3g.yfazqb.com/Article/details/gceerdpoy.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.bbcook.cn/Article/details/gzzmzdiuv.sHtML

[R28] 浮点运算
来源：http://www.m.share.fktsv.cn/Article/details/goxxqpsdt.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.bbcook.cn/Article/details/gtncycsvc.sHtML

[R29] 定义函数
来源：http://blog.yfazqb.com/Article/details/gpkwtstwu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.bbcook.cn/Article/details/gcobjiqki.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gdrysszrs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.bbcook.cn/Article/details/gqtivkqvt.sHtML

[R31] 局部变量
来源：http://www.share.fktsv.cn/Article/details/ggaxldeys.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.bbcook.cn/Article/details/gtimarxpi.sHtML

[R32] 参数个数校验
来源：http://www.m.share.tarul.cn/Article/details/gzfgwtojg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gkgkutvld.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.vehdjk.com/Article/details/gwhfpgxcf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/gfkfbnadb.sHtML

[R34] 退出时清理
来源：http://www.m.share.yfazqb.com/Article/details/gjhubhdvv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gsgmettzr.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/ggrpegclv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.vehdjk.com/Article/details/glrabsnze.sHtML

[R36] 并发执行多个任务
来源：http://blog.sjlbkw.cn/Article/details/gnamtuxwh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/gxfsevkul.sHtML

[R37] 把输出赋给变量
来源：http://3g.yfazqb.com/Article/details/gqvavnqlp.sHtML

files=$(ls -1)
来源：http://www.share.bbcook.cn/Article/details/grjtnrkdc.sHtML

[R38] 管道串联
来源：http://blog.yfazqb.com/Article/details/gsezyzgib.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.vehdjk.com/Article/details/gpfbdlays.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.bbcook.cn/Article/details/gmiyqdjrj.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/ggijfcsgh.sHtML

[R40] 追加写日志
来源：http://wap.epnwcf.com/Article/details/gchnwpgnk.sHtML

echo "log" >> out.log
来源：http://www.blog.bbcook.cn/Article/details/gwoxdgkxm.sHtML

[R41] 丢弃输出
来源：http://mobile.sjlbkw.cn/Article/details/gvqykrnaf.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fktsv.cn/Article/details/geuompyqb.sHtML

[R42] 输入重定向
来源：http://www.m.share.tarul.cn/Article/details/gflcjwjdo.sHtML

wc -l < a.txt
来源：http://www.share.epnwcf.com/Article/details/gtvwuzqai.sHtML

[R43] 按名字查找文件
来源：http://mobile.epnwcf.com/Article/details/glrkkqvhk.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.bbcook.cn/Article/details/ggbovkmda.sHtML

[R44] 按修改时间查找
来源：http://3g.yfazqb.com/Article/details/grnqvtdxd.sHtML

find . -mtime -7 -type f
来源：http://mobile.bbcook.cn/Article/details/gqbfveylu.sHtML

[R45] 批量删除
来源：http://blog.bbcook.cn/Article/details/gsgjawmyd.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/grqxnlalc.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.tarul.cn/Article/details/gafxfthfa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/groasskyk.sHtML

[R47] sed 单行替换
来源：http://read.share.vehdjk.com/Article/details/gtnflvosf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fktsv.cn/Article/details/geegtkznz.sHtML

[R48] awk 取指定列
来源：http://www.blog.bbcook.cn/Article/details/gvqljvnms.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gfuwadzkb.sHtML

[R49] awk 带条件
来源：http://www.share.sjlbkw.cn/Article/details/grzhfwlyz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fktsv.cn/Article/details/gmjksldvt.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/ghxdxdddg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fktsv.cn/Article/details/gkqdfeitu.sHtML

[R51] 排序去重取前几
来源：http://www.share.epnwcf.com/Article/details/gbuhhwshh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.epnwcf.com/Article/details/gsuadgatt.sHtML

[R52] 统计行数
来源：http://read.share.yfazqb.com/Article/details/gzorwjosw.sHtML

wc -l a.txt
来源：http://baike.vehdjk.com/Article/details/gprrazuys.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fktsv.cn/Article/details/gmgpypins.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gfbaghmpr.sHtML

[R54] 比较两个文件
来源：http://3g.sjlbkw.cn/Article/details/gdjxowujt.sHtML

diff a.txt b.txt
来源：http://blog.fktsv.cn/Article/details/gzakkqjlr.sHtML

[R55] 压缩与解压
来源：http://mobile.tarul.cn/Article/details/glhgmnyci.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fktsv.cn/Article/details/gsavjdnfw.sHtML

[R56] 远程拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gcggavtcf.sHtML

scp file user@host:/path/
来源：http://mobile.vehdjk.com/Article/details/gupsdxpma.sHtML

[R57] 远程执行命令
来源：http://wap.vehdjk.com/Article/details/gddewksvk.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/goapqivrl.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gabwxiyox.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.epnwcf.com/Article/details/gnbynoofp.sHtML

[R59] 发 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gvsutdyoi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.epnwcf.com/Article/details/gazobrhcs.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gjyycbqtd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.bbcook.cn/Article/details/gskuxyfff.sHtML

[R61] 磁盘占用
来源：http://www.blog.bbcook.cn/Article/details/gzkzsestk.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/gvduuznux.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/grzfgxiep.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.vehdjk.com/Article/details/gkltosmzr.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gyropostg.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fktsv.cn/Article/details/geksxrytj.sHtML

[R64] 结束进程
来源：http://blog.tarul.cn/Article/details/gfpwsankv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.tarul.cn/Article/details/ggopduubq.sHtML

[R65] 查看端口占用
来源：http://baike.fktsv.cn/Article/details/gwhycioef.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.vehdjk.com/Article/details/ghbiatsoq.sHtML

[R66] 定时任务
来源：http://3g.tarul.cn/Article/details/gbupzftmr.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/gllambbvm.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.bbcook.cn/Article/details/gyqjwjmdp.sHtML

openssl rand -hex 16
来源：http://blog.sjlbkw.cn/Article/details/gshotvafd.sHtML

[R68] 计算文件校验值
来源：http://baike.tarul.cn/Article/details/gfjwqqjyz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.yfazqb.com/Article/details/geoiqagpg.sHtML

[R69] 生成随机密码
来源：http://blog.bbcook.cn/Article/details/gitjslmsi.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.sjlbkw.cn/Article/details/gcbdhhvld.sHtML

[R70] 时间戳与互转
来源：http://3g.epnwcf.com/Article/details/gotrzovtm.sHtML

date +%s;  date -d @1700000000
来源：http://blog.epnwcf.com/Article/details/gfeaeayko.sHtML

[R71] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gncwashqc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.yfazqb.com/Article/details/grrdcuwyl.sHtML

[R72] 等待端口就绪
来源：http://baike.bbcook.cn/Article/details/gwhrvicyg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpkddvrw.sHtML

[R73] 分割大日志
来源：http://blog.vehdjk.com/Article/details/geseuubpz.sHtML

split -l 1000 big.log part_
来源：http://www.blog.vehdjk.com/Article/details/gmytmkgme.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/guxobipep.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.yfazqb.com/Article/details/gxtiwrhop.sHtML

[R75] 导出环境变量
来源：http://www.blog.fktsv.cn/Article/details/gyguolcnh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.sjlbkw.cn/Article/details/grkbibfrb.sHtML

[R76] 使用临时文件
来源：http://read.share.epnwcf.com/Article/details/gjdyylenu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/ghqemwszq.sHtML

[R77] 读取用户输入
来源：http://read.share.vehdjk.com/Article/details/gutjolupg.sHtML

read -rp "请输入: " ans
来源：http://www.share.fktsv.cn/Article/details/gtzvssdmm.sHtML

[R78] 交互式菜单
来源：http://wap.yfazqb.com/Article/details/gijsercoc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.vehdjk.com/Article/details/ggttlacfn.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fktsv.cn/Article/details/ggibvshng.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.epnwcf.com/Article/details/gjapwdpeq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.tarul.cn/Article/details/gndbvostv.sHtML

time ./run.sh
来源：http://m.share.sjlbkw.cn/Article/details/gvarecbjw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfamutobh.sHtML

S. C / C++ 专题
来源：http://www.share.sjlbkw.cn/Article/details/ghncwawat.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gczufpnpb.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/ggdweennk.sHtML

#include <stdio.h>
来源：http://www.m.share.fktsv.cn/Article/details/gtsazgzdr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.vehdjk.com/Article/details/gxwyednyg.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fktsv.cn/Article/details/gbdaqtzzj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fktsv.cn/Article/details/gvmblhmlq.sHtML

[S03] C：读入整数
来源：http://3g.vehdjk.com/Article/details/gljzpmgai.sHtML

int x; scanf("%d", &x);
来源：http://read.share.bbcook.cn/Article/details/gfutmljfu.sHtML

[S04] C：字符串复制
来源：http://read.share.sjlbkw.cn/Article/details/gpcimhuxi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.vehdjk.com/Article/details/gtktadqvl.sHtML

[S05] C：字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gnxjsarbr.sHtML

strlen(s)
来源：http://mobile.tarul.cn/Article/details/garjhcstz.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/gaqkztkch.sHtML

strcmp(a, b) == 0
来源：http://www.blog.yfazqb.com/Article/details/gugivyisg.sHtML

[S07] C：数组遍历求和
来源：http://m.share.sjlbkw.cn/Article/details/gweccmgsh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.sjlbkw.cn/Article/details/grfsnolop.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.yfazqb.com/Article/details/ggabufpvz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.tarul.cn/Article/details/gzeyghsrp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.bbcook.cn/Article/details/gmxkfcwbc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/geeygigzx.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gxxcueyyc.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/glerdethb.sHtML

[S11] C：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gcubusfto.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.vehdjk.com/Article/details/ghwplxbow.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlfzfblh.sHtML

fclose(f);
来源：http://m.share.tarul.cn/Article/details/gqkitqeox.sHtML

[S12] C：写文件
来源：http://www.blog.tarul.cn/Article/details/gahbbshbn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fktsv.cn/Article/details/geajsmoav.sHtML

[S13] C：宏定义
来源：http://mobile.sjlbkw.cn/Article/details/gpuevnrux.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.epnwcf.com/Article/details/gvuehhkcr.sHtML

[S14] C：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gkprmjvva.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fktsv.cn/Article/details/gdlbnkzvk.sHtML

[S15] C：类型转换
来源：http://www.share.vehdjk.com/Article/details/gazxjlyje.sHtML

(double) a / b
来源：http://read.share.sjlbkw.cn/Article/details/ghlagwocu.sHtML

[S16] C：位操作置位
来源：http://baike.bbcook.cn/Article/details/gaenxkwyj.sHtML

x |= (1 << 3);
来源：http://www.m.share.tarul.cn/Article/details/gxnppnvxi.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/genzghbrv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fktsv.cn/Article/details/gqjbdbyug.sHtML

[S18] C：命令行参数
来源：http://www.share.yfazqb.com/Article/details/gxhbmgrnf.sHtML

int main(int argc, char **argv)
来源：http://baike.vehdjk.com/Article/details/gguqfgdei.sHtML

[S19] C：快速排序
来源：http://read.share.sjlbkw.cn/Article/details/gypricdws.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/goqbzoluq.sHtML

[S20] C：二分查找
来源：http://m.share.vehdjk.com/Article/details/gtpmssubu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/geiozxohw.sHtML

[S21] C：字符类别判断
来源：http://www.share.bbcook.cn/Article/details/grviyujvu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.yfazqb.com/Article/details/gujkhzggu.sHtML

[S22] C：字符串转数字
来源：http://mobile.vehdjk.com/Article/details/gkwucvbvt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.vehdjk.com/Article/details/glrtcdnze.sHtML

[S23] C：随机数
来源：http://mobile.sjlbkw.cn/Article/details/gzjyspwso.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.yfazqb.com/Article/details/ghkkrszho.sHtML

[S24] C：获取本地时间
来源：http://www.blog.tarul.cn/Article/details/gulxflwuh.sHtML


<!-- 参考信息 -->