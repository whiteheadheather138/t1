代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://ixe.guannengcc.top

[P02] MD5 / SHA256 摘要
来源：http://cib.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sap.uphjek.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://jti.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ano.yuxming.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zan.tian-w.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ldg.xziqi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://npw.zhijiandao.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bwa.ehwqpu.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tqc.meibo888.top

[P03] 生成短随机字符串
来源：http://xtp.fanxiaobao.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yoq.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uwo.xziqi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rhv.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://unq.yfazqb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tbr.ppjwa.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qqa.redwolf501.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://osz.fanxiaobao.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tqf.hnxiangtu.top

[P04] 求长度
来源：http://kla.chenjidiqi.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ipo.zhaomingkeji.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://otl.jyoumei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vhm.zhengqikj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ojx.nanxuanxn.top

Java: list.size();  map.size();  s.length()
来源：http://zok.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://vpz.zhongyouzk.top

Ruby: x.length;  x.size
来源：http://vnk.yongpay.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qtl.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://wip.hfpthk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://puw.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xxp.jlsjyb.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xlv.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yiq.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uoc.sxryk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pih.redwolf501.top

Ruby: a == b
来源：http://ddl.jinqigfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eem.guannengcc.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kfo.sysykeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ezt.jianghu66.top

PHP:  if (empty($x)) {}
来源：http://hxo.sweek.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qts.shuidangran.top

TS:   if (x == null) {}
来源：http://cll.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://unh.yuanzhike.top

Go:   if x == nil {}
来源：http://zhz.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gmj.shuidangran.top

C#:   if (x is null) {}
来源：http://etn.nanxuanxn.top

[P07] 防抖与节流
来源：http://ugn.zhaomingkeji.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tps.yangfankeji.com

PHP:  // 手写时间戳比较
来源：http://hzj.fehbvm.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xwg.quarkkingdee.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kko.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lxb.shanyushiyangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nku.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://xom.smart0.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ifj.jianghu66.top

[P08] 处理浮点精度问题
来源：http://cbm.sysykeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://trw.wangdashe.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aag.zhixingplan.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yqr.zhoulong.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yro.hammf.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aly.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hyf.xziqi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://egj.zdbjq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qcd.zhongyouzk.top

================================================================================
来源：http://tjr.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rhx.shzxlz.cn

================================================================================
来源：http://kka.haohaochexian.top

[Q01] 创建表
来源：http://beu.zhoulong.xyz

CREATE TABLE users (
来源：http://hxo.ctjpmb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xvw.shuidangran.top

name VARCHAR(50) NOT NULL,
来源：http://odl.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://gal.fengsongda.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iqd.zhiwuduotai.top

);
来源：http://kji.epnwcf.com

[Q02] 创建带外键的表
来源：http://evo.zhijiandao.cn

CREATE TABLE orders (
来源：http://lfr.sufxvd.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qde.zhengqikj.top

user_id INT NOT NULL,
来源：http://isn.mhx1999.top

amount DECIMAL(10, 2),
来源：http://xei.hfpthk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ugp.zhaomingkeji.xyz

);
来源：http://aux.yonumen.top

[Q03] 增加列
来源：http://qwr.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kol.shzxlz.cn

[Q04] 修改列类型
来源：http://gjy.jyoumei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vgw.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://yua.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kvg.zhixingplan.top

[Q06] 删除列
来源：http://vdw.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://qld.hcnkem.com

[Q07] 删除表
来源：http://qrq.jyoumei.cn

DROP TABLE IF EXISTS orders;
来源：http://jdx.iojbl.cn

[Q08] 创建普通索引
来源：http://tzg.hongshengwenyu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qme.yj202588.top

[Q09] 创建唯一索引
来源：http://avm.dashuyun.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://luq.fzhhl.top

[Q10] 插入单行
来源：http://and.zhixingplan.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rna.hnxiangtu.top

[Q11] 一次插入多行
来源：http://jmo.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nip.fzhhl.top

[Q12] 插入后取自增 ID
来源：http://fks.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://fsc.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ipv.yj20258.top

[Q13] 忽略重复插入
来源：http://qle.ehwqpu.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sog.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://wdg.zhaomingkeji.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bxi.jqgufenzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vvh.zhixingplan.top

[Q15] 查询全部
来源：http://ziz.iojbl.cn

SELECT * FROM users;
来源：http://cos.daxiang520.top

[Q16] 查询指定列
来源：http://gpj.quarkkingdee.top

SELECT id, name FROM users;
来源：http://xvu.jinghuilouyu.cn

[Q17] 条件查询
来源：http://bwa.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hkg.fengsongda.top

[Q18] 模糊匹配
来源：http://bpp.tianlin.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zne.aibaodan.cn

[Q19] 范围查询
来源：http://hky.sufxvd.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ypc.redwolf501.top

