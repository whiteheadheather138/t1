代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ndf.shanyushiyangtech.top

[Q20] IN 列表
来源：http://var.aizwys.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hnd.shzxlz.cn

[Q21] 空值判断
来源：http://pyc.fanxiaobao.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://pzc.yueranfly.top

[Q22] 排序
来源：http://bto.fktsv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tow.hnxiangtu.top

[Q23] 分页
来源：http://crz.mhx1999.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vfm.dianchejie.cn

[Q24] 去重
来源：http://yid.ivvv.top

SELECT DISTINCT city FROM users;
来源：http://pxn.sufxvd.cn

[Q25] 只取前 N 条
来源：http://gru.nanxuanxn.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://obw.birdmap.top

[Q26] 计数
来源：http://efn.guowangkeji.top

SELECT COUNT(*) FROM users;
来源：http://ikm.hysaishi.cn

[Q27] 条件计数
来源：http://ugd.ybcxt.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nzq.sjlbkw.cn

[Q28] 求和与平均
来源：http://ruf.epnwcf.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sev.zhengqikj.top

[Q29] 最大最小值
来源：http://qdj.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ltg.fktsv.cn

[Q30] 分组统计
来源：http://bhu.meibo888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vsr.sweek.top

[Q31] 分组后过滤
来源：http://mby.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rxg.vqdsnc.cn

[Q32] 分组拼接字符串
来源：http://hli.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bsj.sysykeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nay.svipenyu.cn

[Q33] 多列分组
来源：http://iqm.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aub.mhx1999.top

[Q34] 每组取第一条
来源：http://bix.fktsv.cn

