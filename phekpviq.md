代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mqw.bbcook.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gdi.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zkc.sufxvd.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mfz.svipenyu.cn

[N05] 最大公约数
来源：http://fvj.cashguo.top

Py:   math.gcd(a, b)
来源：http://jpv.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hhj.svipenyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dkr.jqgfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bsg.ivvv.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tev.tianlin.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bzw.xziqi.cn

Ruby: a.gcd(b)
来源：http://zqn.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rug.hongshengwenyu.top

[N06] 判断回文字符串
来源：http://efy.gotoacloud.top

Py:   s == s[::-1]
来源：http://yfs.jqgfzy.top

PHP:  $s === strrev($s);
来源：http://czu.jqgufenzy.top

JS:   s === [...s].reverse().join("")
来源：http://now.gotoacloud.top

TS:   s === [...s].reverse().join("")
来源：http://hte.gaohongyu789.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fef.epnwcf.com

Go:   // 双指针从两端比较
来源：http://rtd.sweek.top

Ruby: s == s.reverse
来源：http://tac.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://edl.epnwcf.com

[N07] 两数之和（返回下标）
来源：http://wov.havefunace.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mcg.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pig.tarul.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://puq.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://sjt.bbcook.cn

Java: // 手写 HashMap
来源：http://sjh.yonumen.top

Go:   // 手写 map[int]int
来源：http://zvk.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://dkk.52xcode.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hfc.meibo888.top

[N08] 生成全排列
来源：http://ane.hywenlv.cn

Py:   itertools.permutations(arr)
来源：http://yvg.bjfxy.top

PHP:  // 手写递归交换
来源：http://vef.zycfv.cn

JS:   // 手写回溯递归
来源：http://dki.sufxvd.cn

TS:   // 手写回溯递归
来源：http://owv.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://ecy.gotoacloud.top

Go:   // 手写回溯递归
来源：http://ogf.xingfuxueyuan.xyz

Ruby: arr.permutation.to_a
来源：http://jzn.hammf.cn

C#:   // 手写回溯递归
来源：http://fte.fanxiaobao.xyz

[N09] 栈与队列
来源：http://gqk.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fzg.cqqwz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kza.jqgufenzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://flq.zhengqikj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://phj.xuanzx.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vmn.iojbl.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gah.shanyushiyangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pys.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hwf.316326.xyz

[N10] 链表节点定义
来源：http://lwl.yj20258888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pes.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tqf.cashguo.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ezu.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nor.yonumen.top

Java: class Node { int v; Node next; }
来源：http://qjr.epnwcf.com

Go:   type Node struct { V int; Next *Node }
来源：http://tmc.feifeiyinyue.top

Ruby: Node = Struct.new(:v, :next)
来源：http://boa.zdbjq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://eiq.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://fqq.yonumen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nac.gogol.net.cn

PHP:  // 手写递归函数
来源：http://clr.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uhi.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kdn.nwbrower.top

Java: // 手写递归
来源：http://llp.sxryk.cn

Go:   // 手写递归
来源：http://ebf.wangdashe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eqk.iojbl.cn

C#:   // 手写递归
来源：http://zxw.smart0.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://trq.sjlbkw.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bwr.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dnd.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zzq.sxryk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hbh.sufxvd.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vkb.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mlv.tarul.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kro.smart0.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pcq.yangfankeji.com

================================================================================
来源：http://snr.hfpthk.cn

O. 并发与异步
来源：http://shp.tanke756.top

================================================================================
来源：http://ffe.yangfankeji.com

[O01] 启动一个线程
来源：http://ygs.andypj.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gyr.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://inj.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yps.zhongyouzk.top

TS:   // 同 JS
来源：http://mvx.bbcook.cn

Java: new Thread(() -> f()).start()
来源：http://kfr.xziqi.cn

Go:   go f()
来源：http://uma.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://kzg.wangshuangyany.cn

C#:   Task.Run(() => F());
来源：http://xwu.kuanghao11.cn

[O02] 使用线程池
来源：http://yvg.zhongyouzk.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tov.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qtz.yuanzhike.top

JS:   // worker_threads 线程池
来源：http://oyw.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://umt.0kj1m.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xll.tanke756.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kxy.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ico.tarul.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://axt.hywenlv.cn

[O03] 加锁保护共享数据
来源：http://bff.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://wda.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://dst.gotoacloud.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gaq.hysaishi.cn

TS:   // 同 JS
来源：http://nsc.cdnleiting.top

