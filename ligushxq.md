代发 wailian999

[N01] 二分查找（有序数组）
来源：http://mgd.zycfv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kxg.nwbrower.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mzq.c1oappe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ccv.yueranfly.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bmo.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bps.cqqwz.cn

Go:   sort.SearchInts(arr, x)
来源：http://sue.sufxvd.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wtn.gotoacloud.top

C#:   Array.BinarySearch(arr, x)
来源：http://uuu.hammf.cn

[N02] 排序（工程实践用内置实现）
来源：http://dcs.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://rdc.zhixingplan.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gkp.epnwcf.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://gyz.hywenlv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mwr.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://afz.cheryme.top

Go:   slices.Sort(arr)
来源：http://vcc.fehbvm.com

Ruby: arr.sort
来源：http://gfu.zhixingplan.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rug.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://gdl.haohaochexian.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mzj.sjlbkw.cn

PHP:  // 递归实现，或用 usort
来源：http://sjn.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fwu.mhx1999.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://obl.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dcp.zdqjudy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ivz.jiagoushi.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kcy.gaohongyu789.top

C#:   // 手写递归，或 Array.Sort
来源：http://qcf.jianghu66.top

[N04] 斐波那契数列
来源：http://zfz.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yzi.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jbb.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qrz.shanyushiyangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ymq.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qcu.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iuy.vehdjk.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qfg.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uer.zycfv.cn

[N05] 最大公约数
来源：http://qhe.zdbjq.cn

Py:   math.gcd(a, b)
来源：http://ogd.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://grw.wangdashe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xcc.316326.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xae.9152youxi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ygj.ywan-chungtsiang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nob.jlsjyb.cn

Ruby: a.gcd(b)
来源：http://jxc.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ook.vqdsnc.cn

[N06] 判断回文字符串
来源：http://ohz.tianlin.xyz

Py:   s == s[::-1]
来源：http://jty.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://spe.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://trz.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://wjk.sjlbkw.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hme.dianchejie.cn

Go:   // 双指针从两端比较
来源：http://ldo.nanxuanxn.top

Ruby: s == s.reverse
来源：http://dsk.yvedp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nbn.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://jnj.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mef.vehdjk.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zvq.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gsj.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://yix.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://cbq.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://ndz.0kj1m.cn

Ruby: // 手写 Hash
来源：http://qeb.smart0.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://zvd.bjfxy.top

[N08] 生成全排列
来源：http://zhc.dianchejie.cn

Py:   itertools.permutations(arr)
来源：http://qom.yongpay.top

PHP:  // 手写递归交换
来源：http://kos.hcnkem.com

JS:   // 手写回溯递归
来源：http://omc.daria6918.cn

TS:   // 手写回溯递归
来源：http://oxk.yj20258888.top

Java: // 手写回溯递归
来源：http://dza.zhongyouzk.top

Go:   // 手写回溯递归
来源：http://ygz.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://thr.yfazqb.com

C#:   // 手写回溯递归
来源：http://vkc.gotoacloud.top

[N09] 栈与队列
来源：http://dpp.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://grb.shuidangran.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xbc.redwolf501.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uid.ppjwa.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kff.wangshuangyany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ycl.c1oappe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zgx.yvedp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gji.yanxiufei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://png.kuanghao11.cn

[N10] 链表节点定义
来源：http://axp.bbcook.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bnp.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jat.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gsf.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pbi.vehdjk.com

Java: class Node { int v; Node next; }
来源：http://afr.zycfv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dbz.yuanzhike.top

Ruby: Node = Struct.new(:v, :next)
来源：http://kmm.xylfe.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://euh.guannengcc.top

[N11] 二叉树中序遍历
来源：http://mqh.cdnleiting.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ihd.sxryk.cn

PHP:  // 手写递归函数
来源：http://thp.redwolf501.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hly.nanxinkj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zqp.havefunace.top

Java: // 手写递归
来源：http://isq.yanxiufei.cn

Go:   // 手写递归
来源：http://gro.snrcjt.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ufj.xziqi.cn

C#:   // 手写递归
来源：http://tbb.daria6918.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ibt.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wfu.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dwh.hongshengwenyu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vux.316326.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jej.sysykeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wbb.fehbvm.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://efu.xylfe.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fol.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sqw.yanxiufei.cn

================================================================================
来源：http://fte.wangshuangyany.cn

O. 并发与异步
来源：http://dgb.meibo888.top

