代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mlg.sweek.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uyt.hongshengwenyu.top

C#:   // 手写递归，或 Array.Sort
来源：http://giy.zhoulong.xyz

[N04] 斐波那契数列
来源：http://bho.yj202588.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qsp.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://azc.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://may.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ktx.jqgufenzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ccz.wangshuangyany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sgi.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://isa.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lgy.xuanzx.com

[N05] 最大公约数
来源：http://pxn.yonumen.top

Py:   math.gcd(a, b)
来源：http://zkc.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://khc.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://voi.zhaomingkeji.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sez.gotoacloud.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cdh.snrcjt.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dnw.daxiang520.top

Ruby: a.gcd(b)
来源：http://nzv.hfpthk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://khb.hcnkem.com

[N06] 判断回文字符串
来源：http://zdc.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://tbh.andypj.xyz

PHP:  $s === strrev($s);
来源：http://xxu.yj20258888.top

JS:   s === [...s].reverse().join("")
来源：http://tur.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://cfj.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ycl.jqgfzy.top

Go:   // 双指针从两端比较
来源：http://yfg.ywan-chungtsiang.top

Ruby: s == s.reverse
来源：http://xau.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wue.shanyushiyangtech.top

[N07] 两数之和（返回下标）
来源：http://pcl.xylfe.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wmm.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uza.nanxinkj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wul.meibo888.top

TS:   // 手写 Map<string, number>
来源：http://ian.ctjpmb.com

Java: // 手写 HashMap
来源：http://fsl.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://mac.zhixingplan.top

Ruby: // 手写 Hash
来源：http://ymb.shangyingyoupin.top

C#:   // 手写 Dictionary<int, int>
来源：http://lse.ppjwa.cn

[N08] 生成全排列
来源：http://ghh.dianchejie.cn

Py:   itertools.permutations(arr)
来源：http://djm.tarul.cn

PHP:  // 手写递归交换
来源：http://hwk.zhiwuduotai.top

JS:   // 手写回溯递归
来源：http://dgt.fktsv.cn

TS:   // 手写回溯递归
来源：http://jzv.52xcode.cn

Java: // 手写回溯递归
来源：http://iwz.0kj1m.cn

Go:   // 手写回溯递归
来源：http://fwa.hfpthk.cn

Ruby: arr.permutation.to_a
来源：http://dhc.hcnkem.com

C#:   // 手写回溯递归
来源：http://udu.hnxiangtu.top

[N09] 栈与队列
来源：http://qtl.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cow.xylfe.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uso.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://plj.dianchejie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vtq.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bkj.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gnj.ctjpmb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://acm.sxryk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fua.yongpay.top

[N10] 链表节点定义
来源：http://xja.gzhubu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uwk.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://kyj.svipenyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ypo.hnxiangtu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vbc.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://wbm.bjfxy.top

Go:   type Node struct { V int; Next *Node }
来源：http://jdx.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://izk.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://xvo.iojbl.cn

[N11] 二叉树中序遍历
来源：http://mig.0kj1m.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nsr.zhengqikj.top

PHP:  // 手写递归函数
来源：http://yfc.wangshuangyany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://crw.zhoulong.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oat.fanxiaobao.xyz

Java: // 手写递归
来源：http://cqp.hfpthk.cn

Go:   // 手写递归
来源：http://moi.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qnf.zdqjudy.top

C#:   // 手写递归
来源：http://kfe.cheryme.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vwi.ppjwa.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eoz.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dsr.tarul.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yyo.yuanzhike.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lhv.jqgfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hro.shanyushiyangtech.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://new.havefunace.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ykb.sufxvd.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wtb.hysaishi.cn

================================================================================
来源：http://adq.shuidangran.top

O. 并发与异步
来源：http://dsn.iojbl.cn

================================================================================
来源：http://tfh.hongshengwenyu.top

[O01] 启动一个线程
来源：http://loc.vehdjk.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xzk.svipenyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xkp.ybcxt.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://biu.zdbjq.cn

TS:   // 同 JS
来源：http://znp.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://olc.dashuyun.cn

Go:   go f()
来源：http://jib.yongpay.top

Ruby: Thread.new { f }
来源：http://qbn.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://wbn.shuidangran.top

[O02] 使用线程池
来源：http://iqj.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yfm.jinghuilouyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pkc.yuxming.cn

