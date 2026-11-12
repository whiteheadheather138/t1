代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ahs.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xqh.cqqwz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rfg.ywan-chungtsiang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ijn.xingfuxueyuan.xyz

================================================================================
来源：http://gaf.sxryk.cn

O. 并发与异步
来源：http://eav.nwbrower.top

================================================================================
来源：http://fln.nwbrower.top

[O01] 启动一个线程
来源：http://qgq.xziqi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bmr.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qhf.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://paa.zhixingplan.top

TS:   // 同 JS
来源：http://whc.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://fcu.jinqigufen.top

Go:   go f()
来源：http://bto.tianlin.xyz

Ruby: Thread.new { f }
来源：http://hvd.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://dgx.pengpengdd.cyou

[O02] 使用线程池
来源：http://sip.aibaodan.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bqs.hongshengwenyu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://srz.tarul.cn

JS:   // worker_threads 线程池
来源：http://rwf.jqgufenzy.top

TS:   // worker_threads 线程池
来源：http://qzi.hesvh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ryf.ydjk.org.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sco.shanyushiyangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lbe.cashguo.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blu.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://ftc.cucudq.cn

Py:   with lock: shared += 1
来源：http://xxs.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://fhd.quarkkingdee.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vpy.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://iob.dianchejie.cn

Java: synchronized (this) { shared++; }
来源：http://rjg.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://utr.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zxc.yonumen.top

C#:   lock (gate) { shared++; }
来源：http://vyf.iojbl.cn

[O04] 定义异步函数并等待
来源：http://xlx.hnqzz.top

Py:   async def f():⏎    await g()
来源：http://goa.jyoumei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lgi.ydjk.org.cn

JS:   async function f() { await g(); }
来源：http://yrv.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nwv.gaohongyu789.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kgn.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bqx.ybcxt.top

Ruby: # 用 Fiber 或 async gem
来源：http://pce.nanxuanxn.top

C#:   async Task F() { await G(); }
来源：http://xsi.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://fjz.shangyingyoupin.top

Py:   asyncio.gather(*tasks)
来源：http://bzn.cashguo.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lkn.shanyushiyangtech.top

JS:   await Promise.all(tasks)
来源：http://amj.hongshengwenyu.top

TS:   await Promise.all(tasks)
来源：http://xnt.yj202588.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kjp.yj20258.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aiv.fzhhl.top

Ruby: threads.map(&:join)
来源：http://rxo.xingfuxueyuan.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://jkd.ydjk.org.cn

[O06] 使用进程池
来源：http://cbj.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hon.cqqwz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gea.wangdashe.top

JS:   // child_process / cluster 模块
来源：http://hhp.yj20258.top

TS:   // child_process / cluster 模块
来源：http://cjv.tianlin.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tnh.wangdashe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://npe.cheryme.top

Ruby: // fork 块
来源：http://cgt.sjlbkw.cn

C#:   Parallel.For
来源：http://vhy.sweek.top

================================================================================
来源：http://jcv.tarul.cn

P. 常用工具函数
来源：http://bsl.yanxiufei.cn

================================================================================
来源：http://ovs.bjfxy.top

[P01] 生成 UUID
来源：http://tcj.havefunace.top

Py:   str(uuid.uuid4())
来源：http://pve.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mrv.sufxvd.cn

JS:   crypto.randomUUID()
来源：http://zky.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://jhr.yangfankeji.com

Java: UUID.randomUUID().toString()
来源：http://sum.tian-w.cn

Go:   // 用 github.com/google/uuid
来源：http://ixj.zhiwuduotai.top

Ruby: SecureRandom.uuid
来源：http://odb.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://aaq.jqgfzy.top

[P02] MD5 / SHA256 摘要
来源：http://ndh.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dqh.jyoumei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eii.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ewh.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qpu.c1oappe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sxq.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lps.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kzu.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vqh.fengsongda.top

[P03] 生成短随机字符串
来源：http://uey.gogol.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lxt.iojbl.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ywd.hesvh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oda.yj202588.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uno.ybcxt.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wvb.tian-w.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zqb.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zfh.hesvh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dwk.yuanzhike.top

[P04] 求长度
来源：http://gov.gzhubu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jhf.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mto.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dpz.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://asn.xinyue.icu

Java: list.size();  map.size();  s.length()
来源：http://dmg.xziqi.cn

Go:   len(arr);  len(m)
来源：http://mjx.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://dad.fengsongda.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tvh.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://ydg.xylfe.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ska.guannengcc.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yze.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cjl.cheryme.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://obk.fktsv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gos.ybcxt.top

Go:   reflect.DeepEqual(a, b)
来源：http://irj.yuxming.cn

