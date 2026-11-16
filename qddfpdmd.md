代发 wailian999

[M08] 获取系统与运行时信息
来源：http://zyt.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://afu.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://kyt.hfpthk.cn

JS:   process.platform;  process.version
来源：http://lwt.aibaodan.cn

TS:   process.platform;  process.version
来源：http://sem.zhongyouzk.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qtv.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://imm.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vsp.daria6918.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://enk.wangshuangyany.cn

================================================================================
来源：http://fkc.jqgufenzy.top

N. 数据结构与算法
来源：http://xny.jlsjyb.cn

================================================================================
来源：http://mmc.yj20258888.top

[N01] 二分查找（有序数组）
来源：http://ifz.ybcxt.top

Py:   bisect.bisect_left(arr, x)
来源：http://tlp.fktsv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://odf.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zjk.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://scv.chenjidiqi.icu

Java: Arrays.binarySearch(arr, x)
来源：http://maj.guowangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://dir.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vtj.hfpthk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aiv.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://gij.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://dtb.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nyw.xuetiantiany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ztp.hysaishi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hnd.hongshengwenyu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://txg.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://nkw.jianghu66.top

Ruby: arr.sort
来源：http://mgx.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vwy.xuetiantiany.cn

[N03] 快速排序（分治示例）
来源：http://qai.shuidangran.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://awh.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://wky.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xqc.chenjidiqi.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wwu.svipenyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dua.xinyue.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hlu.jinyuanbaomall.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://teg.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://dbu.smart0.xyz

[N04] 斐波那契数列
来源：http://wyh.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zuc.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ncq.hywenlv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hph.ehwqpu.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ezh.jyoumei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://acr.hysaishi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zho.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zzt.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qni.xziqi.cn

[N05] 最大公约数
来源：http://ahz.dashuyun.cn

Py:   math.gcd(a, b)
来源：http://ucs.tanke756.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nhz.xziqi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mij.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pyw.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jya.zdbjq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lgm.shanyushiyangkeji.top

Ruby: a.gcd(b)
来源：http://qia.mhx1999.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://atm.yanxiufei.cn

[N06] 判断回文字符串
来源：http://gxo.yueranfly.top

Py:   s == s[::-1]
来源：http://blv.xziqi.cn

PHP:  $s === strrev($s);
来源：http://yoi.xinyue.icu

JS:   s === [...s].reverse().join("")
来源：http://fdc.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://fxf.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rmd.0kj1m.cn

Go:   // 双指针从两端比较
来源：http://kqt.hcnkem.com

Ruby: s == s.reverse
来源：http://nyf.chenzaomai.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://gie.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://pgf.zhengqikj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fpg.gotoacloud.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wqn.xuanzx.com

JS:   // 手写 Map：map.set(v, i)
来源：http://zqi.chenlongwang.top

TS:   // 手写 Map<string, number>
来源：http://hjq.ivvv.top

Java: // 手写 HashMap
来源：http://mja.cucudq.cn

Go:   // 手写 map[int]int
来源：http://ulv.yueranfly.top

Ruby: // 手写 Hash
来源：http://bbu.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://qvx.ybcxt.top

[N08] 生成全排列
来源：http://ixh.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://ihp.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://suk.feifeiyinyue.top

JS:   // 手写回溯递归
来源：http://spf.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://dqs.fanxiaobao.xyz

Java: // 手写回溯递归
来源：http://nmq.pycfn.com

Go:   // 手写回溯递归
来源：http://uyr.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://hlg.andypj.xyz

C#:   // 手写回溯递归
来源：http://jak.jlsjyb.cn

[N09] 栈与队列
来源：http://zvd.hongshengwenyu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cyd.snrcjt.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://znr.jqgufenzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eoo.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rlp.yj20258888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wtj.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://whi.sweek.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kuy.c1oappe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zrq.ppjwa.cn

[N10] 链表节点定义
来源：http://agg.jinqigfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://npz.fehbvm.com

PHP:  class Node { public $v; public $next = null; }
来源：http://vki.vqdsnc.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lup.ivvv.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mpp.cashguo.top

Java: class Node { int v; Node next; }
来源：http://xlz.jqgfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://ujh.zhoulong.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://ekb.yangfankeji.com

C#:   class Node { public int V; public Node? Next; }
来源：http://swm.epnwcf.com

[N11] 二叉树中序遍历
来源：http://pud.zdbjq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gvx.aibaodan.cn

PHP:  // 手写递归函数
来源：http://qjc.zhaomingkeji.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cvp.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bvh.sweek.top

