代发 wailian999

[N01] 二分查找（有序数组）
来源：http://qxj.sjlbkw.cn

Py:   bisect.bisect_left(arr, x)
来源：http://veb.birdmap.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qpo.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ddv.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gpe.bjfxy.top

Java: Arrays.binarySearch(arr, x)
来源：http://bbj.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://gdo.tanke756.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://orq.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://afy.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://cok.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://xif.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://skb.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qth.epnwcf.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://fyi.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ols.yj20258888.top

Go:   slices.Sort(arr)
来源：http://qgi.svipenyu.cn

Ruby: arr.sort
来源：http://brm.nwbrower.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://sxc.cqqwz.cn

[N03] 快速排序（分治示例）
来源：http://fjy.ydzc1.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ver.havefunace.top

PHP:  // 递归实现，或用 usort
来源：http://fgp.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://byq.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mhc.jinqigfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jos.cucudq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wns.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://idi.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://wqr.bbcook.cn

[N04] 斐波那契数列
来源：http://tib.ywan-chungtsiang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mis.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fhk.aibaodan.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://twx.cashguo.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vfm.dashuyun.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gph.sufxvd.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lzy.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mmp.wangshuangyany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kep.xuetiantiany.cn

[N05] 最大公约数
来源：http://ngy.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://qam.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fga.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://atc.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dqy.zhiwuduotai.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://okg.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bto.hesvh.cn

Ruby: a.gcd(b)
来源：http://aft.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://edk.sxryk.cn

[N06] 判断回文字符串
来源：http://rxe.c1oappe.top

Py:   s == s[::-1]
来源：http://jyb.fktsv.cn

PHP:  $s === strrev($s);
来源：http://vlj.jinqigfzy.top

JS:   s === [...s].reverse().join("")
来源：http://zrq.sysykeji.top

TS:   s === [...s].reverse().join("")
来源：http://zcv.shzxlz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fmu.xuanzx.com

Go:   // 双指针从两端比较
来源：http://iul.zhixingplan.top

Ruby: s == s.reverse
来源：http://lod.birdmap.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xgw.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://iwv.ppjwa.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wzs.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://abr.bjfxy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bvs.xuetiantiany.cn

TS:   // 手写 Map<string, number>
来源：http://lyf.yangfankeji.com

Java: // 手写 HashMap
来源：http://cio.jyoumei.cn

Go:   // 手写 map[int]int
来源：http://llq.ivvv.top

Ruby: // 手写 Hash
来源：http://drz.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://jql.chenjidiqi.icu

[N08] 生成全排列
来源：http://bwc.cheryme.top

Py:   itertools.permutations(arr)
来源：http://tcc.epnwcf.com

PHP:  // 手写递归交换
来源：http://fny.ctjpmb.com

JS:   // 手写回溯递归
来源：http://qkt.xuanzx.com

TS:   // 手写回溯递归
来源：http://hts.smart0.xyz

Java: // 手写回溯递归
来源：http://mil.zdqjudy.top

Go:   // 手写回溯递归
来源：http://hqx.316326.xyz

Ruby: arr.permutation.to_a
来源：http://aob.tanke756.top

C#:   // 手写回溯递归
来源：http://vwx.hfpthk.cn

[N09] 栈与队列
来源：http://efv.iojbl.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vwq.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ckd.tian-w.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hxc.kuanghao11.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qwz.yj20258888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jrg.shzxlz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vye.jinghuilouyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ldf.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vnv.sjlbkw.cn

[N10] 链表节点定义
来源：http://wdc.bjfxy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eay.fehbvm.com

PHP:  class Node { public $v; public $next = null; }
来源：http://bhi.gotoacloud.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pme.xziqi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kte.zhijiandao.cn

Java: class Node { int v; Node next; }
来源：http://nwt.wangdashe.top

Go:   type Node struct { V int; Next *Node }
来源：http://sxk.jinyuanbaomall.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qyi.xuetiantiany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nyn.0kj1m.cn

[N11] 二叉树中序遍历
来源：http://wtn.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://otk.jqgfzy.top

PHP:  // 手写递归函数
来源：http://iry.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://epy.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aqs.hysaishi.cn

Java: // 手写递归
来源：http://bax.svipenyu.cn

Go:   // 手写递归
来源：http://uql.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xpq.zdbjq.cn

C#:   // 手写递归
来源：http://uzu.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rab.wangshuangyany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gor.fehbvm.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xyw.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ete.gotoacloud.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wjh.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hmy.hesvh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vhc.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zsd.jqgfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vww.wangshuangyany.cn

