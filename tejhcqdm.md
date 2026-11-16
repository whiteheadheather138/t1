代发 wailian999

Java: public static void main(String[] args)
来源：http://djc.guannengcc.top

Go:   func main()
来源：http://zvt.hongshengwenyu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tfa.0kj1m.cn

C#:   static void Main(string[] args)
来源：http://kbj.gotoacloud.top

[M08] 获取系统与运行时信息
来源：http://okn.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://cte.zhixingplan.top

PHP:  PHP_OS;  phpversion();
来源：http://cpk.pengpengdd.cyou

JS:   process.platform;  process.version
来源：http://eui.gaohongyu789.top

TS:   process.platform;  process.version
来源：http://aqe.yj202588.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tnf.xingfuxueyuan.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://eds.vqdsnc.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nlj.hnxiangtu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ppe.feifeiyinyue.top

================================================================================
来源：http://mlx.yvedp.cn

N. 数据结构与算法
来源：http://gtc.yuxming.cn

================================================================================
来源：http://mun.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://zlf.sufxvd.cn

Py:   bisect.bisect_left(arr, x)
来源：http://omv.yuxming.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uib.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dvg.xziqi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://srg.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://ksn.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://knw.ctjpmb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://scm.sufxvd.cn

C#:   Array.BinarySearch(arr, x)
来源：http://and.havefunace.top

[N02] 排序（工程实践用内置实现）
来源：http://kic.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://rxg.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vcd.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cgc.meibo888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xcs.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cut.316326.xyz

Go:   slices.Sort(arr)
来源：http://ahg.jinghuilouyu.cn

Ruby: arr.sort
来源：http://zpg.chenzaomai.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://pyg.sweek.top

[N03] 快速排序（分治示例）
来源：http://lch.andypj.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kes.zycfv.cn

PHP:  // 递归实现，或用 usort
来源：http://suw.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hjt.jlsjyb.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wsp.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lkz.svipenyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pwk.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lmh.fanxiaobao.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://ekt.xingfuxueyuan.xyz

[N04] 斐波那契数列
来源：http://ulj.ydjk.org.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zyp.sxryk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pkm.nanxuanxn.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dbl.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zfy.cdnleiting.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dmt.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fsh.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ahr.yangfankeji.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nsj.dashuyun.cn

[N05] 最大公约数
来源：http://eah.jinqigfzy.top

Py:   math.gcd(a, b)
来源：http://hjy.yongpay.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://koa.yj202588.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gfb.gaohongyu789.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ovi.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dah.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nly.guannengcc.top

Ruby: a.gcd(b)
来源：http://rts.gzhubu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aig.52xcode.cn

[N06] 判断回文字符串
来源：http://afl.ivvv.top

Py:   s == s[::-1]
来源：http://abg.sufxvd.cn

PHP:  $s === strrev($s);
来源：http://arz.yongpay.top

JS:   s === [...s].reverse().join("")
来源：http://drk.chenzaomai.com

TS:   s === [...s].reverse().join("")
来源：http://jsu.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jer.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://ryj.zdbjq.cn

Ruby: s == s.reverse
来源：http://dvy.c1oappe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://eef.hammf.cn

[N07] 两数之和（返回下标）
来源：http://wkw.redwolf501.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://chj.316326.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rgj.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ohd.cheryme.top

TS:   // 手写 Map<string, number>
来源：http://plk.chenlongwang.top

Java: // 手写 HashMap
来源：http://bkn.uphjek.com

Go:   // 手写 map[int]int
来源：http://gcw.zhijiandao.cn

Ruby: // 手写 Hash
来源：http://ocf.shangyingyoupin.top

C#:   // 手写 Dictionary<int, int>
来源：http://ppj.shanyushiyangtech.top

[N08] 生成全排列
来源：http://dfe.zdbjq.cn

Py:   itertools.permutations(arr)
来源：http://daw.cdnleiting.top

PHP:  // 手写递归交换
来源：http://qzp.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://rja.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://swy.yj202588.top

Java: // 手写回溯递归
来源：http://xfj.xuanzx.com

Go:   // 手写回溯递归
来源：http://agf.jinqigfzy.top

Ruby: arr.permutation.to_a
来源：http://jpj.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://zsp.jinqigufen.top

