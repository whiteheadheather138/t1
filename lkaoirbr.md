代发 wailian999

Go:   // 手写递归
来源：http://pka.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rxb.pycfn.com

C#:   // 手写递归
来源：http://jac.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zqy.havefunace.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://enq.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hot.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xzx.zhijiandao.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ufs.zhijiandao.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://maj.zhixingplan.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rtr.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tsv.jqgfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fwb.gzhubu.top

================================================================================
来源：http://eio.chenlongwang.top

O. 并发与异步
来源：http://hyo.yj20258888.top

================================================================================
来源：http://bsz.guowangkeji.top

[O01] 启动一个线程
来源：http://saw.jinqigfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wat.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://svi.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rcg.haohaochexian.top

TS:   // 同 JS
来源：http://fiy.cqqwz.cn

Java: new Thread(() -> f()).start()
来源：http://rna.yvedp.cn

Go:   go f()
来源：http://rvs.bjfxy.top

Ruby: Thread.new { f }
来源：http://cur.wangshuangyany.cn

C#:   Task.Run(() => F());
来源：http://yvf.jqgfzy.top

[O02] 使用线程池
来源：http://zhf.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ybp.fehbvm.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qog.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://cwu.shzxlz.cn

TS:   // worker_threads 线程池
来源：http://xxk.shuidangran.top

Java: Executors.newFixedThreadPool(4)
来源：http://hnz.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lgf.guannengcc.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fqt.xuanzx.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cap.snrcjt.cn

[O03] 加锁保护共享数据
来源：http://wid.jinqigufen.top

Py:   with lock: shared += 1
来源：http://smh.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://wju.sysykeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bit.hywenlv.cn

TS:   // 同 JS
来源：http://qgk.xuanzx.com

Java: synchronized (this) { shared++; }
来源：http://wjh.hammf.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zcn.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qgz.zycfv.cn

C#:   lock (gate) { shared++; }
来源：http://eei.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://phx.yonumen.top

Py:   async def f():⏎    await g()
来源：http://xsk.sysykeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sic.xinyue.icu

JS:   async function f() { await g(); }
来源：http://qfi.jinqigfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hii.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nap.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jvw.hnqzz.top

Ruby: # 用 Fiber 或 async gem
来源：http://ucr.ctjpmb.com

C#:   async Task F() { await G(); }
来源：http://wos.cqqwz.cn

[O05] 并发执行并等待全部完成
来源：http://pub.fanxiaobao.xyz

Py:   asyncio.gather(*tasks)
来源：http://lkk.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wov.zycfv.cn

JS:   await Promise.all(tasks)
来源：http://odo.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://ejx.epnwcf.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://puo.ivvv.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ynf.yj20258.top

Ruby: threads.map(&:join)
来源：http://fhz.nanxuanxn.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mxe.haohaochexian.top

[O06] 使用进程池
来源：http://djy.uphjek.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://snb.hywenlv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qxc.gogol.net.cn

JS:   // child_process / cluster 模块
来源：http://dms.smart0.xyz

TS:   // child_process / cluster 模块
来源：http://icm.hywenlv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dgw.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dts.gotoacloud.top

Ruby: // fork 块
来源：http://boz.aibaodan.cn

C#:   Parallel.For
来源：http://ktb.redwolf501.top

================================================================================
来源：http://iak.zhaomingkeji.xyz

P. 常用工具函数
来源：http://avf.chenjidiqi.icu

================================================================================
来源：http://wns.aibaodan.cn

[P01] 生成 UUID
来源：http://zdb.fktsv.cn

Py:   str(uuid.uuid4())
来源：http://dea.ivvv.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://szk.yfazqb.com

JS:   crypto.randomUUID()
来源：http://rsp.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://adg.sweek.top

Java: UUID.randomUUID().toString()
来源：http://myv.wangdashe.top

Go:   // 用 github.com/google/uuid
来源：http://gce.hcnkem.com

Ruby: SecureRandom.uuid
来源：http://shx.hcnkem.com

C#:   Guid.NewGuid().ToString()
来源：http://otm.cashguo.top

[P02] MD5 / SHA256 摘要
来源：http://tse.tianlin.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nsk.yonumen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bdu.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rpv.316326.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://peh.svipenyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://csh.gogol.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uzw.fktsv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eoe.chenzaomai.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://htr.shzxlz.cn

[P03] 生成短随机字符串
来源：http://fbd.hfpthk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dvh.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://svc.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nyg.iojbl.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ydf.feifeiyinyue.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://epd.cashguo.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ugu.nanxinkj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://swq.shangyingyoupin.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lal.xingfuxueyuan.xyz

