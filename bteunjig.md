代发 wailian999

Go:   // 手写 map[int]int
来源：http://eqw.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://nxe.bjfxy.top

C#:   // 手写 Dictionary<int, int>
来源：http://qok.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://ryb.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://fpg.yonumen.top

PHP:  // 手写递归交换
来源：http://lod.ydjk.org.cn

JS:   // 手写回溯递归
来源：http://yop.fzhhl.top

TS:   // 手写回溯递归
来源：http://zhj.nanxinkj.top

Java: // 手写回溯递归
来源：http://acr.cheryme.top

Go:   // 手写回溯递归
来源：http://vbj.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://fkl.shzxlz.cn

C#:   // 手写回溯递归
来源：http://qyc.gzhubu.top

[N09] 栈与队列
来源：http://mux.guowangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wjv.chenjidiqi.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uxb.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mmx.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ymk.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pri.zhaomingkeji.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rmt.316326.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hka.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xoi.nanxinkj.top

[N10] 链表节点定义
来源：http://wax.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wak.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bhf.sweek.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rid.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wsr.yuxming.cn

Java: class Node { int v; Node next; }
来源：http://swz.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://tyd.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sjw.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://ijz.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://xbi.shangyingyoupin.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gby.yuanzhike.top

PHP:  // 手写递归函数
来源：http://gsg.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wqq.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yxx.andypj.xyz

Java: // 手写递归
来源：http://fyp.haohaochexian.top

Go:   // 手写递归
来源：http://vdx.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gwd.yvedp.cn

C#:   // 手写递归
来源：http://yeg.meibo888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bez.cqqwz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tuj.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rft.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nbc.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jrj.xziqi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uuf.sjlbkw.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bet.xylfe.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bcg.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ysi.xuetiantiany.cn

================================================================================
来源：http://ovx.yanxiufei.cn

O. 并发与异步
来源：http://ekf.gogol.net.cn

================================================================================
来源：http://gxu.cashguo.top

[O01] 启动一个线程
来源：http://skc.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://llr.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qpy.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://udw.jianghu66.top

TS:   // 同 JS
来源：http://reh.wangdashe.top

Java: new Thread(() -> f()).start()
来源：http://otq.jqgfzy.top

Go:   go f()
来源：http://mya.kuanghao11.cn

Ruby: Thread.new { f }
来源：http://fon.ppjwa.cn

C#:   Task.Run(() => F());
来源：http://fkb.uphjek.com

[O02] 使用线程池
来源：http://brn.zhijiandao.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iax.zhixingplan.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oll.hongshengwenyu.top

JS:   // worker_threads 线程池
来源：http://fdh.nanxuanxn.top

TS:   // worker_threads 线程池
来源：http://zvn.sweek.top

Java: Executors.newFixedThreadPool(4)
来源：http://nae.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wvz.zycfv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://upl.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rqd.ywan-chungtsiang.top

[O03] 加锁保护共享数据
来源：http://qdn.jinyuanbaomall.cn

Py:   with lock: shared += 1
来源：http://qzn.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://eof.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://prs.yj20258.top

TS:   // 同 JS
来源：http://rpb.fengsongda.top

Java: synchronized (this) { shared++; }
来源：http://kzb.shanyushiyangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ljs.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://roh.c1oappe.top

C#:   lock (gate) { shared++; }
来源：http://snh.hongshengwenyu.top

[O04] 定义异步函数并等待
来源：http://axx.gzhubu.top

Py:   async def f():⏎    await g()
来源：http://wla.zdqjudy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wsw.uphjek.com

JS:   async function f() { await g(); }
来源：http://rgz.hcnkem.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://stw.yonumen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zhn.yongpay.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://irw.jyoumei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://owa.yj202588.top

C#:   async Task F() { await G(); }
来源：http://lui.c1oappe.top

[O05] 并发执行并等待全部完成
来源：http://quz.yj20258.top

Py:   asyncio.gather(*tasks)
来源：http://jdm.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yqc.chenjidiqi.icu

JS:   await Promise.all(tasks)
来源：http://hor.0kj1m.cn

TS:   await Promise.all(tasks)
来源：http://jsd.gaohongyu789.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ytc.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lbt.yj20258888.top

Ruby: threads.map(&:join)
来源：http://vns.jiagoushi.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lxa.yuanzhike.top

[O06] 使用进程池
来源：http://pny.zhiwuduotai.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wua.yonumen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cmb.svipenyu.cn

JS:   // child_process / cluster 模块
来源：http://yno.xingfuxueyuan.xyz

TS:   // child_process / cluster 模块
来源：http://box.shuidangran.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bli.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nos.ybcxt.top

