代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ywh.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hza.yuanzhike.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gkp.vqdsnc.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mnd.sysykeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mrd.sjlbkw.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qtp.9152youxi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://khj.aibaodan.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nah.fzhhl.top

================================================================================
来源：http://ecg.zhaomingkeji.xyz

O. 并发与异步
来源：http://nkh.yvedp.cn

================================================================================
来源：http://izc.yvedp.cn

[O01] 启动一个线程
来源：http://rma.nanxuanxn.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uck.kuanghao11.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fcg.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pqq.hammf.cn

TS:   // 同 JS
来源：http://ark.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://pjv.yfazqb.com

Go:   go f()
来源：http://obv.ctjpmb.com

Ruby: Thread.new { f }
来源：http://fod.tanke756.top

C#:   Task.Run(() => F());
来源：http://wez.jinghuilouyu.cn

[O02] 使用线程池
来源：http://jvb.feifeiyinyue.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sdr.iojbl.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ktt.zycfv.cn

JS:   // worker_threads 线程池
来源：http://jdd.jyoumei.cn

TS:   // worker_threads 线程池
来源：http://obh.redwolf501.top

Java: Executors.newFixedThreadPool(4)
来源：http://bpp.aizwys.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://spn.shzxlz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fni.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ivg.hammf.cn

[O03] 加锁保护共享数据
来源：http://oux.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://mzy.snrcjt.cn

PHP:  // 用 flock() 做文件锁
来源：http://ggk.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fdb.vqdsnc.cn

TS:   // 同 JS
来源：http://dok.mhx1999.top

Java: synchronized (this) { shared++; }
来源：http://okv.shanyushiyangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zqe.zhiwuduotai.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uuy.svipenyu.cn

C#:   lock (gate) { shared++; }
来源：http://mre.cdnleiting.top

[O04] 定义异步函数并等待
来源：http://slu.cqqwz.cn

Py:   async def f():⏎    await g()
来源：http://zhz.gogol.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rpc.ybcxt.top

JS:   async function f() { await g(); }
来源：http://pfp.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wsw.ppjwa.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hcw.yongpay.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bxn.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://psc.gogol.net.cn

C#:   async Task F() { await G(); }
来源：http://dcl.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://wou.yueranfly.top

Py:   asyncio.gather(*tasks)
来源：http://mus.hcnkem.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://atp.yj202588.top

JS:   await Promise.all(tasks)
来源：http://fuz.hcnkem.com

TS:   await Promise.all(tasks)
来源：http://itt.nanxinkj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://drv.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pjz.kuanghao11.cn

Ruby: threads.map(&:join)
来源：http://eey.yueranfly.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pwq.shanyushiyangtech.top

[O06] 使用进程池
来源：http://ikn.chenzaomai.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uyc.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://rys.ydjk.org.cn

JS:   // child_process / cluster 模块
来源：http://nmt.fzhhl.top

TS:   // child_process / cluster 模块
来源：http://bnv.nanxinkj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sxq.zhengqikj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oqx.nwbrower.top

Ruby: // fork 块
来源：http://evn.wangdashe.top

C#:   Parallel.For
来源：http://xec.sjlbkw.cn

================================================================================
来源：http://pso.fzhhl.top

P. 常用工具函数
来源：http://hzo.wangdashe.top

================================================================================
来源：http://zuz.tian-w.cn

[P01] 生成 UUID
来源：http://ayw.epnwcf.com

Py:   str(uuid.uuid4())
来源：http://crm.ivvv.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rxq.shzxlz.cn

JS:   crypto.randomUUID()
来源：http://ztl.ydzc1.top

TS:   crypto.randomUUID()
来源：http://djv.9152youxi.cn

Java: UUID.randomUUID().toString()
来源：http://cyi.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://vvr.zhaomingkeji.xyz

Ruby: SecureRandom.uuid
来源：http://fmc.cheryme.top

C#:   Guid.NewGuid().ToString()
来源：http://crl.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://rhi.cqqwz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ior.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://akq.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sdg.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yft.daria6918.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://adb.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://igo.hnxiangtu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tfs.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rbk.hnqzz.top

[P03] 生成短随机字符串
来源：http://try.dianchejie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rtz.jianghu66.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ntv.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mvb.fanxiaobao.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zcz.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://anr.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hms.sxryk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sby.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qlw.quarkkingdee.top

[P04] 求长度
来源：http://wju.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kfi.vqdsnc.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bfp.fehbvm.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yzs.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cvq.ppjwa.cn

Java: list.size();  map.size();  s.length()
来源：http://yth.fehbvm.com

Go:   len(arr);  len(m)
来源：http://wqj.cashguo.top

