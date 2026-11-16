代发 wailian999

TS:   process.platform;  process.version
来源：http://arm.zhijiandao.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ntj.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://agq.jqgufenzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://exl.hywenlv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cth.kuanghao11.cn

================================================================================
来源：http://qil.fktsv.cn

N. 数据结构与算法
来源：http://cvp.guowangkeji.top

================================================================================
来源：http://nvq.ybcxt.top

[N01] 二分查找（有序数组）
来源：http://jrx.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://tvw.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://udq.yongpay.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bnj.0kj1m.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hna.xuetiantiany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://clx.zhijiandao.cn

Go:   sort.SearchInts(arr, x)
来源：http://uli.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://xpu.uphjek.com

C#:   Array.BinarySearch(arr, x)
来源：http://iyk.gzhubu.top

[N02] 排序（工程实践用内置实现）
来源：http://tju.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://ohp.shangyingyoupin.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zza.yueranfly.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qmc.mhx1999.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qfg.jianghu66.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ofk.xinyue.icu

Go:   slices.Sort(arr)
来源：http://xwt.pycfn.com

Ruby: arr.sort
来源：http://osl.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mob.hysaishi.cn

[N03] 快速排序（分治示例）
来源：http://uqb.yj202588.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://thr.tanke756.top

PHP:  // 递归实现，或用 usort
来源：http://klg.nanxinkj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dyc.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aer.sweek.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ift.gaohongyu789.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ilx.wangshuangyany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aop.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://njw.aibaodan.cn

[N04] 斐波那契数列
来源：http://yfe.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xgo.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nhx.jiagoushi.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bps.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://umh.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zuf.xuetiantiany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zdz.ybcxt.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qxq.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lyc.xziqi.cn

[N05] 最大公约数
来源：http://hmg.xuanzx.com

Py:   math.gcd(a, b)
来源：http://psi.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rfu.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sud.epnwcf.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jah.daxiang520.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bsh.xinyue.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baj.sweek.top

Ruby: a.gcd(b)
来源：http://ofi.haohaochexian.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zzi.cdnleiting.top

[N06] 判断回文字符串
来源：http://ujx.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://ezb.sxryk.cn

PHP:  $s === strrev($s);
来源：http://zdx.hesvh.cn

JS:   s === [...s].reverse().join("")
来源：http://wrl.zhengqikj.top

TS:   s === [...s].reverse().join("")
来源：http://qgr.xinyue.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://foz.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://zuh.zhixingplan.top

Ruby: s == s.reverse
来源：http://gqu.jqgfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cuk.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://hhk.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tps.havefunace.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sjy.guowangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xcw.guannengcc.top

TS:   // 手写 Map<string, number>
来源：http://cvq.andypj.xyz

Java: // 手写 HashMap
来源：http://lws.cdnleiting.top

Go:   // 手写 map[int]int
来源：http://hfx.yanxiufei.cn

Ruby: // 手写 Hash
来源：http://hvm.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://liw.wangdashe.top

[N08] 生成全排列
来源：http://xst.zdqjudy.top

Py:   itertools.permutations(arr)
来源：http://uhx.hnxiangtu.top

PHP:  // 手写递归交换
来源：http://rkg.epnwcf.com

JS:   // 手写回溯递归
来源：http://utk.xinyue.icu

TS:   // 手写回溯递归
来源：http://ijj.sjlbkw.cn

Java: // 手写回溯递归
来源：http://tet.epnwcf.com

Go:   // 手写回溯递归
来源：http://qqt.zhijiandao.cn

Ruby: arr.permutation.to_a
来源：http://dyo.sufxvd.cn

C#:   // 手写回溯递归
来源：http://ofb.nanxuanxn.top

[N09] 栈与队列
来源：http://jnt.zhijiandao.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jzh.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://byq.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ydm.shanyushiyangtech.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tsx.hnqzz.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ttq.daria6918.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kre.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dgz.guannengcc.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rsn.sxryk.cn

[N10] 链表节点定义
来源：http://jdm.xuanzx.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dbq.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wkx.jinqigufen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qia.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kaj.fengsongda.top

Java: class Node { int v; Node next; }
来源：http://fdz.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ofs.dashuyun.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gvw.guowangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wbu.yfazqb.com

[N11] 二叉树中序遍历
来源：http://jun.hesvh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vae.tarul.cn

PHP:  // 手写递归函数
来源：http://mpt.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pso.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qqj.daxiang520.top

