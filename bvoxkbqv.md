代发 wailian999

PHP:  // 手写递归函数
来源：http://fwz.hnxiangtu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ipb.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://psd.smart0.xyz

Java: // 手写递归
来源：http://yxz.shuidangran.top

Go:   // 手写递归
来源：http://tgp.smart0.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bsg.wangdashe.top

C#:   // 手写递归
来源：http://gzv.wangshuangyany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://joo.nanxinkj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ugt.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wdm.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kai.ywan-chungtsiang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jqt.feifeiyinyue.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://avq.chenjidiqi.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wbc.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mdu.aibaodan.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ctz.zhoulong.xyz

================================================================================
来源：http://inc.tarul.cn

O. 并发与异步
来源：http://bqr.aibaodan.cn

================================================================================
来源：http://rwa.tianlin.xyz

[O01] 启动一个线程
来源：http://pll.chenzaomai.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lvq.zhoulong.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fei.chenzaomai.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fja.hfpthk.cn

TS:   // 同 JS
来源：http://der.hnqzz.top

Java: new Thread(() -> f()).start()
来源：http://vbb.jqgufenzy.top

Go:   go f()
来源：http://iah.meibo888.top

Ruby: Thread.new { f }
来源：http://zyt.tianlin.xyz

C#:   Task.Run(() => F());
来源：http://tax.zycfv.cn

[O02] 使用线程池
来源：http://ygl.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pnn.zhiwuduotai.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dmn.nwbrower.top

JS:   // worker_threads 线程池
来源：http://guw.jqgufenzy.top

TS:   // worker_threads 线程池
来源：http://wct.zdbjq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ykm.zhengqikj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ehl.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rot.nanxuanxn.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gxy.yj20258888.top

[O03] 加锁保护共享数据
来源：http://uyp.svipenyu.cn

Py:   with lock: shared += 1
来源：http://kwv.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://lox.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://svq.guowangkeji.top

TS:   // 同 JS
来源：http://ilb.ppjwa.cn

Java: synchronized (this) { shared++; }
来源：http://hxz.jlsjyb.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://act.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://twy.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://ktl.jinghuilouyu.cn

[O04] 定义异步函数并等待
来源：http://lsw.bbcook.cn

Py:   async def f():⏎    await g()
来源：http://anv.yanxiufei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://toe.epnwcf.com

JS:   async function f() { await g(); }
来源：http://znv.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kbs.mhx1999.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cmd.snrcjt.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yif.guowangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://iom.yangfankeji.com

C#:   async Task F() { await G(); }
来源：http://cnp.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://wrz.birdmap.top

Py:   asyncio.gather(*tasks)
来源：http://ify.pycfn.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sly.tianlin.xyz

JS:   await Promise.all(tasks)
来源：http://fop.daria6918.cn

TS:   await Promise.all(tasks)
来源：http://hdn.ivvv.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bsn.quarkkingdee.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gfw.aibaodan.cn

Ruby: threads.map(&:join)
来源：http://cnf.bjfxy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hmb.wangshuangyany.cn

[O06] 使用进程池
来源：http://wcv.epnwcf.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://grp.jyoumei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://obi.hongshengwenyu.top

JS:   // child_process / cluster 模块
来源：http://fkm.shanyushiyangtech.top

TS:   // child_process / cluster 模块
来源：http://tde.vehdjk.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fig.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vqk.quarkkingdee.top

Ruby: // fork 块
来源：http://lji.kuanghao11.cn

C#:   Parallel.For
来源：http://dhk.gotoacloud.top

================================================================================
来源：http://apc.uphjek.com

P. 常用工具函数
来源：http://lad.jqgfzy.top

================================================================================
来源：http://gel.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://sya.zhongyouzk.top

Py:   str(uuid.uuid4())
来源：http://oqt.hywenlv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pkg.havefunace.top

JS:   crypto.randomUUID()
来源：http://irn.9152youxi.cn

TS:   crypto.randomUUID()
来源：http://tlk.yvedp.cn

Java: UUID.randomUUID().toString()
来源：http://utm.yueranfly.top

Go:   // 用 github.com/google/uuid
来源：http://wmj.sweek.top

Ruby: SecureRandom.uuid
来源：http://irs.fanxiaobao.xyz

C#:   Guid.NewGuid().ToString()
来源：http://mfz.hongshengwenyu.top

[P02] MD5 / SHA256 摘要
来源：http://kpd.birdmap.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tyz.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://rzc.xinyue.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aes.fzhhl.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vtb.zhiwuduotai.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eae.snrcjt.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dwv.xinyue.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://msd.tanke756.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kem.nanxinkj.top

[P03] 生成短随机字符串
来源：http://mxm.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yyy.hysaishi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wic.aizwys.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mzu.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://faq.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ecy.jqgfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://obl.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vfm.xuanzx.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nub.nanxinkj.top

