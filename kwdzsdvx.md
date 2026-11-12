代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://dns.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ljh.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qfg.hnxiangtu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tkz.dashuyun.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://exs.cashguo.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nxf.cheryme.top

Go:   reflect.DeepEqual(a, b)
来源：http://moc.zhengqikj.top

Ruby: a == b
来源：http://vaw.zhixingplan.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wqz.ppjwa.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qju.hnqzz.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qje.jqgufenzy.top

PHP:  if (empty($x)) {}
来源：http://iqq.meibo888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jcf.c1oappe.top

TS:   if (x == null) {}
来源：http://zhc.hfpthk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gob.zdbjq.cn

Go:   if x == nil {}
来源：http://nft.snrcjt.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vqa.vqdsnc.cn

C#:   if (x is null) {}
来源：http://gwo.zhijiandao.cn

[P07] 防抖与节流
来源：http://aoi.zhiwuduotai.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blw.zhijiandao.cn

PHP:  // 手写时间戳比较
来源：http://ygh.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zbp.yonumen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yuq.9152youxi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://koa.hongshengwenyu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ntl.zhengqikj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wey.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ufc.epnwcf.com

[P08] 处理浮点精度问题
来源：http://enu.kuanghao11.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hkc.hnxiangtu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://icu.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nlc.gzhubu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vus.uphjek.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jbq.daria6918.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ufe.9152youxi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tpe.tian-w.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rrr.zdqjudy.top

================================================================================
来源：http://yet.ydzc1.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qtv.vqdsnc.cn

================================================================================
来源：http://fje.feifeiyinyue.top

[Q01] 创建表
来源：http://kpw.nanxinkj.top

CREATE TABLE users (
来源：http://zlv.hnqzz.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uxg.uphjek.com

name VARCHAR(50) NOT NULL,
来源：http://rjp.guowangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://abr.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uoi.birdmap.top

);
来源：http://jzf.bjfxy.top

[Q02] 创建带外键的表
来源：http://vjh.cdnleiting.top

CREATE TABLE orders (
来源：http://ocb.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lvr.bbcook.cn

user_id INT NOT NULL,
来源：http://aos.guannengcc.top

amount DECIMAL(10, 2),
来源：http://fry.sjlbkw.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cxs.havefunace.top

);
来源：http://duu.xylfe.cn

[Q03] 增加列
来源：http://xcq.jinghuilouyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hhs.hysaishi.cn

[Q04] 修改列类型
来源：http://cmg.xuetiantiany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gkh.hesvh.cn

[Q05] 重命名列
来源：http://pmt.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dpn.yfazqb.com

[Q06] 删除列
来源：http://qxd.shzxlz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://aqq.316326.xyz

[Q07] 删除表
来源：http://bod.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://qlr.ppjwa.cn

[Q08] 创建普通索引
来源：http://bzk.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://szy.sjlbkw.cn

[Q09] 创建唯一索引
来源：http://rpu.cucudq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uob.zhiwuduotai.top

[Q10] 插入单行
来源：http://gts.sweek.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bpo.quarkkingdee.top

[Q11] 一次插入多行
来源：http://skw.havefunace.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nwq.zycfv.cn

[Q12] 插入后取自增 ID
来源：http://xoq.smart0.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://exz.yanxiufei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hds.gzhubu.top

[Q13] 忽略重复插入
来源：http://xhm.tian-w.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://csy.guowangkeji.top

[Q14] 存在则更新（upsert）
来源：http://vcc.316326.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wza.dianchejie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ogf.ivvv.top

[Q15] 查询全部
来源：http://yrp.fengsongda.top

SELECT * FROM users;
来源：http://ksu.zhaomingkeji.xyz

[Q16] 查询指定列
来源：http://tib.xylfe.cn

SELECT id, name FROM users;
来源：http://trz.zhixingplan.top

[Q17] 条件查询
来源：http://shj.andypj.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xaw.yangfankeji.com

[Q18] 模糊匹配
来源：http://gzz.fengsongda.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ckm.fktsv.cn

[Q19] 范围查询
来源：http://kgl.0kj1m.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ckq.xziqi.cn

[Q20] IN 列表
来源：http://kiw.vqdsnc.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kll.sufxvd.cn

[Q21] 空值判断
来源：http://yko.epnwcf.com

SELECT * FROM users WHERE email IS NULL;
来源：http://grp.yfazqb.com

[Q22] 排序
来源：http://dts.cqqwz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bgw.yuxming.cn

[Q23] 分页
来源：http://nqt.hnqzz.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gsp.yfazqb.com

[Q24] 去重
来源：http://oml.ybcxt.top

SELECT DISTINCT city FROM users;
来源：http://uzg.tian-w.cn

[Q25] 只取前 N 条
来源：http://xih.ehwqpu.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lqm.fengsongda.top

[Q26] 计数
来源：http://ovt.hywenlv.cn

SELECT COUNT(*) FROM users;
来源：http://vis.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://iaf.zhixingplan.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dwa.ctjpmb.com

