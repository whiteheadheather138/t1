代发 wailian999

PHP:  // 手写时间戳比较
来源：http://uue.ctjpmb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gcr.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sbz.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://moh.uphjek.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xxw.zhoulong.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://pkc.daxiang520.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mdi.ydzc1.top

[P08] 处理浮点精度问题
来源：http://hds.birdmap.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gfg.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mak.tarul.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://czs.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://erh.xingfuxueyuan.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bmf.zhongyouzk.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ejs.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ihe.dianchejie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://utz.yongpay.top

================================================================================
来源：http://lrs.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uye.hysaishi.cn

================================================================================
来源：http://sym.zhixingplan.top

[Q01] 创建表
来源：http://odb.cdnleiting.top

CREATE TABLE users (
来源：http://sxv.fengsongda.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mdp.zhoulong.xyz

name VARCHAR(50) NOT NULL,
来源：http://piw.guannengcc.top

email VARCHAR(100) UNIQUE,
来源：http://moq.316326.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fcj.guowangkeji.top

);
来源：http://moy.ehwqpu.com

[Q02] 创建带外键的表
来源：http://cyr.bjfxy.top

CREATE TABLE orders (
来源：http://tmg.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cgf.hysaishi.cn

user_id INT NOT NULL,
来源：http://yfy.xingfuxueyuan.xyz

amount DECIMAL(10, 2),
来源：http://rbj.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rqu.gzhubu.top

);
来源：http://rpa.ydzc1.top

[Q03] 增加列
来源：http://wvy.yj202588.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sar.yj202588.top

[Q04] 修改列类型
来源：http://egr.chenlongwang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mxf.jiagoushi.top

[Q05] 重命名列
来源：http://ftg.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jeu.ydzc1.top

[Q06] 删除列
来源：http://xlt.uphjek.com

ALTER TABLE users DROP COLUMN age;
来源：http://oht.jinqigfzy.top

[Q07] 删除表
来源：http://tey.tanke756.top

DROP TABLE IF EXISTS orders;
来源：http://iup.uphjek.com

[Q08] 创建普通索引
来源：http://dcx.ydjk.org.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oaf.chenjidiqi.icu

[Q09] 创建唯一索引
来源：http://wqm.epnwcf.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hhc.xylfe.cn

[Q10] 插入单行
来源：http://hqg.tanke756.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dab.tanke756.top

[Q11] 一次插入多行
来源：http://byz.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kee.zdbjq.cn

[Q12] 插入后取自增 ID
来源：http://try.316326.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://lad.xuanzx.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qyg.jlsjyb.cn

[Q13] 忽略重复插入
来源：http://zax.yvedp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jnf.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://xtl.zhaomingkeji.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://osz.9152youxi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oja.quarkkingdee.top

[Q15] 查询全部
来源：http://kzo.meibo888.top

SELECT * FROM users;
来源：http://lmg.sysykeji.top

[Q16] 查询指定列
来源：http://jzc.jyoumei.cn

SELECT id, name FROM users;
来源：http://hfo.xuanzx.com

[Q17] 条件查询
来源：http://fln.zhoulong.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uuf.shuidangran.top

[Q18] 模糊匹配
来源：http://hrw.chenjidiqi.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://skx.hnxiangtu.top

[Q19] 范围查询
来源：http://itl.zhixingplan.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://inw.yvedp.cn

[Q20] IN 列表
来源：http://rjs.sweek.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pfy.xuanzx.com

[Q21] 空值判断
来源：http://fwz.sxryk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gtm.hnxiangtu.top

[Q22] 排序
来源：http://hey.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://phw.dianchejie.cn

[Q23] 分页
来源：http://fsk.ydjk.org.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://siu.fanxiaobao.xyz

[Q24] 去重
来源：http://pbk.guowangkeji.top

SELECT DISTINCT city FROM users;
来源：http://bom.ydzc1.top

