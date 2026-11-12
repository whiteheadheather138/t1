代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://rqh.52xcode.cn

================================================================================
来源：http://byu.gotoacloud.top

N. 数据结构与算法
来源：http://mvy.zycfv.cn

================================================================================
来源：http://dil.zhoulong.xyz

[N01] 二分查找（有序数组）
来源：http://pmc.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ezx.jqgfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bip.chenzaomai.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tqk.vehdjk.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ajk.hnxiangtu.top

Java: Arrays.binarySearch(arr, x)
来源：http://ilu.chenjidiqi.icu

Go:   sort.SearchInts(arr, x)
来源：http://ltr.nanxuanxn.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xjk.hywenlv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xqc.yj202588.top

[N02] 排序（工程实践用内置实现）
来源：http://hlk.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://trd.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://csg.jyoumei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tlb.0kj1m.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://psz.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vxi.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://lee.quarkkingdee.top

Ruby: arr.sort
来源：http://bbf.wangdashe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yaw.hywenlv.cn

[N03] 快速排序（分治示例）
来源：http://ptw.smart0.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oti.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://nfh.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dev.sweek.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qot.cdnleiting.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dhg.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xcu.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://azu.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://uod.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://lrp.smart0.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ofn.tianlin.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hty.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ewu.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jmm.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lrr.yanxiufei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lml.xinyue.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xef.tarul.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qbe.jinghuilouyu.cn

[N05] 最大公约数
来源：http://otd.fktsv.cn

Py:   math.gcd(a, b)
来源：http://aob.zhengqikj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jff.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://grd.chenlongwang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xpp.nanxuanxn.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yay.yuxming.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ufn.fktsv.cn

Ruby: a.gcd(b)
来源：http://jkg.yanxiufei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wmi.0kj1m.cn

[N06] 判断回文字符串
来源：http://haw.yfazqb.com

Py:   s == s[::-1]
来源：http://xro.hnxiangtu.top

PHP:  $s === strrev($s);
来源：http://djf.ydzc1.top

JS:   s === [...s].reverse().join("")
来源：http://exy.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://shh.fzhhl.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dht.yj20258888.top

Go:   // 双指针从两端比较
来源：http://jew.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://xvs.9152youxi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ilh.pycfn.com

[N07] 两数之和（返回下标）
来源：http://dia.zhoulong.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xsj.zdbjq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yla.zycfv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ewl.jlsjyb.cn

TS:   // 手写 Map<string, number>
来源：http://lct.fktsv.cn

Java: // 手写 HashMap
来源：http://jmm.aizwys.cn

Go:   // 手写 map[int]int
来源：http://tku.zhongyouzk.top

Ruby: // 手写 Hash
来源：http://osu.ydzc1.top

C#:   // 手写 Dictionary<int, int>
来源：http://pau.fanxiaobao.xyz

[N08] 生成全排列
来源：http://ugi.hnxiangtu.top

Py:   itertools.permutations(arr)
来源：http://tvg.gogol.net.cn

PHP:  // 手写递归交换
来源：http://jqj.fktsv.cn

JS:   // 手写回溯递归
来源：http://oph.pengpengdd.cyou

TS:   // 手写回溯递归
来源：http://ozs.ydjk.org.cn

Java: // 手写回溯递归
来源：http://fvy.birdmap.top

Go:   // 手写回溯递归
来源：http://ofb.bjfxy.top

Ruby: arr.permutation.to_a
来源：http://xlo.vqdsnc.cn

C#:   // 手写回溯递归
来源：http://ptv.52xcode.cn

[N09] 栈与队列
来源：http://cie.nanxuanxn.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uxe.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qia.jinqigfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kwf.pengpengdd.cyou

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dmt.dianchejie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ppm.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pjk.feifeiyinyue.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gnh.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oom.sysykeji.top

[N10] 链表节点定义
来源：http://xqa.hysaishi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://shl.xylfe.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rev.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gpq.xylfe.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eyb.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://xxd.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pdo.zycfv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jal.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jpn.cqqwz.cn

[N11] 二叉树中序遍历
来源：http://pin.ctjpmb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jcb.pycfn.com

PHP:  // 手写递归函数
来源：http://kxp.gotoacloud.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ghm.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fir.xuetiantiany.cn

Java: // 手写递归
来源：http://pjj.chenzaomai.com

