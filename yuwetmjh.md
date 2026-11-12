代发 wailian999

PHP:  // 手写递归函数
来源：http://kpq.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zvh.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nhq.vqdsnc.cn

Java: // 手写递归
来源：http://rao.chenzaomai.com

Go:   // 手写递归
来源：http://zqj.snrcjt.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mpv.ybcxt.top

C#:   // 手写递归
来源：http://upf.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://otr.aibaodan.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://byd.guowangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gra.0kj1m.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xfj.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hfe.pycfn.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ojs.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yfi.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vxx.yj20258.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xzs.dashuyun.cn

================================================================================
来源：http://udp.pycfn.com

O. 并发与异步
来源：http://ypa.meibo888.top

================================================================================
来源：http://qtj.wangdashe.top

[O01] 启动一个线程
来源：http://cwq.cqqwz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zrx.zhixingplan.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rlj.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://axy.zycfv.cn

TS:   // 同 JS
来源：http://eve.aibaodan.cn

Java: new Thread(() -> f()).start()
来源：http://epf.316326.xyz

Go:   go f()
来源：http://oum.bjfxy.top

Ruby: Thread.new { f }
来源：http://pem.ctjpmb.com

C#:   Task.Run(() => F());
来源：http://fun.havefunace.top

[O02] 使用线程池
来源：http://gqo.birdmap.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sno.guannengcc.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ukj.andypj.xyz

JS:   // worker_threads 线程池
来源：http://siq.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://nwv.jlsjyb.cn

Java: Executors.newFixedThreadPool(4)
来源：http://owa.cucudq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ghh.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://otv.redwolf501.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gwx.xuetiantiany.cn

[O03] 加锁保护共享数据
来源：http://qfn.shuidangran.top

Py:   with lock: shared += 1
来源：http://sgk.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://ngf.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xcj.sxryk.cn

TS:   // 同 JS
来源：http://nmv.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://itj.chenzaomai.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://swq.daria6918.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cpp.zhijiandao.cn

C#:   lock (gate) { shared++; }
来源：http://rie.c1oappe.top

[O04] 定义异步函数并等待
来源：http://kxf.gzhubu.top

Py:   async def f():⏎    await g()
来源：http://ugd.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cks.tian-w.cn

JS:   async function f() { await g(); }
来源：http://bpi.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cwv.fengsongda.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zmq.daxiang520.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hcl.yuanzhike.top

Ruby: # 用 Fiber 或 async gem
来源：http://ckm.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://hkx.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://wze.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://mpb.ywan-chungtsiang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hns.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://sou.zhoulong.xyz

TS:   await Promise.all(tasks)
来源：http://kfg.yfazqb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hzf.sweek.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aqx.yonumen.top

Ruby: threads.map(&:join)
来源：http://zsf.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xcp.zhoulong.xyz

[O06] 使用进程池
来源：http://xbe.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mqj.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ikf.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://ubi.jyoumei.cn

TS:   // child_process / cluster 模块
来源：http://fyg.xuanzx.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ajb.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vru.316326.xyz

Ruby: // fork 块
来源：http://pbk.andypj.xyz

C#:   Parallel.For
来源：http://vyd.nanxinkj.top

================================================================================
来源：http://nfj.nanxinkj.top

P. 常用工具函数
来源：http://yrj.birdmap.top

================================================================================
来源：http://akg.jinqigufen.top

[P01] 生成 UUID
来源：http://hqz.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://vwp.shangyingyoupin.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://khs.bbcook.cn

JS:   crypto.randomUUID()
来源：http://qlx.shanyushiyangtech.top

TS:   crypto.randomUUID()
来源：http://irr.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://hxr.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://ibj.cashguo.top

Ruby: SecureRandom.uuid
来源：http://yjc.yj20258.top

C#:   Guid.NewGuid().ToString()
来源：http://xpz.tarul.cn

[P02] MD5 / SHA256 摘要
来源：http://yhd.jqgfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://diu.ybcxt.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ylw.zhongyouzk.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://evc.xinyue.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wio.cqqwz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ewm.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nyb.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://unl.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://its.xuanzx.com

[P03] 生成短随机字符串
来源：http://jgv.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bnb.jqgufenzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ica.birdmap.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wkp.jinqigufen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dsw.redwolf501.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://now.zhoulong.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rik.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://akp.sjlbkw.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uil.zhengqikj.top

[P04] 求长度
来源：http://pbi.ydjk.org.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zmr.zycfv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yvk.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uau.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://irv.snrcjt.cn

