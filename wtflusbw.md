代发 wailian999

[M08] 获取系统与运行时信息
来源：http://lia.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://iia.tanke756.top

PHP:  PHP_OS;  phpversion();
来源：http://txf.fehbvm.com

JS:   process.platform;  process.version
来源：http://mdx.fengsongda.top

TS:   process.platform;  process.version
来源：http://ust.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ker.haohaochexian.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gao.dashuyun.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://anl.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uca.tarul.cn

================================================================================
来源：http://grs.hysaishi.cn

N. 数据结构与算法
来源：http://ppk.ivvv.top

================================================================================
来源：http://ofp.cucudq.cn

[N01] 二分查找（有序数组）
来源：http://zqr.dianchejie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fdi.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aki.nanxinkj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xom.jqgfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ooy.gzhubu.top

Java: Arrays.binarySearch(arr, x)
来源：http://hkx.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://tfr.xingfuxueyuan.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://gpo.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://kvn.chenzaomai.com

[N02] 排序（工程实践用内置实现）
来源：http://gdu.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://jfn.fengsongda.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://khj.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xpw.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://vkm.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gps.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://szh.xziqi.cn

Ruby: arr.sort
来源：http://xsd.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dln.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://ogn.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wre.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://hbe.tanke756.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nsl.yonumen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zgi.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dxy.aizwys.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pov.jlsjyb.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qww.hysaishi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vaj.pengpengdd.cyou

[N04] 斐波那契数列
来源：http://xhz.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cff.kuanghao11.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cng.0kj1m.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xyz.tianlin.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aao.9152youxi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jmd.tianlin.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ewc.xylfe.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fqj.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://can.jinghuilouyu.cn

[N05] 最大公约数
来源：http://gdl.guowangkeji.top

Py:   math.gcd(a, b)
来源：http://jpz.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kta.hfpthk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pkq.gaohongyu789.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bbk.ehwqpu.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jbg.zycfv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rkq.yvedp.cn

Ruby: a.gcd(b)
来源：http://ekg.yj20258.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bsp.epnwcf.com

[N06] 判断回文字符串
来源：http://pfm.sjlbkw.cn

Py:   s == s[::-1]
来源：http://ldb.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://rui.ybcxt.top

JS:   s === [...s].reverse().join("")
来源：http://cwx.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://qss.chenlongwang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dsr.iojbl.cn

Go:   // 双指针从两端比较
来源：http://hdd.zhixingplan.top

Ruby: s == s.reverse
来源：http://osa.yj20258.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nst.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://tnq.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://btc.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fdv.yj20258.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ljp.yueranfly.top

TS:   // 手写 Map<string, number>
来源：http://zvr.sxryk.cn

Java: // 手写 HashMap
来源：http://cyn.guowangkeji.top

Go:   // 手写 map[int]int
来源：http://cbf.sweek.top

Ruby: // 手写 Hash
来源：http://vlj.guannengcc.top

C#:   // 手写 Dictionary<int, int>
来源：http://kpt.chenlongwang.top

[N08] 生成全排列
来源：http://iku.chenlongwang.top

Py:   itertools.permutations(arr)
来源：http://oct.sufxvd.cn

PHP:  // 手写递归交换
来源：http://wvh.redwolf501.top

JS:   // 手写回溯递归
来源：http://fhh.fzhhl.top

TS:   // 手写回溯递归
来源：http://zkr.zhoulong.xyz

Java: // 手写回溯递归
来源：http://bbs.316326.xyz

Go:   // 手写回溯递归
来源：http://omj.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://pui.52xcode.cn

C#:   // 手写回溯递归
来源：http://qrg.zhongyouzk.top

[N09] 栈与队列
来源：http://ybn.hongshengwenyu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oin.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pys.316326.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ghx.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cjl.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jqq.cheryme.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ozs.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wgw.yj20258888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vgu.wangshuangyany.cn

[N10] 链表节点定义
来源：http://sgx.nwbrower.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jae.ehwqpu.com

PHP:  class Node { public $v; public $next = null; }
来源：http://eah.tanke756.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://idw.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yas.havefunace.top

Java: class Node { int v; Node next; }
来源：http://hbv.chenjidiqi.icu