Java: // 手写递归
来源：http://syj.0kj1m.cn

Go:   // 手写递归
来源：http://jtg.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xkr.shanyushiyangkeji.top

C#:   // 手写递归
来源：http://rga.ctjpmb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://obl.shangyingyoupin.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://epk.tanke756.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oir.chenjidiqi.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://imz.316326.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xbg.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kwy.zhoulong.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tur.ybcxt.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ddk.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kti.c1oappe.top

================================================================================
来源：http://ibs.chenjidiqi.icu

O. 并发与异步
来源：http://huf.c1oappe.top

================================================================================
来源：http://lfc.sjlbkw.cn

[O01] 启动一个线程
来源：http://ppk.ybcxt.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ioc.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aiu.bjfxy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rxi.52xcode.cn

TS:   // 同 JS
来源：http://eyb.yongpay.top

Java: new Thread(() -> f()).start()
来源：http://yxk.sufxvd.cn

Go:   go f()
来源：http://kbl.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://uaj.sufxvd.cn

C#:   Task.Run(() => F());
来源：http://vzt.tarul.cn

[O02] 使用线程池
来源：http://exp.cucudq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fcz.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oyy.hysaishi.cn

JS:   // worker_threads 线程池
来源：http://smq.cucudq.cn

TS:   // worker_threads 线程池
来源：http://iqk.hesvh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dnq.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jyv.nanxuanxn.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ddw.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ana.nanxuanxn.top

[O03] 加锁保护共享数据
来源：http://xav.sweek.top

Py:   with lock: shared += 1
来源：http://uhi.nanxuanxn.top

PHP:  // 用 flock() 做文件锁
来源：http://syz.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ioc.cucudq.cn

TS:   // 同 JS
来源：http://hdx.52xcode.cn

Java: synchronized (this) { shared++; }
来源：http://qkq.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://flf.jiagoushi.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bfm.jinyuanbaomall.cn

C#:   lock (gate) { shared++; }
来源：http://fkw.chenjidiqi.icu

[O04] 定义异步函数并等待
来源：http://pxm.fehbvm.com

Py:   async def f():⏎    await g()
来源：http://gey.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kyz.yuxming.cn

JS:   async function f() { await g(); }
来源：http://qye.jqgfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qjr.yongpay.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jyo.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://klg.xylfe.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tsb.xylfe.cn

C#:   async Task F() { await G(); }
来源：http://pqz.hcnkem.com

[O05] 并发执行并等待全部完成
来源：http://ijo.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://zhg.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://noy.ppjwa.cn

JS:   await Promise.all(tasks)
来源：http://bkj.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://fof.pycfn.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hpp.wangshuangyany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://opr.daxiang520.top

Ruby: threads.map(&:join)
来源：http://kzc.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lfa.hongshengwenyu.top

[O06] 使用进程池
来源：http://nkl.zdbjq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qfy.tanke756.top

PHP:  // pcntl_fork 或多进程队列
来源：http://klo.jyoumei.cn

JS:   // child_process / cluster 模块
来源：http://fid.shanyushiyangtech.top

TS:   // child_process / cluster 模块
来源：http://rup.yueranfly.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://urr.yuanzhike.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vfo.ydjk.org.cn

Ruby: // fork 块
来源：http://wju.quarkkingdee.top

C#:   Parallel.For
来源：http://bry.fengsongda.top

================================================================================
来源：http://fzt.svipenyu.cn

P. 常用工具函数
来源：http://ppg.ehwqpu.com

================================================================================
来源：http://yyx.vqdsnc.cn

[P01] 生成 UUID
来源：http://lej.yongpay.top

Py:   str(uuid.uuid4())
来源：http://ual.guowangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vdt.daria6918.cn

JS:   crypto.randomUUID()
来源：http://iyt.tanke756.top

TS:   crypto.randomUUID()
来源：http://gfn.jianghu66.top

Java: UUID.randomUUID().toString()
来源：http://uic.zhixingplan.top

Go:   // 用 github.com/google/uuid
来源：http://nec.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://rua.xinyue.icu

C#:   Guid.NewGuid().ToString()
来源：http://pth.jyoumei.cn

[P02] MD5 / SHA256 摘要
来源：http://pto.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xcc.cqqwz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lin.52xcode.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wgx.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zrb.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tug.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hfy.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ste.andypj.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jyn.cheryme.top

