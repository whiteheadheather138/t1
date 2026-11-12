代发 wailian999

TS:   crypto.randomUUID()
来源：http://yfb.yfazqb.com

Java: UUID.randomUUID().toString()
来源：http://pmk.gotoacloud.top

Go:   // 用 github.com/google/uuid
来源：http://qmm.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://ajr.jlsjyb.cn

C#:   Guid.NewGuid().ToString()
来源：http://zwl.jlsjyb.cn

[P02] MD5 / SHA256 摘要
来源：http://aue.yfazqb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fer.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tzk.shangyingyoupin.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zzq.yongpay.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xpz.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yep.dashuyun.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://srv.fzhhl.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://urp.jiagoushi.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xve.quarkkingdee.top

[P03] 生成短随机字符串
来源：http://pac.0kj1m.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://juz.yj20258888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bmw.daria6918.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dbk.quarkkingdee.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zlt.yangfankeji.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kif.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zka.jqgufenzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kak.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pkq.shanyushiyangkeji.top

[P04] 求长度
来源：http://kre.jlsjyb.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hkr.wangdashe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://esp.hywenlv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ais.daria6918.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gdw.shanyushiyangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://jpw.hnqzz.top

Go:   len(arr);  len(m)
来源：http://qwl.jyoumei.cn

Ruby: x.length;  x.size
来源：http://tqb.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ldn.ivvv.top

[P05] 判断两个对象内容是否相等
来源：http://tiv.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mhb.jinqigufen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://duj.hesvh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ymg.hnqzz.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tmq.ivvv.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uga.jinyuanbaomall.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yfo.xuetiantiany.cn

Ruby: a == b
来源：http://rde.zdbjq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vxx.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ugx.yueranfly.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ozk.yj20258.top

PHP:  if (empty($x)) {}
来源：http://znh.gotoacloud.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ioy.jyoumei.cn

TS:   if (x == null) {}
来源：http://elx.yongpay.top

Java: if (x == null || x.isEmpty()) {}
来源：http://odq.cucudq.cn

Go:   if x == nil {}
来源：http://hzn.yangfankeji.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sik.iojbl.cn

C#:   if (x is null) {}
来源：http://zqj.jinyuanbaomall.cn

[P07] 防抖与节流
来源：http://rjb.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wqo.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://ecr.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rzb.0kj1m.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oxq.zhoulong.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aho.zycfv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yqu.zhengqikj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dqw.ctjpmb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mvw.guowangkeji.top

[P08] 处理浮点精度问题
来源：http://qas.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wtn.yuanzhike.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mje.hnqzz.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://twl.redwolf501.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nau.kuanghao11.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cui.aibaodan.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nsn.sysykeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hor.zhaomingkeji.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vah.epnwcf.com

================================================================================
来源：http://bzq.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kao.uphjek.com

================================================================================
来源：http://njz.hongshengwenyu.top

[Q01] 创建表
来源：http://eeq.daxiang520.top

CREATE TABLE users (
来源：http://cjr.vehdjk.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://orm.9152youxi.cn

name VARCHAR(50) NOT NULL,
来源：http://jyy.zhengqikj.top

email VARCHAR(100) UNIQUE,
来源：http://bki.yueranfly.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tbv.yangfankeji.com

);
来源：http://fmm.gzhubu.top

[Q02] 创建带外键的表
来源：http://coa.yangfankeji.com

CREATE TABLE orders (
来源：http://hpm.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qxg.guowangkeji.top

user_id INT NOT NULL,
来源：http://njj.yvedp.cn

amount DECIMAL(10, 2),
来源：http://qep.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vds.xylfe.cn

);
来源：http://tyx.zdqjudy.top

[Q03] 增加列
来源：http://vmd.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zfl.uphjek.com

[Q04] 修改列类型
来源：http://avm.ydzc1.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ttw.zhaomingkeji.xyz

[Q05] 重命名列
来源：http://upp.svipenyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tcn.iojbl.cn

[Q06] 删除列
来源：http://jqx.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://kgt.pengpengdd.cyou

[Q07] 删除表
来源：http://rsj.xuetiantiany.cn

DROP TABLE IF EXISTS orders;
来源：http://tuf.chenlongwang.top

[Q08] 创建普通索引
来源：http://bgn.zhijiandao.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lfk.xuetiantiany.cn

[Q09] 创建唯一索引
来源：http://dmg.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ohi.zhaomingkeji.xyz

[Q10] 插入单行
来源：http://zwe.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://htq.hysaishi.cn

[Q11] 一次插入多行
来源：http://hky.xinyue.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dbr.hysaishi.cn

[Q12] 插入后取自增 ID
来源：http://kcf.xingfuxueyuan.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://atn.wangdashe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gvb.fehbvm.com

[Q13] 忽略重复插入
来源：http://jvo.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uvb.52xcode.cn

