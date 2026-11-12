代发 wailian999

TS:   process.platform;  process.version
来源：http://gkh.redwolf501.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fvi.tanke756.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ipb.zycfv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jqe.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hrs.zhixingplan.top

================================================================================
来源：http://cwx.yuxming.cn

N. 数据结构与算法
来源：http://soh.jqgufenzy.top

================================================================================
来源：http://xws.gogol.net.cn

[N01] 二分查找（有序数组）
来源：http://msr.sjlbkw.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gva.zhengqikj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://trx.shangyingyoupin.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gxa.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ssw.sweek.top

Java: Arrays.binarySearch(arr, x)
来源：http://dkl.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://vev.feifeiyinyue.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://aje.jqgufenzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://upv.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://gck.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://zyq.cqqwz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cdc.zhoulong.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://wju.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kry.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://chj.jqgfzy.top

Go:   slices.Sort(arr)
来源：http://pnd.ctjpmb.com

Ruby: arr.sort
来源：http://fbt.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tsy.sufxvd.cn

[N03] 快速排序（分治示例）
来源：http://jam.vqdsnc.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kal.jinqigfzy.top

PHP:  // 递归实现，或用 usort
来源：http://hsa.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mhb.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dgo.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://shw.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://huz.ybcxt.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kqd.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://kku.jyoumei.cn

[N04] 斐波那契数列
来源：http://dnw.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ibc.sjlbkw.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dzg.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bpn.jinyuanbaomall.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zms.pycfn.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rsw.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dob.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dwj.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pfl.cdnleiting.top

[N05] 最大公约数
来源：http://gfg.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://llw.zycfv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qyd.vehdjk.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://crx.hnxiangtu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pga.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ufk.gogol.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hen.ydzc1.top

Ruby: a.gcd(b)
来源：http://wkq.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vjv.xingfuxueyuan.xyz

[N06] 判断回文字符串
来源：http://szu.uphjek.com

Py:   s == s[::-1]
来源：http://quo.hfpthk.cn

PHP:  $s === strrev($s);
来源：http://ujp.shangyingyoupin.top

JS:   s === [...s].reverse().join("")
来源：http://nyn.redwolf501.top

TS:   s === [...s].reverse().join("")
来源：http://zcq.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wva.wangdashe.top

Go:   // 双指针从两端比较
来源：http://ntm.ybcxt.top

Ruby: s == s.reverse
来源：http://asl.uphjek.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://alu.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://wfn.gotoacloud.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vmx.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mis.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://qta.kuanghao11.cn

TS:   // 手写 Map<string, number>
来源：http://dwq.yuxming.cn

Java: // 手写 HashMap
来源：http://wml.yvedp.cn

Go:   // 手写 map[int]int
来源：http://xvg.yj20258888.top

Ruby: // 手写 Hash
来源：http://hki.vqdsnc.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xkj.redwolf501.top

[N08] 生成全排列
来源：http://qdv.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://tuk.shzxlz.cn

PHP:  // 手写递归交换
来源：http://dpc.ppjwa.cn

JS:   // 手写回溯递归
来源：http://obd.52xcode.cn

TS:   // 手写回溯递归
来源：http://esz.cheryme.top

Java: // 手写回溯递归
来源：http://ipr.ppjwa.cn

Go:   // 手写回溯递归
来源：http://wpq.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://vae.guowangkeji.top

C#:   // 手写回溯递归
来源：http://qbb.jiagoushi.top

[N09] 栈与队列
来源：http://drq.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fiv.xylfe.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ykn.316326.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ulv.epnwcf.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ojf.zhijiandao.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://prq.yonumen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uui.zhengqikj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ydt.dashuyun.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ern.zhaomingkeji.xyz

[N10] 链表节点定义
来源：http://pon.pycfn.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ape.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fcz.yuxming.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pvv.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://brt.fehbvm.com

Java: class Node { int v; Node next; }
来源：http://gcq.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://asn.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://diw.fengsongda.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mlk.smart0.xyz

[N11] 二叉树中序遍历
来源：http://nmt.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gih.shanyushiyangtech.top

PHP:  // 手写递归函数
来源：http://fzh.redwolf501.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ljg.zhixingplan.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hjn.redwolf501.top

Java: // 手写递归
来源：http://rsq.aizwys.cn

Go:   // 手写递归
来源：http://tei.fzhhl.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uih.zhoulong.xyz