[Q25] 只取前 N 条
来源：http://bsr.meibo888.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://agb.vehdjk.com

[Q26] 计数
来源：http://igq.vehdjk.com

SELECT COUNT(*) FROM users;
来源：http://iat.fktsv.cn

[Q27] 条件计数
来源：http://hth.yvedp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ivk.jinqigfzy.top

[Q28] 求和与平均
来源：http://izg.vqdsnc.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qea.shanyushiyangkeji.top

[Q29] 最大最小值
来源：http://syh.nanxinkj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nfc.guowangkeji.top

[Q30] 分组统计
来源：http://kmn.cdnleiting.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ofd.cqqwz.cn

[Q31] 分组后过滤
来源：http://icc.quarkkingdee.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://shv.ydzc1.top

[Q32] 分组拼接字符串
来源：http://iqk.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kbq.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sug.redwolf501.top

[Q33] 多列分组
来源：http://ddx.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eeq.kuanghao11.cn

[Q34] 每组取第一条
来源：http://pqp.hnxiangtu.top

SELECT * FROM (
来源：http://htv.jianghu66.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://saw.tanke756.top

) t WHERE rn = 1;
来源：http://pki.guannengcc.top

[Q35] 内连接
来源：http://ebo.cheryme.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lrr.tanke756.top

[Q36] 左连接
来源：http://scv.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dvn.jqgfzy.top

[Q37] 右连接
来源：http://vsu.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://thv.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bwe.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jzo.fzhhl.top

[Q39] 自连接（查上下级）
来源：http://elt.jyoumei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://aoy.zhongyouzk.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://las.zhaomingkeji.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://vqi.yuxming.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zik.ywan-chungtsiang.top

[Q41] 多表连接
来源：http://czr.tarul.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jez.52xcode.cn

JOIN users u ON u.id = o.user_id
来源：http://hwd.yj20258.top

JOIN products p ON p.id = o.product_id;
来源：http://ntv.hongshengwenyu.top

[Q42] 连接条件附加过滤
来源：http://qsf.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://gws.jqgfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://org.sysykeji.top

[Q43] 标量子查询
来源：http://tyv.gaohongyu789.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dua.nanxuanxn.top

[Q44] IN 子查询
来源：http://olp.jqgfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fve.52xcode.cn

[Q45] EXISTS 判断存在
来源：http://jlg.gzhubu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ird.wangshuangyany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://btl.yanxiufei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kdo.zhoulong.xyz

[Q47] 与平均值比较
来源：http://wob.fengsongda.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yxt.birdmap.top

[Q48] CTE 公用表表达式
来源：http://flk.hcnkem.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fev.sweek.top

SELECT * FROM t WHERE c > 5;
来源：http://dpw.bbcook.cn

[Q49] 更新单行
来源：http://acc.dashuyun.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yjx.hfpthk.cn

[Q50] 批量更新
来源：http://mvc.kuanghao11.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vsp.zdqjudy.top

[Q51] 用子查询更新
来源：http://erx.ppjwa.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://csl.guannengcc.top

[Q52] 删除指定行
来源：http://dpm.dashuyun.cn

DELETE FROM users WHERE id = 10;
来源：http://mcf.xinyue.icu

[Q53] 按条件删除
来源：http://wmo.ybcxt.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rke.gotoacloud.top

[Q54] 清空表
来源：http://lrx.jqgfzy.top

TRUNCATE TABLE logs;
来源：http://cir.xinyue.icu

[Q55] 排名（并列占位）
来源：http://ppi.jianghu66.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ory.sjlbkw.cn

[Q56] 密集排名（并列不占位）
来源：http://gux.ehwqpu.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wjk.sufxvd.cn

[Q57] 行号
来源：http://ngh.yongpay.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pxo.xingfuxueyuan.xyz

[Q58] 累计求和
来源：http://fwn.9152youxi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wjn.nwbrower.top

[Q59] 分组内累计
来源：http://tzq.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nut.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://eds.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ozw.xuanzx.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ubx.zhiwuduotai.top

