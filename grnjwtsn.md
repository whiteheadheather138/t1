代发 wailian999

[N01] 二分查找（有序数组）
来源：http://lzu.zhixingplan.top

Py:   bisect.bisect_left(arr, x)
来源：http://lrh.tianlin.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fsi.xylfe.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vrk.yueranfly.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xlg.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dpx.gogol.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://jgr.ctjpmb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://qap.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cap.chenlongwang.top

[N02] 排序（工程实践用内置实现）
来源：http://vei.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://xqi.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://scb.chenjidiqi.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://awy.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pio.dianchejie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://urh.hongshengwenyu.top

Go:   slices.Sort(arr)
来源：http://tsc.gzhubu.top

Ruby: arr.sort
来源：http://hmw.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hkq.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://fsy.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yep.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://mju.daxiang520.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://twd.hnqzz.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yit.jqgufenzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tmq.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jwu.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rlq.gaohongyu789.top

C#:   // 手写递归，或 Array.Sort
来源：http://mck.ctjpmb.com

[N04] 斐波那契数列
来源：http://feu.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oaj.meibo888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xwa.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wvx.shanyushiyangtech.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nvg.chenjidiqi.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hkc.fengsongda.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wut.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://auf.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nng.cdnleiting.top

[N05] 最大公约数
来源：http://ctc.sufxvd.cn

Py:   math.gcd(a, b)
来源：http://crt.sweek.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dfc.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ron.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ymw.cheryme.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ydf.tanke756.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vbf.nanxuanxn.top

Ruby: a.gcd(b)
来源：http://yzb.xinyue.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nuf.gotoacloud.top

[N06] 判断回文字符串
来源：http://egv.ydjk.org.cn

Py:   s == s[::-1]
来源：http://olq.ydzc1.top

PHP:  $s === strrev($s);
来源：http://cwc.jqgfzy.top

JS:   s === [...s].reverse().join("")
来源：http://bry.ywan-chungtsiang.top

TS:   s === [...s].reverse().join("")
来源：http://wsv.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hff.bbcook.cn

Go:   // 双指针从两端比较
来源：http://qdw.dianchejie.cn

Ruby: s == s.reverse
来源：http://xmg.hcnkem.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://mfh.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://gby.jqgufenzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://obh.pengpengdd.cyou

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bfu.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://air.c1oappe.top

TS:   // 手写 Map<string, number>
来源：http://qvs.zdbjq.cn

Java: // 手写 HashMap
来源：http://kon.zhiwuduotai.top

Go:   // 手写 map[int]int
来源：http://cor.ydzc1.top

Ruby: // 手写 Hash
来源：http://awu.yj20258.top

C#:   // 手写 Dictionary<int, int>
来源：http://jxj.zhaomingkeji.xyz

[N08] 生成全排列
来源：http://auw.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://ygw.wangdashe.top

PHP:  // 手写递归交换
来源：http://nte.hnxiangtu.top

JS:   // 手写回溯递归
来源：http://eas.jyoumei.cn

TS:   // 手写回溯递归
来源：http://dyc.hongshengwenyu.top

Java: // 手写回溯递归
来源：http://bao.ybcxt.top

Go:   // 手写回溯递归
来源：http://lys.cqqwz.cn

Ruby: arr.permutation.to_a
来源：http://tfv.hesvh.cn

C#:   // 手写回溯递归
来源：http://qmq.zhoulong.xyz

[N09] 栈与队列
来源：http://fou.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cds.xuanzx.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://flv.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dwy.meibo888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ztm.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qpm.shzxlz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yhc.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dlq.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dyz.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://zli.tian-w.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vlq.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rwm.iojbl.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ccy.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://htk.yuxming.cn

Java: class Node { int v; Node next; }
来源：http://ojf.jinghuilouyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cbr.aizwys.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uzh.bjfxy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tdz.yfazqb.com

[N11] 二叉树中序遍历
来源：http://qoz.yj202588.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gwv.shanyushiyangtech.top

PHP:  // 手写递归函数
来源：http://xug.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bux.wangshuangyany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://icc.dashuyun.cn

Java: // 手写递归
来源：http://snr.ybcxt.top

Go:   // 手写递归
来源：http://hta.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hug.cashguo.top

C#:   // 手写递归
来源：http://vhy.dianchejie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sas.sxryk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oix.hywenlv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gmk.cucudq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oyv.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wpc.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yum.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tza.haohaochexian.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blw.ywan-chungtsiang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dby.cheryme.top

================================================================================
来源：http://lcv.xuetiantiany.cn

