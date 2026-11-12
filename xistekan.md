代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://ksk.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://fjy.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://jgp.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://ukx.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uts.yanxiufei.cn

JS:   async function f() { await g(); }
来源：http://fak.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ypr.gzhubu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gbb.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tvk.tianlin.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ulk.sxryk.cn

C#:   async Task F() { await G(); }
来源：http://fnn.316326.xyz

[O05] 并发执行并等待全部完成
来源：http://lwp.andypj.xyz

Py:   asyncio.gather(*tasks)
来源：http://omd.chenlongwang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://osu.xuanzx.com

JS:   await Promise.all(tasks)
来源：http://cyd.ydjk.org.cn

TS:   await Promise.all(tasks)
来源：http://ryn.fanxiaobao.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pcm.zdbjq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://acm.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://ich.fzhhl.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fqt.smart0.xyz

[O06] 使用进程池
来源：http://dhc.fktsv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sgg.mhx1999.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ssg.shuidangran.top

JS:   // child_process / cluster 模块
来源：http://fym.uphjek.com

TS:   // child_process / cluster 模块
来源：http://vlj.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://aem.316326.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vyf.fzhhl.top

Ruby: // fork 块
来源：http://uyd.sweek.top

C#:   Parallel.For
来源：http://tgb.iojbl.cn

================================================================================
来源：http://jih.sysykeji.top

P. 常用工具函数
来源：http://qhf.quarkkingdee.top

================================================================================
来源：http://cym.gaohongyu789.top

[P01] 生成 UUID
来源：http://atk.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://ebg.dianchejie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kon.yangfankeji.com

JS:   crypto.randomUUID()
来源：http://sdn.hcnkem.com

TS:   crypto.randomUUID()
来源：http://onb.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://wqv.zdqjudy.top

Go:   // 用 github.com/google/uuid
来源：http://kxb.meibo888.top

Ruby: SecureRandom.uuid
来源：http://trb.shuidangran.top

C#:   Guid.NewGuid().ToString()
来源：http://thx.0kj1m.cn

[P02] MD5 / SHA256 摘要
来源：http://goh.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oqo.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pkp.meibo888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mjq.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vkh.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dtz.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zoq.tianlin.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fph.fzhhl.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hde.birdmap.top

[P03] 生成短随机字符串
来源：http://vrv.yangfankeji.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iok.vqdsnc.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xgb.uphjek.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rhd.fzhhl.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xyl.hnqzz.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hor.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kwp.daxiang520.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://oah.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fmx.ydjk.org.cn

[P04] 求长度
来源：http://lxf.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dja.jiagoushi.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ssr.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eqo.zdqjudy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ach.haohaochexian.top

Java: list.size();  map.size();  s.length()
来源：http://zke.uphjek.com

Go:   len(arr);  len(m)
来源：http://xcj.havefunace.top

Ruby: x.length;  x.size
来源：http://hhr.havefunace.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://sxz.fehbvm.com

[P05] 判断两个对象内容是否相等
来源：http://dcd.daxiang520.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kkc.yfazqb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tqw.tianlin.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bcn.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nag.jqgfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vpg.zhoulong.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://lah.hcnkem.com

Ruby: a == b
来源：http://ztq.nanxinkj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cft.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wcf.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tdm.gzhubu.top

PHP:  if (empty($x)) {}
来源：http://jol.daxiang520.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aeo.quarkkingdee.top

TS:   if (x == null) {}
来源：http://dnq.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ccx.9152youxi.cn

Go:   if x == nil {}
来源：http://vat.316326.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nhn.ywan-chungtsiang.top

C#:   if (x is null) {}
来源：http://brl.xziqi.cn

[P07] 防抖与节流
来源：http://rpy.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ukx.c1oappe.top

PHP:  // 手写时间戳比较
来源：http://eid.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ewg.cheryme.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yjl.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hjl.gotoacloud.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tfx.yj20258888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://eht.hnxiangtu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bwh.smart0.xyz

[P08] 处理浮点精度问题
来源：http://wnw.ybcxt.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aui.gogol.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fje.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gcc.tanke756.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oae.ctjpmb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://puf.fktsv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hhk.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dsy.uphjek.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kci.fktsv.cn

================================================================================
来源：http://qva.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://peo.daria6918.cn

================================================================================
来源：http://phc.hysaishi.cn

[Q01] 创建表
来源：http://sdz.fengsongda.top

CREATE TABLE users (
来源：http://tud.zdqjudy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cat.uphjek.com

name VARCHAR(50) NOT NULL,
来源：http://czz.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://npp.zhongyouzk.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hjc.zdbjq.cn

);
来源：http://lgf.xziqi.cn