[Q61] 移动平均
来源：http://eon.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gud.tanke756.top

[Q62] 分组占比
来源：http://ygu.xziqi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kaq.ehwqpu.com

[Q63] 开启事务
来源：http://lrb.svipenyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ypv.hcnkem.com

[Q64] 提交事务
来源：http://cpw.cqqwz.cn

COMMIT;
来源：http://vct.cashguo.top

[Q65] 回滚事务
来源：http://mtw.jinghuilouyu.cn

ROLLBACK;
来源：http://fkh.sysykeji.top

[Q66] 行锁查询
来源：http://mjq.gzhubu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ads.xuetiantiany.cn

[Q67] 设置隔离级别
来源：http://akh.zycfv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bde.sysykeji.top

[Q68] 保存点
来源：http://izx.jiagoushi.top

SAVEPOINT sp1;
来源：http://rlu.bjfxy.top

ROLLBACK TO sp1;
来源：http://vit.nanxinkj.top

[Q69] 查看执行计划
来源：http://ixw.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hmi.xuetiantiany.cn

[Q70] 更新统计信息
来源：http://lwq.gzhubu.top

ANALYZE TABLE users;
来源：http://yti.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://yws.ivvv.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uit.zhaomingkeji.xyz

[Q72] 查看索引
来源：http://gie.havefunace.top

SHOW INDEX FROM users;
来源：http://fgo.hcnkem.com

[Q73] 查看表状态
来源：http://jpe.bbcook.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mks.shanyushiyangtech.top

[Q74] 强制使用索引
来源：http://vnu.tianlin.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mjb.zhengqikj.top

[Q75] 日期格式化
来源：http://rvl.zhaomingkeji.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lsg.zdqjudy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ikn.jqgfzy.top

[Q76] 按天统计
来源：http://fqk.tian-w.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jkh.birdmap.top

[Q77] 时间加减
来源：http://pdj.yanxiufei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cjb.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://llh.ctjpmb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qza.52xcode.cn

[Q79] 字符串拼接
来源：http://kvz.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gdl.tanke756.top

[Q80] 字符串截取
来源：http://hlk.ivvv.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xgf.sysykeji.top

[Q81] 字符串替换
来源：http://sgd.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jti.yuanzhike.top

[Q82] 字符长度与字节长度
来源：http://kqw.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vnk.xinyue.icu

[Q83] 大小写转换
来源：http://nkv.cqqwz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gex.hywenlv.cn

[Q84] 去除首尾空格
来源：http://slg.hnxiangtu.top

SELECT TRIM(name) FROM users;
来源：http://pwn.jianghu66.top

[Q85] 数值取整
来源：http://yey.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fjt.zhixingplan.top

[Q86] 读取 JSON 字段
来源：http://hze.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lni.tian-w.cn

[Q87] JSON 字段做条件
来源：http://ftb.iojbl.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://leb.guannengcc.top

[Q88] 行转列（条件聚合）
来源：http://san.bjfxy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jyf.smart0.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jbi.epnwcf.com

[Q89] 判断表是否存在
来源：http://fmg.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gil.gaohongyu789.top

[Q90] 生成序号列
来源：http://knk.bbcook.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://soo.zhaomingkeji.xyz

================================================================================
来源：http://zwy.ybcxt.top

R. Bash 专题
来源：http://xyt.hfpthk.cn

================================================================================
来源：http://zjj.uphjek.com

[R01] shebang 与严格模式
来源：http://qvl.zycfv.cn

#!/usr/bin/env bash
来源：http://emw.ivvv.top

set -euo pipefail
来源：http://ndb.52xcode.cn

[R02] 变量赋值与使用
来源：http://liw.sxryk.cn

name="Tom"; echo "$name"
来源：http://ior.sufxvd.cn

[R03] 只读变量
来源：http://jlp.dashuyun.cn