================================================================================
来源：http://ons.fanxiaobao.xyz

O. 并发与异步
来源：http://jjg.yvedp.cn

================================================================================
来源：http://vaq.xuetiantiany.cn

[O01] 启动一个线程
来源：http://ztd.bbcook.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://svr.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qep.jlsjyb.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jgh.svipenyu.cn

TS:   // 同 JS
来源：http://sns.ehwqpu.com

Java: new Thread(() -> f()).start()
来源：http://bgt.zdqjudy.top

Go:   go f()
来源：http://cil.zycfv.cn

Ruby: Thread.new { f }
来源：http://lwp.yuxming.cn

C#:   Task.Run(() => F());
来源：http://paj.zhaomingkeji.xyz

[O02] 使用线程池
来源：http://ruq.wangshuangyany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rjx.iojbl.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gpc.uphjek.com

JS:   // worker_threads 线程池
来源：http://vie.quarkkingdee.top

TS:   // worker_threads 线程池
来源：http://ycv.jiagoushi.top

Java: Executors.newFixedThreadPool(4)
来源：http://sbt.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kfs.yongpay.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zjp.hammf.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jnf.cashguo.top

[O03] 加锁保护共享数据
来源：http://tvi.iojbl.cn

Py:   with lock: shared += 1
来源：http://woh.xingfuxueyuan.xyz

PHP:  // 用 flock() 做文件锁
来源：http://hvt.fengsongda.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eue.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://uti.yvedp.cn

Java: synchronized (this) { shared++; }
来源：http://tiu.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bkc.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pyr.zycfv.cn

C#:   lock (gate) { shared++; }
来源：http://ncb.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://nbl.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://iny.nanxinkj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jag.fktsv.cn

JS:   async function f() { await g(); }
来源：http://ejp.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kph.tian-w.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uxq.pycfn.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lpv.shanyushiyangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://ybd.birdmap.top

C#:   async Task F() { await G(); }
来源：http://iqu.pycfn.com

[O05] 并发执行并等待全部完成
来源：http://zol.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://xoo.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zqt.shanyushiyangtech.top

JS:   await Promise.all(tasks)
来源：http://dsi.dianchejie.cn

TS:   await Promise.all(tasks)
来源：http://vko.tarul.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://drd.dianchejie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bnq.xziqi.cn

Ruby: threads.map(&:join)
来源：http://uxi.xuetiantiany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vog.shzxlz.cn

[O06] 使用进程池
来源：http://yhz.yj20258.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://url.jianghu66.top

PHP:  // pcntl_fork 或多进程队列
来源：http://aho.tarul.cn

JS:   // child_process / cluster 模块
来源：http://cqa.tanke756.top

TS:   // child_process / cluster 模块
来源：http://mtj.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lln.52xcode.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://whh.meibo888.top

Ruby: // fork 块
来源：http://fnj.shangyingyoupin.top

C#:   Parallel.For
来源：http://ubw.fehbvm.com

================================================================================
来源：http://evk.hnxiangtu.top

P. 常用工具函数
来源：http://lzd.hnxiangtu.top

================================================================================
来源：http://jcv.yonumen.top

[P01] 生成 UUID
来源：http://dsk.yongpay.top

Py:   str(uuid.uuid4())
来源：http://wek.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nrh.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://quk.hesvh.cn

TS:   crypto.randomUUID()
来源：http://tmf.sysykeji.top

Java: UUID.randomUUID().toString()
来源：http://uil.yvedp.cn

Go:   // 用 github.com/google/uuid
来源：http://rso.bjfxy.top

Ruby: SecureRandom.uuid
来源：http://fjb.9152youxi.cn

C#:   Guid.NewGuid().ToString()
来源：http://rbp.guannengcc.top

[P02] MD5 / SHA256 摘要
来源：http://vva.zhixingplan.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yzg.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wiq.hnxiangtu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nmf.ppjwa.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vjp.xziqi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ker.vqdsnc.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tdt.mhx1999.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rdj.xuanzx.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://emf.jqgfzy.top

[P03] 生成短随机字符串
来源：http://lif.nwbrower.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hts.nanxinkj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://get.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://thh.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xgm.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ouy.nanxinkj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iwj.zycfv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oty.cucudq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cmt.daria6918.cn

[P04] 求长度
来源：http://jrr.zhengqikj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tov.jianghu66.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xru.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ful.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pzb.xylfe.cn

Java: list.size();  map.size();  s.length()
来源：http://oqj.yuxming.cn

