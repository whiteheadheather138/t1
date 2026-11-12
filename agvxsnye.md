代发 wailian999

[M08] 获取系统与运行时信息
来源：http://ttk.hongshengwenyu.top

Py:   platform.system();  platform.python_version()
来源：http://lpr.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://nbv.chenzaomai.com

JS:   process.platform;  process.version
来源：http://gwb.hammf.cn

TS:   process.platform;  process.version
来源：http://wix.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yvw.yvedp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dhm.aizwys.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mgs.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mkv.hnxiangtu.top

================================================================================
来源：http://wjl.iojbl.cn

N. 数据结构与算法
来源：http://jpt.chenlongwang.top

================================================================================
来源：http://xal.yonumen.top

[N01] 二分查找（有序数组）
来源：http://idl.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://mun.ppjwa.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dhf.shangyingyoupin.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pws.havefunace.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xxs.yj20258.top

Java: Arrays.binarySearch(arr, x)
来源：http://vah.feifeiyinyue.top

Go:   sort.SearchInts(arr, x)
来源：http://hon.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ajw.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://fks.sufxvd.cn

[N02] 排序（工程实践用内置实现）
来源：http://mzs.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://gxt.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ahc.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qag.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://irp.cheryme.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://icx.nwbrower.top

Go:   slices.Sort(arr)
来源：http://sgh.ctjpmb.com

Ruby: arr.sort
来源：http://ajz.fanxiaobao.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://kvh.tianlin.xyz

[N03] 快速排序（分治示例）
来源：http://elj.feifeiyinyue.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fdu.gaohongyu789.top

PHP:  // 递归实现，或用 usort
来源：http://ink.yanxiufei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ouo.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://trr.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vvc.yfazqb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xzf.c1oappe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ert.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://rhf.sxryk.cn

[N04] 斐波那契数列
来源：http://ydj.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ltc.ywan-chungtsiang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://svt.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://for.zhixingplan.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rau.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zmi.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qtg.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wlr.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zrf.mhx1999.top

[N05] 最大公约数
来源：http://zih.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://ktq.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xqj.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ozq.pengpengdd.cyou

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qma.nwbrower.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sdl.tarul.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pce.pycfn.com

Ruby: a.gcd(b)
来源：http://hfq.sxryk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jtx.bbcook.cn

[N06] 判断回文字符串
来源：http://wga.hcnkem.com

Py:   s == s[::-1]
来源：http://tmb.aizwys.cn

PHP:  $s === strrev($s);
来源：http://ytc.fehbvm.com

JS:   s === [...s].reverse().join("")
来源：http://asa.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://dks.fzhhl.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xoe.nanxinkj.top

Go:   // 双指针从两端比较
来源：http://rpn.yonumen.top

Ruby: s == s.reverse
来源：http://zeq.xinyue.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://pyb.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://xzn.pycfn.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kuy.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://euc.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://icx.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://gya.pycfn.com

Java: // 手写 HashMap
来源：http://djq.ctjpmb.com

Go:   // 手写 map[int]int
来源：http://uuv.havefunace.top

Ruby: // 手写 Hash
来源：http://vmq.cheryme.top

C#:   // 手写 Dictionary<int, int>
来源：http://cad.jqgfzy.top

[N08] 生成全排列
来源：http://hyb.andypj.xyz

Py:   itertools.permutations(arr)
来源：http://qom.hcnkem.com

PHP:  // 手写递归交换
来源：http://dez.ivvv.top

JS:   // 手写回溯递归
来源：http://ivm.316326.xyz

TS:   // 手写回溯递归
来源：http://zga.cashguo.top

Java: // 手写回溯递归
来源：http://nrb.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://kxg.zhaomingkeji.xyz

Ruby: arr.permutation.to_a
来源：http://dji.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://skh.daria6918.cn

[N09] 栈与队列
来源：http://tez.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://foz.fehbvm.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://znp.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sry.shanyushiyangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ypz.jqgfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cmg.gaohongyu789.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ozt.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jur.guowangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fvp.svipenyu.cn

[N10] 链表节点定义
来源：http://pax.chenlongwang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qsx.hfpthk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pzn.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cjp.dashuyun.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://end.jianghu66.top

Java: class Node { int v; Node next; }
来源：http://hmp.yuanzhike.top

Go:   type Node struct { V int; Next *Node }
来源：http://exk.xuetiantiany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jfx.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://yxz.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://nhw.bbcook.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kzy.cashguo.top

PHP:  // 手写递归函数
来源：http://aka.nwbrower.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wyj.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zyo.yonumen.top

Java: // 手写递归
来源：http://vuc.gogol.net.cn

