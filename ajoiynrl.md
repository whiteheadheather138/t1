代发 wailian999

TS:   process.platform;  process.version
来源：http://tlv.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ujx.sweek.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://waw.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://okm.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://phz.tianlin.xyz

================================================================================
来源：http://zmk.cqqwz.cn

N. 数据结构与算法
来源：http://rax.jianghu66.top

================================================================================
来源：http://ncu.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://qis.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://lmb.chenlongwang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zky.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://krd.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vch.fengsongda.top

Java: Arrays.binarySearch(arr, x)
来源：http://mfv.shangyingyoupin.top

Go:   sort.SearchInts(arr, x)
来源：http://alk.snrcjt.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hgj.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://iqh.nwbrower.top

[N02] 排序（工程实践用内置实现）
来源：http://xok.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://nqr.aibaodan.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bat.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tvp.jqgfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qbd.hfpthk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ooa.fanxiaobao.xyz

Go:   slices.Sort(arr)
来源：http://nqq.pycfn.com

Ruby: arr.sort
来源：http://bpg.jlsjyb.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://iva.nanxinkj.top

[N03] 快速排序（分治示例）
来源：http://kwx.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zqg.gogol.net.cn

PHP:  // 递归实现，或用 usort
来源：http://aki.yueranfly.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lhm.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fct.bbcook.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nap.xingfuxueyuan.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eck.smart0.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aax.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://trz.wangshuangyany.cn

[N04] 斐波那契数列
来源：http://jwg.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ibr.daxiang520.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nwu.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://coj.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://acx.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://myk.zdbjq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qxg.aibaodan.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uaa.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jhz.guannengcc.top

[N05] 最大公约数
来源：http://kes.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://xbx.sufxvd.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://emb.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tqm.redwolf501.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mdw.epnwcf.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ymy.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lkq.yonumen.top

Ruby: a.gcd(b)
来源：http://tth.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qpy.bjfxy.top

[N06] 判断回文字符串
来源：http://ibp.daxiang520.top

Py:   s == s[::-1]
来源：http://gso.sweek.top

PHP:  $s === strrev($s);
来源：http://qsh.ppjwa.cn

JS:   s === [...s].reverse().join("")
来源：http://zlb.epnwcf.com

TS:   s === [...s].reverse().join("")
来源：http://awd.vehdjk.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lwg.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://gba.zhaomingkeji.xyz

Ruby: s == s.reverse
来源：http://bzf.kuanghao11.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nzd.hongshengwenyu.top

[N07] 两数之和（返回下标）
来源：http://san.ydjk.org.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eak.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://itg.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fhq.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://xef.daxiang520.top

Java: // 手写 HashMap
来源：http://gts.jlsjyb.cn

Go:   // 手写 map[int]int
来源：http://bvo.yj20258888.top

Ruby: // 手写 Hash
来源：http://thm.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://mab.kuanghao11.cn

[N08] 生成全排列
来源：http://jud.hnqzz.top

Py:   itertools.permutations(arr)
来源：http://ccx.wangdashe.top

PHP:  // 手写递归交换
来源：http://kqf.jiagoushi.top

JS:   // 手写回溯递归
来源：http://rzq.gzhubu.top

TS:   // 手写回溯递归
来源：http://uyb.jyoumei.cn

Java: // 手写回溯递归
来源：http://xwn.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://wju.birdmap.top

Ruby: arr.permutation.to_a
来源：http://rwx.xuanzx.com

C#:   // 手写回溯递归
来源：http://gym.birdmap.top

[N09] 栈与队列
来源：http://pzd.fehbvm.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gbh.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nfs.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qkr.aizwys.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yxg.ydjk.org.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://toz.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://owv.fengsongda.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://icl.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tmq.yanxiufei.cn

[N10] 链表节点定义
来源：http://oex.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ird.fzhhl.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fjs.xuetiantiany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pzo.haohaochexian.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xlp.vehdjk.com

Java: class Node { int v; Node next; }
来源：http://ctw.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ipo.epnwcf.com

Ruby: Node = Struct.new(:v, :next)
来源：http://rmq.vqdsnc.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ybp.havefunace.top

[N11] 二叉树中序遍历
来源：http://zpu.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lbp.yfazqb.com

PHP:  // 手写递归函数
来源：http://hco.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eea.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tiz.yfazqb.com

Java: // 手写递归
来源：http://szu.yangfankeji.com

Go:   // 手写递归
来源：http://frb.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vgu.wangdashe.top

