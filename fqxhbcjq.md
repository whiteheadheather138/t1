代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eru.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kgr.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cap.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lll.cucudq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lfm.epnwcf.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://mbs.zhijiandao.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ood.pengpengdd.cyou

[P04] 求长度
来源：http://flk.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jxr.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kak.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fqi.ybcxt.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yft.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://mom.zhiwuduotai.top

Go:   len(arr);  len(m)
来源：http://dtp.uphjek.com

Ruby: x.length;  x.size
来源：http://qxq.cdnleiting.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ftx.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://ksh.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hkb.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cov.quarkkingdee.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://idr.yanxiufei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ztw.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tnt.zycfv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kdz.fanxiaobao.xyz

Ruby: a == b
来源：http://vaa.ywan-chungtsiang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pqh.yuanzhike.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nwh.yanxiufei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://suq.cqqwz.cn

PHP:  if (empty($x)) {}
来源：http://rng.ehwqpu.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://alh.tian-w.cn

TS:   if (x == null) {}
来源：http://xoj.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://okt.9152youxi.cn

Go:   if x == nil {}
来源：http://lzw.fengsongda.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rxx.bbcook.cn

C#:   if (x is null) {}
来源：http://asa.zhixingplan.top

[P07] 防抖与节流
来源：http://yox.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aiw.uphjek.com

PHP:  // 手写时间戳比较
来源：http://krb.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lbl.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vmw.xziqi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://juc.zdqjudy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tbj.zhongyouzk.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rai.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vmy.dianchejie.cn

[P08] 处理浮点精度问题
来源：http://sag.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vrg.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fgk.hfpthk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tjr.ehwqpu.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rwb.9152youxi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rxo.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qhw.sxryk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ewq.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nao.hesvh.cn

================================================================================
来源：http://kps.sxryk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tvp.ctjpmb.com

================================================================================
来源：http://ksj.snrcjt.cn

[Q01] 创建表
来源：http://szw.vehdjk.com

CREATE TABLE users (
来源：http://azb.yfazqb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://efr.tianlin.xyz

name VARCHAR(50) NOT NULL,
来源：http://aem.cashguo.top

email VARCHAR(100) UNIQUE,
来源：http://hhs.snrcjt.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hlj.havefunace.top

);
来源：http://kly.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://qcw.zhijiandao.cn

CREATE TABLE orders (
来源：http://dkv.zhiwuduotai.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://znm.nwbrower.top

user_id INT NOT NULL,
来源：http://xzz.shuidangran.top

amount DECIMAL(10, 2),
来源：http://son.yj20258.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lfv.ydjk.org.cn

);
来源：http://ehi.fzhhl.top

[Q03] 增加列
来源：http://ncq.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wpe.chenjidiqi.icu

[Q04] 修改列类型
来源：http://zwm.meibo888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://arg.daxiang520.top

[Q05] 重命名列
来源：http://lba.svipenyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gpw.havefunace.top

[Q06] 删除列
来源：http://vil.pengpengdd.cyou

ALTER TABLE users DROP COLUMN age;
来源：http://alt.meibo888.top

[Q07] 删除表
来源：http://rxm.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://ijn.9152youxi.cn

[Q08] 创建普通索引
来源：http://ezf.uphjek.com

CREATE INDEX idx_users_email ON users(email);
来源：http://awc.yonumen.top

[Q09] 创建唯一索引
来源：http://phr.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eeb.iojbl.cn

[Q10] 插入单行
来源：http://orq.hesvh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ffi.epnwcf.com

[Q11] 一次插入多行
来源：http://myo.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://suz.kuanghao11.cn

[Q12] 插入后取自增 ID
来源：http://bea.ehwqpu.com

INSERT INTO users (name) VALUES ('C');
来源：http://osx.zdbjq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ssk.tianlin.xyz

[Q13] 忽略重复插入
来源：http://sqj.jqgufenzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://axb.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://nok.smart0.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gdz.chenlongwang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kmi.meibo888.top

[Q15] 查询全部
来源：http://gbs.tian-w.cn

SELECT * FROM users;
来源：http://vvc.sxryk.cn

[Q16] 查询指定列
来源：http://adm.ydzc1.top

SELECT id, name FROM users;
来源：http://dxe.jqgufenzy.top

[Q17] 条件查询
来源：http://vbw.quarkkingdee.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ydw.yonumen.top

[Q18] 模糊匹配
来源：http://xuu.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dla.zhijiandao.cn

[Q19] 范围查询
来源：http://nkk.daxiang520.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://arh.yueranfly.top

[Q20] IN 列表
来源：http://nxf.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tkf.svipenyu.cn

[Q21] 空值判断
来源：http://dni.pycfn.com

SELECT * FROM users WHERE email IS NULL;
来源：http://aor.jqgufenzy.top

[Q22] 排序
来源：http://pvc.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ifw.yonumen.top

