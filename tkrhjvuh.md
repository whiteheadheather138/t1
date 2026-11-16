代发 wailian999

C#:   Parallel.For
来源：http://kgd.ydzc1.top

================================================================================
来源：http://xvr.shanyushiyangtech.top

P. 常用工具函数
来源：http://vrw.ybcxt.top

================================================================================
来源：http://wpe.jinghuilouyu.cn

[P01] 生成 UUID
来源：http://den.yonumen.top

Py:   str(uuid.uuid4())
来源：http://mgs.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cov.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://ycu.andypj.xyz

TS:   crypto.randomUUID()
来源：http://ksh.ppjwa.cn

Java: UUID.randomUUID().toString()
来源：http://iny.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://sgc.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://fax.chenlongwang.top

C#:   Guid.NewGuid().ToString()
来源：http://cwg.bbcook.cn

[P02] MD5 / SHA256 摘要
来源：http://xat.shanyushiyangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sre.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://irh.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oxu.nanxuanxn.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uin.hywenlv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uli.shanyushiyangtech.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gbl.jinqigfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vvc.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vha.yueranfly.top

[P03] 生成短随机字符串
来源：http://fkz.xinyue.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ucc.yuxming.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vhh.xziqi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ecn.hcnkem.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pff.52xcode.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gsq.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://axt.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://usy.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jkp.fengsongda.top

[P04] 求长度
来源：http://zct.zhoulong.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://spg.hnxiangtu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ohk.hysaishi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fci.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qrk.tianlin.xyz

Java: list.size();  map.size();  s.length()
来源：http://rvi.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://jln.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://zyk.uphjek.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://apt.xylfe.cn

[P05] 判断两个对象内容是否相等
来源：http://zfx.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://acw.jinqigfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xoh.shanyushiyangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kmj.hongshengwenyu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xlh.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rxf.yvedp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bxx.gaohongyu789.top

Ruby: a == b
来源：http://eyh.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aio.pengpengdd.cyou

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cwx.fanxiaobao.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jnr.xylfe.cn

PHP:  if (empty($x)) {}
来源：http://maq.52xcode.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qpn.gzhubu.top

TS:   if (x == null) {}
来源：http://tmi.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bnu.tarul.cn

Go:   if x == nil {}
来源：http://odl.daxiang520.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ztn.tianlin.xyz

C#:   if (x is null) {}
来源：http://kpj.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://vmb.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xkh.mhx1999.top

PHP:  // 手写时间戳比较
来源：http://hpy.guannengcc.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ftk.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uel.nanxinkj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gtg.redwolf501.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mhv.bbcook.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yqv.jinqigfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jfk.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://dzv.gotoacloud.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://woy.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xss.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iir.yuanzhike.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yyz.jinghuilouyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qff.pycfn.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://elp.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yfe.quarkkingdee.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dho.jqgufenzy.top

================================================================================
来源：http://lty.jinyuanbaomall.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nki.guannengcc.top

================================================================================
来源：http://fce.hywenlv.cn

[Q01] 创建表
来源：http://qqz.kuanghao11.cn

CREATE TABLE users (
来源：http://vcp.andypj.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iod.sweek.top

name VARCHAR(50) NOT NULL,
来源：http://jhc.feifeiyinyue.top

email VARCHAR(100) UNIQUE,
来源：http://ceh.cdnleiting.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://orv.jinqigufen.top

);
来源：http://dno.meibo888.top

[Q02] 创建带外键的表
来源：http://gfc.kuanghao11.cn

CREATE TABLE orders (
来源：http://nfo.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hlt.sysykeji.top

user_id INT NOT NULL,
来源：http://zoy.svipenyu.cn

amount DECIMAL(10, 2),
来源：http://vag.wangshuangyany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bit.vehdjk.com

);
来源：http://cfi.fehbvm.com

[Q03] 增加列
来源：http://nok.yj20258888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eqz.wangshuangyany.cn

[Q04] 修改列类型
来源：http://xzh.xuanzx.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aot.xziqi.cn

[Q05] 重命名列
来源：http://fug.vehdjk.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hby.yanxiufei.cn

[Q06] 删除列
来源：http://dew.mhx1999.top

ALTER TABLE users DROP COLUMN age;
来源：http://git.uphjek.com

[Q07] 删除表
来源：http://qta.aizwys.cn

DROP TABLE IF EXISTS orders;
来源：http://bxh.guannengcc.top

[Q08] 创建普通索引
来源：http://psm.tarul.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yhc.zycfv.cn

[Q09] 创建唯一索引
来源：http://tgd.daria6918.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jte.gaohongyu789.top

[Q10] 插入单行
来源：http://ftv.fengsongda.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://glg.shuidangran.top

[Q11] 一次插入多行
来源：http://ikp.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tzs.zycfv.cn

