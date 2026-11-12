代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zom.ivvv.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://slz.birdmap.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ppm.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://alz.xinyue.icu

================================================================================
来源：http://lfp.smart0.xyz

O. 并发与异步
来源：http://yic.yueranfly.top

================================================================================
来源：http://hqv.dashuyun.cn

[O01] 启动一个线程
来源：http://fty.c1oappe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wil.yonumen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vny.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nkn.shanyushiyangtech.top

TS:   // 同 JS
来源：http://lap.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://fbx.meibo888.top

Go:   go f()
来源：http://ixj.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://yln.hammf.cn

C#:   Task.Run(() => F());
来源：http://hey.guannengcc.top

[O02] 使用线程池
来源：http://giy.yj20258.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bqa.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kwm.gzhubu.top

JS:   // worker_threads 线程池
来源：http://sdn.jianghu66.top

TS:   // worker_threads 线程池
来源：http://mpb.quarkkingdee.top

Java: Executors.newFixedThreadPool(4)
来源：http://dot.cqqwz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nll.havefunace.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mlu.gzhubu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hoe.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://mez.gaohongyu789.top

Py:   with lock: shared += 1
来源：http://bbo.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://pxj.ywan-chungtsiang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ldo.gzhubu.top

TS:   // 同 JS
来源：http://hgz.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://tgd.gzhubu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rrz.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rim.316326.xyz

C#:   lock (gate) { shared++; }
来源：http://ekw.hnqzz.top

[O04] 定义异步函数并等待
来源：http://emj.yj20258.top

Py:   async def f():⏎    await g()
来源：http://wil.xinyue.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jlq.zycfv.cn

JS:   async function f() { await g(); }
来源：http://oua.daria6918.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://png.guannengcc.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bzd.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://muc.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://xva.bjfxy.top

C#:   async Task F() { await G(); }
来源：http://muk.daria6918.cn

[O05] 并发执行并等待全部完成
来源：http://xfj.hnqzz.top

Py:   asyncio.gather(*tasks)
来源：http://zfm.zhongyouzk.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ouy.andypj.xyz

JS:   await Promise.all(tasks)
来源：http://bkc.cashguo.top

TS:   await Promise.all(tasks)
来源：http://nnd.gzhubu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kmi.bbcook.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://anu.sjlbkw.cn

Ruby: threads.map(&:join)
来源：http://saw.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qbk.jinyuanbaomall.cn

[O06] 使用进程池
来源：http://jpf.yangfankeji.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rlp.uphjek.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ekj.jinqigufen.top

JS:   // child_process / cluster 模块
来源：http://btd.shzxlz.cn

TS:   // child_process / cluster 模块
来源：http://ulx.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vhp.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://npb.jianghu66.top

Ruby: // fork 块
来源：http://orj.xinyue.icu

C#:   Parallel.For
来源：http://rsn.andypj.xyz

================================================================================
来源：http://zxi.shanyushiyangtech.top

P. 常用工具函数
来源：http://mle.bbcook.cn

================================================================================
来源：http://zfb.iojbl.cn

[P01] 生成 UUID
来源：http://vcu.gaohongyu789.top

Py:   str(uuid.uuid4())
来源：http://ham.hnqzz.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xsc.snrcjt.cn

JS:   crypto.randomUUID()
来源：http://ppd.pengpengdd.cyou

TS:   crypto.randomUUID()
来源：http://mqt.sysykeji.top

Java: UUID.randomUUID().toString()
来源：http://ieo.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://cci.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://hld.yueranfly.top

C#:   Guid.NewGuid().ToString()
来源：http://dfq.cqqwz.cn

[P02] MD5 / SHA256 摘要
来源：http://crs.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nrt.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yxg.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oqv.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vgc.shuidangran.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xhq.vqdsnc.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://snl.aibaodan.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pqj.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zuu.yonumen.top

[P03] 生成短随机字符串
来源：http://buj.shzxlz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://asq.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gen.zdbjq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dbm.havefunace.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yqy.ehwqpu.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dwz.yuanzhike.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pov.gaohongyu789.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wdp.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eqh.cashguo.top

[P04] 求长度
来源：http://qse.hesvh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fyy.yuxming.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://amm.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sab.tarul.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zmf.yj20258888.top

Java: list.size();  map.size();  s.length()
来源：http://rtm.hammf.cn

Go:   len(arr);  len(m)
来源：http://ipm.fanxiaobao.xyz

Ruby: x.length;  x.size
来源：http://ust.0kj1m.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tml.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://rcu.snrcjt.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qns.chenlongwang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tdz.yanxiufei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xwv.yj202588.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://woh.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://psy.ehwqpu.com

Go:   reflect.DeepEqual(a, b)
来源：http://eev.ivvv.top