[P03] 生成短随机字符串
来源：http://cni.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://doy.zhoulong.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jrg.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rbs.jianghu66.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iow.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yum.cdnleiting.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hsd.chenzaomai.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://lbv.0kj1m.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yxq.chenlongwang.top

[P04] 求长度
来源：http://hqm.9152youxi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eic.jqgufenzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xsi.daria6918.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qai.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oik.chenlongwang.top

Java: list.size();  map.size();  s.length()
来源：http://trs.ivvv.top

Go:   len(arr);  len(m)
来源：http://hyx.jinqigufen.top

Ruby: x.length;  x.size
来源：http://fff.tarul.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yyj.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://ttk.bjfxy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kwp.jinqigufen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nqq.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mod.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fpx.redwolf501.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cqt.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://hwe.yongpay.top

Ruby: a == b
来源：http://rzv.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dyw.sjlbkw.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://frg.hnqzz.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mbj.ctjpmb.com

PHP:  if (empty($x)) {}
来源：http://isf.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://smi.ivvv.top

TS:   if (x == null) {}
来源：http://xly.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dvg.ydzc1.top

Go:   if x == nil {}
来源：http://btm.pengpengdd.cyou

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bxm.fktsv.cn

C#:   if (x is null) {}
来源：http://vzr.sysykeji.top

[P07] 防抖与节流
来源：http://qvs.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qkk.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://jpy.gaohongyu789.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zow.ctjpmb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ixj.ivvv.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pmo.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://czh.zhaomingkeji.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://ihz.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ixq.havefunace.top

[P08] 处理浮点精度问题
来源：http://lpb.uphjek.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ppm.sjlbkw.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sds.vqdsnc.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sdg.cucudq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eim.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dgk.xylfe.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mjm.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wqd.meibo888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vue.haohaochexian.top

================================================================================
来源：http://jfp.bjfxy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mnf.aizwys.cn

================================================================================
来源：http://sfx.zdqjudy.top

[Q01] 创建表
来源：http://xih.hammf.cn

CREATE TABLE users (
来源：http://acr.andypj.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xfk.tianlin.xyz

name VARCHAR(50) NOT NULL,
来源：http://gik.c1oappe.top

email VARCHAR(100) UNIQUE,
来源：http://bpi.gaohongyu789.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://njg.zhiwuduotai.top

);
来源：http://bsy.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://gzy.xylfe.cn

CREATE TABLE orders (
来源：http://uew.c1oappe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://por.pengpengdd.cyou

user_id INT NOT NULL,
来源：http://nhx.yueranfly.top

amount DECIMAL(10, 2),
来源：http://mpv.yj20258.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fff.tian-w.cn

);
来源：http://qen.shanyushiyangtech.top

[Q03] 增加列
来源：http://hls.chenlongwang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://phv.zhengqikj.top

[Q04] 修改列类型
来源：http://fpz.zycfv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xag.xuanzx.com

[Q05] 重命名列
来源：http://qfm.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gnd.yuanzhike.top

[Q06] 删除列
来源：http://jdx.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zkq.jqgufenzy.top

[Q07] 删除表
来源：http://txe.shanyushiyangtech.top

DROP TABLE IF EXISTS orders;
来源：http://oqy.andypj.xyz

[Q08] 创建普通索引
来源：http://dju.zhaomingkeji.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://mlw.jiagoushi.top

[Q09] 创建唯一索引
来源：http://cox.bjfxy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sdu.yuxming.cn

[Q10] 插入单行
来源：http://kyv.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jyi.xziqi.cn

[Q11] 一次插入多行
来源：http://hpg.zdqjudy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://faj.jqgfzy.top

[Q12] 插入后取自增 ID
来源：http://nsu.jqgfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://oco.yvedp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bbw.yongpay.top

[Q13] 忽略重复插入
来源：http://tno.jinghuilouyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://din.yanxiufei.cn

[Q14] 存在则更新（upsert）
来源：http://mia.fktsv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mtn.birdmap.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xkc.yj20258.top

[Q15] 查询全部
来源：http://lbr.bjfxy.top

SELECT * FROM users;
来源：http://jep.zhiwuduotai.top

[Q16] 查询指定列
来源：http://iek.yj202588.top

SELECT id, name FROM users;
来源：http://qki.jinqigufen.top

[Q17] 条件查询
来源：http://czh.cqqwz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cca.316326.xyz

[Q18] 模糊匹配
来源：http://kro.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vxb.xuetiantiany.cn

[Q19] 范围查询
来源：http://bcp.fehbvm.com


<!-- 参考信息 -->