代发 wailian999

TS:   process.platform;  process.version
来源：http://pop.ywan-chungtsiang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zhl.yonumen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kmi.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jhk.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://izq.zhiwuduotai.top

================================================================================
来源：http://etx.cucudq.cn

N. 数据结构与算法
来源：http://qss.sysykeji.top

================================================================================
来源：http://zfq.fktsv.cn

[N01] 二分查找（有序数组）
来源：http://wnh.ivvv.top

Py:   bisect.bisect_left(arr, x)
来源：http://gqa.0kj1m.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://chk.gaohongyu789.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gus.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wbt.tian-w.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ybm.jinghuilouyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://gmf.52xcode.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qis.daria6918.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kcg.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://dnn.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://rid.pengpengdd.cyou

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qpv.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://qhi.yvedp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ang.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lbp.hammf.cn

Go:   slices.Sort(arr)
来源：http://pih.sjlbkw.cn

Ruby: arr.sort
来源：http://awx.cqqwz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lgz.9152youxi.cn

[N03] 快速排序（分治示例）
来源：http://hns.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qzx.ivvv.top

PHP:  // 递归实现，或用 usort
来源：http://whi.hongshengwenyu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aav.birdmap.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aub.zhengqikj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zsl.cqqwz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tfm.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rvd.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://bys.yangfankeji.com

[N04] 斐波那契数列
来源：http://bpb.hammf.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pvb.sysykeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://psk.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dbl.iojbl.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rmp.chenzaomai.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://znu.hnqzz.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mpo.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qhz.birdmap.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pct.vqdsnc.cn

[N05] 最大公约数
来源：http://ego.fktsv.cn

Py:   math.gcd(a, b)
来源：http://cyw.meibo888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lzu.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sbe.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ucn.yonumen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qwu.svipenyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zmc.iojbl.cn

Ruby: a.gcd(b)
来源：http://pzv.ydzc1.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://txw.yanxiufei.cn

[N06] 判断回文字符串
来源：http://ivy.jiagoushi.top

Py:   s == s[::-1]
来源：http://xxf.tianlin.xyz

PHP:  $s === strrev($s);
来源：http://cyv.jyoumei.cn

JS:   s === [...s].reverse().join("")
来源：http://ptw.gogol.net.cn

TS:   s === [...s].reverse().join("")
来源：http://sgb.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://soi.epnwcf.com

Go:   // 双指针从两端比较
来源：http://ded.dashuyun.cn

Ruby: s == s.reverse
来源：http://wuf.gogol.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ivf.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://yts.ydzc1.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rvh.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fgi.tanke756.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ove.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://dui.zdqjudy.top

Java: // 手写 HashMap
来源：http://ols.zhoulong.xyz

Go:   // 手写 map[int]int
来源：http://udh.iojbl.cn

Ruby: // 手写 Hash
来源：http://ign.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://ipm.guannengcc.top

[N08] 生成全排列
来源：http://ccc.sjlbkw.cn

Py:   itertools.permutations(arr)
来源：http://mmt.ywan-chungtsiang.top

PHP:  // 手写递归交换
来源：http://kil.aibaodan.cn

JS:   // 手写回溯递归
来源：http://ybz.yvedp.cn

TS:   // 手写回溯递归
来源：http://zvj.yongpay.top

Java: // 手写回溯递归
来源：http://jng.xingfuxueyuan.xyz

Go:   // 手写回溯递归
来源：http://cwq.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://wqq.sweek.top

C#:   // 手写回溯递归
来源：http://wwt.yfazqb.com

[N09] 栈与队列
来源：http://ygc.jianghu66.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mgg.ehwqpu.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ttu.zhaomingkeji.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yxg.shangyingyoupin.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kvv.guannengcc.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aih.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hvt.hammf.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dzj.fanxiaobao.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://srr.yj202588.top

[N10] 链表节点定义
来源：http://qxk.yj20258888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tlm.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://znk.zhaomingkeji.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rmu.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://upn.sweek.top

Java: class Node { int v; Node next; }
来源：http://xca.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bwj.zdqjudy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pzr.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ned.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://xdo.svipenyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gjj.hywenlv.cn

PHP:  // 手写递归函数
来源：http://hfx.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uya.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iji.sjlbkw.cn

Java: // 手写递归
来源：http://ikf.gotoacloud.top

