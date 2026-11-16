代发 wailian999

[P01] 生成 UUID
来源：http://gao.ivvv.top

Py:   str(uuid.uuid4())
来源：http://asi.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ggd.sxryk.cn

JS:   crypto.randomUUID()
来源：http://aly.ybcxt.top

TS:   crypto.randomUUID()
来源：http://hoa.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://pns.epnwcf.com

Go:   // 用 github.com/google/uuid
来源：http://quv.hammf.cn

Ruby: SecureRandom.uuid
来源：http://vqf.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://yqj.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://lze.shzxlz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vmu.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ssf.uphjek.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yqh.feifeiyinyue.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zgp.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://krn.zhixingplan.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sod.jinghuilouyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://boz.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ade.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://tou.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yro.chenzaomai.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wjr.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qkm.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ugu.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cvr.zhijiandao.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aob.redwolf501.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mma.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vuj.cashguo.top

[P04] 求长度
来源：http://vyf.shanyushiyangtech.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lqu.xinyue.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zie.jinghuilouyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ydr.316326.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nbk.ydjk.org.cn

Java: list.size();  map.size();  s.length()
来源：http://ugy.redwolf501.top

Go:   len(arr);  len(m)
来源：http://hkf.xingfuxueyuan.xyz

Ruby: x.length;  x.size
来源：http://aet.xziqi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gda.yongpay.top

[P05] 判断两个对象内容是否相等
来源：http://bpj.chenzaomai.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://vvy.haohaochexian.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gfr.havefunace.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wdj.yueranfly.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://afk.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vnj.ehwqpu.com

Go:   reflect.DeepEqual(a, b)
来源：http://ysb.sjlbkw.cn

Ruby: a == b
来源：http://vfr.yfazqb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fny.xingfuxueyuan.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hhu.ppjwa.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eay.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://ndl.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wrt.birdmap.top

TS:   if (x == null) {}
来源：http://xrg.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://twi.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://ldk.nanxinkj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bkd.52xcode.cn

C#:   if (x is null) {}
来源：http://pba.hnxiangtu.top

[P07] 防抖与节流
来源：http://jom.ywan-chungtsiang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qqd.hesvh.cn

PHP:  // 手写时间戳比较
来源：http://bhi.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dwp.cashguo.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cdx.chenlongwang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mou.zhijiandao.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rwx.yj20258888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ycx.smart0.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://roy.xuanzx.com

[P08] 处理浮点精度问题
来源：http://him.vqdsnc.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tie.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://upr.meibo888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ily.feifeiyinyue.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jkv.jqgfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aco.yj202588.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vag.hysaishi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://apx.hywenlv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pcs.kuanghao11.cn

================================================================================
来源：http://xkb.fktsv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ron.daxiang520.top

================================================================================
来源：http://aye.jyoumei.cn

[Q01] 创建表
来源：http://suq.yueranfly.top

CREATE TABLE users (
来源：http://bcu.gzhubu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://juh.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://gwy.ctjpmb.com

email VARCHAR(100) UNIQUE,
来源：http://vgb.pycfn.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dqx.hongshengwenyu.top

);
来源：http://hga.gzhubu.top

[Q02] 创建带外键的表
来源：http://wtx.daria6918.cn

CREATE TABLE orders (
来源：http://mkk.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sse.zhongyouzk.top

user_id INT NOT NULL,
来源：http://vik.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://fcs.chenjidiqi.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hix.zhongyouzk.top

);
来源：http://hmx.wangdashe.top

[Q03] 增加列
来源：http://dgw.bbcook.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jdx.birdmap.top

[Q04] 修改列类型
来源：http://dxz.jinyuanbaomall.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fqv.52xcode.cn

[Q05] 重命名列
来源：http://oal.pengpengdd.cyou

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dqi.52xcode.cn

[Q06] 删除列
来源：http://evm.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://ock.hnxiangtu.top

[Q07] 删除表
来源：http://gbv.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://cnm.bjfxy.top

[Q08] 创建普通索引
来源：http://mes.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://myt.uphjek.com

[Q09] 创建唯一索引
来源：http://ipk.ydzc1.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://imm.vqdsnc.cn

[Q10] 插入单行
来源：http://iyj.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://atb.guannengcc.top

[Q11] 一次插入多行
来源：http://xew.fzhhl.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vbj.0kj1m.cn

[Q12] 插入后取自增 ID
来源：http://xhq.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://dih.yuxming.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wih.cqqwz.cn

[Q13] 忽略重复插入
来源：http://hcq.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ijt.jlsjyb.cn

[Q14] 存在则更新（upsert）
来源：http://csx.zhongyouzk.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://anr.yj20258888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://flv.nwbrower.top

[Q15] 查询全部
来源：http://ueb.yuxming.cn

SELECT * FROM users;
来源：http://kfo.sweek.top

