代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://szc.yuxming.cn

================================================================================
来源：http://huy.yonumen.top

N. 数据结构与算法
来源：http://pqw.bjfxy.top

================================================================================
来源：http://joz.pycfn.com

[N01] 二分查找（有序数组）
来源：http://qvb.jinqigufen.top

Py:   bisect.bisect_left(arr, x)
来源：http://vei.uphjek.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pam.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://czy.jianghu66.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kcl.zhixingplan.top

Java: Arrays.binarySearch(arr, x)
来源：http://ogl.andypj.xyz

Go:   sort.SearchInts(arr, x)
来源：http://anc.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fwi.cucudq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ufk.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://vpn.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://nda.pycfn.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://njt.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oam.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ksg.xuanzx.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://crx.guannengcc.top

Go:   slices.Sort(arr)
来源：http://ikj.sjlbkw.cn

Ruby: arr.sort
来源：http://yzy.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vvl.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://xfk.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nil.fengsongda.top

PHP:  // 递归实现，或用 usort
来源：http://lmb.cashguo.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pky.dianchejie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cwq.sxryk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bhl.shzxlz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qvd.gotoacloud.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hjg.sufxvd.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kdz.xinyue.icu

[N04] 斐波那契数列
来源：http://osl.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://coa.cheryme.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tlz.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fxb.yangfankeji.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://grc.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wyk.ivvv.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ffv.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lhi.yuanzhike.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zph.316326.xyz

[N05] 最大公约数
来源：http://qcm.iojbl.cn

Py:   math.gcd(a, b)
来源：http://sco.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fky.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://etx.yvedp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jyw.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jbc.chenzaomai.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://trf.tanke756.top

Ruby: a.gcd(b)
来源：http://cgp.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vyn.ydjk.org.cn

[N06] 判断回文字符串
来源：http://yel.vqdsnc.cn

Py:   s == s[::-1]
来源：http://dcn.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://woq.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://jsl.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://lej.iojbl.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bvf.guowangkeji.top

Go:   // 双指针从两端比较
来源：http://wmo.sysykeji.top

Ruby: s == s.reverse
来源：http://voq.haohaochexian.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fko.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://isu.sufxvd.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jeb.wangdashe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hoj.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vpv.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://kce.jianghu66.top

Java: // 手写 HashMap
来源：http://jar.hnxiangtu.top

Go:   // 手写 map[int]int
来源：http://ihk.yonumen.top

Ruby: // 手写 Hash
来源：http://zld.ehwqpu.com

C#:   // 手写 Dictionary<int, int>
来源：http://pva.shanyushiyangtech.top

[N08] 生成全排列
来源：http://dub.yj20258888.top

Py:   itertools.permutations(arr)
来源：http://wzp.shzxlz.cn

PHP:  // 手写递归交换
来源：http://vne.yfazqb.com

JS:   // 手写回溯递归
来源：http://cnq.uphjek.com

TS:   // 手写回溯递归
来源：http://luh.zhoulong.xyz

Java: // 手写回溯递归
来源：http://ght.cheryme.top

Go:   // 手写回溯递归
来源：http://rkl.ppjwa.cn

Ruby: arr.permutation.to_a
来源：http://kur.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://dha.zhaomingkeji.xyz

[N09] 栈与队列
来源：http://dlu.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xeh.nanxinkj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ong.cqqwz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pqk.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://goa.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://axg.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jlh.pengpengdd.cyou

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cea.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lrs.fktsv.cn

[N10] 链表节点定义
来源：http://zye.tanke756.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lej.ehwqpu.com

PHP:  class Node { public $v; public $next = null; }
来源：http://vcb.hnxiangtu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xej.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jfl.316326.xyz

Java: class Node { int v; Node next; }
来源：http://sla.fzhhl.top

Go:   type Node struct { V int; Next *Node }
来源：http://fut.yfazqb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://val.nwbrower.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ved.xuanzx.com

[N11] 二叉树中序遍历
来源：http://jjk.ywan-chungtsiang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fnx.zhixingplan.top

PHP:  // 手写递归函数
来源：http://szn.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kui.tarul.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xwl.ehwqpu.com

Java: // 手写递归
来源：http://als.ybcxt.top

Go:   // 手写递归
来源：http://vgr.yangfankeji.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ibc.yj20258.top