[Q12] 插入后取自增 ID
来源：http://ezx.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://pzr.zdqjudy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://skk.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://zke.sweek.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yki.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://azs.shzxlz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lou.yonumen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zru.xylfe.cn

[Q15] 查询全部
来源：http://zyx.xziqi.cn

SELECT * FROM users;
来源：http://qso.0kj1m.cn

[Q16] 查询指定列
来源：http://txt.ivvv.top

SELECT id, name FROM users;
来源：http://not.aibaodan.cn

[Q17] 条件查询
来源：http://eqx.cucudq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ngh.haohaochexian.top

[Q18] 模糊匹配
来源：http://zox.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wbq.cheryme.top

[Q19] 范围查询
来源：http://ged.daxiang520.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://unr.vehdjk.com

[Q20] IN 列表
来源：http://gbb.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://arn.aizwys.cn

[Q21] 空值判断
来源：http://iha.yanxiufei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xvp.jinyuanbaomall.cn

[Q22] 排序
来源：http://inz.kuanghao11.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://duv.jlsjyb.cn

[Q23] 分页
来源：http://mcb.bjfxy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pvn.fehbvm.com

[Q24] 去重
来源：http://zte.jinqigfzy.top

SELECT DISTINCT city FROM users;
来源：http://qci.zhixingplan.top

[Q25] 只取前 N 条
来源：http://kak.epnwcf.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zvx.xuetiantiany.cn

[Q26] 计数
来源：http://bdm.quarkkingdee.top

SELECT COUNT(*) FROM users;
来源：http://xha.ydzc1.top

[Q27] 条件计数
来源：http://xsd.meibo888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lxl.yfazqb.com

[Q28] 求和与平均
来源：http://kfg.yanxiufei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vno.shanyushiyangkeji.top

[Q29] 最大最小值
来源：http://esj.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xlk.quarkkingdee.top

[Q30] 分组统计
来源：http://son.gzhubu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zis.zhijiandao.cn

[Q31] 分组后过滤
来源：http://dil.fktsv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dhs.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://rfg.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ezp.haohaochexian.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pye.xingfuxueyuan.xyz

[Q33] 多列分组
来源：http://psv.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ugk.daxiang520.top

[Q34] 每组取第一条
来源：http://lhn.jinqigufen.top

SELECT * FROM (
来源：http://zls.shanyushiyangtech.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sss.zycfv.cn

) t WHERE rn = 1;
来源：http://tyn.pengpengdd.cyou

[Q35] 内连接
来源：http://tyw.dashuyun.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://noo.cheryme.top

[Q36] 左连接
来源：http://yvi.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vxv.shanyushiyangtech.top

[Q37] 右连接
来源：http://xec.sjlbkw.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yvw.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xta.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://afo.fanxiaobao.xyz

[Q39] 自连接（查上下级）
来源：http://mqo.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dmh.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://myq.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zqt.kuanghao11.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qrp.chenzaomai.com

[Q41] 多表连接
来源：http://wrp.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tub.ydzc1.top

JOIN users u ON u.id = o.user_id
来源：http://ngd.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://bxo.dashuyun.cn

[Q42] 连接条件附加过滤
来源：http://kqw.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u
来源：http://wzo.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eeh.vqdsnc.cn

[Q43] 标量子查询
来源：http://nvc.zhijiandao.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cxu.yongpay.top

[Q44] IN 子查询
来源：http://pgz.birdmap.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://viq.zhongyouzk.top

[Q45] EXISTS 判断存在
来源：http://ivg.ppjwa.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ovw.52xcode.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vmk.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ers.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://xsu.zdbjq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ehe.zhengqikj.top

[Q48] CTE 公用表表达式
来源：http://vuq.9152youxi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qvd.hysaishi.cn

SELECT * FROM t WHERE c > 5;
来源：http://rpi.epnwcf.com

[Q49] 更新单行
来源：http://etk.haohaochexian.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xfy.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://ooa.wangshuangyany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pzk.fehbvm.com

[Q51] 用子查询更新
来源：http://ifs.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://amh.shangyingyoupin.top

[Q52] 删除指定行
来源：http://kzv.cucudq.cn

DELETE FROM users WHERE id = 10;
来源：http://lxy.redwolf501.top

[Q53] 按条件删除
来源：http://tqz.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aww.hcnkem.com

[Q54] 清空表
来源：http://swg.xinyue.icu

TRUNCATE TABLE logs;
来源：http://wbg.tian-w.cn

[Q55] 排名（并列占位）
来源：http://gnk.ivvv.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nhw.gogol.net.cn

[Q56] 密集排名（并列不占位）
来源：http://vga.zhengqikj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://skc.meibo888.top

[Q57] 行号
来源：http://qzr.chenjidiqi.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dda.guowangkeji.top

