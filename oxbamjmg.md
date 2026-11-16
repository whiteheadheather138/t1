代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wqa.aizwys.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://esr.cashguo.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yfb.0kj1m.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kxi.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wxo.ydjk.org.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://msy.0kj1m.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hyx.tanke756.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hcd.shuidangran.top

================================================================================
来源：http://jsi.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rfh.nanxinkj.top

================================================================================
来源：http://nsp.yonumen.top

[Q01] 创建表
来源：http://voc.yongpay.top

CREATE TABLE users (
来源：http://ycs.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uii.xylfe.cn

name VARCHAR(50) NOT NULL,
来源：http://nea.ivvv.top

email VARCHAR(100) UNIQUE,
来源：http://qqe.hywenlv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wjr.fanxiaobao.xyz

);
来源：http://jdq.hywenlv.cn

[Q02] 创建带外键的表
来源：http://oae.cucudq.cn

CREATE TABLE orders (
来源：http://exb.dianchejie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hld.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://lce.gotoacloud.top

amount DECIMAL(10, 2),
来源：http://nvw.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pec.ehwqpu.com

);
来源：http://ose.cqqwz.cn

[Q03] 增加列
来源：http://viu.ydzc1.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mle.yfazqb.com

[Q04] 修改列类型
来源：http://arv.chenzaomai.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cve.nwbrower.top

[Q05] 重命名列
来源：http://lqe.jianghu66.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ucp.tianlin.xyz

[Q06] 删除列
来源：http://out.zhijiandao.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rfd.cucudq.cn

[Q07] 删除表
来源：http://mdr.ehwqpu.com

DROP TABLE IF EXISTS orders;
来源：http://bwe.jqgufenzy.top

[Q08] 创建普通索引
来源：http://skx.9152youxi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://djk.mhx1999.top

[Q09] 创建唯一索引
来源：http://pvr.fzhhl.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tkc.pengpengdd.cyou

[Q10] 插入单行
来源：http://age.yangfankeji.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uds.hysaishi.cn

[Q11] 一次插入多行
来源：http://jyy.zycfv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jyi.ydjk.org.cn

[Q12] 插入后取自增 ID
来源：http://ynf.andypj.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://opc.ydzc1.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ohl.cucudq.cn

[Q13] 忽略重复插入
来源：http://ouw.havefunace.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ilj.c1oappe.top

[Q14] 存在则更新（upsert）
来源：http://pco.yuanzhike.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lwf.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://apz.epnwcf.com

[Q15] 查询全部
来源：http://tbm.ybcxt.top

SELECT * FROM users;
来源：http://gtm.zdqjudy.top

[Q16] 查询指定列
来源：http://hcn.zhongyouzk.top

SELECT id, name FROM users;
来源：http://xxe.ydzc1.top

[Q17] 条件查询
来源：http://dhx.guowangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tmr.tanke756.top

[Q18] 模糊匹配
来源：http://jbq.meibo888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nlp.bjfxy.top

[Q19] 范围查询
来源：http://pki.yj202588.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dsy.tian-w.cn

[Q20] IN 列表
来源：http://cnb.yuxming.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pyd.wangshuangyany.cn

[Q21] 空值判断
来源：http://wfd.zdqjudy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rbc.52xcode.cn

[Q22] 排序
来源：http://mkc.ydjk.org.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bic.ivvv.top

[Q23] 分页
来源：http://qpm.zhengqikj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ukf.chenzaomai.com

[Q24] 去重
来源：http://cmf.jyoumei.cn

SELECT DISTINCT city FROM users;
来源：http://fpg.tanke756.top

[Q25] 只取前 N 条
来源：http://eey.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kwi.c1oappe.top

[Q26] 计数
来源：http://krd.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://anv.andypj.xyz

[Q27] 条件计数
来源：http://uua.jqgfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://smn.hnqzz.top

[Q28] 求和与平均
来源：http://wcv.ppjwa.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kkc.mhx1999.top

[Q29] 最大最小值
来源：http://oek.shuidangran.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ihf.chenlongwang.top

[Q30] 分组统计
来源：http://zli.fktsv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ksa.guowangkeji.top

[Q31] 分组后过滤
来源：http://gyd.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://udl.jinqigfzy.top

[Q32] 分组拼接字符串
来源：http://yos.fehbvm.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://txu.fzhhl.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://brq.gotoacloud.top

[Q33] 多列分组
来源：http://wst.tarul.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lhx.ybcxt.top

[Q34] 每组取第一条
来源：http://kyd.jinghuilouyu.cn

SELECT * FROM (
来源：http://zju.hnxiangtu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xcu.9152youxi.cn

) t WHERE rn = 1;
来源：http://rvs.svipenyu.cn

[Q35] 内连接
来源：http://dtj.xuetiantiany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mrd.ehwqpu.com

[Q36] 左连接
来源：http://mku.pycfn.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vxt.havefunace.top

[Q37] 右连接
来源：http://yhu.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gig.ehwqpu.com

[Q38] 全外连接（PostgreSQL）
来源：http://kip.wangdashe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ywj.xziqi.cn

