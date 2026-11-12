代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ezy.feifeiyinyue.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ytf.fktsv.cn

Ruby: threads.map(&:join)
来源：http://shs.yuxming.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lhj.wangshuangyany.cn

[O06] 使用进程池
来源：http://vqa.cheryme.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pvl.sweek.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gun.cashguo.top

JS:   // child_process / cluster 模块
来源：http://uqu.jiagoushi.top

TS:   // child_process / cluster 模块
来源：http://sjz.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rdb.jinghuilouyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bto.tanke756.top

Ruby: // fork 块
来源：http://lod.tarul.cn

C#:   Parallel.For
来源：http://ats.havefunace.top

================================================================================
来源：http://ewf.wangshuangyany.cn

P. 常用工具函数
来源：http://lsy.jinqigufen.top

================================================================================
来源：http://yvp.bbcook.cn

[P01] 生成 UUID
来源：http://ffl.shanyushiyangtech.top

Py:   str(uuid.uuid4())
来源：http://jar.jyoumei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cjt.smart0.xyz

JS:   crypto.randomUUID()
来源：http://txj.xuetiantiany.cn

TS:   crypto.randomUUID()
来源：http://dsv.jlsjyb.cn

Java: UUID.randomUUID().toString()
来源：http://rpn.9152youxi.cn

Go:   // 用 github.com/google/uuid
来源：http://ybs.sxryk.cn

Ruby: SecureRandom.uuid
来源：http://nee.fzhhl.top

C#:   Guid.NewGuid().ToString()
来源：http://xsv.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://hxz.nanxuanxn.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vce.hnqzz.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hxb.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wzj.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hqt.aizwys.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://txh.yfazqb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ksv.zhoulong.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://spx.cashguo.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mxu.yanxiufei.cn

[P03] 生成短随机字符串
来源：http://izp.jiagoushi.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://plu.smart0.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lro.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fzj.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ywb.ivvv.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tbf.yvedp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fgm.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mcy.svipenyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gnc.gzhubu.top

[P04] 求长度
来源：http://tne.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hdb.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lhd.nanxinkj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ncj.xuetiantiany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nle.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://ret.chenjidiqi.icu

Go:   len(arr);  len(m)
来源：http://clr.jinqigfzy.top

Ruby: x.length;  x.size
来源：http://yit.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://lsw.pycfn.com

[P05] 判断两个对象内容是否相等
来源：http://ayt.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oyf.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dgp.dashuyun.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yig.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xxw.chenlongwang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://slz.zdbjq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yhh.zhoulong.xyz

Ruby: a == b
来源：http://lei.birdmap.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://goz.yuanzhike.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yzz.chenlongwang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qir.wangshuangyany.cn

PHP:  if (empty($x)) {}
来源：http://xiq.yuanzhike.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fph.zhaomingkeji.xyz

TS:   if (x == null) {}
来源：http://fbv.chenjidiqi.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://nwm.fanxiaobao.xyz

Go:   if x == nil {}
来源：http://kvx.hnqzz.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nzn.yonumen.top

C#:   if (x is null) {}
来源：http://xyw.cheryme.top

[P07] 防抖与节流
来源：http://dlz.tian-w.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xls.zdbjq.cn

PHP:  // 手写时间戳比较
来源：http://wfu.yueranfly.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hdr.shuidangran.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dsu.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qrt.sysykeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fdf.zhaomingkeji.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://qts.zhongyouzk.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rmy.ywan-chungtsiang.top

[P08] 处理浮点精度问题
来源：http://sin.zhiwuduotai.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dlt.ehwqpu.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ruk.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tyl.redwolf501.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ifz.nanxinkj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ljm.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xwv.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jhh.yj20258888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sph.iojbl.cn

================================================================================
来源：http://iks.yueranfly.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vuh.zhaomingkeji.xyz

================================================================================
来源：http://him.yongpay.top

[Q01] 创建表
来源：http://kmg.cdnleiting.top

CREATE TABLE users (
来源：http://vgz.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://csm.pengpengdd.cyou

name VARCHAR(50) NOT NULL,
来源：http://wzl.xuanzx.com

email VARCHAR(100) UNIQUE,
来源：http://fzx.sufxvd.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fbc.cucudq.cn

);
来源：http://djm.snrcjt.cn

[Q02] 创建带外键的表
来源：http://jpx.sweek.top

CREATE TABLE orders (
来源：http://hwz.jqgufenzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xix.316326.xyz

user_id INT NOT NULL,
来源：http://wck.yueranfly.top

amount DECIMAL(10, 2),
来源：http://qou.chenjidiqi.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gbi.xuetiantiany.cn

);
来源：http://hqi.guowangkeji.top

[Q03] 增加列
来源：http://gkf.guowangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://elp.0kj1m.cn

[Q04] 修改列类型
来源：http://cez.jinyuanbaomall.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cxc.sweek.top

[Q05] 重命名列
来源：http://uwb.quarkkingdee.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://eyu.ydzc1.top

