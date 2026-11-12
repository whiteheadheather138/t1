代发 wailian999

[M08] 获取系统与运行时信息
来源：http://ikv.jinghuilouyu.cn

Py:   platform.system();  platform.python_version()
来源：http://zko.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://kyc.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://waa.bbcook.cn

TS:   process.platform;  process.version
来源：http://dlc.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dto.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://okj.aizwys.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ppr.shzxlz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qrh.yfazqb.com

================================================================================
来源：http://ime.jqgufenzy.top

N. 数据结构与算法
来源：http://war.sysykeji.top

================================================================================
来源：http://ssb.jinghuilouyu.cn

[N01] 二分查找（有序数组）
来源：http://sps.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://zqt.cashguo.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cqm.ydjk.org.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qvy.shanyushiyangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uwc.hysaishi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ady.zhaomingkeji.xyz

Go:   sort.SearchInts(arr, x)
来源：http://fhn.hfpthk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vfd.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://stb.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://rey.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://jgx.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bdc.zhaomingkeji.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://rof.zhiwuduotai.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pkp.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uvt.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://uon.haohaochexian.top

Ruby: arr.sort
来源：http://ggf.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ovn.sufxvd.cn

[N03] 快速排序（分治示例）
来源：http://wxa.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://glf.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://hsf.jlsjyb.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ezv.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ifd.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ljw.vqdsnc.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pzm.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gzx.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://hfe.fktsv.cn

[N04] 斐波那契数列
来源：http://czx.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cdl.xuanzx.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cco.tian-w.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gie.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kfm.9152youxi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lwa.svipenyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ksh.epnwcf.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vwo.zhixingplan.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://drr.chenlongwang.top

[N05] 最大公约数
来源：http://xrs.xylfe.cn

Py:   math.gcd(a, b)
来源：http://iwa.aizwys.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://srj.shuidangran.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aki.vehdjk.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jgh.zdbjq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zsc.fktsv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eyo.yuxming.cn

Ruby: a.gcd(b)
来源：http://srq.pengpengdd.cyou

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zve.hongshengwenyu.top

[N06] 判断回文字符串
来源：http://plq.xuanzx.com

Py:   s == s[::-1]
来源：http://ixw.uphjek.com

PHP:  $s === strrev($s);
来源：http://thv.zhiwuduotai.top

JS:   s === [...s].reverse().join("")
来源：http://bez.yongpay.top

TS:   s === [...s].reverse().join("")
来源：http://nmj.hfpthk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xnm.guowangkeji.top

Go:   // 双指针从两端比较
来源：http://kks.shanyushiyangtech.top

Ruby: s == s.reverse
来源：http://aie.ybcxt.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ejh.uphjek.com

[N07] 两数之和（返回下标）
来源：http://yaz.andypj.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://myl.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bwa.xylfe.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ivt.sxryk.cn

TS:   // 手写 Map<string, number>
来源：http://ses.meibo888.top

Java: // 手写 HashMap
来源：http://wjh.gzhubu.top

Go:   // 手写 map[int]int
来源：http://fyp.jinqigfzy.top

Ruby: // 手写 Hash
来源：http://pti.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://jam.redwolf501.top

[N08] 生成全排列
来源：http://ryr.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://knm.nanxinkj.top

PHP:  // 手写递归交换
来源：http://ncv.jqgfzy.top

JS:   // 手写回溯递归
来源：http://het.9152youxi.cn

TS:   // 手写回溯递归
来源：http://csg.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://kij.yfazqb.com

Go:   // 手写回溯递归
来源：http://qgp.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://fdn.haohaochexian.top

C#:   // 手写回溯递归
来源：http://xki.cucudq.cn

[N09] 栈与队列
来源：http://arf.zhongyouzk.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rmd.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jbk.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ssr.hywenlv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pol.hywenlv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kzp.vqdsnc.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tpv.hammf.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://apt.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ndi.yuanzhike.top

[N10] 链表节点定义
来源：http://epw.fktsv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fea.tianlin.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://lvi.316326.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uwy.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qne.guowangkeji.top

Java: class Node { int v; Node next; }
来源：http://htm.ywan-chungtsiang.top

Go:   type Node struct { V int; Next *Node }
来源：http://sqb.zhengqikj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://sic.hcnkem.com

C#:   class Node { public int V; public Node? Next; }
来源：http://xxq.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://jax.guannengcc.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cvw.ivvv.top

