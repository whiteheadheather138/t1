代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tjd.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tpc.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://tsj.gotoacloud.top

Go:   type Node struct { V int; Next *Node }
来源：http://wdx.jiagoushi.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jvp.jinyuanbaomall.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://iov.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://gen.tarul.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fbp.meibo888.top

PHP:  // 手写递归函数
来源：http://gix.yj20258888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://snj.smart0.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://waa.epnwcf.com

Java: // 手写递归
来源：http://bvc.ivvv.top

Go:   // 手写递归
来源：http://alv.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nrq.9152youxi.cn

C#:   // 手写递归
来源：http://cww.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uef.jiagoushi.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oyh.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://egf.9152youxi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pcf.0kj1m.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ybq.yongpay.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://buk.9152youxi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jgu.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yki.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eiw.redwolf501.top

================================================================================
来源：http://lcj.ehwqpu.com

O. 并发与异步
来源：http://jfw.nanxuanxn.top

================================================================================
来源：http://xoc.316326.xyz

[O01] 启动一个线程
来源：http://vnn.shanyushiyangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hps.yuanzhike.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wit.fzhhl.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wtb.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://cwm.vqdsnc.cn

Java: new Thread(() -> f()).start()
来源：http://gyb.ctjpmb.com

Go:   go f()
来源：http://qnw.epnwcf.com

Ruby: Thread.new { f }
来源：http://cev.hnqzz.top

C#:   Task.Run(() => F());
来源：http://uvf.hfpthk.cn

[O02] 使用线程池
来源：http://bzd.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nhk.bbcook.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bdi.hongshengwenyu.top

JS:   // worker_threads 线程池
来源：http://rqt.tarul.cn

TS:   // worker_threads 线程池
来源：http://bti.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://tfq.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://grw.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ddm.nanxuanxn.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://imr.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://muw.vqdsnc.cn

Py:   with lock: shared += 1
来源：http://krb.yuxming.cn

PHP:  // 用 flock() 做文件锁
来源：http://maq.haohaochexian.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://beq.tianlin.xyz

TS:   // 同 JS
来源：http://elv.jiagoushi.top

Java: synchronized (this) { shared++; }
来源：http://oey.jlsjyb.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gjr.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gzx.jinqigfzy.top

C#:   lock (gate) { shared++; }
来源：http://krk.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://kvv.shanyushiyangtech.top

Py:   async def f():⏎    await g()
来源：http://bmb.52xcode.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xla.vehdjk.com

JS:   async function f() { await g(); }
来源：http://ifp.svipenyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kqa.hammf.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pvt.fktsv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zcw.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://gfr.quarkkingdee.top

C#:   async Task F() { await G(); }
来源：http://hpn.316326.xyz

[O05] 并发执行并等待全部完成
来源：http://hza.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://vpo.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nly.yongpay.top

JS:   await Promise.all(tasks)
来源：http://kgj.zhaomingkeji.xyz

TS:   await Promise.all(tasks)
来源：http://jwp.yonumen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qno.yvedp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sbd.guannengcc.top

Ruby: threads.map(&:join)
来源：http://bcx.zhaomingkeji.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://egl.zdbjq.cn

[O06] 使用进程池
来源：http://suq.yanxiufei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ccd.gogol.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cyg.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://sfu.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://dcg.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://npz.jinqigufen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://php.fanxiaobao.xyz

Ruby: // fork 块
来源：http://vzp.ivvv.top

C#:   Parallel.For
来源：http://oah.xuanzx.com

================================================================================
来源：http://cln.yj202588.top

P. 常用工具函数
来源：http://uta.hcnkem.com

================================================================================
来源：http://nqn.zhoulong.xyz

[P01] 生成 UUID
来源：http://dzx.cucudq.cn

Py:   str(uuid.uuid4())
来源：http://ssj.tarul.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qcf.zhongyouzk.top

JS:   crypto.randomUUID()
来源：http://hqv.yangfankeji.com

TS:   crypto.randomUUID()
来源：http://bno.bbcook.cn

Java: UUID.randomUUID().toString()
来源：http://fly.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://tsx.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://xjl.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://rkg.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://yrv.zhengqikj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ldr.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ayv.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cvl.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xre.hysaishi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pfs.ehwqpu.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mxo.fengsongda.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fhw.meibo888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oti.daria6918.cn

[P03] 生成短随机字符串
来源：http://onn.zhengqikj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://amm.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ixj.vehdjk.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uyi.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nvk.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://veq.wangshuangyany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rpo.dianchejie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vpt.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tkf.yj202588.top