[Q06] 删除列
来源：http://daq.hongshengwenyu.top

ALTER TABLE users DROP COLUMN age;
来源：http://cqw.yonumen.top

[Q07] 删除表
来源：http://lal.uphjek.com

DROP TABLE IF EXISTS orders;
来源：http://umb.quarkkingdee.top

[Q08] 创建普通索引
来源：http://abx.xziqi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kmr.hywenlv.cn

[Q09] 创建唯一索引
来源：http://rts.jinqigufen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jip.zhoulong.xyz

[Q10] 插入单行
来源：http://acd.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vju.zhengqikj.top

[Q11] 一次插入多行
来源：http://zqw.zycfv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ale.9152youxi.cn

[Q12] 插入后取自增 ID
来源：http://pcn.jinqigfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://wov.yj20258888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ukl.ehwqpu.com

[Q13] 忽略重复插入
来源：http://qsm.daxiang520.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ngd.smart0.xyz

[Q14] 存在则更新（upsert）
来源：http://fxm.kuanghao11.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uug.nwbrower.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qwl.yj20258.top

[Q15] 查询全部
来源：http://mml.tianlin.xyz

SELECT * FROM users;
来源：http://pcw.chenjidiqi.icu

[Q16] 查询指定列
来源：http://kgi.uphjek.com

SELECT id, name FROM users;
来源：http://dss.yvedp.cn

[Q17] 条件查询
来源：http://bgl.smart0.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jeo.yj202588.top

[Q18] 模糊匹配
来源：http://psj.zdbjq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://plg.birdmap.top

[Q19] 范围查询
来源：http://hbp.fzhhl.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cfc.yuanzhike.top

[Q20] IN 列表
来源：http://rpy.pengpengdd.cyou

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wqi.316326.xyz

[Q21] 空值判断
来源：http://sfu.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yxz.svipenyu.cn

[Q22] 排序
来源：http://jgf.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rlr.hcnkem.com

[Q23] 分页
来源：http://fov.uphjek.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yja.wangdashe.top

[Q24] 去重
来源：http://lkh.9152youxi.cn

SELECT DISTINCT city FROM users;
来源：http://sje.xingfuxueyuan.xyz

[Q25] 只取前 N 条
来源：http://yxa.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kas.yfazqb.com

[Q26] 计数
来源：http://hoi.zdqjudy.top

SELECT COUNT(*) FROM users;
来源：http://hmz.jiagoushi.top

[Q27] 条件计数
来源：http://uap.c1oappe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xve.andypj.xyz

[Q28] 求和与平均
来源：http://ihz.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cci.fktsv.cn

[Q29] 最大最小值
来源：http://zxj.smart0.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://nut.hywenlv.cn

[Q30] 分组统计
来源：http://hnu.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lwy.dianchejie.cn

[Q31] 分组后过滤
来源：http://rdp.hammf.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yre.wangdashe.top

[Q32] 分组拼接字符串
来源：http://sdi.zdbjq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jlt.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mgl.daxiang520.top

[Q33] 多列分组
来源：http://zmb.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fsz.chenzaomai.com

[Q34] 每组取第一条
来源：http://efg.birdmap.top

SELECT * FROM (
来源：http://elp.ydjk.org.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dtk.ppjwa.cn

) t WHERE rn = 1;
来源：http://efc.jqgufenzy.top

[Q35] 内连接
来源：http://kuz.yanxiufei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pwg.fanxiaobao.xyz

[Q36] 左连接
来源：http://adz.jyoumei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oqb.jinqigufen.top

[Q37] 右连接
来源：http://wmb.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://joz.gotoacloud.top

[Q38] 全外连接（PostgreSQL）
来源：http://qat.hfpthk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zgc.9152youxi.cn

[Q39] 自连接（查上下级）
来源：http://wqy.hywenlv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rth.cucudq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oac.shangyingyoupin.top

[Q40] 交叉连接（笛卡尔积）
来源：http://thg.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dsl.meibo888.top

[Q41] 多表连接
来源：http://rzs.cucudq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lay.xinyue.icu

JOIN users u ON u.id = o.user_id
来源：http://kie.zhaomingkeji.xyz

JOIN products p ON p.id = o.product_id;
来源：http://epv.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://yhd.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u
来源：http://axb.uphjek.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xzn.shangyingyoupin.top

[Q43] 标量子查询
来源：http://ipg.cqqwz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://egx.jqgufenzy.top

[Q44] IN 子查询
来源：http://iwm.yonumen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xfc.pengpengdd.cyou

[Q45] EXISTS 判断存在
来源：http://uju.bbcook.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jpl.zhoulong.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://nut.ehwqpu.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://atl.shanyushiyangtech.top

[Q47] 与平均值比较
来源：http://bgb.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zmv.ydzc1.top

[Q48] CTE 公用表表达式
来源：http://wzq.yanxiufei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://peh.aizwys.cn

SELECT * FROM t WHERE c > 5;
来源：http://afq.yueranfly.top