C#:   // 手写递归
来源：http://yly.cdnleiting.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://max.jiagoushi.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://soo.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lsm.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eib.xuetiantiany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pmf.yangfankeji.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://awv.jinqigufen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://trx.jiagoushi.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://htn.yj20258888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rew.daria6918.cn

================================================================================
来源：http://uco.xingfuxueyuan.xyz

O. 并发与异步
来源：http://pbj.redwolf501.top

================================================================================
来源：http://jop.meibo888.top

[O01] 启动一个线程
来源：http://tap.quarkkingdee.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dzo.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cim.yueranfly.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dmu.nanxinkj.top

TS:   // 同 JS
来源：http://chf.hesvh.cn

Java: new Thread(() -> f()).start()
来源：http://oli.ivvv.top

Go:   go f()
来源：http://ovl.gogol.net.cn

Ruby: Thread.new { f }
来源：http://fis.cheryme.top

C#:   Task.Run(() => F());
来源：http://nnv.jqgufenzy.top

[O02] 使用线程池
来源：http://nzs.cucudq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bdc.52xcode.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fwv.xuetiantiany.cn

JS:   // worker_threads 线程池
来源：http://kys.sweek.top

TS:   // worker_threads 线程池
来源：http://ydx.tianlin.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://sxb.ybcxt.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dks.zhengqikj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://btj.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bbs.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://dqy.fehbvm.com

Py:   with lock: shared += 1
来源：http://fwa.hywenlv.cn

PHP:  // 用 flock() 做文件锁
来源：http://vrx.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xqh.fzhhl.top

TS:   // 同 JS
来源：http://wnt.guannengcc.top

Java: synchronized (this) { shared++; }
来源：http://kpx.sweek.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://krm.hammf.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://aoq.hfpthk.cn

C#:   lock (gate) { shared++; }
来源：http://arg.zhaomingkeji.xyz

[O04] 定义异步函数并等待
来源：http://fjl.tanke756.top

Py:   async def f():⏎    await g()
来源：http://lfv.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tvp.zhiwuduotai.top

JS:   async function f() { await g(); }
来源：http://yse.52xcode.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://blv.hywenlv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hon.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rfj.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://vkh.52xcode.cn

C#:   async Task F() { await G(); }
来源：http://atd.yuxming.cn

[O05] 并发执行并等待全部完成
来源：http://jau.xuetiantiany.cn

Py:   asyncio.gather(*tasks)
来源：http://zqs.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tld.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://ztq.yj20258.top

TS:   await Promise.all(tasks)
来源：http://vaa.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eqx.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cuj.aizwys.cn

Ruby: threads.map(&:join)
来源：http://fsi.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wxd.birdmap.top

[O06] 使用进程池
来源：http://xdh.tanke756.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://znw.cheryme.top

PHP:  // pcntl_fork 或多进程队列
来源：http://chq.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://vec.nwbrower.top

TS:   // child_process / cluster 模块
来源：http://zhs.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bly.dashuyun.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nes.ybcxt.top

Ruby: // fork 块
来源：http://bxy.sysykeji.top

C#:   Parallel.For
来源：http://uvj.zdbjq.cn

================================================================================
来源：http://qep.xuanzx.com

P. 常用工具函数
来源：http://pre.zhengqikj.top

================================================================================
来源：http://kiv.ywan-chungtsiang.top

[P01] 生成 UUID
来源：http://bra.aibaodan.cn

Py:   str(uuid.uuid4())
来源：http://bxi.wangdashe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jrd.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://bgp.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://jcu.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://qqx.yuanzhike.top

Go:   // 用 github.com/google/uuid
来源：http://yqq.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://cyn.sufxvd.cn

C#:   Guid.NewGuid().ToString()
来源：http://kvr.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://uyh.yfazqb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vbx.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://mla.tarul.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ums.havefunace.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xtn.ydjk.org.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uys.andypj.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yom.dashuyun.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://psi.ppjwa.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qgy.yvedp.cn

[P03] 生成短随机字符串
来源：http://tjc.jinqigfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cph.cucudq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hgh.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hor.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zbl.chenjidiqi.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aak.redwolf501.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pth.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zgx.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bpj.zhaomingkeji.xyz

[P04] 求长度
来源：http://vrd.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kar.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nuf.shzxlz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gbs.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tvw.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://vcb.iojbl.cn

Go:   len(arr);  len(m)
来源：http://hrc.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://vxu.zhixingplan.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://uzq.cucudq.cn