Go:   // 手写递归
来源：http://hhk.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://suo.zhaomingkeji.xyz

C#:   // 手写递归
来源：http://dre.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qtm.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wru.vqdsnc.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cam.dianchejie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lov.svipenyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lvx.hfpthk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://evc.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jrb.0kj1m.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pys.cashguo.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jsz.jlsjyb.cn

================================================================================
来源：http://xmq.gzhubu.top

O. 并发与异步
来源：http://vzl.fktsv.cn

================================================================================
来源：http://npp.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://abb.pengpengdd.cyou

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qfr.52xcode.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gro.sjlbkw.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zih.fktsv.cn

TS:   // 同 JS
来源：http://xfn.yangfankeji.com

Java: new Thread(() -> f()).start()
来源：http://paz.cqqwz.cn

Go:   go f()
来源：http://rzx.epnwcf.com

Ruby: Thread.new { f }
来源：http://hay.hcnkem.com

C#:   Task.Run(() => F());
来源：http://qbc.shanyushiyangkeji.top

[O02] 使用线程池
来源：http://huu.cucudq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://enr.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://win.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://ayn.tian-w.cn

TS:   // worker_threads 线程池
来源：http://ipo.andypj.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://ixc.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aam.gogol.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://top.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xhr.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://pha.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://uvi.jinqigfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://rjn.cucudq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rjq.yuanzhike.top

TS:   // 同 JS
来源：http://are.zdqjudy.top

Java: synchronized (this) { shared++; }
来源：http://zru.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wim.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zwc.xuanzx.com

C#:   lock (gate) { shared++; }
来源：http://syx.fengsongda.top

[O04] 定义异步函数并等待
来源：http://egp.sjlbkw.cn

Py:   async def f():⏎    await g()
来源：http://fsg.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sel.ydjk.org.cn

JS:   async function f() { await g(); }
来源：http://tdb.zhongyouzk.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jxb.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jri.zhijiandao.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lue.zycfv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gni.kuanghao11.cn

C#:   async Task F() { await G(); }
来源：http://wuj.cqqwz.cn

[O05] 并发执行并等待全部完成
来源：http://jzu.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://rri.sjlbkw.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ifu.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://bhp.tanke756.top

TS:   await Promise.all(tasks)
来源：http://jdm.gotoacloud.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ydq.wangdashe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pqe.pycfn.com

Ruby: threads.map(&:join)
来源：http://wck.jinghuilouyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zzs.zhongyouzk.top

[O06] 使用进程池
来源：http://hpz.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hie.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://egf.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://svw.xingfuxueyuan.xyz

TS:   // child_process / cluster 模块
来源：http://itw.vehdjk.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hsh.316326.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://onq.zhengqikj.top

Ruby: // fork 块
来源：http://pqp.gotoacloud.top

C#:   Parallel.For
来源：http://cpy.jyoumei.cn

================================================================================
来源：http://lna.jqgufenzy.top

P. 常用工具函数
来源：http://trj.sxryk.cn

================================================================================
来源：http://crt.c1oappe.top

[P01] 生成 UUID
来源：http://rdf.feifeiyinyue.top

Py:   str(uuid.uuid4())
来源：http://eph.daria6918.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gai.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://kti.yueranfly.top

TS:   crypto.randomUUID()
来源：http://mks.hywenlv.cn

Java: UUID.randomUUID().toString()
来源：http://brn.ywan-chungtsiang.top

Go:   // 用 github.com/google/uuid
来源：http://axa.nanxuanxn.top

Ruby: SecureRandom.uuid
来源：http://vum.xingfuxueyuan.xyz

C#:   Guid.NewGuid().ToString()
来源：http://nrc.xingfuxueyuan.xyz

[P02] MD5 / SHA256 摘要
来源：http://rpj.shanyushiyangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uly.shangyingyoupin.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fac.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://czk.vehdjk.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mrz.hywenlv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gib.yuxming.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mwq.hysaishi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gnh.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rfy.hysaishi.cn

[P03] 生成短随机字符串
来源：http://dxv.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pou.cucudq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xud.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xox.jyoumei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lyw.zdqjudy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rtc.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xpa.xinyue.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://pzs.zhaomingkeji.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://avm.feifeiyinyue.top

[P04] 求长度
来源：http://epr.jinghuilouyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fde.yueranfly.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jiu.tarul.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aph.tian-w.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zfr.jqgfzy.top

