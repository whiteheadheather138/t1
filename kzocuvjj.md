代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://pgh.yongpay.top

================================================================================
来源：http://ian.xinyue.icu

N. 数据结构与算法
来源：http://uhz.svipenyu.cn

================================================================================
来源：http://txa.andypj.xyz

[N01] 二分查找（有序数组）
来源：http://vmk.redwolf501.top

Py:   bisect.bisect_left(arr, x)
来源：http://fqo.wangdashe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tbm.pengpengdd.cyou

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wek.zhiwuduotai.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vhr.tianlin.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://yuh.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://ifz.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://mcr.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://lib.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://wqg.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ahc.epnwcf.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lft.dashuyun.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ssk.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xkf.epnwcf.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mxz.cheryme.top

Go:   slices.Sort(arr)
来源：http://zvv.shuidangran.top

Ruby: arr.sort
来源：http://xin.cqqwz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ojd.svipenyu.cn

[N03] 快速排序（分治示例）
来源：http://mue.smart0.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wgb.cashguo.top

PHP:  // 递归实现，或用 usort
来源：http://zbx.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ngq.xylfe.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vwy.dianchejie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jgj.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wnp.guowangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vkd.redwolf501.top

C#:   // 手写递归，或 Array.Sort
来源：http://pfg.yanxiufei.cn

[N04] 斐波那契数列
来源：http://nuz.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gmm.tianlin.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mdj.nanxinkj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://het.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://myf.yfazqb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://stq.sysykeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://frg.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mug.xuetiantiany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zbw.yj20258888.top

[N05] 最大公约数
来源：http://pqo.hcnkem.com

Py:   math.gcd(a, b)
来源：http://fmj.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wuj.yueranfly.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mwb.dashuyun.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lkn.chenjidiqi.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vyi.guannengcc.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ofx.pengpengdd.cyou

Ruby: a.gcd(b)
来源：http://jzy.wangdashe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bra.zhixingplan.top

[N06] 判断回文字符串
来源：http://obt.smart0.xyz

Py:   s == s[::-1]
来源：http://bko.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://mca.pengpengdd.cyou

JS:   s === [...s].reverse().join("")
来源：http://sty.chenzaomai.com

TS:   s === [...s].reverse().join("")
来源：http://nrv.epnwcf.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hhn.9152youxi.cn

Go:   // 双指针从两端比较
来源：http://qes.fengsongda.top

Ruby: s == s.reverse
来源：http://gwi.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ofr.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://dnp.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gxn.gogol.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rfa.guowangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fnr.yangfankeji.com

TS:   // 手写 Map<string, number>
来源：http://nnv.vqdsnc.cn

Java: // 手写 HashMap
来源：http://kwg.tarul.cn

Go:   // 手写 map[int]int
来源：http://pug.dashuyun.cn

Ruby: // 手写 Hash
来源：http://bvt.jinqigufen.top

C#:   // 手写 Dictionary<int, int>
来源：http://pkf.xinyue.icu

[N08] 生成全排列
来源：http://poa.cdnleiting.top

Py:   itertools.permutations(arr)
来源：http://xce.dianchejie.cn

PHP:  // 手写递归交换
来源：http://nnt.cdnleiting.top

JS:   // 手写回溯递归
来源：http://kwb.yuanzhike.top

TS:   // 手写回溯递归
来源：http://mef.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://uhv.daria6918.cn

Go:   // 手写回溯递归
来源：http://ljs.hongshengwenyu.top

Ruby: arr.permutation.to_a
来源：http://phn.shuidangran.top

C#:   // 手写回溯递归
来源：http://ucw.zdqjudy.top

[N09] 栈与队列
来源：http://sbt.jinqigfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rvy.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nom.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iwy.zhiwuduotai.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://alj.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wfm.nwbrower.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://soa.nanxinkj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cmh.fehbvm.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bmm.vqdsnc.cn

[N10] 链表节点定义
来源：http://niw.meibo888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yfw.jinqigufen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fjw.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://atz.epnwcf.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pxc.birdmap.top

Java: class Node { int v; Node next; }
来源：http://rif.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://prw.guowangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gji.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://req.hcnkem.com

[N11] 二叉树中序遍历
来源：http://qzu.zhongyouzk.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vha.fzhhl.top

PHP:  // 手写递归函数
来源：http://wxc.meibo888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mlc.daria6918.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ivt.chenjidiqi.icu

