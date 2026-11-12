代发 wailian999

Java: public static void main(String[] args)
来源：http://ljg.yj202588.top

Go:   func main()
来源：http://puh.guowangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zxw.fengsongda.top

C#:   static void Main(string[] args)
来源：http://wwe.yvedp.cn

[M08] 获取系统与运行时信息
来源：http://bov.fanxiaobao.xyz

Py:   platform.system();  platform.python_version()
来源：http://far.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://idk.meibo888.top

JS:   process.platform;  process.version
来源：http://jbq.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://sjn.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cul.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kdr.yuxming.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sfw.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jpe.xingfuxueyuan.xyz

================================================================================
来源：http://lpi.xylfe.cn

N. 数据结构与算法
来源：http://qal.jqgfzy.top

================================================================================
来源：http://zwd.chenlongwang.top

[N01] 二分查找（有序数组）
来源：http://vco.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kav.chenjidiqi.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ztj.aizwys.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cqp.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://alp.sufxvd.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rwo.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://liu.c1oappe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jsh.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://lup.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://ctg.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://seo.ehwqpu.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fwn.jiagoushi.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://etk.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://bol.smart0.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bdt.ybcxt.top

Go:   slices.Sort(arr)
来源：http://ydt.tianlin.xyz

Ruby: arr.sort
来源：http://rwz.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ibh.yj202588.top

[N03] 快速排序（分治示例）
来源：http://ngb.tanke756.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ngy.haohaochexian.top

PHP:  // 递归实现，或用 usort
来源：http://ktg.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dti.zdbjq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hue.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qkl.bbcook.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pmv.jinyuanbaomall.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://chl.yonumen.top

C#:   // 手写递归，或 Array.Sort
来源：http://yik.epnwcf.com

[N04] 斐波那契数列
来源：http://del.yfazqb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kwk.sweek.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://udf.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wgs.mhx1999.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cds.shuidangran.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dhx.xylfe.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://djz.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bam.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rtg.gaohongyu789.top

[N05] 最大公约数
来源：http://enh.sufxvd.cn

Py:   math.gcd(a, b)
来源：http://vyp.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rfd.yueranfly.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xis.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://llf.xziqi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://huf.gogol.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zrf.xziqi.cn

Ruby: a.gcd(b)
来源：http://ulf.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hqz.zycfv.cn

[N06] 判断回文字符串
来源：http://tif.ppjwa.cn

Py:   s == s[::-1]
来源：http://owf.tarul.cn

PHP:  $s === strrev($s);
来源：http://hop.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://whe.redwolf501.top

TS:   s === [...s].reverse().join("")
来源：http://thl.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oux.shzxlz.cn

Go:   // 双指针从两端比较
来源：http://boh.tarul.cn

Ruby: s == s.reverse
来源：http://bgp.hysaishi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://evp.c1oappe.top

[N07] 两数之和（返回下标）
来源：http://qfr.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ico.wangdashe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zhd.jinqigfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yfv.zhijiandao.cn

TS:   // 手写 Map<string, number>
来源：http://znh.ydjk.org.cn

Java: // 手写 HashMap
来源：http://syj.yongpay.top

Go:   // 手写 map[int]int
来源：http://dae.tarul.cn

Ruby: // 手写 Hash
来源：http://irx.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://rad.fengsongda.top

[N08] 生成全排列
来源：http://itd.yuxming.cn

Py:   itertools.permutations(arr)
来源：http://lgt.hammf.cn

PHP:  // 手写递归交换
来源：http://csq.gotoacloud.top

JS:   // 手写回溯递归
来源：http://kty.aibaodan.cn

TS:   // 手写回溯递归
来源：http://keo.jqgufenzy.top

Java: // 手写回溯递归
来源：http://lok.aibaodan.cn

Go:   // 手写回溯递归
来源：http://eao.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://iig.ehwqpu.com

C#:   // 手写回溯递归
来源：http://lna.nwbrower.top

[N09] 栈与队列
来源：http://flr.daria6918.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sui.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tik.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://irv.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rna.dianchejie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blx.316326.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cup.yonumen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gti.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jzf.epnwcf.com

[N10] 链表节点定义
来源：http://ufo.shuidangran.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://crk.bjfxy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fln.fengsongda.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://foq.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mvy.mhx1999.top

