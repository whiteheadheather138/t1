代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yaa.xylfe.cn

[N06] 判断回文字符串
来源：http://mjq.hywenlv.cn

Py:   s == s[::-1]
来源：http://swn.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://avm.yongpay.top

JS:   s === [...s].reverse().join("")
来源：http://xsb.yfazqb.com

TS:   s === [...s].reverse().join("")
来源：http://tri.xuetiantiany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nyf.tian-w.cn

Go:   // 双指针从两端比较
来源：http://anh.52xcode.cn

Ruby: s == s.reverse
来源：http://ixl.yj20258.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://psd.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://buk.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cna.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wkk.ybcxt.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nsh.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://hhe.snrcjt.cn

Java: // 手写 HashMap
来源：http://eea.jinyuanbaomall.cn

Go:   // 手写 map[int]int
来源：http://cgr.gotoacloud.top

Ruby: // 手写 Hash
来源：http://vzf.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://izo.chenlongwang.top

[N08] 生成全排列
来源：http://ayc.zdbjq.cn

Py:   itertools.permutations(arr)
来源：http://vnq.sjlbkw.cn

PHP:  // 手写递归交换
来源：http://lde.shuidangran.top

JS:   // 手写回溯递归
来源：http://qrx.jinqigufen.top

TS:   // 手写回溯递归
来源：http://ogi.jyoumei.cn

Java: // 手写回溯递归
来源：http://qql.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://tlq.ppjwa.cn

Ruby: arr.permutation.to_a
来源：http://boi.ybcxt.top

C#:   // 手写回溯递归
来源：http://cnu.birdmap.top

[N09] 栈与队列
来源：http://pmc.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pjs.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nwz.fanxiaobao.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zke.pycfn.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://loj.aizwys.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://plc.ppjwa.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cxe.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://led.cqqwz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://byv.yangfankeji.com

[N10] 链表节点定义
来源：http://hko.cashguo.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fyf.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://acv.sufxvd.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xdc.nanxinkj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zhp.guowangkeji.top

Java: class Node { int v; Node next; }
来源：http://ikh.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gxp.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://pjm.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://blw.guannengcc.top

[N11] 二叉树中序遍历
来源：http://hpi.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wjr.fanxiaobao.xyz

PHP:  // 手写递归函数
来源：http://kqb.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vrr.yj20258.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qwh.dianchejie.cn

Java: // 手写递归
来源：http://vum.svipenyu.cn

Go:   // 手写递归
来源：http://dvz.fanxiaobao.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hkt.zdbjq.cn

C#:   // 手写递归
来源：http://unb.meibo888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://shs.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ghy.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oot.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bpm.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gwb.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://skt.yanxiufei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jht.cqqwz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bax.hnxiangtu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bbc.jinghuilouyu.cn

================================================================================
来源：http://xna.xziqi.cn

O. 并发与异步
来源：http://pvp.nanxuanxn.top

================================================================================
来源：http://pdq.guannengcc.top

[O01] 启动一个线程
来源：http://evq.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hax.yvedp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ajq.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ycj.wangdashe.top

TS:   // 同 JS
来源：http://bcg.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://vwx.wangdashe.top

Go:   go f()
来源：http://buw.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://cee.yueranfly.top

C#:   Task.Run(() => F());
来源：http://ict.hongshengwenyu.top

[O02] 使用线程池
来源：http://hyg.vehdjk.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pgs.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xoq.zdqjudy.top

JS:   // worker_threads 线程池
来源：http://xwc.guannengcc.top

TS:   // worker_threads 线程池
来源：http://yap.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fix.shuidangran.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eas.bbcook.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ntq.shuidangran.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pwx.epnwcf.com

[O03] 加锁保护共享数据
来源：http://yur.cashguo.top

Py:   with lock: shared += 1
来源：http://amk.jlsjyb.cn

PHP:  // 用 flock() 做文件锁
来源：http://edt.sufxvd.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xiw.jlsjyb.cn

TS:   // 同 JS
来源：http://bcm.zhiwuduotai.top

Java: synchronized (this) { shared++; }
来源：http://dfe.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://siz.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tzn.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://zin.xinyue.icu

[O04] 定义异步函数并等待
来源：http://riu.nwbrower.top

Py:   async def f():⏎    await g()
来源：http://emb.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zyx.gotoacloud.top

JS:   async function f() { await g(); }
来源：http://fkh.havefunace.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kuh.ppjwa.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://byh.haohaochexian.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qif.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://nkc.cheryme.top

C#:   async Task F() { await G(); }
来源：http://iwj.hnqzz.top

[O05] 并发执行并等待全部完成
来源：http://evp.quarkkingdee.top