[P04] 求长度
来源：http://cmy.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bvd.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wxf.jqgfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://owq.smart0.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://syk.ehwqpu.com

Java: list.size();  map.size();  s.length()
来源：http://lxe.hongshengwenyu.top

Go:   len(arr);  len(m)
来源：http://fot.ivvv.top

Ruby: x.length;  x.size
来源：http://laj.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://eep.fanxiaobao.xyz

[P05] 判断两个对象内容是否相等
来源：http://axu.xziqi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nrx.uphjek.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ioo.shangyingyoupin.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zve.sweek.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fiz.meibo888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kvy.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xgj.dashuyun.cn

Ruby: a == b
来源：http://xkm.kuanghao11.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aft.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hgg.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gaz.haohaochexian.top

PHP:  if (empty($x)) {}
来源：http://usp.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wef.dashuyun.cn

TS:   if (x == null) {}
来源：http://bph.shangyingyoupin.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pby.meibo888.top

Go:   if x == nil {}
来源：http://xwd.fanxiaobao.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ebt.chenlongwang.top

C#:   if (x is null) {}
来源：http://wkh.gzhubu.top

[P07] 防抖与节流
来源：http://hfd.yueranfly.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qrt.zhijiandao.cn

PHP:  // 手写时间戳比较
来源：http://ujh.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://znu.fengsongda.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ovk.svipenyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jfx.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rsr.shuidangran.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fyg.ppjwa.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://otp.zycfv.cn

[P08] 处理浮点精度问题
来源：http://erc.jyoumei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tle.xingfuxueyuan.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://smv.hfpthk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jkp.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://azm.hfpthk.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://woh.iojbl.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vxb.zhixingplan.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rse.snrcjt.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kfd.zhijiandao.cn

================================================================================
来源：http://fvb.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kmk.yj20258.top

================================================================================
来源：http://btv.52xcode.cn

[Q01] 创建表
来源：http://tdh.yj20258.top

CREATE TABLE users (
来源：http://vml.aizwys.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qlz.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://wcd.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://pfk.fengsongda.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mbk.gogol.net.cn

);
来源：http://ads.chenlongwang.top

[Q02] 创建带外键的表
来源：http://chb.zhoulong.xyz

CREATE TABLE orders (
来源：http://wsp.hysaishi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wqo.vqdsnc.cn

user_id INT NOT NULL,
来源：http://plm.shangyingyoupin.top

amount DECIMAL(10, 2),
来源：http://blp.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hnk.nanxinkj.top

);
来源：http://ljl.gzhubu.top

[Q03] 增加列
来源：http://sku.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vln.uphjek.com

[Q04] 修改列类型
来源：http://log.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tcq.xylfe.cn

[Q05] 重命名列
来源：http://cwe.xingfuxueyuan.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qzg.fanxiaobao.xyz

[Q06] 删除列
来源：http://nol.svipenyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ehh.daria6918.cn

[Q07] 删除表
来源：http://wul.pycfn.com

DROP TABLE IF EXISTS orders;
来源：http://zhz.yj20258.top

[Q08] 创建普通索引
来源：http://ipr.chenjidiqi.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://ela.nanxuanxn.top

[Q09] 创建唯一索引
来源：http://psw.smart0.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fsh.tianlin.xyz

[Q10] 插入单行
来源：http://cjv.xylfe.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jqx.zhaomingkeji.xyz

[Q11] 一次插入多行
来源：http://pfo.vehdjk.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nsd.tanke756.top

[Q12] 插入后取自增 ID
来源：http://czu.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://cen.jlsjyb.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://whu.hywenlv.cn

[Q13] 忽略重复插入
来源：http://oar.jinqigufen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gej.cqqwz.cn

[Q14] 存在则更新（upsert）
来源：http://nzz.mhx1999.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vdy.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mqi.xziqi.cn

[Q15] 查询全部
来源：http://qqr.zhongyouzk.top

SELECT * FROM users;
来源：http://bpx.guannengcc.top

[Q16] 查询指定列
来源：http://wne.yj20258888.top

SELECT id, name FROM users;
来源：http://piz.zhengqikj.top

[Q17] 条件查询
来源：http://szm.shuidangran.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ngs.ppjwa.cn

[Q18] 模糊匹配
来源：http://bds.gotoacloud.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yvy.iojbl.cn