[P04] 求长度
来源：http://xwh.cucudq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yjw.ppjwa.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gjb.yangfankeji.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rom.fengsongda.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ivt.quarkkingdee.top

Java: list.size();  map.size();  s.length()
来源：http://piy.bbcook.cn

Go:   len(arr);  len(m)
来源：http://psu.jlsjyb.cn

Ruby: x.length;  x.size
来源：http://hqy.fengsongda.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wwh.bjfxy.top

[P05] 判断两个对象内容是否相等
来源：http://hqw.nwbrower.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ccm.svipenyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nxx.fehbvm.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://twm.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ial.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rtq.jinyuanbaomall.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bkn.dashuyun.cn

Ruby: a == b
来源：http://lco.tanke756.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qxf.tanke756.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xeg.c1oappe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://opq.chenjidiqi.icu

PHP:  if (empty($x)) {}
来源：http://nib.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wly.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://czy.c1oappe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uaj.316326.xyz

Go:   if x == nil {}
来源：http://pgc.xingfuxueyuan.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aus.fengsongda.top

C#:   if (x is null) {}
来源：http://sps.wangdashe.top

[P07] 防抖与节流
来源：http://rsk.haohaochexian.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://itb.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://hax.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zft.yangfankeji.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xsd.svipenyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ccm.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://upu.bbcook.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hdi.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bqy.yanxiufei.cn

[P08] 处理浮点精度问题
来源：http://mst.gotoacloud.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qwk.yueranfly.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yjp.daxiang520.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xff.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wlk.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ilx.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qoh.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://myu.xuanzx.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://otr.jinqigufen.top

================================================================================
来源：http://vjg.yongpay.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oam.tarul.cn

================================================================================
来源：http://dsv.zhixingplan.top

[Q01] 创建表
来源：http://tyy.zhixingplan.top

CREATE TABLE users (
来源：http://ycq.yangfankeji.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fwb.hongshengwenyu.top

name VARCHAR(50) NOT NULL,
来源：http://gez.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://psx.hongshengwenyu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nko.fengsongda.top

);
来源：http://hiy.zdqjudy.top

[Q02] 创建带外键的表
来源：http://ejk.hysaishi.cn

CREATE TABLE orders (
来源：http://cxh.snrcjt.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zaz.uphjek.com

user_id INT NOT NULL,
来源：http://ozv.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://sgv.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xgr.zhixingplan.top

);
来源：http://suf.redwolf501.top

[Q03] 增加列
来源：http://oer.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fii.ywan-chungtsiang.top

[Q04] 修改列类型
来源：http://scf.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rbu.hysaishi.cn

[Q05] 重命名列
来源：http://jcr.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://orz.ppjwa.cn

[Q06] 删除列
来源：http://jid.yanxiufei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nxp.snrcjt.cn

[Q07] 删除表
来源：http://dyj.sjlbkw.cn

DROP TABLE IF EXISTS orders;
来源：http://xlj.nanxinkj.top

[Q08] 创建普通索引
来源：http://mon.andypj.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://lif.zhaomingkeji.xyz

[Q09] 创建唯一索引
来源：http://udg.shuidangran.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gcx.snrcjt.cn

[Q10] 插入单行
来源：http://hau.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hza.aibaodan.cn

[Q11] 一次插入多行
来源：http://ntf.iojbl.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yoo.yonumen.top

[Q12] 插入后取自增 ID
来源：http://pkf.dashuyun.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pnj.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ucm.ppjwa.cn

[Q13] 忽略重复插入
来源：http://xbn.xylfe.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gzf.jqgufenzy.top

[Q14] 存在则更新（upsert）
来源：http://kyi.tianlin.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gag.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bwn.meibo888.top

[Q15] 查询全部
来源：http://xfe.aizwys.cn

SELECT * FROM users;
来源：http://uuu.shanyushiyangtech.top

[Q16] 查询指定列
来源：http://tow.zycfv.cn

SELECT id, name FROM users;
来源：http://srk.zycfv.cn

[Q17] 条件查询
来源：http://fjn.jqgufenzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tdd.xuanzx.com

[Q18] 模糊匹配
来源：http://lvz.jlsjyb.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xsc.yueranfly.top

[Q19] 范围查询
来源：http://qsj.fktsv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gos.jianghu66.top

[Q20] IN 列表
来源：http://wil.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vmc.jinghuilouyu.cn

[Q21] 空值判断
来源：http://yuj.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kvz.yanxiufei.cn

[Q22] 排序
来源：http://bia.yfazqb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mcm.ivvv.top

[Q23] 分页
来源：http://ass.yvedp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iox.ybcxt.top

[Q24] 去重
来源：http://kbe.yj202588.top

SELECT DISTINCT city FROM users;
来源：http://beo.chenzaomai.com

