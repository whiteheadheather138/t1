代发 wailian999

[O02] 使用线程池
来源：http://wdp.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oft.havefunace.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ylt.mhx1999.top

JS:   // worker_threads 线程池
来源：http://ssp.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://iyf.yj20258888.top

Java: Executors.newFixedThreadPool(4)
来源：http://zbb.hywenlv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://akf.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vxp.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eas.yangfankeji.com

[O03] 加锁保护共享数据
来源：http://pmb.tanke756.top

Py:   with lock: shared += 1
来源：http://yld.tanke756.top

PHP:  // 用 flock() 做文件锁
来源：http://dda.yongpay.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kcs.snrcjt.cn

TS:   // 同 JS
来源：http://efg.gogol.net.cn

Java: synchronized (this) { shared++; }
来源：http://ayq.ivvv.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yqk.smart0.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://uug.dianchejie.cn

C#:   lock (gate) { shared++; }
来源：http://hlh.yj202588.top

[O04] 定义异步函数并等待
来源：http://ejy.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://yyh.shanyushiyangtech.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vay.bbcook.cn

JS:   async function f() { await g(); }
来源：http://gpv.vehdjk.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://gci.zycfv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://irc.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://euw.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tta.sufxvd.cn

C#:   async Task F() { await G(); }
来源：http://wpz.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://nji.sxryk.cn

Py:   asyncio.gather(*tasks)
来源：http://sjo.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bqr.9152youxi.cn

JS:   await Promise.all(tasks)
来源：http://coz.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://hkf.zhengqikj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xzh.tarul.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ogq.hesvh.cn

Ruby: threads.map(&:join)
来源：http://rwd.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://syp.daxiang520.top

[O06] 使用进程池
来源：http://odp.yanxiufei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wqi.cheryme.top

PHP:  // pcntl_fork 或多进程队列
来源：http://lma.smart0.xyz

JS:   // child_process / cluster 模块
来源：http://rwq.hesvh.cn

TS:   // child_process / cluster 模块
来源：http://kxu.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dde.xuetiantiany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ohd.jinqigufen.top

Ruby: // fork 块
来源：http://mov.tarul.cn

C#:   Parallel.For
来源：http://xlp.ehwqpu.com

================================================================================
来源：http://lke.tarul.cn

P. 常用工具函数
来源：http://kbh.nanxuanxn.top

================================================================================
来源：http://cgj.zhiwuduotai.top

[P01] 生成 UUID
来源：http://llr.wangshuangyany.cn

Py:   str(uuid.uuid4())
来源：http://oaz.cucudq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ymn.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://lbo.shuidangran.top

TS:   crypto.randomUUID()
来源：http://gfc.chenlongwang.top

Java: UUID.randomUUID().toString()
来源：http://xhu.shuidangran.top

Go:   // 用 github.com/google/uuid
来源：http://dxr.ivvv.top

Ruby: SecureRandom.uuid
来源：http://kjr.sweek.top

C#:   Guid.NewGuid().ToString()
来源：http://wcx.uphjek.com

[P02] MD5 / SHA256 摘要
来源：http://pfw.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qyc.havefunace.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rsm.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ydp.hesvh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tzo.zhijiandao.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://otq.cucudq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://odl.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://khz.zhijiandao.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gli.zhixingplan.top

[P03] 生成短随机字符串
来源：http://soe.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cnl.fanxiaobao.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gna.zhiwuduotai.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gxi.andypj.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jzg.haohaochexian.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dyu.hnqzz.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nea.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://brf.nwbrower.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lok.cqqwz.cn

[P04] 求长度
来源：http://cus.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wss.vqdsnc.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ves.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iss.yonumen.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xso.daxiang520.top

Java: list.size();  map.size();  s.length()
来源：http://xpg.wangdashe.top

Go:   len(arr);  len(m)
来源：http://iqg.cucudq.cn

Ruby: x.length;  x.size
来源：http://hqr.ppjwa.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lqt.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://joq.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rze.meibo888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gia.aibaodan.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nbi.xingfuxueyuan.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ceh.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xzd.svipenyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wsb.pycfn.com

Ruby: a == b
来源：http://rjt.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pbj.meibo888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fix.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kjy.yuxming.cn

PHP:  if (empty($x)) {}
来源：http://mym.birdmap.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ejm.chenjidiqi.icu

TS:   if (x == null) {}
来源：http://hgk.feifeiyinyue.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yhh.cdnleiting.top

Go:   if x == nil {}
来源：http://jga.52xcode.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ifk.quarkkingdee.top

C#:   if (x is null) {}
来源：http://gcd.gogol.net.cn

[P07] 防抖与节流
来源：http://umn.xingfuxueyuan.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uwy.yj20258.top

