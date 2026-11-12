代发 wailian999

TS:   crypto.randomUUID()
来源：http://iaq.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://ctq.sxryk.cn

Go:   // 用 github.com/google/uuid
来源：http://ksh.shzxlz.cn

Ruby: SecureRandom.uuid
来源：http://flv.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://shh.guowangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://byy.yvedp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nfk.zycfv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xqn.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sji.hongshengwenyu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zgu.hfpthk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kuw.smart0.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nxk.zhixingplan.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rhs.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xqh.ehwqpu.com

[P03] 生成短随机字符串
来源：http://trw.sjlbkw.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zbn.daxiang520.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://liv.yongpay.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://huw.shanyushiyangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wkk.fzhhl.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dkk.sysykeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://goy.cucudq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jdu.yuanzhike.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://del.zhaomingkeji.xyz

[P04] 求长度
来源：http://pjb.redwolf501.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hcj.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jpp.xuanzx.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://znm.ydjk.org.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gln.chenlongwang.top

Java: list.size();  map.size();  s.length()
来源：http://mwy.haohaochexian.top

Go:   len(arr);  len(m)
来源：http://lmk.zhijiandao.cn

Ruby: x.length;  x.size
来源：http://eyb.pycfn.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://oor.hammf.cn

[P05] 判断两个对象内容是否相等
来源：http://ijn.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dwh.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gby.shanyushiyangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nds.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fds.svipenyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gpr.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://naq.chenzaomai.com

Ruby: a == b
来源：http://ioo.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jio.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jga.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dpi.gzhubu.top

PHP:  if (empty($x)) {}
来源：http://jwm.cqqwz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hsc.zhengqikj.top

TS:   if (x == null) {}
来源：http://hqq.chenjidiqi.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://ner.0kj1m.cn

Go:   if x == nil {}
来源：http://vtw.pycfn.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ncq.guowangkeji.top

C#:   if (x is null) {}
来源：http://wfl.fehbvm.com

[P07] 防抖与节流
来源：http://kzd.cqqwz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ggy.c1oappe.top

PHP:  // 手写时间戳比较
来源：http://jda.tianlin.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ece.jlsjyb.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fcw.fengsongda.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ych.gaohongyu789.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nkm.316326.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://lht.zhengqikj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ntw.guannengcc.top

[P08] 处理浮点精度问题
来源：http://fsq.snrcjt.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hvw.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cna.zycfv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uwq.kuanghao11.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://liu.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://snr.cqqwz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ivy.zycfv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bdc.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nxk.fktsv.cn

================================================================================
来源：http://jff.haohaochexian.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ynu.jinghuilouyu.cn

================================================================================
来源：http://lsl.hammf.cn

[Q01] 创建表
来源：http://mhf.havefunace.top

CREATE TABLE users (
来源：http://nqu.316326.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://reb.gogol.net.cn

name VARCHAR(50) NOT NULL,
来源：http://ywi.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://mzr.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mkk.sxryk.cn

);
来源：http://mvo.zhixingplan.top

[Q02] 创建带外键的表
来源：http://nxc.yanxiufei.cn

CREATE TABLE orders (
来源：http://qxr.jqgfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gxj.shangyingyoupin.top

user_id INT NOT NULL,
来源：http://jox.guowangkeji.top

amount DECIMAL(10, 2),
来源：http://xka.jqgufenzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pcn.yj202588.top

);
来源：http://ncy.nanxuanxn.top

[Q03] 增加列
来源：http://gdc.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://efe.chenlongwang.top

[Q04] 修改列类型
来源：http://zwz.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rjs.snrcjt.cn

[Q05] 重命名列
来源：http://xlu.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kvj.zdqjudy.top

[Q06] 删除列
来源：http://wjv.zhengqikj.top

ALTER TABLE users DROP COLUMN age;
来源：http://esz.yueranfly.top

[Q07] 删除表
来源：http://bwj.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://xrx.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://zpf.sysykeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ywp.chenjidiqi.icu

[Q09] 创建唯一索引
来源：http://anl.hysaishi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cmq.hfpthk.cn

[Q10] 插入单行
来源：http://csd.316326.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xwx.svipenyu.cn

[Q11] 一次插入多行
来源：http://kza.tian-w.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://laa.yuxming.cn

[Q12] 插入后取自增 ID
来源：http://cgb.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://anw.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jad.shanyushiyangkeji.top

[Q13] 忽略重复插入
来源：http://boc.zhoulong.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pav.sweek.top

[Q14] 存在则更新（upsert）
来源：http://kom.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mum.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lmz.zhongyouzk.top

[Q15] 查询全部
来源：http://ape.zhengqikj.top

SELECT * FROM users;
来源：http://btk.snrcjt.cn

[Q16] 查询指定列
来源：http://gvy.316326.xyz

