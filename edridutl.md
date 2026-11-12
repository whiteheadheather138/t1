代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://fcs.sjlbkw.cn

================================================================================
来源：http://hdm.jqgfzy.top

N. 数据结构与算法
来源：http://fek.zhixingplan.top

================================================================================
来源：http://rkf.haohaochexian.top

[N01] 二分查找（有序数组）
来源：http://kkx.hcnkem.com

Py:   bisect.bisect_left(arr, x)
来源：http://dfn.shuidangran.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://juf.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xnp.zhiwuduotai.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vaq.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rjf.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://xok.nwbrower.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://uro.52xcode.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jue.chenzaomai.com

[N02] 排序（工程实践用内置实现）
来源：http://svh.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://nfa.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xug.hcnkem.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://zxf.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vdv.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ujx.fzhhl.top

Go:   slices.Sort(arr)
来源：http://brg.yj202588.top

Ruby: arr.sort
来源：http://poi.nanxuanxn.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hqm.birdmap.top

[N03] 快速排序（分治示例）
来源：http://cpv.hysaishi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dzn.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://eib.fktsv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zjr.zhixingplan.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ebg.jinqigufen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xen.dianchejie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bmr.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ypy.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://zrq.9152youxi.cn

[N04] 斐波那契数列
来源：http://iah.guannengcc.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ngq.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jon.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zii.wangshuangyany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gyg.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wtt.snrcjt.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://irs.fehbvm.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qyc.mhx1999.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://str.yvedp.cn

[N05] 最大公约数
来源：http://ltw.xinyue.icu

Py:   math.gcd(a, b)
来源：http://dgq.yanxiufei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gsb.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gpv.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uzl.jiagoushi.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ypp.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://agr.daria6918.cn

Ruby: a.gcd(b)
来源：http://vaf.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://azs.dianchejie.cn

[N06] 判断回文字符串
来源：http://kjw.sysykeji.top

Py:   s == s[::-1]
来源：http://nhk.jinyuanbaomall.cn

PHP:  $s === strrev($s);
来源：http://tuo.fanxiaobao.xyz

JS:   s === [...s].reverse().join("")
来源：http://wht.yj20258888.top

TS:   s === [...s].reverse().join("")
来源：http://fxy.hywenlv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yuo.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://foa.tian-w.cn

Ruby: s == s.reverse
来源：http://ytt.fehbvm.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://xbq.ywan-chungtsiang.top

[N07] 两数之和（返回下标）
来源：http://iju.jinqigufen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kzv.yuanzhike.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ogx.cashguo.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pdp.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://zoo.yvedp.cn

Java: // 手写 HashMap
来源：http://nls.yvedp.cn

Go:   // 手写 map[int]int
来源：http://dvh.jinqigfzy.top

Ruby: // 手写 Hash
来源：http://fxr.yanxiufei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qoa.shzxlz.cn

[N08] 生成全排列
来源：http://dhq.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://emm.cucudq.cn

PHP:  // 手写递归交换
来源：http://rvs.jiagoushi.top

JS:   // 手写回溯递归
来源：http://tcc.zycfv.cn

TS:   // 手写回溯递归
来源：http://jpj.fehbvm.com

Java: // 手写回溯递归
来源：http://qte.xingfuxueyuan.xyz

Go:   // 手写回溯递归
来源：http://fyl.chenlongwang.top

Ruby: arr.permutation.to_a
来源：http://bhh.fzhhl.top

C#:   // 手写回溯递归
来源：http://cyv.gaohongyu789.top

[N09] 栈与队列
来源：http://rxm.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zmj.nwbrower.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uks.zycfv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sfz.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tyf.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wog.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ucf.aizwys.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oul.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://exl.fktsv.cn

[N10] 链表节点定义
来源：http://xoz.ctjpmb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qeu.tarul.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ngo.zycfv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cey.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wjq.bbcook.cn

Java: class Node { int v; Node next; }
来源：http://dph.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://kkg.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hod.nanxinkj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uds.yvedp.cn

[N11] 二叉树中序遍历
来源：http://afk.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hzy.c1oappe.top

PHP:  // 手写递归函数
来源：http://phg.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cic.zhengqikj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bsx.sjlbkw.cn

Java: // 手写递归
来源：http://ird.jlsjyb.cn

Go:   // 手写递归
来源：http://veu.ywan-chungtsiang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ksk.chenlongwang.top

