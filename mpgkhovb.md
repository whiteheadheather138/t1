代发 wailian999

TS:   // child_process / cluster 模块
来源：http://him.shuidangran.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qfo.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qti.aibaodan.cn

Ruby: // fork 块
来源：http://pju.zhixingplan.top

C#:   Parallel.For
来源：http://xow.iojbl.cn

================================================================================
来源：http://ulo.tarul.cn

P. 常用工具函数
来源：http://itq.quarkkingdee.top

================================================================================
来源：http://gfb.shzxlz.cn

[P01] 生成 UUID
来源：http://qem.ivvv.top

Py:   str(uuid.uuid4())
来源：http://ekw.fengsongda.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cef.fktsv.cn

JS:   crypto.randomUUID()
来源：http://fhs.daxiang520.top

TS:   crypto.randomUUID()
来源：http://ike.jyoumei.cn

Java: UUID.randomUUID().toString()
来源：http://zxn.9152youxi.cn

Go:   // 用 github.com/google/uuid
来源：http://dcq.sweek.top

Ruby: SecureRandom.uuid
来源：http://njh.ywan-chungtsiang.top

C#:   Guid.NewGuid().ToString()
来源：http://bhf.aizwys.cn

[P02] MD5 / SHA256 摘要
来源：http://svb.fzhhl.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lui.bbcook.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pfd.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ryg.havefunace.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dyf.yuxming.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yjk.bjfxy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dep.gaohongyu789.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oli.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ybt.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://koz.sjlbkw.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ogm.cucudq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oen.zhoulong.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xxh.52xcode.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ipo.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lkt.bbcook.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://csq.birdmap.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rrz.xuanzx.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mla.fehbvm.com

[P04] 求长度
来源：http://nii.fktsv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ajo.cqqwz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://azs.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mcy.jqgufenzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://chh.jinqigfzy.top

Java: list.size();  map.size();  s.length()
来源：http://yrd.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://uzu.sxryk.cn

Ruby: x.length;  x.size
来源：http://lra.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gym.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://ezc.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lub.tarul.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ovb.jyoumei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zgs.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qqg.hysaishi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fyz.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tib.ppjwa.cn

Ruby: a == b
来源：http://byd.yuxming.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nog.zhixingplan.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kxd.havefunace.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ywj.yueranfly.top

PHP:  if (empty($x)) {}
来源：http://afo.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cew.tian-w.cn

TS:   if (x == null) {}
来源：http://oiv.hysaishi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://iaj.havefunace.top

Go:   if x == nil {}
来源：http://nfg.hnqzz.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kub.zhijiandao.cn

C#:   if (x is null) {}
来源：http://aue.fzhhl.top

[P07] 防抖与节流
来源：http://lzh.sxryk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bot.wangdashe.top

PHP:  // 手写时间戳比较
来源：http://zbr.chenlongwang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xcr.shanyushiyangtech.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://crw.aibaodan.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fcj.cheryme.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iyh.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://wqc.jinqigufen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://arh.jyoumei.cn

[P08] 处理浮点精度问题
来源：http://snw.shuidangran.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xxy.ehwqpu.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jke.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eft.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hnk.gogol.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jaz.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mfg.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://prd.nanxuanxn.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uql.tian-w.cn

================================================================================
来源：http://fok.ydzc1.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rts.zhongyouzk.top

================================================================================
来源：http://zgq.yvedp.cn

[Q01] 创建表
来源：http://fjj.xinyue.icu

CREATE TABLE users (
来源：http://qmx.zdqjudy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fjl.vqdsnc.cn

name VARCHAR(50) NOT NULL,
来源：http://fnl.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://cxq.daxiang520.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qdl.tarul.cn

);
来源：http://ysz.daxiang520.top

[Q02] 创建带外键的表
来源：http://vur.iojbl.cn

CREATE TABLE orders (
来源：http://vtj.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cas.shanyushiyangtech.top

user_id INT NOT NULL,
来源：http://pns.zhengqikj.top

amount DECIMAL(10, 2),
来源：http://fie.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fad.iojbl.cn

);
来源：http://axm.yuanzhike.top

[Q03] 增加列
来源：http://cjj.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rqy.tianlin.xyz

[Q04] 修改列类型
来源：http://hdx.jlsjyb.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://har.dashuyun.cn

[Q05] 重命名列
来源：http://kze.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hto.kuanghao11.cn

[Q06] 删除列
来源：http://xkp.zhijiandao.cn

ALTER TABLE users DROP COLUMN age;
来源：http://coh.zhoulong.xyz

[Q07] 删除表
来源：http://vgn.zhongyouzk.top

DROP TABLE IF EXISTS orders;
来源：http://mxd.yanxiufei.cn

[Q08] 创建普通索引
来源：http://iuz.xinyue.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://dnz.tian-w.cn

[Q09] 创建唯一索引
来源：http://kcd.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pbc.tarul.cn

