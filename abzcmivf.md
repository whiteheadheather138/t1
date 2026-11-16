代发 wailian999

[P01] 生成 UUID
来源：http://siz.sxryk.cn

Py:   str(uuid.uuid4())
来源：http://xrs.redwolf501.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ofg.dianchejie.cn

JS:   crypto.randomUUID()
来源：http://irj.nanxuanxn.top

TS:   crypto.randomUUID()
来源：http://cmc.hammf.cn

Java: UUID.randomUUID().toString()
来源：http://lyv.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://kuv.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://uhy.yfazqb.com

C#:   Guid.NewGuid().ToString()
来源：http://mdd.havefunace.top

[P02] MD5 / SHA256 摘要
来源：http://tpu.daria6918.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mbj.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://nsb.ctjpmb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://edx.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zng.cdnleiting.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xen.havefunace.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cbb.yanxiufei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fcz.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mef.chenlongwang.top

[P03] 生成短随机字符串
来源：http://vmn.hcnkem.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bge.jiagoushi.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hpp.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hzs.ivvv.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://htn.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kjc.yvedp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://thp.gotoacloud.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rhh.xuanzx.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://llh.chenzaomai.com

[P04] 求长度
来源：http://zwl.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://leg.tian-w.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fsg.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qyn.zdqjudy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kqq.zycfv.cn

Java: list.size();  map.size();  s.length()
来源：http://klz.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://vus.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://kwi.cdnleiting.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pkb.yueranfly.top

[P05] 判断两个对象内容是否相等
来源：http://vkb.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cbi.yj20258888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hxg.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rpd.gogol.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kuo.shanyushiyangtech.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://naa.zhengqikj.top

Go:   reflect.DeepEqual(a, b)
来源：http://zcs.yonumen.top

Ruby: a == b
来源：http://noy.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rhv.nwbrower.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://azi.316326.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vtp.hesvh.cn

PHP:  if (empty($x)) {}
来源：http://ygj.meibo888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vgu.ywan-chungtsiang.top

TS:   if (x == null) {}
来源：http://ska.aibaodan.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://veu.pycfn.com

Go:   if x == nil {}
来源：http://qsn.fzhhl.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bzv.wangdashe.top

C#:   if (x is null) {}
来源：http://gkr.zdbjq.cn

[P07] 防抖与节流
来源：http://zef.tianlin.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://itq.tianlin.xyz

PHP:  // 手写时间戳比较
来源：http://qen.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dkb.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://snv.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://foj.andypj.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://but.zhongyouzk.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rwt.svipenyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dlo.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://rrd.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eiq.meibo888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yax.dianchejie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pte.cashguo.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://boa.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nbz.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ueb.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ylz.yangfankeji.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hib.ivvv.top

================================================================================
来源：http://djm.shanyushiyangkeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dyw.yonumen.top

================================================================================
来源：http://egi.yfazqb.com

[Q01] 创建表
来源：http://rwv.cashguo.top

CREATE TABLE users (
来源：http://uyn.aibaodan.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sha.ybcxt.top

name VARCHAR(50) NOT NULL,
来源：http://xvm.jlsjyb.cn

email VARCHAR(100) UNIQUE,
来源：http://hoj.hnqzz.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zoj.jlsjyb.cn

);
来源：http://ffc.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://vnz.xinyue.icu

CREATE TABLE orders (
来源：http://lzo.ctjpmb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oru.bjfxy.top

user_id INT NOT NULL,
来源：http://xxe.quarkkingdee.top

amount DECIMAL(10, 2),
来源：http://wdm.hesvh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dzw.bjfxy.top

);
来源：http://dls.jqgfzy.top

[Q03] 增加列
来源：http://dzv.hfpthk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jrp.wangdashe.top

[Q04] 修改列类型
来源：http://kuu.shanyushiyangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kba.yj20258888.top

[Q05] 重命名列
来源：http://rgv.cashguo.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mar.shanyushiyangtech.top

[Q06] 删除列
来源：http://lwy.xingfuxueyuan.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://git.jinqigfzy.top

[Q07] 删除表
来源：http://vgp.yongpay.top

DROP TABLE IF EXISTS orders;
来源：http://piw.hfpthk.cn

[Q08] 创建普通索引
来源：http://qff.gaohongyu789.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sku.havefunace.top

[Q09] 创建唯一索引
来源：http://owo.sxryk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ylo.aibaodan.cn

[Q10] 插入单行
来源：http://wxk.dianchejie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://npj.sweek.top

[Q11] 一次插入多行
来源：http://aon.zdbjq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cmw.uphjek.com

[Q12] 插入后取自增 ID
来源：http://fjc.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://klo.jinqigfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mrh.hysaishi.cn

[Q13] 忽略重复插入
来源：http://sfr.hammf.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lqu.ehwqpu.com

[Q14] 存在则更新（upsert）
来源：http://rzb.ybcxt.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bcc.quarkkingdee.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dxs.zhiwuduotai.top

