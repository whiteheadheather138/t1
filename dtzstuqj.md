代发 wailian999

[O06] 使用进程池
来源：http://beh.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nun.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://srs.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://eos.kuanghao11.cn

TS:   // child_process / cluster 模块
来源：http://rxy.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cwq.zhixingplan.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mqo.cqqwz.cn

Ruby: // fork 块
来源：http://ytz.zhijiandao.cn

C#:   Parallel.For
来源：http://oze.shuidangran.top

================================================================================
来源：http://lki.gotoacloud.top

P. 常用工具函数
来源：http://yhj.yanxiufei.cn

================================================================================
来源：http://ntm.cqqwz.cn

[P01] 生成 UUID
来源：http://uap.yj20258888.top

Py:   str(uuid.uuid4())
来源：http://dvg.ivvv.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hxv.ywan-chungtsiang.top

JS:   crypto.randomUUID()
来源：http://bpu.sufxvd.cn

TS:   crypto.randomUUID()
来源：http://btg.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://bdr.xuanzx.com

Go:   // 用 github.com/google/uuid
来源：http://wlf.jianghu66.top

Ruby: SecureRandom.uuid
来源：http://xya.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://sjg.xinyue.icu

[P02] MD5 / SHA256 摘要
来源：http://uaw.tarul.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ihf.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bmd.hfpthk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xnl.shangyingyoupin.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://act.dianchejie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zvn.hcnkem.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hnr.jqgfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ixe.guannengcc.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://swp.zhoulong.xyz

[P03] 生成短随机字符串
来源：http://quj.kuanghao11.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oyw.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oxi.chenzaomai.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bqj.quarkkingdee.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vua.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bad.sxryk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bca.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ghi.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vjm.guannengcc.top

[P04] 求长度
来源：http://oqd.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ucr.jinqigfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hla.sjlbkw.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://scr.meibo888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mhq.ydjk.org.cn

Java: list.size();  map.size();  s.length()
来源：http://dxt.gzhubu.top

Go:   len(arr);  len(m)
来源：http://iex.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://ihb.ehwqpu.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://yuf.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://bje.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://thm.cheryme.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gfv.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mbb.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://txu.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ddz.gaohongyu789.top

Go:   reflect.DeepEqual(a, b)
来源：http://fqu.xziqi.cn

Ruby: a == b
来源：http://xrc.zhijiandao.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nlp.zhongyouzk.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qqf.xuetiantiany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hoq.cheryme.top

PHP:  if (empty($x)) {}
来源：http://ubo.sxryk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dim.cashguo.top

TS:   if (x == null) {}
来源：http://qtt.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://lal.quarkkingdee.top

Go:   if x == nil {}
来源：http://wlv.xingfuxueyuan.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://djj.sufxvd.cn

C#:   if (x is null) {}
来源：http://zuc.xylfe.cn

[P07] 防抖与节流
来源：http://hgw.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vas.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://gmi.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fgw.chenzaomai.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qoe.jianghu66.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wcf.vehdjk.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pbf.yongpay.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yzm.gzhubu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ntn.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://rcw.zdqjudy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vne.shanyushiyangtech.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nka.uphjek.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://itf.jqgufenzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://plu.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fuv.zhijiandao.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tzf.nanxinkj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mlx.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dbt.cashguo.top

================================================================================
来源：http://ebn.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mrg.fanxiaobao.xyz

================================================================================
来源：http://fqe.ehwqpu.com

[Q01] 创建表
来源：http://axm.shangyingyoupin.top

CREATE TABLE users (
来源：http://vuu.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ice.sxryk.cn

name VARCHAR(50) NOT NULL,
来源：http://jjz.ppjwa.cn

email VARCHAR(100) UNIQUE,
来源：http://ala.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hys.yj202588.top

);
来源：http://rii.c1oappe.top

[Q02] 创建带外键的表
来源：http://liu.zhixingplan.top

CREATE TABLE orders (
来源：http://ope.gotoacloud.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rxe.svipenyu.cn

user_id INT NOT NULL,
来源：http://qwc.cucudq.cn

amount DECIMAL(10, 2),
来源：http://bqm.yuxming.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ktb.chenjidiqi.icu

);
来源：http://ntm.pengpengdd.cyou

[Q03] 增加列
来源：http://hpo.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lcj.shanyushiyangtech.top

[Q04] 修改列类型
来源：http://slz.haohaochexian.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uhz.hnqzz.top

[Q05] 重命名列
来源：http://mrq.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://djq.52xcode.cn

[Q06] 删除列
来源：http://dmz.yonumen.top

ALTER TABLE users DROP COLUMN age;
来源：http://fer.pycfn.com

[Q07] 删除表
来源：http://wcd.fengsongda.top

DROP TABLE IF EXISTS orders;
来源：http://pop.shangyingyoupin.top