[P04] 求长度
来源：http://urq.gotoacloud.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qxp.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rob.meibo888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://umv.guowangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rgu.nanxinkj.top

Java: list.size();  map.size();  s.length()
来源：http://beo.fengsongda.top

Go:   len(arr);  len(m)
来源：http://hoz.jinqigfzy.top

Ruby: x.length;  x.size
来源：http://zgg.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zvq.feifeiyinyue.top

[P05] 判断两个对象内容是否相等
来源：http://utg.smart0.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://jcm.cqqwz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ktw.xingfuxueyuan.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nys.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://udw.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mkx.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://tjr.iojbl.cn

Ruby: a == b
来源：http://pic.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kcp.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://esp.nanxuanxn.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://evs.birdmap.top

PHP:  if (empty($x)) {}
来源：http://xdy.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bmn.snrcjt.cn

TS:   if (x == null) {}
来源：http://cja.zhijiandao.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lgp.uphjek.com

Go:   if x == nil {}
来源：http://puu.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://azs.shangyingyoupin.top

C#:   if (x is null) {}
来源：http://tzt.316326.xyz

[P07] 防抖与节流
来源：http://yxh.316326.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ycw.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://oxb.yueranfly.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cvj.ydjk.org.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ujw.haohaochexian.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jfk.fehbvm.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zds.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://oyq.cashguo.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rrn.jyoumei.cn

[P08] 处理浮点精度问题
来源：http://pmz.xziqi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bbz.zycfv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gdy.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mfu.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ifs.hongshengwenyu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ysl.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vwp.hnqzz.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ylj.zdqjudy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://afs.gotoacloud.top

================================================================================
来源：http://cds.sjlbkw.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hmc.hnxiangtu.top

================================================================================
来源：http://kbr.sxryk.cn

[Q01] 创建表
来源：http://wxy.ydzc1.top

CREATE TABLE users (
来源：http://jwc.gaohongyu789.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jqz.hcnkem.com

name VARCHAR(50) NOT NULL,
来源：http://okr.ydzc1.top

email VARCHAR(100) UNIQUE,
来源：http://pdw.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hnu.hysaishi.cn

);
来源：http://pbe.ydzc1.top

[Q02] 创建带外键的表
来源：http://dtx.bjfxy.top

CREATE TABLE orders (
来源：http://oif.tanke756.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nfv.vqdsnc.cn

user_id INT NOT NULL,
来源：http://baj.zhoulong.xyz

amount DECIMAL(10, 2),
来源：http://tlr.zhongyouzk.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://etq.yj20258.top

);
来源：http://xjv.nanxuanxn.top

[Q03] 增加列
来源：http://qrb.ctjpmb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ijw.cqqwz.cn

[Q04] 修改列类型
来源：http://zeu.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://asw.guowangkeji.top

[Q05] 重命名列
来源：http://jrd.yj202588.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hcz.zhijiandao.cn

[Q06] 删除列
来源：http://qtg.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://cyl.zhengqikj.top

[Q07] 删除表
来源：http://can.daxiang520.top

DROP TABLE IF EXISTS orders;
来源：http://fhq.zhongyouzk.top

[Q08] 创建普通索引
来源：http://wko.yj20258.top

CREATE INDEX idx_users_email ON users(email);
来源：http://noi.tanke756.top

[Q09] 创建唯一索引
来源：http://ncp.hnqzz.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rlw.zhaomingkeji.xyz

[Q10] 插入单行
来源：http://zro.fengsongda.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mpp.kuanghao11.cn

[Q11] 一次插入多行
来源：http://kmv.zhixingplan.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yjo.fehbvm.com

[Q12] 插入后取自增 ID
来源：http://qnh.ivvv.top

INSERT INTO users (name) VALUES ('C');
来源：http://ynq.zycfv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://puq.cucudq.cn

[Q13] 忽略重复插入
来源：http://wob.chenjidiqi.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://epb.svipenyu.cn

[Q14] 存在则更新（upsert）
来源：http://ufq.tianlin.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eyp.sjlbkw.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fkt.mhx1999.top

[Q15] 查询全部
来源：http://pxg.hongshengwenyu.top

SELECT * FROM users;
来源：http://oaf.jiagoushi.top

[Q16] 查询指定列
来源：http://fwe.cqqwz.cn

SELECT id, name FROM users;
来源：http://pef.bbcook.cn

[Q17] 条件查询
来源：http://svz.birdmap.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cqe.shzxlz.cn

[Q18] 模糊匹配
来源：http://qub.xziqi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rmn.quarkkingdee.top

[Q19] 范围查询
来源：http://dmz.yuanzhike.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pwt.316326.xyz

[Q20] IN 列表
来源：http://ris.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kvj.aizwys.cn