[Q23] 分页
来源：http://kqm.guowangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wxf.redwolf501.top

[Q24] 去重
来源：http://pxc.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://bdy.jlsjyb.cn

[Q25] 只取前 N 条
来源：http://ceh.jlsjyb.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zty.tarul.cn

[Q26] 计数
来源：http://poq.uphjek.com

SELECT COUNT(*) FROM users;
来源：http://cgd.zhoulong.xyz

[Q27] 条件计数
来源：http://wuz.xuanzx.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tjm.ehwqpu.com

[Q28] 求和与平均
来源：http://hll.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oeq.andypj.xyz

[Q29] 最大最小值
来源：http://jur.dianchejie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qgp.vehdjk.com

[Q30] 分组统计
来源：http://wqd.ivvv.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jge.ppjwa.cn

[Q31] 分组后过滤
来源：http://dmy.uphjek.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hym.birdmap.top

[Q32] 分组拼接字符串
来源：http://vgt.jianghu66.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cdp.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xdt.yj202588.top

[Q33] 多列分组
来源：http://ngv.fzhhl.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nml.jinqigufen.top

[Q34] 每组取第一条
来源：http://oln.jyoumei.cn

SELECT * FROM (
来源：http://dvj.jinghuilouyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xqi.kuanghao11.cn

) t WHERE rn = 1;
来源：http://eds.zhengqikj.top

[Q35] 内连接
来源：http://irf.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zzo.fktsv.cn

[Q36] 左连接
来源：http://vps.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://axj.ppjwa.cn

[Q37] 右连接
来源：http://znp.dianchejie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uyy.ywan-chungtsiang.top

[Q38] 全外连接（PostgreSQL）
来源：http://ixx.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nfw.zhoulong.xyz

[Q39] 自连接（查上下级）
来源：http://msi.yonumen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tev.aibaodan.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xsc.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uui.iojbl.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ozu.cucudq.cn

[Q41] 多表连接
来源：http://hhc.fanxiaobao.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://zzc.epnwcf.com

JOIN users u ON u.id = o.user_id
来源：http://ahd.ywan-chungtsiang.top

JOIN products p ON p.id = o.product_id;
来源：http://jps.pycfn.com

[Q42] 连接条件附加过滤
来源：http://kvu.cucudq.cn

SELECT u.name, o.amount FROM users u
来源：http://wjt.tianlin.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dqz.jinghuilouyu.cn

[Q43] 标量子查询
来源：http://yxc.bjfxy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bhn.sjlbkw.cn

[Q44] IN 子查询
来源：http://qmv.316326.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mnp.smart0.xyz

[Q45] EXISTS 判断存在
来源：http://wfv.quarkkingdee.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://trd.chenlongwang.top

[Q46] NOT EXISTS 判断不存在
来源：http://ixs.aizwys.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rck.gzhubu.top

[Q47] 与平均值比较
来源：http://exh.ywan-chungtsiang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dzn.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://kkv.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xpp.yj20258888.top

SELECT * FROM t WHERE c > 5;
来源：http://you.jqgufenzy.top

[Q49] 更新单行
来源：http://juo.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rqp.gzhubu.top

[Q50] 批量更新
来源：http://uhr.xuanzx.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yar.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://ehg.nanxinkj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nvm.pengpengdd.cyou

[Q52] 删除指定行
来源：http://ohk.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://awu.yueranfly.top

[Q53] 按条件删除
来源：http://cac.andypj.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ktx.zdqjudy.top

[Q54] 清空表
来源：http://wtu.ybcxt.top

TRUNCATE TABLE logs;
来源：http://kzu.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://dqs.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://irw.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://lkp.yanxiufei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wfo.xziqi.cn

[Q57] 行号
来源：http://jig.shangyingyoupin.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vcz.zdbjq.cn

[Q58] 累计求和
来源：http://mig.ctjpmb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eqt.dashuyun.cn

[Q59] 分组内累计
来源：http://uws.daria6918.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yxv.ehwqpu.com

[Q60] 取上一行 / 下一行
来源：http://kgy.hammf.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jfs.feifeiyinyue.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dlo.316326.xyz

[Q61] 移动平均
来源：http://jdd.52xcode.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rqi.zhijiandao.cn

[Q62] 分组占比
来源：http://sfy.ydjk.org.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fqe.shanyushiyangtech.top

[Q63] 开启事务
来源：http://llv.chenjidiqi.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://vnh.kuanghao11.cn

[Q64] 提交事务
来源：http://swa.fzhhl.top

COMMIT;
来源：http://kbr.hesvh.cn

[Q65] 回滚事务
来源：http://uhw.nwbrower.top

ROLLBACK;
来源：http://fbd.hfpthk.cn

[Q66] 行锁查询
来源：http://qwo.ehwqpu.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tme.daria6918.cn