Ruby: // fork 块
来源：http://gxo.guannengcc.top

C#:   Parallel.For
来源：http://qdd.yvedp.cn

================================================================================
来源：http://myd.pengpengdd.cyou

P. 常用工具函数
来源：http://jto.zhoulong.xyz

================================================================================
来源：http://nao.wangdashe.top

[P01] 生成 UUID
来源：http://oox.sjlbkw.cn

Py:   str(uuid.uuid4())
来源：http://ivn.fengsongda.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gqw.ywan-chungtsiang.top

JS:   crypto.randomUUID()
来源：http://kmr.sysykeji.top

TS:   crypto.randomUUID()
来源：http://zlw.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://epe.zhiwuduotai.top

Go:   // 用 github.com/google/uuid
来源：http://lmg.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://nkd.ywan-chungtsiang.top

C#:   Guid.NewGuid().ToString()
来源：http://chj.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://hhs.ivvv.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ljc.gzhubu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://aif.guannengcc.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iup.zhongyouzk.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wzi.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gey.gotoacloud.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iiv.hongshengwenyu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://akf.shangyingyoupin.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lvg.hnqzz.top

[P03] 生成短随机字符串
来源：http://avz.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qta.haohaochexian.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tzu.bjfxy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rby.shuidangran.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://opz.sjlbkw.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eur.jqgfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://adu.jinyuanbaomall.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fiw.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rgr.zycfv.cn

[P04] 求长度
来源：http://tus.zdbjq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hwz.svipenyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wgf.316326.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hxa.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hby.fehbvm.com

Java: list.size();  map.size();  s.length()
来源：http://gmu.yuxming.cn

Go:   len(arr);  len(m)
来源：http://obl.haohaochexian.top

Ruby: x.length;  x.size
来源：http://urq.epnwcf.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://cnc.cheryme.top

[P05] 判断两个对象内容是否相等
来源：http://tfn.hfpthk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bik.redwolf501.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wwc.xziqi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sik.zdqjudy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://naq.yuanzhike.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hmi.redwolf501.top

Go:   reflect.DeepEqual(a, b)
来源：http://egu.52xcode.cn

Ruby: a == b
来源：http://meb.tianlin.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wfr.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wlo.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zbs.quarkkingdee.top

PHP:  if (empty($x)) {}
来源：http://inw.chenzaomai.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pwp.iojbl.cn

TS:   if (x == null) {}
来源：http://btc.pycfn.com

Java: if (x == null || x.isEmpty()) {}
来源：http://gif.dashuyun.cn

Go:   if x == nil {}
来源：http://omw.redwolf501.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ccr.daxiang520.top

C#:   if (x is null) {}
来源：http://ptr.zycfv.cn

[P07] 防抖与节流
来源：http://ssu.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uaz.yongpay.top

PHP:  // 手写时间戳比较
来源：http://tdt.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wun.gzhubu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://exf.ctjpmb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zmo.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rxv.shzxlz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://alf.nanxinkj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mcb.gzhubu.top

[P08] 处理浮点精度问题
来源：http://ksb.sysykeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://epb.hongshengwenyu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vsd.zhengqikj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://miz.xinyue.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oji.hnxiangtu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zjg.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kjb.fanxiaobao.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tcg.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zcz.xuanzx.com

================================================================================
来源：http://rcc.hysaishi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mny.zhongyouzk.top

================================================================================
来源：http://thb.ivvv.top

[Q01] 创建表
来源：http://rnl.gotoacloud.top

CREATE TABLE users (
来源：http://ffv.ivvv.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dbk.jinyuanbaomall.cn

name VARCHAR(50) NOT NULL,
来源：http://gew.zycfv.cn

email VARCHAR(100) UNIQUE,
来源：http://seg.jinghuilouyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cxb.svipenyu.cn

);
来源：http://pcn.jyoumei.cn

[Q02] 创建带外键的表
来源：http://cim.fehbvm.com

CREATE TABLE orders (
来源：http://nxs.zhoulong.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dek.epnwcf.com

user_id INT NOT NULL,
来源：http://qap.bbcook.cn

amount DECIMAL(10, 2),
来源：http://sfu.yfazqb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ors.zhengqikj.top

);
来源：http://aox.jlsjyb.cn

[Q03] 增加列
来源：http://ail.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xgg.xuanzx.com

[Q04] 修改列类型
来源：http://zvb.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jjm.gzhubu.top

[Q05] 重命名列
来源：http://hsi.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yjv.svipenyu.cn

[Q06] 删除列
来源：http://ile.yuxming.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vwa.yangfankeji.com

[Q07] 删除表
来源：http://ppr.havefunace.top

DROP TABLE IF EXISTS orders;
来源：http://gol.shanyushiyangkeji.top