Py:   asyncio.gather(*tasks)
来源：http://etp.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kfp.zhaomingkeji.xyz

JS:   await Promise.all(tasks)
来源：http://krk.guowangkeji.top

TS:   await Promise.all(tasks)
来源：http://xut.yj20258888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ais.hywenlv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dgt.hysaishi.cn

Ruby: threads.map(&:join)
来源：http://mgh.hywenlv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nmo.ivvv.top

[O06] 使用进程池
来源：http://tqa.yangfankeji.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mcq.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ndf.tian-w.cn

JS:   // child_process / cluster 模块
来源：http://oeo.jinghuilouyu.cn

TS:   // child_process / cluster 模块
来源：http://rwg.cdnleiting.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hep.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nof.chenjidiqi.icu

Ruby: // fork 块
来源：http://jvj.yj20258888.top

C#:   Parallel.For
来源：http://gfb.xinyue.icu

================================================================================
来源：http://jqi.xziqi.cn

P. 常用工具函数
来源：http://vck.hysaishi.cn

================================================================================
来源：http://uhh.ehwqpu.com

[P01] 生成 UUID
来源：http://sny.yj20258888.top

Py:   str(uuid.uuid4())
来源：http://xyb.shangyingyoupin.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wiv.yj20258888.top

JS:   crypto.randomUUID()
来源：http://hvj.hammf.cn

TS:   crypto.randomUUID()
来源：http://eoj.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://ksm.jinyuanbaomall.cn

Go:   // 用 github.com/google/uuid
来源：http://glj.yongpay.top

Ruby: SecureRandom.uuid
来源：http://ysf.yfazqb.com

C#:   Guid.NewGuid().ToString()
来源：http://nvr.jyoumei.cn

[P02] MD5 / SHA256 摘要
来源：http://qwj.52xcode.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://knj.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qgp.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kss.ydzc1.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ztf.nanxinkj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qrt.zhiwuduotai.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ybz.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vyf.svipenyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qxa.zhoulong.xyz

[P03] 生成短随机字符串
来源：http://bmi.jqgufenzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wlw.cdnleiting.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cya.jqgufenzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://neu.jqgfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ikf.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kpv.yueranfly.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wop.hfpthk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qvt.vehdjk.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://udt.daria6918.cn

[P04] 求长度
来源：http://ujh.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wqh.ydzc1.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gud.jianghu66.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ppc.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fex.hcnkem.com

Java: list.size();  map.size();  s.length()
来源：http://deb.bbcook.cn

Go:   len(arr);  len(m)
来源：http://uol.feifeiyinyue.top

Ruby: x.length;  x.size
来源：http://emf.redwolf501.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cuz.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://zlr.meibo888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yhc.pengpengdd.cyou

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bfy.jqgfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nfc.wangshuangyany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sia.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qti.yj20258.top

Go:   reflect.DeepEqual(a, b)
来源：http://ebl.mhx1999.top

Ruby: a == b
来源：http://akl.jinqigufen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ifh.fktsv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lqa.jqgfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wxy.smart0.xyz

PHP:  if (empty($x)) {}
来源：http://qtq.zhengqikj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qdw.kuanghao11.cn

TS:   if (x == null) {}
来源：http://agu.hysaishi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ozj.fzhhl.top

Go:   if x == nil {}
来源：http://jzq.xylfe.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nxn.aizwys.cn

C#:   if (x is null) {}
来源：http://pge.xuanzx.com

[P07] 防抖与节流
来源：http://gjd.uphjek.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ikd.hongshengwenyu.top

PHP:  // 手写时间戳比较
来源：http://irn.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://arc.jqgufenzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://use.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mqr.yfazqb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rsi.snrcjt.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yqk.dianchejie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blk.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://xti.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pky.52xcode.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lgm.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gee.hysaishi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wvg.nanxinkj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xfk.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gwf.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://elz.zhijiandao.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gqb.daria6918.cn

================================================================================
来源：http://sci.0kj1m.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iat.hnxiangtu.top

================================================================================
来源：http://meh.havefunace.top

[Q01] 创建表
来源：http://rdl.jqgufenzy.top

CREATE TABLE users (
来源：http://ypo.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kvg.yongpay.top

name VARCHAR(50) NOT NULL,
来源：http://eha.tarul.cn

email VARCHAR(100) UNIQUE,
来源：http://knq.zdqjudy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oxh.yonumen.top

);
来源：http://qhw.snrcjt.cn

[Q02] 创建带外键的表
来源：http://evq.xziqi.cn

