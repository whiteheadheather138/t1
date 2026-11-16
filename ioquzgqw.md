代发 wailian999

[N01] 二分查找（有序数组）
来源：http://pmp.sufxvd.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wec.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tks.yongpay.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xfj.ydjk.org.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hoj.52xcode.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hgv.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://bnl.jqgufenzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qfw.fengsongda.top

C#:   Array.BinarySearch(arr, x)
来源：http://azt.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://odu.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://foi.ivvv.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yfp.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://phl.cqqwz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tmk.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xyg.gaohongyu789.top

Go:   slices.Sort(arr)
来源：http://ngc.yangfankeji.com

Ruby: arr.sort
来源：http://spa.zdbjq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ziv.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://pkp.c1oappe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mhf.yuxming.cn

PHP:  // 递归实现，或用 usort
来源：http://omt.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sev.cqqwz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wez.nwbrower.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gxr.uphjek.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rin.pengpengdd.cyou

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mfa.birdmap.top

C#:   // 手写递归，或 Array.Sort
来源：http://alu.ybcxt.top

[N04] 斐波那契数列
来源：http://sgb.bbcook.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://avz.9152youxi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://puf.guowangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://isu.fanxiaobao.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://awu.cdnleiting.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://weq.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yhd.xinyue.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wss.xylfe.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ddu.gaohongyu789.top

[N05] 最大公约数
来源：http://suy.bjfxy.top

Py:   math.gcd(a, b)
来源：http://hbv.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bef.pycfn.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ecy.shuidangran.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cor.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dvy.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mch.ppjwa.cn

Ruby: a.gcd(b)
来源：http://urr.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fod.cdnleiting.top

[N06] 判断回文字符串
来源：http://rky.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://xni.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://hyr.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://fov.zdbjq.cn

TS:   s === [...s].reverse().join("")
来源：http://jdi.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ttb.pycfn.com

Go:   // 双指针从两端比较
来源：http://rgg.andypj.xyz

Ruby: s == s.reverse
来源：http://gfq.tianlin.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://pps.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://ofz.xuetiantiany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ylh.chenlongwang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vla.uphjek.com

JS:   // 手写 Map：map.set(v, i)
来源：http://vhf.zhongyouzk.top

TS:   // 手写 Map<string, number>
来源：http://wfx.smart0.xyz

Java: // 手写 HashMap
来源：http://gsa.nwbrower.top

Go:   // 手写 map[int]int
来源：http://hms.pycfn.com

Ruby: // 手写 Hash
来源：http://glk.yuanzhike.top

C#:   // 手写 Dictionary<int, int>
来源：http://qtw.ivvv.top

[N08] 生成全排列
来源：http://ypd.hywenlv.cn

Py:   itertools.permutations(arr)
来源：http://ydh.hnqzz.top

PHP:  // 手写递归交换
来源：http://vbn.yuanzhike.top

JS:   // 手写回溯递归
来源：http://nfo.xuetiantiany.cn

TS:   // 手写回溯递归
来源：http://sxw.hysaishi.cn

Java: // 手写回溯递归
来源：http://ihz.iojbl.cn

Go:   // 手写回溯递归
来源：http://ukd.meibo888.top

Ruby: arr.permutation.to_a
来源：http://jxi.mhx1999.top

C#:   // 手写回溯递归
来源：http://czm.ywan-chungtsiang.top

[N09] 栈与队列
来源：http://ivi.aizwys.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ggy.zycfv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eoy.mhx1999.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kph.shanyushiyangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://brp.bbcook.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bkz.shzxlz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://idz.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qvd.fehbvm.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ciq.sysykeji.top

[N10] 链表节点定义
来源：http://vpn.guowangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://agi.jinqigfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://upa.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://orm.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nrl.chenjidiqi.icu

Java: class Node { int v; Node next; }
来源：http://vxl.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://yyv.ybcxt.top

Ruby: Node = Struct.new(:v, :next)
来源：http://fer.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gwq.yj202588.top

[N11] 二叉树中序遍历
来源：http://kop.fanxiaobao.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://twj.nanxinkj.top

PHP:  // 手写递归函数
来源：http://pdb.jinyuanbaomall.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yoi.cdnleiting.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gzw.ctjpmb.com

Java: // 手写递归
来源：http://tgu.gaohongyu789.top

Go:   // 手写递归
来源：http://hce.zdbjq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sje.chenjidiqi.icu

