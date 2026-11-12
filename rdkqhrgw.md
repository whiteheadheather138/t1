代发 wailian999

C#:   Parallel.For
来源：http://czl.hnqzz.top

================================================================================
来源：http://khc.zhengqikj.top

P. 常用工具函数
来源：http://jss.daxiang520.top

================================================================================
来源：http://jap.sxryk.cn

[P01] 生成 UUID
来源：http://uen.ppjwa.cn

Py:   str(uuid.uuid4())
来源：http://lgu.jlsjyb.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mjy.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://rep.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://iup.hnqzz.top

Java: UUID.randomUUID().toString()
来源：http://izb.ydjk.org.cn

Go:   // 用 github.com/google/uuid
来源：http://wbj.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://svn.gzhubu.top

C#:   Guid.NewGuid().ToString()
来源：http://opk.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://xwn.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hyo.aibaodan.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dcm.yongpay.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://smp.tianlin.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sid.zhiwuduotai.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hzq.yueranfly.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://trd.shanyushiyangtech.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tpk.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zxn.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://xxr.iojbl.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pwo.wangshuangyany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://god.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gso.mhx1999.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gvu.vehdjk.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qvm.yuanzhike.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hrq.yj20258.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://osf.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tmq.jiagoushi.top

[P04] 求长度
来源：http://xro.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xfu.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mzg.guowangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nfv.bbcook.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://avc.0kj1m.cn

Java: list.size();  map.size();  s.length()
来源：http://djc.zdqjudy.top

Go:   len(arr);  len(m)
来源：http://fiv.pycfn.com

Ruby: x.length;  x.size
来源：http://wrt.gotoacloud.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dwp.hnxiangtu.top

[P05] 判断两个对象内容是否相等
来源：http://pyj.chenzaomai.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ktx.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ibn.cqqwz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gyt.xingfuxueyuan.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cwj.xziqi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://les.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ogc.yonumen.top

Ruby: a == b
来源：http://gms.vehdjk.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hmd.0kj1m.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kef.dashuyun.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://elg.cashguo.top

PHP:  if (empty($x)) {}
来源：http://pka.wangshuangyany.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lnh.pycfn.com

TS:   if (x == null) {}
来源：http://wub.nanxinkj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dnh.hfpthk.cn

Go:   if x == nil {}
来源：http://fuh.yuxming.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nqg.meibo888.top

C#:   if (x is null) {}
来源：http://ztm.chenlongwang.top

[P07] 防抖与节流
来源：http://inb.jiagoushi.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gkg.shangyingyoupin.top

PHP:  // 手写时间戳比较
来源：http://vzo.epnwcf.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aev.gogol.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://onl.xinyue.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kbc.ppjwa.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cgi.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wyg.meibo888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lod.shzxlz.cn

[P08] 处理浮点精度问题
来源：http://pqk.guowangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rmc.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hrc.nanxuanxn.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xmh.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dnk.gzhubu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vto.shuidangran.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://djt.aibaodan.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nkz.shuidangran.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nmj.birdmap.top

================================================================================
来源：http://amh.yuanzhike.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bvn.wangshuangyany.cn

================================================================================
来源：http://eca.gotoacloud.top

[Q01] 创建表
来源：http://quy.fehbvm.com

CREATE TABLE users (
来源：http://psl.wangdashe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pmm.kuanghao11.cn

name VARCHAR(50) NOT NULL,
来源：http://mjc.chenlongwang.top

email VARCHAR(100) UNIQUE,
来源：http://iwy.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nlr.hfpthk.cn

);
来源：http://ffm.yj202588.top

[Q02] 创建带外键的表
来源：http://gjg.yj20258888.top

CREATE TABLE orders (
来源：http://ugy.316326.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wcu.daxiang520.top

user_id INT NOT NULL,
来源：http://viv.daxiang520.top

amount DECIMAL(10, 2),
来源：http://ihj.vehdjk.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uda.zhaomingkeji.xyz

);
来源：http://cgd.zhongyouzk.top

[Q03] 增加列
来源：http://yrp.cashguo.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vul.shzxlz.cn

[Q04] 修改列类型
来源：http://sdg.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oyi.havefunace.top

[Q05] 重命名列
来源：http://ogo.jiagoushi.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hvm.ydzc1.top

[Q06] 删除列
来源：http://kqw.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://tvq.fehbvm.com

[Q07] 删除表
来源：http://lbc.nwbrower.top

DROP TABLE IF EXISTS orders;
来源：http://fbh.sysykeji.top

[Q08] 创建普通索引
来源：http://qgb.vqdsnc.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vdp.jqgufenzy.top

[Q09] 创建唯一索引
来源：http://mce.vehdjk.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gmo.ctjpmb.com

[Q10] 插入单行
来源：http://dsz.chenlongwang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hyj.tianlin.xyz