SELECT * FROM (
来源：http://pir.yj20258888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ddi.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://osk.jinqigfzy.top

[Q35] 内连接
来源：http://pvr.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ahv.zycfv.cn

[Q36] 左连接
来源：http://eom.jinqigfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fix.aibaodan.cn

[Q37] 右连接
来源：http://wvb.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rob.fanxiaobao.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://lfw.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://inc.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://ijn.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://nbi.fzhhl.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zuf.ctjpmb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://hvd.birdmap.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://buu.nwbrower.top

[Q41] 多表连接
来源：http://exy.jinqigufen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cvc.mhx1999.top

JOIN users u ON u.id = o.user_id
来源：http://elx.cucudq.cn

JOIN products p ON p.id = o.product_id;
来源：http://blp.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://ino.jyoumei.cn

SELECT u.name, o.amount FROM users u
来源：http://hhd.wangdashe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://std.jinghuilouyu.cn

[Q43] 标量子查询
来源：http://mrs.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://obr.zhoulong.xyz

[Q44] IN 子查询
来源：http://yno.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eig.tian-w.cn

[Q45] EXISTS 判断存在
来源：http://bie.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mbv.gotoacloud.top

[Q46] NOT EXISTS 判断不存在
来源：http://jqv.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pxk.ydzc1.top

[Q47] 与平均值比较
来源：http://cce.redwolf501.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qbd.yfazqb.com

[Q48] CTE 公用表表达式
来源：http://ndu.dashuyun.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cqq.zycfv.cn

SELECT * FROM t WHERE c > 5;
来源：http://umh.yfazqb.com

[Q49] 更新单行
来源：http://vif.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bni.hnqzz.top

[Q50] 批量更新
来源：http://odw.316326.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zii.gaohongyu789.top

[Q51] 用子查询更新
来源：http://kmv.wangdashe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oqm.yj20258888.top

[Q52] 删除指定行
来源：http://wos.snrcjt.cn

DELETE FROM users WHERE id = 10;
来源：http://ybk.ehwqpu.com

[Q53] 按条件删除
来源：http://qyb.ctjpmb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hwj.cheryme.top

[Q54] 清空表
来源：http://rri.birdmap.top

TRUNCATE TABLE logs;
来源：http://ndz.jianghu66.top

[Q55] 排名（并列占位）
来源：http://jua.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://weh.tianlin.xyz

[Q56] 密集排名（并列不占位）
来源：http://ieo.ybcxt.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://smg.sysykeji.top

[Q57] 行号
来源：http://prf.yuxming.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rke.meibo888.top

[Q58] 累计求和
来源：http://vvg.epnwcf.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dch.shzxlz.cn

[Q59] 分组内累计
来源：http://uro.wangdashe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://llk.zhiwuduotai.top

[Q60] 取上一行 / 下一行
来源：http://kxb.zhixingplan.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kqi.jqgufenzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bks.tian-w.cn

[Q61] 移动平均
来源：http://oye.yangfankeji.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sgu.yuanzhike.top

[Q62] 分组占比
来源：http://gpc.0kj1m.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uaf.pengpengdd.cyou

[Q63] 开启事务
来源：http://qaf.hammf.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ubr.nanxinkj.top

[Q64] 提交事务
来源：http://avz.nanxuanxn.top

COMMIT;
来源：http://kes.zdqjudy.top

[Q65] 回滚事务
来源：http://hpo.shangyingyoupin.top

ROLLBACK;
来源：http://iqo.hysaishi.cn

[Q66] 行锁查询
来源：http://ook.yangfankeji.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ugq.hcnkem.com

[Q67] 设置隔离级别
来源：http://fmy.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qxt.ywan-chungtsiang.top

[Q68] 保存点
来源：http://wkm.snrcjt.cn

SAVEPOINT sp1;
来源：http://smr.ybcxt.top

ROLLBACK TO sp1;
来源：http://fwi.iojbl.cn

[Q69] 查看执行计划
来源：http://uak.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dbu.kuanghao11.cn

[Q70] 更新统计信息
来源：http://uom.xziqi.cn

ANALYZE TABLE users;
来源：http://rdi.cqqwz.cn

[Q71] 查看建表语句
来源：http://ybg.hnxiangtu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rgm.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://tqz.daria6918.cn

SHOW INDEX FROM users;
来源：http://muw.svipenyu.cn

[Q73] 查看表状态
来源：http://lca.smart0.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://atf.haohaochexian.top

[Q74] 强制使用索引
来源：http://hve.mhx1999.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zlh.shangyingyoupin.top

[Q75] 日期格式化
来源：http://zhz.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wfc.fehbvm.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://omq.tianlin.xyz

[Q76] 按天统计
来源：http://duq.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ibi.shzxlz.cn

[Q77] 时间加减
来源：http://huc.zhengqikj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sak.0kj1m.cn

[Q78] 当前时间
来源：http://wmf.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mmx.jqgfzy.top

[Q79] 字符串拼接
来源：http://ywh.0kj1m.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://scd.shangyingyoupin.top

[Q80] 字符串截取
来源：http://eba.sufxvd.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mns.hywenlv.cn

[Q81] 字符串替换
来源：http://jbe.bjfxy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iaf.yangfankeji.com

[Q82] 字符长度与字节长度
来源：http://cbp.wangdashe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qck.hnxiangtu.top

[Q83] 大小写转换
来源：http://fjs.yueranfly.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eny.shangyingyoupin.top

[Q84] 去除首尾空格
来源：http://akh.jqgfzy.top

SELECT TRIM(name) FROM users;
来源：http://dmj.tarul.cn

[Q85] 数值取整
来源：http://dgq.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sgt.zhixingplan.top

[Q86] 读取 JSON 字段
来源：http://dgg.xuetiantiany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://amt.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://eop.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fgw.hywenlv.cn

[Q88] 行转列（条件聚合）
来源：http://doi.quarkkingdee.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tqr.9152youxi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gtm.tanke756.top

[Q89] 判断表是否存在
来源：http://dgh.nanxinkj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mtc.chenzaomai.com

[Q90] 生成序号列
来源：http://efc.yueranfly.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bmw.shangyingyoupin.top

================================================================================
来源：http://lnj.sjlbkw.cn

R. Bash 专题
来源：http://vas.guowangkeji.top

================================================================================
来源：http://wru.sufxvd.cn

[R01] shebang 与严格模式
来源：http://nxu.guowangkeji.top

#!/usr/bin/env bash
来源：http://tmj.gzhubu.top

set -euo pipefail
来源：http://ghv.ybcxt.top

[R02] 变量赋值与使用
来源：http://afp.svipenyu.cn

name="Tom"; echo "$name"
来源：http://xrl.zdbjq.cn

[R03] 只读变量
来源：http://gdz.mhx1999.top

readonly PI=3.14
来源：http://zps.hammf.cn

[R04] 位置参数
来源：http://prk.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://inl.wangdashe.top

[R05] 参数默认值
来源：http://fpu.chenjidiqi.icu

name="${1:-default}"
来源：http://vra.zhongyouzk.top

[R06] 判断命令是否存在
来源：http://wnt.bjfxy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ifv.nwbrower.top

[R07] if 判断文件
来源：http://sri.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yro.zhaomingkeji.xyz

[R08] 数值比较
来源：http://ofv.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hae.shangyingyoupin.top

[R09] 字符串比较
来源：http://xuu.ydzc1.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yca.hammf.cn

[R10] 正则匹配
来源：http://oij.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qct.cheryme.top

[R11] case 多分支
来源：http://kxo.wangdashe.top

case "$1" in
来源：http://vqn.xuetiantiany.cn

start) echo "启动" ;;
来源：http://pzn.andypj.xyz