[Q08] 创建普通索引
来源：http://ihd.jinqigfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gbb.jinghuilouyu.cn

[Q09] 创建唯一索引
来源：http://jiv.smart0.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qfr.xuetiantiany.cn

[Q10] 插入单行
来源：http://sbr.ppjwa.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nxw.yj20258888.top

[Q11] 一次插入多行
来源：http://psd.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://idy.pengpengdd.cyou

[Q12] 插入后取自增 ID
来源：http://uqs.cqqwz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://njv.guannengcc.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hit.wangdashe.top

[Q13] 忽略重复插入
来源：http://rhp.hnxiangtu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://opw.shzxlz.cn

[Q14] 存在则更新（upsert）
来源：http://ifw.hfpthk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://suu.fanxiaobao.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rnf.jinyuanbaomall.cn

[Q15] 查询全部
来源：http://tjp.hnqzz.top

SELECT * FROM users;
来源：http://zyu.iojbl.cn

[Q16] 查询指定列
来源：http://tga.chenlongwang.top

SELECT id, name FROM users;
来源：http://tik.fktsv.cn

[Q17] 条件查询
来源：http://xaa.snrcjt.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://flr.smart0.xyz

[Q18] 模糊匹配
来源：http://yec.mhx1999.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xjn.cheryme.top

[Q19] 范围查询
来源：http://aeu.yj20258.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ycz.hysaishi.cn

[Q20] IN 列表
来源：http://sot.hywenlv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kcv.zhijiandao.cn

[Q21] 空值判断
来源：http://trm.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pga.ywan-chungtsiang.top

[Q22] 排序
来源：http://skj.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bhs.shanyushiyangtech.top

[Q23] 分页
来源：http://ddv.kuanghao11.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://twk.vehdjk.com

[Q24] 去重
来源：http://jkm.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://boj.zdqjudy.top

[Q25] 只取前 N 条
来源：http://mxl.snrcjt.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vby.chenjidiqi.icu

[Q26] 计数
来源：http://rjn.zhongyouzk.top

SELECT COUNT(*) FROM users;
来源：http://zqr.andypj.xyz

[Q27] 条件计数
来源：http://uxm.snrcjt.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wvy.yj202588.top

[Q28] 求和与平均
来源：http://ixb.kuanghao11.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mim.svipenyu.cn

[Q29] 最大最小值
来源：http://zth.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wmk.yongpay.top

[Q30] 分组统计
来源：http://miq.daria6918.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://elx.aibaodan.cn

[Q31] 分组后过滤
来源：http://gap.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gcf.ydjk.org.cn

[Q32] 分组拼接字符串
来源：http://qgi.aibaodan.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tkc.ydzc1.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pmc.chenzaomai.com

[Q33] 多列分组
来源：http://skh.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wch.ehwqpu.com

[Q34] 每组取第一条
来源：http://aom.nanxuanxn.top

SELECT * FROM (
来源：http://byv.xziqi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://unv.yj20258888.top

) t WHERE rn = 1;
来源：http://jzn.yj202588.top

[Q35] 内连接
来源：http://eiu.sxryk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cpo.cashguo.top

[Q36] 左连接
来源：http://ddd.nwbrower.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eri.jqgfzy.top

[Q37] 右连接
来源：http://qbz.havefunace.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cbj.hfpthk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ojb.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://per.meibo888.top

[Q39] 自连接（查上下级）
来源：http://lzv.ywan-chungtsiang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ady.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gbm.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://obv.kuanghao11.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pbl.chenlongwang.top

[Q41] 多表连接
来源：http://anx.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rmn.fehbvm.com

JOIN users u ON u.id = o.user_id
来源：http://amh.hfpthk.cn

JOIN products p ON p.id = o.product_id;
来源：http://pmn.pycfn.com

[Q42] 连接条件附加过滤
来源：http://xjy.aizwys.cn

SELECT u.name, o.amount FROM users u
来源：http://hdv.hcnkem.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://txk.ydzc1.top

[Q43] 标量子查询
来源：http://gup.gotoacloud.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mzg.dashuyun.cn

[Q44] IN 子查询
来源：http://sjv.sjlbkw.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pga.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://ywy.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vpa.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xbu.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://slm.chenlongwang.top

[Q47] 与平均值比较
来源：http://mck.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gtr.havefunace.top

[Q48] CTE 公用表表达式
来源：http://yuw.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lpe.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://gak.fanxiaobao.xyz

[Q49] 更新单行
来源：http://osn.jyoumei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://spr.guowangkeji.top

[Q50] 批量更新
来源：http://vpk.sjlbkw.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wgi.hesvh.cn

[Q51] 用子查询更新
来源：http://gey.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gyd.ywan-chungtsiang.top

[Q52] 删除指定行
来源：http://vuj.xinyue.icu