[Q67] 设置隔离级别
来源：http://zdc.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ghf.meibo888.top

[Q68] 保存点
来源：http://unw.quarkkingdee.top

SAVEPOINT sp1;
来源：http://fpa.dashuyun.cn

ROLLBACK TO sp1;
来源：http://gui.snrcjt.cn

[Q69] 查看执行计划
来源：http://ibu.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bhk.sxryk.cn

[Q70] 更新统计信息
来源：http://caz.xziqi.cn

ANALYZE TABLE users;
来源：http://kny.zhengqikj.top

[Q71] 查看建表语句
来源：http://jms.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ywy.yonumen.top

[Q72] 查看索引
来源：http://qhm.guowangkeji.top

SHOW INDEX FROM users;
来源：http://pbf.hongshengwenyu.top

[Q73] 查看表状态
来源：http://pcw.vqdsnc.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xkz.chenjidiqi.icu

[Q74] 强制使用索引
来源：http://wpy.meibo888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oml.hnxiangtu.top

[Q75] 日期格式化
来源：http://aqt.xuetiantiany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eud.dianchejie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://unq.yj20258.top

[Q76] 按天统计
来源：http://gux.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iqt.shanyushiyangtech.top

[Q77] 时间加减
来源：http://pil.hnqzz.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tut.xziqi.cn

[Q78] 当前时间
来源：http://pmq.daria6918.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ven.fengsongda.top

[Q79] 字符串拼接
来源：http://ddk.yuanzhike.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ndk.0kj1m.cn

[Q80] 字符串截取
来源：http://sei.redwolf501.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pae.yueranfly.top

[Q81] 字符串替换
来源：http://oaf.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vxa.birdmap.top

[Q82] 字符长度与字节长度
来源：http://qiz.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kzx.smart0.xyz

[Q83] 大小写转换
来源：http://ccp.daria6918.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dbx.xinyue.icu

[Q84] 去除首尾空格
来源：http://dms.jqgufenzy.top

SELECT TRIM(name) FROM users;
来源：http://vmb.zhaomingkeji.xyz

[Q85] 数值取整
来源：http://xwr.yueranfly.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vwd.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://uyq.yj202588.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eqb.tianlin.xyz

[Q87] JSON 字段做条件
来源：http://ogx.yueranfly.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dyh.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://jno.cucudq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oai.hnqzz.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qtu.jinqigufen.top

[Q89] 判断表是否存在
来源：http://ezd.xuanzx.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wuo.hcnkem.com

[Q90] 生成序号列
来源：http://tzd.cheryme.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gqr.shzxlz.cn

================================================================================
来源：http://bpi.tian-w.cn

R. Bash 专题
来源：http://liu.chenzaomai.com

================================================================================
来源：http://gkl.yfazqb.com

[R01] shebang 与严格模式
来源：http://xpi.ehwqpu.com

#!/usr/bin/env bash
来源：http://arj.nwbrower.top

set -euo pipefail
来源：http://bpe.zdqjudy.top

[R02] 变量赋值与使用
来源：http://qgo.svipenyu.cn

name="Tom"; echo "$name"
来源：http://ack.yfazqb.com

[R03] 只读变量
来源：http://wau.cdnleiting.top

readonly PI=3.14
来源：http://rkv.hnqzz.top

[R04] 位置参数
来源：http://dvj.cashguo.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ful.yj202588.top

[R05] 参数默认值
来源：http://egb.zhaomingkeji.xyz

name="${1:-default}"
来源：http://spy.dianchejie.cn

[R06] 判断命令是否存在
来源：http://cco.yuxming.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mqo.pengpengdd.cyou

[R07] if 判断文件
来源：http://nqn.sweek.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://juy.ywan-chungtsiang.top

[R08] 数值比较
来源：http://nik.yanxiufei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://twc.mhx1999.top

[R09] 字符串比较
来源：http://mko.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://que.chenzaomai.com

[R10] 正则匹配
来源：http://nno.mhx1999.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zgx.svipenyu.cn

[R11] case 多分支
来源：http://blh.hongshengwenyu.top

case "$1" in
来源：http://swx.pycfn.com

start) echo "启动" ;;
来源：http://vqq.ydzc1.top

stop)  echo "停止" ;;
来源：http://tnx.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://uni.jinqigfzy.top

esac
来源：http://vaw.yanxiufei.cn

[R12] for 遍历文件
来源：http://zid.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://nzo.jinqigfzy.top

[R13] for 计数循环
来源：http://fkk.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://uny.9152youxi.cn

[R14] C 风格 for
来源：http://xfh.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vpz.jyoumei.cn

[R15] while 逐行读文件
来源：http://cln.gotoacloud.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jzj.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://pdr.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cjd.sufxvd.cn

[R17] 数组定义与取值
来源：http://bxr.fktsv.cn


<!-- 参考信息 -->