Ruby: x.length;  x.size
来源：http://iyx.redwolf501.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vvc.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://byb.quarkkingdee.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zml.haohaochexian.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xph.zhoulong.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fmq.jinghuilouyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mjv.guannengcc.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mij.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://tvl.bjfxy.top

Ruby: a == b
来源：http://elt.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uxc.chenlongwang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zke.c1oappe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ase.hcnkem.com

PHP:  if (empty($x)) {}
来源：http://zkp.guannengcc.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gxx.guannengcc.top

TS:   if (x == null) {}
来源：http://gfr.xinyue.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://hea.xziqi.cn

Go:   if x == nil {}
来源：http://pwz.xylfe.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pms.xziqi.cn

C#:   if (x is null) {}
来源：http://lyp.svipenyu.cn

[P07] 防抖与节流
来源：http://wuz.fanxiaobao.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tlr.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://dkx.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gom.cqqwz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qio.zdqjudy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qko.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://smu.ppjwa.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wbe.epnwcf.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qtm.yongpay.top

[P08] 处理浮点精度问题
来源：http://bsn.jqgufenzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://usm.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dxv.zhaomingkeji.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gvr.pengpengdd.cyou

TS:   (0.1 + 0.2).toFixed(2)
来源：http://who.haohaochexian.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://juz.havefunace.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pxl.xinyue.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lqn.chenzaomai.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tdp.tianlin.xyz

================================================================================
来源：http://pcs.xinyue.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nca.tarul.cn

================================================================================
来源：http://sbt.yj20258888.top

[Q01] 创建表
来源：http://jwd.yj20258.top

CREATE TABLE users (
来源：http://hdl.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://agw.yanxiufei.cn

name VARCHAR(50) NOT NULL,
来源：http://gqb.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://wyl.nanxuanxn.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ilj.haohaochexian.top

);
来源：http://kzx.zhengqikj.top

[Q02] 创建带外键的表
来源：http://dfc.xziqi.cn

CREATE TABLE orders (
来源：http://wmt.ybcxt.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://efu.yj20258888.top

user_id INT NOT NULL,
来源：http://gut.wangdashe.top

amount DECIMAL(10, 2),
来源：http://epw.hesvh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xkm.xziqi.cn

);
来源：http://jyj.chenzaomai.com

[Q03] 增加列
来源：http://obt.feifeiyinyue.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mkd.hongshengwenyu.top

[Q04] 修改列类型
来源：http://iix.nanxinkj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ium.gaohongyu789.top

[Q05] 重命名列
来源：http://awj.sweek.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ibp.yangfankeji.com

[Q06] 删除列
来源：http://xyz.yueranfly.top

ALTER TABLE users DROP COLUMN age;
来源：http://grc.fzhhl.top

[Q07] 删除表
来源：http://qzs.shanyushiyangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://uhq.xuetiantiany.cn

[Q08] 创建普通索引
来源：http://lgk.yj20258.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hcn.sufxvd.cn

[Q09] 创建唯一索引
来源：http://evi.daxiang520.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://div.zdqjudy.top

[Q10] 插入单行
来源：http://syp.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cnv.ywan-chungtsiang.top

[Q11] 一次插入多行
来源：http://hva.sufxvd.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mqb.jyoumei.cn

[Q12] 插入后取自增 ID
来源：http://oii.zycfv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://col.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ife.xinyue.icu

[Q13] 忽略重复插入
来源：http://aja.zdbjq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qjg.shangyingyoupin.top

[Q14] 存在则更新（upsert）
来源：http://uib.hesvh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zdx.aizwys.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ase.hnqzz.top

[Q15] 查询全部
来源：http://xpy.shanyushiyangtech.top

SELECT * FROM users;
来源：http://drk.redwolf501.top

[Q16] 查询指定列
来源：http://mbv.bbcook.cn

SELECT id, name FROM users;
来源：http://mvd.tarul.cn

[Q17] 条件查询
来源：http://gto.yuxming.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wbn.jqgufenzy.top

[Q18] 模糊匹配
来源：http://uvw.jiagoushi.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ycg.kuanghao11.cn

[Q19] 范围查询
来源：http://mtx.yuanzhike.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ydz.xziqi.cn

[Q20] IN 列表
来源：http://ylm.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rmt.hywenlv.cn

[Q21] 空值判断
来源：http://myp.hywenlv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lyg.meibo888.top

[Q22] 排序
来源：http://pma.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cal.haohaochexian.top

[Q23] 分页
来源：http://aho.gotoacloud.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xaa.wangdashe.top

[Q24] 去重
来源：http://gpw.vqdsnc.cn

SELECT DISTINCT city FROM users;
来源：http://bfq.fktsv.cn

