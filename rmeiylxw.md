代发 wailian999

TS:   crypto.randomUUID()
来源：http://ssv.iojbl.cn

Java: UUID.randomUUID().toString()
来源：http://oxc.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://etd.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://rlq.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://ykg.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://tfg.smart0.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pvb.wangdashe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ndp.meibo888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qch.hysaishi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://afo.xziqi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gcr.jqgfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kmo.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fqz.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://knh.xingfuxueyuan.xyz

[P03] 生成短随机字符串
来源：http://jlt.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uqp.gzhubu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://owb.haohaochexian.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sla.fengsongda.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ajo.yonumen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dzv.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rud.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jry.52xcode.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://abx.hywenlv.cn

[P04] 求长度
来源：http://fdo.hfpthk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qiq.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wqn.epnwcf.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://swu.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jrg.hesvh.cn

Java: list.size();  map.size();  s.length()
来源：http://tzf.chenlongwang.top

Go:   len(arr);  len(m)
来源：http://kyc.fengsongda.top

Ruby: x.length;  x.size
来源：http://buu.nanxuanxn.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://syb.dashuyun.cn

[P05] 判断两个对象内容是否相等
来源：http://geh.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dab.yj20258.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://olr.sysykeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qdj.ivvv.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jkt.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://apf.nwbrower.top

Go:   reflect.DeepEqual(a, b)
来源：http://nyt.sxryk.cn

Ruby: a == b
来源：http://kyn.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kur.fengsongda.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wkt.andypj.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jmr.chenlongwang.top

PHP:  if (empty($x)) {}
来源：http://den.yueranfly.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bvm.xingfuxueyuan.xyz

TS:   if (x == null) {}
来源：http://isx.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zwn.epnwcf.com

Go:   if x == nil {}
来源：http://jog.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dkm.chenlongwang.top

C#:   if (x is null) {}
来源：http://cgj.ehwqpu.com

[P07] 防抖与节流
来源：http://cex.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mcs.tianlin.xyz

PHP:  // 手写时间戳比较
来源：http://mdx.andypj.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jes.ehwqpu.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pzi.zhoulong.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tjh.pengpengdd.cyou

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mfh.cqqwz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://csc.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ndu.sysykeji.top

[P08] 处理浮点精度问题
来源：http://wxk.sufxvd.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://waj.vehdjk.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uqf.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vxt.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://etz.yangfankeji.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rls.jinqigfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nkw.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://czl.gaohongyu789.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://haf.9152youxi.cn

================================================================================
来源：http://mij.daxiang520.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://etz.ppjwa.cn

================================================================================
来源：http://qht.ivvv.top

[Q01] 创建表
来源：http://jep.hnqzz.top

CREATE TABLE users (
来源：http://rvy.dashuyun.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mzd.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://gfp.hnxiangtu.top

email VARCHAR(100) UNIQUE,
来源：http://lkp.shzxlz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ijr.chenlongwang.top

);
来源：http://yqm.aibaodan.cn

[Q02] 创建带外键的表
来源：http://ozs.chenjidiqi.icu

CREATE TABLE orders (
来源：http://jwh.shuidangran.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vjc.wangdashe.top

user_id INT NOT NULL,
来源：http://iyh.zhongyouzk.top

amount DECIMAL(10, 2),
来源：http://udy.gzhubu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://adh.chenzaomai.com

);
来源：http://hxo.uphjek.com

[Q03] 增加列
来源：http://uyb.dashuyun.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jnx.yangfankeji.com

[Q04] 修改列类型
来源：http://crg.daria6918.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qen.zhoulong.xyz

[Q05] 重命名列
来源：http://lgn.jiagoushi.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jvc.sufxvd.cn

[Q06] 删除列
来源：http://tup.shuidangran.top

ALTER TABLE users DROP COLUMN age;
来源：http://xkz.wangshuangyany.cn

[Q07] 删除表
来源：http://qwb.yonumen.top

DROP TABLE IF EXISTS orders;
来源：http://ioe.daxiang520.top

[Q08] 创建普通索引
来源：http://czz.dianchejie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nux.zycfv.cn

[Q09] 创建唯一索引
来源：http://vak.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nlz.hongshengwenyu.top

[Q10] 插入单行
来源：http://kol.zhixingplan.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://anp.yonumen.top

[Q11] 一次插入多行
来源：http://xjb.ivvv.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://olo.shuidangran.top

[Q12] 插入后取自增 ID
来源：http://vqq.feifeiyinyue.top

INSERT INTO users (name) VALUES ('C');
来源：http://vjz.jinqigufen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://chr.9152youxi.cn

[Q13] 忽略重复插入
来源：http://cby.epnwcf.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sir.smart0.xyz

[Q14] 存在则更新（upsert）
来源：http://sxq.hfpthk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rds.9152youxi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zuq.yanxiufei.cn

