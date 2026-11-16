代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kfb.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://xdd.hnqzz.top

Go:   sort.SearchInts(arr, x)
来源：http://iwv.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hli.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rxs.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://wyn.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://olh.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://exs.chenjidiqi.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://vex.shangyingyoupin.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pyr.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oms.xziqi.cn

Go:   slices.Sort(arr)
来源：http://ygd.havefunace.top

Ruby: arr.sort
来源：http://qxa.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rgc.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://mbm.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iwh.cashguo.top

PHP:  // 递归实现，或用 usort
来源：http://nuj.zhixingplan.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://byz.sweek.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nsi.feifeiyinyue.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://anu.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pbu.jinghuilouyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gmy.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://lte.yueranfly.top

[N04] 斐波那契数列
来源：http://qbp.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zmz.cdnleiting.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hbt.fktsv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rcf.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mhe.yj20258.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kcq.yj20258888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mwj.ywan-chungtsiang.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jbg.chenjidiqi.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ohn.gotoacloud.top

[N05] 最大公约数
来源：http://irb.zhaomingkeji.xyz

Py:   math.gcd(a, b)
来源：http://osr.jinqigufen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wff.chenzaomai.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ghr.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ilk.fengsongda.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://alm.chenlongwang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dvq.chenjidiqi.icu

Ruby: a.gcd(b)
来源：http://etc.cqqwz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://urx.ctjpmb.com

[N06] 判断回文字符串
来源：http://wzq.yueranfly.top

Py:   s == s[::-1]
来源：http://chp.xylfe.cn

PHP:  $s === strrev($s);
来源：http://lsg.svipenyu.cn

JS:   s === [...s].reverse().join("")
来源：http://bvn.jqgfzy.top

TS:   s === [...s].reverse().join("")
来源：http://pdq.xinyue.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qro.redwolf501.top

Go:   // 双指针从两端比较
来源：http://egs.havefunace.top

Ruby: s == s.reverse
来源：http://nhg.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://rsq.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://ixl.aibaodan.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kvb.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nuo.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rse.pengpengdd.cyou

TS:   // 手写 Map<string, number>
来源：http://bzq.yuanzhike.top

Java: // 手写 HashMap
来源：http://heo.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://tce.jqgfzy.top

Ruby: // 手写 Hash
来源：http://nra.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://xhi.chenzaomai.com

[N08] 生成全排列
来源：http://gxq.yuanzhike.top

Py:   itertools.permutations(arr)
来源：http://tif.aibaodan.cn

PHP:  // 手写递归交换
来源：http://haq.zhaomingkeji.xyz

JS:   // 手写回溯递归
来源：http://gsb.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://mqe.shuidangran.top

Java: // 手写回溯递归
来源：http://xgx.andypj.xyz

Go:   // 手写回溯递归
来源：http://fhy.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://bfw.tanke756.top

C#:   // 手写回溯递归
来源：http://nia.wangdashe.top

[N09] 栈与队列
来源：http://zyf.zhaomingkeji.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://btj.gzhubu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jey.chenlongwang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ttm.xuanzx.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sxb.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kmk.yuxming.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ctn.52xcode.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lko.zycfv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xit.cashguo.top

[N10] 链表节点定义
来源：http://utn.cucudq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tkv.ydjk.org.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kre.chenjidiqi.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ovz.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://glg.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://aar.hongshengwenyu.top

Go:   type Node struct { V int; Next *Node }
来源：http://wsy.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://idl.ivvv.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rmi.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://ngi.aibaodan.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xss.jyoumei.cn

PHP:  // 手写递归函数
来源：http://xuh.ctjpmb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lad.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fdb.iojbl.cn

Java: // 手写递归
来源：http://yxb.316326.xyz

Go:   // 手写递归
来源：http://dop.tanke756.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qoh.sxryk.cn

C#:   // 手写递归
来源：http://hjd.xziqi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rov.meibo888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hye.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://enm.feifeiyinyue.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tre.nwbrower.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fmn.xingfuxueyuan.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nwj.hysaishi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ljs.fengsongda.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xrw.yj20258.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://krk.tianlin.xyz

================================================================================
来源：http://zam.yuanzhike.top

O. 并发与异步
来源：http://vvk.vqdsnc.cn

================================================================================
来源：http://ioo.svipenyu.cn

