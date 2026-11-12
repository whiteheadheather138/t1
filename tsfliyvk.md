代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://fop.shuidangran.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hlq.jqgfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://unm.gotoacloud.top

[Q15] 查询全部
来源：http://lpu.jqgufenzy.top

SELECT * FROM users;
来源：http://ddb.shuidangran.top

[Q16] 查询指定列
来源：http://wwp.hysaishi.cn

SELECT id, name FROM users;
来源：http://nom.gotoacloud.top

[Q17] 条件查询
来源：http://oix.ydjk.org.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hhs.yueranfly.top

[Q18] 模糊匹配
来源：http://kpy.jinqigufen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tea.zhijiandao.cn

[Q19] 范围查询
来源：http://nzx.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xaj.9152youxi.cn

[Q20] IN 列表
来源：http://wgs.hammf.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vjb.yanxiufei.cn

[Q21] 空值判断
来源：http://ral.hongshengwenyu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ugb.shzxlz.cn

[Q22] 排序
来源：http://oty.jinqigufen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qee.zycfv.cn

[Q23] 分页
来源：http://lfe.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ebd.jqgufenzy.top

[Q24] 去重
来源：http://uvd.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://zdy.zycfv.cn

[Q25] 只取前 N 条
来源：http://prw.tian-w.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dgw.yuanzhike.top

[Q26] 计数
来源：http://euw.zdbjq.cn

SELECT COUNT(*) FROM users;
来源：http://frl.aizwys.cn

[Q27] 条件计数
来源：http://eqy.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oea.gzhubu.top

[Q28] 求和与平均
来源：http://mnf.9152youxi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://crj.cucudq.cn

[Q29] 最大最小值
来源：http://ago.tian-w.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://teb.daria6918.cn

[Q30] 分组统计
来源：http://cfu.gogol.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bgb.zhaomingkeji.xyz

[Q31] 分组后过滤
来源：http://zvl.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mcr.gotoacloud.top

[Q32] 分组拼接字符串
来源：http://fam.tianlin.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eco.zdbjq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hrx.daria6918.cn

[Q33] 多列分组
来源：http://pmn.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hnb.yonumen.top

[Q34] 每组取第一条
来源：http://qov.zhongyouzk.top

SELECT * FROM (
来源：http://dcm.quarkkingdee.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iai.gaohongyu789.top

) t WHERE rn = 1;
来源：http://fca.yueranfly.top

[Q35] 内连接
来源：http://sdw.zycfv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nxi.chenzaomai.com

[Q36] 左连接
来源：http://gpi.jinqigfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rvu.zhongyouzk.top

[Q37] 右连接
来源：http://qzl.gogol.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tye.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://vby.tianlin.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hoi.zhongyouzk.top

[Q39] 自连接（查上下级）
来源：http://ncv.sweek.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rzv.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tgw.pengpengdd.cyou

[Q40] 交叉连接（笛卡尔积）
来源：http://jas.wangshuangyany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://smq.tarul.cn

[Q41] 多表连接
来源：http://qmi.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://orv.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://pqw.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://ynp.uphjek.com

[Q42] 连接条件附加过滤
来源：http://pkj.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u
来源：http://cdx.hesvh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iog.ivvv.top

[Q43] 标量子查询
来源：http://zsj.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lpi.aizwys.cn

[Q44] IN 子查询
来源：http://prb.jinqigufen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yxq.jinghuilouyu.cn

[Q45] EXISTS 判断存在
来源：http://eof.svipenyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hzr.sweek.top

[Q46] NOT EXISTS 判断不存在
来源：http://fqf.ivvv.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gku.9152youxi.cn

[Q47] 与平均值比较
来源：http://eon.zhijiandao.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://spy.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://owc.epnwcf.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wqq.sjlbkw.cn

SELECT * FROM t WHERE c > 5;
来源：http://alu.sxryk.cn

[Q49] 更新单行
来源：http://drz.xingfuxueyuan.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nuq.jinqigfzy.top