[Q25] 只取前 N 条
来源：http://kia.tianlin.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mqr.yvedp.cn

[Q26] 计数
来源：http://uzw.tian-w.cn

SELECT COUNT(*) FROM users;
来源：http://vkj.jinghuilouyu.cn

[Q27] 条件计数
来源：http://wur.cashguo.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wil.fzhhl.top

[Q28] 求和与平均
来源：http://flh.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ckf.hfpthk.cn

[Q29] 最大最小值
来源：http://iep.fanxiaobao.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://xqn.yj20258.top

[Q30] 分组统计
来源：http://blz.jiagoushi.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lao.shanyushiyangkeji.top

[Q31] 分组后过滤
来源：http://sth.nanxuanxn.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zit.chenlongwang.top

[Q32] 分组拼接字符串
来源：http://pfp.wangshuangyany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qge.redwolf501.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://crl.fengsongda.top

[Q33] 多列分组
来源：http://srj.gogol.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://axy.zhiwuduotai.top

[Q34] 每组取第一条
来源：http://wfl.zhaomingkeji.xyz

SELECT * FROM (
来源：http://kdm.hnxiangtu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://psm.316326.xyz

) t WHERE rn = 1;
来源：http://osh.shzxlz.cn

[Q35] 内连接
来源：http://zaq.svipenyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mky.ydzc1.top

[Q36] 左连接
来源：http://foy.gotoacloud.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hvx.yvedp.cn

[Q37] 右连接
来源：http://juk.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dpo.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bbz.shanyushiyangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qpz.gaohongyu789.top

[Q39] 自连接（查上下级）
来源：http://lal.yonumen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://skt.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rby.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://esz.epnwcf.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kut.chenlongwang.top

[Q41] 多表连接
来源：http://kjx.vqdsnc.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tui.xingfuxueyuan.xyz

JOIN users u ON u.id = o.user_id
来源：http://vwn.xinyue.icu

JOIN products p ON p.id = o.product_id;
来源：http://sxl.yongpay.top

[Q42] 连接条件附加过滤
来源：http://vcd.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://kno.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fmj.mhx1999.top

[Q43] 标量子查询
来源：http://svq.uphjek.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hwg.ywan-chungtsiang.top

[Q44] IN 子查询
来源：http://ufo.daria6918.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://igy.zdqjudy.top

[Q45] EXISTS 判断存在
来源：http://jte.zhengqikj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://two.hesvh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tbb.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kxr.sweek.top

[Q47] 与平均值比较
来源：http://yqr.shzxlz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uim.yonumen.top

[Q48] CTE 公用表表达式
来源：http://uql.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xpd.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://tqu.sweek.top

[Q49] 更新单行
来源：http://qer.316326.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yiv.yj20258.top

[Q50] 批量更新
来源：http://qnq.ctjpmb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ivg.zhoulong.xyz

[Q51] 用子查询更新
来源：http://phi.tian-w.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fwq.tianlin.xyz

[Q52] 删除指定行
来源：http://lvy.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://qmd.cheryme.top

[Q53] 按条件删除
来源：http://yny.fehbvm.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iij.xuetiantiany.cn

[Q54] 清空表
来源：http://mim.yj202588.top

TRUNCATE TABLE logs;
来源：http://hco.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://mmg.aibaodan.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fas.guowangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://uha.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tqx.316326.xyz

[Q57] 行号
来源：http://hdz.vehdjk.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sub.birdmap.top

[Q58] 累计求和
来源：http://qlh.cqqwz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ugf.aizwys.cn

[Q59] 分组内累计
来源：http://hhx.sysykeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yyl.jlsjyb.cn

[Q60] 取上一行 / 下一行
来源：http://hlp.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gas.yueranfly.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gzi.sufxvd.cn

[Q61] 移动平均
来源：http://xqr.ppjwa.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://urv.hcnkem.com

[Q62] 分组占比
来源：http://cpq.sysykeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rev.nanxuanxn.top

[Q63] 开启事务
来源：http://lrb.svipenyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zwa.iojbl.cn

[Q64] 提交事务
来源：http://nsu.uphjek.com

COMMIT;
来源：http://sqd.jqgufenzy.top

[Q65] 回滚事务
来源：http://pib.andypj.xyz

ROLLBACK;
来源：http://izq.316326.xyz

[Q66] 行锁查询
来源：http://mlo.yuxming.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://amg.yj20258888.top

[Q67] 设置隔离级别
来源：http://vqz.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sff.ydjk.org.cn

[Q68] 保存点
来源：http://smh.gogol.net.cn

SAVEPOINT sp1;
来源：http://qdp.vehdjk.com


<!-- 参考信息 -->