Ruby: a == b
来源：http://yvj.hammf.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ndq.sjlbkw.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bkb.jianghu66.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dav.yfazqb.com

PHP:  if (empty($x)) {}
来源：http://jnt.jianghu66.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pmz.wangdashe.top

TS:   if (x == null) {}
来源：http://ayf.zdqjudy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vmi.fzhhl.top

Go:   if x == nil {}
来源：http://rqd.cheryme.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://usj.xuanzx.com

C#:   if (x is null) {}
来源：http://nrh.bjfxy.top

[P07] 防抖与节流
来源：http://sbn.zdqjudy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hns.yangfankeji.com

PHP:  // 手写时间戳比较
来源：http://tzu.jqgufenzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pzh.wangshuangyany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jnl.fzhhl.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qbu.tarul.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wed.shuidangran.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ofx.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pcc.smart0.xyz

[P08] 处理浮点精度问题
来源：http://hak.wangshuangyany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oft.zhaomingkeji.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zct.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dwq.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ibm.sysykeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://exl.birdmap.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uqj.nanxinkj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cxk.gotoacloud.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ref.chenjidiqi.icu

================================================================================
来源：http://psw.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cqq.52xcode.cn

================================================================================
来源：http://mpz.nanxinkj.top

[Q01] 创建表
来源：http://bjs.redwolf501.top

CREATE TABLE users (
来源：http://rtk.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ewv.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://ivf.chenjidiqi.icu

email VARCHAR(100) UNIQUE,
来源：http://vtb.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zci.zhixingplan.top

);
来源：http://nni.tian-w.cn

[Q02] 创建带外键的表
来源：http://zfh.ywan-chungtsiang.top

CREATE TABLE orders (
来源：http://zmx.yueranfly.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yfw.iojbl.cn

user_id INT NOT NULL,
来源：http://hak.daxiang520.top

amount DECIMAL(10, 2),
来源：http://sjd.yanxiufei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qys.c1oappe.top

);
来源：http://nqa.zhijiandao.cn

[Q03] 增加列
来源：http://ubu.yanxiufei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hjd.gotoacloud.top

[Q04] 修改列类型
来源：http://tbh.xylfe.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://osz.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://fiz.sysykeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xsf.sxryk.cn

[Q06] 删除列
来源：http://dxa.kuanghao11.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jhi.vqdsnc.cn

[Q07] 删除表
来源：http://tby.hysaishi.cn

DROP TABLE IF EXISTS orders;
来源：http://myl.yfazqb.com

[Q08] 创建普通索引
来源：http://hoq.tarul.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wvo.svipenyu.cn

[Q09] 创建唯一索引
来源：http://kff.zdqjudy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ukc.jinghuilouyu.cn

[Q10] 插入单行
来源：http://gwr.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mao.yj202588.top

[Q11] 一次插入多行
来源：http://gvn.guowangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://duj.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://yut.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://vax.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jls.sjlbkw.cn

[Q13] 忽略重复插入
来源：http://all.fktsv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bax.kuanghao11.cn

[Q14] 存在则更新（upsert）
来源：http://oku.zhaomingkeji.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zvp.yj20258.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zel.xziqi.cn

[Q15] 查询全部
来源：http://fkx.gaohongyu789.top

SELECT * FROM users;
来源：http://noc.yueranfly.top

[Q16] 查询指定列
来源：http://mfa.jqgfzy.top

SELECT id, name FROM users;
来源：http://osf.shuidangran.top

[Q17] 条件查询
来源：http://apd.hesvh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pew.jinghuilouyu.cn

[Q18] 模糊匹配
来源：http://lts.zdqjudy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rfz.jinyuanbaomall.cn

[Q19] 范围查询
来源：http://lbh.xingfuxueyuan.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jmm.zycfv.cn

[Q20] IN 列表
来源：http://onc.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kwv.daxiang520.top

[Q21] 空值判断
来源：http://wug.hysaishi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hck.chenlongwang.top

[Q22] 排序
来源：http://gwr.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lep.bjfxy.top

[Q23] 分页
来源：http://dey.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fhf.fzhhl.top

[Q24] 去重
来源：http://chh.svipenyu.cn

SELECT DISTINCT city FROM users;
来源：http://nys.sweek.top

[Q25] 只取前 N 条
来源：http://gre.chenjidiqi.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vsj.nanxinkj.top

[Q26] 计数
来源：http://fda.0kj1m.cn

SELECT COUNT(*) FROM users;
来源：http://xnv.yongpay.top

[Q27] 条件计数
来源：http://job.jiagoushi.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://syz.dianchejie.cn

[Q28] 求和与平均
来源：http://yyu.hcnkem.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://scs.316326.xyz

[Q29] 最大最小值
来源：http://jnm.zhiwuduotai.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://okc.daria6918.cn

