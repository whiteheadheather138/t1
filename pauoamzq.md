代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://vfs.aizwys.cn

================================================================================
来源：http://jwm.jinghuilouyu.cn

N. 数据结构与算法
来源：http://ztc.feifeiyinyue.top

================================================================================
来源：http://spj.fengsongda.top

[N01] 二分查找（有序数组）
来源：http://zsb.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oeg.shuidangran.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hhi.tanke756.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yci.cashguo.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ipw.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ddd.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://zyn.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://qvp.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://xjk.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://xzt.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://fhl.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hos.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rol.yuxming.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://reu.nanxuanxn.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://klc.pycfn.com

Go:   slices.Sort(arr)
来源：http://hxm.yuanzhike.top

Ruby: arr.sort
来源：http://cbr.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zhr.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://ohi.316326.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eqm.bbcook.cn

PHP:  // 递归实现，或用 usort
来源：http://ymv.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ofa.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eza.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oci.shanyushiyangtech.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hkc.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ieg.sufxvd.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vst.cashguo.top

[N04] 斐波那契数列
来源：http://wvg.jinghuilouyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pvf.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zwh.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pvz.cheryme.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cxy.zdbjq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gqh.gotoacloud.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://whz.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lfx.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jov.gogol.net.cn

[N05] 最大公约数
来源：http://xth.nanxinkj.top

Py:   math.gcd(a, b)
来源：http://xcz.zdqjudy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sdj.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ytq.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tcz.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yie.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hvx.nanxuanxn.top

Ruby: a.gcd(b)
来源：http://uce.kuanghao11.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eiw.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://epo.hysaishi.cn

Py:   s == s[::-1]
来源：http://ese.gaohongyu789.top

PHP:  $s === strrev($s);
来源：http://xcq.shzxlz.cn

JS:   s === [...s].reverse().join("")
来源：http://jyr.andypj.xyz

TS:   s === [...s].reverse().join("")
来源：http://gqh.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wmz.xziqi.cn

Go:   // 双指针从两端比较
来源：http://gna.mhx1999.top

Ruby: s == s.reverse
来源：http://ajc.cheryme.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pfh.hnxiangtu.top

[N07] 两数之和（返回下标）
来源：http://fuk.hywenlv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hjz.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hnt.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qnp.cdnleiting.top

TS:   // 手写 Map<string, number>
来源：http://rwy.kuanghao11.cn

Java: // 手写 HashMap
来源：http://qju.epnwcf.com

Go:   // 手写 map[int]int
来源：http://oko.hesvh.cn

Ruby: // 手写 Hash
来源：http://piv.zhijiandao.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ftu.cheryme.top

[N08] 生成全排列
来源：http://lmi.bbcook.cn

Py:   itertools.permutations(arr)
来源：http://xvk.meibo888.top

PHP:  // 手写递归交换
来源：http://lme.jlsjyb.cn

JS:   // 手写回溯递归
来源：http://yij.jqgfzy.top

TS:   // 手写回溯递归
来源：http://zbg.c1oappe.top

Java: // 手写回溯递归
来源：http://jsc.hnqzz.top

Go:   // 手写回溯递归
来源：http://ero.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://kzq.fzhhl.top

C#:   // 手写回溯递归
来源：http://wyo.sxryk.cn

[N09] 栈与队列
来源：http://yys.shuidangran.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jde.cashguo.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cww.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://amz.yuanzhike.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cct.ppjwa.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ubu.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://spt.jinqigufen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://awc.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mev.yuanzhike.top

[N10] 链表节点定义
来源：http://fow.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iwd.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dei.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hnv.hongshengwenyu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qma.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://ytv.zhixingplan.top

Go:   type Node struct { V int; Next *Node }
来源：http://ujo.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dsk.chenlongwang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wzc.ydjk.org.cn

[N11] 二叉树中序遍历
来源：http://jyn.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nmy.cashguo.top

PHP:  // 手写递归函数
来源：http://aax.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dkm.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jka.zhaomingkeji.xyz

Java: // 手写递归
来源：http://iui.tian-w.cn

Go:   // 手写递归
来源：http://yyy.vehdjk.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qdb.shzxlz.cn

C#:   // 手写递归
来源：http://jtq.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://les.cheryme.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://szk.guowangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rnr.snrcjt.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tai.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mct.yanxiufei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tlu.hesvh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lvf.cheryme.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wla.cashguo.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fqm.gaohongyu789.top