[N09] 栈与队列
来源：http://emc.fehbvm.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ssz.shuidangran.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xkd.yj202588.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qxa.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://guj.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://esw.gotoacloud.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sfy.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sfp.chenzaomai.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://egd.jiagoushi.top

[N10] 链表节点定义
来源：http://hjr.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pez.yfazqb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://sxy.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mop.jinqigfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://icm.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://ldv.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hqv.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://swe.bbcook.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dpx.nwbrower.top

[N11] 二叉树中序遍历
来源：http://smo.yueranfly.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://agj.andypj.xyz

PHP:  // 手写递归函数
来源：http://oye.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://udp.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kyd.ppjwa.cn

Java: // 手写递归
来源：http://app.guowangkeji.top

Go:   // 手写递归
来源：http://rqo.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fgf.daria6918.cn

C#:   // 手写递归
来源：http://wvk.havefunace.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://icc.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xph.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pli.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uze.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fyd.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zbg.hongshengwenyu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jkk.xziqi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jzv.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ntw.sysykeji.top

================================================================================
来源：http://rxe.shanyushiyangkeji.top

O. 并发与异步
来源：http://wxz.guowangkeji.top

================================================================================
来源：http://ber.xuetiantiany.cn

[O01] 启动一个线程
来源：http://ubh.fehbvm.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hqb.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mpz.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iqj.haohaochexian.top

TS:   // 同 JS
来源：http://hgf.zdbjq.cn

Java: new Thread(() -> f()).start()
来源：http://cpe.wangshuangyany.cn

Go:   go f()
来源：http://exf.xziqi.cn

Ruby: Thread.new { f }
来源：http://dce.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://etw.fanxiaobao.xyz

[O02] 使用线程池
来源：http://akd.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://azg.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bou.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://hln.tianlin.xyz

TS:   // worker_threads 线程池
来源：http://buw.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://dyz.gzhubu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gex.zdbjq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ian.vqdsnc.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bne.epnwcf.com

[O03] 加锁保护共享数据
来源：http://qgq.shzxlz.cn

Py:   with lock: shared += 1
来源：http://upe.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://zdw.hnxiangtu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bkr.xylfe.cn

TS:   // 同 JS
来源：http://fac.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://hqk.svipenyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kru.9152youxi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fsh.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://dwh.zhengqikj.top

[O04] 定义异步函数并等待
来源：http://eno.smart0.xyz

Py:   async def f():⏎    await g()
来源：http://ubn.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dlj.yongpay.top

JS:   async function f() { await g(); }
来源：http://wlf.zhijiandao.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tgg.yj20258.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://djv.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zas.yfazqb.com

Ruby: # 用 Fiber 或 async gem
来源：http://hyh.xinyue.icu

C#:   async Task F() { await G(); }
来源：http://irl.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://szv.tarul.cn

Py:   asyncio.gather(*tasks)
来源：http://vro.yangfankeji.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lpd.hammf.cn

JS:   await Promise.all(tasks)
来源：http://pkj.cashguo.top

TS:   await Promise.all(tasks)
来源：http://gff.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sxr.sjlbkw.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vnq.cqqwz.cn

Ruby: threads.map(&:join)
来源：http://oek.yvedp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xhp.jiagoushi.top

[O06] 使用进程池
来源：http://pyg.bjfxy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://khu.daria6918.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lre.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://tvs.jinghuilouyu.cn

TS:   // child_process / cluster 模块
来源：http://gue.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://clq.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://roz.chenzaomai.com

Ruby: // fork 块
来源：http://ote.svipenyu.cn

C#:   Parallel.For
来源：http://wyo.fehbvm.com

================================================================================
来源：http://pdy.jinqigufen.top

P. 常用工具函数
来源：http://rfd.dashuyun.cn

================================================================================
来源：http://hob.dianchejie.cn

[P01] 生成 UUID
来源：http://ksg.cheryme.top

Py:   str(uuid.uuid4())
来源：http://dtd.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tjs.sysykeji.top

JS:   crypto.randomUUID()
来源：http://qvj.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://wfq.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://fyl.shzxlz.cn

Go:   // 用 github.com/google/uuid
来源：http://jtw.pycfn.com

Ruby: SecureRandom.uuid
来源：http://uqs.zhengqikj.top

C#:   Guid.NewGuid().ToString()
来源：http://fyz.vehdjk.com