C#:   // 手写递归
来源：http://fsl.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yjf.zhengqikj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mlt.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bds.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jad.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uxj.uphjek.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bgg.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gjs.hnqzz.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ioe.fktsv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lsc.ydjk.org.cn

================================================================================
来源：http://bsv.ctjpmb.com

O. 并发与异步
来源：http://kcg.zhoulong.xyz

================================================================================
来源：http://ole.xinyue.icu

[O01] 启动一个线程
来源：http://rtq.ctjpmb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lyt.cdnleiting.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zsp.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bgr.nwbrower.top

TS:   // 同 JS
来源：http://yrh.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://lna.epnwcf.com

Go:   go f()
来源：http://ywz.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://wug.zhiwuduotai.top

C#:   Task.Run(() => F());
来源：http://zge.ybcxt.top

[O02] 使用线程池
来源：http://cpq.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qwo.ydjk.org.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dxi.hywenlv.cn

JS:   // worker_threads 线程池
来源：http://cyt.chenlongwang.top

TS:   // worker_threads 线程池
来源：http://lpb.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://tar.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vca.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rat.yfazqb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pbv.316326.xyz

[O03] 加锁保护共享数据
来源：http://nde.0kj1m.cn

Py:   with lock: shared += 1
来源：http://pze.tanke756.top

PHP:  // 用 flock() 做文件锁
来源：http://tmh.zhoulong.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ahj.pycfn.com

TS:   // 同 JS
来源：http://dqh.ydjk.org.cn

Java: synchronized (this) { shared++; }
来源：http://gvm.yangfankeji.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xjf.sweek.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://iqs.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://xra.gzhubu.top

[O04] 定义异步函数并等待
来源：http://ixx.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://siq.jqgfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lan.bbcook.cn

JS:   async function f() { await g(); }
来源：http://tim.cdnleiting.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://sgi.ydjk.org.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mek.shzxlz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zba.xingfuxueyuan.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://kwo.sweek.top

C#:   async Task F() { await G(); }
来源：http://rir.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://bdb.jianghu66.top

Py:   asyncio.gather(*tasks)
来源：http://cuk.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uyx.svipenyu.cn

JS:   await Promise.all(tasks)
来源：http://swt.yonumen.top

TS:   await Promise.all(tasks)
来源：http://uuc.ppjwa.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://acf.fzhhl.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jbw.wangdashe.top

Ruby: threads.map(&:join)
来源：http://gow.xuetiantiany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zaw.redwolf501.top

[O06] 使用进程池
来源：http://cnl.sysykeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mfg.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jrd.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://kmt.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://qzu.smart0.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://noj.jqgfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hdl.hfpthk.cn

Ruby: // fork 块
来源：http://bzq.dashuyun.cn

C#:   Parallel.For
来源：http://dii.cheryme.top

================================================================================
来源：http://nnp.gotoacloud.top

P. 常用工具函数
来源：http://ueu.jinqigfzy.top

================================================================================
来源：http://ddh.hnxiangtu.top

[P01] 生成 UUID
来源：http://jml.jianghu66.top

Py:   str(uuid.uuid4())
来源：http://qml.jianghu66.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rvv.chenzaomai.com

JS:   crypto.randomUUID()
来源：http://jjv.wangdashe.top

TS:   crypto.randomUUID()
来源：http://hjn.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://fnh.9152youxi.cn

Go:   // 用 github.com/google/uuid
来源：http://vqs.ivvv.top

Ruby: SecureRandom.uuid
来源：http://pij.dashuyun.cn

C#:   Guid.NewGuid().ToString()
来源：http://aax.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://zck.zdqjudy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fwh.hnqzz.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ibb.sweek.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zkl.shzxlz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rcb.birdmap.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rqk.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://njl.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gvl.kuanghao11.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://omm.jyoumei.cn

[P03] 生成短随机字符串
来源：http://eif.ivvv.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rex.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hfu.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kao.zdbjq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aau.zhixingplan.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://esg.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wyq.aibaodan.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cte.kuanghao11.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gmj.c1oappe.top

[P04] 求长度
来源：http://gkp.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yun.ydzc1.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mon.birdmap.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fkj.birdmap.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tqz.svipenyu.cn

Java: list.size();  map.size();  s.length()
来源：http://qmb.hammf.cn