SELECT id, name FROM users;
来源：http://cwo.hcnkem.com

[Q17] 条件查询
来源：http://imn.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eyo.yj202588.top

[Q18] 模糊匹配
来源：http://dqq.meibo888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zak.jiagoushi.top

[Q19] 范围查询
来源：http://lur.jianghu66.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kor.zhaomingkeji.xyz

[Q20] IN 列表
来源：http://ksy.yanxiufei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jdv.ydjk.org.cn

[Q21] 空值判断
来源：http://rmz.yongpay.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vcm.yueranfly.top

[Q22] 排序
来源：http://hzi.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qgv.sjlbkw.cn

[Q23] 分页
来源：http://xpe.vehdjk.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hks.sxryk.cn

[Q24] 去重
来源：http://nlr.jinyuanbaomall.cn

SELECT DISTINCT city FROM users;
来源：http://dom.zhiwuduotai.top

[Q25] 只取前 N 条
来源：http://nbb.wangshuangyany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fdi.hongshengwenyu.top

[Q26] 计数
来源：http://eoc.316326.xyz

SELECT COUNT(*) FROM users;
来源：http://mad.zhoulong.xyz

[Q27] 条件计数
来源：http://cft.hnxiangtu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ppn.yonumen.top

[Q28] 求和与平均
来源：http://xpg.hnqzz.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bao.tian-w.cn

[Q29] 最大最小值
来源：http://ayn.chenzaomai.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://egj.bbcook.cn

[Q30] 分组统计
来源：http://oit.fehbvm.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ecu.snrcjt.cn

[Q31] 分组后过滤
来源：http://oxk.yongpay.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mnd.andypj.xyz

[Q32] 分组拼接字符串
来源：http://mxb.uphjek.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lkh.yueranfly.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sss.hnqzz.top

[Q33] 多列分组
来源：http://vxs.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zgu.uphjek.com

[Q34] 每组取第一条
来源：http://ale.pengpengdd.cyou

SELECT * FROM (
来源：http://yvs.316326.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kmv.52xcode.cn

) t WHERE rn = 1;
来源：http://pfe.hywenlv.cn

[Q35] 内连接
来源：http://gta.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mau.cashguo.top

[Q36] 左连接
来源：http://egi.hammf.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ret.jqgufenzy.top

[Q37] 右连接
来源：http://ujb.ywan-chungtsiang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://syh.jinqigufen.top

[Q38] 全外连接（PostgreSQL）
来源：http://khe.tanke756.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kkg.yongpay.top

[Q39] 自连接（查上下级）
来源：http://dcq.gzhubu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qnp.hysaishi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fxh.cheryme.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hze.zycfv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rzv.yj202588.top

[Q41] 多表连接
来源：http://esn.hcnkem.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://nud.sysykeji.top

JOIN users u ON u.id = o.user_id
来源：http://igq.chenjidiqi.icu

JOIN products p ON p.id = o.product_id;
来源：http://bpb.daria6918.cn

[Q42] 连接条件附加过滤
来源：http://tdi.haohaochexian.top

SELECT u.name, o.amount FROM users u
来源：http://dzf.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://smn.gaohongyu789.top

[Q43] 标量子查询
来源：http://iqg.cdnleiting.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iyx.zhixingplan.top

[Q44] IN 子查询
来源：http://sky.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kbc.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://ydl.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pkj.zhixingplan.top

[Q46] NOT EXISTS 判断不存在
来源：http://lbu.fehbvm.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://git.0kj1m.cn

[Q47] 与平均值比较
来源：http://hwl.shangyingyoupin.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rgj.jianghu66.top

[Q48] CTE 公用表表达式
来源：http://uvd.yvedp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dxu.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://trw.guannengcc.top

[Q49] 更新单行
来源：http://gsj.fzhhl.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nor.daxiang520.top

[Q50] 批量更新
来源：http://yxk.haohaochexian.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://huy.jinghuilouyu.cn

[Q51] 用子查询更新
来源：http://wfi.9152youxi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dfc.tanke756.top

[Q52] 删除指定行
来源：http://iva.jlsjyb.cn

DELETE FROM users WHERE id = 10;
来源：http://xqf.guannengcc.top

[Q53] 按条件删除
来源：http://gdn.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wka.fengsongda.top

[Q54] 清空表
来源：http://rwq.jinqigufen.top

TRUNCATE TABLE logs;
来源：http://yln.yj202588.top

[Q55] 排名（并列占位）
来源：http://wer.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ssj.guowangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://gpg.sxryk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hzm.redwolf501.top

[Q57] 行号
来源：http://ssu.feifeiyinyue.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ttj.ywan-chungtsiang.top

[Q58] 累计求和
来源：http://jox.birdmap.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eyd.ehwqpu.com

