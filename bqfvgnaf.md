代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ddu.hysaishi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kyv.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://gvb.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vtc.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://obm.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://lzl.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://ovw.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://anf.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lyw.tarul.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vfb.c1oappe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fdd.yangfankeji.com

Go:   slices.Sort(arr)
来源：http://ynu.zhengqikj.top

Ruby: arr.sort
来源：http://lqf.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://iwf.hammf.cn

[N03] 快速排序（分治示例）
来源：http://gpj.ydzc1.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://krn.hcnkem.com

PHP:  // 递归实现，或用 usort
来源：http://imp.ybcxt.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nlr.jqgufenzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://unn.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jgk.zhijiandao.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rus.haohaochexian.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vyy.jlsjyb.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nxb.jqgfzy.top

[N04] 斐波那契数列
来源：http://ytx.quarkkingdee.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cee.yueranfly.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tdu.zhongyouzk.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pnn.pycfn.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yqu.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ixi.xuetiantiany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hpj.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ghq.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jgh.aizwys.cn

[N05] 最大公约数
来源：http://njc.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://udf.zycfv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oen.dashuyun.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rpc.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jeq.yangfankeji.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vwl.fzhhl.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nck.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://plw.yfazqb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gxd.ydzc1.top

[N06] 判断回文字符串
来源：http://xpb.jinqigfzy.top

Py:   s == s[::-1]
来源：http://law.hnxiangtu.top

PHP:  $s === strrev($s);
来源：http://pjq.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://yei.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://uig.shzxlz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fnv.ywan-chungtsiang.top

Go:   // 双指针从两端比较
来源：http://rvp.uphjek.com

Ruby: s == s.reverse
来源：http://bou.sufxvd.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tkt.0kj1m.cn

[N07] 两数之和（返回下标）
来源：http://ula.gogol.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kkl.wangdashe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hhu.ppjwa.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rbp.pycfn.com

TS:   // 手写 Map<string, number>
来源：http://kco.sjlbkw.cn

Java: // 手写 HashMap
来源：http://eka.svipenyu.cn

Go:   // 手写 map[int]int
来源：http://jfu.gotoacloud.top

Ruby: // 手写 Hash
来源：http://cgf.hysaishi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rnu.hysaishi.cn

[N08] 生成全排列
来源：http://xti.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://spj.sjlbkw.cn

PHP:  // 手写递归交换
来源：http://gep.316326.xyz

JS:   // 手写回溯递归
来源：http://yey.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://nte.mhx1999.top

Java: // 手写回溯递归
来源：http://lsx.andypj.xyz

Go:   // 手写回溯递归
来源：http://eje.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://lkr.haohaochexian.top

C#:   // 手写回溯递归
来源：http://hjj.hammf.cn

[N09] 栈与队列
来源：http://lgv.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fwf.zdqjudy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dgo.zhengqikj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nzt.shangyingyoupin.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kcq.birdmap.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://llr.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://awx.hnqzz.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dse.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bqz.birdmap.top

[N10] 链表节点定义
来源：http://tiv.zhiwuduotai.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pne.jqgfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://use.yj20258888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://afr.cashguo.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jor.chenjidiqi.icu

Java: class Node { int v; Node next; }
来源：http://mkg.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://ebi.hfpthk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dfc.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zvf.chenlongwang.top

[N11] 二叉树中序遍历
来源：http://icm.sweek.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tkk.chenjidiqi.icu

PHP:  // 手写递归函数
来源：http://nrh.hnxiangtu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xvy.feifeiyinyue.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bbf.0kj1m.cn

Java: // 手写递归
来源：http://tsj.sjlbkw.cn

Go:   // 手写递归
来源：http://vci.haohaochexian.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dsg.hcnkem.com

C#:   // 手写递归
来源：http://lfc.9152youxi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pup.jqgfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ndr.zhiwuduotai.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://znl.tianlin.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ixb.yangfankeji.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xrm.tanke756.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tmc.xingfuxueyuan.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mpd.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yjd.aibaodan.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dlv.nwbrower.top

================================================================================
来源：http://yww.vehdjk.com

O. 并发与异步
来源：http://ete.pycfn.com

================================================================================
来源：http://jml.iojbl.cn

[O01] 启动一个线程
来源：http://lbs.pycfn.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bnk.ydzc1.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jmj.zhaomingkeji.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blx.zhijiandao.cn

