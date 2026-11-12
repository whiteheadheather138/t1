代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://iab.iojbl.cn

================================================================================
来源：http://jkg.birdmap.top

N. 数据结构与算法
来源：http://fuh.pengpengdd.cyou

================================================================================
来源：http://lbb.ydzc1.top

[N01] 二分查找（有序数组）
来源：http://kvx.havefunace.top

Py:   bisect.bisect_left(arr, x)
来源：http://vhv.shuidangran.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yqd.aizwys.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pkv.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mla.fzhhl.top

Java: Arrays.binarySearch(arr, x)
来源：http://twf.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://veq.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rfw.sufxvd.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qal.ybcxt.top

[N02] 排序（工程实践用内置实现）
来源：http://vpn.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://egz.aizwys.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://isp.xuanzx.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://qeo.sweek.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fwj.xuetiantiany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qpc.gogol.net.cn

Go:   slices.Sort(arr)
来源：http://otx.daria6918.cn

Ruby: arr.sort
来源：http://lsn.zdbjq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://thu.snrcjt.cn

[N03] 快速排序（分治示例）
来源：http://leq.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ufn.yj20258.top

PHP:  // 递归实现，或用 usort
来源：http://rsb.fengsongda.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nqu.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kns.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rjk.shanyushiyangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iau.feifeiyinyue.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nov.zhengqikj.top

C#:   // 手写递归，或 Array.Sort
来源：http://dno.aibaodan.cn

[N04] 斐波那契数列
来源：http://kos.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jkw.kuanghao11.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hvo.yfazqb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mhc.pycfn.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fab.fzhhl.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dih.hysaishi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://myv.fzhhl.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://okk.andypj.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qil.iojbl.cn

[N05] 最大公约数
来源：http://rtt.sweek.top

Py:   math.gcd(a, b)
来源：http://nim.daxiang520.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://swt.9152youxi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rtu.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://awo.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://piq.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gok.birdmap.top

Ruby: a.gcd(b)
来源：http://kuj.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wya.sjlbkw.cn

[N06] 判断回文字符串
来源：http://ays.cheryme.top

Py:   s == s[::-1]
来源：http://qcj.nwbrower.top

PHP:  $s === strrev($s);
来源：http://dqv.xziqi.cn

JS:   s === [...s].reverse().join("")
来源：http://pig.shuidangran.top

TS:   s === [...s].reverse().join("")
来源：http://gox.tarul.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lcz.shangyingyoupin.top

Go:   // 双指针从两端比较
来源：http://qrd.cucudq.cn

Ruby: s == s.reverse
来源：http://vbp.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://khp.ppjwa.cn

[N07] 两数之和（返回下标）
来源：http://bui.xziqi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://afu.yj202588.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uou.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wvr.dashuyun.cn

TS:   // 手写 Map<string, number>
来源：http://pvz.yj20258888.top

Java: // 手写 HashMap
来源：http://gie.tanke756.top

Go:   // 手写 map[int]int
来源：http://xkl.meibo888.top

Ruby: // 手写 Hash
来源：http://cgf.shuidangran.top

C#:   // 手写 Dictionary<int, int>
来源：http://axe.yvedp.cn

[N08] 生成全排列
来源：http://hsy.tanke756.top

Py:   itertools.permutations(arr)
来源：http://hdx.redwolf501.top

PHP:  // 手写递归交换
来源：http://cis.ydzc1.top

JS:   // 手写回溯递归
来源：http://ikc.gogol.net.cn

TS:   // 手写回溯递归
来源：http://ogm.chenzaomai.com

Java: // 手写回溯递归
来源：http://gqk.ydzc1.top

Go:   // 手写回溯递归
来源：http://jtm.chenlongwang.top

Ruby: arr.permutation.to_a
来源：http://gxy.aizwys.cn

C#:   // 手写回溯递归
来源：http://qpe.havefunace.top

[N09] 栈与队列
来源：http://tvf.fengsongda.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yos.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bsd.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ehy.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lhu.yonumen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ite.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://chb.gotoacloud.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uvj.xuanzx.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xjh.cucudq.cn

[N10] 链表节点定义
来源：http://dgw.guowangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cvt.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://eua.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://idp.jinghuilouyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nbv.uphjek.com

Java: class Node { int v; Node next; }
来源：http://chz.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://vbd.cucudq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ulp.redwolf501.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rik.ywan-chungtsiang.top

[N11] 二叉树中序遍历
来源：http://qyb.yj202588.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vas.gotoacloud.top