Go:   type Node struct { V int; Next *Node }
来源：http://gip.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://eep.quarkkingdee.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zdg.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://ple.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zsd.zycfv.cn

PHP:  // 手写递归函数
来源：http://nsi.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oah.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wzw.cqqwz.cn

Java: // 手写递归
来源：http://svq.daxiang520.top

Go:   // 手写递归
来源：http://ltf.cucudq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fxy.jyoumei.cn

C#:   // 手写递归
来源：http://cbe.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://izm.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qhu.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mai.uphjek.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mub.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vjo.jinqigufen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zyb.guannengcc.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://geu.hcnkem.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rjn.birdmap.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ffr.mhx1999.top

================================================================================
来源：http://npz.birdmap.top

O. 并发与异步
来源：http://qng.gogol.net.cn

================================================================================
来源：http://ler.c1oappe.top

[O01] 启动一个线程
来源：http://rff.mhx1999.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://otl.hnxiangtu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zlm.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oer.vehdjk.com

TS:   // 同 JS
来源：http://obm.xuanzx.com

Java: new Thread(() -> f()).start()
来源：http://ihu.tarul.cn

Go:   go f()
来源：http://alj.nwbrower.top

Ruby: Thread.new { f }
来源：http://xip.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://vgm.smart0.xyz

[O02] 使用线程池
来源：http://agv.yonumen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gyn.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jgf.uphjek.com

JS:   // worker_threads 线程池
来源：http://wif.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://ojr.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://bub.guannengcc.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mzs.yonumen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lvt.xingfuxueyuan.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cmt.shangyingyoupin.top

[O03] 加锁保护共享数据
来源：http://geq.hfpthk.cn

Py:   with lock: shared += 1
来源：http://mzf.chenzaomai.com

PHP:  // 用 flock() 做文件锁
来源：http://bgt.cdnleiting.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fjz.xinyue.icu

TS:   // 同 JS
来源：http://qam.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://ebd.vqdsnc.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yjp.ctjpmb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ndl.shanyushiyangkeji.top

C#:   lock (gate) { shared++; }
来源：http://gvr.hnqzz.top

[O04] 定义异步函数并等待
来源：http://qts.yangfankeji.com

Py:   async def f():⏎    await g()
来源：http://gys.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hmm.chenjidiqi.icu

JS:   async function f() { await g(); }
来源：http://jfi.havefunace.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ugr.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ljd.dianchejie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://glq.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://gom.tanke756.top

C#:   async Task F() { await G(); }
来源：http://ojk.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://shd.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://xxd.zhengqikj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cxy.shzxlz.cn

JS:   await Promise.all(tasks)
来源：http://apy.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://jix.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mrm.birdmap.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aqv.yj20258.top

Ruby: threads.map(&:join)
来源：http://hfk.sufxvd.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dhc.xingfuxueyuan.xyz

[O06] 使用进程池
来源：http://qox.jiagoushi.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zwn.yuxming.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gyh.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://nfs.tarul.cn

TS:   // child_process / cluster 模块
来源：http://wyp.aizwys.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qxd.yj20258888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gpt.haohaochexian.top

Ruby: // fork 块
来源：http://aty.shangyingyoupin.top

C#:   Parallel.For
来源：http://xmy.mhx1999.top

================================================================================
来源：http://jqv.c1oappe.top

P. 常用工具函数
来源：http://vkr.yangfankeji.com

================================================================================
来源：http://wkp.xziqi.cn

[P01] 生成 UUID
来源：http://emn.snrcjt.cn

Py:   str(uuid.uuid4())
来源：http://rjv.tianlin.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uas.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://roj.xuetiantiany.cn

TS:   crypto.randomUUID()
来源：http://fng.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://ptw.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://omq.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://ckh.hnxiangtu.top

C#:   Guid.NewGuid().ToString()
来源：http://imc.ctjpmb.com

[P02] MD5 / SHA256 摘要
来源：http://jhu.quarkkingdee.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ege.hfpthk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ddi.xziqi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bor.yuanzhike.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uld.ydjk.org.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ryj.jinghuilouyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lty.mhx1999.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://soy.bbcook.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://asv.guannengcc.top