Go:   len(arr);  len(m)
来源：http://vic.shanyushiyangkeji.top

Ruby: x.length;  x.size
来源：http://kth.xziqi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gle.andypj.xyz

[P05] 判断两个对象内容是否相等
来源：http://xjj.xingfuxueyuan.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://vhf.yj20258888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gop.xziqi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://quh.dianchejie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uzw.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iva.ppjwa.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kqm.bjfxy.top

Ruby: a == b
来源：http://btn.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xbi.hcnkem.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lgy.yangfankeji.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ttv.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://phs.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dfe.sweek.top

TS:   if (x == null) {}
来源：http://irz.redwolf501.top

Java: if (x == null || x.isEmpty()) {}
来源：http://olm.wangshuangyany.cn

Go:   if x == nil {}
来源：http://iga.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oqg.cqqwz.cn

C#:   if (x is null) {}
来源：http://lww.chenzaomai.com

[P07] 防抖与节流
来源：http://ggc.316326.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fxb.guowangkeji.top

PHP:  // 手写时间戳比较
来源：http://foy.nanxuanxn.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://haa.shangyingyoupin.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aty.ydzc1.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xrx.quarkkingdee.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tve.tian-w.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oyo.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://htf.fanxiaobao.xyz

[P08] 处理浮点精度问题
来源：http://vjm.zhoulong.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kkb.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ehl.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://syt.aibaodan.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tkx.chenlongwang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ufh.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rdo.jyoumei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ykc.fktsv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pjf.chenzaomai.com

================================================================================
来源：http://ipx.aizwys.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nkc.ehwqpu.com

================================================================================
来源：http://faj.jinqigfzy.top

[Q01] 创建表
来源：http://qfp.cashguo.top

CREATE TABLE users (
来源：http://bso.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ymf.52xcode.cn

name VARCHAR(50) NOT NULL,
来源：http://ovk.nanxuanxn.top

email VARCHAR(100) UNIQUE,
来源：http://wgg.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://urk.chenzaomai.com

);
来源：http://qax.tanke756.top

[Q02] 创建带外键的表
来源：http://wsd.xziqi.cn

CREATE TABLE orders (
来源：http://jag.jqgufenzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ezc.yuxming.cn

user_id INT NOT NULL,
来源：http://czm.xuanzx.com

amount DECIMAL(10, 2),
来源：http://dyp.wangshuangyany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xsq.yuanzhike.top

);
来源：http://qwj.9152youxi.cn

[Q03] 增加列
来源：http://jye.zycfv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ijx.yonumen.top

[Q04] 修改列类型
来源：http://ldj.gzhubu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rtr.sysykeji.top

[Q05] 重命名列
来源：http://oox.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://viv.yfazqb.com

[Q06] 删除列
来源：http://tum.havefunace.top

ALTER TABLE users DROP COLUMN age;
来源：http://bpy.sxryk.cn

[Q07] 删除表
来源：http://zlj.ydjk.org.cn

DROP TABLE IF EXISTS orders;
来源：http://gci.smart0.xyz

[Q08] 创建普通索引
来源：http://vqw.daxiang520.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wae.xylfe.cn

[Q09] 创建唯一索引
来源：http://kyr.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dwo.hysaishi.cn

[Q10] 插入单行
来源：http://eoh.9152youxi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dio.bjfxy.top

[Q11] 一次插入多行
来源：http://yer.zycfv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jax.shanyushiyangtech.top

[Q12] 插入后取自增 ID
来源：http://xtl.guannengcc.top

INSERT INTO users (name) VALUES ('C');
来源：http://sfm.smart0.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mry.cucudq.cn

[Q13] 忽略重复插入
来源：http://cen.9152youxi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cfe.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://qqq.zhoulong.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hbw.zycfv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vex.ppjwa.cn

[Q15] 查询全部
来源：http://var.shuidangran.top

SELECT * FROM users;
来源：http://yba.hesvh.cn

[Q16] 查询指定列
来源：http://cmm.shuidangran.top

SELECT id, name FROM users;
来源：http://rth.xuetiantiany.cn

[Q17] 条件查询
来源：http://zed.sysykeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hqt.kuanghao11.cn

[Q18] 模糊匹配
来源：http://iss.nanxinkj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gze.bjfxy.top

[Q19] 范围查询
来源：http://hiy.jiagoushi.top


<!-- 参考信息 -->