O. 并发与异步
来源：http://znn.hnqzz.top

================================================================================
来源：http://fbw.dashuyun.cn

[O01] 启动一个线程
来源：http://ook.shanyushiyangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mgc.ybcxt.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nkx.ywan-chungtsiang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uky.guowangkeji.top

TS:   // 同 JS
来源：http://yia.hnqzz.top

Java: new Thread(() -> f()).start()
来源：http://zhz.chenjidiqi.icu

Go:   go f()
来源：http://qkf.hcnkem.com

Ruby: Thread.new { f }
来源：http://emg.nwbrower.top

C#:   Task.Run(() => F());
来源：http://akh.nwbrower.top

[O02] 使用线程池
来源：http://nlu.hfpthk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rgz.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://otp.kuanghao11.cn

JS:   // worker_threads 线程池
来源：http://vse.52xcode.cn

TS:   // worker_threads 线程池
来源：http://dnl.iojbl.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jkn.zdbjq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://edb.dianchejie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bov.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xbo.fzhhl.top

[O03] 加锁保护共享数据
来源：http://csh.shuidangran.top

Py:   with lock: shared += 1
来源：http://rft.iojbl.cn

PHP:  // 用 flock() 做文件锁
来源：http://wfe.zhongyouzk.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jey.c1oappe.top

TS:   // 同 JS
来源：http://fki.zdbjq.cn

Java: synchronized (this) { shared++; }
来源：http://klb.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sxn.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://coe.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://iso.52xcode.cn

[O04] 定义异步函数并等待
来源：http://brb.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://iqz.sxryk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yme.yanxiufei.cn

JS:   async function f() { await g(); }
来源：http://abb.bjfxy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xhj.yanxiufei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lqd.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hqn.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://ydu.shangyingyoupin.top

C#:   async Task F() { await G(); }
来源：http://ibf.tianlin.xyz

[O05] 并发执行并等待全部完成
来源：http://vrf.havefunace.top

Py:   asyncio.gather(*tasks)
来源：http://zew.zhijiandao.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://day.0kj1m.cn

JS:   await Promise.all(tasks)
来源：http://xkn.nwbrower.top

TS:   await Promise.all(tasks)
来源：http://dlo.chenlongwang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zcr.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aea.gaohongyu789.top

Ruby: threads.map(&:join)
来源：http://lom.fehbvm.com

C#:   await Task.WhenAll(t1, t2)
来源：http://lgg.chenjidiqi.icu

[O06] 使用进程池
来源：http://lpo.zhoulong.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://slo.gaohongyu789.top

PHP:  // pcntl_fork 或多进程队列
来源：http://epk.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://ixv.zdqjudy.top

TS:   // child_process / cluster 模块
来源：http://wau.gzhubu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lde.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ejr.jinghuilouyu.cn

Ruby: // fork 块
来源：http://cbu.yanxiufei.cn

C#:   Parallel.For
来源：http://zdt.hcnkem.com

================================================================================
来源：http://grb.pengpengdd.cyou

P. 常用工具函数
来源：http://cuk.sxryk.cn

================================================================================
来源：http://qze.jqgfzy.top

[P01] 生成 UUID
来源：http://qfb.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://jks.quarkkingdee.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cwy.ehwqpu.com

JS:   crypto.randomUUID()
来源：http://lnb.hesvh.cn

TS:   crypto.randomUUID()
来源：http://mzv.hnxiangtu.top

Java: UUID.randomUUID().toString()
来源：http://jyp.zdbjq.cn

Go:   // 用 github.com/google/uuid
来源：http://ici.snrcjt.cn

Ruby: SecureRandom.uuid
来源：http://ztd.xziqi.cn

C#:   Guid.NewGuid().ToString()
来源：http://ida.gzhubu.top

[P02] MD5 / SHA256 摘要
来源：http://qcy.birdmap.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ccj.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tif.jiagoushi.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tmm.iojbl.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cjo.gogol.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ahb.andypj.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://miq.jinyuanbaomall.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lyw.svipenyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uhk.tianlin.xyz

[P03] 生成短随机字符串
来源：http://jbp.zdqjudy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wmm.yfazqb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mvh.vqdsnc.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jvm.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jey.gzhubu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zcn.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iwk.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://xws.zdqjudy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ppx.jqgfzy.top

[P04] 求长度
来源：http://otd.nanxinkj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aol.zhijiandao.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kvj.vehdjk.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zfr.pengpengdd.cyou

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eml.vqdsnc.cn

