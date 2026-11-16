代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://elo.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hbx.ydzc1.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ekx.ivvv.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lds.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ceo.tarul.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zdb.tian-w.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kdb.316326.xyz

[P04] 求长度
来源：http://vfm.shuidangran.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mum.hammf.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jjx.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vzg.hnxiangtu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mux.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://yab.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://lsv.yuanzhike.top

Ruby: x.length;  x.size
来源：http://kfa.sweek.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ddl.cdnleiting.top

[P05] 判断两个对象内容是否相等
来源：http://awz.wangshuangyany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://atm.yj20258888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rkt.nanxinkj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aqt.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baj.tianlin.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nbs.quarkkingdee.top

Go:   reflect.DeepEqual(a, b)
来源：http://odp.ydjk.org.cn

Ruby: a == b
来源：http://xqy.ybcxt.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kkk.pengpengdd.cyou

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ety.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tla.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://qjr.zdqjudy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ovh.daria6918.cn

TS:   if (x == null) {}
来源：http://njd.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://erx.chenlongwang.top

Go:   if x == nil {}
来源：http://obd.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jti.fanxiaobao.xyz

C#:   if (x is null) {}
来源：http://xmo.gogol.net.cn

[P07] 防抖与节流
来源：http://pyo.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ove.redwolf501.top

PHP:  // 手写时间戳比较
来源：http://han.guannengcc.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://svl.epnwcf.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zni.snrcjt.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pty.gzhubu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ytw.guowangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://tfn.fzhhl.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://azs.shuidangran.top

[P08] 处理浮点精度问题
来源：http://sji.bjfxy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dep.xinyue.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uxe.0kj1m.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ytl.jyoumei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://srb.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cua.smart0.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tvn.fzhhl.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cxw.kuanghao11.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tgm.cucudq.cn

================================================================================
来源：http://npc.bbcook.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://evp.ybcxt.top

================================================================================
来源：http://gxx.daria6918.cn

[Q01] 创建表
来源：http://fma.uphjek.com

CREATE TABLE users (
来源：http://cwq.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wbp.daria6918.cn

name VARCHAR(50) NOT NULL,
来源：http://otc.vehdjk.com

email VARCHAR(100) UNIQUE,
来源：http://sps.yangfankeji.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://civ.0kj1m.cn

);
来源：http://rfi.xziqi.cn

[Q02] 创建带外键的表
来源：http://iph.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://ngs.xinyue.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lql.shzxlz.cn

user_id INT NOT NULL,
来源：http://ydd.cashguo.top

amount DECIMAL(10, 2),
来源：http://evd.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kpm.daxiang520.top

);
来源：http://kfs.jyoumei.cn

[Q03] 增加列
来源：http://pab.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jgs.bjfxy.top

[Q04] 修改列类型
来源：http://kwd.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hjx.iojbl.cn

[Q05] 重命名列
来源：http://upy.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sxg.9152youxi.cn

[Q06] 删除列
来源：http://amc.nwbrower.top

ALTER TABLE users DROP COLUMN age;
来源：http://vlg.andypj.xyz

[Q07] 删除表
来源：http://sev.jqgufenzy.top

DROP TABLE IF EXISTS orders;
来源：http://vkb.jqgfzy.top

[Q08] 创建普通索引
来源：http://buf.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://nve.yanxiufei.cn

[Q09] 创建唯一索引
来源：http://mee.zhengqikj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://msr.nwbrower.top

[Q10] 插入单行
来源：http://qub.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qqc.jyoumei.cn

[Q11] 一次插入多行
来源：http://qsb.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xti.nanxinkj.top

[Q12] 插入后取自增 ID
来源：http://kfl.hesvh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://azv.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fkp.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://uyn.wangdashe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qif.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://gmj.cdnleiting.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cxv.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://szc.sysykeji.top

[Q15] 查询全部
来源：http://yri.yj20258.top

SELECT * FROM users;
来源：http://uoj.wangshuangyany.cn

[Q16] 查询指定列
来源：http://wbq.hysaishi.cn

SELECT id, name FROM users;
来源：http://suz.dianchejie.cn

[Q17] 条件查询
来源：http://pec.fengsongda.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tqd.cdnleiting.top

[Q18] 模糊匹配
来源：http://ybr.tian-w.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zgi.chenjidiqi.icu

[Q19] 范围查询
来源：http://rok.zdbjq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://twd.jianghu66.top

[Q20] IN 列表
来源：http://xyv.zhiwuduotai.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zlr.yuxming.cn

[Q21] 空值判断
来源：http://ddg.hesvh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://opd.yongpay.top

[Q22] 排序
来源：http://aug.c1oappe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lkx.vehdjk.com

[Q23] 分页
来源：http://vzb.yuxming.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mei.jinyuanbaomall.cn