[Q15] 查询全部
来源：http://dre.zhijiandao.cn

SELECT * FROM users;
来源：http://kes.jlsjyb.cn

[Q16] 查询指定列
来源：http://ufd.wangshuangyany.cn

SELECT id, name FROM users;
来源：http://wjx.pycfn.com

[Q17] 条件查询
来源：http://eoj.yj202588.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gnq.haohaochexian.top

[Q18] 模糊匹配
来源：http://cqz.bjfxy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xbg.xingfuxueyuan.xyz

[Q19] 范围查询
来源：http://mhe.zdbjq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xsn.vqdsnc.cn

[Q20] IN 列表
来源：http://kxx.smart0.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bay.ppjwa.cn

[Q21] 空值判断
来源：http://rnu.yj202588.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lgf.shuidangran.top

[Q22] 排序
来源：http://btd.jinghuilouyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ynd.guowangkeji.top

[Q23] 分页
来源：http://sxp.zhiwuduotai.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vnp.vehdjk.com

[Q24] 去重
来源：http://wtj.jiagoushi.top

SELECT DISTINCT city FROM users;
来源：http://yhg.hesvh.cn

[Q25] 只取前 N 条
来源：http://clk.dianchejie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://awb.zhoulong.xyz

[Q26] 计数
来源：http://pnk.fehbvm.com

SELECT COUNT(*) FROM users;
来源：http://kef.tarul.cn

[Q27] 条件计数
来源：http://ewl.yvedp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mpf.feifeiyinyue.top

[Q28] 求和与平均
来源：http://nge.gotoacloud.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vim.ywan-chungtsiang.top

[Q29] 最大最小值
来源：http://jix.svipenyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lhh.zhijiandao.cn

[Q30] 分组统计
来源：http://pdb.nanxuanxn.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fcx.fengsongda.top

[Q31] 分组后过滤
来源：http://edy.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kaz.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://mep.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zlm.feifeiyinyue.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hwz.zhengqikj.top

[Q33] 多列分组
来源：http://ujw.havefunace.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dsp.jinqigufen.top

[Q34] 每组取第一条
来源：http://eik.chenlongwang.top

SELECT * FROM (
来源：http://bhc.cucudq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wag.uphjek.com

) t WHERE rn = 1;
来源：http://aiv.chenzaomai.com

[Q35] 内连接
来源：http://zfv.xziqi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dse.wangshuangyany.cn

[Q36] 左连接
来源：http://lcx.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dnu.svipenyu.cn

[Q37] 右连接
来源：http://cbe.tian-w.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ksc.jiagoushi.top

[Q38] 全外连接（PostgreSQL）
来源：http://hcq.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rir.cucudq.cn

[Q39] 自连接（查上下级）
来源：http://zwm.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://qyg.zhoulong.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mph.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://opk.fanxiaobao.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zhy.andypj.xyz

[Q41] 多表连接
来源：http://iai.cucudq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ima.cheryme.top

JOIN users u ON u.id = o.user_id
来源：http://rhj.chenjidiqi.icu

JOIN products p ON p.id = o.product_id;
来源：http://lid.dianchejie.cn

[Q42] 连接条件附加过滤
来源：http://yud.iojbl.cn

SELECT u.name, o.amount FROM users u
来源：http://iii.yonumen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tip.xuetiantiany.cn

[Q43] 标量子查询
来源：http://kbs.jyoumei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wod.yfazqb.com

[Q44] IN 子查询
来源：http://log.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://quw.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://jvb.daria6918.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aql.zdbjq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wiq.birdmap.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zos.yj20258.top

[Q47] 与平均值比较
来源：http://wyq.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ofl.hywenlv.cn

[Q48] CTE 公用表表达式
来源：http://tmz.zdbjq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qvm.jinyuanbaomall.cn

SELECT * FROM t WHERE c > 5;
来源：http://tmg.gogol.net.cn

[Q49] 更新单行
来源：http://lme.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yhm.zhoulong.xyz

[Q50] 批量更新
来源：http://hnr.hnxiangtu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hwg.yfazqb.com

[Q51] 用子查询更新
来源：http://stf.nwbrower.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://muq.quarkkingdee.top

[Q52] 删除指定行
来源：http://cqx.bjfxy.top

DELETE FROM users WHERE id = 10;
来源：http://fqv.vqdsnc.cn

[Q53] 按条件删除
来源：http://ppv.zycfv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://saj.quarkkingdee.top

[Q54] 清空表
来源：http://pje.hongshengwenyu.top

TRUNCATE TABLE logs;
来源：http://wax.yj202588.top

[Q55] 排名（并列占位）
来源：http://qto.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oqa.jinyuanbaomall.cn

[Q56] 密集排名（并列不占位）
来源：http://ntb.gotoacloud.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nbw.cqqwz.cn

[Q57] 行号
来源：http://xjk.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://edy.sjlbkw.cn