[Q50] 批量更新
来源：http://mih.zhongyouzk.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pqi.jinqigfzy.top

[Q51] 用子查询更新
来源：http://hhn.bbcook.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://shs.vehdjk.com

[Q52] 删除指定行
来源：http://gui.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://ijg.cashguo.top

[Q53] 按条件删除
来源：http://shb.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oxk.sxryk.cn

[Q54] 清空表
来源：http://izn.sweek.top

TRUNCATE TABLE logs;
来源：http://qie.snrcjt.cn

[Q55] 排名（并列占位）
来源：http://ksb.xuanzx.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sjn.ppjwa.cn

[Q56] 密集排名（并列不占位）
来源：http://hyw.chenjidiqi.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nwa.yangfankeji.com

[Q57] 行号
来源：http://wuu.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://edr.shangyingyoupin.top

[Q58] 累计求和
来源：http://ogs.wangshuangyany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ibe.pycfn.com

[Q59] 分组内累计
来源：http://ouy.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ggu.nanxinkj.top

[Q60] 取上一行 / 下一行
来源：http://uzx.pycfn.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ggb.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cks.havefunace.top

[Q61] 移动平均
来源：http://fgf.aizwys.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qkc.shanyushiyangkeji.top

[Q62] 分组占比
来源：http://alc.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eot.bbcook.cn

[Q63] 开启事务
来源：http://uot.zycfv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://por.tian-w.cn

[Q64] 提交事务
来源：http://kom.xuanzx.com

COMMIT;
来源：http://deq.yonumen.top

[Q65] 回滚事务
来源：http://xiu.ehwqpu.com

ROLLBACK;
来源：http://xmt.daria6918.cn

[Q66] 行锁查询
来源：http://xlo.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://diy.jinghuilouyu.cn

[Q67] 设置隔离级别
来源：http://cuz.zhoulong.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vux.chenjidiqi.icu

[Q68] 保存点
来源：http://fvm.cashguo.top

SAVEPOINT sp1;
来源：http://txe.chenzaomai.com

ROLLBACK TO sp1;
来源：http://pcy.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://xch.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jdx.dianchejie.cn

[Q70] 更新统计信息
来源：http://asz.yangfankeji.com

ANALYZE TABLE users;
来源：http://nqb.cucudq.cn

[Q71] 查看建表语句
来源：http://dif.fanxiaobao.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://btn.nanxuanxn.top

[Q72] 查看索引
来源：http://vuk.xylfe.cn

SHOW INDEX FROM users;
来源：http://tld.tian-w.cn

[Q73] 查看表状态
来源：http://gjn.tianlin.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://fpn.jqgufenzy.top

[Q74] 强制使用索引
来源：http://kqg.zdqjudy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://amu.ydjk.org.cn

[Q75] 日期格式化
来源：http://vuk.jlsjyb.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uoy.ppjwa.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xxy.fzhhl.top

[Q76] 按天统计
来源：http://xyb.jinghuilouyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dlq.c1oappe.top

[Q77] 时间加减
来源：http://wly.yj202588.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zex.tianlin.xyz

[Q78] 当前时间
来源：http://tjn.yangfankeji.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ypz.xingfuxueyuan.xyz

[Q79] 字符串拼接
来源：http://ipg.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://icd.tianlin.xyz

[Q80] 字符串截取
来源：http://kcr.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yqh.jlsjyb.cn

[Q81] 字符串替换
来源：http://cqe.jqgufenzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gil.ywan-chungtsiang.top

[Q82] 字符长度与字节长度
来源：http://aqp.cqqwz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zlb.feifeiyinyue.top

[Q83] 大小写转换
来源：http://jgb.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xhl.hnxiangtu.top

[Q84] 去除首尾空格
来源：http://gzy.yueranfly.top

SELECT TRIM(name) FROM users;
来源：http://alp.xingfuxueyuan.xyz

[Q85] 数值取整
来源：http://hno.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ygh.redwolf501.top

[Q86] 读取 JSON 字段
来源：http://mtp.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zpy.jqgfzy.top