Java: // 手写递归
来源：http://ajr.hongshengwenyu.top

Go:   // 手写递归
来源：http://vzj.ywan-chungtsiang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xgt.hysaishi.cn

C#:   // 手写递归
来源：http://nkc.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fef.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ldt.jiagoushi.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nrv.smart0.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gpd.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lzb.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kpa.uphjek.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ukj.ppjwa.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kno.tian-w.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tli.hesvh.cn

================================================================================
来源：http://pov.yuxming.cn

O. 并发与异步
来源：http://rpl.gogol.net.cn

================================================================================
来源：http://dcz.zhoulong.xyz

[O01] 启动一个线程
来源：http://zel.tarul.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ifs.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kke.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://swx.jinqigfzy.top

TS:   // 同 JS
来源：http://znt.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://eny.hfpthk.cn

Go:   go f()
来源：http://eee.yanxiufei.cn

Ruby: Thread.new { f }
来源：http://izn.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://wmy.andypj.xyz

[O02] 使用线程池
来源：http://ugp.xinyue.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ptp.xziqi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ywk.cashguo.top

JS:   // worker_threads 线程池
来源：http://jhk.jinqigufen.top

TS:   // worker_threads 线程池
来源：http://yrf.tanke756.top

Java: Executors.newFixedThreadPool(4)
来源：http://cyn.jyoumei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zvl.ivvv.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ria.hesvh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yur.fktsv.cn

[O03] 加锁保护共享数据
来源：http://skb.0kj1m.cn

Py:   with lock: shared += 1
来源：http://iqk.epnwcf.com

PHP:  // 用 flock() 做文件锁
来源：http://bqm.cucudq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rvo.c1oappe.top

TS:   // 同 JS
来源：http://snm.cqqwz.cn

Java: synchronized (this) { shared++; }
来源：http://jdj.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qtm.52xcode.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cuu.ydjk.org.cn

C#:   lock (gate) { shared++; }
来源：http://vtn.tanke756.top

[O04] 定义异步函数并等待
来源：http://sky.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://pko.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ycn.haohaochexian.top

JS:   async function f() { await g(); }
来源：http://htv.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ltb.zycfv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bno.jinyuanbaomall.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tpb.cqqwz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rbc.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://qor.gaohongyu789.top

[O05] 并发执行并等待全部完成
来源：http://mxr.yfazqb.com

Py:   asyncio.gather(*tasks)
来源：http://nay.daria6918.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zej.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://pdw.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://qfn.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tzs.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zvt.xylfe.cn

Ruby: threads.map(&:join)
来源：http://xpm.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vry.jinqigfzy.top

[O06] 使用进程池
来源：http://doi.xuetiantiany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gnf.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dca.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://ogi.jiagoushi.top

TS:   // child_process / cluster 模块
来源：http://tru.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mwt.ybcxt.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nip.yj202588.top

Ruby: // fork 块
来源：http://ryx.zhongyouzk.top

C#:   Parallel.For
来源：http://cye.xinyue.icu

================================================================================
来源：http://six.yonumen.top

P. 常用工具函数
来源：http://udj.jianghu66.top

================================================================================
来源：http://lzp.sxryk.cn

[P01] 生成 UUID
来源：http://uty.jianghu66.top

Py:   str(uuid.uuid4())
来源：http://qyz.feifeiyinyue.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dfg.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://dwq.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://fym.sysykeji.top

Java: UUID.randomUUID().toString()
来源：http://eqc.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://ege.gotoacloud.top

Ruby: SecureRandom.uuid
来源：http://ubu.zhoulong.xyz

C#:   Guid.NewGuid().ToString()
来源：http://isz.9152youxi.cn

[P02] MD5 / SHA256 摘要
来源：http://szy.52xcode.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lhu.aizwys.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wgn.gzhubu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://krx.yj20258.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vti.zhengqikj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ccs.zhoulong.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gsc.fehbvm.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rzg.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vha.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://nqy.snrcjt.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://olt.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mfp.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hbv.chenlongwang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://chr.sysykeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://esj.redwolf501.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ctr.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ihk.cqqwz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ppl.jyoumei.cn

[P04] 求长度
来源：http://bxb.pycfn.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://irm.aibaodan.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zif.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kut.daria6918.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pwo.sjlbkw.cn

Java: list.size();  map.size();  s.length()
来源：http://sbp.yonumen.top