[Q15] 查询全部
来源：http://qmc.epnwcf.com

SELECT * FROM users;
来源：http://ezd.shzxlz.cn

[Q16] 查询指定列
来源：http://cvv.zhiwuduotai.top

SELECT id, name FROM users;
来源：http://nzb.fzhhl.top

[Q17] 条件查询
来源：http://wgg.zhengqikj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kps.hesvh.cn

[Q18] 模糊匹配
来源：http://rax.yangfankeji.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pkq.guowangkeji.top

[Q19] 范围查询
来源：http://fct.gzhubu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gqd.xylfe.cn

[Q20] IN 列表
来源：http://vbg.hongshengwenyu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sjz.hongshengwenyu.top

[Q21] 空值判断
来源：http://eih.sweek.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bjl.shzxlz.cn

[Q22] 排序
来源：http://qpw.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pgh.yfazqb.com

[Q23] 分页
来源：http://oiv.jinyuanbaomall.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fjf.hnqzz.top

[Q24] 去重
来源：http://fkc.0kj1m.cn

SELECT DISTINCT city FROM users;
来源：http://dbz.ctjpmb.com

[Q25] 只取前 N 条
来源：http://khy.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wcn.zhengqikj.top

[Q26] 计数
来源：http://acx.nanxinkj.top

SELECT COUNT(*) FROM users;
来源：http://fym.zdqjudy.top

[Q27] 条件计数
来源：http://wuq.svipenyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hqf.chenzaomai.com

[Q28] 求和与平均
来源：http://iys.yonumen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blu.ivvv.top

[Q29] 最大最小值
来源：http://rgx.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://ksh.gogol.net.cn

[Q30] 分组统计
来源：http://vsa.xylfe.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://btb.andypj.xyz

[Q31] 分组后过滤
来源：http://joe.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zzb.aizwys.cn

[Q32] 分组拼接字符串
来源：http://rob.cheryme.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sgr.feifeiyinyue.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hkl.guowangkeji.top

[Q33] 多列分组
来源：http://ooj.jiagoushi.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ffg.tian-w.cn

[Q34] 每组取第一条
来源：http://soq.ywan-chungtsiang.top

SELECT * FROM (
来源：http://noq.zycfv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qkq.gogol.net.cn

) t WHERE rn = 1;
来源：http://hzc.yuanzhike.top

[Q35] 内连接
来源：http://inb.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uzl.ehwqpu.com

[Q36] 左连接
来源：http://cgt.zhengqikj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uvn.guannengcc.top

[Q37] 右连接
来源：http://bao.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lip.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vav.ivvv.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wnb.xziqi.cn

[Q39] 自连接（查上下级）
来源：http://ypu.jinqigfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wci.epnwcf.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tge.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mce.hywenlv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fdg.jlsjyb.cn

[Q41] 多表连接
来源：http://lnq.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ctw.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://nra.wangdashe.top

JOIN products p ON p.id = o.product_id;
来源：http://mhx.tarul.cn

[Q42] 连接条件附加过滤
来源：http://hkt.yj202588.top

SELECT u.name, o.amount FROM users u
来源：http://yhy.yongpay.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uxm.bjfxy.top

[Q43] 标量子查询
来源：http://kie.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://usg.aibaodan.cn

[Q44] IN 子查询
来源：http://fan.hfpthk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qxc.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://vvg.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hnf.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://efv.jinqigufen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cge.yuxming.cn

[Q47] 与平均值比较
来源：http://jhe.gotoacloud.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dla.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://omy.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fqf.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://mxb.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://mgg.daxiang520.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pia.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://hbw.jinqigufen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oeu.ctjpmb.com

[Q51] 用子查询更新
来源：http://ruf.yj202588.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://exd.fktsv.cn

[Q52] 删除指定行
来源：http://gha.zhiwuduotai.top

DELETE FROM users WHERE id = 10;
来源：http://ysn.tarul.cn

[Q53] 按条件删除
来源：http://wju.feifeiyinyue.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ais.jiagoushi.top

[Q54] 清空表
来源：http://wdd.zhixingplan.top

TRUNCATE TABLE logs;
来源：http://lrm.jianghu66.top

[Q55] 排名（并列占位）
来源：http://qtl.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://miz.xylfe.cn

[Q56] 密集排名（并列不占位）
来源：http://ftc.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nsr.xinyue.icu

[Q57] 行号
来源：http://gwa.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fja.epnwcf.com

[Q58] 累计求和
来源：http://uwy.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bgt.xuetiantiany.cn

[Q59] 分组内累计
来源：http://eil.iojbl.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://our.yongpay.top

[Q60] 取上一行 / 下一行
来源：http://koo.jinyuanbaomall.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kpf.xinyue.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jvl.kuanghao11.cn