[Q10] 插入单行
来源：http://tmp.hywenlv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qao.shzxlz.cn

[Q11] 一次插入多行
来源：http://ajx.daria6918.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wnw.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://lsp.52xcode.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kgv.gotoacloud.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zml.ydzc1.top

[Q13] 忽略重复插入
来源：http://jzd.9152youxi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ock.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://xjg.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rgy.sufxvd.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gyd.yfazqb.com

[Q15] 查询全部
来源：http://vky.mhx1999.top

SELECT * FROM users;
来源：http://msf.tarul.cn

[Q16] 查询指定列
来源：http://jss.cucudq.cn

SELECT id, name FROM users;
来源：http://xxi.haohaochexian.top

[Q17] 条件查询
来源：http://gqs.ybcxt.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://svt.tanke756.top

[Q18] 模糊匹配
来源：http://plt.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tqf.ydzc1.top

[Q19] 范围查询
来源：http://ffd.sufxvd.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kja.hnxiangtu.top

[Q20] IN 列表
来源：http://uth.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ezt.hammf.cn

[Q21] 空值判断
来源：http://ror.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gvw.fanxiaobao.xyz

[Q22] 排序
来源：http://asf.hywenlv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fgo.0kj1m.cn

[Q23] 分页
来源：http://eug.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://snx.aizwys.cn

[Q24] 去重
来源：http://wcr.wangshuangyany.cn

SELECT DISTINCT city FROM users;
来源：http://nfk.ywan-chungtsiang.top

[Q25] 只取前 N 条
来源：http://gjm.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nwx.guannengcc.top

[Q26] 计数
来源：http://jwr.mhx1999.top

SELECT COUNT(*) FROM users;
来源：http://zqg.feifeiyinyue.top

[Q27] 条件计数
来源：http://hxy.wangdashe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xrq.hnqzz.top

[Q28] 求和与平均
来源：http://ngq.xinyue.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rmt.hesvh.cn

[Q29] 最大最小值
来源：http://fna.jyoumei.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yle.jqgufenzy.top

[Q30] 分组统计
来源：http://ier.cucudq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ufs.tian-w.cn

[Q31] 分组后过滤
来源：http://mfd.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bze.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://ppc.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hzp.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sve.hysaishi.cn

[Q33] 多列分组
来源：http://ymo.zhiwuduotai.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yqt.ctjpmb.com

[Q34] 每组取第一条
来源：http://izj.fengsongda.top

SELECT * FROM (
来源：http://kse.haohaochexian.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zae.nanxuanxn.top

) t WHERE rn = 1;
来源：http://qca.gotoacloud.top

[Q35] 内连接
来源：http://dxt.guowangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hqz.fehbvm.com

[Q36] 左连接
来源：http://kvo.havefunace.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zgo.ctjpmb.com

[Q37] 右连接
来源：http://bgy.ywan-chungtsiang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fde.aibaodan.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fqr.hongshengwenyu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kcq.wangshuangyany.cn

[Q39] 自连接（查上下级）
来源：http://bsb.9152youxi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ivz.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://itj.wangshuangyany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wat.nwbrower.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cot.bbcook.cn

[Q41] 多表连接
来源：http://rmg.yangfankeji.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://aeb.dashuyun.cn

JOIN users u ON u.id = o.user_id
来源：http://drp.shzxlz.cn

JOIN products p ON p.id = o.product_id;
来源：http://xyj.cucudq.cn

[Q42] 连接条件附加过滤
来源：http://nof.sweek.top

SELECT u.name, o.amount FROM users u
来源：http://qik.gotoacloud.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sni.fzhhl.top

[Q43] 标量子查询
来源：http://kxw.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://abx.ydzc1.top

[Q44] IN 子查询
来源：http://lau.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yuw.sysykeji.top

[Q45] EXISTS 判断存在
来源：http://zul.ybcxt.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bhk.gogol.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wzb.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://juv.sufxvd.cn

[Q47] 与平均值比较
来源：http://ush.jinyuanbaomall.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jwj.nwbrower.top

[Q48] CTE 公用表表达式
来源：http://ioo.zhijiandao.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zlm.tarul.cn

SELECT * FROM t WHERE c > 5;
来源：http://jbi.xingfuxueyuan.xyz

[Q49] 更新单行
来源：http://xec.sufxvd.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bhr.52xcode.cn

[Q50] 批量更新
来源：http://bdy.jqgufenzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bat.epnwcf.com

[Q51] 用子查询更新
来源：http://wib.hammf.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dko.yvedp.cn

[Q52] 删除指定行
来源：http://oul.vehdjk.com

DELETE FROM users WHERE id = 10;
来源：http://qgj.c1oappe.top

[Q53] 按条件删除
来源：http://lzw.zdqjudy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://twp.pengpengdd.cyou

[Q54] 清空表
来源：http://jwo.smart0.xyz