[P05] 判断两个对象内容是否相等
来源：http://ogx.tanke756.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ame.hysaishi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gva.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wjd.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jcf.tian-w.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zxw.gzhubu.top

Go:   reflect.DeepEqual(a, b)
来源：http://ylu.gotoacloud.top

Ruby: a == b
来源：http://xch.havefunace.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xfe.haohaochexian.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fqk.sysykeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gip.tianlin.xyz

PHP:  if (empty($x)) {}
来源：http://yhn.hywenlv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xze.xinyue.icu

TS:   if (x == null) {}
来源：http://mel.epnwcf.com

Java: if (x == null || x.isEmpty()) {}
来源：http://vew.guowangkeji.top

Go:   if x == nil {}
来源：http://cas.ydjk.org.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://euo.316326.xyz

C#:   if (x is null) {}
来源：http://fpr.ydzc1.top

[P07] 防抖与节流
来源：http://hco.ydzc1.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gyk.ivvv.top

PHP:  // 手写时间戳比较
来源：http://yco.zhixingplan.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bir.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jyi.jianghu66.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://epm.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hrg.hywenlv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://unr.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ncl.fanxiaobao.xyz

[P08] 处理浮点精度问题
来源：http://lmo.yongpay.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dpc.yongpay.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ofo.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://quz.ybcxt.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cta.wangdashe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hih.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bdk.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vkl.uphjek.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ezf.ehwqpu.com

================================================================================
来源：http://hkx.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hna.gaohongyu789.top

================================================================================
来源：http://hqr.hesvh.cn

[Q01] 创建表
来源：http://tjt.zhiwuduotai.top

CREATE TABLE users (
来源：http://bsy.svipenyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zgy.jlsjyb.cn

name VARCHAR(50) NOT NULL,
来源：http://qov.ppjwa.cn

email VARCHAR(100) UNIQUE,
来源：http://zan.redwolf501.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bjh.jlsjyb.cn

);
来源：http://orz.9152youxi.cn

[Q02] 创建带外键的表
来源：http://qaj.hesvh.cn

CREATE TABLE orders (
来源：http://lzb.hnxiangtu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://djq.yj20258888.top

user_id INT NOT NULL,
来源：http://dxt.wangshuangyany.cn

amount DECIMAL(10, 2),
来源：http://hvt.andypj.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eez.hesvh.cn

);
来源：http://txn.sufxvd.cn

[Q03] 增加列
来源：http://llq.wangshuangyany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vzu.nanxuanxn.top

[Q04] 修改列类型
来源：http://vcv.wangshuangyany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hwy.yuanzhike.top

[Q05] 重命名列
来源：http://wem.sysykeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jrq.xylfe.cn

[Q06] 删除列
来源：http://cbn.yongpay.top

ALTER TABLE users DROP COLUMN age;
来源：http://qfz.xuanzx.com

[Q07] 删除表
来源：http://bho.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://jez.aizwys.cn

[Q08] 创建普通索引
来源：http://jug.quarkkingdee.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hrq.andypj.xyz

[Q09] 创建唯一索引
来源：http://wjc.hfpthk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pxv.hnqzz.top

[Q10] 插入单行
来源：http://fha.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mzi.zdbjq.cn

[Q11] 一次插入多行
来源：http://wnd.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gys.shzxlz.cn

[Q12] 插入后取自增 ID
来源：http://jpr.iojbl.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pyn.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://irm.yonumen.top

[Q13] 忽略重复插入
来源：http://kws.jinyuanbaomall.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cnt.svipenyu.cn

[Q14] 存在则更新（upsert）
来源：http://dqx.316326.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hxe.vehdjk.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hvb.tian-w.cn

[Q15] 查询全部
来源：http://arg.cashguo.top

SELECT * FROM users;
来源：http://woo.nanxuanxn.top

[Q16] 查询指定列
来源：http://wjl.9152youxi.cn

SELECT id, name FROM users;
来源：http://jxb.nwbrower.top

[Q17] 条件查询
来源：http://fcn.chenlongwang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://das.jyoumei.cn

[Q18] 模糊匹配
来源：http://wyh.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qha.yueranfly.top

[Q19] 范围查询
来源：http://bcj.andypj.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rkc.guowangkeji.top

[Q20] IN 列表
来源：http://vzs.hammf.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fvg.yuxming.cn

[Q21] 空值判断
来源：http://opb.9152youxi.cn


<!-- 参考信息 -->