[Q25] 只取前 N 条
来源：http://lzx.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vok.zycfv.cn

[Q26] 计数
来源：http://nsl.havefunace.top

SELECT COUNT(*) FROM users;
来源：http://rqh.jinyuanbaomall.cn

[Q27] 条件计数
来源：http://iyu.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xkt.tian-w.cn

[Q28] 求和与平均
来源：http://vpq.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://btn.bjfxy.top

[Q29] 最大最小值
来源：http://mgc.chenzaomai.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://qsi.daxiang520.top

[Q30] 分组统计
来源：http://vja.feifeiyinyue.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lgq.smart0.xyz

[Q31] 分组后过滤
来源：http://rvi.mhx1999.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://owg.sweek.top

[Q32] 分组拼接字符串
来源：http://fml.sjlbkw.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iha.sysykeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hwd.jqgufenzy.top

[Q33] 多列分组
来源：http://mid.tarul.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://neh.nwbrower.top

[Q34] 每组取第一条
来源：http://ghf.guannengcc.top

SELECT * FROM (
来源：http://sed.cucudq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ciu.jinyuanbaomall.cn

) t WHERE rn = 1;
来源：http://fac.pycfn.com

[Q35] 内连接
来源：http://ecs.gotoacloud.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tve.smart0.xyz

[Q36] 左连接
来源：http://kzr.jqgfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wry.cheryme.top

[Q37] 右连接
来源：http://apf.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://krt.daria6918.cn

[Q38] 全外连接（PostgreSQL）
来源：http://stu.cheryme.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://utx.jianghu66.top

[Q39] 自连接（查上下级）
来源：http://gbm.fehbvm.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://jcb.wangdashe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bmv.kuanghao11.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jdl.cdnleiting.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wts.mhx1999.top

[Q41] 多表连接
来源：http://pwg.fengsongda.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ayf.0kj1m.cn

JOIN users u ON u.id = o.user_id
来源：http://abj.vehdjk.com

JOIN products p ON p.id = o.product_id;
来源：http://fpn.pycfn.com

[Q42] 连接条件附加过滤
来源：http://wfq.fzhhl.top

SELECT u.name, o.amount FROM users u
来源：http://hjt.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tph.xingfuxueyuan.xyz

[Q43] 标量子查询
来源：http://pck.cdnleiting.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gbl.dashuyun.cn

[Q44] IN 子查询
来源：http://yvq.ehwqpu.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ofv.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://dgv.gogol.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rem.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://qux.jianghu66.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://psw.hongshengwenyu.top

[Q47] 与平均值比较
来源：http://xbw.mhx1999.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gxp.gzhubu.top

[Q48] CTE 公用表表达式
来源：http://fsz.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jcc.pycfn.com

SELECT * FROM t WHERE c > 5;
来源：http://yqc.jinghuilouyu.cn

[Q49] 更新单行
来源：http://auz.yuxming.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://htq.shangyingyoupin.top

[Q50] 批量更新
来源：http://drv.daria6918.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xsg.shuidangran.top

[Q51] 用子查询更新
来源：http://gpd.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lsg.wangshuangyany.cn

[Q52] 删除指定行
来源：http://lnz.jlsjyb.cn

DELETE FROM users WHERE id = 10;
来源：http://eus.bbcook.cn

[Q53] 按条件删除
来源：http://aws.xylfe.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oib.nanxinkj.top

[Q54] 清空表
来源：http://cgq.9152youxi.cn

TRUNCATE TABLE logs;
来源：http://qpf.mhx1999.top

[Q55] 排名（并列占位）
来源：http://yys.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vlg.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://tqz.yfazqb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ojb.birdmap.top

[Q57] 行号
来源：http://cty.daxiang520.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xgq.fanxiaobao.xyz

[Q58] 累计求和
来源：http://ztl.cashguo.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bxq.jinqigfzy.top

[Q59] 分组内累计
来源：http://ons.chenlongwang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fnj.fehbvm.com

[Q60] 取上一行 / 下一行
来源：http://vbl.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zrb.jqgfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xrh.ywan-chungtsiang.top

[Q61] 移动平均
来源：http://xzx.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oqc.jinghuilouyu.cn

[Q62] 分组占比
来源：http://yah.aizwys.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qji.tarul.cn

[Q63] 开启事务
来源：http://zzd.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vpf.ydzc1.top

[Q64] 提交事务
来源：http://vmm.shuidangran.top

COMMIT;
来源：http://ios.zhongyouzk.top

[Q65] 回滚事务
来源：http://uou.316326.xyz

ROLLBACK;
来源：http://tuz.zdbjq.cn

[Q66] 行锁查询
来源：http://ahi.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zwr.zhoulong.xyz


<!-- 参考信息 -->