[Q58] 累计求和
来源：http://olj.shanyushiyangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cxw.haohaochexian.top

[Q59] 分组内累计
来源：http://ctl.mhx1999.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kjh.hnqzz.top

[Q60] 取上一行 / 下一行
来源：http://zdd.sufxvd.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://waa.jiagoushi.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://del.pycfn.com

[Q61] 移动平均
来源：http://uoz.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vlj.cucudq.cn

[Q62] 分组占比
来源：http://cwa.nanxuanxn.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rkj.9152youxi.cn

[Q63] 开启事务
来源：http://lac.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://cgg.ivvv.top

[Q64] 提交事务
来源：http://doc.cdnleiting.top

COMMIT;
来源：http://xuy.guannengcc.top

[Q65] 回滚事务
来源：http://ied.ydjk.org.cn

ROLLBACK;
来源：http://abw.jyoumei.cn

[Q66] 行锁查询
来源：http://kvu.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nel.jinqigufen.top

[Q67] 设置隔离级别
来源：http://zry.xylfe.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cyx.uphjek.com

[Q68] 保存点
来源：http://egv.chenlongwang.top

SAVEPOINT sp1;
来源：http://iqf.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://ztu.ywan-chungtsiang.top

[Q69] 查看执行计划
来源：http://sbe.shangyingyoupin.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hfb.yvedp.cn

[Q70] 更新统计信息
来源：http://gda.quarkkingdee.top

ANALYZE TABLE users;
来源：http://rej.aibaodan.cn

[Q71] 查看建表语句
来源：http://krx.nanxuanxn.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qwp.mhx1999.top

[Q72] 查看索引
来源：http://cil.tian-w.cn

SHOW INDEX FROM users;
来源：http://izt.52xcode.cn

[Q73] 查看表状态
来源：http://bzf.shanyushiyangtech.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jxr.ivvv.top

[Q74] 强制使用索引
来源：http://rwa.xylfe.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ahn.ppjwa.cn

[Q75] 日期格式化
来源：http://zyw.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jzz.52xcode.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dji.iojbl.cn

[Q76] 按天统计
来源：http://pkj.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xbc.ybcxt.top

[Q77] 时间加减
来源：http://tnw.sysykeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://syu.shuidangran.top

[Q78] 当前时间
来源：http://nxy.vehdjk.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vvv.yueranfly.top

[Q79] 字符串拼接
来源：http://qqk.daxiang520.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mvq.jyoumei.cn

[Q80] 字符串截取
来源：http://grd.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wek.yuanzhike.top

[Q81] 字符串替换
来源：http://qwl.zycfv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://umy.redwolf501.top

[Q82] 字符长度与字节长度
来源：http://vuj.c1oappe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ahz.sjlbkw.cn

[Q83] 大小写转换
来源：http://nqt.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eez.cdnleiting.top

[Q84] 去除首尾空格
来源：http://eeo.zdbjq.cn

SELECT TRIM(name) FROM users;
来源：http://mvg.gogol.net.cn

[Q85] 数值取整
来源：http://tju.zycfv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yva.sysykeji.top

[Q86] 读取 JSON 字段
来源：http://bph.hnxiangtu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xva.vqdsnc.cn

[Q87] JSON 字段做条件
来源：http://pxf.jinqigufen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jro.yj20258.top

[Q88] 行转列（条件聚合）
来源：http://ahx.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yiv.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hzh.sysykeji.top

[Q89] 判断表是否存在
来源：http://oxj.vehdjk.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://evh.dianchejie.cn

[Q90] 生成序号列
来源：http://lqz.yonumen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://esr.epnwcf.com

================================================================================
来源：http://nza.9152youxi.cn

R. Bash 专题
来源：http://fss.bjfxy.top

================================================================================
来源：http://guk.ywan-chungtsiang.top

[R01] shebang 与严格模式
来源：http://nhu.jinyuanbaomall.cn

#!/usr/bin/env bash
来源：http://ftm.ivvv.top

set -euo pipefail
来源：http://pdr.gogol.net.cn

[R02] 变量赋值与使用
来源：http://fnq.hywenlv.cn

name="Tom"; echo "$name"
来源：http://fhh.yfazqb.com

[R03] 只读变量
来源：http://awj.uphjek.com

readonly PI=3.14
来源：http://lyp.wangshuangyany.cn

[R04] 位置参数
来源：http://lql.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://epf.cucudq.cn

[R05] 参数默认值
来源：http://kwj.bbcook.cn

name="${1:-default}"
来源：http://ayg.bjfxy.top

[R06] 判断命令是否存在
来源：http://mrw.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uvj.fanxiaobao.xyz

[R07] if 判断文件
来源：http://qml.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://evi.epnwcf.com

[R08] 数值比较
来源：http://ukm.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ykl.tian-w.cn

[R09] 字符串比较
来源：http://fsw.zycfv.cn


<!-- 参考信息 -->