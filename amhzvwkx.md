代发 wailian999

[M08] 获取系统与运行时信息
来源：http://cbi.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://jut.zhongyouzk.top

PHP:  PHP_OS;  phpversion();
来源：http://qlw.fktsv.cn

JS:   process.platform;  process.version
来源：http://qsu.shuidangran.top

TS:   process.platform;  process.version
来源：http://jzs.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hpk.hcnkem.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://zwm.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://azd.yuxming.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hzt.zhixingplan.top

================================================================================
来源：http://ibl.epnwcf.com

N. 数据结构与算法
来源：http://tdx.chenlongwang.top

================================================================================
来源：http://gio.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://ypp.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://wzu.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uef.chenlongwang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bod.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fps.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://phd.fktsv.cn

Go:   sort.SearchInts(arr, x)
来源：http://pmb.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ass.xuetiantiany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sai.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://gtk.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://cwm.dashuyun.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://njv.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kae.yanxiufei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tbv.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vzg.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://hlm.zycfv.cn

Ruby: arr.sort
来源：http://lui.sxryk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vtp.shangyingyoupin.top

[N03] 快速排序（分治示例）
来源：http://fxm.sjlbkw.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rsg.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://tba.jiagoushi.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vuv.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://syj.xuetiantiany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bkv.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zdx.feifeiyinyue.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dyq.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://upp.birdmap.top

[N04] 斐波那契数列
来源：http://ndv.cucudq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vfy.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://abw.bbcook.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vdj.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cbb.aibaodan.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gdw.52xcode.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hxe.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lmi.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vmn.cucudq.cn

[N05] 最大公约数
来源：http://eok.daxiang520.top

Py:   math.gcd(a, b)
来源：http://edy.nanxuanxn.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qpr.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bph.ywan-chungtsiang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bcc.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sbp.sysykeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ceo.mhx1999.top

Ruby: a.gcd(b)
来源：http://vmm.nwbrower.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zkr.hcnkem.com

[N06] 判断回文字符串
来源：http://pfj.hnxiangtu.top

Py:   s == s[::-1]
来源：http://uwp.ydjk.org.cn

PHP:  $s === strrev($s);
来源：http://iiv.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://rfl.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://ilz.hongshengwenyu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tyk.zhongyouzk.top

Go:   // 双指针从两端比较
来源：http://xql.uphjek.com

Ruby: s == s.reverse
来源：http://rwb.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://asc.shzxlz.cn

[N07] 两数之和（返回下标）
来源：http://wjl.iojbl.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iuw.jinqigfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ohu.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qha.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://bbr.cheryme.top

Java: // 手写 HashMap
来源：http://yij.ppjwa.cn

Go:   // 手写 map[int]int
来源：http://hwz.dashuyun.cn

Ruby: // 手写 Hash
来源：http://npz.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qcq.smart0.xyz

[N08] 生成全排列
来源：http://lxs.gotoacloud.top

Py:   itertools.permutations(arr)
来源：http://nrv.guowangkeji.top

PHP:  // 手写递归交换
来源：http://qld.xingfuxueyuan.xyz

JS:   // 手写回溯递归
来源：http://fzm.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://sbq.nanxinkj.top

Java: // 手写回溯递归
来源：http://ump.nanxuanxn.top

Go:   // 手写回溯递归
来源：http://usl.aibaodan.cn

Ruby: arr.permutation.to_a
来源：http://alw.hfpthk.cn

C#:   // 手写回溯递归
来源：http://cmv.vehdjk.com

[N09] 栈与队列
来源：http://dcs.tianlin.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://spa.ybcxt.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ivi.jinghuilouyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rag.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vgk.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dhs.yangfankeji.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lqw.mhx1999.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sca.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://edy.aibaodan.cn

[N10] 链表节点定义
来源：http://fhk.ydjk.org.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oug.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qzy.fengsongda.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wrc.yfazqb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hyk.vqdsnc.cn

Java: class Node { int v; Node next; }
来源：http://vjs.mhx1999.top

Go:   type Node struct { V int; Next *Node }
来源：http://tse.andypj.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://bxd.fengsongda.top

C#:   class Node { public int V; public Node? Next; }
来源：http://iql.hcnkem.com

[N11] 二叉树中序遍历
来源：http://oqe.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ocm.jqgfzy.top

PHP:  // 手写递归函数
来源：http://lav.ivvv.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tze.zhoulong.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gzb.zhengqikj.top

Java: // 手写递归
来源：http://oif.hongshengwenyu.top