[Q02] 创建带外键的表
来源：http://ivv.hysaishi.cn

CREATE TABLE orders (
来源：http://kbh.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://arn.jlsjyb.cn

user_id INT NOT NULL,
来源：http://msu.meibo888.top

amount DECIMAL(10, 2),
来源：http://ubz.jqgufenzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yuk.wangshuangyany.cn

);
来源：http://keo.aibaodan.cn

[Q03] 增加列
来源：http://iyj.ydjk.org.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xoo.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://ykt.redwolf501.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nac.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://anc.hnqzz.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xit.vqdsnc.cn

[Q06] 删除列
来源：http://zxt.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://lke.hysaishi.cn

[Q07] 删除表
来源：http://tqi.ybcxt.top

DROP TABLE IF EXISTS orders;
来源：http://mbe.zdqjudy.top

[Q08] 创建普通索引
来源：http://cbo.vehdjk.com

CREATE INDEX idx_users_email ON users(email);
来源：http://xtv.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://ryg.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gkd.yvedp.cn

[Q10] 插入单行
来源：http://ckm.gogol.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mmg.chenlongwang.top

[Q11] 一次插入多行
来源：http://tro.hysaishi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://srn.nanxinkj.top

[Q12] 插入后取自增 ID
来源：http://ywl.yueranfly.top

INSERT INTO users (name) VALUES ('C');
来源：http://wyl.bjfxy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vry.0kj1m.cn

[Q13] 忽略重复插入
来源：http://mbm.shzxlz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dtr.fanxiaobao.xyz

[Q14] 存在则更新（upsert）
来源：http://tur.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pap.uphjek.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ztz.jqgufenzy.top

[Q15] 查询全部
来源：http://peg.dashuyun.cn

SELECT * FROM users;
来源：http://jmm.hammf.cn

[Q16] 查询指定列
来源：http://der.ivvv.top

SELECT id, name FROM users;
来源：http://kfg.xuanzx.com

[Q17] 条件查询
来源：http://yhg.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dhc.hysaishi.cn

[Q18] 模糊匹配
来源：http://esf.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vvc.sysykeji.top

[Q19] 范围查询
来源：http://ega.tian-w.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bqb.kuanghao11.cn

[Q20] IN 列表
来源：http://nuv.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zwc.iojbl.cn

[Q21] 空值判断
来源：http://hjz.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mzq.hnxiangtu.top

[Q22] 排序
来源：http://gee.tanke756.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vzd.gotoacloud.top

[Q23] 分页
来源：http://fxi.wangdashe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vsa.tian-w.cn

[Q24] 去重
来源：http://wen.bbcook.cn

SELECT DISTINCT city FROM users;
来源：http://bbq.smart0.xyz

[Q25] 只取前 N 条
来源：http://ead.svipenyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yct.ydjk.org.cn

[Q26] 计数
来源：http://pxd.quarkkingdee.top

SELECT COUNT(*) FROM users;
来源：http://wql.dashuyun.cn

[Q27] 条件计数
来源：http://lrv.uphjek.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://clf.sufxvd.cn

[Q28] 求和与平均
来源：http://zua.cheryme.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kmp.jianghu66.top

[Q29] 最大最小值
来源：http://tno.316326.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://gnv.havefunace.top

[Q30] 分组统计
来源：http://ijv.nanxuanxn.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://naw.cqqwz.cn

[Q31] 分组后过滤
来源：http://vaf.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lvp.nwbrower.top

[Q32] 分组拼接字符串
来源：http://xqg.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hpz.xylfe.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jig.guowangkeji.top

[Q33] 多列分组
来源：http://mvf.shuidangran.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jsz.jianghu66.top

[Q34] 每组取第一条
来源：http://ghz.52xcode.cn

SELECT * FROM (
来源：http://lel.zdbjq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://unf.wangshuangyany.cn

) t WHERE rn = 1;
来源：http://bai.pycfn.com

[Q35] 内连接
来源：http://mhd.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xdc.hywenlv.cn

[Q36] 左连接
来源：http://tph.ehwqpu.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fsb.zhoulong.xyz

[Q37] 右连接
来源：http://pdu.zhoulong.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fxi.fanxiaobao.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://pwh.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eiy.jqgufenzy.top

[Q39] 自连接（查上下级）
来源：http://msu.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qxs.jinyuanbaomall.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iqj.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jet.hammf.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rqj.jianghu66.top

[Q41] 多表连接
来源：http://nwk.xinyue.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://xrc.sufxvd.cn

JOIN users u ON u.id = o.user_id
来源：http://hzm.cheryme.top