PHP:  // 手写时间戳比较
来源：http://nlc.smart0.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://npw.nanxinkj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hxg.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xso.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kdl.xylfe.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lnx.ctjpmb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kgd.dianchejie.cn

[P08] 处理浮点精度问题
来源：http://dzm.xingfuxueyuan.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sut.zycfv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wqp.meibo888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xdj.zdbjq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://erb.nanxuanxn.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lkv.aizwys.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bdj.gaohongyu789.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kgx.hnxiangtu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qnu.cdnleiting.top

================================================================================
来源：http://ory.9152youxi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qyh.52xcode.cn

================================================================================
来源：http://lel.ydzc1.top

[Q01] 创建表
来源：http://bru.cqqwz.cn

CREATE TABLE users (
来源：http://qpz.ppjwa.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tza.xylfe.cn

name VARCHAR(50) NOT NULL,
来源：http://blh.yangfankeji.com

email VARCHAR(100) UNIQUE,
来源：http://yyr.gzhubu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rgh.jinqigufen.top

);
来源：http://bfl.dashuyun.cn

[Q02] 创建带外键的表
来源：http://yik.sxryk.cn

CREATE TABLE orders (
来源：http://qlm.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://afi.yangfankeji.com

user_id INT NOT NULL,
来源：http://qdd.hongshengwenyu.top

amount DECIMAL(10, 2),
来源：http://yoy.vqdsnc.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jxd.cucudq.cn

);
来源：http://kdz.zhixingplan.top

[Q03] 增加列
来源：http://rcp.zycfv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ztm.hammf.cn

[Q04] 修改列类型
来源：http://qeu.cqqwz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ykp.haohaochexian.top

[Q05] 重命名列
来源：http://fbv.ywan-chungtsiang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uan.chenlongwang.top

[Q06] 删除列
来源：http://jvg.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ccc.hysaishi.cn

[Q07] 删除表
来源：http://rmj.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://kff.yvedp.cn

[Q08] 创建普通索引
来源：http://nwj.shanyushiyangtech.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gcr.xylfe.cn

[Q09] 创建唯一索引
来源：http://hcu.wangdashe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uii.havefunace.top

[Q10] 插入单行
来源：http://fpf.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zdp.fehbvm.com

[Q11] 一次插入多行
来源：http://wpx.jinqigufen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ybp.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://now.jlsjyb.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oqn.nanxinkj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eem.nanxinkj.top

[Q13] 忽略重复插入
来源：http://upx.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wma.fanxiaobao.xyz

[Q14] 存在则更新（upsert）
来源：http://zsh.xinyue.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fxr.jiagoushi.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zjt.redwolf501.top

[Q15] 查询全部
来源：http://rir.zhengqikj.top

SELECT * FROM users;
来源：http://nxf.jinqigufen.top

[Q16] 查询指定列
来源：http://nvk.yvedp.cn

SELECT id, name FROM users;
来源：http://upx.chenlongwang.top

[Q17] 条件查询
来源：http://aks.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tdw.xinyue.icu

[Q18] 模糊匹配
来源：http://wbv.sxryk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://aqq.guannengcc.top

[Q19] 范围查询
来源：http://qrj.sysykeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zoz.shzxlz.cn

[Q20] IN 列表
来源：http://pje.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://neu.fanxiaobao.xyz

[Q21] 空值判断
来源：http://fbc.snrcjt.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://oal.yanxiufei.cn

[Q22] 排序
来源：http://htc.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pvf.hongshengwenyu.top

[Q23] 分页
来源：http://btb.hcnkem.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lzv.hesvh.cn

[Q24] 去重
来源：http://zhz.yueranfly.top

SELECT DISTINCT city FROM users;
来源：http://atz.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://jqs.gzhubu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gqd.epnwcf.com

[Q26] 计数
来源：http://gem.chenlongwang.top

SELECT COUNT(*) FROM users;
来源：http://tpz.nwbrower.top

[Q27] 条件计数
来源：http://rmz.haohaochexian.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nvl.gzhubu.top

[Q28] 求和与平均
来源：http://ikl.uphjek.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tcf.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://etu.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vto.hnqzz.top

[Q30] 分组统计
来源：http://swo.fehbvm.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://icy.wangshuangyany.cn

[Q31] 分组后过滤
来源：http://htx.vehdjk.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wje.uphjek.com

[Q32] 分组拼接字符串
来源：http://pqs.sysykeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ryy.ivvv.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://axw.ybcxt.top

[Q33] 多列分组
来源：http://obu.sxryk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hbe.hfpthk.cn

[Q34] 每组取第一条
来源：http://jdk.guannengcc.top

SELECT * FROM (
来源：http://ztw.ppjwa.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gev.jinqigufen.top

) t WHERE rn = 1;
来源：http://pbk.birdmap.top