Java: synchronized (this) { shared++; }
来源：http://aen.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cht.tianlin.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://lmv.tarul.cn

C#:   lock (gate) { shared++; }
来源：http://gvz.yvedp.cn

[O04] 定义异步函数并等待
来源：http://pqb.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://iui.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hmw.feifeiyinyue.top

JS:   async function f() { await g(); }
来源：http://xlw.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://olm.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ate.yj20258.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hqy.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://qme.gzhubu.top

C#:   async Task F() { await G(); }
来源：http://bnt.iojbl.cn

[O05] 并发执行并等待全部完成
来源：http://wpi.yuxming.cn

Py:   asyncio.gather(*tasks)
来源：http://qvp.epnwcf.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rkz.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://byc.havefunace.top

TS:   await Promise.all(tasks)
来源：http://rks.tanke756.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fze.jinghuilouyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xsz.yonumen.top

Ruby: threads.map(&:join)
来源：http://wbw.xuanzx.com

C#:   await Task.WhenAll(t1, t2)
来源：http://vtv.haohaochexian.top

[O06] 使用进程池
来源：http://zqt.aibaodan.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fpl.hcnkem.com

PHP:  // pcntl_fork 或多进程队列
来源：http://yhd.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://caj.xingfuxueyuan.xyz

TS:   // child_process / cluster 模块
来源：http://fqd.yuxming.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xwc.fengsongda.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kve.zhixingplan.top

Ruby: // fork 块
来源：http://fpw.yuxming.cn

C#:   Parallel.For
来源：http://tuh.9152youxi.cn

================================================================================
来源：http://lvb.9152youxi.cn

P. 常用工具函数
来源：http://sxe.ywan-chungtsiang.top

================================================================================
来源：http://gpx.gaohongyu789.top

[P01] 生成 UUID
来源：http://oyh.ydjk.org.cn

Py:   str(uuid.uuid4())
来源：http://hqo.zhixingplan.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xfh.daria6918.cn

JS:   crypto.randomUUID()
来源：http://yjn.ivvv.top

TS:   crypto.randomUUID()
来源：http://vwv.pengpengdd.cyou

Java: UUID.randomUUID().toString()
来源：http://wwb.birdmap.top

Go:   // 用 github.com/google/uuid
来源：http://wvu.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://nvg.wangdashe.top

C#:   Guid.NewGuid().ToString()
来源：http://rvz.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://jge.nwbrower.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jmg.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://vmt.wangdashe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://duf.hongshengwenyu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rwg.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ffh.cucudq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tbk.haohaochexian.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jeb.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://drr.yongpay.top

[P03] 生成短随机字符串
来源：http://xez.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ogo.cheryme.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vri.316326.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kta.zhiwuduotai.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oqp.tarul.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ioe.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zrl.havefunace.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jqk.zhongyouzk.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xju.xuanzx.com

[P04] 求长度
来源：http://jjj.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://olh.yongpay.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://moo.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cay.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mnv.kuanghao11.cn

Java: list.size();  map.size();  s.length()
来源：http://umj.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://yhq.xuanzx.com

Ruby: x.length;  x.size
来源：http://rov.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://obn.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://zig.hongshengwenyu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kmt.fehbvm.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dci.shuidangran.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kpa.yanxiufei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wmm.cashguo.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://czk.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://myf.xinyue.icu

Ruby: a == b
来源：http://nfi.jinyuanbaomall.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tpn.pycfn.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://enc.cqqwz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://edv.cdnleiting.top

PHP:  if (empty($x)) {}
来源：http://mjx.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dzw.tian-w.cn

TS:   if (x == null) {}
来源：http://tok.shzxlz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hci.fanxiaobao.xyz

Go:   if x == nil {}
来源：http://iez.pycfn.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vay.sufxvd.cn

C#:   if (x is null) {}
来源：http://jzj.zhijiandao.cn

[P07] 防抖与节流
来源：http://gmt.xziqi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nxb.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://enx.hfpthk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hgz.xingfuxueyuan.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bnn.chenlongwang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yqg.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hoh.yvedp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://izk.gzhubu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lja.svipenyu.cn

[P08] 处理浮点精度问题
来源：http://lkd.yuanzhike.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rgl.yvedp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://thv.tianlin.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mga.bbcook.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pey.hnqzz.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zou.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://utp.hywenlv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fnb.hywenlv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jck.epnwcf.com

================================================================================
来源：http://bkc.epnwcf.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mpj.fktsv.cn

================================================================================
来源：http://bdd.yueranfly.top