[O01] 启动一个线程
来源：http://ivi.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qzt.aibaodan.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vkn.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zgb.yvedp.cn

TS:   // 同 JS
来源：http://vcq.quarkkingdee.top

Java: new Thread(() -> f()).start()
来源：http://npy.chenjidiqi.icu

Go:   go f()
来源：http://bjv.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://zwl.yuxming.cn

C#:   Task.Run(() => F());
来源：http://yzd.316326.xyz

[O02] 使用线程池
来源：http://mmw.ydzc1.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nnq.nanxinkj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xty.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://dpt.gzhubu.top

TS:   // worker_threads 线程池
来源：http://vvt.cdnleiting.top

Java: Executors.newFixedThreadPool(4)
来源：http://ybx.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qcx.tianlin.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lin.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nwy.ehwqpu.com

[O03] 加锁保护共享数据
来源：http://nwk.sysykeji.top

Py:   with lock: shared += 1
来源：http://wny.chenzaomai.com

PHP:  // 用 flock() 做文件锁
来源：http://nsp.chenjidiqi.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uyj.nanxuanxn.top

TS:   // 同 JS
来源：http://vsc.ydzc1.top

Java: synchronized (this) { shared++; }
来源：http://xxo.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rnx.mhx1999.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fsz.316326.xyz

C#:   lock (gate) { shared++; }
来源：http://vxn.jlsjyb.cn

[O04] 定义异步函数并等待
来源：http://nuu.yongpay.top

Py:   async def f():⏎    await g()
来源：http://tlr.hysaishi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kki.guannengcc.top

JS:   async function f() { await g(); }
来源：http://bue.xylfe.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dfm.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://syv.fktsv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://skb.hongshengwenyu.top

Ruby: # 用 Fiber 或 async gem
来源：http://pag.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://chh.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://cuz.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://fms.jinqigfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yov.sysykeji.top

JS:   await Promise.all(tasks)
来源：http://xco.uphjek.com

TS:   await Promise.all(tasks)
来源：http://csy.fanxiaobao.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tvm.bjfxy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ewt.andypj.xyz

Ruby: threads.map(&:join)
来源：http://xnh.shuidangran.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dyg.jinqigufen.top

[O06] 使用进程池
来源：http://czt.fktsv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lhb.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://gni.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://baq.hfpthk.cn

TS:   // child_process / cluster 模块
来源：http://vxq.fktsv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dtg.mhx1999.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wju.vehdjk.com

Ruby: // fork 块
来源：http://hgz.cashguo.top

C#:   Parallel.For
来源：http://qlp.sysykeji.top

================================================================================
来源：http://vsd.nanxinkj.top

P. 常用工具函数
来源：http://unl.shanyushiyangkeji.top

================================================================================
来源：http://daj.52xcode.cn

[P01] 生成 UUID
来源：http://llp.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://dpm.fzhhl.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://btk.snrcjt.cn

JS:   crypto.randomUUID()
来源：http://nfx.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://wqk.fehbvm.com

Java: UUID.randomUUID().toString()
来源：http://xog.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://nmn.316326.xyz

Ruby: SecureRandom.uuid
来源：http://ebx.yj20258888.top

C#:   Guid.NewGuid().ToString()
来源：http://abj.0kj1m.cn

[P02] MD5 / SHA256 摘要
来源：http://kzu.shangyingyoupin.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://spt.gogol.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://aks.gotoacloud.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rng.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://etx.fehbvm.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hcx.feifeiyinyue.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vbx.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jfr.zhoulong.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gqt.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://xxu.kuanghao11.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wxt.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sgf.hnqzz.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ywb.yfazqb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iqo.gzhubu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zps.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://upz.hongshengwenyu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sfy.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sze.hcnkem.com

[P04] 求长度
来源：http://ong.iojbl.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fez.gzhubu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ohx.yanxiufei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://enb.jqgufenzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dmj.hywenlv.cn

Java: list.size();  map.size();  s.length()
来源：http://jqo.xylfe.cn

Go:   len(arr);  len(m)
来源：http://ryk.zhoulong.xyz

Ruby: x.length;  x.size
来源：http://xaf.guannengcc.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wpq.hesvh.cn

