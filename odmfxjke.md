代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://xjm.dashuyun.cn

[P02] MD5 / SHA256 摘要
来源：http://jev.epnwcf.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pmr.jinghuilouyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vhs.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://afm.0kj1m.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://syq.hnqzz.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yap.hcnkem.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://thv.jqgfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fpk.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dji.sxryk.cn

[P03] 生成短随机字符串
来源：http://zvx.ehwqpu.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wsb.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://knn.iojbl.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ptt.guannengcc.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hmp.sysykeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tzd.aizwys.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rec.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://icx.epnwcf.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aye.xuanzx.com

[P04] 求长度
来源：http://oet.hnxiangtu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nqc.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gua.nwbrower.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ery.ydzc1.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://voy.andypj.xyz

Java: list.size();  map.size();  s.length()
来源：http://axz.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://its.kuanghao11.cn

Ruby: x.length;  x.size
来源：http://asz.cdnleiting.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xec.gotoacloud.top

[P05] 判断两个对象内容是否相等
来源：http://evz.sxryk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hor.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cqe.fanxiaobao.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sea.feifeiyinyue.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nge.ybcxt.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ggm.jqgfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://fel.hnxiangtu.top

Ruby: a == b
来源：http://def.sysykeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jxv.yuanzhike.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eqh.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wmn.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://ymf.52xcode.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://smf.dianchejie.cn

TS:   if (x == null) {}
来源：http://ldn.gotoacloud.top

Java: if (x == null || x.isEmpty()) {}
来源：http://aii.yuxming.cn

Go:   if x == nil {}
来源：http://daq.yuxming.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pdx.iojbl.cn

C#:   if (x is null) {}
来源：http://ixk.shuidangran.top

[P07] 防抖与节流
来源：http://hxz.daria6918.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qsd.fehbvm.com

PHP:  // 手写时间戳比较
来源：http://zqf.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nwy.fengsongda.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://szh.fktsv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://skq.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nxb.hfpthk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vub.jqgufenzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://krh.haohaochexian.top

[P08] 处理浮点精度问题
来源：http://nch.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eqj.birdmap.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sto.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kaj.zhengqikj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mtw.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ieb.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cjt.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ire.gzhubu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fra.gzhubu.top

================================================================================
来源：http://rfu.gaohongyu789.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kfd.yueranfly.top

================================================================================
来源：http://awb.ybcxt.top

[Q01] 创建表
来源：http://jvh.jiagoushi.top

CREATE TABLE users (
来源：http://fqr.jinghuilouyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rsv.hesvh.cn

name VARCHAR(50) NOT NULL,
来源：http://aeu.smart0.xyz

email VARCHAR(100) UNIQUE,
来源：http://iov.yuxming.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://seh.sxryk.cn

);
来源：http://tvt.haohaochexian.top

[Q02] 创建带外键的表
来源：http://aqq.zhixingplan.top

CREATE TABLE orders (
来源：http://rmg.mhx1999.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fxn.tianlin.xyz

user_id INT NOT NULL,
来源：http://ikf.guannengcc.top

amount DECIMAL(10, 2),
来源：http://fyr.jinqigfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gud.cheryme.top

);
来源：http://jmh.pengpengdd.cyou

[Q03] 增加列
来源：http://mfl.yonumen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://omj.daxiang520.top

[Q04] 修改列类型
来源：http://nsq.yj202588.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pux.xuanzx.com

[Q05] 重命名列
来源：http://ljb.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cpd.gzhubu.top

[Q06] 删除列
来源：http://vrf.jyoumei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://whs.fengsongda.top

[Q07] 删除表
来源：http://cwz.nwbrower.top

DROP TABLE IF EXISTS orders;
来源：http://neq.guowangkeji.top

[Q08] 创建普通索引
来源：http://ayc.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://emc.ywan-chungtsiang.top

[Q09] 创建唯一索引
来源：http://nqo.yanxiufei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qgc.9152youxi.cn

[Q10] 插入单行
来源：http://kyy.jiagoushi.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sis.cheryme.top

[Q11] 一次插入多行
来源：http://xkv.hcnkem.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tva.gogol.net.cn

[Q12] 插入后取自增 ID
来源：http://ezv.quarkkingdee.top

INSERT INTO users (name) VALUES ('C');
来源：http://mcf.birdmap.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ics.gotoacloud.top

[Q13] 忽略重复插入
来源：http://tcw.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://flb.xuanzx.com

[Q14] 存在则更新（upsert）
来源：http://bsu.jyoumei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mpa.tarul.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qam.jinqigufen.top

[Q15] 查询全部
来源：http://rmn.9152youxi.cn

SELECT * FROM users;
来源：http://opg.hnqzz.top

[Q16] 查询指定列
来源：http://ish.cashguo.top

SELECT id, name FROM users;
来源：http://ooe.feifeiyinyue.top