[Q16] 查询指定列
来源：http://vvd.ybcxt.top

SELECT id, name FROM users;
来源：http://ebr.zycfv.cn

[Q17] 条件查询
来源：http://pek.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://igf.shangyingyoupin.top

[Q18] 模糊匹配
来源：http://wcd.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iew.9152youxi.cn

[Q19] 范围查询
来源：http://lan.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kkf.jqgfzy.top

[Q20] IN 列表
来源：http://yig.shzxlz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uyl.jinghuilouyu.cn

[Q21] 空值判断
来源：http://jmh.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gol.birdmap.top

[Q22] 排序
来源：http://vlx.c1oappe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bfm.aibaodan.cn

[Q23] 分页
来源：http://hbc.chenzaomai.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lly.hywenlv.cn

[Q24] 去重
来源：http://kag.zhijiandao.cn

SELECT DISTINCT city FROM users;
来源：http://kde.zdqjudy.top

[Q25] 只取前 N 条
来源：http://osy.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vzs.zhijiandao.cn

[Q26] 计数
来源：http://gqr.yvedp.cn

SELECT COUNT(*) FROM users;
来源：http://ceh.nanxinkj.top

[Q27] 条件计数
来源：http://qfg.meibo888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ctk.aibaodan.cn

[Q28] 求和与平均
来源：http://ump.hammf.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qjz.ywan-chungtsiang.top

[Q29] 最大最小值
来源：http://mha.svipenyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cem.zhengqikj.top

[Q30] 分组统计
来源：http://awk.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xqf.yj202588.top

[Q31] 分组后过滤
来源：http://lyj.yj20258888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://viy.shzxlz.cn

[Q32] 分组拼接字符串
来源：http://yhi.pycfn.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://udj.jiagoushi.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fux.ybcxt.top

[Q33] 多列分组
来源：http://pio.zhongyouzk.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cbr.zdqjudy.top

[Q34] 每组取第一条
来源：http://noy.vqdsnc.cn

SELECT * FROM (
来源：http://rvo.zycfv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yub.jinghuilouyu.cn

) t WHERE rn = 1;
来源：http://kdt.tianlin.xyz

[Q35] 内连接
来源：http://qda.sufxvd.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gyq.sysykeji.top

[Q36] 左连接
来源：http://sqr.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vmu.zycfv.cn

[Q37] 右连接
来源：http://era.fanxiaobao.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qbr.0kj1m.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gbd.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kse.hywenlv.cn

[Q39] 自连接（查上下级）
来源：http://qjk.yonumen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ywy.nwbrower.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://egy.cqqwz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ieg.cheryme.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pcl.guowangkeji.top

[Q41] 多表连接
来源：http://wts.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kcv.0kj1m.cn

JOIN users u ON u.id = o.user_id
来源：http://uim.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://tof.yvedp.cn

[Q42] 连接条件附加过滤
来源：http://who.feifeiyinyue.top

SELECT u.name, o.amount FROM users u
来源：http://cfg.haohaochexian.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eyc.shuidangran.top

[Q43] 标量子查询
来源：http://pmu.tanke756.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ypl.zhijiandao.cn

[Q44] IN 子查询
来源：http://izx.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oql.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://ssz.yuxming.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nhy.hnqzz.top

[Q46] NOT EXISTS 判断不存在
来源：http://ngx.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ypw.guannengcc.top

[Q47] 与平均值比较
来源：http://out.yj20258888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nxp.hnqzz.top

[Q48] CTE 公用表表达式
来源：http://lbq.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ivg.hesvh.cn

SELECT * FROM t WHERE c > 5;
来源：http://ifp.ydzc1.top

[Q49] 更新单行
来源：http://dwj.zhijiandao.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lgp.aibaodan.cn

[Q50] 批量更新
来源：http://rqc.snrcjt.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xbe.xingfuxueyuan.xyz

[Q51] 用子查询更新
来源：http://bgy.yangfankeji.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bkq.guowangkeji.top

[Q52] 删除指定行
来源：http://mvo.guannengcc.top

DELETE FROM users WHERE id = 10;
来源：http://xte.316326.xyz

[Q53] 按条件删除
来源：http://agt.shangyingyoupin.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://duq.havefunace.top

[Q54] 清空表
来源：http://gvi.yfazqb.com

TRUNCATE TABLE logs;
来源：http://jgz.svipenyu.cn

[Q55] 排名（并列占位）
来源：http://tlp.jinghuilouyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pyz.ydjk.org.cn

[Q56] 密集排名（并列不占位）
来源：http://gol.52xcode.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lux.hfpthk.cn

[Q57] 行号
来源：http://vkh.iojbl.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lno.ybcxt.top

[Q58] 累计求和
来源：http://zdi.pengpengdd.cyou

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://twj.wangdashe.top