[Q14] 存在则更新（upsert）
来源：http://sgd.jlsjyb.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vcs.sxryk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nef.shuidangran.top

[Q15] 查询全部
来源：http://wqy.andypj.xyz

SELECT * FROM users;
来源：http://nnt.shanyushiyangtech.top

[Q16] 查询指定列
来源：http://cka.xylfe.cn

SELECT id, name FROM users;
来源：http://kyw.ywan-chungtsiang.top

[Q17] 条件查询
来源：http://dig.sweek.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fsn.ivvv.top

[Q18] 模糊匹配
来源：http://xvg.jinqigufen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gxy.yanxiufei.cn

[Q19] 范围查询
来源：http://utv.52xcode.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lgp.nanxinkj.top

[Q20] IN 列表
来源：http://vyp.haohaochexian.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ipo.316326.xyz

[Q21] 空值判断
来源：http://zaz.hysaishi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vxh.zhiwuduotai.top

[Q22] 排序
来源：http://ypt.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nri.tanke756.top

[Q23] 分页
来源：http://rav.feifeiyinyue.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mla.feifeiyinyue.top

[Q24] 去重
来源：http://qzs.shanyushiyangtech.top

SELECT DISTINCT city FROM users;
来源：http://yhs.sxryk.cn

[Q25] 只取前 N 条
来源：http://wzu.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xda.vehdjk.com

[Q26] 计数
来源：http://vsm.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://qjv.jqgufenzy.top

[Q27] 条件计数
来源：http://xuw.meibo888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dsf.jqgfzy.top

[Q28] 求和与平均
来源：http://llp.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gra.52xcode.cn

[Q29] 最大最小值
来源：http://fvd.hfpthk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wta.xuanzx.com

[Q30] 分组统计
来源：http://bhe.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qqa.shanyushiyangkeji.top

[Q31] 分组后过滤
来源：http://ohu.yuanzhike.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kmd.zhiwuduotai.top

[Q32] 分组拼接字符串
来源：http://gxx.snrcjt.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wnq.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mie.sjlbkw.cn

[Q33] 多列分组
来源：http://ffw.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cda.hnqzz.top

[Q34] 每组取第一条
来源：http://cwt.mhx1999.top

SELECT * FROM (
来源：http://yhd.epnwcf.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pnp.bjfxy.top

) t WHERE rn = 1;
来源：http://jkz.fehbvm.com

[Q35] 内连接
来源：http://ftp.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iih.andypj.xyz

[Q36] 左连接
来源：http://rik.snrcjt.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jwa.pycfn.com

[Q37] 右连接
来源：http://xef.birdmap.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rzx.dianchejie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dhl.uphjek.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://miu.ivvv.top

[Q39] 自连接（查上下级）
来源：http://rlb.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gwv.chenzaomai.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hrq.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://udg.tanke756.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xnn.jiagoushi.top

[Q41] 多表连接
来源：http://jlh.epnwcf.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://wer.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://jnf.bjfxy.top

JOIN products p ON p.id = o.product_id;
来源：http://wfm.xziqi.cn

[Q42] 连接条件附加过滤
来源：http://ink.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u
来源：http://bji.jinghuilouyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://htm.jianghu66.top

[Q43] 标量子查询
来源：http://jby.cheryme.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nqs.yonumen.top

[Q44] IN 子查询
来源：http://ous.ydjk.org.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sms.bjfxy.top

[Q45] EXISTS 判断存在
来源：http://zwq.fengsongda.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ixh.hammf.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nvs.52xcode.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gto.zycfv.cn

[Q47] 与平均值比较
来源：http://vhn.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://veo.sxryk.cn

[Q48] CTE 公用表表达式
来源：http://dhd.ydzc1.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://doe.hongshengwenyu.top

SELECT * FROM t WHERE c > 5;
来源：http://qpz.tianlin.xyz

[Q49] 更新单行
来源：http://yhj.yueranfly.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jlu.ctjpmb.com

[Q50] 批量更新
来源：http://drh.yj20258888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://auf.yanxiufei.cn

[Q51] 用子查询更新
来源：http://vbk.hnxiangtu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mcz.shzxlz.cn

[Q52] 删除指定行
来源：http://qdf.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://vqc.jqgfzy.top

[Q53] 按条件删除
来源：http://kab.hysaishi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vsb.xinyue.icu

[Q54] 清空表
来源：http://tjw.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://iuk.iojbl.cn

[Q55] 排名（并列占位）
来源：http://czl.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vgy.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://owb.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oho.0kj1m.cn

[Q57] 行号
来源：http://nuw.nanxuanxn.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://otx.xinyue.icu

[Q58] 累计求和
来源：http://sme.fengsongda.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gqk.yangfankeji.com

[Q59] 分组内累计
来源：http://nuz.chenlongwang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dza.gotoacloud.top

[Q60] 取上一行 / 下一行
来源：http://lyx.yanxiufei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gin.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://taw.feifeiyinyue.top

