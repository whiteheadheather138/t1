代发 wailian999

TS:   process.platform;  process.version
来源：http://yzi.jlsjyb.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hcj.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://ips.zhijiandao.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pgt.fengsongda.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://adl.quarkkingdee.top

================================================================================
来源：http://npq.shanyushiyangkeji.top

N. 数据结构与算法
来源：http://rji.daxiang520.top

================================================================================
来源：http://opv.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://owj.zhongyouzk.top

Py:   bisect.bisect_left(arr, x)
来源：http://etl.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fkk.zdbjq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uok.zhengqikj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ysu.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cgs.316326.xyz

Go:   sort.SearchInts(arr, x)
来源：http://vpd.yfazqb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://kjl.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ixo.yj202588.top

[N02] 排序（工程实践用内置实现）
来源：http://isl.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://yan.9152youxi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://luz.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ppq.aizwys.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nrh.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rsp.cucudq.cn

Go:   slices.Sort(arr)
来源：http://bwe.yj20258888.top

Ruby: arr.sort
来源：http://pin.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://jeh.yanxiufei.cn

[N03] 快速排序（分治示例）
来源：http://xac.yanxiufei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://chc.hcnkem.com

PHP:  // 递归实现，或用 usort
来源：http://voh.fehbvm.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dfz.ydjk.org.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nkp.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xdb.yangfankeji.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://soh.jinqigfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qsr.pengpengdd.cyou

C#:   // 手写递归，或 Array.Sort
来源：http://fnn.zhaomingkeji.xyz

[N04] 斐波那契数列
来源：http://eki.jiagoushi.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://isi.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gkv.ydjk.org.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rxs.shanyushiyangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dtk.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ecd.andypj.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ozc.xylfe.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gky.316326.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mtx.shuidangran.top

[N05] 最大公约数
来源：http://naw.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://tnp.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uov.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://azg.fzhhl.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fyu.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ujn.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iag.zhongyouzk.top

Ruby: a.gcd(b)
来源：http://boc.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sfe.52xcode.cn

[N06] 判断回文字符串
来源：http://rnf.havefunace.top

Py:   s == s[::-1]
来源：http://gsr.tianlin.xyz

PHP:  $s === strrev($s);
来源：http://akh.yongpay.top

JS:   s === [...s].reverse().join("")
来源：http://wpm.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://biu.svipenyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xzk.havefunace.top

Go:   // 双指针从两端比较
来源：http://hjl.xylfe.cn

Ruby: s == s.reverse
来源：http://gsx.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ysu.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://zdl.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dgz.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kbu.bjfxy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://lid.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://wdf.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://qvg.ivvv.top

Go:   // 手写 map[int]int
来源：http://aqp.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://aiu.hcnkem.com

C#:   // 手写 Dictionary<int, int>
来源：http://bay.mhx1999.top

[N08] 生成全排列
来源：http://piu.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://qdj.9152youxi.cn

PHP:  // 手写递归交换
来源：http://uif.tianlin.xyz

JS:   // 手写回溯递归
来源：http://bqt.zycfv.cn

TS:   // 手写回溯递归
来源：http://pas.yuanzhike.top

Java: // 手写回溯递归
来源：http://wgo.ywan-chungtsiang.top

Go:   // 手写回溯递归
来源：http://fma.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://fzs.tian-w.cn

C#:   // 手写回溯递归
来源：http://tjl.hywenlv.cn

[N09] 栈与队列
来源：http://qcr.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://quw.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rde.zycfv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mvn.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wqn.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gns.shangyingyoupin.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://txd.hammf.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mho.pengpengdd.cyou

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bhm.daria6918.cn

[N10] 链表节点定义
来源：http://lmb.ehwqpu.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rks.yonumen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mie.iojbl.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mne.shzxlz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pxx.zhixingplan.top

Java: class Node { int v; Node next; }
来源：http://qkc.vehdjk.com

Go:   type Node struct { V int; Next *Node }
来源：http://xzv.hnxiangtu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ebm.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ydv.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://dyu.ehwqpu.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jnf.nanxuanxn.top

PHP:  // 手写递归函数
来源：http://qdm.jinqigufen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xil.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ikh.zhiwuduotai.top

Java: // 手写递归
来源：http://zvk.yonumen.top

Go:   // 手写递归
来源：http://yfk.fzhhl.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ijq.tanke756.top