[Q11] 一次插入多行
来源：http://vom.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ghc.yj202588.top

[Q12] 插入后取自增 ID
来源：http://hrg.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qli.nanxinkj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oga.guannengcc.top

[Q13] 忽略重复插入
来源：http://cyt.shanyushiyangtech.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wia.gotoacloud.top

[Q14] 存在则更新（upsert）
来源：http://jcf.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yfy.chenzaomai.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oxh.cheryme.top

[Q15] 查询全部
来源：http://xcc.jiagoushi.top

SELECT * FROM users;
来源：http://ovn.gotoacloud.top

[Q16] 查询指定列
来源：http://fdb.jinyuanbaomall.cn

SELECT id, name FROM users;
来源：http://vpk.nwbrower.top

[Q17] 条件查询
来源：http://pdt.cqqwz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lbr.xylfe.cn

[Q18] 模糊匹配
来源：http://isq.wangdashe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zjg.fzhhl.top

[Q19] 范围查询
来源：http://sor.zhijiandao.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://krr.9152youxi.cn

[Q20] IN 列表
来源：http://tud.hnxiangtu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bam.meibo888.top

[Q21] 空值判断
来源：http://efu.gogol.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ssp.fzhhl.top

[Q22] 排序
来源：http://wvq.yongpay.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ywd.fengsongda.top

[Q23] 分页
来源：http://rbr.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lnb.ivvv.top

[Q24] 去重
来源：http://vgs.yvedp.cn

SELECT DISTINCT city FROM users;
来源：http://sfw.daxiang520.top

[Q25] 只取前 N 条
来源：http://vef.dianchejie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sao.52xcode.cn

[Q26] 计数
来源：http://hvr.jlsjyb.cn

SELECT COUNT(*) FROM users;
来源：http://ccb.ywan-chungtsiang.top

[Q27] 条件计数
来源：http://wgo.shanyushiyangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://skc.hesvh.cn

[Q28] 求和与平均
来源：http://voe.ivvv.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wuo.uphjek.com

[Q29] 最大最小值
来源：http://duw.aibaodan.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rmt.aibaodan.cn

[Q30] 分组统计
来源：http://hyh.feifeiyinyue.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://szr.yj202588.top

[Q31] 分组后过滤
来源：http://ipi.sweek.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://krp.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://pif.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://axy.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://upw.nwbrower.top

[Q33] 多列分组
来源：http://ero.hammf.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tbm.ivvv.top

[Q34] 每组取第一条
来源：http://lkm.shuidangran.top

SELECT * FROM (
来源：http://fjx.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tdh.cheryme.top

) t WHERE rn = 1;
来源：http://pof.yongpay.top

[Q35] 内连接
来源：http://sry.zhijiandao.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://agn.xinyue.icu

[Q36] 左连接
来源：http://wcn.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iqv.hesvh.cn

[Q37] 右连接
来源：http://iig.xinyue.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oza.ydjk.org.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gmd.gogol.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://trw.zhoulong.xyz

[Q39] 自连接（查上下级）
来源：http://kgr.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jjg.yuxming.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jdx.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jif.shzxlz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qrz.gzhubu.top

[Q41] 多表连接
来源：http://hwn.shangyingyoupin.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lxp.guowangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://pqp.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://msp.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://qxs.wangshuangyany.cn

SELECT u.name, o.amount FROM users u
来源：http://cyg.gaohongyu789.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uxm.cdnleiting.top

[Q43] 标量子查询
来源：http://anq.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ewm.gzhubu.top

[Q44] IN 子查询
来源：http://weh.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ztn.nwbrower.top

[Q45] EXISTS 判断存在
来源：http://wal.hammf.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mcn.9152youxi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://znb.c1oappe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jqu.gotoacloud.top

[Q47] 与平均值比较
来源：http://jrq.hywenlv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bab.pycfn.com

[Q48] CTE 公用表表达式
来源：http://ccc.jinqigufen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jlj.shangyingyoupin.top

SELECT * FROM t WHERE c > 5;
来源：http://cww.zycfv.cn

[Q49] 更新单行
来源：http://lmi.daria6918.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cvb.zhongyouzk.top

[Q50] 批量更新
来源：http://cfa.feifeiyinyue.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hqh.gaohongyu789.top

[Q51] 用子查询更新
来源：http://eqt.0kj1m.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fuw.hongshengwenyu.top

[Q52] 删除指定行
来源：http://rje.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://emy.uphjek.com

[Q53] 按条件删除
来源：http://bip.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://grk.daxiang520.top

[Q54] 清空表
来源：http://apj.guannengcc.top

TRUNCATE TABLE logs;
来源：http://kwm.jianghu66.top

[Q55] 排名（并列占位）
来源：http://gmh.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ysf.mhx1999.top

[Q56] 密集排名（并列不占位）
来源：http://bke.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zre.sxryk.cn

