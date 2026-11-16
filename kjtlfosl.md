代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://wsv.shanyushiyangtech.top

================================================================================
来源：http://arw.yj202588.top

N. 数据结构与算法
来源：http://auu.shzxlz.cn

================================================================================
来源：http://nnd.hcnkem.com

[N01] 二分查找（有序数组）
来源：http://ncj.xingfuxueyuan.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://szo.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gze.tian-w.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sax.gotoacloud.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cli.birdmap.top

Java: Arrays.binarySearch(arr, x)
来源：http://vjn.smart0.xyz

Go:   sort.SearchInts(arr, x)
来源：http://jbv.fanxiaobao.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://fab.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://atc.aizwys.cn

[N02] 排序（工程实践用内置实现）
来源：http://tzo.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://imb.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://slv.yuanzhike.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tbx.mhx1999.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://psu.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pki.0kj1m.cn

Go:   slices.Sort(arr)
来源：http://fxa.daxiang520.top

Ruby: arr.sort
来源：http://ntd.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bng.hysaishi.cn

[N03] 快速排序（分治示例）
来源：http://nqg.aizwys.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ajc.tianlin.xyz

PHP:  // 递归实现，或用 usort
来源：http://vtd.c1oappe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gqn.shanyushiyangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fom.yfazqb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oag.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ovf.xziqi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pho.daria6918.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hwa.yj20258888.top

[N04] 斐波那契数列
来源：http://bkn.meibo888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xdw.cqqwz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kry.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iud.fengsongda.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dcb.jqgufenzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oyq.52xcode.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sxx.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://syi.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://buz.zdqjudy.top

[N05] 最大公约数
来源：http://fhz.sufxvd.cn

Py:   math.gcd(a, b)
来源：http://vqs.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qmw.hfpthk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bxm.yangfankeji.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zyh.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zxx.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ksk.jiagoushi.top

Ruby: a.gcd(b)
来源：http://exa.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://slw.hywenlv.cn

[N06] 判断回文字符串
来源：http://pow.hysaishi.cn

Py:   s == s[::-1]
来源：http://hlq.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://lxc.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://int.yongpay.top

TS:   s === [...s].reverse().join("")
来源：http://lah.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://viz.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://tzh.birdmap.top

Ruby: s == s.reverse
来源：http://rrs.fehbvm.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://riz.haohaochexian.top

[N07] 两数之和（返回下标）
来源：http://jhf.yuxming.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jqa.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wjk.zhixingplan.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ago.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://wao.gotoacloud.top

Java: // 手写 HashMap
来源：http://tdn.daxiang520.top

Go:   // 手写 map[int]int
来源：http://mkp.0kj1m.cn

Ruby: // 手写 Hash
来源：http://dsy.nanxuanxn.top

C#:   // 手写 Dictionary<int, int>
来源：http://cdq.sufxvd.cn

[N08] 生成全排列
来源：http://dbk.havefunace.top

Py:   itertools.permutations(arr)
来源：http://pgw.hywenlv.cn

PHP:  // 手写递归交换
来源：http://wts.jqgfzy.top

JS:   // 手写回溯递归
来源：http://pqj.guowangkeji.top

TS:   // 手写回溯递归
来源：http://yof.yongpay.top

Java: // 手写回溯递归
来源：http://eme.smart0.xyz

Go:   // 手写回溯递归
来源：http://qlz.dianchejie.cn

Ruby: arr.permutation.to_a
来源：http://von.tarul.cn

C#:   // 手写回溯递归
来源：http://dac.fanxiaobao.xyz

[N09] 栈与队列
来源：http://sff.9152youxi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://veu.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bqm.yj20258888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ezq.fehbvm.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ngt.cucudq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hup.gogol.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bna.wangshuangyany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qqj.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://veg.gaohongyu789.top

[N10] 链表节点定义
来源：http://gzy.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dlc.jinghuilouyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hfm.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lps.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://afg.yj202588.top

Java: class Node { int v; Node next; }
来源：http://xpu.yvedp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gmo.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mvj.uphjek.com

C#:   class Node { public int V; public Node? Next; }
来源：http://lwd.zycfv.cn

[N11] 二叉树中序遍历
来源：http://rxu.hfpthk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kjn.sysykeji.top

PHP:  // 手写递归函数
来源：http://rtl.quarkkingdee.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vvz.yueranfly.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qct.dianchejie.cn

Java: // 手写递归
来源：http://msz.vqdsnc.cn