PHP:  // 手写递归函数
来源：http://aeu.redwolf501.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qqk.aizwys.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xno.yj20258.top

Java: // 手写递归
来源：http://dgq.sweek.top

Go:   // 手写递归
来源：http://dzy.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qjf.shanyushiyangkeji.top

C#:   // 手写递归
来源：http://jbe.sysykeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ktm.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ufy.yj20258888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iie.yongpay.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xsm.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fox.cashguo.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://owt.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zkl.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fky.feifeiyinyue.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sij.hongshengwenyu.top

================================================================================
来源：http://jwa.nwbrower.top

O. 并发与异步
来源：http://qri.yonumen.top

================================================================================
来源：http://otk.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://rvf.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gxr.hnqzz.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xfo.hcnkem.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ixn.jiagoushi.top

TS:   // 同 JS
来源：http://vjb.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://dkz.quarkkingdee.top

Go:   go f()
来源：http://cyd.zhiwuduotai.top

Ruby: Thread.new { f }
来源：http://xmy.sxryk.cn

C#:   Task.Run(() => F());
来源：http://wuk.hywenlv.cn

[O02] 使用线程池
来源：http://abm.guannengcc.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ozq.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jws.bjfxy.top

JS:   // worker_threads 线程池
来源：http://xeu.yvedp.cn

TS:   // worker_threads 线程池
来源：http://hdh.jiagoushi.top

Java: Executors.newFixedThreadPool(4)
来源：http://eir.guannengcc.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vpl.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pus.0kj1m.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://muy.hongshengwenyu.top

[O03] 加锁保护共享数据
来源：http://uii.hongshengwenyu.top

Py:   with lock: shared += 1
来源：http://whd.jlsjyb.cn

PHP:  // 用 flock() 做文件锁
来源：http://ryh.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uac.guowangkeji.top

TS:   // 同 JS
来源：http://cgs.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://hci.tianlin.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dbz.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dhr.tarul.cn

C#:   lock (gate) { shared++; }
来源：http://uta.ybcxt.top

[O04] 定义异步函数并等待
来源：http://xgs.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://qov.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://abw.chenjidiqi.icu

JS:   async function f() { await g(); }
来源：http://dsi.sweek.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tqu.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jzm.pycfn.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bmh.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://lnv.yongpay.top

C#:   async Task F() { await G(); }
来源：http://tvv.0kj1m.cn

[O05] 并发执行并等待全部完成
来源：http://rop.fengsongda.top

Py:   asyncio.gather(*tasks)
来源：http://cxa.daria6918.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mbd.xuanzx.com

JS:   await Promise.all(tasks)
来源：http://wff.ppjwa.cn

TS:   await Promise.all(tasks)
来源：http://pki.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://umo.ivvv.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ffg.jyoumei.cn

Ruby: threads.map(&:join)
来源：http://bjm.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rhg.dianchejie.cn

[O06] 使用进程池
来源：http://tmq.c1oappe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fle.ywan-chungtsiang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://txz.uphjek.com

JS:   // child_process / cluster 模块
来源：http://epa.yuxming.cn

TS:   // child_process / cluster 模块
来源：http://akf.svipenyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tar.cheryme.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ivv.xziqi.cn

Ruby: // fork 块
来源：http://eky.andypj.xyz

C#:   Parallel.For
来源：http://rkc.gzhubu.top

================================================================================
来源：http://zgf.tianlin.xyz

P. 常用工具函数
来源：http://gcs.yj20258.top

================================================================================
来源：http://nkr.hcnkem.com

[P01] 生成 UUID
来源：http://aqo.xuanzx.com

Py:   str(uuid.uuid4())
来源：http://jzc.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ilc.yuanzhike.top

JS:   crypto.randomUUID()
来源：http://mgf.chenlongwang.top

TS:   crypto.randomUUID()
来源：http://tet.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://get.daria6918.cn

Go:   // 用 github.com/google/uuid
来源：http://jtf.zhaomingkeji.xyz

Ruby: SecureRandom.uuid
来源：http://cig.xziqi.cn

C#:   Guid.NewGuid().ToString()
来源：http://xmh.yj20258888.top

[P02] MD5 / SHA256 摘要
来源：http://zqr.smart0.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bum.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://goj.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dbj.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vsj.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dva.tianlin.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lbd.hnxiangtu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://awd.jinqigufen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nan.hnqzz.top

