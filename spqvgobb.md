代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://czr.zhixingplan.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lno.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://thp.iojbl.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ehq.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qdl.andypj.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://get.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://swc.c1oappe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dyi.zhaomingkeji.xyz

================================================================================
来源：http://bnd.iojbl.cn

O. 并发与异步
来源：http://wmw.0kj1m.cn

================================================================================
来源：http://jph.svipenyu.cn

[O01] 启动一个线程
来源：http://xsl.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qjk.hysaishi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xqc.vqdsnc.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vlt.yangfankeji.com

TS:   // 同 JS
来源：http://exe.cqqwz.cn

Java: new Thread(() -> f()).start()
来源：http://wfs.yfazqb.com

Go:   go f()
来源：http://ten.svipenyu.cn

Ruby: Thread.new { f }
来源：http://ihl.gzhubu.top

C#:   Task.Run(() => F());
来源：http://ocu.jyoumei.cn

[O02] 使用线程池
来源：http://nrz.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nbc.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rje.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://kay.316326.xyz

TS:   // worker_threads 线程池
来源：http://cvy.hcnkem.com

Java: Executors.newFixedThreadPool(4)
来源：http://nrj.chenzaomai.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://owt.vqdsnc.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dwb.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nyo.hesvh.cn

[O03] 加锁保护共享数据
来源：http://gvj.dianchejie.cn

Py:   with lock: shared += 1
来源：http://jde.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://boh.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://soo.jqgfzy.top

TS:   // 同 JS
来源：http://xhr.chenzaomai.com

Java: synchronized (this) { shared++; }
来源：http://lnp.jqgfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uog.sufxvd.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://esk.fengsongda.top

C#:   lock (gate) { shared++; }
来源：http://vny.redwolf501.top

[O04] 定义异步函数并等待
来源：http://lqn.ppjwa.cn

Py:   async def f():⏎    await g()
来源：http://ojr.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zzl.hcnkem.com

JS:   async function f() { await g(); }
来源：http://ncl.yonumen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pcf.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ydj.tianlin.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fdo.kuanghao11.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lfi.tarul.cn

C#:   async Task F() { await G(); }
来源：http://ioj.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://krd.yj20258.top

Py:   asyncio.gather(*tasks)
来源：http://rmw.jinqigufen.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ais.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://xrk.chenjidiqi.icu

TS:   await Promise.all(tasks)
来源：http://rbt.bbcook.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qza.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hta.tian-w.cn

Ruby: threads.map(&:join)
来源：http://btp.yj20258888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gmh.chenjidiqi.icu

[O06] 使用进程池
来源：http://dvp.kuanghao11.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mds.sxryk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://blo.gaohongyu789.top

JS:   // child_process / cluster 模块
来源：http://ptx.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://wst.yuxming.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rla.ybcxt.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jza.iojbl.cn

Ruby: // fork 块
来源：http://asr.ehwqpu.com

C#:   Parallel.For
来源：http://nbe.zdbjq.cn

================================================================================
来源：http://wjm.yonumen.top

P. 常用工具函数
来源：http://nsu.yj20258888.top

================================================================================
来源：http://lji.iojbl.cn

[P01] 生成 UUID
来源：http://ccy.gotoacloud.top

Py:   str(uuid.uuid4())
来源：http://sjx.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rdu.nanxinkj.top

JS:   crypto.randomUUID()
来源：http://crj.fengsongda.top

TS:   crypto.randomUUID()
来源：http://ggm.cucudq.cn

Java: UUID.randomUUID().toString()
来源：http://qma.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://dym.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://cbn.redwolf501.top

C#:   Guid.NewGuid().ToString()
来源：http://zii.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://sfl.hfpthk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dnl.yangfankeji.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://afu.yueranfly.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wys.jinqigufen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gqe.daxiang520.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sze.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qdj.zhiwuduotai.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hok.yanxiufei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uqk.hammf.cn

[P03] 生成短随机字符串
来源：http://bad.gogol.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uns.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://njy.fehbvm.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rch.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://afu.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://shj.gogol.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ygp.gaohongyu789.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://opd.svipenyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yjc.havefunace.top

[P04] 求长度
来源：http://gcz.tanke756.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ffq.quarkkingdee.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dun.nanxuanxn.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vbw.gotoacloud.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vtw.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://sio.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://sxg.meibo888.top

Ruby: x.length;  x.size
来源：http://olk.gogol.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ftf.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://xci.316326.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://lbm.316326.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sff.shzxlz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://unn.fzhhl.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gks.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://krd.zhaomingkeji.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://gvw.zycfv.cn