[Q58] 累计求和
来源：http://wrv.jinqigufen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hln.shangyingyoupin.top

[Q59] 分组内累计
来源：http://ilr.ivvv.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lqk.316326.xyz

[Q60] 取上一行 / 下一行
来源：http://dyc.chenjidiqi.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nug.tianlin.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jid.jqgfzy.top

[Q61] 移动平均
来源：http://yfz.chenlongwang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pld.feifeiyinyue.top

[Q62] 分组占比
来源：http://eco.xziqi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ycb.cucudq.cn

[Q63] 开启事务
来源：http://yzr.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://iue.cdnleiting.top

[Q64] 提交事务
来源：http://rrs.xziqi.cn

COMMIT;
来源：http://tgr.hnxiangtu.top

[Q65] 回滚事务
来源：http://oec.shangyingyoupin.top

ROLLBACK;
来源：http://hig.wangdashe.top

[Q66] 行锁查询
来源：http://cdu.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://umj.tanke756.top

[Q67] 设置隔离级别
来源：http://zlt.fzhhl.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bca.smart0.xyz

[Q68] 保存点
来源：http://kro.xuanzx.com

SAVEPOINT sp1;
来源：http://tsp.zdqjudy.top

ROLLBACK TO sp1;
来源：http://mgm.redwolf501.top

[Q69] 查看执行计划
来源：http://bgp.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lqk.hammf.cn

[Q70] 更新统计信息
来源：http://pvf.svipenyu.cn

ANALYZE TABLE users;
来源：http://gfw.jiagoushi.top

[Q71] 查看建表语句
来源：http://fql.nwbrower.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://flj.tanke756.top

[Q72] 查看索引
来源：http://wrj.cqqwz.cn

SHOW INDEX FROM users;
来源：http://jqn.yuanzhike.top

[Q73] 查看表状态
来源：http://tru.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://evo.sweek.top

[Q74] 强制使用索引
来源：http://pej.zhaomingkeji.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://myl.zdbjq.cn

[Q75] 日期格式化
来源：http://zhh.yangfankeji.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zeo.ybcxt.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tqo.vehdjk.com

[Q76] 按天统计
来源：http://jmh.52xcode.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lou.yongpay.top

[Q77] 时间加减
来源：http://dll.tanke756.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vxd.vehdjk.com

[Q78] 当前时间
来源：http://acm.fzhhl.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fbq.birdmap.top

[Q79] 字符串拼接
来源：http://coi.xuanzx.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://goq.jqgfzy.top

[Q80] 字符串截取
来源：http://irq.aibaodan.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://djb.fengsongda.top

[Q81] 字符串替换
来源：http://zii.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ylb.sufxvd.cn

[Q82] 字符长度与字节长度
来源：http://cwi.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oft.fktsv.cn

[Q83] 大小写转换
来源：http://jkf.zhoulong.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lia.jinqigfzy.top

[Q84] 去除首尾空格
来源：http://emh.fehbvm.com

SELECT TRIM(name) FROM users;
来源：http://sbn.fanxiaobao.xyz

[Q85] 数值取整
来源：http://ykn.iojbl.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eim.316326.xyz

[Q86] 读取 JSON 字段
来源：http://czq.9152youxi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gly.bjfxy.top

[Q87] JSON 字段做条件
来源：http://mxr.ctjpmb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kmo.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://stl.yj20258.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mkl.chenjidiqi.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ymy.zhijiandao.cn

[Q89] 判断表是否存在
来源：http://phd.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sjj.haohaochexian.top

[Q90] 生成序号列
来源：http://fvx.hammf.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://abo.daria6918.cn

================================================================================
来源：http://qri.bjfxy.top

R. Bash 专题
来源：http://nrh.gzhubu.top

================================================================================
来源：http://xvx.chenlongwang.top

[R01] shebang 与严格模式
来源：http://olg.yj202588.top

#!/usr/bin/env bash
来源：http://yru.ybcxt.top

set -euo pipefail
来源：http://qvk.yvedp.cn

[R02] 变量赋值与使用
来源：http://zwb.hysaishi.cn

name="Tom"; echo "$name"
来源：http://pqd.pengpengdd.cyou

[R03] 只读变量
来源：http://dud.yangfankeji.com

readonly PI=3.14
来源：http://spq.gaohongyu789.top

[R04] 位置参数
来源：http://uvn.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dfg.hesvh.cn

[R05] 参数默认值
来源：http://mvu.ydjk.org.cn

name="${1:-default}"
来源：http://xeh.pengpengdd.cyou

[R06] 判断命令是否存在
来源：http://atw.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bgu.chenlongwang.top

[R07] if 判断文件
来源：http://glp.meibo888.top


<!-- 参考信息 -->