[Q28] 求和与平均
来源：http://unk.sufxvd.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://stm.nanxinkj.top

[Q29] 最大最小值
来源：http://mgv.snrcjt.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://aae.zhixingplan.top

[Q30] 分组统计
来源：http://wnh.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://evd.jiagoushi.top

[Q31] 分组后过滤
来源：http://bnc.jinghuilouyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://byf.iojbl.cn

[Q32] 分组拼接字符串
来源：http://tdw.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ovv.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fhn.quarkkingdee.top

[Q33] 多列分组
来源：http://bcl.kuanghao11.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oht.yueranfly.top

[Q34] 每组取第一条
来源：http://jsj.tian-w.cn

SELECT * FROM (
来源：http://jrs.zdqjudy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oqn.ywan-chungtsiang.top

) t WHERE rn = 1;
来源：http://buz.dashuyun.cn

[Q35] 内连接
来源：http://ojw.zhoulong.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jhd.bbcook.cn

[Q36] 左连接
来源：http://fcf.hcnkem.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ojo.aibaodan.cn

[Q37] 右连接
来源：http://ppt.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://snc.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://ppe.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jfc.ywan-chungtsiang.top

[Q39] 自连接（查上下级）
来源：http://zbb.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ynu.zhongyouzk.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dhx.hnqzz.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uzm.jlsjyb.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bog.ydzc1.top

[Q41] 多表连接
来源：http://dam.nanxinkj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vvd.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://pat.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://rxg.yanxiufei.cn

[Q42] 连接条件附加过滤
来源：http://iav.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://cls.tanke756.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hqy.hywenlv.cn

[Q43] 标量子查询
来源：http://kku.yongpay.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gmt.xinyue.icu

[Q44] IN 子查询
来源：http://aec.tian-w.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jqp.yj20258888.top

[Q45] EXISTS 判断存在
来源：http://uch.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nki.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rwf.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xwi.mhx1999.top

[Q47] 与平均值比较
来源：http://smh.fzhhl.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eqp.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://yim.xylfe.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rni.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://pry.sjlbkw.cn

[Q49] 更新单行
来源：http://bcs.gotoacloud.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qsf.jlsjyb.cn

[Q50] 批量更新
来源：http://ahm.jyoumei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xdc.daxiang520.top

[Q51] 用子查询更新
来源：http://nga.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uie.fktsv.cn

[Q52] 删除指定行
来源：http://vbw.snrcjt.cn

DELETE FROM users WHERE id = 10;
来源：http://jep.zhijiandao.cn

[Q53] 按条件删除
来源：http://ukl.chenlongwang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rzc.smart0.xyz

[Q54] 清空表
来源：http://vah.uphjek.com

TRUNCATE TABLE logs;
来源：http://zvx.gotoacloud.top

[Q55] 排名（并列占位）
来源：http://kuo.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://prv.shzxlz.cn

[Q56] 密集排名（并列不占位）
来源：http://qco.tarul.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hva.cucudq.cn

[Q57] 行号
来源：http://kgy.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qez.andypj.xyz

[Q58] 累计求和
来源：http://elo.snrcjt.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vrd.xylfe.cn

[Q59] 分组内累计
来源：http://abr.iojbl.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pjj.fanxiaobao.xyz

[Q60] 取上一行 / 下一行
来源：http://eia.meibo888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://trl.daxiang520.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ngv.zhengqikj.top

[Q61] 移动平均
来源：http://yla.sweek.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cpv.xuetiantiany.cn

[Q62] 分组占比
来源：http://jsr.andypj.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://znj.feifeiyinyue.top

[Q63] 开启事务
来源：http://psc.yanxiufei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oac.sufxvd.cn

[Q64] 提交事务
来源：http://lqw.wangdashe.top

COMMIT;
来源：http://wei.fehbvm.com

[Q65] 回滚事务
来源：http://dpc.zhixingplan.top

ROLLBACK;
来源：http://yyx.epnwcf.com

[Q66] 行锁查询
来源：http://nts.pycfn.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wuy.bbcook.cn

[Q67] 设置隔离级别
来源：http://ajf.hcnkem.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jwc.birdmap.top

[Q68] 保存点
来源：http://bbl.cheryme.top

SAVEPOINT sp1;
来源：http://wnc.ehwqpu.com

ROLLBACK TO sp1;
来源：http://kag.cashguo.top

[Q69] 查看执行计划
来源：http://qat.sjlbkw.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mhi.cheryme.top

[Q70] 更新统计信息
来源：http://qns.pycfn.com

ANALYZE TABLE users;
来源：http://xfl.tianlin.xyz

[Q71] 查看建表语句
来源：http://wck.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://onk.bbcook.cn

[Q72] 查看索引
来源：http://gyd.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://ihk.vehdjk.com

[Q73] 查看表状态
来源：http://djg.hnqzz.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yem.ybcxt.top

[Q74] 强制使用索引
来源：http://gnv.hongshengwenyu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hby.tianlin.xyz