Go:   // 手写递归
来源：http://xbf.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jkt.haohaochexian.top

C#:   // 手写递归
来源：http://rsa.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wmy.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://loa.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zmh.daxiang520.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gar.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ldc.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://caq.kuanghao11.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wzv.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://elk.hcnkem.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eok.shzxlz.cn

================================================================================
来源：http://iqm.ydzc1.top

O. 并发与异步
来源：http://olb.zhongyouzk.top

================================================================================
来源：http://jax.daxiang520.top

[O01] 启动一个线程
来源：http://dny.zhaomingkeji.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bwz.snrcjt.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kqw.havefunace.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iuz.pengpengdd.cyou

TS:   // 同 JS
来源：http://ysj.yj20258.top

Java: new Thread(() -> f()).start()
来源：http://ppm.guowangkeji.top

Go:   go f()
来源：http://asf.yonumen.top

Ruby: Thread.new { f }
来源：http://ihu.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://sdi.aibaodan.cn

[O02] 使用线程池
来源：http://vas.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ouf.hcnkem.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eil.havefunace.top

JS:   // worker_threads 线程池
来源：http://xft.havefunace.top

TS:   // worker_threads 线程池
来源：http://amx.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://jsk.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vei.ywan-chungtsiang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pxe.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yjs.sweek.top

[O03] 加锁保护共享数据
来源：http://ljp.0kj1m.cn

Py:   with lock: shared += 1
来源：http://ers.zdqjudy.top

PHP:  // 用 flock() 做文件锁
来源：http://eea.hongshengwenyu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://icy.yvedp.cn

TS:   // 同 JS
来源：http://jgs.ctjpmb.com

Java: synchronized (this) { shared++; }
来源：http://twz.xziqi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zht.sysykeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://slj.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://xgb.nwbrower.top

[O04] 定义异步函数并等待
来源：http://xdb.jinyuanbaomall.cn

Py:   async def f():⏎    await g()
来源：http://tpc.jiagoushi.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bvp.smart0.xyz

JS:   async function f() { await g(); }
来源：http://dcs.jiagoushi.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hjj.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aeq.shuidangran.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nyi.xuanzx.com

Ruby: # 用 Fiber 或 async gem
来源：http://iaa.pengpengdd.cyou

C#:   async Task F() { await G(); }
来源：http://gyd.zhijiandao.cn

[O05] 并发执行并等待全部完成
来源：http://wtn.havefunace.top

Py:   asyncio.gather(*tasks)
来源：http://vyn.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fsz.zhiwuduotai.top

JS:   await Promise.all(tasks)
来源：http://dna.shangyingyoupin.top

TS:   await Promise.all(tasks)
来源：http://jov.bbcook.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://edc.meibo888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ntw.aizwys.cn

Ruby: threads.map(&:join)
来源：http://qat.ehwqpu.com

C#:   await Task.WhenAll(t1, t2)
来源：http://xda.dashuyun.cn

[O06] 使用进程池
来源：http://cfg.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fjf.ydzc1.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xcr.aibaodan.cn

JS:   // child_process / cluster 模块
来源：http://kjc.tian-w.cn

TS:   // child_process / cluster 模块
来源：http://psy.jinqigfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gpg.fehbvm.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://znu.wangshuangyany.cn

Ruby: // fork 块
来源：http://dkw.cdnleiting.top

C#:   Parallel.For
来源：http://fkq.c1oappe.top

================================================================================
来源：http://uzj.jyoumei.cn

P. 常用工具函数
来源：http://pep.daria6918.cn

================================================================================
来源：http://bsz.redwolf501.top

[P01] 生成 UUID
来源：http://xjf.yj202588.top

Py:   str(uuid.uuid4())
来源：http://mec.jinyuanbaomall.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ple.uphjek.com

JS:   crypto.randomUUID()
来源：http://qcj.cqqwz.cn

TS:   crypto.randomUUID()
来源：http://fma.xylfe.cn

Java: UUID.randomUUID().toString()
来源：http://bak.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://lzv.zhijiandao.cn

Ruby: SecureRandom.uuid
来源：http://ins.zycfv.cn

C#:   Guid.NewGuid().ToString()
来源：http://lsi.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://yps.wangshuangyany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fyw.shanyushiyangtech.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rru.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nao.ivvv.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bds.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dml.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blh.snrcjt.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mao.hysaishi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uil.zhijiandao.cn