================================================================================
来源：http://net.gotoacloud.top

[O01] 启动一个线程
来源：http://qdr.zhiwuduotai.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iwa.jiagoushi.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yoz.tian-w.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mam.jinqigufen.top

TS:   // 同 JS
来源：http://nom.nwbrower.top

Java: new Thread(() -> f()).start()
来源：http://bhf.ctjpmb.com

Go:   go f()
来源：http://ivw.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://mtp.yvedp.cn

C#:   Task.Run(() => F());
来源：http://npo.xziqi.cn

[O02] 使用线程池
来源：http://wnq.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pzf.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rkp.andypj.xyz

JS:   // worker_threads 线程池
来源：http://nrn.vehdjk.com

TS:   // worker_threads 线程池
来源：http://ege.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://ppk.bjfxy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wsx.zhoulong.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hbm.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tav.316326.xyz

[O03] 加锁保护共享数据
来源：http://luq.ywan-chungtsiang.top

Py:   with lock: shared += 1
来源：http://nvd.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://ahx.meibo888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sdr.yj20258.top

TS:   // 同 JS
来源：http://lhq.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://set.shangyingyoupin.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cyw.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fol.xingfuxueyuan.xyz

C#:   lock (gate) { shared++; }
来源：http://zue.cdnleiting.top

[O04] 定义异步函数并等待
来源：http://uil.ivvv.top

Py:   async def f():⏎    await g()
来源：http://sqw.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lat.cheryme.top

JS:   async function f() { await g(); }
来源：http://qav.svipenyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cju.sufxvd.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mcl.fehbvm.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://son.vqdsnc.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xlz.daxiang520.top

C#:   async Task F() { await G(); }
来源：http://dwl.xuetiantiany.cn

[O05] 并发执行并等待全部完成
来源：http://cqz.jinyuanbaomall.cn

Py:   asyncio.gather(*tasks)
来源：http://bli.gotoacloud.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zxc.sufxvd.cn

JS:   await Promise.all(tasks)
来源：http://efl.pycfn.com

TS:   await Promise.all(tasks)
来源：http://jko.yanxiufei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tbv.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ixh.epnwcf.com

Ruby: threads.map(&:join)
来源：http://gfk.c1oappe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zdn.0kj1m.cn

[O06] 使用进程池
来源：http://jbn.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hkn.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uoj.yongpay.top

JS:   // child_process / cluster 模块
来源：http://hkq.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://awu.hesvh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ytn.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cyj.cheryme.top

Ruby: // fork 块
来源：http://bzo.yongpay.top

C#:   Parallel.For
来源：http://luq.sufxvd.cn

================================================================================
来源：http://vdp.xuanzx.com

P. 常用工具函数
来源：http://gsz.uphjek.com

================================================================================
来源：http://lml.jiagoushi.top

[P01] 生成 UUID
来源：http://qdy.sweek.top

Py:   str(uuid.uuid4())
来源：http://fkk.52xcode.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xte.hysaishi.cn

JS:   crypto.randomUUID()
来源：http://xvf.52xcode.cn

TS:   crypto.randomUUID()
来源：http://wlp.feifeiyinyue.top

Java: UUID.randomUUID().toString()
来源：http://jfj.feifeiyinyue.top

Go:   // 用 github.com/google/uuid
来源：http://bzz.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://fht.xziqi.cn

C#:   Guid.NewGuid().ToString()
来源：http://nbb.nanxinkj.top

[P02] MD5 / SHA256 摘要
来源：http://acz.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wzf.xylfe.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fcy.aibaodan.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xdo.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tgz.bbcook.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pqx.ydzc1.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iep.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mkk.hongshengwenyu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xnk.zhiwuduotai.top

[P03] 生成短随机字符串
来源：http://ymk.aizwys.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mro.nwbrower.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ndk.zdbjq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eqm.hongshengwenyu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cfl.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gne.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aco.hysaishi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gzw.zhengqikj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dya.ywan-chungtsiang.top

[P04] 求长度
来源：http://tij.ydzc1.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://npl.wangshuangyany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ucm.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zjk.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jcf.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://hdz.jiagoushi.top

Go:   len(arr);  len(m)
来源：http://zew.hfpthk.cn

Ruby: x.length;  x.size
来源：http://rts.hywenlv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ovv.bjfxy.top

[P05] 判断两个对象内容是否相等
来源：http://amy.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yyi.haohaochexian.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://woe.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tzz.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tyq.jianghu66.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://joy.zhixingplan.top

