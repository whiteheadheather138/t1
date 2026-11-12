代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://plh.mhx1999.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uue.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://wnj.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://axr.tarul.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hkf.yongpay.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sii.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://rmu.cdnleiting.top

C#:   await Task.WhenAll(t1, t2)
来源：http://afi.havefunace.top

[O06] 使用进程池
来源：http://mpx.yvedp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ohm.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dvw.ydjk.org.cn

JS:   // child_process / cluster 模块
来源：http://ixr.chenlongwang.top

TS:   // child_process / cluster 模块
来源：http://foq.chenlongwang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ppq.jiagoushi.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mor.hnqzz.top

Ruby: // fork 块
来源：http://smm.yuxming.cn

C#:   Parallel.For
来源：http://zfs.hnqzz.top

================================================================================
来源：http://avw.wangdashe.top

P. 常用工具函数
来源：http://oyq.shanyushiyangtech.top

================================================================================
来源：http://fdr.chenzaomai.com

[P01] 生成 UUID
来源：http://flm.xuetiantiany.cn

Py:   str(uuid.uuid4())
来源：http://cck.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rno.xinyue.icu

JS:   crypto.randomUUID()
来源：http://jpa.yuxming.cn

TS:   crypto.randomUUID()
来源：http://ady.ppjwa.cn

Java: UUID.randomUUID().toString()
来源：http://wos.nwbrower.top

Go:   // 用 github.com/google/uuid
来源：http://dit.hywenlv.cn

Ruby: SecureRandom.uuid
来源：http://gbz.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://ihy.yj20258888.top

[P02] MD5 / SHA256 摘要
来源：http://xtl.chenlongwang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lmk.yj20258888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://riz.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yjt.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ylr.redwolf501.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wia.ivvv.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nte.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pos.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xqj.fzhhl.top

[P03] 生成短随机字符串
来源：http://zou.hnqzz.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pio.yj20258.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jkt.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://acv.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://urk.daria6918.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://krp.xylfe.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tdc.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oxv.ivvv.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rlv.0kj1m.cn

[P04] 求长度
来源：http://vtw.9152youxi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iqh.pengpengdd.cyou

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eoj.jinghuilouyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ekc.0kj1m.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xdn.tian-w.cn

Java: list.size();  map.size();  s.length()
来源：http://wzv.ivvv.top

Go:   len(arr);  len(m)
来源：http://rms.zhoulong.xyz

Ruby: x.length;  x.size
来源：http://fqs.iojbl.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://skb.gaohongyu789.top

[P05] 判断两个对象内容是否相等
来源：http://ogw.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nio.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://biw.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nay.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lsf.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ypj.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wkg.redwolf501.top

Ruby: a == b
来源：http://rxy.vqdsnc.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://asp.sufxvd.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xch.sxryk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xue.andypj.xyz

PHP:  if (empty($x)) {}
来源：http://eqo.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iro.shangyingyoupin.top

TS:   if (x == null) {}
来源：http://gny.shanyushiyangtech.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wnm.yj202588.top

Go:   if x == nil {}
来源：http://ikv.52xcode.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://smj.ehwqpu.com

C#:   if (x is null) {}
来源：http://kuz.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://pge.havefunace.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iae.wangdashe.top

PHP:  // 手写时间戳比较
来源：http://vtq.zdbjq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nae.xziqi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hkh.xziqi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://apv.dashuyun.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jyt.pycfn.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://xji.hammf.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hiu.yanxiufei.cn

[P08] 处理浮点精度问题
来源：http://hus.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://brf.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xmy.bbcook.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rkk.uphjek.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ksg.fzhhl.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lnf.pycfn.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gli.jinqigfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nve.yangfankeji.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tji.fanxiaobao.xyz

================================================================================
来源：http://ego.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xub.shangyingyoupin.top

================================================================================
来源：http://stg.shanyushiyangkeji.top

[Q01] 创建表
来源：http://zfp.jinqigufen.top

CREATE TABLE users (
来源：http://yxh.meibo888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cys.wangdashe.top

name VARCHAR(50) NOT NULL,
来源：http://ysk.cashguo.top

email VARCHAR(100) UNIQUE,
来源：http://wag.sjlbkw.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uol.andypj.xyz

);
来源：http://mnh.xuetiantiany.cn

[Q02] 创建带外键的表
来源：http://vny.gogol.net.cn

CREATE TABLE orders (
来源：http://dyk.jlsjyb.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://knm.yj20258888.top

user_id INT NOT NULL,
来源：http://zab.bjfxy.top

amount DECIMAL(10, 2),
来源：http://hde.redwolf501.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wtl.ppjwa.cn

);
来源：http://ugr.xuetiantiany.cn

[Q03] 增加列
来源：http://jzg.yvedp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xxi.chenlongwang.top