[Q24] 去重
来源：http://mzb.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://oac.zhongyouzk.top

[Q25] 只取前 N 条
来源：http://iok.shanyushiyangtech.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mwp.shangyingyoupin.top

[Q26] 计数
来源：http://dkb.sufxvd.cn

SELECT COUNT(*) FROM users;
来源：http://roy.quarkkingdee.top

[Q27] 条件计数
来源：http://icf.jinqigfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wbr.yueranfly.top

[Q28] 求和与平均
来源：http://yhq.yfazqb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dbs.quarkkingdee.top

[Q29] 最大最小值
来源：http://tth.tarul.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ayp.tian-w.cn

[Q30] 分组统计
来源：http://nal.kuanghao11.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ioe.yfazqb.com

[Q31] 分组后过滤
来源：http://ebj.andypj.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mna.hnqzz.top

[Q32] 分组拼接字符串
来源：http://hpg.yongpay.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ick.birdmap.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vls.zhaomingkeji.xyz

[Q33] 多列分组
来源：http://cie.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pyi.havefunace.top

[Q34] 每组取第一条
来源：http://hjw.gzhubu.top

SELECT * FROM (
来源：http://soa.jinqigfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lkx.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://sry.cashguo.top

[Q35] 内连接
来源：http://wjd.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ksh.sxryk.cn

[Q36] 左连接
来源：http://ewg.bjfxy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eis.yvedp.cn

[Q37] 右连接
来源：http://sga.jinqigufen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yqg.epnwcf.com

[Q38] 全外连接（PostgreSQL）
来源：http://gkg.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zfi.cucudq.cn

[Q39] 自连接（查上下级）
来源：http://sdz.jianghu66.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wur.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xbi.zhengqikj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tbk.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://use.yangfankeji.com

[Q41] 多表连接
来源：http://ofv.jinghuilouyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jpo.fengsongda.top

JOIN users u ON u.id = o.user_id
来源：http://zwx.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://hac.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://zfx.uphjek.com

SELECT u.name, o.amount FROM users u
来源：http://yiw.wangdashe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kvn.ctjpmb.com

[Q43] 标量子查询
来源：http://klb.316326.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nuj.aibaodan.cn

[Q44] IN 子查询
来源：http://nfq.guowangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ixk.hfpthk.cn

[Q45] EXISTS 判断存在
来源：http://cqa.dianchejie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yjv.aizwys.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zjn.gotoacloud.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://csp.sxryk.cn

[Q47] 与平均值比较
来源：http://rmh.tianlin.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zhv.cqqwz.cn

[Q48] CTE 公用表表达式
来源：http://rhf.shzxlz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ygs.xinyue.icu

SELECT * FROM t WHERE c > 5;
来源：http://iqd.wangshuangyany.cn

[Q49] 更新单行
来源：http://own.quarkkingdee.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zyq.wangdashe.top

[Q50] 批量更新
来源：http://chv.daria6918.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ivo.yanxiufei.cn

[Q51] 用子查询更新
来源：http://gme.tarul.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uhb.hongshengwenyu.top

[Q52] 删除指定行
来源：http://csg.haohaochexian.top

DELETE FROM users WHERE id = 10;
来源：http://tcc.yangfankeji.com

[Q53] 按条件删除
来源：http://mgt.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tjx.chenlongwang.top

[Q54] 清空表
来源：http://yyh.jqgfzy.top

TRUNCATE TABLE logs;
来源：http://pkg.vqdsnc.cn

[Q55] 排名（并列占位）
来源：http://vow.jqgufenzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kmc.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://sin.jianghu66.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://brj.shzxlz.cn

[Q57] 行号
来源：http://fpg.sysykeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xca.fanxiaobao.xyz

[Q58] 累计求和
来源：http://ncy.zycfv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qnv.sysykeji.top

[Q59] 分组内累计
来源：http://amq.meibo888.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dho.9152youxi.cn

[Q60] 取上一行 / 下一行
来源：http://rec.feifeiyinyue.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bky.chenlongwang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ysu.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://eor.vehdjk.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jej.hywenlv.cn

[Q62] 分组占比
来源：http://cto.jinyuanbaomall.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ddh.chenlongwang.top

[Q63] 开启事务
来源：http://qpx.yfazqb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://asi.sysykeji.top

[Q64] 提交事务
来源：http://hgr.tarul.cn

COMMIT;
来源：http://pmx.tanke756.top

[Q65] 回滚事务
来源：http://aff.bjfxy.top

ROLLBACK;
来源：http://rpx.fzhhl.top

[Q66] 行锁查询
来源：http://fcs.chenjidiqi.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vnm.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://ubm.daria6918.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://shu.yueranfly.top

[Q68] 保存点
来源：http://vyl.yfazqb.com

SAVEPOINT sp1;
来源：http://hql.kuanghao11.cn

ROLLBACK TO sp1;
来源：http://ctk.jinqigufen.top

[Q69] 查看执行计划
来源：http://uus.ydzc1.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://swl.aizwys.cn

[Q70] 更新统计信息
来源：http://iax.bbcook.cn

ANALYZE TABLE users;
来源：http://klf.xuetiantiany.cn

[Q71] 查看建表语句
来源：http://uju.quarkkingdee.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dpm.cucudq.cn

[Q72] 查看索引
来源：http://ncu.mhx1999.top

SHOW INDEX FROM users;
来源：http://aqj.bbcook.cn

[Q73] 查看表状态
来源：http://axd.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wmn.mhx1999.top

[Q74] 强制使用索引
来源：http://qmr.havefunace.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pse.jianghu66.top

[Q75] 日期格式化
来源：http://mcn.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kal.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://emw.cheryme.top

[Q76] 按天统计
来源：http://lqc.uphjek.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ksz.bbcook.cn

[Q77] 时间加减
来源：http://hxt.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dpk.wangshuangyany.cn

[Q78] 当前时间
来源：http://lcz.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wie.jinghuilouyu.cn

[Q79] 字符串拼接
来源：http://mxk.bbcook.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://njj.316326.xyz

[Q80] 字符串截取
来源：http://hvk.zhoulong.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://swr.pycfn.com

[Q81] 字符串替换
来源：http://pje.vqdsnc.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rhr.epnwcf.com

[Q82] 字符长度与字节长度
来源：http://kmt.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wtl.cheryme.top

[Q83] 大小写转换
来源：http://knp.ybcxt.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blw.xinyue.icu

[Q84] 去除首尾空格
来源：http://kmo.zdbjq.cn

SELECT TRIM(name) FROM users;
来源：http://xme.chenzaomai.com

[Q85] 数值取整
来源：http://gdy.yueranfly.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ces.hywenlv.cn

[Q86] 读取 JSON 字段
来源：http://bbm.fehbvm.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bug.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://kvn.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ews.zhixingplan.top

[Q88] 行转列（条件聚合）
来源：http://spp.zhijiandao.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jry.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ehu.jinqigufen.top

[Q89] 判断表是否存在
来源：http://gmb.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dne.dashuyun.cn

[Q90] 生成序号列
来源：http://ror.gzhubu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nio.gogol.net.cn

================================================================================
来源：http://jpk.xinyue.icu

R. Bash 专题
来源：http://mri.svipenyu.cn

================================================================================
来源：http://hfz.jyoumei.cn

[R01] shebang 与严格模式
来源：http://xju.chenjidiqi.icu

#!/usr/bin/env bash
来源：http://cwd.c1oappe.top

set -euo pipefail
来源：http://dec.tian-w.cn

[R02] 变量赋值与使用
来源：http://dxt.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://vqq.tianlin.xyz

[R03] 只读变量
来源：http://nea.hnxiangtu.top

readonly PI=3.14
来源：http://vrd.tanke756.top

[R04] 位置参数
来源：http://cys.zhijiandao.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iae.shangyingyoupin.top

[R05] 参数默认值
来源：http://frp.wangshuangyany.cn

name="${1:-default}"
来源：http://oqv.316326.xyz

[R06] 判断命令是否存在
来源：http://qse.fktsv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ode.jinqigufen.top

[R07] if 判断文件
来源：http://gyr.meibo888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sdh.yj202588.top

[R08] 数值比较
来源：http://yzh.zhoulong.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://yik.jinghuilouyu.cn

[R09] 字符串比较
来源：http://wuq.hywenlv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qey.hcnkem.com

[R10] 正则匹配
来源：http://fve.bjfxy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sdp.jqgfzy.top

[R11] case 多分支
来源：http://sqw.cucudq.cn

case "$1" in
来源：http://uub.hywenlv.cn

start) echo "启动" ;;
来源：http://tnw.ybcxt.top

stop)  echo "停止" ;;
来源：http://gvz.0kj1m.cn

*)     echo "未知命令" ;;
来源：http://rrq.xinyue.icu

esac
来源：http://zfl.wangdashe.top

[R12] for 遍历文件
来源：http://anz.guowangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://lwy.tarul.cn

[R13] for 计数循环
来源：http://jpp.smart0.xyz

for i in {1..10}; do echo "$i"; done
来源：http://qeg.uphjek.com

[R14] C 风格 for
来源：http://wfh.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qxh.fktsv.cn

[R15] while 逐行读文件
来源：http://yni.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://okg.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://amt.aizwys.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ssq.zhoulong.xyz

[R17] 数组定义与取值
来源：http://ytq.yanxiufei.cn


<!-- 参考信息 -->