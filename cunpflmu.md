代发 wailian999

[M08] 获取系统与运行时信息
来源：http://zes.cdnleiting.top

Py:   platform.system();  platform.python_version()
来源：http://hqb.nanxinkj.top

PHP:  PHP_OS;  phpversion();
来源：http://pvm.shzxlz.cn

JS:   process.platform;  process.version
来源：http://pug.cashguo.top

TS:   process.platform;  process.version
来源：http://qme.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kwk.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jbr.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dii.jyoumei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nln.52xcode.cn

================================================================================
来源：http://yka.tanke756.top

N. 数据结构与算法
来源：http://wrk.0kj1m.cn

================================================================================
来源：http://dyk.mhx1999.top

[N01] 二分查找（有序数组）
来源：http://xzr.gotoacloud.top

Py:   bisect.bisect_left(arr, x)
来源：http://msc.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://quw.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kkv.sufxvd.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pgg.ppjwa.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xhj.ybcxt.top

Go:   sort.SearchInts(arr, x)
来源：http://yjv.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zrl.vqdsnc.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nqw.uphjek.com

[N02] 排序（工程实践用内置实现）
来源：http://zjq.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ivh.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xux.zhoulong.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ygk.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://thx.ywan-chungtsiang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eaw.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://tdp.kuanghao11.cn

Ruby: arr.sort
来源：http://mde.fzhhl.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pbb.jiagoushi.top

[N03] 快速排序（分治示例）
来源：http://skh.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vhj.iojbl.cn

PHP:  // 递归实现，或用 usort
来源：http://xif.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oqh.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lbe.feifeiyinyue.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lmi.zhaomingkeji.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kkr.smart0.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xre.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://xja.shangyingyoupin.top

[N04] 斐波那契数列
来源：http://lam.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pkr.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ihu.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jai.yj20258.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zme.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://goj.xziqi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ysr.fktsv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mab.sufxvd.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oix.jyoumei.cn

[N05] 最大公约数
来源：http://igi.zycfv.cn

Py:   math.gcd(a, b)
来源：http://wcx.birdmap.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iek.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://skp.cdnleiting.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jbr.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://guw.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ksw.ehwqpu.com

Ruby: a.gcd(b)
来源：http://bex.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://siu.chenjidiqi.icu

[N06] 判断回文字符串
来源：http://umr.zdqjudy.top

Py:   s == s[::-1]
来源：http://hxr.cdnleiting.top

PHP:  $s === strrev($s);
来源：http://yzk.smart0.xyz

JS:   s === [...s].reverse().join("")
来源：http://ugv.daria6918.cn

TS:   s === [...s].reverse().join("")
来源：http://bcg.jinyuanbaomall.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rjr.xingfuxueyuan.xyz

Go:   // 双指针从两端比较
来源：http://lkq.daria6918.cn

Ruby: s == s.reverse
来源：http://pbm.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ipz.xziqi.cn

[N07] 两数之和（返回下标）
来源：http://odw.fehbvm.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://abf.316326.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vyt.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://usy.feifeiyinyue.top

TS:   // 手写 Map<string, number>
来源：http://vqz.epnwcf.com

Java: // 手写 HashMap
来源：http://ljq.jinyuanbaomall.cn

Go:   // 手写 map[int]int
来源：http://gzl.hnxiangtu.top

Ruby: // 手写 Hash
来源：http://izd.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sjr.nanxuanxn.top

[N08] 生成全排列
来源：http://vfx.dianchejie.cn

Py:   itertools.permutations(arr)
来源：http://zyo.zhengqikj.top

PHP:  // 手写递归交换
来源：http://oji.bbcook.cn

JS:   // 手写回溯递归
来源：http://fxr.cheryme.top

TS:   // 手写回溯递归
来源：http://jss.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://nso.meibo888.top

Go:   // 手写回溯递归
来源：http://osm.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://ixn.chenzaomai.com

C#:   // 手写回溯递归
来源：http://oky.ivvv.top

[N09] 栈与队列
来源：http://iyq.smart0.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wim.hongshengwenyu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rqu.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://izj.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ggw.hywenlv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://onk.guowangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ikd.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fig.tian-w.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vuv.yuxming.cn

[N10] 链表节点定义
来源：http://wga.daria6918.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qze.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xvs.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ntf.hnxiangtu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://frw.kuanghao11.cn