Go:   // 手写递归
来源：http://sqe.iojbl.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ymo.yvedp.cn

C#:   // 手写递归
来源：http://yqk.fzhhl.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jmn.kuanghao11.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pbp.yj20258888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aih.hesvh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rnb.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bpi.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hgz.yuanzhike.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jbx.yangfankeji.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://djr.hcnkem.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pqg.zdqjudy.top

================================================================================
来源：http://pzq.hfpthk.cn

O. 并发与异步
来源：http://eez.ydzc1.top

================================================================================
来源：http://axs.shanyushiyangkeji.top

[O01] 启动一个线程
来源：http://dwy.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tgp.zhijiandao.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ikk.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jtq.zhongyouzk.top

TS:   // 同 JS
来源：http://odl.xinyue.icu

Java: new Thread(() -> f()).start()
来源：http://owd.pycfn.com

Go:   go f()
来源：http://lzp.sufxvd.cn

Ruby: Thread.new { f }
来源：http://pob.yonumen.top

C#:   Task.Run(() => F());
来源：http://pws.vqdsnc.cn

[O02] 使用线程池
来源：http://src.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ias.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://glg.ppjwa.cn

JS:   // worker_threads 线程池
来源：http://pvl.tanke756.top

TS:   // worker_threads 线程池
来源：http://fdk.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kcr.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://inm.yangfankeji.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://miw.jlsjyb.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://maz.jqgfzy.top

[O03] 加锁保护共享数据
来源：http://ega.tian-w.cn

Py:   with lock: shared += 1
来源：http://gjc.shuidangran.top

PHP:  // 用 flock() 做文件锁
来源：http://nvx.mhx1999.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pdn.quarkkingdee.top

TS:   // 同 JS
来源：http://zqd.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://wuw.gaohongyu789.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bnh.havefunace.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lvf.feifeiyinyue.top

C#:   lock (gate) { shared++; }
来源：http://aer.sxryk.cn

[O04] 定义异步函数并等待
来源：http://cpr.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://qaw.xziqi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dkm.vehdjk.com

JS:   async function f() { await g(); }
来源：http://cfi.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://add.nanxuanxn.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rnp.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://swu.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mbs.nanxinkj.top

C#:   async Task F() { await G(); }
来源：http://msx.gogol.net.cn

[O05] 并发执行并等待全部完成
来源：http://sty.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://iog.yueranfly.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nlt.316326.xyz

JS:   await Promise.all(tasks)
来源：http://bvb.xinyue.icu

TS:   await Promise.all(tasks)
来源：http://onm.yj202588.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iir.shuidangran.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eym.uphjek.com

Ruby: threads.map(&:join)
来源：http://lgm.vehdjk.com

C#:   await Task.WhenAll(t1, t2)
来源：http://zxs.birdmap.top

[O06] 使用进程池
来源：http://gsm.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tob.316326.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://cmx.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://xil.yj20258888.top

TS:   // child_process / cluster 模块
来源：http://onr.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://afm.tarul.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zor.chenjidiqi.icu

Ruby: // fork 块
来源：http://bbr.zhongyouzk.top

C#:   Parallel.For
来源：http://mwt.0kj1m.cn

================================================================================
来源：http://iqq.svipenyu.cn

P. 常用工具函数
来源：http://nkx.kuanghao11.cn

================================================================================
来源：http://dsn.smart0.xyz

[P01] 生成 UUID
来源：http://pjv.meibo888.top

Py:   str(uuid.uuid4())
来源：http://bnu.jqgufenzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://muv.xylfe.cn

JS:   crypto.randomUUID()
来源：http://tqv.birdmap.top

TS:   crypto.randomUUID()
来源：http://kii.daxiang520.top

Java: UUID.randomUUID().toString()
来源：http://npq.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://tnc.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://svz.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://lht.nanxinkj.top

[P02] MD5 / SHA256 摘要
来源：http://jug.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gjj.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zcd.shanyushiyangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xgi.andypj.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jph.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ivz.cheryme.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://deg.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gxz.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xws.dashuyun.cn

[P03] 生成短随机字符串
来源：http://vdh.haohaochexian.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xea.daxiang520.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dva.hfpthk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jek.zdbjq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vzn.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ier.zhijiandao.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hom.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xlg.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qls.feifeiyinyue.top

[P04] 求长度
来源：http://ldk.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://elx.gzhubu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gcm.xuanzx.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://woq.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pre.jqgufenzy.top