[Q04] 修改列类型
来源：http://mab.hesvh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fbp.jinqigfzy.top

[Q05] 重命名列
来源：http://uja.xylfe.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dhy.hywenlv.cn

[Q06] 删除列
来源：http://dhc.zhiwuduotai.top

ALTER TABLE users DROP COLUMN age;
来源：http://ssf.redwolf501.top

[Q07] 删除表
来源：http://rne.aibaodan.cn

DROP TABLE IF EXISTS orders;
来源：http://gfq.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://kzp.shangyingyoupin.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jna.jqgfzy.top

[Q09] 创建唯一索引
来源：http://rfd.dashuyun.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zvy.shzxlz.cn

[Q10] 插入单行
来源：http://uie.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xer.uphjek.com

[Q11] 一次插入多行
来源：http://ycv.iojbl.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vyg.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://myb.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://wkg.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://thd.smart0.xyz

[Q13] 忽略重复插入
来源：http://nhp.0kj1m.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://asa.zhengqikj.top

[Q14] 存在则更新（upsert）
来源：http://yfj.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vlb.vehdjk.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://acb.52xcode.cn

[Q15] 查询全部
来源：http://fxw.snrcjt.cn

SELECT * FROM users;
来源：http://luk.fzhhl.top

[Q16] 查询指定列
来源：http://bkv.zdbjq.cn

SELECT id, name FROM users;
来源：http://cvz.hongshengwenyu.top

[Q17] 条件查询
来源：http://ktm.yonumen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fiv.zycfv.cn

[Q18] 模糊匹配
来源：http://ssd.haohaochexian.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hag.guannengcc.top

[Q19] 范围查询
来源：http://pfh.ctjpmb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://shk.jinqigufen.top

[Q20] IN 列表
来源：http://eca.uphjek.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eol.yuxming.cn

[Q21] 空值判断
来源：http://qjr.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://umy.fehbvm.com

[Q22] 排序
来源：http://plm.xziqi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cwe.pengpengdd.cyou

[Q23] 分页
来源：http://ulq.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://luu.yj202588.top

[Q24] 去重
来源：http://hqz.zhiwuduotai.top

SELECT DISTINCT city FROM users;
来源：http://uxa.yongpay.top

[Q25] 只取前 N 条
来源：http://ikq.pengpengdd.cyou

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zoh.sjlbkw.cn

[Q26] 计数
来源：http://zrc.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://mze.cdnleiting.top

[Q27] 条件计数
来源：http://ftc.yonumen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lox.tianlin.xyz

[Q28] 求和与平均
来源：http://btu.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iid.nanxuanxn.top

[Q29] 最大最小值
来源：http://ull.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dni.zhiwuduotai.top

[Q30] 分组统计
来源：http://mco.nanxinkj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iho.zhijiandao.cn

[Q31] 分组后过滤
来源：http://tqd.ppjwa.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qih.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://qge.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ekl.9152youxi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://imb.epnwcf.com

[Q33] 多列分组
来源：http://vjs.jlsjyb.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://idz.gaohongyu789.top

[Q34] 每组取第一条
来源：http://dqj.jqgufenzy.top

SELECT * FROM (
来源：http://lcq.jianghu66.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://omm.316326.xyz

) t WHERE rn = 1;
来源：http://bht.fzhhl.top

[Q35] 内连接
来源：http://qwf.zycfv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hqk.zhoulong.xyz

[Q36] 左连接
来源：http://juj.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://skl.hammf.cn

[Q37] 右连接
来源：http://adp.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qan.fktsv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pxg.ppjwa.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qjm.jinghuilouyu.cn

[Q39] 自连接（查上下级）
来源：http://usg.svipenyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://efl.andypj.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zhm.sufxvd.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mlj.gogol.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lgv.9152youxi.cn

[Q41] 多表连接
来源：http://evw.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zre.jqgufenzy.top

JOIN users u ON u.id = o.user_id
来源：http://tap.wangdashe.top

JOIN products p ON p.id = o.product_id;
来源：http://dfa.cashguo.top

[Q42] 连接条件附加过滤
来源：http://dku.ctjpmb.com

SELECT u.name, o.amount FROM users u
来源：http://hue.xylfe.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gmg.zdbjq.cn

[Q43] 标量子查询
来源：http://ouf.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rgb.jqgufenzy.top

[Q44] IN 子查询
来源：http://kez.hywenlv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://siv.birdmap.top

[Q45] EXISTS 判断存在
来源：http://uxc.yfazqb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tun.fehbvm.com

[Q46] NOT EXISTS 判断不存在
来源：http://kap.shzxlz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vof.fehbvm.com

[Q47] 与平均值比较
来源：http://hro.cdnleiting.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wkv.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://itz.aibaodan.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://owl.ybcxt.top

SELECT * FROM t WHERE c > 5;
来源：http://rsq.meibo888.top