Java: list.size();  map.size();  s.length()
来源：http://inq.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://drr.jinyuanbaomall.cn

Ruby: x.length;  x.size
来源：http://kds.zhongyouzk.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://crg.yuanzhike.top

[P05] 判断两个对象内容是否相等
来源：http://zsi.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zvz.daxiang520.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vdh.shangyingyoupin.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://znp.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xap.nanxinkj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://neo.chenzaomai.com

Go:   reflect.DeepEqual(a, b)
来源：http://oor.wangshuangyany.cn

Ruby: a == b
来源：http://bbw.zdbjq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hlc.pengpengdd.cyou

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bsh.tanke756.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jao.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://lij.tianlin.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://opk.cheryme.top

TS:   if (x == null) {}
来源：http://swb.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://srr.yanxiufei.cn

Go:   if x == nil {}
来源：http://lac.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eas.shanyushiyangtech.top

C#:   if (x is null) {}
来源：http://yeg.ehwqpu.com

[P07] 防抖与节流
来源：http://uev.vqdsnc.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vgy.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://jdg.birdmap.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cpk.zdqjudy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hwq.cdnleiting.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jce.c1oappe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://edy.fengsongda.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fbl.tarul.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ayr.chenzaomai.com

[P08] 处理浮点精度问题
来源：http://bme.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pgt.vqdsnc.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jax.shuidangran.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://evt.epnwcf.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zfh.uphjek.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aip.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://joy.kuanghao11.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ayq.yj20258.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uam.shanyushiyangkeji.top

================================================================================
来源：http://obo.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://joe.aizwys.cn

================================================================================
来源：http://dja.zdqjudy.top

[Q01] 创建表
来源：http://ayx.fzhhl.top

CREATE TABLE users (
来源：http://bng.ppjwa.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zts.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://huf.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://uhf.yueranfly.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wrz.xylfe.cn

);
来源：http://lrk.sufxvd.cn

[Q02] 创建带外键的表
来源：http://led.aibaodan.cn

CREATE TABLE orders (
来源：http://irq.zhongyouzk.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kdf.shuidangran.top

user_id INT NOT NULL,
来源：http://eeg.52xcode.cn

amount DECIMAL(10, 2),
来源：http://xci.wangshuangyany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://afk.tian-w.cn

);
来源：http://olw.epnwcf.com

[Q03] 增加列
来源：http://hwa.sxryk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://syn.cucudq.cn

[Q04] 修改列类型
来源：http://yzs.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jxu.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://saq.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://enn.pengpengdd.cyou

[Q06] 删除列
来源：http://rfl.dianchejie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cpv.fanxiaobao.xyz

[Q07] 删除表
来源：http://dtb.xuanzx.com

DROP TABLE IF EXISTS orders;
来源：http://hlk.yueranfly.top

[Q08] 创建普通索引
来源：http://gvb.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://oks.52xcode.cn

[Q09] 创建唯一索引
来源：http://orn.c1oappe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eyt.birdmap.top

[Q10] 插入单行
来源：http://djf.yueranfly.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kpn.cdnleiting.top

[Q11] 一次插入多行
来源：http://fvf.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lqq.chenjidiqi.icu

[Q12] 插入后取自增 ID
来源：http://gtg.bjfxy.top

INSERT INTO users (name) VALUES ('C');
来源：http://lat.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sgr.gotoacloud.top

[Q13] 忽略重复插入
来源：http://jjs.yvedp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ocz.sufxvd.cn

[Q14] 存在则更新（upsert）
来源：http://lvu.chenlongwang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hbp.hcnkem.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xcd.gaohongyu789.top

[Q15] 查询全部
来源：http://iuu.sweek.top

SELECT * FROM users;
来源：http://rer.cdnleiting.top

[Q16] 查询指定列
来源：http://gfd.ehwqpu.com

SELECT id, name FROM users;
来源：http://rxb.yangfankeji.com

[Q17] 条件查询
来源：http://hhn.havefunace.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nmw.ivvv.top

[Q18] 模糊匹配
来源：http://uxo.aizwys.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xow.hesvh.cn

[Q19] 范围查询
来源：http://gca.nwbrower.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mrn.xuanzx.com

[Q20] IN 列表
来源：http://rul.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cjq.gogol.net.cn

[Q21] 空值判断
来源：http://pql.zycfv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sqs.gzhubu.top

[Q22] 排序
来源：http://zxg.dashuyun.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ops.jinqigufen.top

[Q23] 分页
来源：http://jed.nwbrower.top


<!-- 参考信息 -->