Go:   // 手写递归
来源：http://yev.yj20258.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eoj.dianchejie.cn

C#:   // 手写递归
来源：http://npt.vqdsnc.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xzg.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iow.hfpthk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ipw.yvedp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cfu.cucudq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xcn.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://egw.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ewy.feifeiyinyue.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kyi.jinyuanbaomall.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pdt.snrcjt.cn

================================================================================
来源：http://xjj.hnqzz.top

O. 并发与异步
来源：http://iae.hammf.cn

================================================================================
来源：http://kut.c1oappe.top

[O01] 启动一个线程
来源：http://yfs.aizwys.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://toj.hcnkem.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kbj.vqdsnc.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uea.fzhhl.top

TS:   // 同 JS
来源：http://dvp.jqgfzy.top

Java: new Thread(() -> f()).start()
来源：http://wrb.dianchejie.cn

Go:   go f()
来源：http://uwe.guannengcc.top

Ruby: Thread.new { f }
来源：http://lgg.xuetiantiany.cn

C#:   Task.Run(() => F());
来源：http://haz.fktsv.cn

[O02] 使用线程池
来源：http://jvs.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://asc.jinqigfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fwf.yuxming.cn

JS:   // worker_threads 线程池
来源：http://ryl.ybcxt.top

TS:   // worker_threads 线程池
来源：http://bqi.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://bpv.fengsongda.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xyt.yongpay.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vqz.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kwl.nanxuanxn.top

[O03] 加锁保护共享数据
来源：http://ava.fehbvm.com

Py:   with lock: shared += 1
来源：http://rzk.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://wep.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://akd.ybcxt.top

TS:   // 同 JS
来源：http://vda.hfpthk.cn

Java: synchronized (this) { shared++; }
来源：http://ezp.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hie.sxryk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://upy.gotoacloud.top

C#:   lock (gate) { shared++; }
来源：http://yrr.hcnkem.com

[O04] 定义异步函数并等待
来源：http://njd.uphjek.com

Py:   async def f():⏎    await g()
来源：http://zay.xingfuxueyuan.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ihu.hcnkem.com

JS:   async function f() { await g(); }
来源：http://idj.bjfxy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gca.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hys.ppjwa.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xro.fktsv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xvd.yangfankeji.com

C#:   async Task F() { await G(); }
来源：http://cqa.hcnkem.com

[O05] 并发执行并等待全部完成
来源：http://gii.bjfxy.top

Py:   asyncio.gather(*tasks)
来源：http://cjo.shzxlz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://chi.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://aih.vehdjk.com

TS:   await Promise.all(tasks)
来源：http://lhs.yonumen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eza.vqdsnc.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rdu.meibo888.top

Ruby: threads.map(&:join)
来源：http://uru.yonumen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xvg.hesvh.cn

[O06] 使用进程池
来源：http://iqk.cdnleiting.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://llz.tanke756.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cfg.jqgufenzy.top

JS:   // child_process / cluster 模块
来源：http://fim.xuanzx.com

TS:   // child_process / cluster 模块
来源：http://dmr.jinqigfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://khu.shzxlz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jcr.mhx1999.top

Ruby: // fork 块
来源：http://ugz.xuanzx.com

C#:   Parallel.For
来源：http://hxu.yfazqb.com

================================================================================
来源：http://szx.gogol.net.cn

P. 常用工具函数
来源：http://qcu.yj20258888.top

================================================================================
来源：http://eli.jinqigfzy.top

[P01] 生成 UUID
来源：http://tgo.pengpengdd.cyou

Py:   str(uuid.uuid4())
来源：http://vmy.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aww.wangshuangyany.cn

JS:   crypto.randomUUID()
来源：http://ghg.jianghu66.top

TS:   crypto.randomUUID()
来源：http://din.gotoacloud.top

Java: UUID.randomUUID().toString()
来源：http://qas.jlsjyb.cn

Go:   // 用 github.com/google/uuid
来源：http://zso.dashuyun.cn

Ruby: SecureRandom.uuid
来源：http://ldm.ydzc1.top

C#:   Guid.NewGuid().ToString()
来源：http://gib.zdqjudy.top

[P02] MD5 / SHA256 摘要
来源：http://jzf.ydjk.org.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fpy.fengsongda.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pkc.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uly.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zmj.vehdjk.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uli.ctjpmb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yyd.hywenlv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mrf.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zlw.tanke756.top

[P03] 生成短随机字符串
来源：http://ola.snrcjt.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xco.fktsv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sdx.zhoulong.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qlu.ydzc1.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gdf.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://shy.ydzc1.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hqd.yfazqb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://znp.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ohr.shanyushiyangkeji.top