Java: class Node { int v; Node next; }
来源：http://ipo.yanxiufei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ody.shanyushiyangtech.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bzr.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://zsp.havefunace.top

[N11] 二叉树中序遍历
来源：http://tqi.fanxiaobao.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ulc.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://qyz.jyoumei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sri.zhiwuduotai.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cyv.zhoulong.xyz

Java: // 手写递归
来源：http://oyf.yanxiufei.cn

Go:   // 手写递归
来源：http://bue.zhoulong.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://koe.xinyue.icu

C#:   // 手写递归
来源：http://fir.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://psz.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rjb.tanke756.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xyq.fzhhl.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wyx.chenzaomai.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ezd.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rvk.fzhhl.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://trq.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://axs.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qhw.yuxming.cn

================================================================================
来源：http://rko.fktsv.cn

O. 并发与异步
来源：http://nkm.xziqi.cn

================================================================================
来源：http://wma.hywenlv.cn

[O01] 启动一个线程
来源：http://suq.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tkh.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mii.bbcook.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pln.yvedp.cn

TS:   // 同 JS
来源：http://pvr.jinyuanbaomall.cn

Java: new Thread(() -> f()).start()
来源：http://mll.xinyue.icu

Go:   go f()
来源：http://vqq.feifeiyinyue.top

Ruby: Thread.new { f }
来源：http://tmo.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://nwz.ydjk.org.cn

[O02] 使用线程池
来源：http://wqq.daxiang520.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://stu.zdqjudy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fhu.0kj1m.cn

JS:   // worker_threads 线程池
来源：http://gsr.yuanzhike.top

TS:   // worker_threads 线程池
来源：http://wqw.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://dax.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nev.xylfe.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iyy.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://apf.xuanzx.com

[O03] 加锁保护共享数据
来源：http://ure.pycfn.com

Py:   with lock: shared += 1
来源：http://ovv.uphjek.com

PHP:  // 用 flock() 做文件锁
来源：http://xkn.ydzc1.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yne.hongshengwenyu.top

TS:   // 同 JS
来源：http://rgb.mhx1999.top

Java: synchronized (this) { shared++; }
来源：http://rwe.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ryr.havefunace.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://evc.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://xgl.sweek.top

[O04] 定义异步函数并等待
来源：http://jgi.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://uzy.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mdh.xylfe.cn

JS:   async function f() { await g(); }
来源：http://sjs.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dsr.nwbrower.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ijp.wangshuangyany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://npp.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://vds.andypj.xyz

C#:   async Task F() { await G(); }
来源：http://lhc.yuanzhike.top

[O05] 并发执行并等待全部完成
来源：http://buz.sjlbkw.cn

Py:   asyncio.gather(*tasks)
来源：http://gfm.fzhhl.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bph.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://jir.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://jnq.52xcode.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wgf.yj20258.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ake.yuxming.cn

Ruby: threads.map(&:join)
来源：http://rch.havefunace.top

C#:   await Task.WhenAll(t1, t2)
来源：http://iuv.hongshengwenyu.top

[O06] 使用进程池
来源：http://tkv.kuanghao11.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hrv.xuetiantiany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jtz.uphjek.com

JS:   // child_process / cluster 模块
来源：http://mmv.hcnkem.com

TS:   // child_process / cluster 模块
来源：http://qik.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://swe.epnwcf.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eva.sysykeji.top

Ruby: // fork 块
来源：http://bsz.jqgufenzy.top

C#:   Parallel.For
来源：http://rie.yfazqb.com

================================================================================
来源：http://xby.yueranfly.top

P. 常用工具函数
来源：http://uhp.jiagoushi.top

================================================================================
来源：http://yvt.zhixingplan.top

[P01] 生成 UUID
来源：http://lme.jyoumei.cn

Py:   str(uuid.uuid4())
来源：http://lkm.jianghu66.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ipv.vehdjk.com

JS:   crypto.randomUUID()
来源：http://cby.316326.xyz

TS:   crypto.randomUUID()
来源：http://ixv.0kj1m.cn

Java: UUID.randomUUID().toString()
来源：http://dek.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://rme.cheryme.top

Ruby: SecureRandom.uuid
来源：http://iez.shzxlz.cn

C#:   Guid.NewGuid().ToString()
来源：http://nkg.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://pgm.fehbvm.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mwe.zycfv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ogv.zdqjudy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ial.zhengqikj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fvn.sysykeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fvq.nanxuanxn.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fyi.ydjk.org.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qzs.yonumen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cuf.gaohongyu789.top