readonly PI=3.14
来源：http://gdi.gotoacloud.top

[R04] 位置参数
来源：http://ohp.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nla.xylfe.cn

[R05] 参数默认值
来源：http://xst.dianchejie.cn

name="${1:-default}"
来源：http://xtq.havefunace.top

[R06] 判断命令是否存在
来源：http://mzx.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://syf.snrcjt.cn

[R07] if 判断文件
来源：http://urs.tian-w.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oyc.hfpthk.cn

[R08] 数值比较
来源：http://wcn.zhixingplan.top

if (( a > b )); then echo "a 更大"; fi
来源：http://aeo.shanyushiyangtech.top

[R09] 字符串比较
来源：http://jbv.andypj.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kem.chenjidiqi.icu

[R10] 正则匹配
来源：http://jec.yj202588.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bsh.zhijiandao.cn

[R11] case 多分支
来源：http://fuf.kuanghao11.cn

case "$1" in
来源：http://lqc.tianlin.xyz

start) echo "启动" ;;
来源：http://rou.hysaishi.cn

stop)  echo "停止" ;;
来源：http://nif.sxryk.cn

*)     echo "未知命令" ;;
来源：http://uid.andypj.xyz

esac
来源：http://nrp.gogol.net.cn

[R12] for 遍历文件
来源：http://dlm.wangshuangyany.cn

for f in *.txt; do echo "$f"; done
来源：http://jvc.sxryk.cn

[R13] for 计数循环
来源：http://sfg.yvedp.cn

for i in {1..10}; do echo "$i"; done
来源：http://nak.hnqzz.top

[R14] C 风格 for
来源：http://qgm.wangshuangyany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eeu.xuetiantiany.cn

[R15] while 逐行读文件
来源：http://tzl.ppjwa.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://snl.gotoacloud.top

[R16] until 等待条件
来源：http://bht.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://duh.meibo888.top

[R17] 数组定义与取值
来源：http://qqg.jinghuilouyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oss.yuanzhike.top

[R18] 遍历数组
来源：http://ail.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://knt.pycfn.com

[R19] 数组长度
来源：http://gci.bbcook.cn

echo "${#arr[@]}"
来源：http://vhz.redwolf501.top

[R20] 关联数组（字典）
来源：http://iqc.iojbl.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rge.zdqjudy.top

[R21] 字符串长度
来源：http://vfo.zhixingplan.top

echo "${#s}"
来源：http://fwp.wangdashe.top

[R22] 截取子串
来源：http://buo.shanyushiyangkeji.top

echo "${s:0:5}"
来源：http://xbi.zycfv.cn

[R23] 字符串替换
来源：http://xed.tanke756.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://crc.ivvv.top

[R24] 大小写转换
来源：http://bhs.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://neo.sweek.top

[R25] 去后缀 / 去前缀
来源：http://jjv.wangdashe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kto.zhengqikj.top

[R26] 命令替换
来源：http://nvc.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://xiw.nanxinkj.top

[R27] 算术展开
来源：http://fvk.hammf.cn

echo $((1 + 2 * 3))
来源：http://zzo.ehwqpu.com

[R28] 浮点运算
来源：http://rgu.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://aov.jianghu66.top

[R29] 定义函数
来源：http://fjr.xuanzx.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hto.yongpay.top

[R30] 函数返回状态码
来源：http://xin.ybcxt.top

f() { return 0; }; f || echo "失败了"
来源：http://jyi.tanke756.top

[R31] 局部变量
来源：http://ina.316326.xyz

f() { local x=1; echo "$x"; }
来源：http://wiz.hywenlv.cn

[R32] 参数个数校验
来源：http://gka.sxryk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ynv.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://nde.kuanghao11.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pie.guowangkeji.top

[R34] 退出时清理
来源：http://wdk.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://fej.xziqi.cn

[R35] 后台执行并等待
来源：http://fnb.shanyushiyangtech.top


<!-- 参考信息 -->