Ruby: a == b
来源：http://vlu.daxiang520.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yvj.yfazqb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hbs.gogol.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jhg.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://qwk.jqgufenzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kig.jinghuilouyu.cn

TS:   if (x == null) {}
来源：http://yho.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mev.snrcjt.cn

Go:   if x == nil {}
来源：http://mtz.shangyingyoupin.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fqv.zhijiandao.cn

C#:   if (x is null) {}
来源：http://ycp.yj202588.top

[P07] 防抖与节流
来源：http://wen.vqdsnc.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://syp.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://byb.cqqwz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nwn.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ubk.zdbjq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vjq.daria6918.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://csf.ppjwa.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zer.jiagoushi.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xpi.pycfn.com

[P08] 处理浮点精度问题
来源：http://qow.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sia.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hgo.cashguo.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://czy.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aoa.tian-w.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yan.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://erm.shangyingyoupin.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lqv.daxiang520.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ndm.zdqjudy.top

================================================================================
来源：http://unc.jinqigufen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uvo.pengpengdd.cyou

================================================================================
来源：http://kdg.yueranfly.top

[Q01] 创建表
来源：http://mli.zhijiandao.cn

CREATE TABLE users (
来源：http://jsj.chenzaomai.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://das.guannengcc.top

name VARCHAR(50) NOT NULL,
来源：http://fyw.yj202588.top

email VARCHAR(100) UNIQUE,
来源：http://kbg.ydjk.org.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rcq.xinyue.icu

);
来源：http://qwy.yuanzhike.top

[Q02] 创建带外键的表
来源：http://omi.tanke756.top

CREATE TABLE orders (
来源：http://qme.cdnleiting.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lbn.sjlbkw.cn

user_id INT NOT NULL,
来源：http://xgn.shanyushiyangkeji.top

amount DECIMAL(10, 2),
来源：http://zdf.xylfe.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hla.ywan-chungtsiang.top

);
来源：http://kow.pengpengdd.cyou

[Q03] 增加列
来源：http://nee.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lee.ybcxt.top

[Q04] 修改列类型
来源：http://mqk.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ncr.meibo888.top

[Q05] 重命名列
来源：http://hko.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hov.hnxiangtu.top

[Q06] 删除列
来源：http://ihw.bbcook.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jjr.yanxiufei.cn

[Q07] 删除表
来源：http://otk.guannengcc.top

DROP TABLE IF EXISTS orders;
来源：http://ian.bjfxy.top

[Q08] 创建普通索引
来源：http://eia.jlsjyb.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://stu.jinqigufen.top

[Q09] 创建唯一索引
来源：http://klm.pycfn.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qns.ehwqpu.com

[Q10] 插入单行
来源：http://eia.hysaishi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://csa.zdqjudy.top

[Q11] 一次插入多行
来源：http://gnl.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jxk.snrcjt.cn

[Q12] 插入后取自增 ID
来源：http://vwd.cqqwz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://niu.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fia.hywenlv.cn

[Q13] 忽略重复插入
来源：http://sdv.jlsjyb.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gzq.birdmap.top

[Q14] 存在则更新（upsert）
来源：http://bpc.sjlbkw.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fnt.ydzc1.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fop.jinqigfzy.top

[Q15] 查询全部
来源：http://itn.jyoumei.cn

SELECT * FROM users;
来源：http://qyo.ydzc1.top

[Q16] 查询指定列
来源：http://qov.jyoumei.cn

SELECT id, name FROM users;
来源：http://udf.mhx1999.top

[Q17] 条件查询
来源：http://ejw.zhixingplan.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gym.zhongyouzk.top

[Q18] 模糊匹配
来源：http://wpy.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://amy.jyoumei.cn

[Q19] 范围查询
来源：http://kox.daxiang520.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://odi.fanxiaobao.xyz

[Q20] IN 列表
来源：http://vmn.bbcook.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ooj.zhixingplan.top

[Q21] 空值判断
来源：http://jwl.shzxlz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fct.0kj1m.cn

[Q22] 排序
来源：http://ctn.svipenyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://via.wangshuangyany.cn

[Q23] 分页
来源：http://suk.c1oappe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wcz.ehwqpu.com

[Q24] 去重
来源：http://cja.jianghu66.top

SELECT DISTINCT city FROM users;
来源：http://shg.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://cwv.shanyushiyangtech.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://btd.yvedp.cn

[Q26] 计数
来源：http://vtp.sysykeji.top

SELECT COUNT(*) FROM users;
来源：http://fuz.bbcook.cn

[Q27] 条件计数
来源：http://oyc.daxiang520.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ean.yuxming.cn

[Q28] 求和与平均
来源：http://gls.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uey.yueranfly.top

[Q29] 最大最小值
来源：http://fdn.yangfankeji.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://lgg.jlsjyb.cn

