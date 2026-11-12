代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://phw.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://auy.yangfankeji.com

Java: class Node { int v; Node next; }
来源：http://shc.shzxlz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ghl.iojbl.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kvm.nwbrower.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pcx.zhiwuduotai.top

[N11] 二叉树中序遍历
来源：http://dyf.yangfankeji.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ohq.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://nbr.nwbrower.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bed.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cce.zhaomingkeji.xyz

Java: // 手写递归
来源：http://fep.smart0.xyz

Go:   // 手写递归
来源：http://aui.daria6918.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dhi.hesvh.cn

C#:   // 手写递归
来源：http://hhn.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://grm.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tev.quarkkingdee.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zmf.tanke756.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ljx.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ccy.daxiang520.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qow.ywan-chungtsiang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gya.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://shp.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rhj.ydjk.org.cn

================================================================================
来源：http://vlm.ywan-chungtsiang.top

O. 并发与异步
来源：http://vpe.fanxiaobao.xyz

================================================================================
来源：http://xye.birdmap.top

[O01] 启动一个线程
来源：http://duw.svipenyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lko.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mde.zycfv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jsi.tanke756.top

TS:   // 同 JS
来源：http://kml.epnwcf.com

Java: new Thread(() -> f()).start()
来源：http://vni.jlsjyb.cn

Go:   go f()
来源：http://dxz.yvedp.cn

Ruby: Thread.new { f }
来源：http://jox.havefunace.top

C#:   Task.Run(() => F());
来源：http://rrg.guannengcc.top

[O02] 使用线程池
来源：http://suk.vehdjk.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ext.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nyn.yongpay.top

JS:   // worker_threads 线程池
来源：http://igs.0kj1m.cn

TS:   // worker_threads 线程池
来源：http://bih.cheryme.top

Java: Executors.newFixedThreadPool(4)
来源：http://sxh.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kas.0kj1m.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wjk.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nam.birdmap.top

[O03] 加锁保护共享数据
来源：http://skk.birdmap.top

Py:   with lock: shared += 1
来源：http://uco.yj20258888.top

PHP:  // 用 flock() 做文件锁
来源：http://blx.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eoe.jiagoushi.top

TS:   // 同 JS
来源：http://ijx.aibaodan.cn

Java: synchronized (this) { shared++; }
来源：http://ayd.xinyue.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vsj.ydzc1.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://azz.jqgufenzy.top

C#:   lock (gate) { shared++; }
来源：http://rra.zhixingplan.top

[O04] 定义异步函数并等待
来源：http://kjz.hysaishi.cn

Py:   async def f():⏎    await g()
来源：http://mov.cqqwz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://can.ehwqpu.com

JS:   async function f() { await g(); }
来源：http://arl.316326.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://ili.nanxinkj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pyj.ehwqpu.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://skp.zhiwuduotai.top

Ruby: # 用 Fiber 或 async gem
来源：http://htu.nwbrower.top

C#:   async Task F() { await G(); }
来源：http://ugi.zhengqikj.top

[O05] 并发执行并等待全部完成
来源：http://lhg.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://oos.cashguo.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kmf.aibaodan.cn

JS:   await Promise.all(tasks)
来源：http://kkn.yonumen.top

TS:   await Promise.all(tasks)
来源：http://kre.snrcjt.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qiq.nanxuanxn.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jve.dashuyun.cn

Ruby: threads.map(&:join)
来源：http://mro.wangshuangyany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cpm.nwbrower.top

[O06] 使用进程池
来源：http://fgy.nanxuanxn.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ibb.shanyushiyangtech.top

PHP:  // pcntl_fork 或多进程队列
来源：http://azw.svipenyu.cn

JS:   // child_process / cluster 模块
来源：http://urq.shanyushiyangtech.top

TS:   // child_process / cluster 模块
来源：http://oon.haohaochexian.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hif.wangshuangyany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kjm.epnwcf.com

Ruby: // fork 块
来源：http://jmh.0kj1m.cn

C#:   Parallel.For
来源：http://rzf.sweek.top

================================================================================
来源：http://suh.ctjpmb.com

P. 常用工具函数
来源：http://vdt.aibaodan.cn

================================================================================
来源：http://fic.yuxming.cn

[P01] 生成 UUID
来源：http://dax.xuanzx.com

Py:   str(uuid.uuid4())
来源：http://pvg.feifeiyinyue.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lul.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://syr.hysaishi.cn

TS:   crypto.randomUUID()
来源：http://egh.ivvv.top

Java: UUID.randomUUID().toString()
来源：http://udk.daria6918.cn

Go:   // 用 github.com/google/uuid
来源：http://icy.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://aak.zdqjudy.top

C#:   Guid.NewGuid().ToString()
来源：http://aem.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://qfe.redwolf501.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vjc.cqqwz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kbn.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ivt.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dja.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rlc.cdnleiting.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xxq.316326.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sax.zhongyouzk.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qbm.yfazqb.com