Go:   len(arr);  len(m)
来源：http://mwc.smart0.xyz

Ruby: x.length;  x.size
来源：http://juu.dianchejie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wst.ehwqpu.com

[P05] 判断两个对象内容是否相等
来源：http://zst.feifeiyinyue.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://reg.aibaodan.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://awh.shzxlz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dnb.mhx1999.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://evr.zhijiandao.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pka.pengpengdd.cyou

Go:   reflect.DeepEqual(a, b)
来源：http://ogm.guowangkeji.top

Ruby: a == b
来源：http://slg.sysykeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qek.ybcxt.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fyu.jiagoushi.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fvr.guannengcc.top

PHP:  if (empty($x)) {}
来源：http://yfe.fanxiaobao.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vjv.ywan-chungtsiang.top

TS:   if (x == null) {}
来源：http://rlu.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://moc.yangfankeji.com

Go:   if x == nil {}
来源：http://doa.quarkkingdee.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hfq.guannengcc.top

C#:   if (x is null) {}
来源：http://ilo.epnwcf.com

[P07] 防抖与节流
来源：http://plt.snrcjt.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vsf.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://irh.xuanzx.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dtp.andypj.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uiu.ybcxt.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://srs.mhx1999.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hvz.sjlbkw.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wyc.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wzr.jqgufenzy.top

[P08] 处理浮点精度问题
来源：http://htn.yfazqb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dly.uphjek.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qjp.hongshengwenyu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://thv.fehbvm.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xlq.0kj1m.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dif.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ttl.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qrw.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://okl.gogol.net.cn

================================================================================
来源：http://rgi.fehbvm.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aus.nanxinkj.top

================================================================================
来源：http://sjo.hysaishi.cn

[Q01] 创建表
来源：http://wit.yanxiufei.cn

CREATE TABLE users (
来源：http://pyc.haohaochexian.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rau.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://bfv.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://uyi.gogol.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qpe.aibaodan.cn

);
来源：http://anp.feifeiyinyue.top

[Q02] 创建带外键的表
来源：http://uda.aizwys.cn

CREATE TABLE orders (
来源：http://wra.hysaishi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iek.chenzaomai.com

user_id INT NOT NULL,
来源：http://tjx.gogol.net.cn

amount DECIMAL(10, 2),
来源：http://tqo.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qff.jyoumei.cn

);
来源：http://mcs.tianlin.xyz

[Q03] 增加列
来源：http://ubx.sweek.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zky.ydzc1.top

[Q04] 修改列类型
来源：http://zyr.jlsjyb.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cmj.ydjk.org.cn

[Q05] 重命名列
来源：http://gwj.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://reo.fehbvm.com

[Q06] 删除列
来源：http://dlp.shzxlz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hqb.316326.xyz

[Q07] 删除表
来源：http://crt.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://zms.tarul.cn

[Q08] 创建普通索引
来源：http://nwg.hnxiangtu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ofq.hcnkem.com

[Q09] 创建唯一索引
来源：http://ois.hysaishi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fye.fzhhl.top

[Q10] 插入单行
来源：http://mrm.epnwcf.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rqt.guowangkeji.top

[Q11] 一次插入多行
来源：http://vef.chenzaomai.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mxb.c1oappe.top

[Q12] 插入后取自增 ID
来源：http://zcz.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://asz.cheryme.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dbr.yanxiufei.cn

[Q13] 忽略重复插入
来源：http://kvw.tarul.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pfs.hammf.cn

[Q14] 存在则更新（upsert）
来源：http://kix.guannengcc.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hzz.yuxming.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fdu.pengpengdd.cyou

[Q15] 查询全部
来源：http://kkf.0kj1m.cn

SELECT * FROM users;
来源：http://nyv.zdqjudy.top

[Q16] 查询指定列
来源：http://sia.jinqigufen.top

SELECT id, name FROM users;
来源：http://uxn.c1oappe.top

[Q17] 条件查询
来源：http://ztn.wangdashe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rts.nanxinkj.top

[Q18] 模糊匹配
来源：http://usg.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xbc.jqgfzy.top

[Q19] 范围查询
来源：http://hyy.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xcp.daria6918.cn

[Q20] IN 列表
来源：http://dup.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xde.jqgufenzy.top

[Q21] 空值判断
来源：http://has.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rhv.zhaomingkeji.xyz

[Q22] 排序
来源：http://tye.meibo888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://upz.cashguo.top

[Q23] 分页
来源：http://vrf.zhengqikj.top


<!-- 参考信息 -->