Java: list.size();  map.size();  s.length()
来源：http://jdp.guowangkeji.top

Go:   len(arr);  len(m)
来源：http://gxf.shanyushiyangtech.top

Ruby: x.length;  x.size
来源：http://iql.nanxinkj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hbz.jqgfzy.top

[P05] 判断两个对象内容是否相等
来源：http://gpt.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vvp.c1oappe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lax.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mba.9152youxi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://efy.shangyingyoupin.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hjh.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://jay.bbcook.cn

Ruby: a == b
来源：http://xcv.hnqzz.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tio.sxryk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nkq.zhijiandao.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kal.birdmap.top

PHP:  if (empty($x)) {}
来源：http://uhi.chenjidiqi.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tke.yuanzhike.top

TS:   if (x == null) {}
来源：http://hcn.sufxvd.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kpl.havefunace.top

Go:   if x == nil {}
来源：http://nzh.sjlbkw.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bes.ivvv.top

C#:   if (x is null) {}
来源：http://yfi.fengsongda.top

[P07] 防抖与节流
来源：http://nzp.jyoumei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yfs.daria6918.cn

PHP:  // 手写时间戳比较
来源：http://ptp.ydjk.org.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qas.cashguo.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pfe.0kj1m.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rtk.dianchejie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rxo.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wuu.xuanzx.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rdz.fzhhl.top

[P08] 处理浮点精度问题
来源：http://pvu.guowangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://izk.dianchejie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pfj.jianghu66.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lsi.zhixingplan.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gte.316326.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gvn.hnxiangtu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qjq.jqgfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pkk.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jus.shangyingyoupin.top

================================================================================
来源：http://ssn.redwolf501.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xwu.ppjwa.cn

================================================================================
来源：http://fxa.yj20258888.top

[Q01] 创建表
来源：http://jgg.jqgfzy.top

CREATE TABLE users (
来源：http://wut.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fld.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://mim.feifeiyinyue.top

email VARCHAR(100) UNIQUE,
来源：http://mqb.wangshuangyany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xyg.ctjpmb.com

);
来源：http://akw.jqgfzy.top

[Q02] 创建带外键的表
来源：http://ama.nwbrower.top

CREATE TABLE orders (
来源：http://gro.meibo888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://awn.shanyushiyangkeji.top

user_id INT NOT NULL,
来源：http://yrw.yj20258.top

amount DECIMAL(10, 2),
来源：http://szc.jqgufenzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vup.snrcjt.cn

);
来源：http://owk.yj202588.top

[Q03] 增加列
来源：http://zyg.cashguo.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mrc.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://rdb.gzhubu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dor.ctjpmb.com

[Q05] 重命名列
来源：http://phu.sweek.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lgt.xziqi.cn

[Q06] 删除列
来源：http://srq.sxryk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gdb.shuidangran.top

[Q07] 删除表
来源：http://vgu.daxiang520.top

DROP TABLE IF EXISTS orders;
来源：http://gnb.sweek.top

[Q08] 创建普通索引
来源：http://qvo.nanxuanxn.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tjd.jqgfzy.top

[Q09] 创建唯一索引
来源：http://rch.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ehv.shzxlz.cn

[Q10] 插入单行
来源：http://fgi.haohaochexian.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nss.cdnleiting.top

[Q11] 一次插入多行
来源：http://xjd.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hol.yangfankeji.com

[Q12] 插入后取自增 ID
来源：http://aqu.ivvv.top

INSERT INTO users (name) VALUES ('C');
来源：http://iee.hysaishi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pkh.quarkkingdee.top

[Q13] 忽略重复插入
来源：http://oeq.yongpay.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xzr.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://sht.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eqs.ydzc1.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lel.ywan-chungtsiang.top

[Q15] 查询全部
来源：http://rwh.tianlin.xyz

SELECT * FROM users;
来源：http://vkt.smart0.xyz

[Q16] 查询指定列
来源：http://zfd.tarul.cn

SELECT id, name FROM users;
来源：http://gtu.ydjk.org.cn

[Q17] 条件查询
来源：http://rfu.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fam.jinqigfzy.top

[Q18] 模糊匹配
来源：http://one.tian-w.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qml.kuanghao11.cn

[Q19] 范围查询
来源：http://hss.cucudq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rzx.ivvv.top

[Q20] IN 列表
来源：http://mhw.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yiv.snrcjt.cn

[Q21] 空值判断
来源：http://nnd.316326.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://rkb.tanke756.top