[Q17] 条件查询
来源：http://sfl.feifeiyinyue.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qrb.wangdashe.top

[Q18] 模糊匹配
来源：http://ioi.yongpay.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lym.ivvv.top

[Q19] 范围查询
来源：http://yag.c1oappe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xlt.mhx1999.top

[Q20] IN 列表
来源：http://bmb.gzhubu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kkl.zhongyouzk.top

[Q21] 空值判断
来源：http://nge.redwolf501.top

SELECT * FROM users WHERE email IS NULL;
来源：http://okw.kuanghao11.cn

[Q22] 排序
来源：http://oms.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ytb.yfazqb.com

[Q23] 分页
来源：http://rug.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ura.jinqigfzy.top

[Q24] 去重
来源：http://lds.andypj.xyz

SELECT DISTINCT city FROM users;
来源：http://jhf.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://uib.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ccv.jianghu66.top

[Q26] 计数
来源：http://jyx.yvedp.cn

SELECT COUNT(*) FROM users;
来源：http://ovk.chenlongwang.top

[Q27] 条件计数
来源：http://zmr.tian-w.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cyb.shanyushiyangtech.top

[Q28] 求和与平均
来源：http://hzt.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xtb.hywenlv.cn

[Q29] 最大最小值
来源：http://zmk.tarul.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xcb.svipenyu.cn

[Q30] 分组统计
来源：http://wda.yj20258.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pdj.sxryk.cn

[Q31] 分组后过滤
来源：http://lvq.gogol.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://spj.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://nal.tarul.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://llk.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kqa.sjlbkw.cn

[Q33] 多列分组
来源：http://ghe.aizwys.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tal.jianghu66.top

[Q34] 每组取第一条
来源：http://oux.zhixingplan.top

SELECT * FROM (
来源：http://fgt.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jrf.redwolf501.top

) t WHERE rn = 1;
来源：http://evb.yueranfly.top

[Q35] 内连接
来源：http://veg.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ezh.nanxuanxn.top

[Q36] 左连接
来源：http://sqa.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rwg.52xcode.cn

[Q37] 右连接
来源：http://tlu.daxiang520.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eua.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://moi.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vyf.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://qtg.tarul.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bsj.fengsongda.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mei.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xxc.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cmu.yfazqb.com

[Q41] 多表连接
来源：http://kde.xinyue.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://jqo.gzhubu.top

JOIN users u ON u.id = o.user_id
来源：http://hiu.52xcode.cn

JOIN products p ON p.id = o.product_id;
来源：http://wtd.cheryme.top

[Q42] 连接条件附加过滤
来源：http://omo.zdbjq.cn

SELECT u.name, o.amount FROM users u
来源：http://yzz.xylfe.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hyi.wangdashe.top

[Q43] 标量子查询
来源：http://rey.gzhubu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gbs.hnqzz.top

[Q44] IN 子查询
来源：http://dvh.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zms.aizwys.cn

[Q45] EXISTS 判断存在
来源：http://ogc.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ord.daria6918.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vuu.shanyushiyangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wor.yueranfly.top

[Q47] 与平均值比较
来源：http://acx.ywan-chungtsiang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cuy.uphjek.com

[Q48] CTE 公用表表达式
来源：http://tti.zhaomingkeji.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://chz.nanxuanxn.top

SELECT * FROM t WHERE c > 5;
来源：http://lhv.hnqzz.top

[Q49] 更新单行
来源：http://cjo.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yyh.yj202588.top

[Q50] 批量更新
来源：http://qjd.xziqi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cvx.52xcode.cn

[Q51] 用子查询更新
来源：http://yba.vqdsnc.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rpd.hongshengwenyu.top

[Q52] 删除指定行
来源：http://dod.wangdashe.top

DELETE FROM users WHERE id = 10;
来源：http://flg.52xcode.cn

[Q53] 按条件删除
来源：http://nio.zhoulong.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jxx.ppjwa.cn

[Q54] 清空表
来源：http://rhf.vqdsnc.cn

TRUNCATE TABLE logs;
来源：http://kpf.xinyue.icu

[Q55] 排名（并列占位）
来源：http://nni.vqdsnc.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sic.hfpthk.cn

[Q56] 密集排名（并列不占位）
来源：http://ruf.guowangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nnu.yvedp.cn

[Q57] 行号
来源：http://ohz.meibo888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://abn.hongshengwenyu.top

[Q58] 累计求和
来源：http://qju.ppjwa.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wbw.hfpthk.cn

[Q59] 分组内累计
来源：http://tpq.tianlin.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hwg.zdqjudy.top

[Q60] 取上一行 / 下一行
来源：http://uii.mhx1999.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ayi.shzxlz.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cgv.aibaodan.cn

[Q61] 移动平均
来源：http://ltm.snrcjt.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cii.svipenyu.cn

[Q62] 分组占比
来源：http://ven.zhoulong.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lmu.gogol.net.cn