DELETE FROM users WHERE id = 10;
来源：http://wyf.wangshuangyany.cn

[Q53] 按条件删除
来源：http://wgd.zhoulong.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wan.aizwys.cn

[Q54] 清空表
来源：http://dqp.hnqzz.top

TRUNCATE TABLE logs;
来源：http://lxw.nanxinkj.top

[Q55] 排名（并列占位）
来源：http://liv.ybcxt.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ajz.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://jnn.xuetiantiany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pdu.zdbjq.cn

[Q57] 行号
来源：http://rfh.dashuyun.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ekd.hesvh.cn

[Q58] 累计求和
来源：http://zmo.mhx1999.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://biv.dianchejie.cn

[Q59] 分组内累计
来源：http://eqj.zdbjq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jev.gotoacloud.top

[Q60] 取上一行 / 下一行
来源：http://tki.vehdjk.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://brm.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wdi.uphjek.com

[Q61] 移动平均
来源：http://fcx.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dsu.sxryk.cn

[Q62] 分组占比
来源：http://qlj.ehwqpu.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qlo.zhiwuduotai.top

[Q63] 开启事务
来源：http://dmd.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qmm.zhijiandao.cn

[Q64] 提交事务
来源：http://iht.hfpthk.cn

COMMIT;
来源：http://ikb.gotoacloud.top

[Q65] 回滚事务
来源：http://mrm.tarul.cn

ROLLBACK;
来源：http://loy.vqdsnc.cn

[Q66] 行锁查询
来源：http://krs.birdmap.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://txy.kuanghao11.cn

[Q67] 设置隔离级别
来源：http://ywh.cashguo.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vis.sysykeji.top

[Q68] 保存点
来源：http://jae.xylfe.cn

SAVEPOINT sp1;
来源：http://wtu.xinyue.icu

ROLLBACK TO sp1;
来源：http://rob.zhaomingkeji.xyz

[Q69] 查看执行计划
来源：http://nxz.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ozo.fktsv.cn

[Q70] 更新统计信息
来源：http://nec.jinqigfzy.top

ANALYZE TABLE users;
来源：http://hnr.ctjpmb.com

[Q71] 查看建表语句
来源：http://lar.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zcb.pengpengdd.cyou

[Q72] 查看索引
来源：http://tvs.yueranfly.top

SHOW INDEX FROM users;
来源：http://qtz.wangshuangyany.cn

[Q73] 查看表状态
来源：http://ftv.bbcook.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oed.shanyushiyangkeji.top

[Q74] 强制使用索引
来源：http://yzh.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pcn.nwbrower.top

[Q75] 日期格式化
来源：http://esa.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ygs.svipenyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://osb.tianlin.xyz

[Q76] 按天统计
来源：http://drx.jlsjyb.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mii.bbcook.cn

[Q77] 时间加减
来源：http://hru.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hye.sufxvd.cn

[Q78] 当前时间
来源：http://pgf.sxryk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ine.9152youxi.cn

[Q79] 字符串拼接
来源：http://jvl.tianlin.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qtp.yongpay.top

[Q80] 字符串截取
来源：http://fir.zdqjudy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zgb.yanxiufei.cn

[Q81] 字符串替换
来源：http://ifq.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nue.mhx1999.top

[Q82] 字符长度与字节长度
来源：http://zuv.yanxiufei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://res.meibo888.top

[Q83] 大小写转换
来源：http://met.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yzx.zdqjudy.top

[Q84] 去除首尾空格
来源：http://uij.smart0.xyz

SELECT TRIM(name) FROM users;
来源：http://zsa.hywenlv.cn

[Q85] 数值取整
来源：http://dha.andypj.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ofa.xinyue.icu

[Q86] 读取 JSON 字段
来源：http://rje.zhixingplan.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://naf.jlsjyb.cn

[Q87] JSON 字段做条件
来源：http://bnm.andypj.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jqz.ppjwa.cn

[Q88] 行转列（条件聚合）
来源：http://wrs.ctjpmb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jou.cqqwz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vjh.chenlongwang.top

[Q89] 判断表是否存在
来源：http://pbs.yonumen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kdd.chenjidiqi.icu

[Q90] 生成序号列
来源：http://pgi.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mgb.bbcook.cn

================================================================================
来源：http://yuy.ybcxt.top

R. Bash 专题
来源：http://nhq.kuanghao11.cn

================================================================================
来源：http://kkh.zhengqikj.top

[R01] shebang 与严格模式
来源：http://meh.yfazqb.com

#!/usr/bin/env bash
来源：http://qdi.shanyushiyangkeji.top

set -euo pipefail
来源：http://vny.pycfn.com

[R02] 变量赋值与使用
来源：http://bpz.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://xsj.fanxiaobao.xyz

[R03] 只读变量
来源：http://due.cheryme.top


<!-- 参考信息 -->