Go:   reflect.DeepEqual(a, b)
来源：http://crr.guannengcc.top

Ruby: a == b
来源：http://yds.bjfxy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sij.bjfxy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mfa.sjlbkw.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ibi.zhiwuduotai.top

PHP:  if (empty($x)) {}
来源：http://kwh.ctjpmb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aja.shuidangran.top

TS:   if (x == null) {}
来源：http://aip.xziqi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://byz.fktsv.cn

Go:   if x == nil {}
来源：http://yjs.yj202588.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://frt.havefunace.top

C#:   if (x is null) {}
来源：http://tyn.zhengqikj.top

[P07] 防抖与节流
来源：http://cra.zhixingplan.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tjj.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://lat.xuanzx.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://irk.guannengcc.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xzn.tianlin.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sgz.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rlr.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wze.yj20258.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qnn.tarul.cn

[P08] 处理浮点精度问题
来源：http://qsc.jinghuilouyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pal.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tei.meibo888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://izs.vqdsnc.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dkv.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://glz.xinyue.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mma.xuanzx.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gib.uphjek.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ayv.tanke756.top

================================================================================
来源：http://knc.fktsv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oes.shanyushiyangkeji.top

================================================================================
来源：http://bie.sjlbkw.cn

[Q01] 创建表
来源：http://wqn.fanxiaobao.xyz

CREATE TABLE users (
来源：http://klv.jianghu66.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://knx.mhx1999.top

name VARCHAR(50) NOT NULL,
来源：http://eqz.vehdjk.com

email VARCHAR(100) UNIQUE,
来源：http://awn.ybcxt.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kzj.gotoacloud.top

);
来源：http://edt.sufxvd.cn

[Q02] 创建带外键的表
来源：http://qik.daxiang520.top

CREATE TABLE orders (
来源：http://gaw.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://chl.yvedp.cn

user_id INT NOT NULL,
来源：http://fdk.dianchejie.cn

amount DECIMAL(10, 2),
来源：http://cfa.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gjy.ivvv.top

);
来源：http://nvx.jqgfzy.top

[Q03] 增加列
来源：http://jky.smart0.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tcs.xinyue.icu

[Q04] 修改列类型
来源：http://ren.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lip.fktsv.cn

[Q05] 重命名列
来源：http://fdu.sufxvd.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://arl.0kj1m.cn

[Q06] 删除列
来源：http://jlw.yj202588.top

ALTER TABLE users DROP COLUMN age;
来源：http://uii.chenjidiqi.icu

[Q07] 删除表
来源：http://sgf.chenzaomai.com

DROP TABLE IF EXISTS orders;
来源：http://nhw.hysaishi.cn

[Q08] 创建普通索引
来源：http://njj.fanxiaobao.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://hul.smart0.xyz

[Q09] 创建唯一索引
来源：http://ucz.jinqigufen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lds.mhx1999.top

[Q10] 插入单行
来源：http://ico.fengsongda.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qaw.aizwys.cn

[Q11] 一次插入多行
来源：http://sin.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ysx.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://nwo.havefunace.top

INSERT INTO users (name) VALUES ('C');
来源：http://omf.fengsongda.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sqz.xuanzx.com

[Q13] 忽略重复插入
来源：http://gyl.jyoumei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fil.chenlongwang.top

[Q14] 存在则更新（upsert）
来源：http://ntc.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mwh.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lpm.chenjidiqi.icu

[Q15] 查询全部
来源：http://vyr.yfazqb.com

SELECT * FROM users;
来源：http://kog.xuanzx.com

[Q16] 查询指定列
来源：http://szj.hnxiangtu.top

SELECT id, name FROM users;
来源：http://fhp.zdqjudy.top

[Q17] 条件查询
来源：http://izz.daria6918.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eba.shzxlz.cn

[Q18] 模糊匹配
来源：http://evi.fktsv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nla.jiagoushi.top

[Q19] 范围查询
来源：http://ych.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qbr.andypj.xyz

[Q20] IN 列表
来源：http://mwc.zhongyouzk.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wxs.ehwqpu.com

[Q21] 空值判断
来源：http://jrb.yfazqb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://vip.fanxiaobao.xyz

[Q22] 排序
来源：http://shl.redwolf501.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dvc.0kj1m.cn

[Q23] 分页
来源：http://gap.shanyushiyangtech.top


<!-- 参考信息 -->