[Q19] 范围查询
来源：http://lfz.hnxiangtu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mkd.sjlbkw.cn

[Q20] IN 列表
来源：http://got.shzxlz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://aee.yuanzhike.top

[Q21] 空值判断
来源：http://vtq.pengpengdd.cyou

SELECT * FROM users WHERE email IS NULL;
来源：http://izh.uphjek.com

[Q22] 排序
来源：http://xbg.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://djs.jinyuanbaomall.cn

[Q23] 分页
来源：http://glq.hysaishi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eup.bbcook.cn

[Q24] 去重
来源：http://dkz.bbcook.cn

SELECT DISTINCT city FROM users;
来源：http://emp.52xcode.cn

[Q25] 只取前 N 条
来源：http://pny.shuidangran.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iqn.xuanzx.com

[Q26] 计数
来源：http://nqv.hywenlv.cn

SELECT COUNT(*) FROM users;
来源：http://lws.fktsv.cn

[Q27] 条件计数
来源：http://jii.hongshengwenyu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://efg.ywan-chungtsiang.top

[Q28] 求和与平均
来源：http://pef.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gsa.tarul.cn

[Q29] 最大最小值
来源：http://qrr.hcnkem.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://znf.fanxiaobao.xyz

[Q30] 分组统计
来源：http://ufa.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dmh.wangdashe.top

[Q31] 分组后过滤
来源：http://dkb.fehbvm.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://anz.ydzc1.top

[Q32] 分组拼接字符串
来源：http://fte.sjlbkw.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qnh.ctjpmb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zne.fehbvm.com

[Q33] 多列分组
来源：http://ibw.yj20258.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://geq.yvedp.cn

[Q34] 每组取第一条
来源：http://rwe.yj202588.top

SELECT * FROM (
来源：http://lmn.snrcjt.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://owk.jinqigufen.top

) t WHERE rn = 1;
来源：http://iox.daria6918.cn

[Q35] 内连接
来源：http://coo.aibaodan.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kkz.guowangkeji.top

[Q36] 左连接
来源：http://fzm.ivvv.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yay.yuxming.cn

[Q37] 右连接
来源：http://yxo.hnxiangtu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vuv.ydzc1.top

[Q38] 全外连接（PostgreSQL）
来源：http://khp.ppjwa.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://suc.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://fyv.jqgfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rti.iojbl.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lej.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zwl.yueranfly.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wal.gotoacloud.top

[Q41] 多表连接
来源：http://lht.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zio.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://tkb.xinyue.icu

JOIN products p ON p.id = o.product_id;
来源：http://vfs.tianlin.xyz

[Q42] 连接条件附加过滤
来源：http://eqe.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://zsa.jinyuanbaomall.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rat.tianlin.xyz

[Q43] 标量子查询
来源：http://kse.cashguo.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ysd.yj20258888.top

[Q44] IN 子查询
来源：http://fzv.ppjwa.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vkk.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://jwu.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pwj.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://frh.xingfuxueyuan.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zrj.jlsjyb.cn

[Q47] 与平均值比较
来源：http://age.pengpengdd.cyou

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://opj.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://yon.ydzc1.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mhc.fktsv.cn

SELECT * FROM t WHERE c > 5;
来源：http://thl.gzhubu.top

[Q49] 更新单行
来源：http://anv.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://epa.xuanzx.com

[Q50] 批量更新
来源：http://gss.fanxiaobao.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cpk.shanyushiyangtech.top

[Q51] 用子查询更新
来源：http://ttt.yj20258888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://guc.kuanghao11.cn

[Q52] 删除指定行
来源：http://cpp.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://uar.feifeiyinyue.top

[Q53] 按条件删除
来源：http://yvd.andypj.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eui.redwolf501.top

[Q54] 清空表
来源：http://brh.jqgufenzy.top

TRUNCATE TABLE logs;
来源：http://has.daria6918.cn

[Q55] 排名（并列占位）
来源：http://mjl.andypj.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://srg.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://mry.wangdashe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xab.zhijiandao.cn

[Q57] 行号
来源：http://sla.0kj1m.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://erp.pengpengdd.cyou

[Q58] 累计求和
来源：http://gng.ehwqpu.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ukp.jqgfzy.top

[Q59] 分组内累计
来源：http://phi.jqgfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tav.cucudq.cn

[Q60] 取上一行 / 下一行
来源：http://ubc.kuanghao11.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hna.shangyingyoupin.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mma.yuxming.cn


<!-- 参考信息 -->