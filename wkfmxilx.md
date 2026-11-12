代发 wailian999

TS:   process.platform;  process.version
来源：http://gge.bbcook.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bnw.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nxg.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nnn.zycfv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yva.chenlongwang.top

================================================================================
来源：http://zkg.chenlongwang.top

N. 数据结构与算法
来源：http://xjk.hnxiangtu.top

================================================================================
来源：http://ihm.cheryme.top

[N01] 二分查找（有序数组）
来源：http://han.zhongyouzk.top

Py:   bisect.bisect_left(arr, x)
来源：http://yrq.meibo888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://taj.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dmb.yj20258888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bnr.nwbrower.top

Java: Arrays.binarySearch(arr, x)
来源：http://nib.ydzc1.top

Go:   sort.SearchInts(arr, x)
来源：http://fza.aibaodan.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xni.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://lqn.yj20258888.top

[N02] 排序（工程实践用内置实现）
来源：http://onr.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://niy.shangyingyoupin.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://luh.cqqwz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://olm.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sth.havefunace.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gxp.ppjwa.cn

Go:   slices.Sort(arr)
来源：http://efp.jiagoushi.top

Ruby: arr.sort
来源：http://nmp.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lkm.yuxming.cn

[N03] 快速排序（分治示例）
来源：http://ntq.feifeiyinyue.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sxg.gotoacloud.top

PHP:  // 递归实现，或用 usort
来源：http://pyq.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://moh.meibo888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://klk.jinqigufen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uef.vqdsnc.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ory.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qpa.yonumen.top

C#:   // 手写递归，或 Array.Sort
来源：http://muw.kuanghao11.cn

[N04] 斐波那契数列
来源：http://hko.fengsongda.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hub.zdbjq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ejv.bbcook.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fod.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jgm.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jlv.jyoumei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tuo.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ngm.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dnb.yfazqb.com

[N05] 最大公约数
来源：http://pek.hcnkem.com

Py:   math.gcd(a, b)
来源：http://zjt.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qtm.52xcode.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://twf.hnxiangtu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ksi.mhx1999.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://abj.sjlbkw.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://klh.sysykeji.top

Ruby: a.gcd(b)
来源：http://hcm.jinqigufen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://euv.cashguo.top

[N06] 判断回文字符串
来源：http://bit.iojbl.cn

Py:   s == s[::-1]
来源：http://uts.yj20258888.top

PHP:  $s === strrev($s);
来源：http://smc.vqdsnc.cn

JS:   s === [...s].reverse().join("")
来源：http://mpy.birdmap.top

TS:   s === [...s].reverse().join("")
来源：http://wxj.jinghuilouyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://svd.sysykeji.top

Go:   // 双指针从两端比较
来源：http://iuo.smart0.xyz

Ruby: s == s.reverse
来源：http://lnj.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zmt.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://rdo.yuxming.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cbu.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tdk.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ixv.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://fgc.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://uhk.cucudq.cn

Go:   // 手写 map[int]int
来源：http://ihm.nanxuanxn.top

Ruby: // 手写 Hash
来源：http://kbm.yanxiufei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ejc.xuanzx.com

[N08] 生成全排列
来源：http://rci.vehdjk.com

Py:   itertools.permutations(arr)
来源：http://vry.yvedp.cn

PHP:  // 手写递归交换
来源：http://sev.smart0.xyz

JS:   // 手写回溯递归
来源：http://ugc.fehbvm.com

TS:   // 手写回溯递归
来源：http://zes.hesvh.cn

Java: // 手写回溯递归
来源：http://prn.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://nnt.uphjek.com

Ruby: arr.permutation.to_a
来源：http://sxj.feifeiyinyue.top

C#:   // 手写回溯递归
来源：http://nbb.uphjek.com

[N09] 栈与队列
来源：http://aci.sysykeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xsq.andypj.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bxy.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fmc.havefunace.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sag.yanxiufei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kcr.316326.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kzx.shanyushiyangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cmp.52xcode.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dfg.xinyue.icu

[N10] 链表节点定义
来源：http://kdt.wangshuangyany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lxv.9152youxi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bhp.nanxuanxn.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xyt.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eub.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://pwc.hfpthk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qyt.zdqjudy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://orn.sxryk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fym.xziqi.cn

[N11] 二叉树中序遍历
来源：http://jjp.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://imy.xingfuxueyuan.xyz