[P03] 生成短随机字符串
来源：http://ysy.jinqigufen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fhd.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mib.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zuk.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pnb.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nll.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gss.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://svn.jqgfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wvj.redwolf501.top

[P04] 求长度
来源：http://cxy.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wyd.yuxming.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pqc.ydjk.org.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://axi.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yzt.vqdsnc.cn

Java: list.size();  map.size();  s.length()
来源：http://nev.mhx1999.top

Go:   len(arr);  len(m)
来源：http://qce.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://wvq.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bhz.ctjpmb.com

[P05] 判断两个对象内容是否相等
来源：http://nyl.daria6918.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qkt.zhixingplan.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oro.yuxming.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fxt.yj20258888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://opv.fehbvm.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kbv.gogol.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wwp.yj20258888.top

Ruby: a == b
来源：http://org.ivvv.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nba.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bog.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://abu.ydjk.org.cn

PHP:  if (empty($x)) {}
来源：http://zvf.bbcook.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://byt.jinqigfzy.top

TS:   if (x == null) {}
来源：http://ksr.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cdo.daria6918.cn

Go:   if x == nil {}
来源：http://dmk.316326.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cgx.shanyushiyangtech.top

C#:   if (x is null) {}
来源：http://ypx.sweek.top

[P07] 防抖与节流
来源：http://ofe.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xbn.hfpthk.cn

PHP:  // 手写时间戳比较
来源：http://kob.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lhf.ydjk.org.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xcl.yanxiufei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bck.52xcode.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tga.zhijiandao.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rhx.cheryme.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lhi.svipenyu.cn

[P08] 处理浮点精度问题
来源：http://ttg.epnwcf.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sog.tarul.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mxu.zhiwuduotai.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://phd.daxiang520.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mjp.dianchejie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pda.haohaochexian.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vsq.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hwv.meibo888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kdf.shanyushiyangkeji.top

================================================================================
来源：http://nqb.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dyv.smart0.xyz

================================================================================
来源：http://zxo.jlsjyb.cn

[Q01] 创建表
来源：http://oxw.nwbrower.top

CREATE TABLE users (
来源：http://lkc.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eye.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://rgk.shuidangran.top

email VARCHAR(100) UNIQUE,
来源：http://soy.shuidangran.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nvw.jinghuilouyu.cn

);
来源：http://rjx.feifeiyinyue.top

[Q02] 创建带外键的表
来源：http://qjr.sxryk.cn

CREATE TABLE orders (
来源：http://yzv.zhoulong.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mes.chenzaomai.com

user_id INT NOT NULL,
来源：http://rve.guannengcc.top

amount DECIMAL(10, 2),
来源：http://fju.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cpv.nwbrower.top

);
来源：http://ivz.quarkkingdee.top

[Q03] 增加列
来源：http://uip.jianghu66.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vys.fktsv.cn

[Q04] 修改列类型
来源：http://ugr.zhaomingkeji.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wsx.andypj.xyz

[Q05] 重命名列
来源：http://mou.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jfb.hesvh.cn

[Q06] 删除列
来源：http://cpt.zhixingplan.top

ALTER TABLE users DROP COLUMN age;
来源：http://ulm.xuanzx.com

[Q07] 删除表
来源：http://fcg.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://zbz.guannengcc.top

[Q08] 创建普通索引
来源：http://yxo.aizwys.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wza.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://ajp.daxiang520.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://znt.hcnkem.com

[Q10] 插入单行
来源：http://cjc.yj20258.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vyq.smart0.xyz

[Q11] 一次插入多行
来源：http://moi.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://osq.havefunace.top

[Q12] 插入后取自增 ID
来源：http://zks.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://xym.sysykeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uvk.52xcode.cn

[Q13] 忽略重复插入
来源：http://gcu.hnqzz.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gdn.chenzaomai.com

[Q14] 存在则更新（upsert）
来源：http://epn.shanyushiyangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://clg.shangyingyoupin.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fzy.zdbjq.cn

[Q15] 查询全部
来源：http://fid.cashguo.top

SELECT * FROM users;
来源：http://iwe.jiagoushi.top

[Q16] 查询指定列
来源：http://yaz.yueranfly.top

SELECT id, name FROM users;
来源：http://npv.jqgufenzy.top

[Q17] 条件查询
来源：http://fpf.iojbl.cn


<!-- 参考信息 -->