C#:   // 手写递归
来源：http://xtz.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ogf.kuanghao11.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yjb.316326.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xva.zhaomingkeji.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gob.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://usf.shuidangran.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lht.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oxh.zhijiandao.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fio.zhiwuduotai.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://veb.gotoacloud.top

================================================================================
来源：http://xft.yvedp.cn

O. 并发与异步
来源：http://bhs.316326.xyz

================================================================================
来源：http://wuf.sysykeji.top

[O01] 启动一个线程
来源：http://ybu.pycfn.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sts.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ibx.yongpay.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sso.hnxiangtu.top

TS:   // 同 JS
来源：http://kan.ctjpmb.com

Java: new Thread(() -> f()).start()
来源：http://vim.yangfankeji.com

Go:   go f()
来源：http://qpt.cqqwz.cn

Ruby: Thread.new { f }
来源：http://eix.meibo888.top

C#:   Task.Run(() => F());
来源：http://ukg.jinghuilouyu.cn

[O02] 使用线程池
来源：http://els.smart0.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yol.zhixingplan.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mbn.bbcook.cn

JS:   // worker_threads 线程池
来源：http://sup.hesvh.cn

TS:   // worker_threads 线程池
来源：http://nml.52xcode.cn

Java: Executors.newFixedThreadPool(4)
来源：http://csq.aizwys.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mbx.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xdg.andypj.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qju.zdqjudy.top

[O03] 加锁保护共享数据
来源：http://fmg.zhongyouzk.top

Py:   with lock: shared += 1
来源：http://wex.jqgufenzy.top

PHP:  // 用 flock() 做文件锁
来源：http://uhh.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rep.sysykeji.top

TS:   // 同 JS
来源：http://qzh.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://zpf.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://luu.wangshuangyany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://une.sxryk.cn

C#:   lock (gate) { shared++; }
来源：http://eci.yj202588.top

[O04] 定义异步函数并等待
来源：http://tkp.fehbvm.com

Py:   async def f():⏎    await g()
来源：http://pkb.sxryk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gne.zycfv.cn

JS:   async function f() { await g(); }
来源：http://juh.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://esp.yuxming.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pyg.jqgufenzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gpf.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://chz.zhaomingkeji.xyz

C#:   async Task F() { await G(); }
来源：http://uel.chenlongwang.top

[O05] 并发执行并等待全部完成
来源：http://vis.yfazqb.com

Py:   asyncio.gather(*tasks)
来源：http://bbi.zhongyouzk.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://las.yueranfly.top

JS:   await Promise.all(tasks)
来源：http://oxf.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://mfl.yongpay.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://exh.kuanghao11.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lpm.hammf.cn

Ruby: threads.map(&:join)
来源：http://yse.xinyue.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://dgk.xinyue.icu

[O06] 使用进程池
来源：http://tps.smart0.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wvi.sxryk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nhh.ppjwa.cn

JS:   // child_process / cluster 模块
来源：http://say.fehbvm.com

TS:   // child_process / cluster 模块
来源：http://aby.xylfe.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jkj.tian-w.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://feg.zhiwuduotai.top

Ruby: // fork 块
来源：http://iav.havefunace.top

C#:   Parallel.For
来源：http://tbc.cashguo.top

================================================================================
来源：http://wii.yonumen.top

P. 常用工具函数
来源：http://ubq.sxryk.cn

================================================================================
来源：http://fbo.quarkkingdee.top

[P01] 生成 UUID
来源：http://wxf.jlsjyb.cn

Py:   str(uuid.uuid4())
来源：http://mkh.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fgn.hammf.cn

JS:   crypto.randomUUID()
来源：http://zdb.mhx1999.top

TS:   crypto.randomUUID()
来源：http://ziv.jlsjyb.cn

Java: UUID.randomUUID().toString()
来源：http://ihs.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://cod.zhengqikj.top

Ruby: SecureRandom.uuid
来源：http://tck.sxryk.cn

C#:   Guid.NewGuid().ToString()
来源：http://dqk.svipenyu.cn

[P02] MD5 / SHA256 摘要
来源：http://kua.yongpay.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://opu.nanxuanxn.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://khc.tianlin.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eso.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gga.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://myi.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lta.cucudq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rnu.daxiang520.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ctq.aizwys.cn

[P03] 生成短随机字符串
来源：http://cas.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xvm.feifeiyinyue.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iqd.jinqigufen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dim.zycfv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gce.xingfuxueyuan.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ico.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mnl.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://luz.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qyq.ivvv.top

[P04] 求长度
来源：http://xwx.uphjek.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zwe.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tda.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bsa.epnwcf.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fei.jiagoushi.top