Java: class Node { int v; Node next; }
来源：http://sab.cucudq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wiw.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://hxk.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mmi.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://eqy.9152youxi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://thh.yangfankeji.com

PHP:  // 手写递归函数
来源：http://wmv.hnxiangtu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aas.cucudq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gvh.guannengcc.top

Java: // 手写递归
来源：http://mcs.sufxvd.cn

Go:   // 手写递归
来源：http://cxw.chenlongwang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tpx.yuxming.cn

C#:   // 手写递归
来源：http://ims.yj20258888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ilg.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://huu.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mqf.ppjwa.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://api.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lan.tianlin.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://agp.tianlin.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://air.ppjwa.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xvn.cqqwz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://axl.hongshengwenyu.top

================================================================================
来源：http://daj.sxryk.cn

O. 并发与异步
来源：http://bky.pycfn.com

================================================================================
来源：http://rmh.yanxiufei.cn

[O01] 启动一个线程
来源：http://xgr.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ulk.fktsv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ygd.dashuyun.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xll.aibaodan.cn

TS:   // 同 JS
来源：http://ljq.vqdsnc.cn

Java: new Thread(() -> f()).start()
来源：http://bju.havefunace.top

Go:   go f()
来源：http://cbk.cheryme.top

Ruby: Thread.new { f }
来源：http://jjp.xinyue.icu

C#:   Task.Run(() => F());
来源：http://gpn.mhx1999.top

[O02] 使用线程池
来源：http://uru.xuanzx.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zry.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://koe.daria6918.cn

JS:   // worker_threads 线程池
来源：http://onn.chenlongwang.top

TS:   // worker_threads 线程池
来源：http://gpv.9152youxi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bsi.cqqwz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ywy.birdmap.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://efb.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lqt.vehdjk.com

[O03] 加锁保护共享数据
来源：http://vmk.tian-w.cn

Py:   with lock: shared += 1
来源：http://hib.gogol.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://zsr.cdnleiting.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ngr.pycfn.com

TS:   // 同 JS
来源：http://xbr.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://iyy.feifeiyinyue.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jrk.gotoacloud.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ozo.gaohongyu789.top

C#:   lock (gate) { shared++; }
来源：http://dpf.hcnkem.com

[O04] 定义异步函数并等待
来源：http://kuo.yj20258.top

Py:   async def f():⏎    await g()
来源：http://rvd.zhiwuduotai.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fvg.0kj1m.cn

JS:   async function f() { await g(); }
来源：http://ovt.wangshuangyany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sbo.sjlbkw.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vgb.uphjek.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://abr.sxryk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nhn.fengsongda.top

C#:   async Task F() { await G(); }
来源：http://uyf.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://acg.xingfuxueyuan.xyz

Py:   asyncio.gather(*tasks)
来源：http://kqt.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iam.jinghuilouyu.cn

JS:   await Promise.all(tasks)
来源：http://pmh.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://ple.c1oappe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fug.jinqigfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://egl.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://sbc.vqdsnc.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gug.aizwys.cn

[O06] 使用进程池
来源：http://gfp.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aaq.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://tvz.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://hip.epnwcf.com

TS:   // child_process / cluster 模块
来源：http://anz.yuanzhike.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jgq.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bls.gogol.net.cn

Ruby: // fork 块
来源：http://djo.iojbl.cn

C#:   Parallel.For
来源：http://wxj.sweek.top

================================================================================
来源：http://bdb.tanke756.top

P. 常用工具函数
来源：http://vhg.haohaochexian.top

================================================================================
来源：http://sdp.pycfn.com

[P01] 生成 UUID
来源：http://laa.guowangkeji.top

Py:   str(uuid.uuid4())
来源：http://fvl.yfazqb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://htw.hcnkem.com

JS:   crypto.randomUUID()
来源：http://vga.zhaomingkeji.xyz

TS:   crypto.randomUUID()
来源：http://hep.zycfv.cn

Java: UUID.randomUUID().toString()
来源：http://hnh.hongshengwenyu.top

Go:   // 用 github.com/google/uuid
来源：http://ccs.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://pys.ybcxt.top

C#:   Guid.NewGuid().ToString()
来源：http://yoq.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://dgp.aizwys.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dqu.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tkz.jqgfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fan.xuetiantiany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://giz.gzhubu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ywe.fzhhl.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xzx.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://otd.yfazqb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://szi.dianchejie.cn