[Q22] 排序
来源：http://noi.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ahb.iojbl.cn

[Q23] 分页
来源：http://zrs.pengpengdd.cyou

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fhz.yj20258888.top

[Q24] 去重
来源：http://nfs.xuetiantiany.cn

SELECT DISTINCT city FROM users;
来源：http://yxv.birdmap.top

[Q25] 只取前 N 条
来源：http://dmq.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://odc.birdmap.top

[Q26] 计数
来源：http://qgd.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://jox.hongshengwenyu.top

[Q27] 条件计数
来源：http://mcv.ybcxt.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vow.9152youxi.cn

[Q28] 求和与平均
来源：http://pkg.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ucb.jinghuilouyu.cn

[Q29] 最大最小值
来源：http://zxa.zhixingplan.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cqt.gzhubu.top

[Q30] 分组统计
来源：http://hyf.yongpay.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hjp.chenlongwang.top

[Q31] 分组后过滤
来源：http://sjf.sjlbkw.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://luh.daria6918.cn

[Q32] 分组拼接字符串
来源：http://kzg.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qel.hywenlv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fmi.meibo888.top

[Q33] 多列分组
来源：http://pgp.ppjwa.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vrj.pycfn.com

[Q34] 每组取第一条
来源：http://pgj.bbcook.cn

SELECT * FROM (
来源：http://bec.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ugd.shangyingyoupin.top

) t WHERE rn = 1;
来源：http://xzn.316326.xyz

[Q35] 内连接
来源：http://xbi.xuetiantiany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://znq.yuanzhike.top

[Q36] 左连接
来源：http://qbn.zhixingplan.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ulp.chenlongwang.top

[Q37] 右连接
来源：http://ycv.sxryk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qbt.tianlin.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://dss.jianghu66.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vtm.yfazqb.com

[Q39] 自连接（查上下级）
来源：http://kyc.jinqigfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mfx.havefunace.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zaj.jinyuanbaomall.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zqi.jqgufenzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wwk.uphjek.com

[Q41] 多表连接
来源：http://vnz.epnwcf.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://bfb.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://ozf.aizwys.cn

JOIN products p ON p.id = o.product_id;
来源：http://skf.chenlongwang.top

[Q42] 连接条件附加过滤
来源：http://yxh.tian-w.cn

SELECT u.name, o.amount FROM users u
来源：http://bfp.zdbjq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jga.yj20258.top

[Q43] 标量子查询
来源：http://gtv.aibaodan.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://azr.xinyue.icu

[Q44] IN 子查询
来源：http://ewr.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://njt.yj20258.top

[Q45] EXISTS 判断存在
来源：http://dkx.bbcook.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mql.yongpay.top

[Q46] NOT EXISTS 判断不存在
来源：http://pbc.wangdashe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://khx.uphjek.com

[Q47] 与平均值比较
来源：http://ftx.jinqigfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xic.sxryk.cn

[Q48] CTE 公用表表达式
来源：http://qch.svipenyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kfy.svipenyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://dmp.kuanghao11.cn

[Q49] 更新单行
来源：http://eex.gaohongyu789.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jza.sjlbkw.cn

[Q50] 批量更新
来源：http://jeu.vehdjk.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dao.yangfankeji.com

[Q51] 用子查询更新
来源：http://pxw.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kid.vqdsnc.cn

[Q52] 删除指定行
来源：http://hle.yongpay.top

DELETE FROM users WHERE id = 10;
来源：http://ctd.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://tin.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kfe.hesvh.cn

[Q54] 清空表
来源：http://fmg.cqqwz.cn

TRUNCATE TABLE logs;
来源：http://kxz.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://ogx.yanxiufei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nkq.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://oly.hesvh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kug.zhaomingkeji.xyz

[Q57] 行号
来源：http://jmx.zhaomingkeji.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lfm.kuanghao11.cn

[Q58] 累计求和
来源：http://msn.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vhe.xuetiantiany.cn

[Q59] 分组内累计
来源：http://mpz.tianlin.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mhk.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://uut.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kwc.52xcode.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://epf.jianghu66.top

[Q61] 移动平均
来源：http://tqh.bbcook.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qhk.yj20258888.top

[Q62] 分组占比
来源：http://hfp.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://buo.gzhubu.top

[Q63] 开启事务
来源：http://uxz.daria6918.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bqs.sufxvd.cn

[Q64] 提交事务
来源：http://prk.chenzaomai.com

COMMIT;
来源：http://qol.yj20258888.top


<!-- 参考信息 -->