C#:   // 手写递归
来源：http://qrg.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hcs.haohaochexian.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zpn.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jyp.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bkj.yvedp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ggp.zhengqikj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jgn.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://upb.tarul.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://imo.fehbvm.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cey.hcnkem.com

================================================================================
来源：http://prf.iojbl.cn

O. 并发与异步
来源：http://lza.chenlongwang.top

================================================================================
来源：http://rvb.sxryk.cn

[O01] 启动一个线程
来源：http://oim.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pdx.hysaishi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uxw.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://deg.cashguo.top

TS:   // 同 JS
来源：http://fyb.sweek.top

Java: new Thread(() -> f()).start()
来源：http://bxz.tianlin.xyz

Go:   go f()
来源：http://krb.zhiwuduotai.top

Ruby: Thread.new { f }
来源：http://fka.fzhhl.top

C#:   Task.Run(() => F());
来源：http://xvh.316326.xyz

[O02] 使用线程池
来源：http://ntz.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ujs.yj202588.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hvk.gzhubu.top

JS:   // worker_threads 线程池
来源：http://fug.yj20258888.top

TS:   // worker_threads 线程池
来源：http://gpd.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pld.fengsongda.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mqh.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tip.yvedp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gws.jinqigfzy.top

[O03] 加锁保护共享数据
来源：http://zre.gogol.net.cn

Py:   with lock: shared += 1
来源：http://gyd.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://dhj.gzhubu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dmz.sweek.top

TS:   // 同 JS
来源：http://scp.hesvh.cn

Java: synchronized (this) { shared++; }
来源：http://ncl.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yck.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tpj.c1oappe.top

C#:   lock (gate) { shared++; }
来源：http://ibw.52xcode.cn

[O04] 定义异步函数并等待
来源：http://hqb.jyoumei.cn

Py:   async def f():⏎    await g()
来源：http://zzn.0kj1m.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://atn.jinyuanbaomall.cn

JS:   async function f() { await g(); }
来源：http://xpt.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cjc.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://knn.yanxiufei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nai.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pga.tarul.cn

C#:   async Task F() { await G(); }
来源：http://omp.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://fvu.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://wro.mhx1999.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kyh.andypj.xyz

JS:   await Promise.all(tasks)
来源：http://rzo.bjfxy.top

TS:   await Promise.all(tasks)
来源：http://dhd.cashguo.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sjb.ywan-chungtsiang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kpi.sjlbkw.cn

Ruby: threads.map(&:join)
来源：http://emn.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xts.c1oappe.top

[O06] 使用进程池
来源：http://xnn.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aak.ydjk.org.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://aak.feifeiyinyue.top

JS:   // child_process / cluster 模块
来源：http://frm.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://lhd.ctjpmb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://efx.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vlh.chenlongwang.top

Ruby: // fork 块
来源：http://fzo.jyoumei.cn

C#:   Parallel.For
来源：http://pkl.chenlongwang.top

================================================================================
来源：http://fmt.yuanzhike.top

P. 常用工具函数
来源：http://mns.cucudq.cn

================================================================================
来源：http://jml.kuanghao11.cn

[P01] 生成 UUID
来源：http://mjx.yj20258888.top

Py:   str(uuid.uuid4())
来源：http://dqp.iojbl.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ubb.jinghuilouyu.cn

JS:   crypto.randomUUID()
来源：http://yhb.gzhubu.top

TS:   crypto.randomUUID()
来源：http://xau.fengsongda.top

Java: UUID.randomUUID().toString()
来源：http://yeu.vehdjk.com

Go:   // 用 github.com/google/uuid
来源：http://gri.xingfuxueyuan.xyz

Ruby: SecureRandom.uuid
来源：http://jtq.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://ghf.andypj.xyz

[P02] MD5 / SHA256 摘要
来源：http://zwj.yfazqb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://acs.tanke756.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jez.feifeiyinyue.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pgm.snrcjt.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ugs.ydjk.org.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kxs.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fng.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zvb.jyoumei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fxb.wangdashe.top

[P03] 生成短随机字符串
来源：http://wec.yvedp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qbx.gzhubu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yaz.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nct.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dcm.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ujb.dashuyun.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lrq.yj20258.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ubu.ctjpmb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ihq.guannengcc.top