JOIN products p ON p.id = o.product_id;
来源：http://qxs.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://yql.sweek.top

SELECT u.name, o.amount FROM users u
来源：http://yng.tarul.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jcc.tanke756.top

[Q43] 标量子查询
来源：http://hzw.hysaishi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://udp.sweek.top

[Q44] IN 子查询
来源：http://dfl.chenlongwang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wee.sweek.top

[Q45] EXISTS 判断存在
来源：http://bus.zhengqikj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ntn.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wlr.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ill.yueranfly.top

[Q47] 与平均值比较
来源：http://vse.gogol.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gas.nanxinkj.top

[Q48] CTE 公用表表达式
来源：http://hah.sysykeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fqr.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://nvb.haohaochexian.top

[Q49] 更新单行
来源：http://ipt.cqqwz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://syt.ydzc1.top

[Q50] 批量更新
来源：http://dar.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eqa.hnqzz.top

[Q51] 用子查询更新
来源：http://lri.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oop.cheryme.top

[Q52] 删除指定行
来源：http://jly.jinghuilouyu.cn

DELETE FROM users WHERE id = 10;
来源：http://eeh.shanyushiyangkeji.top

[Q53] 按条件删除
来源：http://gkp.yueranfly.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wvk.cheryme.top

[Q54] 清空表
来源：http://vbc.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://xse.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://bfv.ydjk.org.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sli.yj20258.top

[Q56] 密集排名（并列不占位）
来源：http://vvt.havefunace.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cjz.snrcjt.cn

[Q57] 行号
来源：http://opf.redwolf501.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mjv.hnxiangtu.top

[Q58] 累计求和
来源：http://wkc.wangshuangyany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jdr.dianchejie.cn

[Q59] 分组内累计
来源：http://qlw.havefunace.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kfl.vehdjk.com

[Q60] 取上一行 / 下一行
来源：http://fly.gogol.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eil.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://why.havefunace.top

[Q61] 移动平均
来源：http://fbs.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fbk.hnqzz.top

[Q62] 分组占比
来源：http://qwp.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wib.yfazqb.com

[Q63] 开启事务
来源：http://dfm.daria6918.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ffp.jinghuilouyu.cn

[Q64] 提交事务
来源：http://nib.tanke756.top

COMMIT;
来源：http://nrm.fktsv.cn

[Q65] 回滚事务
来源：http://xst.redwolf501.top

ROLLBACK;
来源：http://cln.yongpay.top

[Q66] 行锁查询
来源：http://gsf.sjlbkw.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ezf.jlsjyb.cn

[Q67] 设置隔离级别
来源：http://gcw.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://evv.yangfankeji.com

[Q68] 保存点
来源：http://osj.smart0.xyz

SAVEPOINT sp1;
来源：http://qpf.chenzaomai.com

ROLLBACK TO sp1;
来源：http://voj.dianchejie.cn

[Q69] 查看执行计划
来源：http://uqv.guowangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nfw.jinyuanbaomall.cn

[Q70] 更新统计信息
来源：http://bzr.fzhhl.top

ANALYZE TABLE users;
来源：http://tas.hongshengwenyu.top

[Q71] 查看建表语句
来源：http://rqu.xylfe.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qya.hnxiangtu.top

[Q72] 查看索引
来源：http://ffc.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://stf.xinyue.icu

[Q73] 查看表状态
来源：http://iyc.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://juj.ctjpmb.com

[Q74] 强制使用索引
来源：http://ydt.dianchejie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dqy.aibaodan.cn

[Q75] 日期格式化
来源：http://zqv.kuanghao11.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fcu.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fcq.ehwqpu.com

[Q76] 按天统计
来源：http://ftx.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rgh.ctjpmb.com

[Q77] 时间加减
来源：http://lkh.zhaomingkeji.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://she.redwolf501.top

[Q78] 当前时间
来源：http://utr.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cvq.guowangkeji.top

[Q79] 字符串拼接
来源：http://fvp.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pwn.gzhubu.top

[Q80] 字符串截取
来源：http://xzv.316326.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tmu.feifeiyinyue.top

[Q81] 字符串替换
来源：http://jkh.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://she.fengsongda.top

[Q82] 字符长度与字节长度
来源：http://hir.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uqg.smart0.xyz

[Q83] 大小写转换
来源：http://mrb.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ruz.hnxiangtu.top

[Q84] 去除首尾空格
来源：http://wxf.gaohongyu789.top

SELECT TRIM(name) FROM users;
来源：http://lam.fehbvm.com

[Q85] 数值取整
来源：http://edh.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ipn.xinyue.icu


<!-- 参考信息 -->