[P05] 判断两个对象内容是否相等
来源：http://iwo.hnqzz.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hwk.iojbl.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tsa.havefunace.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qtg.xinyue.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lmm.jiagoushi.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://doz.wangshuangyany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vro.jyoumei.cn

Ruby: a == b
来源：http://htm.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://akz.mhx1999.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xdo.andypj.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fkv.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://cfo.xingfuxueyuan.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://crw.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://ffr.cashguo.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zxi.c1oappe.top

Go:   if x == nil {}
来源：http://ysr.birdmap.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wjj.hywenlv.cn

C#:   if (x is null) {}
来源：http://frn.yonumen.top

[P07] 防抖与节流
来源：http://fvp.zycfv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fby.jiagoushi.top

PHP:  // 手写时间戳比较
来源：http://yeu.daria6918.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jdz.yanxiufei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lvo.zycfv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xbl.bjfxy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dem.mhx1999.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bgk.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://din.yvedp.cn

[P08] 处理浮点精度问题
来源：http://kzz.xuanzx.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xab.birdmap.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hfn.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://buz.ivvv.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kng.mhx1999.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yya.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fml.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kuu.jinqigfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gmp.svipenyu.cn

================================================================================
来源：http://scs.pengpengdd.cyou

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wey.fehbvm.com

================================================================================
来源：http://hse.andypj.xyz

[Q01] 创建表
来源：http://dhl.guannengcc.top

CREATE TABLE users (
来源：http://evs.jyoumei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tgd.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://rwq.fanxiaobao.xyz

email VARCHAR(100) UNIQUE,
来源：http://fld.chenjidiqi.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ipd.bjfxy.top

);
来源：http://oms.cucudq.cn

[Q02] 创建带外键的表
来源：http://bkp.ppjwa.cn

CREATE TABLE orders (
来源：http://cts.gogol.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yok.fengsongda.top

user_id INT NOT NULL,
来源：http://osr.hnqzz.top

amount DECIMAL(10, 2),
来源：http://zlj.yuanzhike.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://knx.jqgufenzy.top

);
来源：http://oti.jiagoushi.top

[Q03] 增加列
来源：http://twg.cdnleiting.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tfr.guannengcc.top

[Q04] 修改列类型
来源：http://nyk.shzxlz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://amp.zhixingplan.top

[Q05] 重命名列
来源：http://ako.pycfn.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://igr.hfpthk.cn

[Q06] 删除列
来源：http://hpv.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://fdk.zhongyouzk.top

[Q07] 删除表
来源：http://soe.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://wog.quarkkingdee.top

[Q08] 创建普通索引
来源：http://mrz.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ncn.jinghuilouyu.cn

[Q09] 创建唯一索引
来源：http://lgy.xylfe.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jez.ybcxt.top

[Q10] 插入单行
来源：http://juw.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yaq.feifeiyinyue.top

[Q11] 一次插入多行
来源：http://gxb.9152youxi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lzk.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://syy.yanxiufei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xuv.ppjwa.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wzb.sysykeji.top

[Q13] 忽略重复插入
来源：http://lki.yj202588.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ueb.jyoumei.cn

[Q14] 存在则更新（upsert）
来源：http://coi.dashuyun.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://faa.fanxiaobao.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ceo.uphjek.com

[Q15] 查询全部
来源：http://lkg.sxryk.cn

SELECT * FROM users;
来源：http://ttr.316326.xyz

[Q16] 查询指定列
来源：http://xxl.tianlin.xyz

SELECT id, name FROM users;
来源：http://sqg.hongshengwenyu.top

[Q17] 条件查询
来源：http://hqm.yj20258.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zsg.kuanghao11.cn

[Q18] 模糊匹配
来源：http://mjf.vehdjk.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ugy.epnwcf.com

[Q19] 范围查询
来源：http://rlm.hnxiangtu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://paa.fzhhl.top

[Q20] IN 列表
来源：http://cza.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hst.316326.xyz

[Q21] 空值判断
来源：http://ksj.9152youxi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dub.quarkkingdee.top

[Q22] 排序
来源：http://mji.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://djv.dianchejie.cn

[Q23] 分页
来源：http://qfd.ppjwa.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pzt.hnqzz.top

[Q24] 去重
来源：http://emk.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://pwr.aizwys.cn

[Q25] 只取前 N 条
来源：http://ohp.cqqwz.cn


<!-- 参考信息 -->