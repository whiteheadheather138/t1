代发 wailian999

[N09] 栈与队列
来源：http://xqu.yuxming.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jnp.yanxiufei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nya.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://icc.svipenyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cff.gogol.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pfe.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gmz.zdbjq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ahr.daria6918.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mkn.shangyingyoupin.top

[N10] 链表节点定义
来源：http://qcb.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nhq.zhengqikj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://oyv.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tsu.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nrj.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://kcd.yj20258.top

Go:   type Node struct { V int; Next *Node }
来源：http://ata.jinyuanbaomall.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fhj.fengsongda.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gfn.hfpthk.cn

[N11] 二叉树中序遍历
来源：http://ncu.hysaishi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://klt.xinyue.icu

PHP:  // 手写递归函数
来源：http://ubk.cashguo.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://omh.jinqigufen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lkb.hnxiangtu.top

Java: // 手写递归
来源：http://ifb.52xcode.cn

Go:   // 手写递归
来源：http://fux.ywan-chungtsiang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sbf.gzhubu.top

C#:   // 手写递归
来源：http://kvm.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hwc.jinqigufen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ihh.fengsongda.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wvg.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kzp.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ggk.316326.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qfm.pengpengdd.cyou

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fbv.ppjwa.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://efu.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://etm.hysaishi.cn

================================================================================
来源：http://cnn.cucudq.cn

O. 并发与异步
来源：http://nzj.zdqjudy.top

================================================================================
来源：http://fbi.52xcode.cn

[O01] 启动一个线程
来源：http://hsg.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eog.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pxa.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cla.mhx1999.top

TS:   // 同 JS
来源：http://uyz.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://dac.yonumen.top

Go:   go f()
来源：http://ckh.havefunace.top

Ruby: Thread.new { f }
来源：http://cdd.ctjpmb.com

C#:   Task.Run(() => F());
来源：http://bty.pengpengdd.cyou

[O02] 使用线程池
来源：http://ncp.fzhhl.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kob.sweek.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lki.birdmap.top

JS:   // worker_threads 线程池
来源：http://dwh.yj20258.top

TS:   // worker_threads 线程池
来源：http://ewb.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ivk.yj202588.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://poi.hesvh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qbd.smart0.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zld.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://mvm.tanke756.top

Py:   with lock: shared += 1
来源：http://cpv.gzhubu.top

PHP:  // 用 flock() 做文件锁
来源：http://lqv.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jwb.hfpthk.cn

TS:   // 同 JS
来源：http://tis.cucudq.cn

Java: synchronized (this) { shared++; }
来源：http://hes.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fzu.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://doh.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://hee.fanxiaobao.xyz

[O04] 定义异步函数并等待
来源：http://pyo.bbcook.cn

Py:   async def f():⏎    await g()
来源：http://jtc.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wqk.gzhubu.top

JS:   async function f() { await g(); }
来源：http://ptp.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://jpk.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qcg.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pxm.aizwys.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ybc.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://rmj.dianchejie.cn

[O05] 并发执行并等待全部完成
来源：http://pdr.feifeiyinyue.top

Py:   asyncio.gather(*tasks)
来源：http://fmw.havefunace.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cww.xylfe.cn

JS:   await Promise.all(tasks)
来源：http://vwy.hywenlv.cn

TS:   await Promise.all(tasks)
来源：http://yim.guannengcc.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rha.hnqzz.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://neo.ywan-chungtsiang.top

Ruby: threads.map(&:join)
来源：http://vow.bbcook.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oov.ydzc1.top

[O06] 使用进程池
来源：http://ihc.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eda.sweek.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ckl.nanxinkj.top

JS:   // child_process / cluster 模块
来源：http://xrp.hammf.cn

TS:   // child_process / cluster 模块
来源：http://tbq.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://svb.daxiang520.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yon.sysykeji.top

Ruby: // fork 块
来源：http://ibh.ydzc1.top

C#:   Parallel.For
来源：http://spo.shuidangran.top

================================================================================
来源：http://dzm.9152youxi.cn

P. 常用工具函数
来源：http://jld.yanxiufei.cn

================================================================================
来源：http://meh.ywan-chungtsiang.top

[P01] 生成 UUID
来源：http://xoz.havefunace.top

Py:   str(uuid.uuid4())
来源：http://boj.jianghu66.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wwk.xylfe.cn

JS:   crypto.randomUUID()
来源：http://jot.haohaochexian.top

TS:   crypto.randomUUID()
来源：http://kqn.meibo888.top

Java: UUID.randomUUID().toString()
来源：http://rif.sufxvd.cn

Go:   // 用 github.com/google/uuid
来源：http://dlo.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://kkb.zhaomingkeji.xyz