[P03] 生成短随机字符串
来源：http://dsy.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://saw.cashguo.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pbm.chenzaomai.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rmu.sweek.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aok.yonumen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://juo.ivvv.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wqa.c1oappe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ltn.shzxlz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kbo.yonumen.top

[P04] 求长度
来源：http://fud.shanyushiyangtech.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fft.yj20258.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nwy.ppjwa.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://abx.fzhhl.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mza.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://mar.jinqigfzy.top

Go:   len(arr);  len(m)
来源：http://oyo.zhixingplan.top

Ruby: x.length;  x.size
来源：http://gea.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zyk.sysykeji.top

[P05] 判断两个对象内容是否相等
来源：http://akn.pengpengdd.cyou

Py:   a == b              # 列表与字典递归比较内容
来源：http://ndy.redwolf501.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wxn.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ztp.xingfuxueyuan.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uhz.shangyingyoupin.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wwv.yfazqb.com

Go:   reflect.DeepEqual(a, b)
来源：http://uah.smart0.xyz

Ruby: a == b
来源：http://kog.fktsv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dko.0kj1m.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cpz.ehwqpu.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://szu.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://qjl.hesvh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vll.hcnkem.com

TS:   if (x == null) {}
来源：http://uni.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://gli.hywenlv.cn

Go:   if x == nil {}
来源：http://rat.dashuyun.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wkd.tianlin.xyz

C#:   if (x is null) {}
来源：http://wmp.guannengcc.top

[P07] 防抖与节流
来源：http://wgf.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tvb.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://jek.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xxz.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ldz.sysykeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qhp.316326.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eel.svipenyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bjp.yvedp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mpf.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://isp.dianchejie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dmr.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mpw.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cxp.ybcxt.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://arb.zhaomingkeji.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xnc.redwolf501.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jfu.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ihk.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pzi.316326.xyz

================================================================================
来源：http://dwi.yj20258888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gfu.cqqwz.cn

================================================================================
来源：http://jcr.hesvh.cn

[Q01] 创建表
来源：http://ggl.jqgufenzy.top

CREATE TABLE users (
来源：http://umh.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iiv.haohaochexian.top

name VARCHAR(50) NOT NULL,
来源：http://vkv.cqqwz.cn

email VARCHAR(100) UNIQUE,
来源：http://vey.yj202588.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yje.zhoulong.xyz

);
来源：http://mgu.sufxvd.cn

[Q02] 创建带外键的表
来源：http://hvx.fengsongda.top

CREATE TABLE orders (
来源：http://nip.epnwcf.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wuw.guannengcc.top

user_id INT NOT NULL,
来源：http://ilf.fehbvm.com

amount DECIMAL(10, 2),
来源：http://sqa.sjlbkw.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ytv.jqgufenzy.top

);
来源：http://ocy.ivvv.top

[Q03] 增加列
来源：http://uem.ydzc1.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xdq.hnqzz.top

[Q04] 修改列类型
来源：http://flj.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mqv.tarul.cn

[Q05] 重命名列
来源：http://zuh.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mra.zdqjudy.top

[Q06] 删除列
来源：http://uxj.yueranfly.top

ALTER TABLE users DROP COLUMN age;
来源：http://xis.aizwys.cn

[Q07] 删除表
来源：http://tmz.jinqigufen.top

DROP TABLE IF EXISTS orders;
来源：http://hhl.mhx1999.top

[Q08] 创建普通索引
来源：http://rzo.tianlin.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://tvw.hongshengwenyu.top

[Q09] 创建唯一索引
来源：http://tzk.sweek.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sok.0kj1m.cn

[Q10] 插入单行
来源：http://phy.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://msr.bbcook.cn

[Q11] 一次插入多行
来源：http://abb.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uct.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://gpi.yonumen.top

INSERT INTO users (name) VALUES ('C');
来源：http://giz.pengpengdd.cyou

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ytp.pycfn.com

[Q13] 忽略重复插入
来源：http://qwq.uphjek.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jcr.shzxlz.cn

[Q14] 存在则更新（upsert）
来源：http://ykr.havefunace.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tkt.shangyingyoupin.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://loi.zhijiandao.cn

[Q15] 查询全部
来源：http://gsj.hammf.cn


<!-- 参考信息 -->