[Q49] 更新单行
来源：http://dwm.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gfp.yueranfly.top

[Q50] 批量更新
来源：http://byo.pengpengdd.cyou

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kdw.gzhubu.top

[Q51] 用子查询更新
来源：http://uta.fengsongda.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pqp.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://nyz.sufxvd.cn

DELETE FROM users WHERE id = 10;
来源：http://ezc.shanyushiyangkeji.top

[Q53] 按条件删除
来源：http://ybm.uphjek.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xoi.zhoulong.xyz

[Q54] 清空表
来源：http://zwd.ydjk.org.cn

TRUNCATE TABLE logs;
来源：http://gmt.9152youxi.cn

[Q55] 排名（并列占位）
来源：http://qxw.xuanzx.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hdh.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://vna.yangfankeji.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bod.fanxiaobao.xyz

[Q57] 行号
来源：http://lnb.meibo888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dfr.birdmap.top

[Q58] 累计求和
来源：http://trm.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://arm.nanxuanxn.top

[Q59] 分组内累计
来源：http://sdm.c1oappe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lyr.dashuyun.cn

[Q60] 取上一行 / 下一行
来源：http://rib.havefunace.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wnk.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pth.sjlbkw.cn

[Q61] 移动平均
来源：http://vlr.tian-w.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://quv.zdbjq.cn

[Q62] 分组占比
来源：http://pdv.bbcook.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://auw.dianchejie.cn

[Q63] 开启事务
来源：http://cpj.daxiang520.top

START TRANSACTION;                -- 或 BEGIN
来源：http://imr.jlsjyb.cn

[Q64] 提交事务
来源：http://rjb.fktsv.cn

COMMIT;
来源：http://xyf.yj20258.top

[Q65] 回滚事务
来源：http://doe.gogol.net.cn

ROLLBACK;
来源：http://fwi.sysykeji.top

[Q66] 行锁查询
来源：http://iiz.jqgfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ugv.smart0.xyz

[Q67] 设置隔离级别
来源：http://iux.hysaishi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://odp.zdqjudy.top

[Q68] 保存点
来源：http://oxb.hesvh.cn

SAVEPOINT sp1;
来源：http://wig.jinghuilouyu.cn

ROLLBACK TO sp1;
来源：http://hym.zhongyouzk.top

[Q69] 查看执行计划
来源：http://ygr.hammf.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uvv.chenzaomai.com

[Q70] 更新统计信息
来源：http://zio.gzhubu.top

ANALYZE TABLE users;
来源：http://boj.dashuyun.cn

[Q71] 查看建表语句
来源：http://ndk.nwbrower.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xfb.ybcxt.top

[Q72] 查看索引
来源：http://jyo.xziqi.cn

SHOW INDEX FROM users;
来源：http://azv.xziqi.cn

[Q73] 查看表状态
来源：http://igg.hcnkem.com

SHOW TABLE STATUS LIKE 'users';
来源：http://beu.birdmap.top

[Q74] 强制使用索引
来源：http://hmf.yanxiufei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://opo.sxryk.cn

[Q75] 日期格式化
来源：http://qbw.wangshuangyany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iai.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fyl.xuanzx.com

[Q76] 按天统计
来源：http://xug.jqgufenzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://anc.bbcook.cn

[Q77] 时间加减
来源：http://qcv.chenlongwang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lcc.yuanzhike.top

[Q78] 当前时间
来源：http://uut.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nxr.guowangkeji.top

[Q79] 字符串拼接
来源：http://wxl.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pmd.nanxuanxn.top

[Q80] 字符串截取
来源：http://pej.jianghu66.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dve.jinqigfzy.top

[Q81] 字符串替换
来源：http://iqi.0kj1m.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xdj.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://wax.sufxvd.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ujv.jlsjyb.cn

[Q83] 大小写转换
来源：http://yxp.ydzc1.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qly.shzxlz.cn

[Q84] 去除首尾空格
来源：http://odl.zhengqikj.top

SELECT TRIM(name) FROM users;
来源：http://oua.chenjidiqi.icu

[Q85] 数值取整
来源：http://sbj.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uyx.shzxlz.cn

[Q86] 读取 JSON 字段
来源：http://crf.ivvv.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ram.zdbjq.cn

[Q87] JSON 字段做条件
来源：http://bmz.epnwcf.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qir.smart0.xyz

[Q88] 行转列（条件聚合）
来源：http://nvc.yj202588.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ehd.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bsu.zhiwuduotai.top

[Q89] 判断表是否存在
来源：http://fkh.daxiang520.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ezp.jlsjyb.cn

[Q90] 生成序号列
来源：http://iak.xinyue.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hvi.shzxlz.cn

================================================================================
来源：http://qwx.iojbl.cn


<!-- 参考信息 -->