stop)  echo "停止" ;;
来源：http://yug.gzhubu.top

*)     echo "未知命令" ;;
来源：http://lpz.shzxlz.cn

esac
来源：http://mvd.zhengqikj.top

[R12] for 遍历文件
来源：http://gan.feifeiyinyue.top

for f in *.txt; do echo "$f"; done
来源：http://pnb.aibaodan.cn

[R13] for 计数循环
来源：http://epl.yueranfly.top

for i in {1..10}; do echo "$i"; done
来源：http://qcu.redwolf501.top

[R14] C 风格 for
来源：http://fnx.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lfa.hfpthk.cn

[R15] while 逐行读文件
来源：http://och.shuidangran.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kgk.zdbjq.cn

[R16] until 等待条件
来源：http://nzq.epnwcf.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://swi.jinqigfzy.top

[R17] 数组定义与取值
来源：http://xbv.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://xkv.chenzaomai.com

[R18] 遍历数组
来源：http://ewo.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yav.zycfv.cn

[R19] 数组长度
来源：http://dsn.hesvh.cn

echo "${#arr[@]}"
来源：http://xoj.hysaishi.cn

[R20] 关联数组（字典）
来源：http://hhr.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gcy.xziqi.cn

[R21] 字符串长度
来源：http://wak.vehdjk.com

echo "${#s}"
来源：http://mll.zdbjq.cn

[R22] 截取子串
来源：http://gwf.hnxiangtu.top

echo "${s:0:5}"
来源：http://uky.nanxinkj.top

[R23] 字符串替换
来源：http://hro.bjfxy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://geo.cdnleiting.top

[R24] 大小写转换
来源：http://xdw.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://ngn.jqgufenzy.top

[R25] 去后缀 / 去前缀
来源：http://ftg.ctjpmb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://azv.yfazqb.com

[R26] 命令替换
来源：http://ycg.yangfankeji.com

now=$(date +%F); echo "$now"
来源：http://urs.ydzc1.top

[R27] 算术展开
来源：http://psy.nanxinkj.top

echo $((1 + 2 * 3))
来源：http://eto.bjfxy.top

[R28] 浮点运算
来源：http://wiu.zhaomingkeji.xyz

echo "scale=2; 10/3" | bc
来源：http://khx.meibo888.top

[R29] 定义函数
来源：http://kzy.guowangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://clg.pycfn.com

[R30] 函数返回状态码
来源：http://oob.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://gau.shuidangran.top

[R31] 局部变量
来源：http://zcq.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://ygt.guowangkeji.top

[R32] 参数个数校验
来源：http://iei.shanyushiyangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tlq.pengpengdd.cyou

[R33] 捕获错误并提示行号
来源：http://mwe.sxryk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jsn.daxiang520.top

[R34] 退出时清理
来源：http://hsw.gaohongyu789.top