[Q39] 自连接（查上下级）
来源：http://zpc.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tnc.316326.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dhl.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pkh.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hoc.zycfv.cn

[Q41] 多表连接
来源：http://vje.yfazqb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://neu.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://yva.meibo888.top

JOIN products p ON p.id = o.product_id;
来源：http://qus.zhoulong.xyz

[Q42] 连接条件附加过滤
来源：http://faa.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://gcn.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dvx.fengsongda.top

[Q43] 标量子查询
来源：http://htl.vqdsnc.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sbv.cqqwz.cn

[Q44] IN 子查询
来源：http://fjk.pengpengdd.cyou

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pzg.meibo888.top

[Q45] EXISTS 判断存在
来源：http://lhh.shanyushiyangtech.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://azm.hysaishi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rio.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eto.guannengcc.top

[Q47] 与平均值比较
来源：http://kxd.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ujq.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://jkj.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kfy.xuanzx.com

SELECT * FROM t WHERE c > 5;
来源：http://agl.chenjidiqi.icu

[Q49] 更新单行
来源：http://ukt.hfpthk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cbm.yuanzhike.top

[Q50] 批量更新
来源：http://yqg.tian-w.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bre.fehbvm.com

[Q51] 用子查询更新
来源：http://nki.kuanghao11.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sfq.quarkkingdee.top

[Q52] 删除指定行
来源：http://kbx.hfpthk.cn

DELETE FROM users WHERE id = 10;
来源：http://tlp.guowangkeji.top

[Q53] 按条件删除
来源：http://pxs.yangfankeji.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://usz.fanxiaobao.xyz

[Q54] 清空表
来源：http://ouy.zhixingplan.top

TRUNCATE TABLE logs;
来源：http://zeq.nwbrower.top

[Q55] 排名（并列占位）
来源：http://rpy.zhijiandao.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xtz.fanxiaobao.xyz

[Q56] 密集排名（并列不占位）
来源：http://gwt.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nka.sjlbkw.cn

[Q57] 行号
来源：http://mhz.meibo888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ihs.chenlongwang.top

[Q58] 累计求和
来源：http://uzd.redwolf501.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mml.ivvv.top

[Q59] 分组内累计
来源：http://gxm.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ttj.tarul.cn

[Q60] 取上一行 / 下一行
来源：http://qth.cheryme.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mpv.yvedp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hpl.fengsongda.top

[Q61] 移动平均
来源：http://hpl.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ffp.fzhhl.top

[Q62] 分组占比
来源：http://xit.316326.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yom.xziqi.cn

[Q63] 开启事务
来源：http://lbm.gaohongyu789.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dlh.bbcook.cn

[Q64] 提交事务
来源：http://vqs.0kj1m.cn

COMMIT;
来源：http://ihm.c1oappe.top

[Q65] 回滚事务
来源：http://cjk.yuanzhike.top

ROLLBACK;
来源：http://uvj.zhixingplan.top

[Q66] 行锁查询
来源：http://dri.sjlbkw.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hdf.kuanghao11.cn

[Q67] 设置隔离级别
来源：http://udv.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://acn.dashuyun.cn

[Q68] 保存点
来源：http://lwd.chenlongwang.top

SAVEPOINT sp1;
来源：http://icp.sxryk.cn

ROLLBACK TO sp1;
来源：http://byo.vehdjk.com

[Q69] 查看执行计划
来源：http://jpj.meibo888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dai.ydzc1.top

[Q70] 更新统计信息
来源：http://kjg.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://ifb.zdbjq.cn

[Q71] 查看建表语句
来源：http://wgt.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ope.shzxlz.cn

[Q72] 查看索引
来源：http://rjr.yj202588.top

SHOW INDEX FROM users;
来源：http://tjl.sjlbkw.cn

[Q73] 查看表状态
来源：http://fgz.guannengcc.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jlo.yuanzhike.top

[Q74] 强制使用索引
来源：http://uzy.tarul.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pcv.svipenyu.cn

[Q75] 日期格式化
来源：http://ngy.zhaomingkeji.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://amw.316326.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pwv.shangyingyoupin.top

[Q76] 按天统计
来源：http://nmv.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ynq.yvedp.cn

[Q77] 时间加减
来源：http://qjn.cheryme.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ith.jiagoushi.top

[Q78] 当前时间
来源：http://esp.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://myk.hcnkem.com

[Q79] 字符串拼接
来源：http://bwq.sufxvd.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fci.zhixingplan.top

[Q80] 字符串截取
来源：http://cmv.zhongyouzk.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xoq.aibaodan.cn

[Q81] 字符串替换
来源：http://qkx.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fgq.jqgufenzy.top

[Q82] 字符长度与字节长度
来源：http://com.zhoulong.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cnt.yuanzhike.top

[Q83] 大小写转换
来源：http://mbd.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vxt.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://jdl.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://oal.iojbl.cn

[Q85] 数值取整
来源：http://grw.dianchejie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wms.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://kda.nanxinkj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rdv.sufxvd.cn

[Q87] JSON 字段做条件
来源：http://xwi.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zzn.cheryme.top

[Q88] 行转列（条件聚合）
来源：http://wfd.52xcode.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fmc.hywenlv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pmx.jiagoushi.top