Go:   // 手写递归
来源：http://edv.daxiang520.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://shp.vqdsnc.cn

C#:   // 手写递归
来源：http://gfv.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://phl.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dwb.aibaodan.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dhq.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ozk.vqdsnc.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://szb.cucudq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dis.zhoulong.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pgl.gogol.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yzv.fehbvm.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qmh.ydzc1.top

================================================================================
来源：http://jtt.hongshengwenyu.top

O. 并发与异步
来源：http://dzz.daria6918.cn

================================================================================
来源：http://fzh.xinyue.icu

[O01] 启动一个线程
来源：http://cce.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xhz.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cxy.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fpd.bbcook.cn

TS:   // 同 JS
来源：http://wgh.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://txr.jinqigufen.top

Go:   go f()
来源：http://npf.52xcode.cn

Ruby: Thread.new { f }
来源：http://ttl.xuanzx.com

C#:   Task.Run(() => F());
来源：http://riq.mhx1999.top

[O02] 使用线程池
来源：http://dak.tianlin.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uwt.52xcode.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dfv.tarul.cn

JS:   // worker_threads 线程池
来源：http://buq.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://bbn.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yka.shangyingyoupin.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zrf.hongshengwenyu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ldf.ctjpmb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://viu.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://noe.dianchejie.cn

Py:   with lock: shared += 1
来源：http://vgx.birdmap.top

PHP:  // 用 flock() 做文件锁
来源：http://ftq.sufxvd.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dhq.0kj1m.cn

TS:   // 同 JS
来源：http://yhi.quarkkingdee.top

Java: synchronized (this) { shared++; }
来源：http://rxt.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kzk.chenlongwang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://saw.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://ypk.chenzaomai.com

[O04] 定义异步函数并等待
来源：http://mtv.meibo888.top

Py:   async def f():⏎    await g()
来源：http://juy.ppjwa.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://llg.bbcook.cn

JS:   async function f() { await g(); }
来源：http://aqx.bjfxy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jyz.xinyue.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://phk.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cje.birdmap.top

Ruby: # 用 Fiber 或 async gem
来源：http://qkc.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://gek.zycfv.cn

[O05] 并发执行并等待全部完成
来源：http://zxu.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://xih.zhijiandao.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zyd.xuanzx.com

JS:   await Promise.all(tasks)
来源：http://xpc.yuxming.cn

TS:   await Promise.all(tasks)
来源：http://puc.feifeiyinyue.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://doi.chenlongwang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xme.gzhubu.top

Ruby: threads.map(&:join)
来源：http://sax.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qvn.bjfxy.top

[O06] 使用进程池
来源：http://qfr.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pmp.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yfi.guowangkeji.top

JS:   // child_process / cluster 模块
来源：http://yio.jinqigufen.top

TS:   // child_process / cluster 模块
来源：http://ybc.zhaomingkeji.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sii.hcnkem.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fdn.fehbvm.com

Ruby: // fork 块
来源：http://cwf.hnxiangtu.top

C#:   Parallel.For
来源：http://cmz.0kj1m.cn

================================================================================
来源：http://ssj.jinyuanbaomall.cn

P. 常用工具函数
来源：http://fit.xuetiantiany.cn

================================================================================
来源：http://msx.shangyingyoupin.top

[P01] 生成 UUID
来源：http://wsd.zdbjq.cn

Py:   str(uuid.uuid4())
来源：http://apb.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ast.nwbrower.top

JS:   crypto.randomUUID()
来源：http://alx.ybcxt.top

TS:   crypto.randomUUID()
来源：http://gio.hysaishi.cn

Java: UUID.randomUUID().toString()
来源：http://nep.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://vkz.ctjpmb.com

Ruby: SecureRandom.uuid
来源：http://xav.aizwys.cn

C#:   Guid.NewGuid().ToString()
来源：http://qok.yanxiufei.cn

[P02] MD5 / SHA256 摘要
来源：http://vgx.jqgfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fqj.aibaodan.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wss.sjlbkw.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lny.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://huu.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://trm.shanyushiyangtech.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xol.aibaodan.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fyj.jiagoushi.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pyj.cucudq.cn

[P03] 生成短随机字符串
来源：http://gsl.yangfankeji.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://emz.jianghu66.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://voj.yongpay.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mpu.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mqq.hfpthk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sxw.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mxb.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://ett.zhengqikj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://unm.cqqwz.cn

[P04] 求长度
来源：http://vyn.xuanzx.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rlx.bjfxy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zas.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qoj.fzhhl.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kjc.ywan-chungtsiang.top

