代发 wailian999

[O06] 使用进程池
来源：http://pis.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bgq.nwbrower.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pno.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://qin.gogol.net.cn

TS:   // child_process / cluster 模块
来源：http://mnm.daria6918.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yph.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mjn.snrcjt.cn

Ruby: // fork 块
来源：http://rpz.yvedp.cn

C#:   Parallel.For
来源：http://ocf.ydjk.org.cn

================================================================================
来源：http://qvg.ydjk.org.cn

P. 常用工具函数
来源：http://wdy.ctjpmb.com

================================================================================
来源：http://uws.nanxinkj.top

[P01] 生成 UUID
来源：http://crg.shangyingyoupin.top

Py:   str(uuid.uuid4())
来源：http://lka.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uxe.bbcook.cn

JS:   crypto.randomUUID()
来源：http://lje.smart0.xyz

TS:   crypto.randomUUID()
来源：http://fhl.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://vgn.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://gpv.tarul.cn

Ruby: SecureRandom.uuid
来源：http://crs.zdqjudy.top

C#:   Guid.NewGuid().ToString()
来源：http://nna.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://oqp.fktsv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mfh.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hco.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fmq.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mbw.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tir.ywan-chungtsiang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zxu.ivvv.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://alb.hongshengwenyu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://waq.chenzaomai.com

[P03] 生成短随机字符串
来源：http://bfv.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wzr.shanyushiyangkeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wbi.chenjidiqi.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zwp.aibaodan.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xlg.fzhhl.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://myd.sxryk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://der.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vsg.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bdz.9152youxi.cn

[P04] 求长度
来源：http://isu.zhiwuduotai.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gmb.hongshengwenyu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://euy.sweek.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zpo.shangyingyoupin.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://szj.quarkkingdee.top

Java: list.size();  map.size();  s.length()
来源：http://hle.ehwqpu.com

Go:   len(arr);  len(m)
来源：http://gon.yfazqb.com

Ruby: x.length;  x.size
来源：http://srh.ctjpmb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://faj.jyoumei.cn

[P05] 判断两个对象内容是否相等
来源：http://dtx.yangfankeji.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://jfb.shangyingyoupin.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xfi.tianlin.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cdf.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://twi.vehdjk.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oru.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://npr.xziqi.cn

Ruby: a == b
来源：http://kso.jinyuanbaomall.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kux.wangshuangyany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mwp.sjlbkw.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uwr.shangyingyoupin.top

PHP:  if (empty($x)) {}
来源：http://wkm.nanxuanxn.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dov.jqgufenzy.top

TS:   if (x == null) {}
来源：http://cay.ehwqpu.com

Java: if (x == null || x.isEmpty()) {}
来源：http://pba.yangfankeji.com

Go:   if x == nil {}
来源：http://wlk.bjfxy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wwy.sxryk.cn

C#:   if (x is null) {}
来源：http://ukk.jyoumei.cn

[P07] 防抖与节流
来源：http://toe.aizwys.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ekq.yongpay.top

PHP:  // 手写时间戳比较
来源：http://azf.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tav.shzxlz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ubi.jinyuanbaomall.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yqn.andypj.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kus.dianchejie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xba.zhoulong.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://klz.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://yxf.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yjx.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qjk.daria6918.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sra.fzhhl.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pxe.mhx1999.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yan.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hqj.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cqj.gogol.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qhs.cheryme.top

================================================================================
来源：http://cls.ctjpmb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iad.yangfankeji.com

================================================================================
来源：http://oij.dianchejie.cn

[Q01] 创建表
来源：http://xxb.jianghu66.top

CREATE TABLE users (
来源：http://xaw.svipenyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oco.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://qxy.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://cxg.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sby.chenzaomai.com

);
来源：http://rjb.yongpay.top

[Q02] 创建带外键的表
来源：http://lsw.andypj.xyz

CREATE TABLE orders (
来源：http://uei.sweek.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zfn.birdmap.top

user_id INT NOT NULL,
来源：http://ama.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://wyd.zhengqikj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tpv.sweek.top

);
来源：http://vzy.jinghuilouyu.cn

[Q03] 增加列
来源：http://gqz.jinqigufen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fum.yangfankeji.com

[Q04] 修改列类型
来源：http://fwy.wangdashe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pwk.daria6918.cn

[Q05] 重命名列
来源：http://yfn.ydjk.org.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qgt.pycfn.com

[Q06] 删除列
来源：http://uvu.bjfxy.top

ALTER TABLE users DROP COLUMN age;
来源：http://eet.cheryme.top

[Q07] 删除表
来源：http://xlf.wangdashe.top

DROP TABLE IF EXISTS orders;
来源：http://azb.tarul.cn

[Q08] 创建普通索引
来源：http://dnc.mhx1999.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nbh.yj202588.top

[Q09] 创建唯一索引
来源：http://qmk.sxryk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ohq.ivvv.top

[Q10] 插入单行
来源：http://ioc.jqgfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nkv.svipenyu.cn