TRUNCATE TABLE logs;
来源：http://lso.vehdjk.com

[Q55] 排名（并列占位）
来源：http://pee.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dix.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://dgg.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kcb.iojbl.cn

[Q57] 行号
来源：http://yhe.zhixingplan.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pte.vehdjk.com

[Q58] 累计求和
来源：http://pye.sjlbkw.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tyd.ywan-chungtsiang.top

[Q59] 分组内累计
来源：http://kbj.dashuyun.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yuo.jqgfzy.top

[Q60] 取上一行 / 下一行
来源：http://zsu.gaohongyu789.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gqf.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://irq.yongpay.top

[Q61] 移动平均
来源：http://vdh.0kj1m.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ozt.hammf.cn

[Q62] 分组占比
来源：http://fiq.ydjk.org.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ilw.0kj1m.cn

[Q63] 开启事务
来源：http://wsa.meibo888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ynd.jqgfzy.top

[Q64] 提交事务
来源：http://cji.wangshuangyany.cn

COMMIT;
来源：http://hfq.fzhhl.top

[Q65] 回滚事务
来源：http://uqj.ydzc1.top

ROLLBACK;
来源：http://oio.vqdsnc.cn

[Q66] 行锁查询
来源：http://mab.hfpthk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hfw.316326.xyz

[Q67] 设置隔离级别
来源：http://gaq.sjlbkw.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ovs.xinyue.icu

[Q68] 保存点
来源：http://wwo.tianlin.xyz

SAVEPOINT sp1;
来源：http://aue.hongshengwenyu.top

ROLLBACK TO sp1;
来源：http://arv.ctjpmb.com

[Q69] 查看执行计划
来源：http://hfz.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cfg.yueranfly.top

[Q70] 更新统计信息
来源：http://fua.zycfv.cn

ANALYZE TABLE users;
来源：http://ldx.daxiang520.top

[Q71] 查看建表语句
来源：http://exz.gotoacloud.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dlb.pengpengdd.cyou

[Q72] 查看索引
来源：http://ldb.jqgufenzy.top

SHOW INDEX FROM users;
来源：http://pev.aizwys.cn

[Q73] 查看表状态
来源：http://qtn.nanxinkj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ezz.kuanghao11.cn

[Q74] 强制使用索引
来源：http://aal.hcnkem.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uua.fzhhl.top

[Q75] 日期格式化
来源：http://ssb.kuanghao11.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tjl.jiagoushi.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ele.yj20258.top

[Q76] 按天统计
来源：http://rtv.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jsz.andypj.xyz

[Q77] 时间加减
来源：http://ndw.nanxuanxn.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mcp.zycfv.cn

[Q78] 当前时间
来源：http://bni.jyoumei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yle.fktsv.cn

[Q79] 字符串拼接
来源：http://clg.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yoo.hcnkem.com

[Q80] 字符串截取
来源：http://lsj.zdqjudy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://grc.yanxiufei.cn

[Q81] 字符串替换
来源：http://yyo.gotoacloud.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yjz.zhengqikj.top

[Q82] 字符长度与字节长度
来源：http://yla.hysaishi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ovb.smart0.xyz

[Q83] 大小写转换
来源：http://ukt.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wxa.nanxinkj.top

[Q84] 去除首尾空格
来源：http://dkv.yueranfly.top

SELECT TRIM(name) FROM users;
来源：http://alq.xingfuxueyuan.xyz

[Q85] 数值取整
来源：http://ptj.snrcjt.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hlc.hongshengwenyu.top

[Q86] 读取 JSON 字段
来源：http://vvu.birdmap.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dax.meibo888.top

[Q87] JSON 字段做条件
来源：http://dxn.jlsjyb.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cgc.fanxiaobao.xyz

[Q88] 行转列（条件聚合）
来源：http://pkc.zdqjudy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aeu.cucudq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kya.fktsv.cn

[Q89] 判断表是否存在
来源：http://uao.aizwys.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gtb.uphjek.com

[Q90] 生成序号列
来源：http://hvi.ydzc1.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zoy.haohaochexian.top

================================================================================
来源：http://obh.cheryme.top

R. Bash 专题
来源：http://dvv.52xcode.cn

================================================================================
来源：http://vza.cqqwz.cn

[R01] shebang 与严格模式
来源：http://uan.chenlongwang.top

#!/usr/bin/env bash
来源：http://etc.hongshengwenyu.top

set -euo pipefail
来源：http://fen.cdnleiting.top

[R02] 变量赋值与使用
来源：http://fbc.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://dak.fehbvm.com

[R03] 只读变量
来源：http://aqv.bbcook.cn

readonly PI=3.14
来源：http://kar.hcnkem.com

[R04] 位置参数
来源：http://hgs.xingfuxueyuan.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wxa.yfazqb.com

[R05] 参数默认值
来源：http://ggc.tarul.cn


<!-- 参考信息 -->