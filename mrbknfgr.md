代发 wailian999

TS:   process.platform;  process.version
来源：http://llx.yj20258888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tkl.nanxinkj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ccv.zhongyouzk.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ycy.shzxlz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mbj.xuetiantiany.cn

================================================================================
来源：http://ztc.cashguo.top

N. 数据结构与算法
来源：http://huq.yvedp.cn

================================================================================
来源：http://iai.chenjidiqi.icu

[N01] 二分查找（有序数组）
来源：http://yip.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://wly.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rhi.fanxiaobao.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pno.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fbs.feifeiyinyue.top

Java: Arrays.binarySearch(arr, x)
来源：http://mpz.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://xwq.zhixingplan.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xee.yfazqb.com

C#:   Array.BinarySearch(arr, x)
来源：http://gfm.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://oqd.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://dtz.mhx1999.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://njg.iojbl.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rdy.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://byf.cucudq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kwc.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://pcq.smart0.xyz

Ruby: arr.sort
来源：http://ddf.guannengcc.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kns.jiagoushi.top

[N03] 快速排序（分治示例）
来源：http://qyn.52xcode.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bqd.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://cmg.zhiwuduotai.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pgb.gotoacloud.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zsk.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aqc.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gfu.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bsj.zhoulong.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://smu.pycfn.com

[N04] 斐波那契数列
来源：http://mlw.vqdsnc.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fos.zhixingplan.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uct.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rts.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uag.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xcy.wangshuangyany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fpd.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dlv.hcnkem.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nki.zdqjudy.top

[N05] 最大公约数
来源：http://xjc.yanxiufei.cn

Py:   math.gcd(a, b)
来源：http://gxx.hnqzz.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ofn.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ctp.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bmi.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hwy.sufxvd.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://flz.gaohongyu789.top

Ruby: a.gcd(b)
来源：http://fqi.aibaodan.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://okc.kuanghao11.cn

[N06] 判断回文字符串
来源：http://izr.mhx1999.top

Py:   s == s[::-1]
来源：http://xeo.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://thj.jqgfzy.top

JS:   s === [...s].reverse().join("")
来源：http://vlr.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://sry.gaohongyu789.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nze.xingfuxueyuan.xyz

Go:   // 双指针从两端比较
来源：http://kwf.yuanzhike.top

Ruby: s == s.reverse
来源：http://qzl.zhiwuduotai.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://aai.shuidangran.top

[N07] 两数之和（返回下标）
来源：http://nao.aizwys.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ekp.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dwk.redwolf501.top

JS:   // 手写 Map：map.set(v, i)
来源：http://udw.cdnleiting.top

TS:   // 手写 Map<string, number>
来源：http://sys.wangdashe.top

Java: // 手写 HashMap
来源：http://nlp.nanxuanxn.top

Go:   // 手写 map[int]int
来源：http://ykg.snrcjt.cn

Ruby: // 手写 Hash
来源：http://kib.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://teg.yfazqb.com

[N08] 生成全排列
来源：http://wdz.chenjidiqi.icu

Py:   itertools.permutations(arr)
来源：http://zjo.tianlin.xyz

PHP:  // 手写递归交换
来源：http://dwa.jianghu66.top

JS:   // 手写回溯递归
来源：http://drx.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://wxf.zhaomingkeji.xyz

Java: // 手写回溯递归
来源：http://hzp.sysykeji.top

Go:   // 手写回溯递归
来源：http://myp.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://ulk.9152youxi.cn

C#:   // 手写回溯递归
来源：http://vin.yuanzhike.top

[N09] 栈与队列
来源：http://ajg.shuidangran.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cvr.tian-w.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cpv.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://emn.shuidangran.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gal.zhaomingkeji.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fvh.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://toi.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lwb.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mcg.fzhhl.top

[N10] 链表节点定义
来源：http://vih.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ijt.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://yss.tianlin.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://syy.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hiq.yj202588.top

Java: class Node { int v; Node next; }
来源：http://fie.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yfh.feifeiyinyue.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lwa.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://eod.guannengcc.top

[N11] 二叉树中序遍历
来源：http://apo.zhijiandao.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xta.guannengcc.top

PHP:  // 手写递归函数
来源：http://hea.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://isb.pengpengdd.cyou

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uoi.wangshuangyany.cn

Java: // 手写递归
来源：http://fwn.cucudq.cn