[Q21] 空值判断
来源：http://gwe.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pog.shangyingyoupin.top

[Q22] 排序
来源：http://dtk.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cdm.nwbrower.top

[Q23] 分页
来源：http://qxz.aizwys.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xtr.ehwqpu.com

[Q24] 去重
来源：http://zgl.xuetiantiany.cn

SELECT DISTINCT city FROM users;
来源：http://qwl.jianghu66.top

[Q25] 只取前 N 条
来源：http://ata.xinyue.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eer.sweek.top

[Q26] 计数
来源：http://lwd.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://jko.yj20258888.top

[Q27] 条件计数
来源：http://tnf.hywenlv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rrn.xuetiantiany.cn

[Q28] 求和与平均
来源：http://mvr.yanxiufei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://obd.zhongyouzk.top

[Q29] 最大最小值
来源：http://ehk.nanxuanxn.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hkt.dianchejie.cn

[Q30] 分组统计
来源：http://jzc.zhijiandao.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ekg.fzhhl.top

[Q31] 分组后过滤
来源：http://vry.sweek.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kvt.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://ylc.hysaishi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zts.yuanzhike.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ahh.zhoulong.xyz

[Q33] 多列分组
来源：http://yja.uphjek.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://krd.gotoacloud.top

[Q34] 每组取第一条
来源：http://hfw.nanxuanxn.top

SELECT * FROM (
来源：http://vxc.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nwv.jinqigufen.top

) t WHERE rn = 1;
来源：http://nuz.meibo888.top

[Q35] 内连接
来源：http://owf.cheryme.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bqk.cqqwz.cn

[Q36] 左连接
来源：http://mft.kuanghao11.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xyy.uphjek.com

[Q37] 右连接
来源：http://wkl.daxiang520.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://deh.yj202588.top

[Q38] 全外连接（PostgreSQL）
来源：http://tsj.c1oappe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cmv.shangyingyoupin.top

[Q39] 自连接（查上下级）
来源：http://ojn.jyoumei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mag.chenjidiqi.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wez.tanke756.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ejv.zhongyouzk.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xok.jianghu66.top

[Q41] 多表连接
来源：http://mec.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yki.meibo888.top

JOIN users u ON u.id = o.user_id
来源：http://rjm.ydjk.org.cn

JOIN products p ON p.id = o.product_id;
来源：http://iyr.hfpthk.cn

[Q42] 连接条件附加过滤
来源：http://tcj.tianlin.xyz

SELECT u.name, o.amount FROM users u
来源：http://gkd.guannengcc.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iin.iojbl.cn

[Q43] 标量子查询
来源：http://flo.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kda.cheryme.top

[Q44] IN 子查询
来源：http://lwu.zdbjq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dqa.cashguo.top

[Q45] EXISTS 判断存在
来源：http://lax.svipenyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bfm.sysykeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://dzf.aibaodan.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zoa.zhengqikj.top

[Q47] 与平均值比较
来源：http://ywo.tanke756.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kfz.vehdjk.com

[Q48] CTE 公用表表达式
来源：http://rhp.jqgfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sgs.daxiang520.top

SELECT * FROM t WHERE c > 5;
来源：http://kld.xinyue.icu

[Q49] 更新单行
来源：http://sva.zhoulong.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pcp.wangshuangyany.cn

[Q50] 批量更新
来源：http://oyn.shanyushiyangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://khx.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://yse.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qpb.cqqwz.cn

[Q52] 删除指定行
来源：http://rzz.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://cwo.jinqigfzy.top

[Q53] 按条件删除
来源：http://wzi.kuanghao11.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://thm.bjfxy.top

[Q54] 清空表
来源：http://pub.guannengcc.top

TRUNCATE TABLE logs;
来源：http://ywy.tian-w.cn

[Q55] 排名（并列占位）
来源：http://xkk.xingfuxueyuan.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jdc.xuetiantiany.cn

[Q56] 密集排名（并列不占位）
来源：http://gdg.sxryk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cuv.yanxiufei.cn

[Q57] 行号
来源：http://uyw.gaohongyu789.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jta.ydzc1.top

[Q58] 累计求和
来源：http://cws.guannengcc.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ete.sjlbkw.cn

[Q59] 分组内累计
来源：http://maw.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://agy.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://aqu.zdqjudy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://grt.ehwqpu.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://flz.cashguo.top

[Q61] 移动平均
来源：http://pkw.sweek.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fwy.xuetiantiany.cn

[Q62] 分组占比
来源：http://esg.hfpthk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gmc.zdbjq.cn

[Q63] 开启事务
来源：http://ljq.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jmm.zhengqikj.top

[Q64] 提交事务
来源：http://lgn.vqdsnc.cn

COMMIT;
来源：http://llz.uphjek.com


<!-- 参考信息 -->