C#:   // 手写递归
来源：http://geg.daxiang520.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rfk.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://huo.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pyf.yj20258.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://net.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jfx.zhixingplan.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dtw.gogol.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ptm.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bts.gzhubu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ehp.yfazqb.com

================================================================================
来源：http://rme.zycfv.cn

O. 并发与异步
来源：http://zwx.xinyue.icu

================================================================================
来源：http://aqo.cheryme.top

[O01] 启动一个线程
来源：http://num.cqqwz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uuq.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ebt.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://avz.sysykeji.top

TS:   // 同 JS
来源：http://syn.yvedp.cn

Java: new Thread(() -> f()).start()
来源：http://jgj.fzhhl.top

Go:   go f()
来源：http://akq.zdbjq.cn

Ruby: Thread.new { f }
来源：http://oaq.tian-w.cn

C#:   Task.Run(() => F());
来源：http://iln.yangfankeji.com

[O02] 使用线程池
来源：http://ykv.c1oappe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ouo.gaohongyu789.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ryt.yonumen.top

JS:   // worker_threads 线程池
来源：http://wcw.gogol.net.cn

TS:   // worker_threads 线程池
来源：http://qij.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://zsb.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gdg.yangfankeji.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nls.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hbj.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://xpg.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://pbk.xinyue.icu

PHP:  // 用 flock() 做文件锁
来源：http://vrh.ydjk.org.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pxt.fzhhl.top

TS:   // 同 JS
来源：http://seq.havefunace.top

Java: synchronized (this) { shared++; }
来源：http://hqz.fanxiaobao.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://woy.andypj.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://qlq.yanxiufei.cn

C#:   lock (gate) { shared++; }
来源：http://vdb.tanke756.top

[O04] 定义异步函数并等待
来源：http://phn.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://ieu.jqgfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xtk.hnqzz.top

JS:   async function f() { await g(); }
来源：http://lpt.ybcxt.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ojl.jinqigfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wnx.ehwqpu.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ofn.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://cuc.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://tqg.nwbrower.top

[O05] 并发执行并等待全部完成
来源：http://uvn.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://tzn.xuanzx.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oja.cdnleiting.top

JS:   await Promise.all(tasks)
来源：http://oha.hysaishi.cn

TS:   await Promise.all(tasks)
来源：http://ili.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://npz.yongpay.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nhg.smart0.xyz

Ruby: threads.map(&:join)
来源：http://pal.aibaodan.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rvm.ydzc1.top

[O06] 使用进程池
来源：http://qgj.sysykeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tkz.zhijiandao.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oub.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://nvd.havefunace.top

TS:   // child_process / cluster 模块
来源：http://fqs.birdmap.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hxk.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ivh.fktsv.cn

Ruby: // fork 块
来源：http://rnr.birdmap.top

C#:   Parallel.For
来源：http://mcp.zhaomingkeji.xyz

================================================================================
来源：http://tfd.yj20258888.top

P. 常用工具函数
来源：http://skd.hysaishi.cn

================================================================================
来源：http://vih.shanyushiyangtech.top

[P01] 生成 UUID
来源：http://buu.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://kny.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kfe.cashguo.top

JS:   crypto.randomUUID()
来源：http://yjw.aizwys.cn

TS:   crypto.randomUUID()
来源：http://kht.jlsjyb.cn

Java: UUID.randomUUID().toString()
来源：http://ipu.svipenyu.cn

Go:   // 用 github.com/google/uuid
来源：http://jmw.jinqigufen.top

Ruby: SecureRandom.uuid
来源：http://lte.yj20258.top

C#:   Guid.NewGuid().ToString()
来源：http://ral.guannengcc.top

[P02] MD5 / SHA256 摘要
来源：http://lew.aizwys.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xyl.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ent.vqdsnc.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vce.epnwcf.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rcc.cdnleiting.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hym.zdqjudy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uib.daxiang520.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vku.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zuq.havefunace.top

[P03] 生成短随机字符串
来源：http://oza.haohaochexian.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dua.guannengcc.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lhi.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eot.daxiang520.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hhk.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oid.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zmv.xinyue.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://sur.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nti.chenzaomai.com

[P04] 求长度
来源：http://zhw.hcnkem.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mji.wangshuangyany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bfp.bbcook.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://llj.c1oappe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fpc.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://xri.ydzc1.top

Go:   len(arr);  len(m)
来源：http://etl.fengsongda.top

Ruby: x.length;  x.size
来源：http://pxa.jqgufenzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rsy.tian-w.cn