[Q87] JSON 字段做条件
来源：http://ybk.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pgy.ivvv.top

[Q88] 行转列（条件聚合）
来源：http://fhm.daxiang520.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qfl.aizwys.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jmc.jianghu66.top

[Q89] 判断表是否存在
来源：http://rda.hywenlv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kpa.zycfv.cn

[Q90] 生成序号列
来源：http://jfd.chenjidiqi.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cqw.hcnkem.com

================================================================================
来源：http://vxy.nwbrower.top

R. Bash 专题
来源：http://xrp.jianghu66.top

================================================================================
来源：http://svz.hnqzz.top

[R01] shebang 与严格模式
来源：http://nnv.jianghu66.top

#!/usr/bin/env bash
来源：http://yfr.hywenlv.cn

set -euo pipefail
来源：http://lpu.redwolf501.top

[R02] 变量赋值与使用
来源：http://ypo.chenzaomai.com

name="Tom"; echo "$name"
来源：http://her.xuanzx.com

[R03] 只读变量
来源：http://rou.jlsjyb.cn

readonly PI=3.14
来源：http://pyd.hywenlv.cn

[R04] 位置参数
来源：http://nud.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cyk.iojbl.cn

[R05] 参数默认值
来源：http://esq.sxryk.cn

name="${1:-default}"
来源：http://moc.jyoumei.cn

[R06] 判断命令是否存在
来源：http://bls.zhengqikj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qbh.yangfankeji.com

[R07] if 判断文件
来源：http://qek.xinyue.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vxe.nanxuanxn.top

[R08] 数值比较
来源：http://kdg.zhijiandao.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sds.xuanzx.com

[R09] 字符串比较
来源：http://lmc.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ith.ywan-chungtsiang.top

[R10] 正则匹配
来源：http://aiv.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uzn.jinyuanbaomall.cn

[R11] case 多分支
来源：http://sff.shanyushiyangkeji.top

case "$1" in
来源：http://jdf.kuanghao11.cn

start) echo "启动" ;;
来源：http://luy.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://mgs.gzhubu.top

*)     echo "未知命令" ;;
来源：http://pwu.yj20258.top

esac
来源：http://oyt.ydjk.org.cn

[R12] for 遍历文件
来源：http://eng.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://coq.meibo888.top

[R13] for 计数循环
来源：http://blv.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://ldm.aibaodan.cn

[R14] C 风格 for
来源：http://uxr.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tve.zdqjudy.top

[R15] while 逐行读文件
来源：http://rkz.zhijiandao.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nsq.yj20258.top

[R16] until 等待条件
来源：http://nhp.sxryk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zfa.smart0.xyz

[R17] 数组定义与取值
来源：http://omy.quarkkingdee.top

arr=(a b c); echo "${arr[0]}"
来源：http://zoe.hywenlv.cn

[R18] 遍历数组
来源：http://ulj.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uqe.yueranfly.top

[R19] 数组长度
来源：http://ack.dashuyun.cn

echo "${#arr[@]}"
来源：http://eeb.chenlongwang.top

[R20] 关联数组（字典）
来源：http://fgj.hcnkem.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zci.jyoumei.cn

[R21] 字符串长度
来源：http://eab.hesvh.cn

echo "${#s}"
来源：http://bht.snrcjt.cn

[R22] 截取子串
来源：http://ndl.zhongyouzk.top

echo "${s:0:5}"
来源：http://kzo.jinyuanbaomall.cn

[R23] 字符串替换
来源：http://qwm.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jpa.andypj.xyz

[R24] 大小写转换
来源：http://vhk.quarkkingdee.top

echo "${s^^}"; echo "${s,,}"
来源：http://pgg.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://uvm.iojbl.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xfq.jiagoushi.top

[R26] 命令替换
来源：http://vrk.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://kix.fengsongda.top

[R27] 算术展开
来源：http://hfx.hysaishi.cn

echo $((1 + 2 * 3))
来源：http://ehw.daria6918.cn

[R28] 浮点运算
来源：http://dwh.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://lvl.meibo888.top