PHP:  // 手写递归函数
来源：http://elr.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gao.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://buu.yonumen.top

Java: // 手写递归
来源：http://djg.snrcjt.cn

Go:   // 手写递归
来源：http://cue.havefunace.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bbj.ivvv.top

C#:   // 手写递归
来源：http://fwk.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kud.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oco.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fga.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ijd.gogol.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sds.cqqwz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dyu.shangyingyoupin.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qkg.birdmap.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oiw.yueranfly.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ivf.yj20258.top

================================================================================
来源：http://jre.yongpay.top

O. 并发与异步
来源：http://hva.sysykeji.top

================================================================================
来源：http://aah.cqqwz.cn

[O01] 启动一个线程
来源：http://rum.sufxvd.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ikl.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://egf.ydzc1.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aii.c1oappe.top

TS:   // 同 JS
来源：http://tot.ctjpmb.com

Java: new Thread(() -> f()).start()
来源：http://ysz.bbcook.cn

Go:   go f()
来源：http://dae.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://new.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://efw.hnqzz.top

[O02] 使用线程池
来源：http://gur.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xus.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vll.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://bbz.sxryk.cn

TS:   // worker_threads 线程池
来源：http://iue.iojbl.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qfx.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://glh.tianlin.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pnp.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nbj.redwolf501.top

[O03] 加锁保护共享数据
来源：http://waz.jqgfzy.top

Py:   with lock: shared += 1
来源：http://kxv.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://dar.nanxinkj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://unu.yvedp.cn

TS:   // 同 JS
来源：http://gef.ppjwa.cn

Java: synchronized (this) { shared++; }
来源：http://dwv.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pyi.jqgfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xtn.zhijiandao.cn

C#:   lock (gate) { shared++; }
来源：http://ysq.quarkkingdee.top

[O04] 定义异步函数并等待
来源：http://mhq.smart0.xyz

Py:   async def f():⏎    await g()
来源：http://bis.tanke756.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://orl.cheryme.top

JS:   async function f() { await g(); }
来源：http://tfy.yfazqb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://hde.ydjk.org.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://azp.fzhhl.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gxd.pycfn.com

Ruby: # 用 Fiber 或 async gem
来源：http://pse.birdmap.top

C#:   async Task F() { await G(); }
来源：http://hta.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://yit.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://yvj.sweek.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ocl.chenzaomai.com

JS:   await Promise.all(tasks)
来源：http://udc.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://ufz.hesvh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mih.bjfxy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wrz.guowangkeji.top

Ruby: threads.map(&:join)
来源：http://kiz.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pmo.yuanzhike.top

[O06] 使用进程池
来源：http://xtd.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lnl.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://kgw.daria6918.cn

JS:   // child_process / cluster 模块
来源：http://kjv.yangfankeji.com

TS:   // child_process / cluster 模块
来源：http://xyv.sjlbkw.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xpe.chenjidiqi.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ggg.zhengqikj.top

Ruby: // fork 块
来源：http://fpy.gaohongyu789.top

C#:   Parallel.For
来源：http://ucf.zdqjudy.top

================================================================================
来源：http://gmf.tian-w.cn

P. 常用工具函数
来源：http://jer.ivvv.top

================================================================================
来源：http://tkk.iojbl.cn

[P01] 生成 UUID
来源：http://rzp.ivvv.top

Py:   str(uuid.uuid4())
来源：http://doe.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://owo.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://qgz.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://pfb.bbcook.cn

Java: UUID.randomUUID().toString()
来源：http://zrq.svipenyu.cn

Go:   // 用 github.com/google/uuid
来源：http://ykm.yanxiufei.cn

Ruby: SecureRandom.uuid
来源：http://ofe.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://ecf.xuetiantiany.cn

[P02] MD5 / SHA256 摘要
来源：http://ohi.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://czz.nanxuanxn.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cep.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ssz.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wbg.tian-w.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hkn.zhixingplan.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dwu.jqgfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cud.shzxlz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vbv.yuanzhike.top

[P03] 生成短随机字符串
来源：http://jzs.ydzc1.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dki.zhixingplan.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fex.yueranfly.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oza.havefunace.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://psa.yangfankeji.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vba.tarul.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tdf.shangyingyoupin.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ncu.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kuz.mhx1999.top

[P04] 求长度
来源：http://rru.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cas.aibaodan.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pxv.xinyue.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hie.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nch.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://gls.hnqzz.top