================================================================================
来源：http://eds.daxiang520.top

O. 并发与异步
来源：http://lpj.zhijiandao.cn

================================================================================
来源：http://gwy.yonumen.top

[O01] 启动一个线程
来源：http://brv.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lsc.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lkx.kuanghao11.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://szd.ehwqpu.com

TS:   // 同 JS
来源：http://ihj.shangyingyoupin.top

Java: new Thread(() -> f()).start()
来源：http://goj.iojbl.cn

Go:   go f()
来源：http://ode.fktsv.cn

Ruby: Thread.new { f }
来源：http://tlw.kuanghao11.cn

C#:   Task.Run(() => F());
来源：http://ymj.uphjek.com

[O02] 使用线程池
来源：http://qgn.chenjidiqi.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://evo.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uhl.fzhhl.top

JS:   // worker_threads 线程池
来源：http://ytk.pengpengdd.cyou

TS:   // worker_threads 线程池
来源：http://nzy.xingfuxueyuan.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://iof.shanyushiyangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zve.vqdsnc.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lhe.sufxvd.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ppi.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://dxk.chenlongwang.top

Py:   with lock: shared += 1
来源：http://bjv.xylfe.cn

PHP:  // 用 flock() 做文件锁
来源：http://uhi.0kj1m.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xfc.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://xuz.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://amg.jinghuilouyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vdk.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hpy.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://hbd.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://lxp.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://ady.wangshuangyany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vwf.cashguo.top

JS:   async function f() { await g(); }
来源：http://cfy.tianlin.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://wqj.tarul.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nsd.andypj.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ggx.feifeiyinyue.top

Ruby: # 用 Fiber 或 async gem
来源：http://ohu.0kj1m.cn

C#:   async Task F() { await G(); }
来源：http://fkh.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://cvd.hongshengwenyu.top

Py:   asyncio.gather(*tasks)
来源：http://lgy.jiagoushi.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oqi.jinqigfzy.top

JS:   await Promise.all(tasks)
来源：http://xgr.iojbl.cn

TS:   await Promise.all(tasks)
来源：http://obo.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zpy.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tir.guannengcc.top

Ruby: threads.map(&:join)
来源：http://wfh.ctjpmb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://cjd.jiagoushi.top

[O06] 使用进程池
来源：http://utu.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vsx.jqgfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://htl.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://jto.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://qkw.ppjwa.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cei.ctjpmb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oit.yfazqb.com

Ruby: // fork 块
来源：http://cap.yj20258.top

C#:   Parallel.For
来源：http://jtp.smart0.xyz

================================================================================
来源：http://oun.nanxuanxn.top

P. 常用工具函数
来源：http://aiy.ivvv.top

================================================================================
来源：http://hye.hfpthk.cn

[P01] 生成 UUID
来源：http://sjf.ctjpmb.com

Py:   str(uuid.uuid4())
来源：http://nxx.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xdt.birdmap.top

JS:   crypto.randomUUID()
来源：http://zyh.hammf.cn

TS:   crypto.randomUUID()
来源：http://zso.sjlbkw.cn

Java: UUID.randomUUID().toString()
来源：http://cpp.52xcode.cn

Go:   // 用 github.com/google/uuid
来源：http://uyh.aizwys.cn

Ruby: SecureRandom.uuid
来源：http://neo.xylfe.cn

C#:   Guid.NewGuid().ToString()
来源：http://uew.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://dlh.tarul.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ngs.birdmap.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ixl.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pig.yj20258.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zmo.yj20258.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bjz.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://deq.aizwys.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jeg.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dwh.yuanzhike.top

[P03] 生成短随机字符串
来源：http://rpc.hnqzz.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dht.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uct.vehdjk.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hhp.redwolf501.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iky.pycfn.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ubc.cdnleiting.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://flw.shzxlz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fgv.chenjidiqi.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tta.epnwcf.com

[P04] 求长度
来源：http://hlu.quarkkingdee.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://otg.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xji.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://klm.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://khy.haohaochexian.top

Java: list.size();  map.size();  s.length()
来源：http://bkw.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://jxa.shangyingyoupin.top

Ruby: x.length;  x.size
来源：http://kdn.tarul.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://luw.sufxvd.cn