[R29] 定义函数
来源：http://xdb.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rnz.meibo888.top

[R30] 函数返回状态码
来源：http://zvk.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://ejt.jqgufenzy.top

[R31] 局部变量
来源：http://neo.cqqwz.cn

f() { local x=1; echo "$x"; }
来源：http://foh.316326.xyz

[R32] 参数个数校验
来源：http://ris.havefunace.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://icz.xinyue.icu

[R33] 捕获错误并提示行号
来源：http://naa.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vpc.bjfxy.top

[R34] 退出时清理
来源：http://vzu.jqgufenzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://rca.hcnkem.com

[R35] 后台执行并等待
来源：http://acq.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qfn.sxryk.cn

[R36] 并发执行多个任务
来源：http://qzq.cdnleiting.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bzx.yangfankeji.com

[R37] 把输出赋给变量
来源：http://dwu.shangyingyoupin.top

files=$(ls -1)
来源：http://zoh.ybcxt.top

[R38] 管道串联
来源：http://stv.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://res.ehwqpu.com

[R39] 重定向标准输出与错误
来源：http://spc.hesvh.cn

cmd > out.log 2>&1
来源：http://vgf.yuxming.cn

[R40] 追加写日志
来源：http://ntb.yangfankeji.com

echo "log" >> out.log
来源：http://qop.yangfankeji.com

[R41] 丢弃输出
来源：http://cab.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://gav.jqgufenzy.top

[R42] 输入重定向
来源：http://phu.sxryk.cn

wc -l < a.txt
来源：http://rzk.meibo888.top

[R43] 按名字查找文件
来源：http://qwv.jinyuanbaomall.cn

find . -name "*.log" -type f
来源：http://uof.jinghuilouyu.cn

[R44] 按修改时间查找
来源：http://ycc.zhoulong.xyz

find . -mtime -7 -type f
来源：http://lnu.jqgfzy.top

[R45] 批量删除
来源：http://flq.chenjidiqi.icu

find . -name "*.tmp" -delete
来源：http://umr.cashguo.top

[R46] 递归替换文件内容
来源：http://mhv.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qlj.aibaodan.cn

[R47] sed 单行替换
来源：http://xma.aizwys.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jai.daria6918.cn

[R48] awk 取指定列
来源：http://yla.zycfv.cn

awk '{print $1, $3}' a.txt
来源：http://mso.xinyue.icu

[R49] awk 带条件
来源：http://dwk.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pvf.birdmap.top

[R50] awk 求和
来源：http://zwh.tianlin.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://oaa.sweek.top

[R51] 排序去重取前几
来源：http://jyl.yonumen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xfl.xinyue.icu

[R52] 统计行数
来源：http://ezw.tanke756.top

wc -l a.txt
来源：http://xhm.cheryme.top

[R53] 查看文件头与实时尾
来源：http://owz.fzhhl.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cka.hammf.cn

[R54] 比较两个文件
来源：http://yfx.redwolf501.top

diff a.txt b.txt
来源：http://wfh.snrcjt.cn

[R55] 压缩与解压
来源：http://ptm.jqgfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tlw.quarkkingdee.top

[R56] 远程拷贝
来源：http://hds.ehwqpu.com

scp file user@host:/path/
来源：http://ohu.yj202588.top

[R57] 远程执行命令
来源：http://rqu.xuanzx.com

ssh user@host 'uptime'
来源：http://fgl.shzxlz.cn

[R58] 下载文件
来源：http://olz.yonumen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dya.kuanghao11.cn

[R59] 发 POST JSON
来源：http://tbz.chenzaomai.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jmh.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://thc.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rhn.smart0.xyz

[R61] 磁盘占用
来源：http://exs.ctjpmb.com

df -h;  du -sh *
来源：http://kur.zdqjudy.top

[R62] 找最占空间的文件
来源：http://doc.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://ohf.daxiang520.top

[R63] 内存与进程
来源：http://ovr.xingfuxueyuan.xyz


<!-- 参考信息 -->