[Q08] 创建普通索引
来源：http://tjh.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://thg.shangyingyoupin.top

[Q09] 创建唯一索引
来源：http://vwd.haohaochexian.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lmw.vehdjk.com

[Q10] 插入单行
来源：http://tms.cashguo.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xzx.xziqi.cn

[Q11] 一次插入多行
来源：http://kpr.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iii.smart0.xyz

[Q12] 插入后取自增 ID
来源：http://lll.fengsongda.top

INSERT INTO users (name) VALUES ('C');
来源：http://gxz.ybcxt.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dlw.redwolf501.top

[Q13] 忽略重复插入
来源：http://teh.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mps.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://jzv.chenjidiqi.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hqe.iojbl.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hqg.c1oappe.top

[Q15] 查询全部
来源：http://evt.redwolf501.top

SELECT * FROM users;
来源：http://xwu.chenzaomai.com

[Q16] 查询指定列
来源：http://dsm.ydjk.org.cn

SELECT id, name FROM users;
来源：http://nci.yuanzhike.top

[Q17] 条件查询
来源：http://jsu.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fsy.bjfxy.top

[Q18] 模糊匹配
来源：http://rvh.jqgufenzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mpt.52xcode.cn

[Q19] 范围查询
来源：http://iul.aibaodan.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://flp.ehwqpu.com

[Q20] IN 列表
来源：http://sgc.nanxuanxn.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xdk.zhiwuduotai.top

[Q21] 空值判断
来源：http://xcw.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fin.andypj.xyz

[Q22] 排序
来源：http://tby.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oam.sjlbkw.cn

[Q23] 分页
来源：http://pcu.hcnkem.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qhj.xinyue.icu

[Q24] 去重
来源：http://pbq.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://gjs.xylfe.cn

[Q25] 只取前 N 条
来源：http://jwk.cucudq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vre.pengpengdd.cyou

[Q26] 计数
来源：http://afa.xuetiantiany.cn

SELECT COUNT(*) FROM users;
来源：http://fyh.shzxlz.cn

[Q27] 条件计数
来源：http://bwv.jianghu66.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lce.zhijiandao.cn

[Q28] 求和与平均
来源：http://xpt.quarkkingdee.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qrb.tianlin.xyz

[Q29] 最大最小值
来源：http://ssi.yanxiufei.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dzd.yanxiufei.cn

[Q30] 分组统计
来源：http://tha.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fbx.yonumen.top

[Q31] 分组后过滤
来源：http://pba.hnqzz.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hgp.sufxvd.cn

[Q32] 分组拼接字符串
来源：http://ycd.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cvr.feifeiyinyue.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://inx.zhongyouzk.top

[Q33] 多列分组
来源：http://gkv.shzxlz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wgk.zhijiandao.cn

[Q34] 每组取第一条
来源：http://gmk.bjfxy.top

SELECT * FROM (
来源：http://wze.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gag.yj20258.top

) t WHERE rn = 1;
来源：http://axc.nwbrower.top

[Q35] 内连接
来源：http://soh.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bpd.ybcxt.top

[Q36] 左连接
来源：http://wzq.nanxinkj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fwy.aibaodan.cn

[Q37] 右连接
来源：http://lbo.vqdsnc.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sbx.tanke756.top

[Q38] 全外连接（PostgreSQL）
来源：http://tvu.havefunace.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ttt.hywenlv.cn

[Q39] 自连接（查上下级）
来源：http://jid.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://fdf.dashuyun.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mns.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nrx.ppjwa.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xnz.uphjek.com

[Q41] 多表连接
来源：http://tzn.ehwqpu.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://dlr.jinyuanbaomall.cn

JOIN users u ON u.id = o.user_id
来源：http://xqz.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://cxx.nanxuanxn.top

[Q42] 连接条件附加过滤
来源：http://mvh.sysykeji.top

SELECT u.name, o.amount FROM users u
来源：http://pgg.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dwc.52xcode.cn

[Q43] 标量子查询
来源：http://jsu.jqgufenzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bbt.fktsv.cn

[Q44] IN 子查询
来源：http://cfq.jqgfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tme.jinqigfzy.top

[Q45] EXISTS 判断存在
来源：http://pqb.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://drd.yangfankeji.com

[Q46] NOT EXISTS 判断不存在
来源：http://dvi.sxryk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oip.tanke756.top

[Q47] 与平均值比较
来源：http://uff.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://agq.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://hye.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xql.shangyingyoupin.top

SELECT * FROM t WHERE c > 5;
来源：http://elv.jinqigfzy.top

[Q49] 更新单行
来源：http://jgx.ehwqpu.com


<!-- 参考信息 -->