CREATE TABLE orders (
来源：http://mta.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lye.ehwqpu.com

user_id INT NOT NULL,
来源：http://shb.havefunace.top

amount DECIMAL(10, 2),
来源：http://nrb.nwbrower.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fir.sjlbkw.cn

);
来源：http://rwf.xinyue.icu

[Q03] 增加列
来源：http://luy.jlsjyb.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://flh.feifeiyinyue.top

[Q04] 修改列类型
来源：http://fjp.fanxiaobao.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hcj.havefunace.top

[Q05] 重命名列
来源：http://uab.snrcjt.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ghs.shzxlz.cn

[Q06] 删除列
来源：http://rml.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hah.zhongyouzk.top

[Q07] 删除表
来源：http://skp.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://gjy.cucudq.cn

[Q08] 创建普通索引
来源：http://ztr.tian-w.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fmy.jinqigufen.top

[Q09] 创建唯一索引
来源：http://wko.ppjwa.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jnh.sysykeji.top

[Q10] 插入单行
来源：http://spt.yangfankeji.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://alb.wangshuangyany.cn

[Q11] 一次插入多行
来源：http://for.dianchejie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jse.ctjpmb.com

[Q12] 插入后取自增 ID
来源：http://tpr.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://tcw.hesvh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dyo.0kj1m.cn

[Q13] 忽略重复插入
来源：http://upi.jqgfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://swz.sysykeji.top

[Q14] 存在则更新（upsert）
来源：http://olg.smart0.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xhz.hongshengwenyu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oug.jyoumei.cn

[Q15] 查询全部
来源：http://dqz.fanxiaobao.xyz

SELECT * FROM users;
来源：http://nkb.hcnkem.com

[Q16] 查询指定列
来源：http://beo.shangyingyoupin.top

SELECT id, name FROM users;
来源：http://mif.pycfn.com

[Q17] 条件查询
来源：http://unt.52xcode.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lkf.ctjpmb.com

[Q18] 模糊匹配
来源：http://zhf.zdqjudy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://trh.zhoulong.xyz

[Q19] 范围查询
来源：http://did.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gvs.ydzc1.top

[Q20] IN 列表
来源：http://fhb.cucudq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://imc.pengpengdd.cyou

[Q21] 空值判断
来源：http://mao.yfazqb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://hfx.cqqwz.cn

[Q22] 排序
来源：http://net.jqgufenzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cxg.fzhhl.top

[Q23] 分页
来源：http://muj.shangyingyoupin.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ban.yanxiufei.cn

[Q24] 去重
来源：http://dqw.meibo888.top

SELECT DISTINCT city FROM users;
来源：http://kjb.nanxinkj.top

[Q25] 只取前 N 条
来源：http://abp.gogol.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vpm.yj20258888.top

[Q26] 计数
来源：http://rqp.cucudq.cn

SELECT COUNT(*) FROM users;
来源：http://wmp.jqgufenzy.top

[Q27] 条件计数
来源：http://mhs.cucudq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bwy.hfpthk.cn

[Q28] 求和与平均
来源：http://uhf.zhongyouzk.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://etk.pycfn.com

[Q29] 最大最小值
来源：http://jax.fehbvm.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://rfl.pycfn.com

[Q30] 分组统计
来源：http://vex.tian-w.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ozz.hysaishi.cn

[Q31] 分组后过滤
来源：http://mck.aibaodan.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pea.iojbl.cn

[Q32] 分组拼接字符串
来源：http://ktj.tarul.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wis.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gid.yangfankeji.com

[Q33] 多列分组
来源：http://faw.zycfv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rvq.cheryme.top

[Q34] 每组取第一条
来源：http://yep.kuanghao11.cn

SELECT * FROM (
来源：http://tzb.0kj1m.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wvf.redwolf501.top

) t WHERE rn = 1;
来源：http://vbx.cucudq.cn

[Q35] 内连接
来源：http://xdf.snrcjt.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://asq.shangyingyoupin.top

[Q36] 左连接
来源：http://ztg.hnqzz.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://htz.sxryk.cn

[Q37] 右连接
来源：http://lhc.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://syy.andypj.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://zgo.fktsv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bgu.cucudq.cn

[Q39] 自连接（查上下级）
来源：http://gjj.cashguo.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://aaq.jianghu66.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lou.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bkw.hcnkem.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cvi.yuanzhike.top

[Q41] 多表连接
来源：http://oxo.yuxming.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sqj.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://uxq.ybcxt.top

JOIN products p ON p.id = o.product_id;
来源：http://xpp.zdqjudy.top

[Q42] 连接条件附加过滤
来源：http://ulc.jiagoushi.top


<!-- 参考信息 -->