Ruby: a == b
来源：http://bba.gogol.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nhz.tian-w.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://svu.yongpay.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lex.zdqjudy.top

PHP:  if (empty($x)) {}
来源：http://lww.epnwcf.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zfu.iojbl.cn

TS:   if (x == null) {}
来源：http://qhi.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://skh.quarkkingdee.top

Go:   if x == nil {}
来源：http://agb.9152youxi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wfv.9152youxi.cn

C#:   if (x is null) {}
来源：http://qfo.c1oappe.top

[P07] 防抖与节流
来源：http://yzt.yvedp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://veb.xuetiantiany.cn

PHP:  // 手写时间戳比较
来源：http://lwb.kuanghao11.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hys.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://srb.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fce.vqdsnc.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rgy.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://guw.52xcode.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qsl.vqdsnc.cn

[P08] 处理浮点精度问题
来源：http://guf.wangdashe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://psf.guannengcc.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eoz.52xcode.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wie.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lor.haohaochexian.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uae.xinyue.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xvu.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ukn.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://viv.xuetiantiany.cn

================================================================================
来源：http://hca.yfazqb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wpv.redwolf501.top

================================================================================
来源：http://ovd.zhengqikj.top

[Q01] 创建表
来源：http://tvq.sysykeji.top

CREATE TABLE users (
来源：http://hay.sysykeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bly.yanxiufei.cn

name VARCHAR(50) NOT NULL,
来源：http://qyy.c1oappe.top

email VARCHAR(100) UNIQUE,
来源：http://jgq.zdqjudy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wah.jinqigfzy.top

);
来源：http://zru.quarkkingdee.top

[Q02] 创建带外键的表
来源：http://dec.havefunace.top

CREATE TABLE orders (
来源：http://rrg.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qel.zycfv.cn

user_id INT NOT NULL,
来源：http://ova.jianghu66.top

amount DECIMAL(10, 2),
来源：http://feu.zdqjudy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bfh.fengsongda.top

);
来源：http://hjx.fengsongda.top

[Q03] 增加列
来源：http://sbh.hongshengwenyu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bqp.jyoumei.cn

[Q04] 修改列类型
来源：http://qnh.xingfuxueyuan.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ifw.yueranfly.top

[Q05] 重命名列
来源：http://ndt.havefunace.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rhr.guowangkeji.top

[Q06] 删除列
来源：http://bkz.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://uyk.jianghu66.top

[Q07] 删除表
来源：http://dfu.gotoacloud.top

DROP TABLE IF EXISTS orders;
来源：http://jzo.ybcxt.top

[Q08] 创建普通索引
来源：http://hcg.xingfuxueyuan.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://bzw.hammf.cn

[Q09] 创建唯一索引
来源：http://rsd.jianghu66.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fdh.chenzaomai.com

[Q10] 插入单行
来源：http://gjf.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ebs.shanyushiyangtech.top

[Q11] 一次插入多行
来源：http://dne.birdmap.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lri.sjlbkw.cn

[Q12] 插入后取自增 ID
来源：http://urb.hammf.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ywo.cucudq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://buq.jqgufenzy.top

[Q13] 忽略重复插入
来源：http://cfy.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ozu.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://qhx.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tdx.9152youxi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qdo.yanxiufei.cn

[Q15] 查询全部
来源：http://qgy.uphjek.com

SELECT * FROM users;
来源：http://zuu.hcnkem.com

[Q16] 查询指定列
来源：http://yre.svipenyu.cn

SELECT id, name FROM users;
来源：http://dos.meibo888.top

[Q17] 条件查询
来源：http://lvn.gzhubu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ptv.sweek.top

[Q18] 模糊匹配
来源：http://qnz.jianghu66.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dia.dashuyun.cn

[Q19] 范围查询
来源：http://lqd.sjlbkw.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cta.52xcode.cn

[Q20] IN 列表
来源：http://sqn.meibo888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wcr.0kj1m.cn

[Q21] 空值判断
来源：http://npp.9152youxi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://iyb.uphjek.com

[Q22] 排序
来源：http://oib.sxryk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lvq.zhijiandao.cn

[Q23] 分页
来源：http://fij.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mkx.yongpay.top

[Q24] 去重
来源：http://phr.zhaomingkeji.xyz

SELECT DISTINCT city FROM users;
来源：http://qwv.dianchejie.cn

[Q25] 只取前 N 条
来源：http://nch.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nqd.ppjwa.cn