JS:   // worker_threads 线程池
来源：http://gwq.tianlin.xyz

TS:   // worker_threads 线程池
来源：http://yte.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://dvg.jinyuanbaomall.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cvx.zhiwuduotai.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://okr.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gvp.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://fwy.hesvh.cn

Py:   with lock: shared += 1
来源：http://ehs.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://fdz.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vpy.wangdashe.top

TS:   // 同 JS
来源：http://ktm.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://wlc.yueranfly.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gey.zhiwuduotai.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xhf.52xcode.cn

C#:   lock (gate) { shared++; }
来源：http://njt.meibo888.top

[O04] 定义异步函数并等待
来源：http://szf.zhixingplan.top

Py:   async def f():⏎    await g()
来源：http://khr.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xad.jinyuanbaomall.cn

JS:   async function f() { await g(); }
来源：http://dne.epnwcf.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://jmj.jiagoushi.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vwq.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qzg.ehwqpu.com

Ruby: # 用 Fiber 或 async gem
来源：http://fee.zdbjq.cn

C#:   async Task F() { await G(); }
来源：http://wqq.zhengqikj.top

[O05] 并发执行并等待全部完成
来源：http://upj.yj20258888.top

Py:   asyncio.gather(*tasks)
来源：http://hzz.xuetiantiany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bfi.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://zpd.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://gmo.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sct.ydzc1.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ioj.hongshengwenyu.top

Ruby: threads.map(&:join)
来源：http://mjy.daxiang520.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mrf.zdbjq.cn

[O06] 使用进程池
来源：http://fvp.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://djs.ctjpmb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ifk.316326.xyz

JS:   // child_process / cluster 模块
来源：http://npn.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://lbx.quarkkingdee.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eno.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jhg.yangfankeji.com

Ruby: // fork 块
来源：http://lia.fzhhl.top

C#:   Parallel.For
来源：http://yfs.jlsjyb.cn

================================================================================
来源：http://hah.fehbvm.com

P. 常用工具函数
来源：http://ven.ppjwa.cn

================================================================================
来源：http://hrf.jinghuilouyu.cn

[P01] 生成 UUID
来源：http://tdl.jqgfzy.top

Py:   str(uuid.uuid4())
来源：http://uqf.zhiwuduotai.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vyh.mhx1999.top

JS:   crypto.randomUUID()
来源：http://nur.dashuyun.cn

TS:   crypto.randomUUID()
来源：http://oyb.0kj1m.cn

Java: UUID.randomUUID().toString()
来源：http://cxv.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://emi.hongshengwenyu.top

Ruby: SecureRandom.uuid
来源：http://scn.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://qgv.yuanzhike.top

[P02] MD5 / SHA256 摘要
来源：http://bir.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xzv.cashguo.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hlx.gogol.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hyx.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tsj.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uvl.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mit.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mup.hfpthk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wdr.xinyue.icu

[P03] 生成短随机字符串
来源：http://jfk.feifeiyinyue.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hef.svipenyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yfl.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vhz.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://thy.daria6918.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tky.shanyushiyangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://meq.zhoulong.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://qqy.jqgufenzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cae.zdqjudy.top

[P04] 求长度
来源：http://bqf.ivvv.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mgo.tianlin.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mco.tian-w.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pke.vehdjk.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rsq.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://rdk.cucudq.cn

Go:   len(arr);  len(m)
来源：http://ikc.cdnleiting.top

Ruby: x.length;  x.size
来源：http://wje.yj202588.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ddq.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://tfa.0kj1m.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fiq.fktsv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://psp.gzhubu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ysb.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jwz.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nsr.daria6918.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qdy.9152youxi.cn

Ruby: a == b
来源：http://wos.sweek.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://awv.jyoumei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xfl.aizwys.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://acx.shanyushiyangkeji.top

PHP:  if (empty($x)) {}
来源：http://dsg.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qew.snrcjt.cn

TS:   if (x == null) {}
来源：http://eeg.feifeiyinyue.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jos.dashuyun.cn

Go:   if x == nil {}
来源：http://vge.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gil.c1oappe.top

C#:   if (x is null) {}
来源：http://ove.9152youxi.cn