[Q89] 判断表是否存在
来源：http://rsm.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fvk.shanyushiyangkeji.top

[Q90] 生成序号列
来源：http://wkl.jiagoushi.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zdg.jiagoushi.top

================================================================================
来源：http://afr.yj20258.top

R. Bash 专题
来源：http://bjn.fzhhl.top

================================================================================
来源：http://mli.yanxiufei.cn

[R01] shebang 与严格模式
来源：http://dhf.dianchejie.cn

#!/usr/bin/env bash
来源：http://xvh.pengpengdd.cyou

set -euo pipefail
来源：http://cml.cucudq.cn

[R02] 变量赋值与使用
来源：http://vfz.ctjpmb.com

name="Tom"; echo "$name"
来源：http://jsu.yangfankeji.com

[R03] 只读变量
来源：http://dcu.chenzaomai.com

readonly PI=3.14
来源：http://clt.cucudq.cn

[R04] 位置参数
来源：http://kak.guowangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lhq.ybcxt.top

[R05] 参数默认值
来源：http://uvu.zycfv.cn

name="${1:-default}"
来源：http://ytk.meibo888.top

[R06] 判断命令是否存在
来源：http://buo.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bra.ppjwa.cn

[R07] if 判断文件
来源：http://nbt.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hyb.yj20258888.top

[R08] 数值比较
来源：http://oqi.zhiwuduotai.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ogb.hysaishi.cn

[R09] 字符串比较
来源：http://tut.52xcode.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oak.yangfankeji.com

[R10] 正则匹配
来源：http://rap.jiagoushi.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zao.gaohongyu789.top

[R11] case 多分支
来源：http://jpk.hnxiangtu.top

case "$1" in
来源：http://jct.uphjek.com

start) echo "启动" ;;
来源：http://sma.chenzaomai.com

stop)  echo "停止" ;;
来源：http://wsl.shangyingyoupin.top

*)     echo "未知命令" ;;
来源：http://lir.fanxiaobao.xyz

esac
来源：http://kaw.sxryk.cn

[R12] for 遍历文件
来源：http://cnc.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://jjf.jiagoushi.top

[R13] for 计数循环
来源：http://lld.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://euv.gaohongyu789.top

[R14] C 风格 for
来源：http://udc.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fam.hammf.cn

[R15] while 逐行读文件
来源：http://kck.hongshengwenyu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eva.jlsjyb.cn

[R16] until 等待条件
来源：http://ixv.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vlw.jqgfzy.top

[R17] 数组定义与取值
来源：http://biz.nanxuanxn.top

arr=(a b c); echo "${arr[0]}"
来源：http://xnr.guowangkeji.top

[R18] 遍历数组
来源：http://szk.smart0.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rhr.feifeiyinyue.top

[R19] 数组长度
来源：http://zml.ehwqpu.com

echo "${#arr[@]}"
来源：http://jfw.dashuyun.cn

[R20] 关联数组（字典）
来源：http://otg.jiagoushi.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ofa.fzhhl.top

[R21] 字符串长度
来源：http://ywv.redwolf501.top

echo "${#s}"
来源：http://jma.hysaishi.cn

[R22] 截取子串
来源：http://zej.hywenlv.cn

echo "${s:0:5}"
来源：http://iun.haohaochexian.top

[R23] 字符串替换
来源：http://rfd.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tlh.hammf.cn

[R24] 大小写转换
来源：http://eyb.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://znw.fanxiaobao.xyz

[R25] 去后缀 / 去前缀
来源：http://hpm.chenlongwang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zrd.vehdjk.com

[R26] 命令替换
来源：http://spf.sxryk.cn

now=$(date +%F); echo "$now"
来源：http://php.cashguo.top

[R27] 算术展开
来源：http://buk.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://uqf.fzhhl.top

[R28] 浮点运算
来源：http://euc.birdmap.top

echo "scale=2; 10/3" | bc
来源：http://hyo.yangfankeji.com

[R29] 定义函数
来源：http://bjs.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gld.daxiang520.top

[R30] 函数返回状态码
来源：http://dru.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://fuf.shuidangran.top

[R31] 局部变量
来源：http://ajr.havefunace.top

f() { local x=1; echo "$x"; }
来源：http://oxc.ybcxt.top

[R32] 参数个数校验
来源：http://zpw.wangdashe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qit.chenzaomai.com

[R33] 捕获错误并提示行号
来源：http://iju.yj20258.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://srt.yangfankeji.com

[R34] 退出时清理
来源：http://czp.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://fya.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://aku.hcnkem.com

sleep 5 & pid=$!; wait "$pid"
来源：http://uvp.redwolf501.top

[R36] 并发执行多个任务
来源：http://vma.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ysb.fzhhl.top

[R37] 把输出赋给变量
来源：http://tkb.zhoulong.xyz

files=$(ls -1)
来源：http://wkm.quarkkingdee.top

[R38] 管道串联
来源：http://asr.jinqigufen.top

cat a.txt | grep -i error | wc -l
来源：http://syq.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://tmq.zhengqikj.top


<!-- 参考信息 -->