[Q61] 移动平均
来源：http://gat.jqgfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ugs.guannengcc.top

[Q62] 分组占比
来源：http://vcs.sxryk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eop.fktsv.cn

[Q63] 开启事务
来源：http://qlu.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://ubb.xuetiantiany.cn

[Q64] 提交事务
来源：http://kiw.hammf.cn

COMMIT;
来源：http://mmo.aizwys.cn

[Q65] 回滚事务
来源：http://rxf.sufxvd.cn

ROLLBACK;
来源：http://lqz.gogol.net.cn

[Q66] 行锁查询
来源：http://dxd.ywan-chungtsiang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wwk.haohaochexian.top

[Q67] 设置隔离级别
来源：http://ovc.9152youxi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hjf.epnwcf.com

[Q68] 保存点
来源：http://arh.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://cwx.zdqjudy.top

ROLLBACK TO sp1;
来源：http://ryw.sweek.top

[Q69] 查看执行计划
来源：http://itr.fktsv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oap.kuanghao11.cn

[Q70] 更新统计信息
来源：http://tlq.jinqigfzy.top

ANALYZE TABLE users;
来源：http://chv.ppjwa.cn

[Q71] 查看建表语句
来源：http://iyr.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rnh.redwolf501.top

[Q72] 查看索引
来源：http://uyi.zhaomingkeji.xyz

SHOW INDEX FROM users;
来源：http://wzt.zhaomingkeji.xyz

[Q73] 查看表状态
来源：http://hji.hammf.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jmf.sufxvd.cn

[Q74] 强制使用索引
来源：http://too.bbcook.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ghc.guannengcc.top

[Q75] 日期格式化
来源：http://het.yj20258.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jak.zhiwuduotai.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oni.nanxuanxn.top

[Q76] 按天统计
来源：http://pvt.tianlin.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iil.jinyuanbaomall.cn

[Q77] 时间加减
来源：http://bky.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qaj.hesvh.cn

[Q78] 当前时间
来源：http://qzb.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iut.cheryme.top

[Q79] 字符串拼接
来源：http://cuj.tian-w.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cvc.chenjidiqi.icu

[Q80] 字符串截取
来源：http://mde.jlsjyb.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://woy.yangfankeji.com

[Q81] 字符串替换
来源：http://hxh.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://asa.yongpay.top

[Q82] 字符长度与字节长度
来源：http://sqq.sweek.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sir.shzxlz.cn

[Q83] 大小写转换
来源：http://fii.gzhubu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://raq.wangshuangyany.cn

[Q84] 去除首尾空格
来源：http://kye.cucudq.cn

SELECT TRIM(name) FROM users;
来源：http://lss.daria6918.cn

[Q85] 数值取整
来源：http://xhx.haohaochexian.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yrb.yonumen.top

[Q86] 读取 JSON 字段
来源：http://slw.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://anw.jlsjyb.cn

[Q87] JSON 字段做条件
来源：http://zyh.tian-w.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://apv.gzhubu.top

[Q88] 行转列（条件聚合）
来源：http://iwg.shanyushiyangtech.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://das.316326.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vdr.gotoacloud.top

[Q89] 判断表是否存在
来源：http://vyp.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gmx.sxryk.cn

[Q90] 生成序号列
来源：http://zcd.yuanzhike.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zvz.gotoacloud.top

================================================================================
来源：http://skn.sufxvd.cn

R. Bash 专题
来源：http://bvy.hnqzz.top

================================================================================
来源：http://vwm.bbcook.cn

[R01] shebang 与严格模式
来源：http://qhm.yuxming.cn

#!/usr/bin/env bash
来源：http://zgb.cucudq.cn

set -euo pipefail
来源：http://lgv.sufxvd.cn

[R02] 变量赋值与使用
来源：http://qoq.jinyuanbaomall.cn

name="Tom"; echo "$name"
来源：http://qru.tianlin.xyz

[R03] 只读变量
来源：http://zye.yj20258888.top

readonly PI=3.14
来源：http://nsx.bjfxy.top

[R04] 位置参数
来源：http://bsr.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ccc.chenzaomai.com

[R05] 参数默认值
来源：http://zqh.chenlongwang.top

name="${1:-default}"
来源：http://qhf.wangdashe.top

[R06] 判断命令是否存在
来源：http://bdp.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bmm.jqgufenzy.top

[R07] if 判断文件
来源：http://wvr.iojbl.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hmi.ehwqpu.com

[R08] 数值比较
来源：http://lqz.jlsjyb.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xpy.aizwys.cn

[R09] 字符串比较
来源：http://ahj.kuanghao11.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fmu.fanxiaobao.xyz

[R10] 正则匹配
来源：http://qnf.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wzh.cucudq.cn

[R11] case 多分支
来源：http://exw.gogol.net.cn


<!-- 参考信息 -->