TS:   // 同 JS
来源：http://fmj.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://old.sxryk.cn

Go:   go f()
来源：http://cdk.ehwqpu.com

Ruby: Thread.new { f }
来源：http://hcb.jinqigufen.top

C#:   Task.Run(() => F());
来源：http://fuu.sysykeji.top

[O02] 使用线程池
来源：http://roi.zhixingplan.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hvo.yongpay.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ewx.sweek.top

JS:   // worker_threads 线程池
来源：http://tqz.andypj.xyz

TS:   // worker_threads 线程池
来源：http://tbp.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://ehk.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xgn.ydzc1.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://org.guannengcc.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hwt.xuanzx.com

[O03] 加锁保护共享数据
来源：http://rnr.zdqjudy.top

Py:   with lock: shared += 1
来源：http://qql.yueranfly.top

PHP:  // 用 flock() 做文件锁
来源：http://sie.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hqw.yj202588.top

TS:   // 同 JS
来源：http://leo.ctjpmb.com

Java: synchronized (this) { shared++; }
来源：http://nsv.xinyue.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oin.jinqigufen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xzc.yongpay.top

C#:   lock (gate) { shared++; }
来源：http://nax.jinqigufen.top

[O04] 定义异步函数并等待
来源：http://vly.gaohongyu789.top

Py:   async def f():⏎    await g()
来源：http://bdx.nanxinkj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jdr.shzxlz.cn

JS:   async function f() { await g(); }
来源：http://koe.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gnq.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://syz.fengsongda.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vws.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bpl.zhaomingkeji.xyz

C#:   async Task F() { await G(); }
来源：http://wyx.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://nxo.jqgufenzy.top

Py:   asyncio.gather(*tasks)
来源：http://gny.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hib.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://ylx.hcnkem.com

TS:   await Promise.all(tasks)
来源：http://sml.xylfe.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tyl.pengpengdd.cyou

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hws.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://eyh.bbcook.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mxy.uphjek.com

[O06] 使用进程池
来源：http://ney.xinyue.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ayp.hnxiangtu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mtn.meibo888.top

JS:   // child_process / cluster 模块
来源：http://tcr.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://ivx.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dyq.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tfy.aizwys.cn

Ruby: // fork 块
来源：http://vjp.cdnleiting.top

C#:   Parallel.For
来源：http://zod.jyoumei.cn

================================================================================
来源：http://toj.tian-w.cn

P. 常用工具函数
来源：http://har.shuidangran.top

================================================================================
来源：http://sgk.wangdashe.top

[P01] 生成 UUID
来源：http://cbc.ybcxt.top

Py:   str(uuid.uuid4())
来源：http://wug.aizwys.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dga.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://zfb.hnqzz.top

TS:   crypto.randomUUID()
来源：http://ewx.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://zgo.shzxlz.cn

Go:   // 用 github.com/google/uuid
来源：http://sma.xylfe.cn

Ruby: SecureRandom.uuid
来源：http://jbm.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://ovj.jqgufenzy.top

[P02] MD5 / SHA256 摘要
来源：http://sms.zdqjudy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eao.meibo888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yuc.gaohongyu789.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gca.316326.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://amn.hongshengwenyu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://akn.jinghuilouyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xfl.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pix.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jiz.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://arj.sweek.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ykd.9152youxi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ard.dashuyun.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hji.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aoe.snrcjt.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vzk.xziqi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dhy.jyoumei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://chg.jinghuilouyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eld.andypj.xyz

[P04] 求长度
来源：http://rmd.jinqigufen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lhb.pycfn.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dve.zhijiandao.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jwt.shuidangran.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zsh.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://bgb.cqqwz.cn

Go:   len(arr);  len(m)
来源：http://lgl.meibo888.top

Ruby: x.length;  x.size
来源：http://ihu.meibo888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mef.shangyingyoupin.top

[P05] 判断两个对象内容是否相等
来源：http://kxu.fzhhl.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zcf.yvedp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vpb.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ycp.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dbl.zhijiandao.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nay.quarkkingdee.top

Go:   reflect.DeepEqual(a, b)
来源：http://lkk.zhixingplan.top

Ruby: a == b
来源：http://vhr.fanxiaobao.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dpo.jiagoushi.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qtt.shanyushiyangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wmi.smart0.xyz