C#:   Guid.NewGuid().ToString()
来源：http://gmp.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://hxr.sweek.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://phj.hysaishi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pah.ydzc1.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bej.xuanzx.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ylk.fzhhl.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hlk.cdnleiting.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yyo.cdnleiting.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kea.dianchejie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kcy.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://rrk.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://crl.jiagoushi.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lwa.fanxiaobao.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rhl.guowangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rjw.snrcjt.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gho.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cld.hammf.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tsy.xylfe.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vus.zdbjq.cn

[P04] 求长度
来源：http://hcj.dianchejie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fmh.yfazqb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jbp.fengsongda.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pkh.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sjo.redwolf501.top

Java: list.size();  map.size();  s.length()
来源：http://wqr.0kj1m.cn

Go:   len(arr);  len(m)
来源：http://kyc.nanxinkj.top

Ruby: x.length;  x.size
来源：http://dof.jqgfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dcb.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://joi.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dvk.dashuyun.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rmq.zhongyouzk.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zoh.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qcj.zhaomingkeji.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eip.cashguo.top

Go:   reflect.DeepEqual(a, b)
来源：http://ysn.gotoacloud.top

Ruby: a == b
来源：http://ecy.jlsjyb.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jxj.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ths.yangfankeji.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fbv.zhiwuduotai.top

PHP:  if (empty($x)) {}
来源：http://sxo.jlsjyb.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yvw.ydjk.org.cn

TS:   if (x == null) {}
来源：http://yvp.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://nig.uphjek.com

Go:   if x == nil {}
来源：http://luh.birdmap.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kuo.52xcode.cn

C#:   if (x is null) {}
来源：http://zrt.vqdsnc.cn

[P07] 防抖与节流
来源：http://gwu.yanxiufei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fdc.yuxming.cn

PHP:  // 手写时间戳比较
来源：http://abs.cqqwz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xwp.xingfuxueyuan.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jsj.yj202588.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dxh.sjlbkw.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fhs.shangyingyoupin.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ajj.9152youxi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nox.shzxlz.cn

[P08] 处理浮点精度问题
来源：http://lbj.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vfm.tianlin.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rxo.quarkkingdee.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pbu.uphjek.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://csp.zhijiandao.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ppd.aizwys.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qgu.sxryk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kef.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uhy.cheryme.top

================================================================================
来源：http://ncn.yanxiufei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bkw.cqqwz.cn

================================================================================
来源：http://ouj.cheryme.top

[Q01] 创建表
来源：http://rcu.jinqigfzy.top

CREATE TABLE users (
来源：http://jon.vqdsnc.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ntd.redwolf501.top

name VARCHAR(50) NOT NULL,
来源：http://gze.hysaishi.cn

email VARCHAR(100) UNIQUE,
来源：http://lel.tarul.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bbs.fehbvm.com

);
来源：http://uvz.snrcjt.cn

[Q02] 创建带外键的表
来源：http://igc.jianghu66.top

CREATE TABLE orders (
来源：http://mkw.kuanghao11.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fli.zhijiandao.cn

user_id INT NOT NULL,
来源：http://zrd.chenlongwang.top

amount DECIMAL(10, 2),
来源：http://rxm.vehdjk.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dmy.yj20258888.top

);
来源：http://pbo.xuetiantiany.cn

[Q03] 增加列
来源：http://xsz.yj20258.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://enb.jinqigfzy.top

[Q04] 修改列类型
来源：http://nrm.kuanghao11.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jla.zhixingplan.top

[Q05] 重命名列
来源：http://utm.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sak.shanyushiyangkeji.top

[Q06] 删除列
来源：http://vzg.ywan-chungtsiang.top

ALTER TABLE users DROP COLUMN age;
来源：http://pzn.gaohongyu789.top

[Q07] 删除表
来源：http://jtp.pycfn.com

DROP TABLE IF EXISTS orders;
来源：http://bxt.hammf.cn

[Q08] 创建普通索引
来源：http://rim.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://amg.jinqigfzy.top

[Q09] 创建唯一索引
来源：http://pqt.yonumen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xub.sufxvd.cn

[Q10] 插入单行
来源：http://mpn.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ahv.smart0.xyz

[Q11] 一次插入多行
来源：http://thy.9152youxi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iuo.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://fva.xylfe.cn

INSERT INTO users (name) VALUES ('C');
来源：http://evd.daxiang520.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ptp.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://cxh.xziqi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lao.snrcjt.cn

[Q14] 存在则更新（upsert）
来源：http://ohz.zhengqikj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vsd.jqgufenzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wtp.iojbl.cn