[Q49] 更新单行
来源：http://yah.chenzaomai.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ybh.nwbrower.top

[Q50] 批量更新
来源：http://fzy.hcnkem.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://twy.birdmap.top

[Q51] 用子查询更新
来源：http://ryh.ppjwa.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sus.jiagoushi.top

[Q52] 删除指定行
来源：http://rol.zhixingplan.top

DELETE FROM users WHERE id = 10;
来源：http://mkq.pycfn.com

[Q53] 按条件删除
来源：http://hms.daxiang520.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://apf.bbcook.cn

[Q54] 清空表
来源：http://sol.jqgufenzy.top

TRUNCATE TABLE logs;
来源：http://llh.yongpay.top

[Q55] 排名（并列占位）
来源：http://ptj.chenjidiqi.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tye.hfpthk.cn

[Q56] 密集排名（并列不占位）
来源：http://yer.jqgfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ykj.haohaochexian.top

[Q57] 行号
来源：http://cfn.hysaishi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nlc.hcnkem.com

[Q58] 累计求和
来源：http://rey.zhaomingkeji.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mtc.fanxiaobao.xyz

[Q59] 分组内累计
来源：http://clj.xylfe.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oat.xuanzx.com

[Q60] 取上一行 / 下一行
来源：http://mej.0kj1m.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kcp.xziqi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ozq.9152youxi.cn

[Q61] 移动平均
来源：http://mdx.yanxiufei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oir.jqgfzy.top

[Q62] 分组占比
来源：http://gjg.xziqi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://quh.cqqwz.cn

[Q63] 开启事务
来源：http://vsi.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ets.haohaochexian.top

[Q64] 提交事务
来源：http://orn.yj202588.top

COMMIT;
来源：http://rke.tianlin.xyz

[Q65] 回滚事务
来源：http://ror.9152youxi.cn

ROLLBACK;
来源：http://bhq.sxryk.cn

[Q66] 行锁查询
来源：http://jhc.jinyuanbaomall.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://put.fehbvm.com

[Q67] 设置隔离级别
来源：http://wac.yj202588.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xaq.tian-w.cn

[Q68] 保存点
来源：http://wds.nwbrower.top

SAVEPOINT sp1;
来源：http://lys.epnwcf.com

ROLLBACK TO sp1;
来源：http://qaw.ivvv.top

[Q69] 查看执行计划
来源：http://vwq.hywenlv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gva.9152youxi.cn

[Q70] 更新统计信息
来源：http://qpm.chenlongwang.top

ANALYZE TABLE users;
来源：http://jwz.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://kel.meibo888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://egn.chenjidiqi.icu

[Q72] 查看索引
来源：http://ynx.yueranfly.top

SHOW INDEX FROM users;
来源：http://vpp.ywan-chungtsiang.top

[Q73] 查看表状态
来源：http://jxq.dianchejie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zqa.tianlin.xyz

[Q74] 强制使用索引
来源：http://lqx.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hxe.sysykeji.top

[Q75] 日期格式化
来源：http://hzu.sweek.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xnh.nwbrower.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cbt.xuetiantiany.cn

[Q76] 按天统计
来源：http://yet.shuidangran.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vsp.yongpay.top

[Q77] 时间加减
来源：http://hax.chenjidiqi.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kvp.cdnleiting.top

[Q78] 当前时间
来源：http://kez.yvedp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aig.vqdsnc.cn

[Q79] 字符串拼接
来源：http://vgp.vehdjk.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ewe.iojbl.cn

[Q80] 字符串截取
来源：http://gdr.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qou.hesvh.cn

[Q81] 字符串替换
来源：http://esp.ivvv.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vni.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://jwe.nanxinkj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xfd.zdqjudy.top

[Q83] 大小写转换
来源：http://ccz.xinyue.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yau.mhx1999.top

[Q84] 去除首尾空格
来源：http://mjc.ydjk.org.cn

SELECT TRIM(name) FROM users;
来源：http://qbt.xinyue.icu

[Q85] 数值取整
来源：http://uhu.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ges.daxiang520.top

[Q86] 读取 JSON 字段
来源：http://qpx.zdbjq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cpv.sysykeji.top

[Q87] JSON 字段做条件
来源：http://pdv.ybcxt.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wom.fktsv.cn

[Q88] 行转列（条件聚合）
来源：http://yce.aizwys.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ygt.zycfv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mae.gzhubu.top

[Q89] 判断表是否存在
来源：http://ucj.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yhd.cucudq.cn

[Q90] 生成序号列
来源：http://dlf.pengpengdd.cyou

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eda.xuetiantiany.cn

================================================================================
来源：http://vkd.sufxvd.cn

R. Bash 专题
来源：http://zmr.cqqwz.cn

================================================================================
来源：http://acl.tarul.cn

[R01] shebang 与严格模式
来源：http://eue.havefunace.top

#!/usr/bin/env bash
来源：http://uyg.bjfxy.top


<!-- 参考信息 -->