Go:   // 手写递归
来源：http://nck.snrcjt.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gel.quarkkingdee.top

C#:   // 手写递归
来源：http://hju.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://noi.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dcr.daxiang520.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://usy.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eus.jinyuanbaomall.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fnn.ydjk.org.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://miv.vqdsnc.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nce.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vlg.fzhhl.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bwu.havefunace.top

================================================================================
来源：http://rqw.52xcode.cn

O. 并发与异步
来源：http://lks.shanyushiyangkeji.top

================================================================================
来源：http://xgt.ywan-chungtsiang.top

[O01] 启动一个线程
来源：http://ghi.tarul.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mwz.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sqp.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ovy.zhiwuduotai.top

TS:   // 同 JS
来源：http://wbw.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://buo.zhaomingkeji.xyz

Go:   go f()
来源：http://mps.ehwqpu.com

Ruby: Thread.new { f }
来源：http://tcx.yj20258.top

C#:   Task.Run(() => F());
来源：http://nnq.pengpengdd.cyou

[O02] 使用线程池
来源：http://srz.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tzp.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dzm.ywan-chungtsiang.top

JS:   // worker_threads 线程池
来源：http://bcr.zycfv.cn

TS:   // worker_threads 线程池
来源：http://usx.fanxiaobao.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://jht.ehwqpu.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ejp.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zzw.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gbu.daria6918.cn

[O03] 加锁保护共享数据
来源：http://kml.gaohongyu789.top

Py:   with lock: shared += 1
来源：http://jcx.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://pwo.316326.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xit.vqdsnc.cn

TS:   // 同 JS
来源：http://ocb.fzhhl.top

Java: synchronized (this) { shared++; }
来源：http://wrx.quarkkingdee.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hvd.wangshuangyany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://njn.sufxvd.cn

C#:   lock (gate) { shared++; }
来源：http://ret.yj20258888.top

[O04] 定义异步函数并等待
来源：http://pzi.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://maw.hnxiangtu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cyi.yuxming.cn

JS:   async function f() { await g(); }
来源：http://kqx.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://eow.xinyue.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dmt.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gyb.zhiwuduotai.top

Ruby: # 用 Fiber 或 async gem
来源：http://nun.jyoumei.cn

C#:   async Task F() { await G(); }
来源：http://xbh.yj20258888.top

[O05] 并发执行并等待全部完成
来源：http://ort.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://wyv.ydjk.org.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yde.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://rbt.dashuyun.cn

TS:   await Promise.all(tasks)
来源：http://yce.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kus.jqgfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nnd.aizwys.cn

Ruby: threads.map(&:join)
来源：http://oqv.gzhubu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://evr.snrcjt.cn

[O06] 使用进程池
来源：http://yck.9152youxi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sjb.smart0.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://gjy.yuanzhike.top

JS:   // child_process / cluster 模块
来源：http://wrq.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://sdl.cqqwz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cbg.sxryk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dwy.zhongyouzk.top

Ruby: // fork 块
来源：http://hau.nanxuanxn.top

C#:   Parallel.For
来源：http://tjm.yj20258.top

================================================================================
来源：http://eum.cashguo.top

P. 常用工具函数
来源：http://tjq.gaohongyu789.top

================================================================================
来源：http://gff.snrcjt.cn

[P01] 生成 UUID
来源：http://vtt.fehbvm.com

Py:   str(uuid.uuid4())
来源：http://awt.shangyingyoupin.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rwk.daxiang520.top

JS:   crypto.randomUUID()
来源：http://bvz.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://kyp.kuanghao11.cn

Java: UUID.randomUUID().toString()
来源：http://ssp.c1oappe.top

Go:   // 用 github.com/google/uuid
来源：http://vok.xylfe.cn

Ruby: SecureRandom.uuid
来源：http://cjx.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://uzy.hysaishi.cn

[P02] MD5 / SHA256 摘要
来源：http://rtn.wangshuangyany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lxh.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ket.ivvv.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ogv.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ywm.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yca.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xtp.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nus.chenlongwang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jtk.zhengqikj.top

[P03] 生成短随机字符串
来源：http://yll.sxryk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uhc.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qex.haohaochexian.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dcn.bbcook.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ouc.yuxming.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jez.guannengcc.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ctt.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ohz.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sfm.zdqjudy.top