[Q35] 内连接
来源：http://ovg.zhixingplan.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uiu.haohaochexian.top

[Q36] 左连接
来源：http://dqr.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hbl.shanyushiyangkeji.top

[Q37] 右连接
来源：http://ccd.jinqigufen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cgh.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cqt.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dmn.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://tws.pengpengdd.cyou

SELECT e.name, m.name AS manager FROM employees e
来源：http://yay.yj20258.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ebc.snrcjt.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hyy.316326.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://evh.cashguo.top

[Q41] 多表连接
来源：http://pwn.fengsongda.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://iin.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://igj.jinqigufen.top

JOIN products p ON p.id = o.product_id;
来源：http://ono.fengsongda.top

[Q42] 连接条件附加过滤
来源：http://omx.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://wxv.zhiwuduotai.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qyb.yanxiufei.cn

[Q43] 标量子查询
来源：http://dmg.yangfankeji.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uvk.nwbrower.top

[Q44] IN 子查询
来源：http://alx.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gyf.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://mgd.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bhm.nwbrower.top

[Q46] NOT EXISTS 判断不存在
来源：http://lkq.nanxuanxn.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yxw.cheryme.top

[Q47] 与平均值比较
来源：http://bpo.cheryme.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://usr.hnqzz.top

[Q48] CTE 公用表表达式
来源：http://shr.fehbvm.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nns.fengsongda.top

SELECT * FROM t WHERE c > 5;
来源：http://aie.feifeiyinyue.top

[Q49] 更新单行
来源：http://rnz.zhengqikj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ghn.ydjk.org.cn

[Q50] 批量更新
来源：http://xpd.feifeiyinyue.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sqx.jlsjyb.cn

[Q51] 用子查询更新
来源：http://jus.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uyo.tanke756.top

[Q52] 删除指定行
来源：http://saq.tian-w.cn

DELETE FROM users WHERE id = 10;
来源：http://gsh.gaohongyu789.top

[Q53] 按条件删除
来源：http://wdu.guannengcc.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zcx.yuanzhike.top

[Q54] 清空表
来源：http://rha.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://rfo.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://ofp.smart0.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://piw.zhijiandao.cn

[Q56] 密集排名（并列不占位）
来源：http://qgy.ybcxt.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nhf.epnwcf.com

[Q57] 行号
来源：http://mal.daxiang520.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yen.ivvv.top

[Q58] 累计求和
来源：http://xov.redwolf501.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fwz.9152youxi.cn

[Q59] 分组内累计
来源：http://nsv.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://exu.0kj1m.cn

[Q60] 取上一行 / 下一行
来源：http://lea.c1oappe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pnu.chenlongwang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kqh.guowangkeji.top

[Q61] 移动平均
来源：http://rza.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gnl.yj20258888.top

[Q62] 分组占比
来源：http://uue.sxryk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ili.gogol.net.cn

[Q63] 开启事务
来源：http://cnf.52xcode.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zzt.zdbjq.cn

[Q64] 提交事务
来源：http://eph.aizwys.cn

COMMIT;
来源：http://baz.vehdjk.com

[Q65] 回滚事务
来源：http://ovk.316326.xyz

ROLLBACK;
来源：http://amp.wangdashe.top

[Q66] 行锁查询
来源：http://fxp.vqdsnc.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nrk.jyoumei.cn

[Q67] 设置隔离级别
来源：http://ilq.dashuyun.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hse.chenzaomai.com

[Q68] 保存点
来源：http://uzl.svipenyu.cn

SAVEPOINT sp1;
来源：http://lxz.fehbvm.com

ROLLBACK TO sp1;
来源：http://zrc.shanyushiyangkeji.top

[Q69] 查看执行计划
来源：http://zky.hnxiangtu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fuw.epnwcf.com

[Q70] 更新统计信息
来源：http://krd.ydjk.org.cn

ANALYZE TABLE users;
来源：http://ttr.sxryk.cn

[Q71] 查看建表语句
来源：http://zll.c1oappe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bey.zhengqikj.top

[Q72] 查看索引
来源：http://jan.sjlbkw.cn

SHOW INDEX FROM users;
来源：http://ysb.gogol.net.cn

[Q73] 查看表状态
来源：http://ttj.fzhhl.top

SHOW TABLE STATUS LIKE 'users';
来源：http://hor.daxiang520.top

[Q74] 强制使用索引
来源：http://lfk.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rmn.xuanzx.com

[Q75] 日期格式化
来源：http://xqx.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dnu.snrcjt.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oqu.shanyushiyangkeji.top

[Q76] 按天统计
来源：http://unr.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rel.zycfv.cn

[Q77] 时间加减
来源：http://jjy.snrcjt.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lvf.chenzaomai.com


<!-- 参考信息 -->