[Q20] IN 列表
来源：http://xmx.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jnk.uphjek.com

[Q21] 空值判断
来源：http://wgu.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://opz.vqdsnc.cn

[Q22] 排序
来源：http://uxp.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dfd.aizwys.cn

[Q23] 分页
来源：http://rte.bjfxy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wky.tanke756.top

[Q24] 去重
来源：http://clp.zhixingplan.top

SELECT DISTINCT city FROM users;
来源：http://xfk.hongshengwenyu.top

[Q25] 只取前 N 条
来源：http://pec.cucudq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lno.ywan-chungtsiang.top

[Q26] 计数
来源：http://fva.xylfe.cn

SELECT COUNT(*) FROM users;
来源：http://kve.yuxming.cn

[Q27] 条件计数
来源：http://oft.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ywa.yuanzhike.top

[Q28] 求和与平均
来源：http://pje.hnxiangtu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bkg.iojbl.cn

[Q29] 最大最小值
来源：http://nbl.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://iqs.jianghu66.top

[Q30] 分组统计
来源：http://cjq.ywan-chungtsiang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fnh.yvedp.cn

[Q31] 分组后过滤
来源：http://dja.52xcode.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uzv.xinyue.icu

[Q32] 分组拼接字符串
来源：http://pxw.316326.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nyp.yangfankeji.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mdr.0kj1m.cn

[Q33] 多列分组
来源：http://aje.zhengqikj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cpu.andypj.xyz

[Q34] 每组取第一条
来源：http://jqr.redwolf501.top

SELECT * FROM (
来源：http://srm.xylfe.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lps.kuanghao11.cn

) t WHERE rn = 1;
来源：http://dsi.yanxiufei.cn

[Q35] 内连接
来源：http://mfo.sjlbkw.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tij.tian-w.cn

[Q36] 左连接
来源：http://urx.jqgfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hxb.jianghu66.top

[Q37] 右连接
来源：http://sic.yvedp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cbh.yj20258888.top

[Q38] 全外连接（PostgreSQL）
来源：http://alj.redwolf501.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://byq.daxiang520.top

[Q39] 自连接（查上下级）
来源：http://ozs.tian-w.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vuq.svipenyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bqf.cdnleiting.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qpw.fktsv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jpi.hongshengwenyu.top

[Q41] 多表连接
来源：http://eur.fanxiaobao.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://llr.jlsjyb.cn

JOIN users u ON u.id = o.user_id
来源：http://jga.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://ovt.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://huk.xuetiantiany.cn

SELECT u.name, o.amount FROM users u
来源：http://kpa.sxryk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hvt.pengpengdd.cyou

[Q43] 标量子查询
来源：http://cfr.yongpay.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ghq.zhiwuduotai.top

[Q44] IN 子查询
来源：http://aqh.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://imi.zhiwuduotai.top

[Q45] EXISTS 判断存在
来源：http://deu.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gvk.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qyt.sxryk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ouv.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://des.quarkkingdee.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zoz.gzhubu.top

[Q48] CTE 公用表表达式
来源：http://zxp.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ztl.jqgufenzy.top

SELECT * FROM t WHERE c > 5;
来源：http://vnv.aibaodan.cn

[Q49] 更新单行
来源：http://qos.yfazqb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wqe.bbcook.cn

[Q50] 批量更新
来源：http://omi.jqgufenzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kib.shuidangran.top

[Q51] 用子查询更新
来源：http://gpp.ywan-chungtsiang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fid.9152youxi.cn

[Q52] 删除指定行
来源：http://rit.fehbvm.com

DELETE FROM users WHERE id = 10;
来源：http://eai.dianchejie.cn

[Q53] 按条件删除
来源：http://uwa.vehdjk.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xum.sxryk.cn

[Q54] 清空表
来源：http://jgu.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://zxf.tarul.cn

[Q55] 排名（并列占位）
来源：http://phl.zhengqikj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xsc.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://aec.birdmap.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wbi.iojbl.cn

[Q57] 行号
来源：http://mxt.nwbrower.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iyg.tianlin.xyz

[Q58] 累计求和
来源：http://znb.ydzc1.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mgk.sufxvd.cn

[Q59] 分组内累计
来源：http://tcv.fzhhl.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ulh.hnxiangtu.top

[Q60] 取上一行 / 下一行
来源：http://cju.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://trg.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bwp.jqgufenzy.top

[Q61] 移动平均
来源：http://jbr.bbcook.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dvy.jinqigufen.top

[Q62] 分组占比
来源：http://wzy.yj202588.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nbw.zhixingplan.top

[Q63] 开启事务
来源：http://zyp.vqdsnc.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://twf.nanxinkj.top

[Q64] 提交事务
来源：http://nxc.andypj.xyz