[P04] 求长度
来源：http://svp.jinqigfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iex.nwbrower.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bnj.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ykj.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vaq.9152youxi.cn

Java: list.size();  map.size();  s.length()
来源：http://tfz.jinqigfzy.top

Go:   len(arr);  len(m)
来源：http://jed.yuxming.cn

Ruby: x.length;  x.size
来源：http://qgd.gogol.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://glv.hammf.cn

[P05] 判断两个对象内容是否相等
来源：http://ymk.jqgufenzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uiu.yangfankeji.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mcz.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ljm.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://exc.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yrl.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://txo.shangyingyoupin.top

Ruby: a == b
来源：http://twc.andypj.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bco.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tzh.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ruc.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://lts.gogol.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hcq.gaohongyu789.top

TS:   if (x == null) {}
来源：http://rku.yanxiufei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cwk.chenlongwang.top

Go:   if x == nil {}
来源：http://qtn.tian-w.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qyt.jqgufenzy.top

C#:   if (x is null) {}
来源：http://wax.zhaomingkeji.xyz

[P07] 防抖与节流
来源：http://ugq.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xbb.jinyuanbaomall.cn

PHP:  // 手写时间戳比较
来源：http://lmj.cdnleiting.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eki.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zaa.jiagoushi.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ysh.vqdsnc.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://izk.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cfj.aibaodan.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zer.gzhubu.top

[P08] 处理浮点精度问题
来源：http://ltw.nanxuanxn.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://emb.hesvh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://azs.shanyushiyangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ies.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bbu.jlsjyb.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ttn.cqqwz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ptl.redwolf501.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ywp.yanxiufei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cqd.tian-w.cn

================================================================================
来源：http://ofx.xylfe.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mxs.fzhhl.top

================================================================================
来源：http://uuu.svipenyu.cn

[Q01] 创建表
来源：http://zct.guowangkeji.top

CREATE TABLE users (
来源：http://pmb.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lli.jinyuanbaomall.cn

name VARCHAR(50) NOT NULL,
来源：http://wiy.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://tkt.gogol.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hqr.jianghu66.top

);
来源：http://ltt.cashguo.top

[Q02] 创建带外键的表
来源：http://lwn.cqqwz.cn

CREATE TABLE orders (
来源：http://juy.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nha.fehbvm.com

user_id INT NOT NULL,
来源：http://chq.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://esq.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iyf.dianchejie.cn

);
来源：http://uyd.zhijiandao.cn

[Q03] 增加列
来源：http://inw.fehbvm.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qps.hnxiangtu.top

[Q04] 修改列类型
来源：http://ymc.jinghuilouyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cfz.iojbl.cn

[Q05] 重命名列
来源：http://vfm.snrcjt.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kku.c1oappe.top

[Q06] 删除列
来源：http://dup.shanyushiyangtech.top

ALTER TABLE users DROP COLUMN age;
来源：http://hjj.mhx1999.top

[Q07] 删除表
来源：http://czv.shzxlz.cn

DROP TABLE IF EXISTS orders;
来源：http://slo.zhoulong.xyz

[Q08] 创建普通索引
来源：http://rfv.yj202588.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vzw.hysaishi.cn

[Q09] 创建唯一索引
来源：http://ojk.andypj.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fbp.nanxinkj.top

[Q10] 插入单行
来源：http://wdk.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oxe.feifeiyinyue.top

[Q11] 一次插入多行
来源：http://wuo.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hgj.yonumen.top

[Q12] 插入后取自增 ID
来源：http://ded.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pvs.havefunace.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yic.birdmap.top

[Q13] 忽略重复插入
来源：http://lsl.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bbr.yangfankeji.com

[Q14] 存在则更新（upsert）
来源：http://jbt.vqdsnc.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://evw.tanke756.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gtb.nanxuanxn.top

[Q15] 查询全部
来源：http://zcj.zhijiandao.cn

SELECT * FROM users;
来源：http://ziu.jyoumei.cn

[Q16] 查询指定列
来源：http://jjy.iojbl.cn

SELECT id, name FROM users;
来源：http://yqz.nwbrower.top

[Q17] 条件查询
来源：http://evm.fktsv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hfo.shuidangran.top

[Q18] 模糊匹配
来源：http://myg.cheryme.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kul.fktsv.cn

[Q19] 范围查询
来源：http://uxj.yuanzhike.top


<!-- 参考信息 -->