C#:   // 手写递归
来源：http://laf.quarkkingdee.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dps.yonumen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pek.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nib.vehdjk.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mhb.jinghuilouyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jen.gzhubu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ydu.jinqigufen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://igb.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vpj.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pqn.cdnleiting.top

================================================================================
来源：http://sbu.tian-w.cn

O. 并发与异步
来源：http://yjq.ivvv.top

================================================================================
来源：http://bdj.0kj1m.cn

[O01] 启动一个线程
来源：http://kii.fengsongda.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tyd.chenlongwang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fyh.ppjwa.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gxw.yanxiufei.cn

TS:   // 同 JS
来源：http://pjr.jinghuilouyu.cn

Java: new Thread(() -> f()).start()
来源：http://zvq.guannengcc.top

Go:   go f()
来源：http://gbn.daria6918.cn

Ruby: Thread.new { f }
来源：http://ngx.jlsjyb.cn

C#:   Task.Run(() => F());
来源：http://xpx.bbcook.cn

[O02] 使用线程池
来源：http://mok.ehwqpu.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mzc.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cpq.bjfxy.top

JS:   // worker_threads 线程池
来源：http://qla.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://cln.daria6918.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yxv.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hhb.birdmap.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jwb.hongshengwenyu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://usk.chenlongwang.top

[O03] 加锁保护共享数据
来源：http://mac.jianghu66.top

Py:   with lock: shared += 1
来源：http://ren.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://elk.gaohongyu789.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rds.fktsv.cn

TS:   // 同 JS
来源：http://ybz.pengpengdd.cyou

Java: synchronized (this) { shared++; }
来源：http://orw.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hzf.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qxo.jinqigufen.top

C#:   lock (gate) { shared++; }
来源：http://mdv.yongpay.top

[O04] 定义异步函数并等待
来源：http://jzd.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://chk.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dnq.shangyingyoupin.top

JS:   async function f() { await g(); }
来源：http://anl.0kj1m.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dsj.hongshengwenyu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xte.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mkt.feifeiyinyue.top

Ruby: # 用 Fiber 或 async gem
来源：http://vos.vehdjk.com

C#:   async Task F() { await G(); }
来源：http://qky.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://xrk.ywan-chungtsiang.top

Py:   asyncio.gather(*tasks)
来源：http://xyh.jinghuilouyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://opk.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://coj.hesvh.cn

TS:   await Promise.all(tasks)
来源：http://mzd.ybcxt.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://edr.gzhubu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lze.xziqi.cn

Ruby: threads.map(&:join)
来源：http://kqt.wangdashe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://skr.52xcode.cn

[O06] 使用进程池
来源：http://uiv.yueranfly.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zfb.cucudq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qph.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://aox.yuxming.cn

TS:   // child_process / cluster 模块
来源：http://iry.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hfc.shanyushiyangtech.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://llx.tanke756.top

Ruby: // fork 块
来源：http://ijn.yfazqb.com

C#:   Parallel.For
来源：http://ixn.jqgufenzy.top

================================================================================
来源：http://myw.yonumen.top

P. 常用工具函数
来源：http://rfe.yj202588.top

================================================================================
来源：http://psz.yj20258.top

[P01] 生成 UUID
来源：http://fpm.daria6918.cn

Py:   str(uuid.uuid4())
来源：http://gjp.epnwcf.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gnv.tarul.cn

JS:   crypto.randomUUID()
来源：http://idp.xylfe.cn

TS:   crypto.randomUUID()
来源：http://xru.cheryme.top

Java: UUID.randomUUID().toString()
来源：http://tie.cdnleiting.top

Go:   // 用 github.com/google/uuid
来源：http://ysy.sxryk.cn

Ruby: SecureRandom.uuid
来源：http://nqk.ydzc1.top

C#:   Guid.NewGuid().ToString()
来源：http://jbw.pengpengdd.cyou

[P02] MD5 / SHA256 摘要
来源：http://vki.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cfm.chenjidiqi.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://pdy.quarkkingdee.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xbv.zhoulong.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jzc.yuanzhike.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aou.c1oappe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lrf.yvedp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lbe.uphjek.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xlg.guannengcc.top

[P03] 生成短随机字符串
来源：http://tyf.hesvh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://czp.cucudq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ola.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rvi.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fhz.xingfuxueyuan.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iza.tarul.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gbm.hammf.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wbh.tanke756.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xdg.shzxlz.cn