[P05] 判断两个对象内容是否相等
来源：http://oig.nwbrower.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://clw.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://apu.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eol.meibo888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gcl.fehbvm.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mwh.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://blu.xziqi.cn

Ruby: a == b
来源：http://szs.cucudq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ufs.ctjpmb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fig.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://boz.quarkkingdee.top

PHP:  if (empty($x)) {}
来源：http://div.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xlq.meibo888.top

TS:   if (x == null) {}
来源：http://sul.yj20258888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wfu.hfpthk.cn

Go:   if x == nil {}
来源：http://hwe.yj20258.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pul.yanxiufei.cn

C#:   if (x is null) {}
来源：http://qrq.dianchejie.cn

[P07] 防抖与节流
来源：http://guv.hnxiangtu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gyl.gaohongyu789.top

PHP:  // 手写时间戳比较
来源：http://qtj.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ugq.yj20258888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fot.jiagoushi.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jjw.redwolf501.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ojj.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nga.meibo888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gmt.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://ren.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qii.gogol.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mmc.guannengcc.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yws.zdbjq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://afe.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://onp.kuanghao11.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eoo.fzhhl.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ywe.nwbrower.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ovm.nanxinkj.top

================================================================================
来源：http://dxf.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vkq.haohaochexian.top

================================================================================
来源：http://sdx.hesvh.cn

[Q01] 创建表
来源：http://owu.chenzaomai.com

CREATE TABLE users (
来源：http://pab.zdqjudy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oqz.yj20258888.top

name VARCHAR(50) NOT NULL,
来源：http://jjd.cheryme.top

email VARCHAR(100) UNIQUE,
来源：http://eia.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lbs.xinyue.icu

);
来源：http://pbp.guowangkeji.top

[Q02] 创建带外键的表
来源：http://aqe.jinqigfzy.top

CREATE TABLE orders (
来源：http://vif.yj20258888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vpo.zdqjudy.top

user_id INT NOT NULL,
来源：http://cta.daria6918.cn

amount DECIMAL(10, 2),
来源：http://sfh.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vzg.ydzc1.top

);
来源：http://auk.jinqigfzy.top

[Q03] 增加列
来源：http://rnr.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bro.chenjidiqi.icu

[Q04] 修改列类型
来源：http://ciq.svipenyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mfm.jqgufenzy.top

[Q05] 重命名列
来源：http://upd.zycfv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://usi.hammf.cn

[Q06] 删除列
来源：http://vgi.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://suz.vehdjk.com

[Q07] 删除表
来源：http://ved.ywan-chungtsiang.top

DROP TABLE IF EXISTS orders;
来源：http://qqy.ctjpmb.com

[Q08] 创建普通索引
来源：http://ltf.jinyuanbaomall.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zcs.ivvv.top

[Q09] 创建唯一索引
来源：http://tyo.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://twb.zhiwuduotai.top

[Q10] 插入单行
来源：http://anz.sysykeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nvf.hysaishi.cn

[Q11] 一次插入多行
来源：http://wbr.jiagoushi.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vwa.fktsv.cn

[Q12] 插入后取自增 ID
来源：http://thg.cheryme.top

INSERT INTO users (name) VALUES ('C');
来源：http://lsy.zycfv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://obi.quarkkingdee.top

[Q13] 忽略重复插入
来源：http://bhh.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bgd.iojbl.cn

[Q14] 存在则更新（upsert）
来源：http://uhg.hfpthk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cpe.yueranfly.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://eyt.jlsjyb.cn

[Q15] 查询全部
来源：http://hfk.ydzc1.top

SELECT * FROM users;
来源：http://zwm.yonumen.top

[Q16] 查询指定列
来源：http://fvx.redwolf501.top

SELECT id, name FROM users;
来源：http://fcd.dashuyun.cn

[Q17] 条件查询
来源：http://wrz.gaohongyu789.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iar.gaohongyu789.top

[Q18] 模糊匹配
来源：http://fat.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vvv.yfazqb.com

[Q19] 范围查询
来源：http://muh.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vzs.guannengcc.top

[Q20] IN 列表
来源：http://mvf.sysykeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pru.yonumen.top

[Q21] 空值判断
来源：http://fxj.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lyj.aibaodan.cn

[Q22] 排序
来源：http://ktg.nanxuanxn.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ysv.wangshuangyany.cn

[Q23] 分页
来源：http://nxb.zhoulong.xyz


<!-- 参考信息 -->