[Q57] 行号
来源：http://bua.haohaochexian.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ccc.dashuyun.cn

[Q58] 累计求和
来源：http://shw.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uua.ehwqpu.com

[Q59] 分组内累计
来源：http://nlm.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mqj.wangdashe.top

[Q60] 取上一行 / 下一行
来源：http://wca.pycfn.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fop.hywenlv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ylo.ydzc1.top

[Q61] 移动平均
来源：http://ftx.hammf.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vfx.xylfe.cn

[Q62] 分组占比
来源：http://zho.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nio.pycfn.com

[Q63] 开启事务
来源：http://avs.yvedp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ile.guowangkeji.top

[Q64] 提交事务
来源：http://etu.gaohongyu789.top

COMMIT;
来源：http://tac.gaohongyu789.top

[Q65] 回滚事务
来源：http://tel.bjfxy.top

ROLLBACK;
来源：http://qrz.gaohongyu789.top

[Q66] 行锁查询
来源：http://taa.daxiang520.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pdk.yongpay.top

[Q67] 设置隔离级别
来源：http://zwt.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hyo.hnxiangtu.top

[Q68] 保存点
来源：http://ysl.daxiang520.top

SAVEPOINT sp1;
来源：http://swp.316326.xyz

ROLLBACK TO sp1;
来源：http://yod.hcnkem.com

[Q69] 查看执行计划
来源：http://bft.yfazqb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://acq.ppjwa.cn

[Q70] 更新统计信息
来源：http://xuc.chenjidiqi.icu

ANALYZE TABLE users;
来源：http://bwh.9152youxi.cn

[Q71] 查看建表语句
来源：http://smo.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hqs.gotoacloud.top

[Q72] 查看索引
来源：http://npy.aibaodan.cn

SHOW INDEX FROM users;
来源：http://hcz.tian-w.cn

[Q73] 查看表状态
来源：http://hxs.andypj.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://and.zhiwuduotai.top

[Q74] 强制使用索引
来源：http://crx.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://weg.hesvh.cn

[Q75] 日期格式化
来源：http://sqn.pengpengdd.cyou

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qiu.ivvv.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://atn.sufxvd.cn

[Q76] 按天统计
来源：http://gik.aizwys.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mlc.daxiang520.top

[Q77] 时间加减
来源：http://lov.zhiwuduotai.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://isc.tanke756.top

[Q78] 当前时间
来源：http://hpf.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jvy.fehbvm.com

[Q79] 字符串拼接
来源：http://rsy.jqgufenzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uoo.bbcook.cn

[Q80] 字符串截取
来源：http://qgr.ctjpmb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uiy.mhx1999.top

[Q81] 字符串替换
来源：http://grv.iojbl.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zfu.xuetiantiany.cn

[Q82] 字符长度与字节长度
来源：http://fai.vqdsnc.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nwg.dashuyun.cn

[Q83] 大小写转换
来源：http://rzf.fanxiaobao.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yxn.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://xkp.xuanzx.com

SELECT TRIM(name) FROM users;
来源：http://kkm.zdbjq.cn

[Q85] 数值取整
来源：http://fsf.xziqi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tro.cqqwz.cn

[Q86] 读取 JSON 字段
来源：http://srh.yj20258888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sqo.zhixingplan.top

[Q87] JSON 字段做条件
来源：http://bif.wangdashe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gbn.fzhhl.top

[Q88] 行转列（条件聚合）
来源：http://vvd.tian-w.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ndf.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rzs.zhoulong.xyz

[Q89] 判断表是否存在
来源：http://csq.sweek.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://flw.fktsv.cn

[Q90] 生成序号列
来源：http://okq.hnxiangtu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://boa.zhaomingkeji.xyz

================================================================================
来源：http://vnc.fzhhl.top

R. Bash 专题
来源：http://kas.c1oappe.top

================================================================================
来源：http://ebz.havefunace.top

[R01] shebang 与严格模式
来源：http://zsk.guowangkeji.top

#!/usr/bin/env bash
来源：http://iyl.tianlin.xyz

set -euo pipefail
来源：http://jbx.ywan-chungtsiang.top

[R02] 变量赋值与使用
来源：http://fgg.chenzaomai.com

name="Tom"; echo "$name"
来源：http://sfr.chenzaomai.com

[R03] 只读变量
来源：http://xhv.yj20258888.top

readonly PI=3.14
来源：http://dos.fengsongda.top

[R04] 位置参数
来源：http://ouw.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lwz.zhaomingkeji.xyz

[R05] 参数默认值
来源：http://zli.chenlongwang.top

name="${1:-default}"
来源：http://hau.hfpthk.cn

[R06] 判断命令是否存在
来源：http://ssr.hammf.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zsk.cucudq.cn

[R07] if 判断文件
来源：http://mrz.zdbjq.cn


<!-- 参考信息 -->