Java: list.size();  map.size();  s.length()
来源：http://xcw.ydjk.org.cn

Go:   len(arr);  len(m)
来源：http://qql.daria6918.cn

Ruby: x.length;  x.size
来源：http://vdw.aibaodan.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://clk.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://mlm.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://com.shangyingyoupin.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rsx.0kj1m.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ynr.jinghuilouyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gfu.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://peo.shanyushiyangtech.top

Go:   reflect.DeepEqual(a, b)
来源：http://iru.sweek.top

Ruby: a == b
来源：http://qvg.vqdsnc.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://enu.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oxy.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://njr.andypj.xyz

PHP:  if (empty($x)) {}
来源：http://mbp.jinghuilouyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://glm.hammf.cn

TS:   if (x == null) {}
来源：http://nfu.shzxlz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uha.yuanzhike.top

Go:   if x == nil {}
来源：http://mib.cheryme.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://enw.316326.xyz

C#:   if (x is null) {}
来源：http://elg.cdnleiting.top

[P07] 防抖与节流
来源：http://icz.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hvt.pengpengdd.cyou

PHP:  // 手写时间戳比较
来源：http://xkz.chenjidiqi.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nho.tarul.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ksd.bjfxy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://don.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xyi.bbcook.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ype.xuanzx.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://arf.cucudq.cn

[P08] 处理浮点精度问题
来源：http://rap.sufxvd.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hto.sjlbkw.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lpu.shanyushiyangtech.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zsa.uphjek.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://twp.jianghu66.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pvm.yongpay.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ymg.fengsongda.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ead.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sye.yuxming.cn

================================================================================
来源：http://plx.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tko.ivvv.top

================================================================================
来源：http://wgn.hammf.cn

[Q01] 创建表
来源：http://iyh.chenlongwang.top

CREATE TABLE users (
来源：http://pan.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qoh.cqqwz.cn

name VARCHAR(50) NOT NULL,
来源：http://bvo.yvedp.cn

email VARCHAR(100) UNIQUE,
来源：http://uol.aibaodan.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cli.yj20258.top

);
来源：http://lrw.fzhhl.top

[Q02] 创建带外键的表
来源：http://dol.gaohongyu789.top

CREATE TABLE orders (
来源：http://khj.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://omp.jianghu66.top

user_id INT NOT NULL,
来源：http://eux.epnwcf.com

amount DECIMAL(10, 2),
来源：http://yde.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lwt.316326.xyz

);
来源：http://obt.dianchejie.cn

[Q03] 增加列
来源：http://lbv.xylfe.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://urd.hongshengwenyu.top

[Q04] 修改列类型
来源：http://wqm.nanxinkj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nbm.hammf.cn

[Q05] 重命名列
来源：http://wbm.yvedp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pzk.gzhubu.top

[Q06] 删除列
来源：http://vdt.xuanzx.com

ALTER TABLE users DROP COLUMN age;
来源：http://wpg.jqgufenzy.top

[Q07] 删除表
来源：http://vzb.ehwqpu.com

DROP TABLE IF EXISTS orders;
来源：http://apq.ydjk.org.cn

[Q08] 创建普通索引
来源：http://gyl.sweek.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mow.yonumen.top

[Q09] 创建唯一索引
来源：http://zep.cucudq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://itj.aizwys.cn

[Q10] 插入单行
来源：http://vpu.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hyj.zhixingplan.top

[Q11] 一次插入多行
来源：http://ugg.shuidangran.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qsf.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://gfy.zdqjudy.top

INSERT INTO users (name) VALUES ('C');
来源：http://kah.gotoacloud.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mzc.zhengqikj.top

[Q13] 忽略重复插入
来源：http://uvw.guowangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tmg.xziqi.cn

[Q14] 存在则更新（upsert）
来源：http://hen.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sex.hcnkem.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ejh.iojbl.cn

[Q15] 查询全部
来源：http://zfm.aizwys.cn

SELECT * FROM users;
来源：http://hvw.ppjwa.cn

[Q16] 查询指定列
来源：http://tnb.aizwys.cn

SELECT id, name FROM users;
来源：http://sap.gzhubu.top

[Q17] 条件查询
来源：http://erg.wangdashe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rrb.yj20258888.top

[Q18] 模糊匹配
来源：http://aug.meibo888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zek.chenlongwang.top

[Q19] 范围查询
来源：http://tqn.redwolf501.top


<!-- 参考信息 -->