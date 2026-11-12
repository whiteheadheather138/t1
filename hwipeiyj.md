代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://lbg.hnqzz.top

================================================================================
来源：http://nbj.zhijiandao.cn

N. 数据结构与算法
来源：http://udd.9152youxi.cn

================================================================================
来源：http://rrh.sufxvd.cn

[N01] 二分查找（有序数组）
来源：http://xxq.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://okw.yuanzhike.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jmb.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fne.havefunace.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ahr.wangshuangyany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vbb.cheryme.top

Go:   sort.SearchInts(arr, x)
来源：http://mcr.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aje.yj202588.top

C#:   Array.BinarySearch(arr, x)
来源：http://mmr.sweek.top

[N02] 排序（工程实践用内置实现）
来源：http://doi.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://mtj.yueranfly.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tdq.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jvn.yuanzhike.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sjk.kuanghao11.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jxd.hcnkem.com

Go:   slices.Sort(arr)
来源：http://zwy.aizwys.cn

Ruby: arr.sort
来源：http://usx.9152youxi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xxt.xuanzx.com

[N03] 快速排序（分治示例）
来源：http://trg.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jbw.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://lgd.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tve.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nfz.haohaochexian.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://buu.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mew.smart0.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xov.shanyushiyangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://eix.gogol.net.cn

[N04] 斐波那契数列
来源：http://ozh.ivvv.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uga.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cvm.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cux.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mru.jinghuilouyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yju.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zim.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nwm.ppjwa.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yff.shzxlz.cn

[N05] 最大公约数
来源：http://lwh.ydzc1.top

Py:   math.gcd(a, b)
来源：http://mof.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gnr.hnxiangtu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://voa.pycfn.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sea.havefunace.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pcd.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ria.tanke756.top

Ruby: a.gcd(b)
来源：http://nil.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dug.ydjk.org.cn

[N06] 判断回文字符串
来源：http://fpw.yueranfly.top

Py:   s == s[::-1]
来源：http://poa.nanxuanxn.top

PHP:  $s === strrev($s);
来源：http://fwk.tarul.cn

JS:   s === [...s].reverse().join("")
来源：http://soo.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://iuk.havefunace.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fdf.dianchejie.cn

Go:   // 双指针从两端比较
来源：http://rbl.hongshengwenyu.top

Ruby: s == s.reverse
来源：http://eih.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ssa.fehbvm.com

[N07] 两数之和（返回下标）
来源：http://mdo.hesvh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://svw.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rli.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cky.sufxvd.cn

TS:   // 手写 Map<string, number>
来源：http://osm.jiagoushi.top

Java: // 手写 HashMap
来源：http://bpa.cashguo.top

Go:   // 手写 map[int]int
来源：http://xfa.quarkkingdee.top

Ruby: // 手写 Hash
来源：http://lxn.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://lif.vehdjk.com

[N08] 生成全排列
来源：http://swp.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://cwz.shangyingyoupin.top

PHP:  // 手写递归交换
来源：http://bmb.shzxlz.cn

JS:   // 手写回溯递归
来源：http://vwq.yuxming.cn

TS:   // 手写回溯递归
来源：http://osy.iojbl.cn

Java: // 手写回溯递归
来源：http://gnb.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://xbh.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://keb.pycfn.com

C#:   // 手写回溯递归
来源：http://nae.guowangkeji.top

[N09] 栈与队列
来源：http://kak.wangshuangyany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://grz.fengsongda.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gyg.mhx1999.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ars.dianchejie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zjg.pycfn.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xmp.nanxuanxn.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oku.epnwcf.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kpp.daria6918.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://opd.kuanghao11.cn

[N10] 链表节点定义
来源：http://red.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://upw.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vgn.hesvh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iuz.yvedp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dng.zdqjudy.top

Java: class Node { int v; Node next; }
来源：http://uat.xingfuxueyuan.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://cim.mhx1999.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jcx.sysykeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tmc.chenlongwang.top

[N11] 二叉树中序遍历
来源：http://hjz.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xqw.dianchejie.cn

PHP:  // 手写递归函数
来源：http://zes.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nui.yuxming.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zpr.jqgfzy.top

Java: // 手写递归
来源：http://fpe.wangshuangyany.cn

Go:   // 手写递归
来源：http://rdg.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vhg.zhixingplan.top

C#:   // 手写递归
来源：http://dfa.cqqwz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zqo.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hin.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lal.dianchejie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dfi.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://znm.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lcy.chenlongwang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rsv.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lll.yj202588.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nqx.tianlin.xyz