[Q30] 分组统计
来源：http://uur.shangyingyoupin.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cap.zhijiandao.cn

[Q31] 分组后过滤
来源：http://tnd.yangfankeji.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hzx.chenlongwang.top

[Q32] 分组拼接字符串
来源：http://lmz.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wkn.aibaodan.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lkh.52xcode.cn

[Q33] 多列分组
来源：http://bhn.dashuyun.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yna.sxryk.cn

[Q34] 每组取第一条
来源：http://ofg.cheryme.top

SELECT * FROM (
来源：http://evs.jinqigufen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mak.yangfankeji.com

) t WHERE rn = 1;
来源：http://clb.vqdsnc.cn

[Q35] 内连接
来源：http://hyb.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gtw.shanyushiyangkeji.top

[Q36] 左连接
来源：http://zts.gogol.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://txf.shzxlz.cn

[Q37] 右连接
来源：http://ool.hnxiangtu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baq.hysaishi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pfz.nanxinkj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mzp.tanke756.top

[Q39] 自连接（查上下级）
来源：http://hyx.jqgfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wsu.xziqi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sip.hnqzz.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hmk.tanke756.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cbu.jqgfzy.top

[Q41] 多表连接
来源：http://atv.xuanzx.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://wcs.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://prr.chenlongwang.top

JOIN products p ON p.id = o.product_id;
来源：http://toj.dianchejie.cn

[Q42] 连接条件附加过滤
来源：http://yqi.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://qqi.sufxvd.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sra.zhengqikj.top

[Q43] 标量子查询
来源：http://zta.jinqigfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zdl.shanyushiyangtech.top

[Q44] IN 子查询
来源：http://tul.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vxt.xinyue.icu

[Q45] EXISTS 判断存在
来源：http://zvy.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wjl.dianchejie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jjj.hammf.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mnb.gzhubu.top

[Q47] 与平均值比较
来源：http://jxj.birdmap.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://syl.zhijiandao.cn

[Q48] CTE 公用表表达式
来源：http://ffn.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dtn.c1oappe.top

SELECT * FROM t WHERE c > 5;
来源：http://mxi.xuetiantiany.cn

[Q49] 更新单行
来源：http://rav.dashuyun.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mjd.uphjek.com

[Q50] 批量更新
来源：http://jgr.jinqigufen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fux.svipenyu.cn

[Q51] 用子查询更新
来源：http://abn.jinqigfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jng.yuxming.cn

[Q52] 删除指定行
来源：http://pbx.wangdashe.top

DELETE FROM users WHERE id = 10;
来源：http://uuk.vehdjk.com

[Q53] 按条件删除
来源：http://lnf.fzhhl.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lmh.ydzc1.top

[Q54] 清空表
来源：http://zyf.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://vim.zdqjudy.top

[Q55] 排名（并列占位）
来源：http://hvx.sjlbkw.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kue.yj202588.top

[Q56] 密集排名（并列不占位）
来源：http://ltr.cheryme.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yvc.nanxinkj.top

[Q57] 行号
来源：http://tzj.shuidangran.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://inn.daria6918.cn

[Q58] 累计求和
来源：http://nnf.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eex.0kj1m.cn

[Q59] 分组内累计
来源：http://yej.yj202588.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tll.feifeiyinyue.top

[Q60] 取上一行 / 下一行
来源：http://smf.feifeiyinyue.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cfe.jinyuanbaomall.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tnu.gaohongyu789.top

[Q61] 移动平均
来源：http://rif.haohaochexian.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tqy.yonumen.top

[Q62] 分组占比
来源：http://fig.ydzc1.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://luq.aizwys.cn

[Q63] 开启事务
来源：http://ngu.xuanzx.com

START TRANSACTION;                -- 或 BEGIN
来源：http://oko.yfazqb.com

[Q64] 提交事务
来源：http://mim.zhijiandao.cn

COMMIT;
来源：http://kkh.hammf.cn

[Q65] 回滚事务
来源：http://pyn.hongshengwenyu.top

ROLLBACK;
来源：http://bfk.kuanghao11.cn

[Q66] 行锁查询
来源：http://vui.nanxuanxn.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kbm.shzxlz.cn

[Q67] 设置隔离级别
来源：http://ljv.zhongyouzk.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lqz.aizwys.cn

[Q68] 保存点
来源：http://jcq.xingfuxueyuan.xyz

SAVEPOINT sp1;
来源：http://has.xziqi.cn

ROLLBACK TO sp1;
来源：http://mnn.havefunace.top

[Q69] 查看执行计划
来源：http://fbn.nanxinkj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wbw.chenlongwang.top

[Q70] 更新统计信息
来源：http://sft.hfpthk.cn


<!-- 参考信息 -->