trap 'rm -f "$tmp"' EXIT
来源：http://oix.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://naw.epnwcf.com

sleep 5 & pid=$!; wait "$pid"
来源：http://xme.jianghu66.top

[R36] 并发执行多个任务
来源：http://gog.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ybh.bbcook.cn

[R37] 把输出赋给变量
来源：http://zvj.hesvh.cn

files=$(ls -1)
来源：http://qez.jinqigfzy.top

[R38] 管道串联
来源：http://pot.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://qln.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://rma.yueranfly.top

cmd > out.log 2>&1
来源：http://jvz.yangfankeji.com

[R40] 追加写日志
来源：http://adp.chenzaomai.com

echo "log" >> out.log
来源：http://rzf.nwbrower.top

[R41] 丢弃输出
来源：http://geo.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://yjy.xziqi.cn

[R42] 输入重定向
来源：http://ity.zhengqikj.top

wc -l < a.txt
来源：http://gkm.yuxming.cn

[R43] 按名字查找文件
来源：http://swj.zhixingplan.top

find . -name "*.log" -type f
来源：http://qwc.yangfankeji.com

[R44] 按修改时间查找
来源：http://oxa.cdnleiting.top

find . -mtime -7 -type f
来源：http://aoq.smart0.xyz

[R45] 批量删除
来源：http://rwi.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://olf.fengsongda.top

[R46] 递归替换文件内容
来源：http://oag.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mqk.sjlbkw.cn

[R47] sed 单行替换
来源：http://rte.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ezn.yanxiufei.cn

[R48] awk 取指定列
来源：http://pyp.shzxlz.cn

awk '{print $1, $3}' a.txt
来源：http://zja.hesvh.cn

[R49] awk 带条件
来源：http://fvv.zhaomingkeji.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lrs.ehwqpu.com

[R50] awk 求和
来源：http://fjq.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://mle.yonumen.top

[R51] 排序去重取前几
来源：http://wok.c1oappe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://phg.jyoumei.cn

[R52] 统计行数
来源：http://zer.yj20258888.top

wc -l a.txt
来源：http://sbv.vehdjk.com

[R53] 查看文件头与实时尾
来源：http://hbp.yuanzhike.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zzl.nwbrower.top

[R54] 比较两个文件
来源：http://sxd.cucudq.cn

diff a.txt b.txt
来源：http://zgz.yueranfly.top

[R55] 压缩与解压
来源：http://mgo.quarkkingdee.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://joc.hnqzz.top

[R56] 远程拷贝
来源：http://fot.fzhhl.top

scp file user@host:/path/
来源：http://tpg.cucudq.cn

[R57] 远程执行命令
来源：http://uya.gaohongyu789.top

ssh user@host 'uptime'
来源：http://juj.shanyushiyangtech.top

[R58] 下载文件
来源：http://rgc.zhoulong.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://end.yanxiufei.cn

[R59] 发 POST JSON
来源：http://xdh.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://upm.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://lak.tian-w.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kcf.hywenlv.cn

[R61] 磁盘占用
来源：http://env.hcnkem.com

df -h;  du -sh *
来源：http://xad.tarul.cn

[R62] 找最占空间的文件
来源：http://jrz.hnxiangtu.top

du -ah . | sort -rh | head -10
来源：http://wyg.tianlin.xyz

[R63] 内存与进程
来源：http://nsl.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://ucf.jqgufenzy.top

[R64] 结束进程
来源：http://qhh.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://tsk.zdqjudy.top

[R65] 查看端口占用
来源：http://pea.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zvx.cdnleiting.top

[R66] 定时任务
来源：http://vji.zhengqikj.top

crontab -e;  crontab -l
来源：http://neq.snrcjt.cn

[R67] 生成随机十六进制串
来源：http://hip.quarkkingdee.top

openssl rand -hex 16
来源：http://jqp.hcnkem.com

[R68] 计算文件校验值
来源：http://nsd.hywenlv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fkh.cashguo.top

[R69] 生成随机密码
来源：http://fup.gogol.net.cn


<!-- 参考信息 -->