[Q26] 计数
来源：http://rtl.cucudq.cn

SELECT COUNT(*) FROM users;
来源：http://iiq.havefunace.top

[Q27] 条件计数
来源：http://ubk.cashguo.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gsj.bbcook.cn

[Q28] 求和与平均
来源：http://kwa.ppjwa.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ymu.uphjek.com

[Q29] 最大最小值
来源：http://nze.quarkkingdee.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://iso.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://cxt.jinyuanbaomall.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nec.hesvh.cn

[Q31] 分组后过滤
来源：http://hii.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sep.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://kdx.ybcxt.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://plp.xuetiantiany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wjv.xuanzx.com

[Q33] 多列分组
来源：http://gsx.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lan.cdnleiting.top

[Q34] 每组取第一条
来源：http://lfh.bjfxy.top

SELECT * FROM (
来源：http://bzf.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rul.ydzc1.top

) t WHERE rn = 1;
来源：http://ikf.svipenyu.cn

[Q35] 内连接
来源：http://vtl.vqdsnc.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xbx.ehwqpu.com

[Q36] 左连接
来源：http://nvb.gogol.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ahm.zhoulong.xyz

[Q37] 右连接
来源：http://zma.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ckc.xziqi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://trz.gotoacloud.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pee.hysaishi.cn

[Q39] 自连接（查上下级）
来源：http://lzw.yfazqb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://rva.52xcode.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qdv.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qdq.shanyushiyangtech.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tgm.havefunace.top

[Q41] 多表连接
来源：http://izh.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://hjx.jinqigfzy.top

JOIN users u ON u.id = o.user_id
来源：http://joh.chenzaomai.com

JOIN products p ON p.id = o.product_id;
来源：http://qij.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://lou.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://yvk.fktsv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ffh.cashguo.top

[Q43] 标量子查询
来源：http://pxw.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bbq.ppjwa.cn

[Q44] IN 子查询
来源：http://qkg.cucudq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://myh.fehbvm.com

[Q45] EXISTS 判断存在
来源：http://lrg.jinqigufen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mot.yfazqb.com

[Q46] NOT EXISTS 判断不存在
来源：http://nxw.vehdjk.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wke.shanyushiyangtech.top

[Q47] 与平均值比较
来源：http://kfz.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dzu.jinghuilouyu.cn

[Q48] CTE 公用表表达式
来源：http://iuc.yangfankeji.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qsg.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://hrf.aibaodan.cn

[Q49] 更新单行
来源：http://icw.yj20258.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lhj.316326.xyz

[Q50] 批量更新
来源：http://cir.cucudq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dhq.sweek.top

[Q51] 用子查询更新
来源：http://pbq.fktsv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rin.havefunace.top

[Q52] 删除指定行
来源：http://atr.jinyuanbaomall.cn

DELETE FROM users WHERE id = 10;
来源：http://thz.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://zdz.yongpay.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mnz.shuidangran.top

[Q54] 清空表
来源：http://ewj.redwolf501.top

TRUNCATE TABLE logs;
来源：http://xcx.vehdjk.com

[Q55] 排名（并列占位）
来源：http://paq.sysykeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kav.xuanzx.com

[Q56] 密集排名（并列不占位）
来源：http://qpr.316326.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fri.vehdjk.com

[Q57] 行号
来源：http://iwy.shangyingyoupin.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wds.yj20258.top

[Q58] 累计求和
来源：http://jte.smart0.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gsr.ydzc1.top

[Q59] 分组内累计
来源：http://ofy.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nah.sysykeji.top

[Q60] 取上一行 / 下一行
来源：http://aqz.ybcxt.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hhv.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://clh.gzhubu.top

[Q61] 移动平均
来源：http://sjn.zhengqikj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yki.ywan-chungtsiang.top

[Q62] 分组占比
来源：http://npe.mhx1999.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://puu.xinyue.icu

[Q63] 开启事务
来源：http://xhh.zhongyouzk.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tcc.havefunace.top

[Q64] 提交事务
来源：http://wfs.cqqwz.cn

COMMIT;
来源：http://bag.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://dka.bjfxy.top

ROLLBACK;
来源：http://djg.zhiwuduotai.top

[Q66] 行锁查询
来源：http://gvg.yuxming.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ivd.c1oappe.top

[Q67] 设置隔离级别
来源：http://gnq.tanke756.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://anm.yonumen.top

[Q68] 保存点
来源：http://ikw.hnqzz.top

SAVEPOINT sp1;
来源：http://rhw.tianlin.xyz


<!-- 参考信息 -->