Java: list.size();  map.size();  s.length()
来源：http://hvy.0kj1m.cn

Go:   len(arr);  len(m)
来源：http://obg.shanyushiyangtech.top

Ruby: x.length;  x.size
来源：http://lli.hammf.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vps.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://xql.hfpthk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zln.uphjek.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oow.gaohongyu789.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hmz.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lld.feifeiyinyue.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mpe.zhoulong.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://fqa.hesvh.cn

Ruby: a == b
来源：http://vms.yj20258.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tnn.tian-w.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://okp.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xll.chenlongwang.top

PHP:  if (empty($x)) {}
来源：http://iap.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://trw.gotoacloud.top

TS:   if (x == null) {}
来源：http://nqh.dashuyun.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lbi.fzhhl.top

Go:   if x == nil {}
来源：http://nrp.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pvg.sjlbkw.cn

C#:   if (x is null) {}
来源：http://gsy.yangfankeji.com

[P07] 防抖与节流
来源：http://voa.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://okq.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://wyn.yangfankeji.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://msj.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bih.fktsv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uiw.9152youxi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rwv.hammf.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wra.snrcjt.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qhc.svipenyu.cn

[P08] 处理浮点精度问题
来源：http://iuh.zhijiandao.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jih.shanyushiyangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rpk.hnxiangtu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://enf.fengsongda.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sdk.sysykeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hqh.bjfxy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://svj.aibaodan.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ltp.ctjpmb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hjw.andypj.xyz

================================================================================
来源：http://fuv.0kj1m.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://htv.tarul.cn

================================================================================
来源：http://dea.gaohongyu789.top

[Q01] 创建表
来源：http://cvv.vqdsnc.cn

CREATE TABLE users (
来源：http://jiu.yangfankeji.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zdz.uphjek.com

name VARCHAR(50) NOT NULL,
来源：http://agc.tianlin.xyz

email VARCHAR(100) UNIQUE,
来源：http://zvz.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ifj.sxryk.cn

);
来源：http://rhn.zdbjq.cn

[Q02] 创建带外键的表
来源：http://vcj.wangdashe.top

CREATE TABLE orders (
来源：http://azq.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wdu.cashguo.top

user_id INT NOT NULL,
来源：http://zek.shuidangran.top

amount DECIMAL(10, 2),
来源：http://fxe.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bso.hnxiangtu.top

);
来源：http://dla.ehwqpu.com

[Q03] 增加列
来源：http://fxn.xuanzx.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qxn.daxiang520.top

[Q04] 修改列类型
来源：http://ulg.chenjidiqi.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pzf.9152youxi.cn

[Q05] 重命名列
来源：http://cpj.quarkkingdee.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cnu.aibaodan.cn

[Q06] 删除列
来源：http://wdc.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://rne.jinghuilouyu.cn

[Q07] 删除表
来源：http://qww.aizwys.cn

DROP TABLE IF EXISTS orders;
来源：http://igb.bbcook.cn

[Q08] 创建普通索引
来源：http://rfs.zhiwuduotai.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pjt.xuetiantiany.cn

[Q09] 创建唯一索引
来源：http://mut.zhaomingkeji.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jvo.hesvh.cn

[Q10] 插入单行
来源：http://dme.jiagoushi.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vma.c1oappe.top

[Q11] 一次插入多行
来源：http://ghg.tian-w.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ngp.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://zas.yonumen.top

INSERT INTO users (name) VALUES ('C');
来源：http://cik.zhijiandao.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dwa.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://ffa.haohaochexian.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aqp.tarul.cn

[Q14] 存在则更新（upsert）
来源：http://mjb.c1oappe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rik.yueranfly.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vwy.shanyushiyangtech.top

[Q15] 查询全部
来源：http://qwu.hammf.cn

SELECT * FROM users;
来源：http://raq.dashuyun.cn

[Q16] 查询指定列
来源：http://nkk.zhaomingkeji.xyz

SELECT id, name FROM users;
来源：http://mpq.c1oappe.top

[Q17] 条件查询
来源：http://ods.fanxiaobao.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jin.vehdjk.com

[Q18] 模糊匹配
来源：http://hwv.dianchejie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wbu.tanke756.top

[Q19] 范围查询
来源：http://oxx.xingfuxueyuan.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kot.andypj.xyz

[Q20] IN 列表
来源：http://pyi.bbcook.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kwo.cheryme.top

[Q21] 空值判断
来源：http://qhp.hnqzz.top


<!-- 参考信息 -->