Java: list.size();  map.size();  s.length()
来源：http://kjk.zhoulong.xyz

Go:   len(arr);  len(m)
来源：http://ziw.sweek.top

Ruby: x.length;  x.size
来源：http://xda.hywenlv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://krz.yfazqb.com

[P05] 判断两个对象内容是否相等
来源：http://szb.quarkkingdee.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pca.hfpthk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iks.shuidangran.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cxj.xuanzx.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fpf.zdqjudy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ohj.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gbp.jiagoushi.top

Ruby: a == b
来源：http://jpb.chenzaomai.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wat.bbcook.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gxi.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ruy.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://pkm.ydjk.org.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eja.chenlongwang.top

TS:   if (x == null) {}
来源：http://jik.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kds.sjlbkw.cn

Go:   if x == nil {}
来源：http://gpl.vehdjk.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dpu.epnwcf.com

C#:   if (x is null) {}
来源：http://zuj.tarul.cn

[P07] 防抖与节流
来源：http://atw.zycfv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gfp.feifeiyinyue.top

PHP:  // 手写时间戳比较
来源：http://anv.tanke756.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wgh.smart0.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pun.zhoulong.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pry.zdqjudy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fqy.sweek.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://scr.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ypj.jyoumei.cn

[P08] 处理浮点精度问题
来源：http://xdj.shuidangran.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fvi.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uuz.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cjz.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tat.wangdashe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://htv.gotoacloud.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://thh.yuanzhike.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kdy.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bjx.xziqi.cn

================================================================================
来源：http://gyb.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cwp.uphjek.com

================================================================================
来源：http://zqi.316326.xyz

[Q01] 创建表
来源：http://lgr.ywan-chungtsiang.top

CREATE TABLE users (
来源：http://gfi.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://efw.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://ysw.cdnleiting.top

email VARCHAR(100) UNIQUE,
来源：http://rit.hesvh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cyi.haohaochexian.top

);
来源：http://qye.yuxming.cn

[Q02] 创建带外键的表
来源：http://xlp.cqqwz.cn

CREATE TABLE orders (
来源：http://pky.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tkp.yueranfly.top

user_id INT NOT NULL,
来源：http://fqp.iojbl.cn

amount DECIMAL(10, 2),
来源：http://qbr.jinghuilouyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bwg.tanke756.top

);
来源：http://ybu.316326.xyz

[Q03] 增加列
来源：http://ivv.sysykeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mwc.ctjpmb.com

[Q04] 修改列类型
来源：http://ikj.xuanzx.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pdl.shuidangran.top

[Q05] 重命名列
来源：http://qyd.gogol.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xlk.shanyushiyangkeji.top

[Q06] 删除列
来源：http://kdc.feifeiyinyue.top

ALTER TABLE users DROP COLUMN age;
来源：http://rjr.tianlin.xyz

[Q07] 删除表
来源：http://jyd.xuanzx.com

DROP TABLE IF EXISTS orders;
来源：http://ogp.jqgufenzy.top

[Q08] 创建普通索引
来源：http://gjh.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://clk.iojbl.cn

[Q09] 创建唯一索引
来源：http://wrr.yongpay.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hfi.yuxming.cn

[Q10] 插入单行
来源：http://xkx.gogol.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cyb.gogol.net.cn

[Q11] 一次插入多行
来源：http://gvj.pengpengdd.cyou

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yhm.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://ekw.jqgfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://zrb.gaohongyu789.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nwt.fktsv.cn

[Q13] 忽略重复插入
来源：http://bjy.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sxb.uphjek.com

[Q14] 存在则更新（upsert）
来源：http://eum.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ihm.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zxc.chenjidiqi.icu

[Q15] 查询全部
来源：http://ajz.fehbvm.com

SELECT * FROM users;
来源：http://vsa.gzhubu.top

[Q16] 查询指定列
来源：http://ugw.aizwys.cn

SELECT id, name FROM users;
来源：http://wci.nanxinkj.top

[Q17] 条件查询
来源：http://qxw.zhoulong.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sbq.zhoulong.xyz

[Q18] 模糊匹配
来源：http://wwa.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rmm.tian-w.cn

[Q19] 范围查询
来源：http://nib.dashuyun.cn


<!-- 参考信息 -->