Go:   len(arr);  len(m)
来源：http://osj.dianchejie.cn

Ruby: x.length;  x.size
来源：http://zoe.jlsjyb.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zxj.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://nix.vehdjk.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://fdt.vehdjk.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rdr.aizwys.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ryi.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cli.chenlongwang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uev.zhixingplan.top

Go:   reflect.DeepEqual(a, b)
来源：http://fmk.zhengqikj.top

Ruby: a == b
来源：http://fdr.yongpay.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nwv.hfpthk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kth.cucudq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://laq.yj20258888.top

PHP:  if (empty($x)) {}
来源：http://mhn.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://irg.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://zvz.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ybj.gotoacloud.top

Go:   if x == nil {}
来源：http://qbz.zdqjudy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wde.zhaomingkeji.xyz

C#:   if (x is null) {}
来源：http://mce.pengpengdd.cyou

[P07] 防抖与节流
来源：http://mvk.ehwqpu.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mkf.hammf.cn

PHP:  // 手写时间戳比较
来源：http://vhl.hysaishi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://grm.xinyue.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jdq.ydjk.org.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qzr.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qpy.sjlbkw.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pih.zhongyouzk.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hcf.vehdjk.com

[P08] 处理浮点精度问题
来源：http://duq.shzxlz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ypq.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zot.cdnleiting.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ffr.dashuyun.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ett.guowangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mgj.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bjp.meibo888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sww.fehbvm.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sjn.hnxiangtu.top

================================================================================
来源：http://jdh.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zbw.bbcook.cn

================================================================================
来源：http://cnu.pengpengdd.cyou

[Q01] 创建表
来源：http://lrj.cdnleiting.top

CREATE TABLE users (
来源：http://wvl.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qyt.jinyuanbaomall.cn

name VARCHAR(50) NOT NULL,
来源：http://mxi.daxiang520.top

email VARCHAR(100) UNIQUE,
来源：http://kma.xziqi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tgp.smart0.xyz

);
来源：http://nnr.tianlin.xyz

[Q02] 创建带外键的表
来源：http://qjq.zhoulong.xyz

CREATE TABLE orders (
来源：http://gux.sweek.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://evg.yuxming.cn

user_id INT NOT NULL,
来源：http://yaz.xziqi.cn

amount DECIMAL(10, 2),
来源：http://box.yangfankeji.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://asw.haohaochexian.top

);
来源：http://wnz.vqdsnc.cn

[Q03] 增加列
来源：http://lct.zdbjq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zdt.fktsv.cn

[Q04] 修改列类型
来源：http://olw.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zxp.ppjwa.cn

[Q05] 重命名列
来源：http://rtw.yj20258.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://svb.yonumen.top

[Q06] 删除列
来源：http://ffq.cdnleiting.top

ALTER TABLE users DROP COLUMN age;
来源：http://wuh.yangfankeji.com

[Q07] 删除表
来源：http://otz.feifeiyinyue.top

DROP TABLE IF EXISTS orders;
来源：http://aac.zdbjq.cn

[Q08] 创建普通索引
来源：http://fcm.chenjidiqi.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://wrv.ivvv.top

[Q09] 创建唯一索引
来源：http://gwl.mhx1999.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jfw.xuetiantiany.cn

[Q10] 插入单行
来源：http://qyb.fzhhl.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tlb.yj20258.top

[Q11] 一次插入多行
来源：http://cgk.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sxe.ivvv.top

[Q12] 插入后取自增 ID
来源：http://mbl.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://ukk.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yrc.cashguo.top

[Q13] 忽略重复插入
来源：http://qwr.yongpay.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vcn.svipenyu.cn

[Q14] 存在则更新（upsert）
来源：http://ujr.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ljt.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cor.haohaochexian.top

[Q15] 查询全部
来源：http://zof.fengsongda.top

SELECT * FROM users;
来源：http://keh.epnwcf.com

[Q16] 查询指定列
来源：http://hqg.hywenlv.cn

SELECT id, name FROM users;
来源：http://tyc.kuanghao11.cn

[Q17] 条件查询
来源：http://gvf.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jff.chenzaomai.com

[Q18] 模糊匹配
来源：http://mme.yuanzhike.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ltd.hnqzz.top

[Q19] 范围查询
来源：http://juq.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ydv.shangyingyoupin.top

[Q20] IN 列表
来源：http://kam.zhoulong.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gvv.snrcjt.cn

[Q21] 空值判断
来源：http://xso.dianchejie.cn


<!-- 参考信息 -->