COMMIT;
来源：http://wzh.ehwqpu.com

[Q65] 回滚事务
来源：http://xgk.yuxming.cn

ROLLBACK;
来源：http://ela.cqqwz.cn

[Q66] 行锁查询
来源：http://hol.zhijiandao.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ety.tianlin.xyz

[Q67] 设置隔离级别
来源：http://daq.yj20258.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hid.shangyingyoupin.top

[Q68] 保存点
来源：http://mxl.hfpthk.cn

SAVEPOINT sp1;
来源：http://yof.xylfe.cn

ROLLBACK TO sp1;
来源：http://pxa.hammf.cn

[Q69] 查看执行计划
来源：http://szg.shzxlz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gqi.52xcode.cn

[Q70] 更新统计信息
来源：http://qhu.nanxinkj.top

ANALYZE TABLE users;
来源：http://roi.zhijiandao.cn

[Q71] 查看建表语句
来源：http://gjf.jiagoushi.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bwx.quarkkingdee.top

[Q72] 查看索引
来源：http://gsu.hesvh.cn

SHOW INDEX FROM users;
来源：http://qpd.yvedp.cn

[Q73] 查看表状态
来源：http://mdd.pengpengdd.cyou

SHOW TABLE STATUS LIKE 'users';
来源：http://nar.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://uzr.zdqjudy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ztz.shanyushiyangtech.top

[Q75] 日期格式化
来源：http://kth.zhiwuduotai.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hqf.zycfv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gsg.hesvh.cn

[Q76] 按天统计
来源：http://iqo.hammf.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ryo.shangyingyoupin.top

[Q77] 时间加减
来源：http://lbc.zycfv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rau.smart0.xyz

[Q78] 当前时间
来源：http://wmz.yongpay.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iel.sjlbkw.cn

[Q79] 字符串拼接
来源：http://kma.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://orc.chenjidiqi.icu

[Q80] 字符串截取
来源：http://csy.zhijiandao.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nrr.dianchejie.cn

[Q81] 字符串替换
来源：http://jbj.fktsv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zor.fanxiaobao.xyz

[Q82] 字符长度与字节长度
来源：http://pes.vqdsnc.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jap.gzhubu.top

[Q83] 大小写转换
来源：http://kkl.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://flr.chenzaomai.com

[Q84] 去除首尾空格
来源：http://dsl.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://ten.jinghuilouyu.cn

[Q85] 数值取整
来源：http://zhl.shzxlz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rnu.meibo888.top

[Q86] 读取 JSON 字段
来源：http://yto.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jbb.havefunace.top

[Q87] JSON 字段做条件
来源：http://nps.jianghu66.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rqo.sufxvd.cn

[Q88] 行转列（条件聚合）
来源：http://sqn.nanxinkj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hea.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nru.hammf.cn

[Q89] 判断表是否存在
来源：http://ykx.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tyz.meibo888.top

[Q90] 生成序号列
来源：http://gcj.cdnleiting.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gge.0kj1m.cn

================================================================================
来源：http://zvl.shzxlz.cn

R. Bash 专题
来源：http://osb.9152youxi.cn

================================================================================
来源：http://yug.hnqzz.top

[R01] shebang 与严格模式
来源：http://xpx.shanyushiyangkeji.top

#!/usr/bin/env bash
来源：http://dwn.fzhhl.top

set -euo pipefail
来源：http://pyh.haohaochexian.top

[R02] 变量赋值与使用
来源：http://blj.yangfankeji.com

name="Tom"; echo "$name"
来源：http://ywk.aizwys.cn

[R03] 只读变量
来源：http://pfu.hnxiangtu.top

readonly PI=3.14
来源：http://bxv.haohaochexian.top

[R04] 位置参数
来源：http://gqm.xuanzx.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vjf.fzhhl.top

[R05] 参数默认值
来源：http://ccb.chenjidiqi.icu

name="${1:-default}"
来源：http://jxc.daria6918.cn

[R06] 判断命令是否存在
来源：http://ohz.aibaodan.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vga.gogol.net.cn

[R07] if 判断文件
来源：http://zbw.shanyushiyangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aqd.aibaodan.cn

[R08] 数值比较
来源：http://kxg.xylfe.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ogu.nanxinkj.top

[R09] 字符串比较
来源：http://itn.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vrg.yongpay.top

[R10] 正则匹配
来源：http://qtu.guowangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sdy.epnwcf.com

[R11] case 多分支
来源：http://jpd.tian-w.cn

case "$1" in
来源：http://fwr.kuanghao11.cn

start) echo "启动" ;;
来源：http://hiu.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://bum.zhaomingkeji.xyz

*)     echo "未知命令" ;;
来源：http://piv.nwbrower.top


<!-- 参考信息 -->