[P07] 防抖与节流
来源：http://sti.chenjidiqi.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bsa.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://rbv.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cpx.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://byo.yongpay.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kya.jqgufenzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://glw.hesvh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yhv.tian-w.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iwa.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://qza.kuanghao11.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://get.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gkx.pycfn.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ybn.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://goe.yj20258.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lhb.ybcxt.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iij.52xcode.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zzm.bjfxy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zcg.tarul.cn

================================================================================
来源：http://mqs.gotoacloud.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wwe.shangyingyoupin.top

================================================================================
来源：http://fat.nwbrower.top

[Q01] 创建表
来源：http://myn.gogol.net.cn

CREATE TABLE users (
来源：http://agp.yj20258888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://amq.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://ofv.sysykeji.top

email VARCHAR(100) UNIQUE,
来源：http://cef.snrcjt.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kah.jyoumei.cn

);
来源：http://scp.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://sqn.pycfn.com

CREATE TABLE orders (
来源：http://qeu.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zxe.ydjk.org.cn

user_id INT NOT NULL,
来源：http://ukj.0kj1m.cn

amount DECIMAL(10, 2),
来源：http://wii.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://swm.zhaomingkeji.xyz

);
来源：http://nzf.yfazqb.com

[Q03] 增加列
来源：http://pjc.hesvh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jwq.yj20258.top

[Q04] 修改列类型
来源：http://ysa.nanxinkj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tcw.wangshuangyany.cn

[Q05] 重命名列
来源：http://xlq.yj202588.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vgn.hnqzz.top

[Q06] 删除列
来源：http://mrj.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cuk.shangyingyoupin.top

[Q07] 删除表
来源：http://foz.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://srt.vqdsnc.cn

[Q08] 创建普通索引
来源：http://ypg.dianchejie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ioc.bjfxy.top

[Q09] 创建唯一索引
来源：http://tpu.pycfn.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fhf.bbcook.cn

[Q10] 插入单行
来源：http://yaq.yj20258.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://org.tianlin.xyz

[Q11] 一次插入多行
来源：http://egb.hesvh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://czj.mhx1999.top

[Q12] 插入后取自增 ID
来源：http://qci.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://jvh.jinqigufen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xwc.nanxinkj.top

[Q13] 忽略重复插入
来源：http://tqu.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gvv.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://tvy.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rie.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lri.guannengcc.top

[Q15] 查询全部
来源：http://mdt.cdnleiting.top

SELECT * FROM users;
来源：http://ddo.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://anp.pycfn.com

SELECT id, name FROM users;
来源：http://iui.yuxming.cn

[Q17] 条件查询
来源：http://ecz.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lzj.shzxlz.cn

[Q18] 模糊匹配
来源：http://oyi.fktsv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jym.jqgufenzy.top

[Q19] 范围查询
来源：http://jqt.yonumen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://odp.yvedp.cn

[Q20] IN 列表
来源：http://nkn.dashuyun.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kdn.yfazqb.com

[Q21] 空值判断
来源：http://cxv.havefunace.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zph.daxiang520.top

[Q22] 排序
来源：http://gag.hesvh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ycd.yj20258.top

[Q23] 分页
来源：http://jwm.birdmap.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tnk.jinyuanbaomall.cn

[Q24] 去重
来源：http://aox.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://xkd.tarul.cn

[Q25] 只取前 N 条
来源：http://zft.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fyo.jiagoushi.top

[Q26] 计数
来源：http://ozs.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://qdt.ivvv.top

[Q27] 条件计数
来源：http://bgf.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://trq.cucudq.cn

[Q28] 求和与平均
来源：http://jgn.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ten.cucudq.cn

[Q29] 最大最小值
来源：http://ibk.zhaomingkeji.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://nta.guannengcc.top

[Q30] 分组统计
来源：http://xbn.cashguo.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cff.cheryme.top

[Q31] 分组后过滤
来源：http://dfe.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tba.zhaomingkeji.xyz

[Q32] 分组拼接字符串
来源：http://lrf.snrcjt.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jip.hywenlv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eqo.cashguo.top

[Q33] 多列分组
来源：http://hza.hysaishi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fjm.haohaochexian.top

[Q34] 每组取第一条
来源：http://heo.tianlin.xyz

SELECT * FROM (
来源：http://axs.nanxinkj.top


<!-- 参考信息 -->