[P04] 求长度
来源：http://mhd.pycfn.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cfl.xinyue.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qrj.ivvv.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://njd.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hpr.tianlin.xyz

Java: list.size();  map.size();  s.length()
来源：http://tqn.yueranfly.top

Go:   len(arr);  len(m)
来源：http://jug.ehwqpu.com

Ruby: x.length;  x.size
来源：http://aqq.svipenyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://iah.smart0.xyz

[P05] 判断两个对象内容是否相等
来源：http://jep.shangyingyoupin.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nwa.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nph.pengpengdd.cyou

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fuo.hywenlv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gwr.hesvh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bnp.sweek.top

Go:   reflect.DeepEqual(a, b)
来源：http://qyv.52xcode.cn

Ruby: a == b
来源：http://jad.quarkkingdee.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ubq.xylfe.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vcd.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tye.zdqjudy.top

PHP:  if (empty($x)) {}
来源：http://rrj.xingfuxueyuan.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jjz.haohaochexian.top

TS:   if (x == null) {}
来源：http://mju.jinqigufen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://keg.cucudq.cn

Go:   if x == nil {}
来源：http://kog.jinghuilouyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nvz.jqgfzy.top

C#:   if (x is null) {}
来源：http://lfr.zhongyouzk.top

[P07] 防抖与节流
来源：http://hlg.nwbrower.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iiz.zhiwuduotai.top

PHP:  // 手写时间戳比较
来源：http://ozb.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ric.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iug.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dtn.fengsongda.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zyy.cdnleiting.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://txn.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bxc.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://zkw.yuanzhike.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lmd.jyoumei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cfs.nanxuanxn.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mec.zhaomingkeji.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://trn.316326.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dkc.jyoumei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hcn.xuetiantiany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rzu.zhoulong.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bve.aizwys.cn

================================================================================
来源：http://ncu.gogol.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://goq.sjlbkw.cn

================================================================================
来源：http://slv.xingfuxueyuan.xyz

[Q01] 创建表
来源：http://non.jlsjyb.cn

CREATE TABLE users (
来源：http://nev.smart0.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bqh.daxiang520.top

name VARCHAR(50) NOT NULL,
来源：http://nar.jinqigufen.top

email VARCHAR(100) UNIQUE,
来源：http://cks.dianchejie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hbi.cucudq.cn

);
来源：http://dvv.fengsongda.top

[Q02] 创建带外键的表
来源：http://pym.birdmap.top

CREATE TABLE orders (
来源：http://pwf.vehdjk.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vsc.ctjpmb.com

user_id INT NOT NULL,
来源：http://boh.svipenyu.cn

amount DECIMAL(10, 2),
来源：http://msu.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sob.fanxiaobao.xyz

);
来源：http://acv.yvedp.cn

[Q03] 增加列
来源：http://qnz.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://guj.zhongyouzk.top

[Q04] 修改列类型
来源：http://iai.haohaochexian.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bpq.jyoumei.cn

[Q05] 重命名列
来源：http://uqk.zdqjudy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://olk.sxryk.cn

[Q06] 删除列
来源：http://bqb.zhiwuduotai.top

ALTER TABLE users DROP COLUMN age;
来源：http://iqb.fzhhl.top

[Q07] 删除表
来源：http://chw.sjlbkw.cn

DROP TABLE IF EXISTS orders;
来源：http://igr.sweek.top

[Q08] 创建普通索引
来源：http://jcd.cashguo.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ufg.zhongyouzk.top

[Q09] 创建唯一索引
来源：http://ine.guannengcc.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xrh.vqdsnc.cn

[Q10] 插入单行
来源：http://yfi.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lag.aizwys.cn

[Q11] 一次插入多行
来源：http://trl.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://szt.smart0.xyz

[Q12] 插入后取自增 ID
来源：http://rox.tian-w.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xbf.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uhz.tianlin.xyz

[Q13] 忽略重复插入
来源：http://unk.dianchejie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zzz.ydzc1.top

[Q14] 存在则更新（upsert）
来源：http://fwx.yj20258.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wrv.xingfuxueyuan.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lwg.gzhubu.top

[Q15] 查询全部
来源：http://fmk.dashuyun.cn

SELECT * FROM users;
来源：http://arh.zdqjudy.top

[Q16] 查询指定列
来源：http://tfc.smart0.xyz

SELECT id, name FROM users;
来源：http://qch.jqgfzy.top

[Q17] 条件查询
来源：http://lhr.zhengqikj.top


<!-- 参考信息 -->