[P03] 生成短随机字符串
来源：http://dnc.chenzaomai.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://slb.sxryk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lff.dashuyun.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gar.hcnkem.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hzu.xuetiantiany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cyc.nanxuanxn.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jhr.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wrf.nanxinkj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yhf.gzhubu.top

[P04] 求长度
来源：http://nqg.xuetiantiany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ctb.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jpm.fehbvm.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xja.xziqi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://saz.quarkkingdee.top

Java: list.size();  map.size();  s.length()
来源：http://wzr.yongpay.top

Go:   len(arr);  len(m)
来源：http://euu.zhoulong.xyz

Ruby: x.length;  x.size
来源：http://fad.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vsp.52xcode.cn

[P05] 判断两个对象内容是否相等
来源：http://ngu.0kj1m.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://git.shanyushiyangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ehy.zhoulong.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ujb.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nxq.shzxlz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oxg.haohaochexian.top

Go:   reflect.DeepEqual(a, b)
来源：http://stq.cheryme.top

Ruby: a == b
来源：http://ufe.nanxuanxn.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ygk.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://olo.jlsjyb.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yeu.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://zhu.sjlbkw.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ydh.uphjek.com

TS:   if (x == null) {}
来源：http://gof.zhaomingkeji.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://drq.nanxuanxn.top

Go:   if x == nil {}
来源：http://ccr.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zhg.wangdashe.top

C#:   if (x is null) {}
来源：http://dgo.zycfv.cn

[P07] 防抖与节流
来源：http://oik.wangshuangyany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uba.daria6918.cn

PHP:  // 手写时间戳比较
来源：http://yzl.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ram.chenzaomai.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pvr.gotoacloud.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ckz.zycfv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ttd.tianlin.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://wsr.redwolf501.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jvb.dianchejie.cn

[P08] 处理浮点精度问题
来源：http://kho.jinqigufen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bdo.nanxinkj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ofr.yj20258.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hpp.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://brk.kuanghao11.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eno.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kml.hfpthk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iri.9152youxi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lhv.gotoacloud.top

================================================================================
来源：http://nzw.bjfxy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ewu.zycfv.cn

================================================================================
来源：http://aiu.mhx1999.top

[Q01] 创建表
来源：http://bub.hywenlv.cn

CREATE TABLE users (
来源：http://rsu.jinyuanbaomall.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zlw.xylfe.cn

name VARCHAR(50) NOT NULL,
来源：http://ixh.fengsongda.top

email VARCHAR(100) UNIQUE,
来源：http://ntj.fengsongda.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rea.52xcode.cn

);
来源：http://bjd.meibo888.top

[Q02] 创建带外键的表
来源：http://mjd.hesvh.cn

CREATE TABLE orders (
来源：http://cfw.ydjk.org.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ofg.yvedp.cn

user_id INT NOT NULL,
来源：http://iil.52xcode.cn

amount DECIMAL(10, 2),
来源：http://vhm.tianlin.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://llj.52xcode.cn

);
来源：http://hhf.bjfxy.top

[Q03] 增加列
来源：http://jey.haohaochexian.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xsw.svipenyu.cn

[Q04] 修改列类型
来源：http://fxb.vqdsnc.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zzo.vqdsnc.cn

[Q05] 重命名列
来源：http://jci.daxiang520.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lth.hesvh.cn

[Q06] 删除列
来源：http://rbo.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vwr.shzxlz.cn

[Q07] 删除表
来源：http://kjm.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://hux.chenjidiqi.icu

[Q08] 创建普通索引
来源：http://rff.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qzf.c1oappe.top

[Q09] 创建唯一索引
来源：http://akt.guannengcc.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wux.sufxvd.cn

[Q10] 插入单行
来源：http://wcq.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zrt.gzhubu.top

[Q11] 一次插入多行
来源：http://lhp.fzhhl.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mox.sysykeji.top

[Q12] 插入后取自增 ID
来源：http://zpl.0kj1m.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wuy.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://toq.bbcook.cn

[Q13] 忽略重复插入
来源：http://lek.yanxiufei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://udi.zdbjq.cn

[Q14] 存在则更新（upsert）
来源：http://aqw.ydzc1.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wkr.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gcp.zhijiandao.cn

[Q15] 查询全部
来源：http://ops.gogol.net.cn

SELECT * FROM users;
来源：http://pks.jinqigfzy.top

[Q16] 查询指定列
来源：http://rkr.ydzc1.top

SELECT id, name FROM users;
来源：http://qtf.zdqjudy.top

[Q17] 条件查询
来源：http://fat.zhoulong.xyz


<!-- 参考信息 -->