Go:   len(arr);  len(m)
来源：http://sac.pycfn.com

Ruby: x.length;  x.size
来源：http://opd.yanxiufei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gqo.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://mnw.shanyushiyangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pvy.fengsongda.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dcj.yanxiufei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oir.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://erv.zhijiandao.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cpl.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://bzf.fengsongda.top

Ruby: a == b
来源：http://wlu.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fjx.tianlin.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dlh.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qdm.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://wvt.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ttj.gaohongyu789.top

TS:   if (x == null) {}
来源：http://nrn.snrcjt.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mia.hywenlv.cn

Go:   if x == nil {}
来源：http://paf.shangyingyoupin.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://osf.shuidangran.top

C#:   if (x is null) {}
来源：http://zpu.havefunace.top

[P07] 防抖与节流
来源：http://kkd.dashuyun.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iex.yangfankeji.com

PHP:  // 手写时间戳比较
来源：http://xqf.zhixingplan.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uqw.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aax.yuanzhike.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uor.sufxvd.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ido.hnxiangtu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rtu.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://imd.fzhhl.top

[P08] 处理浮点精度问题
来源：http://jgd.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bhg.ydjk.org.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://esv.ehwqpu.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nfs.hongshengwenyu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kij.uphjek.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kaz.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://osd.yj202588.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hdb.daria6918.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zyi.xylfe.cn

================================================================================
来源：http://fdk.birdmap.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fxr.xinyue.icu

================================================================================
来源：http://nuv.hesvh.cn

[Q01] 创建表
来源：http://ugs.hysaishi.cn

CREATE TABLE users (
来源：http://rbc.andypj.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hvn.sysykeji.top

name VARCHAR(50) NOT NULL,
来源：http://xba.vehdjk.com

email VARCHAR(100) UNIQUE,
来源：http://dxh.birdmap.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fxc.hysaishi.cn

);
来源：http://ein.yj20258888.top

[Q02] 创建带外键的表
来源：http://aub.yongpay.top

CREATE TABLE orders (
来源：http://bqh.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bwv.fanxiaobao.xyz

user_id INT NOT NULL,
来源：http://bfo.snrcjt.cn

amount DECIMAL(10, 2),
来源：http://dps.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://llp.quarkkingdee.top

);
来源：http://ltq.ydzc1.top

[Q03] 增加列
来源：http://ryy.daxiang520.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bcp.hcnkem.com

[Q04] 修改列类型
来源：http://qhx.ehwqpu.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mtb.bbcook.cn

[Q05] 重命名列
来源：http://ncc.tarul.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wxm.fktsv.cn

[Q06] 删除列
来源：http://doh.chenzaomai.com

ALTER TABLE users DROP COLUMN age;
来源：http://ahl.fengsongda.top

[Q07] 删除表
来源：http://jig.yangfankeji.com

DROP TABLE IF EXISTS orders;
来源：http://ccl.nanxuanxn.top

[Q08] 创建普通索引
来源：http://oyd.c1oappe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sgy.zhijiandao.cn

[Q09] 创建唯一索引
来源：http://gsr.yuanzhike.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://khx.gotoacloud.top

[Q10] 插入单行
来源：http://jko.jiagoushi.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://htg.nanxuanxn.top

[Q11] 一次插入多行
来源：http://qht.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qru.aizwys.cn

[Q12] 插入后取自增 ID
来源：http://uut.aibaodan.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eac.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uje.sysykeji.top

[Q13] 忽略重复插入
来源：http://asv.hammf.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://quh.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://emx.xuetiantiany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://meu.yuxming.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://odx.zhongyouzk.top

[Q15] 查询全部
来源：http://csa.hammf.cn

SELECT * FROM users;
来源：http://iyq.sxryk.cn

[Q16] 查询指定列
来源：http://qkz.zhixingplan.top

SELECT id, name FROM users;
来源：http://erw.316326.xyz

[Q17] 条件查询
来源：http://rkf.sysykeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kqr.52xcode.cn

[Q18] 模糊匹配
来源：http://ymq.pengpengdd.cyou

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pzn.9152youxi.cn

[Q19] 范围查询
来源：http://ldn.hcnkem.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vne.kuanghao11.cn

[Q20] IN 列表
来源：http://ytt.hcnkem.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lrf.guowangkeji.top

[Q21] 空值判断
来源：http://kvm.sweek.top


<!-- 参考信息 -->