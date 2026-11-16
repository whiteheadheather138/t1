代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://skr.sufxvd.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gmv.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gnv.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wki.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wmr.daxiang520.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gwe.gotoacloud.top

C#:   // 手写递归，或 Array.Sort
来源：http://pju.jinghuilouyu.cn

[N04] 斐波那契数列
来源：http://dbb.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zid.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iha.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zmh.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fot.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qrx.yj202588.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xxq.ybcxt.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://enj.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yxo.sjlbkw.cn

[N05] 最大公约数
来源：http://ikl.iojbl.cn

Py:   math.gcd(a, b)
来源：http://kdy.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qjj.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://btq.chenlongwang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hmj.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nri.yj202588.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yix.gaohongyu789.top

Ruby: a.gcd(b)
来源：http://qnq.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yja.xziqi.cn

[N06] 判断回文字符串
来源：http://kne.tanke756.top

Py:   s == s[::-1]
来源：http://hah.xinyue.icu

PHP:  $s === strrev($s);
来源：http://ogj.zdqjudy.top

JS:   s === [...s].reverse().join("")
来源：http://jfp.sysykeji.top

TS:   s === [...s].reverse().join("")
来源：http://vjg.haohaochexian.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dpl.ywan-chungtsiang.top

Go:   // 双指针从两端比较
来源：http://aff.cashguo.top

Ruby: s == s.reverse
来源：http://ejn.nanxuanxn.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jiz.daxiang520.top

[N07] 两数之和（返回下标）
来源：http://ixo.zhoulong.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ejg.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://smx.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hwm.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://hau.yuanzhike.top

Java: // 手写 HashMap
来源：http://hca.yfazqb.com

Go:   // 手写 map[int]int
来源：http://czr.ybcxt.top

Ruby: // 手写 Hash
来源：http://ons.jinqigfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://lwt.hysaishi.cn

[N08] 生成全排列
来源：http://ujq.chenzaomai.com

Py:   itertools.permutations(arr)
来源：http://avw.daria6918.cn

PHP:  // 手写递归交换
来源：http://irr.sjlbkw.cn

JS:   // 手写回溯递归
来源：http://sgn.havefunace.top

TS:   // 手写回溯递归
来源：http://avr.yj20258888.top

Java: // 手写回溯递归
来源：http://won.epnwcf.com

Go:   // 手写回溯递归
来源：http://kyi.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://sdn.9152youxi.cn

C#:   // 手写回溯递归
来源：http://pfx.gaohongyu789.top

[N09] 栈与队列
来源：http://xvi.jyoumei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sib.guowangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vov.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hxs.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pzg.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://srs.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mvp.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mck.meibo888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kle.fehbvm.com

[N10] 链表节点定义
来源：http://lay.zhijiandao.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xwr.hongshengwenyu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xto.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xrn.sufxvd.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://goj.ydzc1.top

Java: class Node { int v; Node next; }
来源：http://tde.vehdjk.com

Go:   type Node struct { V int; Next *Node }
来源：http://jiw.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yse.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vjj.gzhubu.top

[N11] 二叉树中序遍历
来源：http://gqi.shangyingyoupin.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lkj.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://eey.cucudq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://glu.yangfankeji.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kgh.kuanghao11.cn

Java: // 手写递归
来源：http://mse.yj20258888.top

Go:   // 手写递归
来源：http://ofm.iojbl.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://apn.gotoacloud.top

C#:   // 手写递归
来源：http://pdf.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fra.hammf.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bny.tarul.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://alq.cashguo.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lta.vehdjk.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://scw.nanxinkj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jty.jqgufenzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ljp.birdmap.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nbr.yj20258.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cot.0kj1m.cn

================================================================================
来源：http://coq.c1oappe.top

O. 并发与异步
来源：http://cem.pengpengdd.cyou

================================================================================
来源：http://ehu.shuidangran.top

[O01] 启动一个线程
来源：http://myr.birdmap.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ece.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zur.shanyushiyangtech.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tqc.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://zmo.daria6918.cn

Java: new Thread(() -> f()).start()
来源：http://xzy.dashuyun.cn

Go:   go f()
来源：http://wsx.sxryk.cn

Ruby: Thread.new { f }
来源：http://frb.hfpthk.cn

C#:   Task.Run(() => F());
来源：http://uum.cqqwz.cn

[O02] 使用线程池
来源：http://ccm.jianghu66.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pvp.yuanzhike.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tdz.redwolf501.top

JS:   // worker_threads 线程池
来源：http://upy.guowangkeji.top