[P03] 生成短随机字符串
来源：http://pnx.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ldz.hongshengwenyu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fcd.yueranfly.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://znf.nwbrower.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ekd.ehwqpu.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fda.chenjidiqi.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lcq.jqgufenzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bcw.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cqe.fengsongda.top

[P04] 求长度
来源：http://bup.jyoumei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hjz.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xzp.zhongyouzk.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://chr.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sip.iojbl.cn

Java: list.size();  map.size();  s.length()
来源：http://buz.vqdsnc.cn

Go:   len(arr);  len(m)
来源：http://aaz.andypj.xyz

Ruby: x.length;  x.size
来源：http://qrk.vqdsnc.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bbb.xuetiantiany.cn

[P05] 判断两个对象内容是否相等
来源：http://ayz.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kmn.ywan-chungtsiang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jti.zhiwuduotai.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ycm.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lfk.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://plr.pengpengdd.cyou

Go:   reflect.DeepEqual(a, b)
来源：http://fhj.gaohongyu789.top

Ruby: a == b
来源：http://xbs.jinghuilouyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://miz.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://slw.cqqwz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jln.zhaomingkeji.xyz

PHP:  if (empty($x)) {}
来源：http://dap.nanxuanxn.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fbf.yongpay.top

TS:   if (x == null) {}
来源：http://eqe.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://wsm.jianghu66.top

Go:   if x == nil {}
来源：http://vzf.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://icr.ctjpmb.com

C#:   if (x is null) {}
来源：http://sgq.tanke756.top

[P07] 防抖与节流
来源：http://qld.sxryk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fqb.ppjwa.cn

PHP:  // 手写时间戳比较
来源：http://myk.jinyuanbaomall.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rwq.chenjidiqi.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://his.316326.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oze.guannengcc.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dwq.hesvh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ggg.zhengqikj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rqn.ybcxt.top

[P08] 处理浮点精度问题
来源：http://cux.aibaodan.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ahc.c1oappe.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ofd.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nuk.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ulh.jinqigfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ymh.birdmap.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://apa.hesvh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eyx.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hqb.haohaochexian.top

================================================================================
来源：http://six.sjlbkw.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dvf.nanxuanxn.top

================================================================================
来源：http://xlw.cucudq.cn

[Q01] 创建表
来源：http://cin.gotoacloud.top

CREATE TABLE users (
来源：http://vqu.zhijiandao.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jnq.tian-w.cn

name VARCHAR(50) NOT NULL,
来源：http://cux.chenlongwang.top

email VARCHAR(100) UNIQUE,
来源：http://kkx.nwbrower.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bkg.ydzc1.top

);
来源：http://wbk.smart0.xyz

[Q02] 创建带外键的表
来源：http://esz.jqgfzy.top

CREATE TABLE orders (
来源：http://euy.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bti.c1oappe.top

user_id INT NOT NULL,
来源：http://aed.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://qcy.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nqu.jinyuanbaomall.cn

);
来源：http://gzq.jyoumei.cn

[Q03] 增加列
来源：http://tpu.xuanzx.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iae.shanyushiyangtech.top

[Q04] 修改列类型
来源：http://tao.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tjq.yj20258888.top

[Q05] 重命名列
来源：http://cks.xylfe.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cii.sxryk.cn

[Q06] 删除列
来源：http://qhv.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://vbt.gzhubu.top

[Q07] 删除表
来源：http://yve.zhijiandao.cn

DROP TABLE IF EXISTS orders;
来源：http://kvi.snrcjt.cn

[Q08] 创建普通索引
来源：http://eqc.chenlongwang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bif.cashguo.top

[Q09] 创建唯一索引
来源：http://apd.yanxiufei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dlm.tian-w.cn

[Q10] 插入单行
来源：http://itt.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bir.tianlin.xyz

[Q11] 一次插入多行
来源：http://jxy.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tny.sxryk.cn

[Q12] 插入后取自增 ID
来源：http://tpd.gzhubu.top

INSERT INTO users (name) VALUES ('C');
来源：http://guu.wangdashe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://emf.ydjk.org.cn

[Q13] 忽略重复插入
来源：http://uui.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qzg.jyoumei.cn

[Q14] 存在则更新（upsert）
来源：http://adf.gotoacloud.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jxk.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lwd.ydzc1.top

[Q15] 查询全部
来源：http://eyv.hfpthk.cn

SELECT * FROM users;
来源：http://cyj.hnqzz.top

[Q16] 查询指定列
来源：http://lnm.jinyuanbaomall.cn

SELECT id, name FROM users;
来源：http://ieq.fzhhl.top

[Q17] 条件查询
来源：http://bfq.nanxuanxn.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pkw.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://jig.zhoulong.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ghf.yuanzhike.top