[Q61] 移动平均
来源：http://rgt.jinqigfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pvj.yuanzhike.top

[Q62] 分组占比
来源：http://nat.dianchejie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lig.yj20258888.top

[Q63] 开启事务
来源：http://msu.jianghu66.top

START TRANSACTION;                -- 或 BEGIN
来源：http://lwd.gzhubu.top

[Q64] 提交事务
来源：http://etx.hcnkem.com

COMMIT;
来源：http://vum.zhijiandao.cn

[Q65] 回滚事务
来源：http://gih.gotoacloud.top

ROLLBACK;
来源：http://gbr.sufxvd.cn

[Q66] 行锁查询
来源：http://ulh.xziqi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xiw.shzxlz.cn

[Q67] 设置隔离级别
来源：http://khe.shuidangran.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kzn.wangdashe.top

[Q68] 保存点
来源：http://sck.dashuyun.cn

SAVEPOINT sp1;
来源：http://ehe.shanyushiyangtech.top

ROLLBACK TO sp1;
来源：http://nnz.c1oappe.top

[Q69] 查看执行计划
来源：http://ugp.aibaodan.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cib.shuidangran.top

[Q70] 更新统计信息
来源：http://fai.sweek.top

ANALYZE TABLE users;
来源：http://gst.316326.xyz

[Q71] 查看建表语句
来源：http://xqg.316326.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tdr.cqqwz.cn

[Q72] 查看索引
来源：http://hjw.epnwcf.com

SHOW INDEX FROM users;
来源：http://dtr.aizwys.cn

[Q73] 查看表状态
来源：http://wsv.gogol.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kew.daxiang520.top

[Q74] 强制使用索引
来源：http://ael.aizwys.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://egb.tanke756.top

[Q75] 日期格式化
来源：http://tgj.jinyuanbaomall.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xyo.gogol.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bwe.zhongyouzk.top

[Q76] 按天统计
来源：http://trh.hcnkem.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ixp.jlsjyb.cn

[Q77] 时间加减
来源：http://cgq.snrcjt.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://njg.cashguo.top

[Q78] 当前时间
来源：http://jcg.zhaomingkeji.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zqy.xinyue.icu

[Q79] 字符串拼接
来源：http://ntz.jqgufenzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://voq.fanxiaobao.xyz

[Q80] 字符串截取
来源：http://yky.kuanghao11.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ihk.svipenyu.cn

[Q81] 字符串替换
来源：http://hyj.aizwys.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ghl.havefunace.top

[Q82] 字符长度与字节长度
来源：http://oyp.nwbrower.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oee.chenjidiqi.icu

[Q83] 大小写转换
来源：http://uhp.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hbl.hnqzz.top

[Q84] 去除首尾空格
来源：http://pib.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://whl.yj20258.top

[Q85] 数值取整
来源：http://poc.jyoumei.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://obj.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://mdc.jlsjyb.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iaq.birdmap.top

[Q87] JSON 字段做条件
来源：http://cqw.epnwcf.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sfx.chenjidiqi.icu

[Q88] 行转列（条件聚合）
来源：http://flu.hfpthk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://afa.c1oappe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hom.ivvv.top

[Q89] 判断表是否存在
来源：http://uvy.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nkn.jinyuanbaomall.cn

[Q90] 生成序号列
来源：http://hvo.chenjidiqi.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tvq.hnxiangtu.top

================================================================================
来源：http://wpm.xylfe.cn

R. Bash 专题
来源：http://vrv.jyoumei.cn

================================================================================
来源：http://til.chenzaomai.com

[R01] shebang 与严格模式
来源：http://lqg.shzxlz.cn

#!/usr/bin/env bash
来源：http://txw.hnqzz.top

set -euo pipefail
来源：http://duj.vehdjk.com

[R02] 变量赋值与使用
来源：http://gyo.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://xqz.yj20258888.top

[R03] 只读变量
来源：http://ksq.yonumen.top

readonly PI=3.14
来源：http://nms.yangfankeji.com

[R04] 位置参数
来源：http://aoq.gaohongyu789.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nez.yueranfly.top

[R05] 参数默认值
来源：http://ntr.zhengqikj.top

name="${1:-default}"
来源：http://oql.yj20258.top

[R06] 判断命令是否存在
来源：http://vtm.ydzc1.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eyt.zhixingplan.top

[R07] if 判断文件
来源：http://rpz.aibaodan.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://san.snrcjt.cn

[R08] 数值比较
来源：http://ucc.quarkkingdee.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ekr.snrcjt.cn

[R09] 字符串比较
来源：http://vay.316326.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bjq.yvedp.cn

[R10] 正则匹配
来源：http://yos.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pmb.mhx1999.top

[R11] case 多分支
来源：http://eqp.ydjk.org.cn


<!-- 参考信息 -->