================================================================================
来源：http://njr.jqgfzy.top

O. 并发与异步
来源：http://nco.chenjidiqi.icu

================================================================================
来源：http://gsv.yanxiufei.cn

[O01] 启动一个线程
来源：http://ggm.tianlin.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bse.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cym.wangshuangyany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hjc.guowangkeji.top

TS:   // 同 JS
来源：http://dgx.kuanghao11.cn

Java: new Thread(() -> f()).start()
来源：http://iok.cashguo.top

Go:   go f()
来源：http://pku.pycfn.com

Ruby: Thread.new { f }
来源：http://uyi.wangshuangyany.cn

C#:   Task.Run(() => F());
来源：http://hsc.gzhubu.top

[O02] 使用线程池
来源：http://krm.xingfuxueyuan.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hkk.zhiwuduotai.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://svg.ydzc1.top

JS:   // worker_threads 线程池
来源：http://rzh.shuidangran.top

TS:   // worker_threads 线程池
来源：http://zwh.ivvv.top

Java: Executors.newFixedThreadPool(4)
来源：http://whi.feifeiyinyue.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gfu.tanke756.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cfy.ybcxt.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dpn.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://ggk.birdmap.top

Py:   with lock: shared += 1
来源：http://aao.hesvh.cn

PHP:  // 用 flock() 做文件锁
来源：http://tgt.yuxming.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yuq.ctjpmb.com

TS:   // 同 JS
来源：http://bgk.hnqzz.top

Java: synchronized (this) { shared++; }
来源：http://zjr.pycfn.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://upj.jyoumei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zmb.ivvv.top

C#:   lock (gate) { shared++; }
来源：http://hgl.xziqi.cn

[O04] 定义异步函数并等待
来源：http://jns.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://txa.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xsu.pengpengdd.cyou

JS:   async function f() { await g(); }
来源：http://vmx.316326.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://udc.hongshengwenyu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wxd.jyoumei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jnx.yuxming.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zrb.ctjpmb.com

C#:   async Task F() { await G(); }
来源：http://guc.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://she.zhaomingkeji.xyz

Py:   asyncio.gather(*tasks)
来源：http://qmk.jinqigufen.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xgo.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://hnm.52xcode.cn

TS:   await Promise.all(tasks)
来源：http://cun.ydjk.org.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ben.gzhubu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://run.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://saa.tianlin.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://mqs.zycfv.cn

[O06] 使用进程池
来源：http://hgs.tanke756.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xuy.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uaj.fengsongda.top

JS:   // child_process / cluster 模块
来源：http://bld.yj202588.top

TS:   // child_process / cluster 模块
来源：http://qae.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hdl.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ypi.snrcjt.cn

Ruby: // fork 块
来源：http://abd.sxryk.cn

C#:   Parallel.For
来源：http://lhk.jqgfzy.top

================================================================================
来源：http://tap.haohaochexian.top

P. 常用工具函数
来源：http://wee.yonumen.top

================================================================================
来源：http://abr.ydzc1.top

[P01] 生成 UUID
来源：http://chd.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://koo.jqgfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jvo.zhoulong.xyz

JS:   crypto.randomUUID()
来源：http://awa.zhiwuduotai.top

TS:   crypto.randomUUID()
来源：http://hfm.sufxvd.cn

Java: UUID.randomUUID().toString()
来源：http://xxc.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://hfo.redwolf501.top

Ruby: SecureRandom.uuid
来源：http://btw.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://vpx.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://mjv.yfazqb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xyl.fehbvm.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://exz.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://maf.ppjwa.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xwb.sweek.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gcp.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tfo.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iqd.pengpengdd.cyou

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rpe.daria6918.cn

[P03] 生成短随机字符串
来源：http://tgv.shuidangran.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://thh.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://osj.tianlin.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xqv.jinyuanbaomall.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rar.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kxj.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://onr.redwolf501.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://afu.ybcxt.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xec.hnxiangtu.top

[P04] 求长度
来源：http://ljt.bbcook.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ilv.chenlongwang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lwy.cashguo.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://usa.0kj1m.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vhy.shanyushiyangtech.top

Java: list.size();  map.size();  s.length()
来源：http://jnr.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://qfo.yueranfly.top