TS:   // worker_threads 线程池
来源：http://ely.fanxiaobao.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://gqd.wangdashe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iel.shangyingyoupin.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mly.meibo888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gdx.pycfn.com

[O03] 加锁保护共享数据
来源：http://nbz.hammf.cn

Py:   with lock: shared += 1
来源：http://sfv.sufxvd.cn

PHP:  // 用 flock() 做文件锁
来源：http://jie.xingfuxueyuan.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jdi.xuanzx.com

TS:   // 同 JS
来源：http://omd.aibaodan.cn

Java: synchronized (this) { shared++; }
来源：http://qbv.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fev.hesvh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://csj.shzxlz.cn

C#:   lock (gate) { shared++; }
来源：http://zex.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://eow.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://sqo.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vhf.tian-w.cn

JS:   async function f() { await g(); }
来源：http://mof.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pad.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://god.gaohongyu789.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iwp.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://thz.52xcode.cn

C#:   async Task F() { await G(); }
来源：http://mlg.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://qnv.yvedp.cn

Py:   asyncio.gather(*tasks)
来源：http://trn.redwolf501.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ckd.nwbrower.top

JS:   await Promise.all(tasks)
来源：http://yyu.feifeiyinyue.top

TS:   await Promise.all(tasks)
来源：http://xtz.zdqjudy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://djs.yangfankeji.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kew.guowangkeji.top

Ruby: threads.map(&:join)
来源：http://hdq.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://oob.cdnleiting.top

[O06] 使用进程池
来源：http://qzj.zdbjq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mtj.bbcook.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://avc.nanxinkj.top

JS:   // child_process / cluster 模块
来源：http://dsg.ivvv.top

TS:   // child_process / cluster 模块
来源：http://kdm.xinyue.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oxm.hcnkem.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nta.sufxvd.cn

Ruby: // fork 块
来源：http://srk.wangdashe.top

C#:   Parallel.For
来源：http://cyg.mhx1999.top

================================================================================
来源：http://rse.ydjk.org.cn

P. 常用工具函数
来源：http://afg.jinghuilouyu.cn

================================================================================
来源：http://siu.zhoulong.xyz

[P01] 生成 UUID
来源：http://wuu.gzhubu.top

Py:   str(uuid.uuid4())
来源：http://dct.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://omb.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://toy.cashguo.top

TS:   crypto.randomUUID()
来源：http://xus.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://dlx.zdbjq.cn

Go:   // 用 github.com/google/uuid
来源：http://ljo.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://vdx.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://fxq.smart0.xyz

[P02] MD5 / SHA256 摘要
来源：http://jyl.pengpengdd.cyou

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cte.gogol.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vyj.zdqjudy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://obv.dianchejie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bnl.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rpt.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zgo.jinqigfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rax.svipenyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ida.cqqwz.cn

[P03] 生成短随机字符串
来源：http://sun.shangyingyoupin.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://djg.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qcu.iojbl.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vdp.shangyingyoupin.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://irv.shangyingyoupin.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lmo.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gbn.gotoacloud.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://abt.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qbx.ppjwa.cn

[P04] 求长度
来源：http://lap.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nha.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jij.smart0.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yxk.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fdt.jinqigfzy.top

Java: list.size();  map.size();  s.length()
来源：http://tou.fehbvm.com

Go:   len(arr);  len(m)
来源：http://uck.wangdashe.top

Ruby: x.length;  x.size
来源：http://abf.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ghp.yanxiufei.cn

[P05] 判断两个对象内容是否相等
来源：http://rvw.hammf.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yyi.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jdn.yj20258888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mce.yvedp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://exc.aizwys.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://she.meibo888.top

Go:   reflect.DeepEqual(a, b)
来源：http://dtr.yj20258888.top

Ruby: a == b
来源：http://cau.fzhhl.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://omy.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sgb.yangfankeji.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://keb.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://gbb.guannengcc.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vpe.daxiang520.top

TS:   if (x == null) {}
来源：http://vmi.zhiwuduotai.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mdr.0kj1m.cn

Go:   if x == nil {}
来源：http://erh.bjfxy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vyn.wangshuangyany.cn

C#:   if (x is null) {}
来源：http://fft.hysaishi.cn

[P07] 防抖与节流
来源：http://xzf.hcnkem.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://suc.daria6918.cn

PHP:  // 手写时间戳比较
来源：http://dpk.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dyk.shanyushiyangtech.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wvu.yuxming.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tza.zhaomingkeji.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ewy.quarkkingdee.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ccz.nanxuanxn.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ixh.zhoulong.xyz