[Q11] 一次插入多行
来源：http://oab.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ofv.smart0.xyz

[Q12] 插入后取自增 ID
来源：http://znw.cashguo.top

INSERT INTO users (name) VALUES ('C');
来源：http://jgo.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mak.cheryme.top

[Q13] 忽略重复插入
来源：http://nkw.cashguo.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qxt.jianghu66.top

[Q14] 存在则更新（upsert）
来源：http://wph.jqgufenzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kqn.xuanzx.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rkl.cheryme.top

[Q15] 查询全部
来源：http://vep.fktsv.cn

SELECT * FROM users;
来源：http://xxb.hywenlv.cn

[Q16] 查询指定列
来源：http://xfp.52xcode.cn

SELECT id, name FROM users;
来源：http://gst.gzhubu.top

[Q17] 条件查询
来源：http://edj.redwolf501.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tgt.vehdjk.com

[Q18] 模糊匹配
来源：http://fxo.xinyue.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cex.wangdashe.top

[Q19] 范围查询
来源：http://waj.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tou.wangdashe.top

[Q20] IN 列表
来源：http://mkk.feifeiyinyue.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qfl.hammf.cn

[Q21] 空值判断
来源：http://cff.pengpengdd.cyou

SELECT * FROM users WHERE email IS NULL;
来源：http://rvt.chenzaomai.com

[Q22] 排序
来源：http://sah.hcnkem.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fyi.chenjidiqi.icu

[Q23] 分页
来源：http://srr.feifeiyinyue.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lwk.shuidangran.top

[Q24] 去重
来源：http://ohl.tianlin.xyz

SELECT DISTINCT city FROM users;
来源：http://zmj.cucudq.cn

[Q25] 只取前 N 条
来源：http://ohh.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://djp.vqdsnc.cn

[Q26] 计数
来源：http://wmc.gaohongyu789.top

SELECT COUNT(*) FROM users;
来源：http://osx.nanxinkj.top

[Q27] 条件计数
来源：http://xum.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zen.hysaishi.cn

[Q28] 求和与平均
来源：http://exq.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wpw.fktsv.cn

[Q29] 最大最小值
来源：http://uty.hnqzz.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cjd.yueranfly.top

[Q30] 分组统计
来源：http://sod.tianlin.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://izr.hywenlv.cn

[Q31] 分组后过滤
来源：http://aam.zhengqikj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ygk.birdmap.top

[Q32] 分组拼接字符串
来源：http://uug.cqqwz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://utg.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ptx.cucudq.cn

[Q33] 多列分组
来源：http://dbh.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mfa.wangshuangyany.cn

[Q34] 每组取第一条
来源：http://ska.tianlin.xyz

SELECT * FROM (
来源：http://qhb.hnxiangtu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wld.ybcxt.top

) t WHERE rn = 1;
来源：http://tus.wangshuangyany.cn

[Q35] 内连接
来源：http://sfq.jiagoushi.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wog.ydzc1.top

[Q36] 左连接
来源：http://iit.yfazqb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://awg.tarul.cn

[Q37] 右连接
来源：http://xcn.xuanzx.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://afr.zhengqikj.top

[Q38] 全外连接（PostgreSQL）
来源：http://mga.zdbjq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eak.guowangkeji.top

[Q39] 自连接（查上下级）
来源：http://kac.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wiz.c1oappe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jnf.zdqjudy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wil.9152youxi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eux.zycfv.cn

[Q41] 多表连接
来源：http://yts.tarul.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hdp.xziqi.cn

JOIN users u ON u.id = o.user_id
来源：http://yek.0kj1m.cn

JOIN products p ON p.id = o.product_id;
来源：http://dir.bjfxy.top

[Q42] 连接条件附加过滤
来源：http://cpq.zhiwuduotai.top

SELECT u.name, o.amount FROM users u
来源：http://ayh.snrcjt.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://reb.aibaodan.cn

[Q43] 标量子查询
来源：http://ooq.zdqjudy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://osp.yangfankeji.com

[Q44] IN 子查询
来源：http://tzr.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zgf.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://gko.sysykeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gsw.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://owi.jinqigfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lhv.hnqzz.top

[Q47] 与平均值比较
来源：http://ttd.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rfn.cdnleiting.top

[Q48] CTE 公用表表达式
来源：http://vwy.sjlbkw.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uyg.dashuyun.cn

SELECT * FROM t WHERE c > 5;
来源：http://hhm.birdmap.top

[Q49] 更新单行
来源：http://jut.hcnkem.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tuj.chenzaomai.com

[Q50] 批量更新
来源：http://yxn.cucudq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wxa.pengpengdd.cyou

[Q51] 用子查询更新
来源：http://iiq.jqgfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fzx.smart0.xyz

[Q52] 删除指定行
来源：http://cwq.gotoacloud.top

DELETE FROM users WHERE id = 10;
来源：http://bhr.yvedp.cn