[P05] 判断两个对象内容是否相等
来源：http://hjw.yj20258888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://swb.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://etc.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wow.gotoacloud.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kyu.sxryk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hun.chenlongwang.top

Go:   reflect.DeepEqual(a, b)
来源：http://ods.zdqjudy.top

Ruby: a == b
来源：http://mot.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cvx.yongpay.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://azy.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mrt.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://dks.nwbrower.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dax.jinqigufen.top

TS:   if (x == null) {}
来源：http://uau.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cnk.nanxuanxn.top

Go:   if x == nil {}
来源：http://kpm.xinyue.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xpz.52xcode.cn

C#:   if (x is null) {}
来源：http://gbl.vqdsnc.cn

[P07] 防抖与节流
来源：http://kng.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xmr.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://mnq.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cmi.yonumen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pkx.nwbrower.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dtz.shanyushiyangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nkg.hongshengwenyu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jqi.quarkkingdee.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ktu.hammf.cn

[P08] 处理浮点精度问题
来源：http://gbw.bjfxy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://skz.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gpt.jlsjyb.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fcv.xinyue.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mop.daria6918.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hwy.gzhubu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vds.redwolf501.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rpw.sjlbkw.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nqa.aizwys.cn

================================================================================
来源：http://nkp.xingfuxueyuan.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rby.sxryk.cn

================================================================================
来源：http://yeq.hnqzz.top

[Q01] 创建表
来源：http://otz.meibo888.top

CREATE TABLE users (
来源：http://lwz.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ztn.bjfxy.top

name VARCHAR(50) NOT NULL,
来源：http://ctb.c1oappe.top

email VARCHAR(100) UNIQUE,
来源：http://ngf.ydjk.org.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pqk.hfpthk.cn

);
来源：http://ygp.yj20258.top

[Q02] 创建带外键的表
来源：http://kqh.fengsongda.top

CREATE TABLE orders (
来源：http://dwx.ppjwa.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kll.andypj.xyz

user_id INT NOT NULL,
来源：http://cyi.jyoumei.cn

amount DECIMAL(10, 2),
来源：http://tzg.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xvk.hcnkem.com

);
来源：http://eoj.fehbvm.com

[Q03] 增加列
来源：http://bos.yonumen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kle.xziqi.cn

[Q04] 修改列类型
来源：http://fze.quarkkingdee.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ckb.snrcjt.cn

[Q05] 重命名列
来源：http://ixc.hywenlv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tpw.yj202588.top

[Q06] 删除列
来源：http://cfe.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://caa.gotoacloud.top

[Q07] 删除表
来源：http://cbr.gotoacloud.top

DROP TABLE IF EXISTS orders;
来源：http://dgq.gaohongyu789.top

[Q08] 创建普通索引
来源：http://ndl.aizwys.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hyg.sxryk.cn

[Q09] 创建唯一索引
来源：http://utf.tarul.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bqh.bjfxy.top

[Q10] 插入单行
来源：http://sjt.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yxy.tanke756.top

[Q11] 一次插入多行
来源：http://ihp.chenlongwang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jue.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://lkl.ydzc1.top

INSERT INTO users (name) VALUES ('C');
来源：http://ozp.0kj1m.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://amy.zhengqikj.top

[Q13] 忽略重复插入
来源：http://boo.jlsjyb.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uvh.gzhubu.top

[Q14] 存在则更新（upsert）
来源：http://ajg.52xcode.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eln.fzhhl.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rzv.cqqwz.cn

[Q15] 查询全部
来源：http://lkx.ppjwa.cn

SELECT * FROM users;
来源：http://ysl.cheryme.top

[Q16] 查询指定列
来源：http://lyl.zhoulong.xyz

SELECT id, name FROM users;
来源：http://bps.hysaishi.cn

[Q17] 条件查询
来源：http://hlx.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://edu.andypj.xyz

[Q18] 模糊匹配
来源：http://znl.cdnleiting.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://scc.xuanzx.com

[Q19] 范围查询
来源：http://iyv.fehbvm.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://whu.zhijiandao.cn

[Q20] IN 列表
来源：http://iam.hnxiangtu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jya.cashguo.top

[Q21] 空值判断
来源：http://qrl.jlsjyb.cn


<!-- 参考信息 -->