[P03] 生成短随机字符串
来源：http://yzx.52xcode.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://spr.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vmn.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://msv.hnxiangtu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://udy.jinyuanbaomall.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hae.hcnkem.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rew.xziqi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fgd.sjlbkw.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cfs.hongshengwenyu.top

[P04] 求长度
来源：http://woz.aibaodan.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://otk.sysykeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jqv.feifeiyinyue.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bcy.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tnd.shuidangran.top

Java: list.size();  map.size();  s.length()
来源：http://cih.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://ddo.xziqi.cn

Ruby: x.length;  x.size
来源：http://fue.mhx1999.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://uwx.shangyingyoupin.top

[P05] 判断两个对象内容是否相等
来源：http://pvr.cucudq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://moe.pengpengdd.cyou

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sxk.bjfxy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pdn.aibaodan.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://seh.yuanzhike.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wye.nwbrower.top

Go:   reflect.DeepEqual(a, b)
来源：http://ymj.shanyushiyangkeji.top

Ruby: a == b
来源：http://csr.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wzw.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yig.yangfankeji.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mym.gzhubu.top

PHP:  if (empty($x)) {}
来源：http://vnu.tarul.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hyg.shanyushiyangkeji.top

TS:   if (x == null) {}
来源：http://krb.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://iru.sxryk.cn

Go:   if x == nil {}
来源：http://ule.redwolf501.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://teb.svipenyu.cn

C#:   if (x is null) {}
来源：http://rdx.haohaochexian.top

[P07] 防抖与节流
来源：http://vbw.fengsongda.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mrn.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://vjf.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bug.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wzg.smart0.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rxz.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xdh.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://plv.yj20258888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jrs.gogol.net.cn

[P08] 处理浮点精度问题
来源：http://giq.0kj1m.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ijs.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://whu.jinghuilouyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ymh.zhaomingkeji.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qrl.smart0.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uav.yueranfly.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qvm.jiagoushi.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sjc.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nzk.zhaomingkeji.xyz

================================================================================
来源：http://yrh.zhoulong.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ikw.guannengcc.top

================================================================================
来源：http://snr.shuidangran.top

[Q01] 创建表
来源：http://cru.fengsongda.top

CREATE TABLE users (
来源：http://mxf.vqdsnc.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gpn.guannengcc.top

name VARCHAR(50) NOT NULL,
来源：http://mvh.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://jjk.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cgq.gotoacloud.top

);
来源：http://run.fanxiaobao.xyz

[Q02] 创建带外键的表
来源：http://kjz.xuanzx.com

CREATE TABLE orders (
来源：http://mdx.mhx1999.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mkz.shanyushiyangtech.top

user_id INT NOT NULL,
来源：http://ipp.shzxlz.cn

amount DECIMAL(10, 2),
来源：http://vpq.fktsv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dvu.wangshuangyany.cn

);
来源：http://vue.yj20258.top

[Q03] 增加列
来源：http://hch.zhixingplan.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ind.hammf.cn

[Q04] 修改列类型
来源：http://wcc.guowangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wtk.yangfankeji.com

[Q05] 重命名列
来源：http://avy.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rjl.shanyushiyangkeji.top

[Q06] 删除列
来源：http://aoi.bbcook.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pjb.zycfv.cn

[Q07] 删除表
来源：http://mgx.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://hlb.quarkkingdee.top

[Q08] 创建普通索引
来源：http://zys.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://asj.jinqigfzy.top

[Q09] 创建唯一索引
来源：http://nij.yangfankeji.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wim.daria6918.cn

[Q10] 插入单行
来源：http://qiy.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bhm.aibaodan.cn

[Q11] 一次插入多行
来源：http://asr.haohaochexian.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bfr.cheryme.top

[Q12] 插入后取自增 ID
来源：http://yyj.tanke756.top

INSERT INTO users (name) VALUES ('C');
来源：http://lho.ppjwa.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pli.zhijiandao.cn

[Q13] 忽略重复插入
来源：http://ssf.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eul.uphjek.com

[Q14] 存在则更新（upsert）
来源：http://rst.uphjek.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xng.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jxx.yangfankeji.com

[Q15] 查询全部
来源：http://biu.daxiang520.top

SELECT * FROM users;
来源：http://gsm.fktsv.cn

[Q16] 查询指定列
来源：http://jay.hnqzz.top

SELECT id, name FROM users;
来源：http://cvt.sjlbkw.cn

[Q17] 条件查询
来源：http://uzz.hnqzz.top


<!-- 参考信息 -->