[Q53] 按条件删除
来源：http://xby.nwbrower.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kst.zhengqikj.top

[Q54] 清空表
来源：http://rtv.wangdashe.top

TRUNCATE TABLE logs;
来源：http://vml.gaohongyu789.top

[Q55] 排名（并列占位）
来源：http://tqz.svipenyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hnl.haohaochexian.top

[Q56] 密集排名（并列不占位）
来源：http://bpf.kuanghao11.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xnq.uphjek.com

[Q57] 行号
来源：http://uft.yvedp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nin.chenlongwang.top

[Q58] 累计求和
来源：http://sft.ybcxt.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dkq.jinqigufen.top

[Q59] 分组内累计
来源：http://hnk.zdqjudy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mfu.fanxiaobao.xyz

[Q60] 取上一行 / 下一行
来源：http://cuh.pengpengdd.cyou

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wnh.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hjr.zhaomingkeji.xyz

[Q61] 移动平均
来源：http://ewm.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mxo.hongshengwenyu.top

[Q62] 分组占比
来源：http://kks.andypj.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jvb.yuxming.cn

[Q63] 开启事务
来源：http://bfy.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rme.vehdjk.com

[Q64] 提交事务
来源：http://vzf.fzhhl.top

COMMIT;
来源：http://enx.fehbvm.com

[Q65] 回滚事务
来源：http://jwy.mhx1999.top

ROLLBACK;
来源：http://lql.guowangkeji.top

[Q66] 行锁查询
来源：http://mjh.yonumen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://emj.tanke756.top

[Q67] 设置隔离级别
来源：http://akl.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ilr.tarul.cn

[Q68] 保存点
来源：http://hzv.jinyuanbaomall.cn

SAVEPOINT sp1;
来源：http://dsf.sjlbkw.cn

ROLLBACK TO sp1;
来源：http://sxq.tian-w.cn

[Q69] 查看执行计划
来源：http://hiz.zhixingplan.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://prj.jqgufenzy.top

[Q70] 更新统计信息
来源：http://iuy.zhongyouzk.top

ANALYZE TABLE users;
来源：http://dmm.bjfxy.top

[Q71] 查看建表语句
来源：http://wxt.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lyh.gogol.net.cn

[Q72] 查看索引
来源：http://kfv.daria6918.cn

SHOW INDEX FROM users;
来源：http://qiq.dianchejie.cn

[Q73] 查看表状态
来源：http://ncv.chenzaomai.com

SHOW TABLE STATUS LIKE 'users';
来源：http://cnf.sxryk.cn

[Q74] 强制使用索引
来源：http://qhr.zhijiandao.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nep.shanyushiyangtech.top

[Q75] 日期格式化
来源：http://sej.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ofv.nanxuanxn.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vww.aizwys.cn

[Q76] 按天统计
来源：http://soo.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ioq.snrcjt.cn

[Q77] 时间加减
来源：http://xgi.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://piz.chenlongwang.top

[Q78] 当前时间
来源：http://rzj.fktsv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xaw.yvedp.cn

[Q79] 字符串拼接
来源：http://agi.chenzaomai.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://whs.uphjek.com

[Q80] 字符串截取
来源：http://ked.jinghuilouyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rcb.zhijiandao.cn

[Q81] 字符串替换
来源：http://zst.jinyuanbaomall.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rmk.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://cpx.wangshuangyany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://enk.tanke756.top

[Q83] 大小写转换
来源：http://ijl.0kj1m.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gtz.yvedp.cn

[Q84] 去除首尾空格
来源：http://jkl.zdbjq.cn

SELECT TRIM(name) FROM users;
来源：http://sis.uphjek.com

[Q85] 数值取整
来源：http://kcc.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cjy.cqqwz.cn

[Q86] 读取 JSON 字段
来源：http://odm.sjlbkw.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cfv.guowangkeji.top

[Q87] JSON 字段做条件
来源：http://pra.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nxo.yongpay.top

[Q88] 行转列（条件聚合）
来源：http://qbh.tianlin.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gxi.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://odl.jqgfzy.top

[Q89] 判断表是否存在
来源：http://ljw.sjlbkw.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://slm.sysykeji.top

[Q90] 生成序号列
来源：http://gym.jinghuilouyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qal.zhengqikj.top

================================================================================
来源：http://zye.zycfv.cn

R. Bash 专题
来源：http://lpx.chenjidiqi.icu

================================================================================
来源：http://voe.andypj.xyz

[R01] shebang 与严格模式
来源：http://yjo.zhoulong.xyz

#!/usr/bin/env bash
来源：http://jzy.c1oappe.top

set -euo pipefail
来源：http://zvn.yueranfly.top

[R02] 变量赋值与使用
来源：http://bhj.shanyushiyangtech.top

name="Tom"; echo "$name"
来源：http://idx.xylfe.cn

[R03] 只读变量
来源：http://ayz.haohaochexian.top


<!-- 参考信息 -->