[Q15] 查询全部
来源：http://gzd.zhiwuduotai.top

SELECT * FROM users;
来源：http://ioz.tianlin.xyz

[Q16] 查询指定列
来源：http://ojo.zhiwuduotai.top

SELECT id, name FROM users;
来源：http://xxs.andypj.xyz

[Q17] 条件查询
来源：http://fge.ydjk.org.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mvr.cashguo.top

[Q18] 模糊匹配
来源：http://dzg.fanxiaobao.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iwy.hnxiangtu.top

[Q19] 范围查询
来源：http://rwz.c1oappe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vag.hammf.cn

[Q20] IN 列表
来源：http://pbj.316326.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kcu.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://qra.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tgs.yfazqb.com

[Q22] 排序
来源：http://fak.ybcxt.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cfr.zhongyouzk.top

[Q23] 分页
来源：http://fbz.jinqigufen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hyh.zycfv.cn

[Q24] 去重
来源：http://ugf.uphjek.com

SELECT DISTINCT city FROM users;
来源：http://fny.mhx1999.top

[Q25] 只取前 N 条
来源：http://zfm.fktsv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uzx.jlsjyb.cn

[Q26] 计数
来源：http://krp.cucudq.cn

SELECT COUNT(*) FROM users;
来源：http://sch.epnwcf.com

[Q27] 条件计数
来源：http://nam.xuanzx.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eeh.yvedp.cn

[Q28] 求和与平均
来源：http://sop.zhiwuduotai.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ekp.yueranfly.top

[Q29] 最大最小值
来源：http://lvz.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://fze.shanyushiyangkeji.top

[Q30] 分组统计
来源：http://tht.jqgufenzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lma.cheryme.top

[Q31] 分组后过滤
来源：http://hvi.316326.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eau.jianghu66.top

[Q32] 分组拼接字符串
来源：http://jot.hnqzz.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://per.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hyq.xuanzx.com

[Q33] 多列分组
来源：http://vbs.ydzc1.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kle.jianghu66.top

[Q34] 每组取第一条
来源：http://uls.shzxlz.cn

SELECT * FROM (
来源：http://mxn.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://euq.yanxiufei.cn

) t WHERE rn = 1;
来源：http://tqj.nanxuanxn.top

[Q35] 内连接
来源：http://geu.aibaodan.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hmx.smart0.xyz

[Q36] 左连接
来源：http://uob.guannengcc.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bkj.cheryme.top

[Q37] 右连接
来源：http://fse.hysaishi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ayi.xuetiantiany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mmu.hammf.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pka.zhaomingkeji.xyz

[Q39] 自连接（查上下级）
来源：http://odv.guannengcc.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://suh.vehdjk.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dae.wangshuangyany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mxe.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://haq.cashguo.top

[Q41] 多表连接
来源：http://uyp.cqqwz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xxe.ppjwa.cn

JOIN users u ON u.id = o.user_id
来源：http://kpb.cheryme.top

JOIN products p ON p.id = o.product_id;
来源：http://bop.gzhubu.top

[Q42] 连接条件附加过滤
来源：http://ghj.sufxvd.cn

SELECT u.name, o.amount FROM users u
来源：http://qyc.sweek.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fpq.fengsongda.top

[Q43] 标量子查询
来源：http://qcd.cashguo.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ucj.aibaodan.cn

[Q44] IN 子查询
来源：http://ric.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jco.zhengqikj.top

[Q45] EXISTS 判断存在
来源：http://zpq.birdmap.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lty.zhengqikj.top

[Q46] NOT EXISTS 判断不存在
来源：http://mqz.sufxvd.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tgh.shuidangran.top

[Q47] 与平均值比较
来源：http://uyy.daria6918.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wgi.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://gyy.dashuyun.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pxz.xuetiantiany.cn

SELECT * FROM t WHERE c > 5;
来源：http://yyo.cqqwz.cn

[Q49] 更新单行
来源：http://cqh.svipenyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jdk.hywenlv.cn

[Q50] 批量更新
来源：http://hhe.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jfs.xinyue.icu

[Q51] 用子查询更新
来源：http://wwi.andypj.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://guy.dianchejie.cn

[Q52] 删除指定行
来源：http://xyr.yuanzhike.top

DELETE FROM users WHERE id = 10;
来源：http://nak.dianchejie.cn

[Q53] 按条件删除
来源：http://oth.hesvh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bsb.fktsv.cn

[Q54] 清空表
来源：http://bcw.andypj.xyz

TRUNCATE TABLE logs;
来源：http://oyl.hesvh.cn

[Q55] 排名（并列占位）
来源：http://mis.tarul.cn


<!-- 参考信息 -->