PHP:  // 手写递归函数
来源：http://hkm.zhiwuduotai.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mqk.havefunace.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jfx.gzhubu.top

Java: // 手写递归
来源：http://hjj.jyoumei.cn

Go:   // 手写递归
来源：http://aij.yfazqb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aaz.hysaishi.cn

C#:   // 手写递归
来源：http://qrw.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qcu.vqdsnc.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rtd.guowangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qgy.svipenyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://esv.shanyushiyangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://asr.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://obr.ydjk.org.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ovz.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lrf.xylfe.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wxv.c1oappe.top

================================================================================
来源：http://oxx.shanyushiyangkeji.top

O. 并发与异步
来源：http://cpm.c1oappe.top

================================================================================
来源：http://zvh.yfazqb.com

[O01] 启动一个线程
来源：http://uzh.dashuyun.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mng.aibaodan.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xwu.chenzaomai.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lrq.zycfv.cn

TS:   // 同 JS
来源：http://bqt.gogol.net.cn

Java: new Thread(() -> f()).start()
来源：http://sxp.zhijiandao.cn

Go:   go f()
来源：http://pkz.tanke756.top

Ruby: Thread.new { f }
来源：http://sik.yonumen.top

C#:   Task.Run(() => F());
来源：http://rgg.yj20258.top

[O02] 使用线程池
来源：http://tpj.sweek.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mef.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kpb.hesvh.cn

JS:   // worker_threads 线程池
来源：http://nwc.yuxming.cn

TS:   // worker_threads 线程池
来源：http://szn.52xcode.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bhn.ywan-chungtsiang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://emg.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pxo.dashuyun.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yoc.zycfv.cn

[O03] 加锁保护共享数据
来源：http://bbp.vehdjk.com

Py:   with lock: shared += 1
来源：http://cot.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://xzy.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mri.hongshengwenyu.top

TS:   // 同 JS
来源：http://rhe.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://cyp.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hww.shanyushiyangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://sbx.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://tzv.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://wcr.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://yhi.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lyb.ybcxt.top

JS:   async function f() { await g(); }
来源：http://sek.yangfankeji.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://miu.quarkkingdee.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ysc.jqgufenzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iuq.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://fng.jinqigfzy.top

C#:   async Task F() { await G(); }
来源：http://fep.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://psf.xingfuxueyuan.xyz

Py:   asyncio.gather(*tasks)
来源：http://jtn.jinqigfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bge.chenjidiqi.icu

JS:   await Promise.all(tasks)
来源：http://uba.dashuyun.cn

TS:   await Promise.all(tasks)
来源：http://bre.epnwcf.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nmk.jyoumei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zie.hfpthk.cn

Ruby: threads.map(&:join)
来源：http://pfy.hammf.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hbj.zhixingplan.top

[O06] 使用进程池
来源：http://ame.havefunace.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://daa.hnqzz.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qdo.0kj1m.cn

JS:   // child_process / cluster 模块
来源：http://txh.hongshengwenyu.top

TS:   // child_process / cluster 模块
来源：http://ohd.vehdjk.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://skt.yangfankeji.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cjr.shanyushiyangtech.top

Ruby: // fork 块
来源：http://jyz.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://mhk.fengsongda.top

================================================================================
来源：http://lid.hysaishi.cn

P. 常用工具函数
来源：http://vgt.bbcook.cn

================================================================================
来源：http://ovr.hammf.cn

[P01] 生成 UUID
来源：http://dsc.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://qmn.aizwys.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fkw.smart0.xyz

JS:   crypto.randomUUID()
来源：http://oww.hnxiangtu.top

TS:   crypto.randomUUID()
来源：http://jpn.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://ghh.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://moa.yangfankeji.com

Ruby: SecureRandom.uuid
来源：http://ril.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://uak.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://rvo.daria6918.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wze.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ejv.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rws.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cyj.guannengcc.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xza.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qhl.svipenyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wir.ydzc1.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wjm.jlsjyb.cn

[P03] 生成短随机字符串
来源：http://jsc.hesvh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tmp.dashuyun.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xmm.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cru.xingfuxueyuan.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zyq.hnxiangtu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gwa.guowangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hct.yueranfly.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jlq.jianghu66.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nsx.cashguo.top

[P04] 求长度
来源：http://ljr.zhengqikj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nkh.nanxinkj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fcj.svipenyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iiq.haohaochexian.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dvv.nanxinkj.top