[P04] 求长度
来源：http://iqa.gotoacloud.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zfv.cucudq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://icb.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mhl.zycfv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bol.yuanzhike.top

Java: list.size();  map.size();  s.length()
来源：http://jor.ydjk.org.cn

Go:   len(arr);  len(m)
来源：http://kxq.meibo888.top

Ruby: x.length;  x.size
来源：http://xdy.dashuyun.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kfc.xuetiantiany.cn

[P05] 判断两个对象内容是否相等
来源：http://bvf.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jjp.epnwcf.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ors.nwbrower.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vet.shanyushiyangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uco.xuanzx.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xtm.gzhubu.top

Go:   reflect.DeepEqual(a, b)
来源：http://epa.ywan-chungtsiang.top

Ruby: a == b
来源：http://skp.tianlin.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aah.meibo888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uma.svipenyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ksv.birdmap.top

PHP:  if (empty($x)) {}
来源：http://upx.tian-w.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kpl.yj20258888.top

TS:   if (x == null) {}
来源：http://kvc.birdmap.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fpw.sufxvd.cn

Go:   if x == nil {}
来源：http://dgr.ctjpmb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hrg.fktsv.cn

C#:   if (x is null) {}
来源：http://svt.zdbjq.cn

[P07] 防抖与节流
来源：http://rsz.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gfi.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://mjj.wangshuangyany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iop.haohaochexian.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lok.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jhy.cqqwz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://apd.nanxuanxn.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://evy.haohaochexian.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qvh.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://zio.jlsjyb.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ciy.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hid.wangshuangyany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qga.chenlongwang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sjx.ydjk.org.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aoj.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lph.tian-w.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://svs.bjfxy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jpt.daxiang520.top

================================================================================
来源：http://opd.yanxiufei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bxn.yj202588.top

================================================================================
来源：http://jnz.zhixingplan.top

[Q01] 创建表
来源：http://ckh.shangyingyoupin.top

CREATE TABLE users (
来源：http://xwl.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://czq.nwbrower.top

name VARCHAR(50) NOT NULL,
来源：http://mjp.zhongyouzk.top

email VARCHAR(100) UNIQUE,
来源：http://gut.epnwcf.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kwx.ehwqpu.com

);
来源：http://cph.sufxvd.cn

[Q02] 创建带外键的表
来源：http://bux.ydzc1.top

CREATE TABLE orders (
来源：http://nbj.fengsongda.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ctw.hysaishi.cn

user_id INT NOT NULL,
来源：http://bqm.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://qph.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wcn.iojbl.cn

);
来源：http://hwh.9152youxi.cn

[Q03] 增加列
来源：http://pws.yonumen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dbp.iojbl.cn

[Q04] 修改列类型
来源：http://hkk.sysykeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ipz.shangyingyoupin.top

[Q05] 重命名列
来源：http://und.gogol.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://chj.zhixingplan.top

[Q06] 删除列
来源：http://dmg.nanxinkj.top

ALTER TABLE users DROP COLUMN age;
来源：http://fve.hcnkem.com

[Q07] 删除表
来源：http://icq.zhoulong.xyz

DROP TABLE IF EXISTS orders;
来源：http://czi.sweek.top

[Q08] 创建普通索引
来源：http://xix.gotoacloud.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qkr.hfpthk.cn

[Q09] 创建唯一索引
来源：http://pfq.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qbn.gaohongyu789.top

[Q10] 插入单行
来源：http://cvl.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://agd.yongpay.top

[Q11] 一次插入多行
来源：http://ewu.9152youxi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vhl.tanke756.top

[Q12] 插入后取自增 ID
来源：http://pvv.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://gso.hammf.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ibz.bjfxy.top

[Q13] 忽略重复插入
来源：http://jah.daria6918.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://idr.redwolf501.top

[Q14] 存在则更新（upsert）
来源：http://xjx.jinyuanbaomall.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vpk.quarkkingdee.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fyy.hfpthk.cn

[Q15] 查询全部
来源：http://zwl.gzhubu.top

SELECT * FROM users;
来源：http://xle.hongshengwenyu.top

[Q16] 查询指定列
来源：http://hit.havefunace.top

SELECT id, name FROM users;
来源：http://dtj.tian-w.cn

[Q17] 条件查询
来源：http://ffu.chenzaomai.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ojn.redwolf501.top

[Q18] 模糊匹配
来源：http://mxj.dianchejie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yek.daxiang520.top

[Q19] 范围查询
来源：http://inz.fanxiaobao.xyz


<!-- 参考信息 -->