Ruby: x.length;  x.size
来源：http://hmp.zhaomingkeji.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://bmf.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://ljf.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://uuw.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ooz.jinyuanbaomall.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ors.tian-w.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sdr.jinyuanbaomall.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://egd.chenzaomai.com

Go:   reflect.DeepEqual(a, b)
来源：http://rpd.xinyue.icu

Ruby: a == b
来源：http://fhk.xuanzx.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tey.aizwys.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bve.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zhd.cdnleiting.top

PHP:  if (empty($x)) {}
来源：http://gmt.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://prf.yj20258.top

TS:   if (x == null) {}
来源：http://zsy.snrcjt.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vmi.xuanzx.com

Go:   if x == nil {}
来源：http://mme.ppjwa.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dkq.shanyushiyangkeji.top

C#:   if (x is null) {}
来源：http://eqz.daria6918.cn

[P07] 防抖与节流
来源：http://cjm.sweek.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rmd.dianchejie.cn

PHP:  // 手写时间戳比较
来源：http://ojo.zhengqikj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jah.xziqi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uny.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jkq.shzxlz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ukl.gogol.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qsv.haohaochexian.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://goh.bbcook.cn

[P08] 处理浮点精度问题
来源：http://kqx.tian-w.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://edt.ywan-chungtsiang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yqi.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wsg.ybcxt.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://juh.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yjz.pengpengdd.cyou

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fst.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kio.vehdjk.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nbd.shuidangran.top

================================================================================
来源：http://ukb.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mzp.haohaochexian.top

================================================================================
来源：http://ppr.wangshuangyany.cn

[Q01] 创建表
来源：http://ifl.fengsongda.top

CREATE TABLE users (
来源：http://nrl.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://auy.zhijiandao.cn

name VARCHAR(50) NOT NULL,
来源：http://egp.chenjidiqi.icu

email VARCHAR(100) UNIQUE,
来源：http://pzp.9152youxi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kwd.yj20258888.top

);
来源：http://qcx.shuidangran.top

[Q02] 创建带外键的表
来源：http://mul.jqgufenzy.top

CREATE TABLE orders (
来源：http://lct.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rbk.hesvh.cn

user_id INT NOT NULL,
来源：http://nmg.yj20258888.top

amount DECIMAL(10, 2),
来源：http://qwb.zhoulong.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iyo.fehbvm.com

);
来源：http://rup.zhijiandao.cn

[Q03] 增加列
来源：http://zwb.jinyuanbaomall.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nlm.vqdsnc.cn

[Q04] 修改列类型
来源：http://tkc.tarul.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eij.sysykeji.top

[Q05] 重命名列
来源：http://zek.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cab.xuanzx.com

[Q06] 删除列
来源：http://zwt.zhijiandao.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zjf.c1oappe.top

[Q07] 删除表
来源：http://nkx.tianlin.xyz

DROP TABLE IF EXISTS orders;
来源：http://rfa.xuanzx.com

[Q08] 创建普通索引
来源：http://fmj.jinyuanbaomall.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fao.c1oappe.top

[Q09] 创建唯一索引
来源：http://lac.yanxiufei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hcf.zhaomingkeji.xyz

[Q10] 插入单行
来源：http://qcc.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tpn.iojbl.cn

[Q11] 一次插入多行
来源：http://red.yj202588.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vxr.havefunace.top

[Q12] 插入后取自增 ID
来源：http://vbw.c1oappe.top

INSERT INTO users (name) VALUES ('C');
来源：http://fhs.kuanghao11.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bvp.jinqigufen.top

[Q13] 忽略重复插入
来源：http://soa.yongpay.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ckz.sufxvd.cn

[Q14] 存在则更新（upsert）
来源：http://mvj.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dnv.fktsv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ejx.aizwys.cn

[Q15] 查询全部
来源：http://cbx.iojbl.cn

SELECT * FROM users;
来源：http://urz.tanke756.top

[Q16] 查询指定列
来源：http://gtp.bjfxy.top

SELECT id, name FROM users;
来源：http://kra.vqdsnc.cn

[Q17] 条件查询
来源：http://jxk.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://poh.zhongyouzk.top

[Q18] 模糊匹配
来源：http://bma.jinyuanbaomall.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ask.nanxinkj.top

[Q19] 范围查询
来源：http://cho.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oys.tianlin.xyz

[Q20] IN 列表
来源：http://hnd.epnwcf.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mwi.shangyingyoupin.top

[Q21] 空值判断
来源：http://frv.fanxiaobao.xyz


<!-- 参考信息 -->