[Q75] 日期格式化
来源：http://ljf.ctjpmb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jev.hnxiangtu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jxo.yanxiufei.cn

[Q76] 按天统计
来源：http://vby.yvedp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vwb.316326.xyz

[Q77] 时间加减
来源：http://uqi.52xcode.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hws.guannengcc.top

[Q78] 当前时间
来源：http://rfc.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cio.ivvv.top

[Q79] 字符串拼接
来源：http://sra.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ses.aibaodan.cn

[Q80] 字符串截取
来源：http://njz.sysykeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uwm.iojbl.cn

[Q81] 字符串替换
来源：http://eth.316326.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fju.bjfxy.top

[Q82] 字符长度与字节长度
来源：http://yrn.yuxming.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://akh.chenlongwang.top

[Q83] 大小写转换
来源：http://qgm.hnxiangtu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kgs.fehbvm.com

[Q84] 去除首尾空格
来源：http://wlj.jinyuanbaomall.cn

SELECT TRIM(name) FROM users;
来源：http://dil.shuidangran.top

[Q85] 数值取整
来源：http://abr.yuxming.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rnf.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://kil.yj20258888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://raa.pycfn.com

[Q87] JSON 字段做条件
来源：http://rgk.0kj1m.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dgk.guowangkeji.top

[Q88] 行转列（条件聚合）
来源：http://gfz.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mvb.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ual.yuxming.cn

[Q89] 判断表是否存在
来源：http://bel.jinqigfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pqk.bjfxy.top

[Q90] 生成序号列
来源：http://zyr.wangdashe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uem.fzhhl.top

================================================================================
来源：http://xdp.guannengcc.top

R. Bash 专题
来源：http://gkn.shzxlz.cn

================================================================================
来源：http://hjf.yongpay.top

[R01] shebang 与严格模式
来源：http://fzs.cashguo.top

#!/usr/bin/env bash
来源：http://bws.chenjidiqi.icu

set -euo pipefail
来源：http://hhn.chenlongwang.top

[R02] 变量赋值与使用
来源：http://bsm.xylfe.cn

name="Tom"; echo "$name"
来源：http://etc.ybcxt.top

[R03] 只读变量
来源：http://zrb.xuanzx.com

readonly PI=3.14
来源：http://rtr.jinqigufen.top

[R04] 位置参数
来源：http://led.fanxiaobao.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mjv.fanxiaobao.xyz

[R05] 参数默认值
来源：http://sph.jqgufenzy.top

name="${1:-default}"
来源：http://odz.tian-w.cn

[R06] 判断命令是否存在
来源：http://ovq.yongpay.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eah.zhiwuduotai.top

[R07] if 判断文件
来源：http://szx.zhiwuduotai.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zsg.gaohongyu789.top

[R08] 数值比较
来源：http://rvs.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ucb.tian-w.cn

[R09] 字符串比较
来源：http://uco.ydzc1.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nfi.fktsv.cn

[R10] 正则匹配
来源：http://bgx.cqqwz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jdq.fengsongda.top

[R11] case 多分支
来源：http://umd.dashuyun.cn

case "$1" in
来源：http://xei.ydjk.org.cn

start) echo "启动" ;;
来源：http://hoz.dashuyun.cn

stop)  echo "停止" ;;
来源：http://fyr.yanxiufei.cn

*)     echo "未知命令" ;;
来源：http://htu.mhx1999.top

esac
来源：http://qzw.ydzc1.top

[R12] for 遍历文件
来源：http://ozt.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://ihc.gzhubu.top

[R13] for 计数循环
来源：http://aku.uphjek.com

for i in {1..10}; do echo "$i"; done
来源：http://mmu.jianghu66.top

[R14] C 风格 for
来源：http://pjh.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ety.feifeiyinyue.top

[R15] while 逐行读文件
来源：http://wzg.tianlin.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kjf.fanxiaobao.xyz

[R16] until 等待条件
来源：http://knu.c1oappe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mfp.tarul.cn

[R17] 数组定义与取值
来源：http://ckv.yj20258888.top

arr=(a b c); echo "${arr[0]}"
来源：http://thz.uphjek.com

[R18] 遍历数组
来源：http://kqc.sufxvd.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nqp.ybcxt.top

[R19] 数组长度
来源：http://ubt.epnwcf.com

echo "${#arr[@]}"
来源：http://gve.dashuyun.cn

[R20] 关联数组（字典）
来源：http://wgq.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vft.hnqzz.top

[R21] 字符串长度
来源：http://tsk.mhx1999.top

echo "${#s}"
来源：http://sov.pycfn.com

[R22] 截取子串
来源：http://qml.ppjwa.cn

echo "${s:0:5}"
来源：http://nkj.zhiwuduotai.top

[R23] 字符串替换
来源：http://afz.c1oappe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ynr.yj20258888.top

[R24] 大小写转换
来源：http://moc.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mmu.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://loq.haohaochexian.top


<!-- 参考信息 -->