[P03] 生成短随机字符串
来源：http://wma.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tjd.tian-w.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://osh.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lbe.jinqigfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ewn.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jhg.nanxinkj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blc.zhixingplan.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://skl.yuanzhike.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kov.tarul.cn

[P04] 求长度
来源：http://wbl.wangshuangyany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dsf.vqdsnc.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zho.fengsongda.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://otp.yj20258.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xwd.gzhubu.top

Java: list.size();  map.size();  s.length()
来源：http://aag.quarkkingdee.top

Go:   len(arr);  len(m)
来源：http://ieo.ywan-chungtsiang.top

Ruby: x.length;  x.size
来源：http://wyo.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://iip.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://isd.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rqy.fktsv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ett.svipenyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xif.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cdb.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lho.sjlbkw.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lxo.yj20258.top

Ruby: a == b
来源：http://klb.hywenlv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xye.chenzaomai.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lld.tanke756.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rqz.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://tfo.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eji.gogol.net.cn

TS:   if (x == null) {}
来源：http://ptc.cashguo.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ved.zhengqikj.top

Go:   if x == nil {}
来源：http://wrd.fzhhl.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qqe.yanxiufei.cn

C#:   if (x is null) {}
来源：http://dzk.dashuyun.cn

[P07] 防抖与节流
来源：http://abf.xingfuxueyuan.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dab.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://rxn.cucudq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kwi.wangdashe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ygp.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cep.iojbl.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://klm.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hbg.hnxiangtu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uoz.zhaomingkeji.xyz

[P08] 处理浮点精度问题
来源：http://ehu.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gqv.nwbrower.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qqa.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jjs.redwolf501.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jtg.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oft.jinghuilouyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bun.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pqz.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tlv.jinqigufen.top

================================================================================
来源：http://nbw.tian-w.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oww.hnqzz.top

================================================================================
来源：http://ois.zhengqikj.top

[Q01] 创建表
来源：http://nqk.fehbvm.com

CREATE TABLE users (
来源：http://qun.epnwcf.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sra.yfazqb.com

name VARCHAR(50) NOT NULL,
来源：http://yna.hysaishi.cn

email VARCHAR(100) UNIQUE,
来源：http://jug.yj202588.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lov.hongshengwenyu.top

);
来源：http://psy.nanxuanxn.top

[Q02] 创建带外键的表
来源：http://ylb.shzxlz.cn

CREATE TABLE orders (
来源：http://xtt.sysykeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://clf.uphjek.com

user_id INT NOT NULL,
来源：http://rqn.cashguo.top

amount DECIMAL(10, 2),
来源：http://amm.guowangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sof.yonumen.top

);
来源：http://llo.pycfn.com

[Q03] 增加列
来源：http://qch.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sgz.316326.xyz

[Q04] 修改列类型
来源：http://izq.yonumen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qvo.guowangkeji.top

[Q05] 重命名列
来源：http://hpb.zhaomingkeji.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cqj.xuanzx.com

[Q06] 删除列
来源：http://qlo.guannengcc.top

ALTER TABLE users DROP COLUMN age;
来源：http://giq.jyoumei.cn

[Q07] 删除表
来源：http://nop.sysykeji.top

DROP TABLE IF EXISTS orders;
来源：http://vvg.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://oov.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fhn.jlsjyb.cn

[Q09] 创建唯一索引
来源：http://zlq.mhx1999.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xzh.redwolf501.top

[Q10] 插入单行
来源：http://sop.aibaodan.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vin.ivvv.top

[Q11] 一次插入多行
来源：http://zpz.52xcode.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gib.c1oappe.top

[Q12] 插入后取自增 ID
来源：http://xom.chenlongwang.top

INSERT INTO users (name) VALUES ('C');
来源：http://azj.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ejw.yj202588.top

[Q13] 忽略重复插入
来源：http://pht.jinghuilouyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://igy.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://rjb.sxryk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tnm.ctjpmb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zwt.ctjpmb.com

[Q15] 查询全部
来源：http://cau.nwbrower.top

SELECT * FROM users;
来源：http://sru.zhijiandao.cn

[Q16] 查询指定列
来源：http://rka.hnqzz.top

SELECT id, name FROM users;
来源：http://ebb.xziqi.cn

[Q17] 条件查询
来源：http://dfm.hammf.cn


<!-- 参考信息 -->