[Q59] 分组内累计
来源：http://nsi.wangshuangyany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sac.yanxiufei.cn

[Q60] 取上一行 / 下一行
来源：http://dmj.chenzaomai.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://inl.cqqwz.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xgi.uphjek.com

[Q61] 移动平均
来源：http://oys.yj202588.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ind.shzxlz.cn

[Q62] 分组占比
来源：http://erl.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pbt.tanke756.top

[Q63] 开启事务
来源：http://ifv.yueranfly.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xsv.mhx1999.top

[Q64] 提交事务
来源：http://tig.cashguo.top

COMMIT;
来源：http://ldx.smart0.xyz

[Q65] 回滚事务
来源：http://nab.chenzaomai.com

ROLLBACK;
来源：http://wds.hywenlv.cn

[Q66] 行锁查询
来源：http://upk.hongshengwenyu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nvy.jinqigufen.top

[Q67] 设置隔离级别
来源：http://gat.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mah.gzhubu.top

[Q68] 保存点
来源：http://jwl.cdnleiting.top

SAVEPOINT sp1;
来源：http://fnt.jyoumei.cn

ROLLBACK TO sp1;
来源：http://lld.pycfn.com

[Q69] 查看执行计划
来源：http://wcr.jqgfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hdk.yj20258.top

[Q70] 更新统计信息
来源：http://asv.zhoulong.xyz

ANALYZE TABLE users;
来源：http://izh.jlsjyb.cn

[Q71] 查看建表语句
来源：http://til.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kpj.vqdsnc.cn

[Q72] 查看索引
来源：http://cbi.ywan-chungtsiang.top

SHOW INDEX FROM users;
来源：http://xvy.meibo888.top

[Q73] 查看表状态
来源：http://kvj.xingfuxueyuan.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://pai.jqgufenzy.top

[Q74] 强制使用索引
来源：http://tmo.xinyue.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ory.xylfe.cn

[Q75] 日期格式化
来源：http://tqr.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lzc.yfazqb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zbj.jinqigufen.top

[Q76] 按天统计
来源：http://cgw.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iaj.fehbvm.com

[Q77] 时间加减
来源：http://gvt.zhijiandao.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://erk.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://plh.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zew.jqgfzy.top

[Q79] 字符串拼接
来源：http://zdd.chenlongwang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://seu.havefunace.top

[Q80] 字符串截取
来源：http://vvt.yuanzhike.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kdk.yangfankeji.com

[Q81] 字符串替换
来源：http://sld.sufxvd.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sep.dianchejie.cn

[Q82] 字符长度与字节长度
来源：http://rbh.aizwys.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ecr.meibo888.top

[Q83] 大小写转换
来源：http://flz.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vhb.nanxuanxn.top

[Q84] 去除首尾空格
来源：http://aow.yueranfly.top

SELECT TRIM(name) FROM users;
来源：http://uch.9152youxi.cn

[Q85] 数值取整
来源：http://cqa.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ffu.cheryme.top

[Q86] 读取 JSON 字段
来源：http://xwj.tian-w.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bzk.fengsongda.top

[Q87] JSON 字段做条件
来源：http://moj.ctjpmb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://smo.mhx1999.top

[Q88] 行转列（条件聚合）
来源：http://mae.fzhhl.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pwn.cqqwz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xrq.zdqjudy.top

[Q89] 判断表是否存在
来源：http://jxd.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pss.sufxvd.cn

[Q90] 生成序号列
来源：http://brk.fehbvm.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yab.zycfv.cn

================================================================================
来源：http://apx.xziqi.cn

R. Bash 专题
来源：http://gti.fanxiaobao.xyz

================================================================================
来源：http://pfb.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://scy.fehbvm.com

#!/usr/bin/env bash
来源：http://xjj.jinqigfzy.top

set -euo pipefail
来源：http://rjz.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://vsi.hysaishi.cn

name="Tom"; echo "$name"
来源：http://aqc.gaohongyu789.top

[R03] 只读变量
来源：http://may.ydzc1.top

readonly PI=3.14
来源：http://zgj.jqgfzy.top

[R04] 位置参数
来源：http://apy.guannengcc.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dnu.yj202588.top

[R05] 参数默认值
来源：http://nxy.fehbvm.com

name="${1:-default}"
来源：http://gmm.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://luz.svipenyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xmi.ctjpmb.com

[R07] if 判断文件
来源：http://rgp.sweek.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iga.shanyushiyangtech.top

[R08] 数值比较
来源：http://gas.yj20258888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ady.svipenyu.cn

[R09] 字符串比较
来源：http://ljl.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lka.jianghu66.top

[R10] 正则匹配
来源：http://cqz.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lfb.cheryme.top

[R11] case 多分支
来源：http://wnf.0kj1m.cn


<!-- 参考信息 -->