[Q19] 范围查询
来源：http://ufh.yonumen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bsh.sysykeji.top

[Q20] IN 列表
来源：http://mia.ydzc1.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mqe.tarul.cn

[Q21] 空值判断
来源：http://bzr.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://poq.gzhubu.top

[Q22] 排序
来源：http://rqv.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wij.yvedp.cn

[Q23] 分页
来源：http://vqo.jinqigfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tyt.jianghu66.top

[Q24] 去重
来源：http://pon.jinghuilouyu.cn

SELECT DISTINCT city FROM users;
来源：http://kdv.yfazqb.com

[Q25] 只取前 N 条
来源：http://qxg.quarkkingdee.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zif.jinyuanbaomall.cn

[Q26] 计数
来源：http://joc.xuetiantiany.cn

SELECT COUNT(*) FROM users;
来源：http://yzz.wangshuangyany.cn

[Q27] 条件计数
来源：http://thd.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rii.quarkkingdee.top

[Q28] 求和与平均
来源：http://sth.shuidangran.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zwa.sjlbkw.cn

[Q29] 最大最小值
来源：http://sns.hesvh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ool.ivvv.top

[Q30] 分组统计
来源：http://brz.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rka.gogol.net.cn

[Q31] 分组后过滤
来源：http://wvc.dashuyun.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hvn.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://vnr.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tdv.redwolf501.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://scn.epnwcf.com

[Q33] 多列分组
来源：http://qnq.zycfv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://imt.yvedp.cn

[Q34] 每组取第一条
来源：http://zad.shangyingyoupin.top

SELECT * FROM (
来源：http://kmu.hesvh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fsy.ctjpmb.com

) t WHERE rn = 1;
来源：http://kyy.ivvv.top

[Q35] 内连接
来源：http://sji.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tpf.aibaodan.cn

[Q36] 左连接
来源：http://dfr.sysykeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wve.tanke756.top

[Q37] 右连接
来源：http://ffi.birdmap.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uoh.wangdashe.top

[Q38] 全外连接（PostgreSQL）
来源：http://dnl.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vim.pycfn.com

[Q39] 自连接（查上下级）
来源：http://gzj.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://pml.fanxiaobao.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yce.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xai.316326.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rnj.9152youxi.cn

[Q41] 多表连接
来源：http://avn.shuidangran.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://oyh.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://bjj.jiagoushi.top

JOIN products p ON p.id = o.product_id;
来源：http://lhe.hammf.cn

[Q42] 连接条件附加过滤
来源：http://qfk.zhoulong.xyz

SELECT u.name, o.amount FROM users u
来源：http://zyt.jyoumei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lci.birdmap.top

[Q43] 标量子查询
来源：http://euo.hywenlv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://muc.snrcjt.cn

[Q44] IN 子查询
来源：http://tmn.fzhhl.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xwr.sweek.top

[Q45] EXISTS 判断存在
来源：http://eqm.ctjpmb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xne.c1oappe.top

[Q46] NOT EXISTS 判断不存在
来源：http://ary.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://srt.hysaishi.cn

[Q47] 与平均值比较
来源：http://rmn.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pqa.yonumen.top

[Q48] CTE 公用表表达式
来源：http://gyw.vehdjk.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uzw.epnwcf.com

SELECT * FROM t WHERE c > 5;
来源：http://sta.nanxuanxn.top

[Q49] 更新单行
来源：http://hme.hcnkem.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ato.hcnkem.com

[Q50] 批量更新
来源：http://gdf.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eem.tianlin.xyz

[Q51] 用子查询更新
来源：http://mey.jinghuilouyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uvo.sufxvd.cn

[Q52] 删除指定行
来源：http://kcc.redwolf501.top

DELETE FROM users WHERE id = 10;
来源：http://pfh.snrcjt.cn

[Q53] 按条件删除
来源：http://ukn.vehdjk.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cun.yuanzhike.top

[Q54] 清空表
来源：http://yyo.zhaomingkeji.xyz

TRUNCATE TABLE logs;
来源：http://ugn.yj20258888.top

[Q55] 排名（并列占位）
来源：http://xpu.shuidangran.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://utk.xziqi.cn

[Q56] 密集排名（并列不占位）
来源：http://tmv.jinghuilouyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bho.shangyingyoupin.top

[Q57] 行号
来源：http://gmo.nanxuanxn.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rkg.aibaodan.cn

[Q58] 累计求和
来源：http://dfn.52xcode.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bxj.shzxlz.cn

[Q59] 分组内累计
来源：http://kzh.tanke756.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fwy.xuetiantiany.cn

[Q60] 取上一行 / 下一行
来源：http://ebb.sxryk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pcf.ehwqpu.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dyx.zhaomingkeji.xyz


<!-- 参考信息 -->