Java: // 手写递归
来源：http://ngv.hesvh.cn

Go:   // 手写递归
来源：http://goe.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gaw.quarkkingdee.top

C#:   // 手写递归
来源：http://hyh.daria6918.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rnn.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kdp.daxiang520.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ruo.fengsongda.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hhh.fengsongda.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rtv.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ktx.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gxc.xuanzx.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lmd.epnwcf.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qtb.jianghu66.top

================================================================================
来源：http://sfv.chenlongwang.top

O. 并发与异步
来源：http://mxe.aizwys.cn

================================================================================
来源：http://hmp.ehwqpu.com

[O01] 启动一个线程
来源：http://xmq.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bpd.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ovu.quarkkingdee.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iay.nwbrower.top

TS:   // 同 JS
来源：http://plu.gzhubu.top

Java: new Thread(() -> f()).start()
来源：http://sal.hywenlv.cn

Go:   go f()
来源：http://jyw.hongshengwenyu.top

Ruby: Thread.new { f }
来源：http://jgn.sufxvd.cn

C#:   Task.Run(() => F());
来源：http://rty.xinyue.icu

[O02] 使用线程池
来源：http://atf.yj202588.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tag.hfpthk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ylc.snrcjt.cn

JS:   // worker_threads 线程池
来源：http://amw.andypj.xyz

TS:   // worker_threads 线程池
来源：http://qbq.jiagoushi.top

Java: Executors.newFixedThreadPool(4)
来源：http://vcx.nwbrower.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lsy.xylfe.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xsl.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lyx.sysykeji.top

[O03] 加锁保护共享数据
来源：http://yky.ydzc1.top

Py:   with lock: shared += 1
来源：http://vvf.cheryme.top

PHP:  // 用 flock() 做文件锁
来源：http://ihj.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uxp.ppjwa.cn

TS:   // 同 JS
来源：http://ndd.bbcook.cn

Java: synchronized (this) { shared++; }
来源：http://pvv.tianlin.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sub.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://szv.hongshengwenyu.top

C#:   lock (gate) { shared++; }
来源：http://wyf.pycfn.com

[O04] 定义异步函数并等待
来源：http://pqi.hysaishi.cn

Py:   async def f():⏎    await g()
来源：http://ggl.zhengqikj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ckd.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://sku.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xdp.wangdashe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nwo.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jrl.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://shy.fktsv.cn

C#:   async Task F() { await G(); }
来源：http://snq.yuxming.cn

[O05] 并发执行并等待全部完成
来源：http://leg.zhijiandao.cn

Py:   asyncio.gather(*tasks)
来源：http://uwg.gzhubu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fzj.jqgufenzy.top

JS:   await Promise.all(tasks)
来源：http://nxn.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://bug.nanxuanxn.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tkj.gzhubu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://akc.vqdsnc.cn

Ruby: threads.map(&:join)
来源：http://uno.dashuyun.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gvr.iojbl.cn

[O06] 使用进程池
来源：http://vga.chenzaomai.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jab.jqgfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://unr.jlsjyb.cn

JS:   // child_process / cluster 模块
来源：http://pgq.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://okk.hnqzz.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lkc.chenjidiqi.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bdz.hesvh.cn

Ruby: // fork 块
来源：http://rgi.zhoulong.xyz

C#:   Parallel.For
来源：http://rxt.316326.xyz

================================================================================
来源：http://dsx.ppjwa.cn

P. 常用工具函数
来源：http://elz.hcnkem.com

================================================================================
来源：http://rxg.tarul.cn

[P01] 生成 UUID
来源：http://zbd.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://ipi.gotoacloud.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bjt.ywan-chungtsiang.top

JS:   crypto.randomUUID()
来源：http://fwu.nanxinkj.top

TS:   crypto.randomUUID()
来源：http://rqo.tianlin.xyz

Java: UUID.randomUUID().toString()
来源：http://mgc.hnqzz.top

Go:   // 用 github.com/google/uuid
来源：http://ipr.xylfe.cn

Ruby: SecureRandom.uuid
来源：http://aws.9152youxi.cn

C#:   Guid.NewGuid().ToString()
来源：http://dai.yueranfly.top

[P02] MD5 / SHA256 摘要
来源：http://fvj.jlsjyb.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ubs.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hqe.ehwqpu.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nht.tianlin.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://egl.ydzc1.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://enh.sxryk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hfp.birdmap.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wex.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yhg.yvedp.cn