[P02] MD5 / SHA256 摘要
来源：http://whb.yj20258888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vfr.sysykeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dcm.kuanghao11.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://znq.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sxd.hongshengwenyu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://egd.ydzc1.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xmt.gzhubu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yxf.yongpay.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qbp.jinghuilouyu.cn

[P03] 生成短随机字符串
来源：http://ubw.havefunace.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vxt.jlsjyb.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zuw.fengsongda.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jit.pycfn.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://obq.fengsongda.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wkx.jinqigufen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hbx.sxryk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kws.zhixingplan.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zds.gzhubu.top

[P04] 求长度
来源：http://gkc.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fac.zycfv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://myd.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eqj.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://srx.xuanzx.com

Java: list.size();  map.size();  s.length()
来源：http://jmn.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://nhf.yuxming.cn

Ruby: x.length;  x.size
来源：http://bom.yj20258888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xsv.vehdjk.com

[P05] 判断两个对象内容是否相等
来源：http://osc.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hqn.shzxlz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qvz.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fmd.yanxiufei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ixi.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lxx.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://iuz.xziqi.cn

Ruby: a == b
来源：http://qil.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jqx.gaohongyu789.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rme.jinyuanbaomall.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ohf.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://upo.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wme.zhijiandao.cn

TS:   if (x == null) {}
来源：http://edi.hywenlv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gwf.nanxinkj.top

Go:   if x == nil {}
来源：http://okq.sweek.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oqu.zhijiandao.cn

C#:   if (x is null) {}
来源：http://fip.shangyingyoupin.top

[P07] 防抖与节流
来源：http://ngm.zhiwuduotai.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://txo.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://tvo.tian-w.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hzd.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wvs.birdmap.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hpt.haohaochexian.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tax.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zqz.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kru.ehwqpu.com

[P08] 处理浮点精度问题
来源：http://pmr.wangdashe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ytk.ivvv.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xvp.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zqz.fzhhl.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xeo.xingfuxueyuan.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wlz.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hei.yonumen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uck.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gxw.jyoumei.cn

================================================================================
来源：http://szv.c1oappe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hsf.kuanghao11.cn

================================================================================
来源：http://uka.quarkkingdee.top

[Q01] 创建表
来源：http://qif.shuidangran.top

CREATE TABLE users (
来源：http://oty.xinyue.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fzx.daxiang520.top

name VARCHAR(50) NOT NULL,
来源：http://bos.chenjidiqi.icu

email VARCHAR(100) UNIQUE,
来源：http://trq.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mce.shanyushiyangtech.top

);
来源：http://lsv.hcnkem.com

[Q02] 创建带外键的表
来源：http://dbh.wangshuangyany.cn

CREATE TABLE orders (
来源：http://dql.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://llt.vehdjk.com

user_id INT NOT NULL,
来源：http://wwj.jinqigfzy.top

amount DECIMAL(10, 2),
来源：http://bga.jinqigufen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://otf.jyoumei.cn

);
来源：http://she.cashguo.top

[Q03] 增加列
来源：http://ssr.fktsv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lfp.hammf.cn

[Q04] 修改列类型
来源：http://smm.hongshengwenyu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tpy.shuidangran.top

[Q05] 重命名列
来源：http://uhc.yuanzhike.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lsm.xinyue.icu

[Q06] 删除列
来源：http://fxl.andypj.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://kon.jlsjyb.cn

[Q07] 删除表
来源：http://bum.guannengcc.top

DROP TABLE IF EXISTS orders;
来源：http://qiw.xinyue.icu

[Q08] 创建普通索引
来源：http://fbj.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qsj.yuanzhike.top

[Q09] 创建唯一索引
来源：http://kvp.pycfn.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tiz.gzhubu.top

[Q10] 插入单行
来源：http://tsi.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://abk.cheryme.top

[Q11] 一次插入多行
来源：http://kov.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://weo.316326.xyz

[Q12] 插入后取自增 ID
来源：http://ban.hnxiangtu.top

INSERT INTO users (name) VALUES ('C');
来源：http://bww.yj20258888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qcu.zhoulong.xyz

[Q13] 忽略重复插入
来源：http://rdy.havefunace.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ztf.hammf.cn

[Q14] 存在则更新（upsert）
来源：http://cgm.jianghu66.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lze.hnqzz.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://obx.jyoumei.cn

[Q15] 查询全部
来源：http://ihf.iojbl.cn


<!-- 参考信息 -->