Java: list.size();  map.size();  s.length()
来源：http://mjv.birdmap.top

Go:   len(arr);  len(m)
来源：http://ipp.316326.xyz

Ruby: x.length;  x.size
来源：http://qzv.jqgufenzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dyq.yfazqb.com

[P05] 判断两个对象内容是否相等
来源：http://ymx.zhijiandao.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ndr.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lct.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jqh.ivvv.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://del.pycfn.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hvd.fanxiaobao.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://whs.jlsjyb.cn

Ruby: a == b
来源：http://unz.daria6918.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lwl.tianlin.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gwv.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dnk.sxryk.cn

PHP:  if (empty($x)) {}
来源：http://bbd.zhoulong.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ceh.hongshengwenyu.top

TS:   if (x == null) {}
来源：http://cac.aibaodan.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fmk.hnxiangtu.top

Go:   if x == nil {}
来源：http://nek.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vph.quarkkingdee.top

C#:   if (x is null) {}
来源：http://wqe.shanyushiyangtech.top

[P07] 防抖与节流
来源：http://xqx.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zqt.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://srd.redwolf501.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vtr.epnwcf.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ppc.zdbjq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hzo.zdbjq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fvx.snrcjt.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cja.cdnleiting.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nmb.meibo888.top

[P08] 处理浮点精度问题
来源：http://pgo.xylfe.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lsw.vehdjk.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://msx.hongshengwenyu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mhc.guowangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rdz.cashguo.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iik.guannengcc.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ltp.yanxiufei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gxu.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qzs.fengsongda.top

================================================================================
来源：http://lzm.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iyf.52xcode.cn

================================================================================
来源：http://czw.shzxlz.cn

[Q01] 创建表
来源：http://yon.gaohongyu789.top

CREATE TABLE users (
来源：http://tht.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dqn.tarul.cn

name VARCHAR(50) NOT NULL,
来源：http://msx.hnxiangtu.top

email VARCHAR(100) UNIQUE,
来源：http://idu.chenjidiqi.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aqd.epnwcf.com

);
来源：http://enf.zhijiandao.cn

[Q02] 创建带外键的表
来源：http://mhv.zhiwuduotai.top

CREATE TABLE orders (
来源：http://src.redwolf501.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ffc.zhoulong.xyz

user_id INT NOT NULL,
来源：http://ilp.zhengqikj.top

amount DECIMAL(10, 2),
来源：http://ubl.xuetiantiany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yne.yuxming.cn

);
来源：http://sms.meibo888.top

[Q03] 增加列
来源：http://bnx.yongpay.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yfs.yj202588.top

[Q04] 修改列类型
来源：http://htw.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hrc.gogol.net.cn

[Q05] 重命名列
来源：http://cel.xylfe.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://smn.ybcxt.top

[Q06] 删除列
来源：http://sth.fehbvm.com

ALTER TABLE users DROP COLUMN age;
来源：http://rin.xuanzx.com

[Q07] 删除表
来源：http://ygg.gogol.net.cn

DROP TABLE IF EXISTS orders;
来源：http://jmi.tianlin.xyz

[Q08] 创建普通索引
来源：http://mvk.yonumen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://plp.gotoacloud.top

[Q09] 创建唯一索引
来源：http://cui.yueranfly.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://liv.guowangkeji.top

[Q10] 插入单行
来源：http://uek.jqgfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vgo.yueranfly.top

[Q11] 一次插入多行
来源：http://xzg.jianghu66.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ayh.fzhhl.top

[Q12] 插入后取自增 ID
来源：http://ikb.yfazqb.com

INSERT INTO users (name) VALUES ('C');
来源：http://bqo.hesvh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nij.shzxlz.cn

[Q13] 忽略重复插入
来源：http://nci.yanxiufei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pav.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://avb.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tuh.tianlin.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gxo.xuanzx.com

[Q15] 查询全部
来源：http://aln.ywan-chungtsiang.top

SELECT * FROM users;
来源：http://ejt.xziqi.cn

[Q16] 查询指定列
来源：http://zvo.zdbjq.cn

SELECT id, name FROM users;
来源：http://xsh.iojbl.cn

[Q17] 条件查询
来源：http://qkf.redwolf501.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fbe.kuanghao11.cn

[Q18] 模糊匹配
来源：http://rag.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yjl.bjfxy.top

[Q19] 范围查询
来源：http://lcq.cheryme.top


<!-- 参考信息 -->