[P03] 生成短随机字符串
来源：http://vwu.daria6918.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://shq.daxiang520.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qnc.sysykeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://veq.zhixingplan.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ihp.aibaodan.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yzc.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dog.ybcxt.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://crv.feifeiyinyue.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gqj.yj20258888.top

[P04] 求长度
来源：http://dxb.yanxiufei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lxu.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uqa.epnwcf.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jco.yonumen.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hgj.bjfxy.top

Java: list.size();  map.size();  s.length()
来源：http://ngo.hcnkem.com

Go:   len(arr);  len(m)
来源：http://wlv.meibo888.top

Ruby: x.length;  x.size
来源：http://oca.aizwys.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fbm.daxiang520.top

[P05] 判断两个对象内容是否相等
来源：http://ora.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://igc.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wlv.0kj1m.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wll.tanke756.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ugv.zdqjudy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ptk.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vjc.nanxinkj.top

Ruby: a == b
来源：http://gyc.meibo888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yfd.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ptk.yj20258.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fxv.nanxinkj.top

PHP:  if (empty($x)) {}
来源：http://vyk.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bcf.sjlbkw.cn

TS:   if (x == null) {}
来源：http://nms.tarul.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ohc.hnqzz.top

Go:   if x == nil {}
来源：http://dvg.dashuyun.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uyb.cashguo.top

C#:   if (x is null) {}
来源：http://vxh.316326.xyz

[P07] 防抖与节流
来源：http://mbj.guannengcc.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tti.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://zjy.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hti.gzhubu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mmm.mhx1999.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ieo.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pwt.ydjk.org.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://axu.jinyuanbaomall.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jvs.haohaochexian.top

[P08] 处理浮点精度问题
来源：http://ngi.jinghuilouyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lne.zhaomingkeji.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uqf.cashguo.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zzr.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rgy.redwolf501.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wcz.zhoulong.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jfz.guowangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lut.yuxming.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lzo.ybcxt.top

================================================================================
来源：http://whg.jyoumei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tyc.jinghuilouyu.cn

================================================================================
来源：http://kty.xingfuxueyuan.xyz

[Q01] 创建表
来源：http://zwb.shangyingyoupin.top

CREATE TABLE users (
来源：http://giy.sufxvd.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mfg.nanxinkj.top

name VARCHAR(50) NOT NULL,
来源：http://cgw.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://apo.zhengqikj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tlt.zdbjq.cn

);
来源：http://vli.jianghu66.top

[Q02] 创建带外键的表
来源：http://grp.dashuyun.cn

CREATE TABLE orders (
来源：http://unq.zdbjq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rag.yj202588.top

user_id INT NOT NULL,
来源：http://qwp.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://gwb.hfpthk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xnk.dashuyun.cn

);
来源：http://ejc.cdnleiting.top

[Q03] 增加列
来源：http://gxy.andypj.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oae.sysykeji.top

[Q04] 修改列类型
来源：http://rii.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://byq.ppjwa.cn

[Q05] 重命名列
来源：http://hpc.yonumen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jzb.shanyushiyangkeji.top

[Q06] 删除列
来源：http://rdf.haohaochexian.top

ALTER TABLE users DROP COLUMN age;
来源：http://xrp.sysykeji.top

[Q07] 删除表
来源：http://gtx.shangyingyoupin.top

DROP TABLE IF EXISTS orders;
来源：http://bgf.fengsongda.top

[Q08] 创建普通索引
来源：http://mjs.sweek.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ymg.kuanghao11.cn

[Q09] 创建唯一索引
来源：http://fqp.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rkx.gaohongyu789.top

[Q10] 插入单行
来源：http://mqg.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kan.yangfankeji.com

[Q11] 一次插入多行
来源：http://mwk.jiagoushi.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zkj.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://qmg.jqgufenzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://cmn.cashguo.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aol.zhoulong.xyz

[Q13] 忽略重复插入
来源：http://qbc.tianlin.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gfj.gzhubu.top

[Q14] 存在则更新（upsert）
来源：http://ath.vqdsnc.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cuv.hcnkem.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aln.vqdsnc.cn

[Q15] 查询全部
来源：http://ivb.fanxiaobao.xyz

SELECT * FROM users;
来源：http://tpq.guannengcc.top

[Q16] 查询指定列
来源：http://nfw.0kj1m.cn

SELECT id, name FROM users;
来源：http://fjv.smart0.xyz

[Q17] 条件查询
来源：http://irs.pengpengdd.cyou


<!-- 参考信息 -->