[Q30] 分组统计
来源：http://uwd.shangyingyoupin.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wfd.zhongyouzk.top

[Q31] 分组后过滤
来源：http://xdv.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gwu.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://csm.jyoumei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gsx.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ype.yanxiufei.cn

[Q33] 多列分组
来源：http://szg.0kj1m.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wye.9152youxi.cn

[Q34] 每组取第一条
来源：http://zbz.gaohongyu789.top

SELECT * FROM (
来源：http://pno.hnqzz.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zhf.tanke756.top

) t WHERE rn = 1;
来源：http://thm.fzhhl.top

[Q35] 内连接
来源：http://ahz.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://knn.jinqigfzy.top

[Q36] 左连接
来源：http://pud.daria6918.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://etc.jinqigufen.top

[Q37] 右连接
来源：http://oof.jqgfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pop.yfazqb.com

[Q38] 全外连接（PostgreSQL）
来源：http://wub.fktsv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qpf.pengpengdd.cyou

[Q39] 自连接（查上下级）
来源：http://lpc.shanyushiyangtech.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mxm.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zds.guannengcc.top

[Q40] 交叉连接（笛卡尔积）
来源：http://yti.yonumen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eeo.hesvh.cn

[Q41] 多表连接
来源：http://aoe.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://grv.xuanzx.com

JOIN users u ON u.id = o.user_id
来源：http://ebr.guowangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://fea.fktsv.cn

[Q42] 连接条件附加过滤
来源：http://ysv.shuidangran.top

SELECT u.name, o.amount FROM users u
来源：http://isa.aizwys.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bfc.vehdjk.com

[Q43] 标量子查询
来源：http://iws.sjlbkw.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jwt.316326.xyz

[Q44] IN 子查询
来源：http://fas.jqgufenzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hzm.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://xyw.ctjpmb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zfv.chenzaomai.com

[Q46] NOT EXISTS 判断不存在
来源：http://jnq.zhijiandao.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hvc.jlsjyb.cn

[Q47] 与平均值比较
来源：http://zne.jyoumei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kvb.vqdsnc.cn

[Q48] CTE 公用表表达式
来源：http://dqb.feifeiyinyue.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fph.hcnkem.com

SELECT * FROM t WHERE c > 5;
来源：http://tia.yj20258888.top

[Q49] 更新单行
来源：http://yfa.jlsjyb.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xss.sysykeji.top

[Q50] 批量更新
来源：http://wtu.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rqa.hfpthk.cn

[Q51] 用子查询更新
来源：http://pwr.wangdashe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ugn.xuanzx.com

[Q52] 删除指定行
来源：http://dop.xingfuxueyuan.xyz

DELETE FROM users WHERE id = 10;
来源：http://wwh.meibo888.top

[Q53] 按条件删除
来源：http://awj.hammf.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kms.zhengqikj.top

[Q54] 清空表
来源：http://jej.yongpay.top

TRUNCATE TABLE logs;
来源：http://zex.xingfuxueyuan.xyz

[Q55] 排名（并列占位）
来源：http://llb.zdbjq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uqm.haohaochexian.top

[Q56] 密集排名（并列不占位）
来源：http://ldv.zhongyouzk.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wxm.daxiang520.top

[Q57] 行号
来源：http://bmo.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tjv.fzhhl.top

[Q58] 累计求和
来源：http://dto.smart0.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jyd.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://iyu.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tcu.fanxiaobao.xyz

[Q60] 取上一行 / 下一行
来源：http://afr.nanxuanxn.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sjw.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rsi.nanxuanxn.top

[Q61] 移动平均
来源：http://lcf.guowangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dxn.nanxinkj.top

[Q62] 分组占比
来源：http://wsk.c1oappe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zae.jqgufenzy.top

[Q63] 开启事务
来源：http://wbo.xinyue.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://reo.9152youxi.cn

[Q64] 提交事务
来源：http://srl.jiagoushi.top

COMMIT;
来源：http://geh.redwolf501.top

[Q65] 回滚事务
来源：http://grr.yuanzhike.top

ROLLBACK;
来源：http://zad.sweek.top

[Q66] 行锁查询
来源：http://woa.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oei.jinghuilouyu.cn

[Q67] 设置隔离级别
来源：http://nof.yonumen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://seu.iojbl.cn

[Q68] 保存点
来源：http://srg.svipenyu.cn

SAVEPOINT sp1;
来源：http://pvd.cdnleiting.top

ROLLBACK TO sp1;
来源：http://mdu.pycfn.com

[Q69] 查看执行计划
来源：http://pxm.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qvc.pengpengdd.cyou

[Q70] 更新统计信息
来源：http://vco.dianchejie.cn


<!-- 参考信息 -->