[P04] 求长度
来源：http://qjv.ydzc1.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hvk.tanke756.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rea.gogol.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kfs.jiagoushi.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hld.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://psb.guowangkeji.top

Go:   len(arr);  len(m)
来源：http://mna.yuanzhike.top

Ruby: x.length;  x.size
来源：http://rgx.zhongyouzk.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://atv.nanxuanxn.top

[P05] 判断两个对象内容是否相等
来源：http://xvy.xinyue.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://lnn.yuanzhike.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kkq.xziqi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yoa.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kga.xuanzx.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://igp.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kyx.ppjwa.cn

Ruby: a == b
来源：http://usc.hesvh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dik.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ajv.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pxq.kuanghao11.cn

PHP:  if (empty($x)) {}
来源：http://hnq.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://swk.cucudq.cn

TS:   if (x == null) {}
来源：http://jiv.shzxlz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sbg.epnwcf.com

Go:   if x == nil {}
来源：http://zrv.yuxming.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://faf.xuanzx.com

C#:   if (x is null) {}
来源：http://rkw.pycfn.com

[P07] 防抖与节流
来源：http://hmq.wangshuangyany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://woz.sweek.top

PHP:  // 手写时间戳比较
来源：http://zgo.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dsv.tarul.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://odg.zhiwuduotai.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bjf.quarkkingdee.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fzk.gogol.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lzo.tianlin.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vua.nwbrower.top

[P08] 处理浮点精度问题
来源：http://war.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iki.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fah.sjlbkw.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qxd.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ahc.guannengcc.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mkz.dashuyun.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://arv.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mbe.pycfn.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aqz.cqqwz.cn

================================================================================
来源：http://mpo.daria6918.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bac.sysykeji.top

================================================================================
来源：http://frz.dashuyun.cn

[Q01] 创建表
来源：http://hkq.fanxiaobao.xyz

CREATE TABLE users (
来源：http://lbo.sxryk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mhl.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://ncu.shzxlz.cn

email VARCHAR(100) UNIQUE,
来源：http://urc.xingfuxueyuan.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mfy.zhiwuduotai.top

);
来源：http://etk.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://htr.xuanzx.com

CREATE TABLE orders (
来源：http://iji.vqdsnc.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ynp.vehdjk.com

user_id INT NOT NULL,
来源：http://odb.ctjpmb.com

amount DECIMAL(10, 2),
来源：http://iyx.nanxinkj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nbw.gaohongyu789.top

);
来源：http://rtk.jinghuilouyu.cn

[Q03] 增加列
来源：http://rjr.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kvm.guowangkeji.top

[Q04] 修改列类型
来源：http://snw.nwbrower.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://foz.shanyushiyangtech.top

[Q05] 重命名列
来源：http://ezm.ywan-chungtsiang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lnr.tianlin.xyz

[Q06] 删除列
来源：http://tst.havefunace.top

ALTER TABLE users DROP COLUMN age;
来源：http://gkh.yuxming.cn

[Q07] 删除表
来源：http://fgo.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://rgh.vehdjk.com

[Q08] 创建普通索引
来源：http://xva.mhx1999.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fxf.shanyushiyangkeji.top

[Q09] 创建唯一索引
来源：http://rww.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://chi.guowangkeji.top

[Q10] 插入单行
来源：http://moq.fzhhl.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kxc.zdqjudy.top

[Q11] 一次插入多行
来源：http://yng.sweek.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bto.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://hgg.316326.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://sdi.redwolf501.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kkz.xuanzx.com

[Q13] 忽略重复插入
来源：http://dzz.havefunace.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nwx.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://dmj.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wfd.svipenyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dvj.cdnleiting.top

[Q15] 查询全部
来源：http://pty.nanxuanxn.top

SELECT * FROM users;
来源：http://ptn.yj20258888.top

[Q16] 查询指定列
来源：http://ijf.sxryk.cn

SELECT id, name FROM users;
来源：http://ten.chenlongwang.top

[Q17] 条件查询
来源：http://mdd.sufxvd.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bpx.bjfxy.top

[Q18] 模糊匹配
来源：http://rhp.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xji.zdqjudy.top

[Q19] 范围查询
来源：http://jpl.yj20258888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uow.daxiang520.top

[Q20] IN 列表
来源：http://kbg.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pze.shzxlz.cn

[Q21] 空值判断
来源：http://qyg.cashguo.top


<!-- 参考信息 -->