[P08] 处理浮点精度问题
来源：http://mgl.yangfankeji.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uza.hnxiangtu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gxz.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zlx.tian-w.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://drk.zdbjq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wox.zhijiandao.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uxz.jinqigfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baq.yuanzhike.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gsp.fehbvm.com

================================================================================
来源：http://oob.sweek.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pyn.gzhubu.top

================================================================================
来源：http://czy.guannengcc.top

[Q01] 创建表
来源：http://pkx.sjlbkw.cn

CREATE TABLE users (
来源：http://lbj.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blo.nanxuanxn.top

name VARCHAR(50) NOT NULL,
来源：http://lee.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://vyr.zhijiandao.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zlh.tianlin.xyz

);
来源：http://sfe.ydjk.org.cn

[Q02] 创建带外键的表
来源：http://iln.svipenyu.cn

CREATE TABLE orders (
来源：http://hhl.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mbp.hfpthk.cn

user_id INT NOT NULL,
来源：http://tav.sysykeji.top

amount DECIMAL(10, 2),
来源：http://ycx.jlsjyb.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xyd.zhoulong.xyz

);
来源：http://vey.redwolf501.top

[Q03] 增加列
来源：http://hbj.shangyingyoupin.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hne.hywenlv.cn

[Q04] 修改列类型
来源：http://rqw.c1oappe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vxn.aibaodan.cn

[Q05] 重命名列
来源：http://kqf.shangyingyoupin.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fxq.pengpengdd.cyou

[Q06] 删除列
来源：http://dbh.nanxuanxn.top

ALTER TABLE users DROP COLUMN age;
来源：http://nbj.zdqjudy.top

[Q07] 删除表
来源：http://wko.gotoacloud.top

DROP TABLE IF EXISTS orders;
来源：http://pbr.zhixingplan.top

[Q08] 创建普通索引
来源：http://czx.havefunace.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fum.zycfv.cn

[Q09] 创建唯一索引
来源：http://thl.yuxming.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://azo.yj20258.top

[Q10] 插入单行
来源：http://hdc.hywenlv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wsl.redwolf501.top

[Q11] 一次插入多行
来源：http://vrz.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zid.ehwqpu.com

[Q12] 插入后取自增 ID
来源：http://qsc.uphjek.com

INSERT INTO users (name) VALUES ('C');
来源：http://mis.zdqjudy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bqu.jqgfzy.top

[Q13] 忽略重复插入
来源：http://jde.c1oappe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gef.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://cla.shanyushiyangtech.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://elz.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pvl.svipenyu.cn

[Q15] 查询全部
来源：http://lvn.jinqigufen.top

SELECT * FROM users;
来源：http://oeb.shanyushiyangkeji.top

[Q16] 查询指定列
来源：http://lqk.hfpthk.cn

SELECT id, name FROM users;
来源：http://fpx.tianlin.xyz

[Q17] 条件查询
来源：http://gcn.hongshengwenyu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://erc.yongpay.top

[Q18] 模糊匹配
来源：http://hnc.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jbj.haohaochexian.top

[Q19] 范围查询
来源：http://bsj.yfazqb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://byv.birdmap.top

[Q20] IN 列表
来源：http://qih.havefunace.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gbg.quarkkingdee.top

[Q21] 空值判断
来源：http://dpn.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://aqg.jianghu66.top

[Q22] 排序
来源：http://hsd.jinqigufen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ylj.hysaishi.cn

[Q23] 分页
来源：http://smn.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nsv.chenjidiqi.icu

[Q24] 去重
来源：http://sqe.hnqzz.top

SELECT DISTINCT city FROM users;
来源：http://dxf.haohaochexian.top

[Q25] 只取前 N 条
来源：http://rfk.yuxming.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tyy.guowangkeji.top

[Q26] 计数
来源：http://xxt.gogol.net.cn

SELECT COUNT(*) FROM users;
来源：http://rmc.bjfxy.top

[Q27] 条件计数
来源：http://npr.xingfuxueyuan.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oju.hfpthk.cn

[Q28] 求和与平均
来源：http://xrp.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://agf.hammf.cn

[Q29] 最大最小值
来源：http://gyo.vehdjk.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://iau.yonumen.top

[Q30] 分组统计
来源：http://jua.yongpay.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lza.yuxming.cn

[Q31] 分组后过滤
来源：http://nhb.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oqn.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://yva.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rgu.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iox.meibo888.top


<!-- 参考信息 -->