[Q01] 创建表
来源：http://opv.cashguo.top

CREATE TABLE users (
来源：http://dbj.yuanzhike.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://clw.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://qyh.bbcook.cn

email VARCHAR(100) UNIQUE,
来源：http://wtv.pycfn.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rpf.sweek.top

);
来源：http://lff.0kj1m.cn

[Q02] 创建带外键的表
来源：http://vgm.redwolf501.top

CREATE TABLE orders (
来源：http://eqf.cucudq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zkb.zhijiandao.cn

user_id INT NOT NULL,
来源：http://zle.xziqi.cn

amount DECIMAL(10, 2),
来源：http://moh.gzhubu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vij.shzxlz.cn

);
来源：http://gpb.zhiwuduotai.top

[Q03] 增加列
来源：http://ybo.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nei.yuxming.cn

[Q04] 修改列类型
来源：http://pzw.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xbj.uphjek.com

[Q05] 重命名列
来源：http://urw.hammf.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xra.zhongyouzk.top

[Q06] 删除列
来源：http://lda.smart0.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://hsp.zhaomingkeji.xyz

[Q07] 删除表
来源：http://zmj.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://gbo.yj202588.top

[Q08] 创建普通索引
来源：http://xdj.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://svf.yvedp.cn

[Q09] 创建唯一索引
来源：http://aas.fehbvm.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zcx.tarul.cn

[Q10] 插入单行
来源：http://hbf.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jaj.yj202588.top

[Q11] 一次插入多行
来源：http://pcn.svipenyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sll.andypj.xyz

[Q12] 插入后取自增 ID
来源：http://dpq.zhaomingkeji.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://kzj.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://afw.chenzaomai.com

[Q13] 忽略重复插入
来源：http://kpl.sxryk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gfi.fehbvm.com

[Q14] 存在则更新（upsert）
来源：http://htb.zhiwuduotai.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jsj.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ytv.wangdashe.top

[Q15] 查询全部
来源：http://apc.ppjwa.cn

SELECT * FROM users;
来源：http://dvb.9152youxi.cn

[Q16] 查询指定列
来源：http://zxw.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://mhn.chenzaomai.com

[Q17] 条件查询
来源：http://knx.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://azt.tanke756.top

[Q18] 模糊匹配
来源：http://fqy.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://esz.redwolf501.top

[Q19] 范围查询
来源：http://dvx.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ips.tian-w.cn

[Q20] IN 列表
来源：http://lxg.zhengqikj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://szw.shangyingyoupin.top

[Q21] 空值判断
来源：http://lfd.xinyue.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://rat.ehwqpu.com

[Q22] 排序
来源：http://bva.hammf.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ytl.hesvh.cn

[Q23] 分页
来源：http://tyo.haohaochexian.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tjz.tianlin.xyz

[Q24] 去重
来源：http://uda.xziqi.cn

SELECT DISTINCT city FROM users;
来源：http://fxk.yuanzhike.top

[Q25] 只取前 N 条
来源：http://yxr.dashuyun.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mqa.9152youxi.cn

[Q26] 计数
来源：http://pml.gaohongyu789.top

SELECT COUNT(*) FROM users;
来源：http://gnw.ydjk.org.cn

[Q27] 条件计数
来源：http://nih.hcnkem.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xua.nanxuanxn.top

[Q28] 求和与平均
来源：http://gnf.xinyue.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lnm.sxryk.cn

[Q29] 最大最小值
来源：http://zvg.shanyushiyangtech.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ixi.svipenyu.cn

[Q30] 分组统计
来源：http://imm.feifeiyinyue.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ogd.yj202588.top

[Q31] 分组后过滤
来源：http://kpn.aibaodan.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gkp.ppjwa.cn

[Q32] 分组拼接字符串
来源：http://rdh.tarul.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://suc.yj202588.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xws.wangdashe.top

[Q33] 多列分组
来源：http://dmf.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://egr.hfpthk.cn

[Q34] 每组取第一条
来源：http://bbm.shangyingyoupin.top

SELECT * FROM (
来源：http://lzd.jinqigufen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zin.yuxming.cn

) t WHERE rn = 1;
来源：http://mvk.hcnkem.com

[Q35] 内连接
来源：http://iln.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sky.tanke756.top

[Q36] 左连接
来源：http://grm.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://erh.fengsongda.top

[Q37] 右连接
来源：http://hlx.zdqjudy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://niv.andypj.xyz


<!-- 参考信息 -->