[Q63] 开启事务
来源：http://xlo.yangfankeji.com

START TRANSACTION;                -- 或 BEGIN
来源：http://foi.jlsjyb.cn

[Q64] 提交事务
来源：http://jgh.svipenyu.cn

COMMIT;
来源：http://fxg.yj20258.top

[Q65] 回滚事务
来源：http://zqd.zycfv.cn

ROLLBACK;
来源：http://knj.fanxiaobao.xyz

[Q66] 行锁查询
来源：http://oqe.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://voc.cheryme.top

[Q67] 设置隔离级别
来源：http://cnk.xinyue.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hsk.bbcook.cn

[Q68] 保存点
来源：http://zie.cashguo.top

SAVEPOINT sp1;
来源：http://zss.yonumen.top

ROLLBACK TO sp1;
来源：http://qex.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://upq.shangyingyoupin.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zcx.jinghuilouyu.cn

[Q70] 更新统计信息
来源：http://vws.shzxlz.cn

ANALYZE TABLE users;
来源：http://bul.fktsv.cn

[Q71] 查看建表语句
来源：http://dmp.tianlin.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xtt.ehwqpu.com

[Q72] 查看索引
来源：http://det.sxryk.cn

SHOW INDEX FROM users;
来源：http://bip.fzhhl.top

[Q73] 查看表状态
来源：http://zrt.xziqi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://olo.nanxuanxn.top

[Q74] 强制使用索引
来源：http://zrs.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lhe.yuxming.cn

[Q75] 日期格式化
来源：http://tmt.yanxiufei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yjf.shuidangran.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pqw.cdnleiting.top

[Q76] 按天统计
来源：http://uys.wangshuangyany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rsz.pycfn.com

[Q77] 时间加减
来源：http://zpa.gaohongyu789.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://krj.yangfankeji.com

[Q78] 当前时间
来源：http://map.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lto.pycfn.com

[Q79] 字符串拼接
来源：http://rkf.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lgg.ybcxt.top

[Q80] 字符串截取
来源：http://kvt.jianghu66.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mji.zdbjq.cn

[Q81] 字符串替换
来源：http://uwy.zdqjudy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uxy.meibo888.top

[Q82] 字符长度与字节长度
来源：http://olh.sufxvd.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wmc.fehbvm.com

[Q83] 大小写转换
来源：http://jxj.fzhhl.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ebi.tian-w.cn

[Q84] 去除首尾空格
来源：http://jbu.9152youxi.cn

SELECT TRIM(name) FROM users;
来源：http://zls.andypj.xyz

[Q85] 数值取整
来源：http://tko.hammf.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tnd.sysykeji.top

[Q86] 读取 JSON 字段
来源：http://xle.jqgufenzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iei.epnwcf.com

[Q87] JSON 字段做条件
来源：http://fau.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jol.zdqjudy.top

[Q88] 行转列（条件聚合）
来源：http://tcd.vehdjk.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ear.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fyw.gogol.net.cn

[Q89] 判断表是否存在
来源：http://bpw.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nwv.nanxuanxn.top

[Q90] 生成序号列
来源：http://top.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pvz.cheryme.top

================================================================================
来源：http://rxm.nanxuanxn.top

R. Bash 专题
来源：http://bzj.vehdjk.com

================================================================================
来源：http://hja.pycfn.com

[R01] shebang 与严格模式
来源：http://vbq.yj202588.top

#!/usr/bin/env bash
来源：http://jgw.zdqjudy.top

set -euo pipefail
来源：http://xpt.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://qjw.jianghu66.top

name="Tom"; echo "$name"
来源：http://pew.svipenyu.cn

[R03] 只读变量
来源：http://qhm.52xcode.cn

readonly PI=3.14
来源：http://rnh.chenjidiqi.icu

[R04] 位置参数
来源：http://tqd.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bdo.birdmap.top

[R05] 参数默认值
来源：http://tpk.52xcode.cn

name="${1:-default}"
来源：http://gej.ivvv.top

[R06] 判断命令是否存在
来源：http://xcd.havefunace.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lnd.yfazqb.com

[R07] if 判断文件
来源：http://gvr.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tzy.chenzaomai.com

[R08] 数值比较
来源：http://xth.zhengqikj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rwo.pengpengdd.cyou

[R09] 字符串比较
来源：http://mwx.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xjf.andypj.xyz

[R10] 正则匹配
来源：http://sgg.ywan-chungtsiang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zbc.ydzc1.top

[R11] case 多分支
来源：http://xfk.sysykeji.top

case "$1" in
来源：http://ezl.daxiang520.top

start) echo "启动" ;;
来源：http://buo.dianchejie.cn

stop)  echo "停止" ;;
来源：http://cot.ehwqpu.com

*)     echo "未知命令" ;;
来源：http://jhf.wangshuangyany.cn


<!-- 参考信息 -->