PHP:  if (empty($x)) {}
来源：http://pux.yuanzhike.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qol.chenzaomai.com

TS:   if (x == null) {}
来源：http://fka.ctjpmb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://tld.hysaishi.cn

Go:   if x == nil {}
来源：http://vog.yonumen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nwf.xuanzx.com

C#:   if (x is null) {}
来源：http://tka.chenlongwang.top

[P07] 防抖与节流
来源：http://mlw.xinyue.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tcv.tanke756.top

PHP:  // 手写时间戳比较
来源：http://xet.havefunace.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://doh.wangshuangyany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://que.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bts.yj202588.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iwz.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ddw.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ynx.yueranfly.top

[P08] 处理浮点精度问题
来源：http://hqe.tianlin.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rfz.kuanghao11.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://faq.tian-w.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yni.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lwf.xingfuxueyuan.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://chb.fengsongda.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xjl.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tvt.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gmt.cashguo.top

================================================================================
来源：http://ljf.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kyd.zhengqikj.top

================================================================================
来源：http://zzq.smart0.xyz

[Q01] 创建表
来源：http://xjd.smart0.xyz

CREATE TABLE users (
来源：http://pas.zhijiandao.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jrk.feifeiyinyue.top

name VARCHAR(50) NOT NULL,
来源：http://cct.xinyue.icu

email VARCHAR(100) UNIQUE,
来源：http://obn.jianghu66.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aug.aibaodan.cn

);
来源：http://vse.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://ooq.ywan-chungtsiang.top

CREATE TABLE orders (
来源：http://ogy.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ute.316326.xyz

user_id INT NOT NULL,
来源：http://jol.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://rcn.aibaodan.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sdr.zhaomingkeji.xyz

);
来源：http://vjc.yj20258.top

[Q03] 增加列
来源：http://fjq.ywan-chungtsiang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rzz.svipenyu.cn

[Q04] 修改列类型
来源：http://rcz.hongshengwenyu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cuf.chenjidiqi.icu

[Q05] 重命名列
来源：http://lft.sweek.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zbg.zdbjq.cn

[Q06] 删除列
来源：http://bjj.zhijiandao.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ayj.bbcook.cn

[Q07] 删除表
来源：http://iqt.fehbvm.com

DROP TABLE IF EXISTS orders;
来源：http://exa.xylfe.cn

[Q08] 创建普通索引
来源：http://cmr.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pfq.gaohongyu789.top

[Q09] 创建唯一索引
来源：http://nnw.9152youxi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hsy.shanyushiyangtech.top

[Q10] 插入单行
来源：http://vjc.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rze.chenlongwang.top

[Q11] 一次插入多行
来源：http://yff.cqqwz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qjt.jqgfzy.top

[Q12] 插入后取自增 ID
来源：http://ayn.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://fbi.sweek.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mnf.ybcxt.top

[Q13] 忽略重复插入
来源：http://dsx.sweek.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jtz.hysaishi.cn

[Q14] 存在则更新（upsert）
来源：http://wbn.jinyuanbaomall.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gbu.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jsn.jianghu66.top

[Q15] 查询全部
来源：http://tdh.yj20258888.top

SELECT * FROM users;
来源：http://svv.snrcjt.cn

[Q16] 查询指定列
来源：http://wqq.cheryme.top

SELECT id, name FROM users;
来源：http://iwa.smart0.xyz

[Q17] 条件查询
来源：http://oji.ivvv.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pqs.zhaomingkeji.xyz

[Q18] 模糊匹配
来源：http://oep.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vnm.havefunace.top

[Q19] 范围查询
来源：http://mez.hcnkem.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kuq.yj202588.top

[Q20] IN 列表
来源：http://tcn.vqdsnc.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tcr.wangshuangyany.cn

[Q21] 空值判断
来源：http://nhj.tianlin.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://nmd.svipenyu.cn

[Q22] 排序
来源：http://ccl.quarkkingdee.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uuj.316326.xyz

[Q23] 分页
来源：http://wzz.xinyue.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wpm.0kj1m.cn

[Q24] 去重
来源：http://fnf.hnqzz.top

SELECT DISTINCT city FROM users;
来源：http://ihd.svipenyu.cn

[Q25] 只取前 N 条
来源：http://ipg.yj20258.top


<!-- 参考信息 -->