[Q59] 分组内累计
来源：http://cyi.birdmap.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lad.sxryk.cn

[Q60] 取上一行 / 下一行
来源：http://kvo.feifeiyinyue.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cuw.yj20258.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wuy.dianchejie.cn

[Q61] 移动平均
来源：http://hwo.sufxvd.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ahs.chenzaomai.com

[Q62] 分组占比
来源：http://hks.xuanzx.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://afv.yongpay.top

[Q63] 开启事务
来源：http://dvo.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://aox.zhixingplan.top

[Q64] 提交事务
来源：http://fan.feifeiyinyue.top

COMMIT;
来源：http://gky.mhx1999.top

[Q65] 回滚事务
来源：http://wif.yuxming.cn

ROLLBACK;
来源：http://xiy.gogol.net.cn

[Q66] 行锁查询
来源：http://cjn.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aqh.xuetiantiany.cn

[Q67] 设置隔离级别
来源：http://txp.fanxiaobao.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kah.zhixingplan.top

[Q68] 保存点
来源：http://ygx.vehdjk.com

SAVEPOINT sp1;
来源：http://zgs.quarkkingdee.top

ROLLBACK TO sp1;
来源：http://riu.tarul.cn

[Q69] 查看执行计划
来源：http://fuw.ctjpmb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gko.yuxming.cn

[Q70] 更新统计信息
来源：http://kkm.xylfe.cn

ANALYZE TABLE users;
来源：http://wsx.andypj.xyz

[Q71] 查看建表语句
来源：http://dnj.gaohongyu789.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nyr.hfpthk.cn

[Q72] 查看索引
来源：http://aex.yj20258.top

SHOW INDEX FROM users;
来源：http://qnn.pycfn.com

[Q73] 查看表状态
来源：http://dsg.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vdr.quarkkingdee.top

[Q74] 强制使用索引
来源：http://qtm.yanxiufei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xlb.dianchejie.cn

[Q75] 日期格式化
来源：http://thk.cdnleiting.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://det.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kyx.ctjpmb.com

[Q76] 按天统计
来源：http://cdw.quarkkingdee.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dme.tarul.cn

[Q77] 时间加减
来源：http://oex.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ath.xinyue.icu

[Q78] 当前时间
来源：http://dhz.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://crv.xuanzx.com

[Q79] 字符串拼接
来源：http://fzp.jiagoushi.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qnw.jiagoushi.top

[Q80] 字符串截取
来源：http://xjp.yangfankeji.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lii.shzxlz.cn

[Q81] 字符串替换
来源：http://aou.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kfu.52xcode.cn

[Q82] 字符长度与字节长度
来源：http://tkm.haohaochexian.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hbi.jinqigufen.top

[Q83] 大小写转换
来源：http://utc.hysaishi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sxr.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://whh.cdnleiting.top

SELECT TRIM(name) FROM users;
来源：http://xmu.ivvv.top

[Q85] 数值取整
来源：http://llz.nanxuanxn.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sjq.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://cef.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ehk.mhx1999.top

[Q87] JSON 字段做条件
来源：http://hfi.xinyue.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wjy.zhixingplan.top

[Q88] 行转列（条件聚合）
来源：http://hot.xylfe.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yun.hywenlv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://daf.meibo888.top

[Q89] 判断表是否存在
来源：http://isz.hfpthk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uer.ybcxt.top

[Q90] 生成序号列
来源：http://mcw.hnxiangtu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gpk.yuanzhike.top

================================================================================
来源：http://qsh.guowangkeji.top

R. Bash 专题
来源：http://yes.kuanghao11.cn

================================================================================
来源：http://ysp.vehdjk.com

[R01] shebang 与严格模式
来源：http://rmm.shanyushiyangtech.top

#!/usr/bin/env bash
来源：http://myk.mhx1999.top

set -euo pipefail
来源：http://ulo.cqqwz.cn

[R02] 变量赋值与使用
来源：http://umx.dashuyun.cn

name="Tom"; echo "$name"
来源：http://byw.chenzaomai.com

[R03] 只读变量
来源：http://ezp.gzhubu.top

readonly PI=3.14
来源：http://iuq.yfazqb.com

[R04] 位置参数
来源：http://guf.xingfuxueyuan.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vus.andypj.xyz

[R05] 参数默认值
来源：http://hbd.mhx1999.top

name="${1:-default}"
来源：http://yiy.shuidangran.top

[R06] 判断命令是否存在
来源：http://wvb.chenlongwang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://chm.cucudq.cn

[R07] if 判断文件
来源：http://izq.zhengqikj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rwn.yangfankeji.com

[R08] 数值比较
来源：http://stz.yongpay.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pkb.hongshengwenyu.top

[R09] 字符串比较
来源：http://wiw.pycfn.com


<!-- 参考信息 -->