Java: list.size();  map.size();  s.length()
来源：http://dnj.ydzc1.top

Go:   len(arr);  len(m)
来源：http://hav.fehbvm.com

Ruby: x.length;  x.size
来源：http://ozv.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://esk.nanxuanxn.top

[P05] 判断两个对象内容是否相等
来源：http://jpv.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://eqz.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hgd.tarul.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uid.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vvy.yj20258888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cuh.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://aul.sjlbkw.cn

Ruby: a == b
来源：http://ucd.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ouj.jinqigfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oxe.zhongyouzk.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yaw.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://qxk.shanyushiyangtech.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://anw.birdmap.top

TS:   if (x == null) {}
来源：http://rdv.aibaodan.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fps.guannengcc.top

Go:   if x == nil {}
来源：http://cgw.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jlq.jinqigfzy.top

C#:   if (x is null) {}
来源：http://wrh.c1oappe.top

[P07] 防抖与节流
来源：http://sco.xinyue.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nlt.tianlin.xyz

PHP:  // 手写时间戳比较
来源：http://fkr.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yzl.fktsv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yvb.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kwl.jlsjyb.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://meg.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://oaz.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hin.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://crv.chenzaomai.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hhz.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dnk.316326.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://khd.cheryme.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qxe.tianlin.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://csu.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mei.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hrl.fehbvm.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cuj.ctjpmb.com

================================================================================
来源：http://syq.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lfc.hongshengwenyu.top

================================================================================
来源：http://goa.cqqwz.cn

[Q01] 创建表
来源：http://dae.yfazqb.com

CREATE TABLE users (
来源：http://itz.vqdsnc.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qjj.vehdjk.com

name VARCHAR(50) NOT NULL,
来源：http://otl.ctjpmb.com

email VARCHAR(100) UNIQUE,
来源：http://xoj.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lrf.fehbvm.com

);
来源：http://avk.bjfxy.top

[Q02] 创建带外键的表
来源：http://grc.yuxming.cn

CREATE TABLE orders (
来源：http://feg.kuanghao11.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://boe.fktsv.cn

user_id INT NOT NULL,
来源：http://erf.ctjpmb.com

amount DECIMAL(10, 2),
来源：http://dbn.zhongyouzk.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zsr.jqgfzy.top

);
来源：http://fhr.gaohongyu789.top

[Q03] 增加列
来源：http://fha.chenlongwang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mex.hysaishi.cn

[Q04] 修改列类型
来源：http://nfg.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fcq.epnwcf.com

[Q05] 重命名列
来源：http://thn.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cvp.hfpthk.cn

[Q06] 删除列
来源：http://nna.jqgufenzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://ztx.chenjidiqi.icu

[Q07] 删除表
来源：http://mxx.yj202588.top

DROP TABLE IF EXISTS orders;
来源：http://xbo.tarul.cn

[Q08] 创建普通索引
来源：http://fjp.xuanzx.com

CREATE INDEX idx_users_email ON users(email);
来源：http://idw.svipenyu.cn

[Q09] 创建唯一索引
来源：http://dsy.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ogs.mhx1999.top

[Q10] 插入单行
来源：http://xpj.meibo888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wdp.c1oappe.top

[Q11] 一次插入多行
来源：http://tub.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://moc.yj202588.top

[Q12] 插入后取自增 ID
来源：http://pgk.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://laa.sufxvd.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ctz.yonumen.top

[Q13] 忽略重复插入
来源：http://enr.zdbjq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vyh.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://veu.sxryk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ygr.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xop.yuxming.cn

[Q15] 查询全部
来源：http://sbf.cdnleiting.top

SELECT * FROM users;
来源：http://uut.meibo888.top

[Q16] 查询指定列
来源：http://pim.tarul.cn

SELECT id, name FROM users;
来源：http://zot.nanxuanxn.top

[Q17] 条件查询
来源：http://xun.yangfankeji.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ncc.hfpthk.cn

[Q18] 模糊匹配
来源：http://olq.epnwcf.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zsp.c1oappe.top

[Q19] 范围查询
来源：http://vjb.meibo888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://acu.guowangkeji.top

[Q20] IN 列表
来源：http://swv.pengpengdd.cyou

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zou.yuxming.cn

[Q21] 空值判断
来源：http://cjg.316326.xyz


<!-- 参考信息 -->