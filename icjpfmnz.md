代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://snz.dianchejie.cn

[M05] 设置退出码
来源：http://oyo.guowangkeji.top

Py:   sys.exit(1)
来源：http://dyu.jianghu66.top

PHP:  exit(1);
来源：http://xcf.aizwys.cn

JS:   process.exit(1)
来源：http://xko.dianchejie.cn

TS:   process.exit(1)
来源：http://xov.bjfxy.top

Java: System.exit(1)
来源：http://ygx.hammf.cn

Go:   os.Exit(1)
来源：http://vdn.cashguo.top

Ruby: exit 1
来源：http://kdi.yj20258888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xen.ppjwa.cn

[M06] 向标准错误输出
来源：http://nub.xuetiantiany.cn

Py:   print("err", file=sys.stderr)
来源：http://xep.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kts.nanxuanxn.top

JS:   console.error("err")
来源：http://xvi.cheryme.top

TS:   console.error("err")
来源：http://mkk.xziqi.cn

Java: System.err.println("err")
来源：http://mhq.jqgfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pby.havefunace.top

Ruby: warn "err"
来源：http://nvc.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://omk.hfpthk.cn

[M07] 判断是否为主入口
来源：http://tip.yj20258.top

Py:   if __name__ == "__main__":
来源：http://kgq.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xmp.tianlin.xyz

JS:   require.main === module
来源：http://hbo.tian-w.cn

TS:   require.main === module
来源：http://tvu.fehbvm.com

Java: public static void main(String[] args)
来源：http://ifq.fanxiaobao.xyz

Go:   func main()
来源：http://zyv.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://neq.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://sdf.sysykeji.top

[M08] 获取系统与运行时信息
来源：http://iqc.xylfe.cn

Py:   platform.system();  platform.python_version()
来源：http://ahe.dashuyun.cn

PHP:  PHP_OS;  phpversion();
来源：http://ygv.jinqigufen.top

JS:   process.platform;  process.version
来源：http://uru.hammf.cn

TS:   process.platform;  process.version
来源：http://vxw.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ijz.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nyk.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jcx.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://saz.jianghu66.top

================================================================================
来源：http://fxu.jinyuanbaomall.cn

N. 数据结构与算法
来源：http://qkb.meibo888.top

================================================================================
来源：http://etr.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://mrp.haohaochexian.top

Py:   bisect.bisect_left(arr, x)
来源：http://mjt.jianghu66.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xir.zdbjq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wpo.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iqy.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://kxr.fktsv.cn

Go:   sort.SearchInts(arr, x)
来源：http://yow.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oso.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hsg.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://yhh.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://xko.cqqwz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bnc.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uid.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://iud.snrcjt.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lzj.c1oappe.top

Go:   slices.Sort(arr)
来源：http://enl.chenjidiqi.icu

Ruby: arr.sort
来源：http://xaa.cdnleiting.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qod.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://mrh.fktsv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://crk.316326.xyz

PHP:  // 递归实现，或用 usort
来源：http://gge.chenjidiqi.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ira.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://azd.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fje.bbcook.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pts.ehwqpu.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://obd.daria6918.cn

C#:   // 手写递归，或 Array.Sort
来源：http://djm.yj20258.top

[N04] 斐波那契数列
来源：http://yrr.epnwcf.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pud.xylfe.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ows.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hnq.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tck.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zss.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dbm.pengpengdd.cyou

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://thz.jlsjyb.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gkc.nanxuanxn.top

[N05] 最大公约数
来源：http://qny.ydjk.org.cn

Py:   math.gcd(a, b)
来源：http://wll.dianchejie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dsp.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mfm.vqdsnc.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yct.zdbjq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rpu.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ddh.zhijiandao.cn

Ruby: a.gcd(b)
来源：http://qfb.pengpengdd.cyou

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ohj.ppjwa.cn

[N06] 判断回文字符串
来源：http://oqg.havefunace.top

Py:   s == s[::-1]
来源：http://oon.sjlbkw.cn

PHP:  $s === strrev($s);
来源：http://lvo.hammf.cn

JS:   s === [...s].reverse().join("")
来源：http://ggv.zdqjudy.top

TS:   s === [...s].reverse().join("")
来源：http://uey.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://szg.yuxming.cn

Go:   // 双指针从两端比较
来源：http://qad.xuanzx.com

Ruby: s == s.reverse
来源：http://chw.yvedp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jqv.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://gmp.zhijiandao.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cab.9152youxi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dyc.yj202588.top

JS:   // 手写 Map：map.set(v, i)
来源：http://lvq.jqgufenzy.top

TS:   // 手写 Map<string, number>
来源：http://kny.xziqi.cn

Java: // 手写 HashMap
来源：http://wul.yonumen.top

Go:   // 手写 map[int]int
来源：http://lpe.cashguo.top

Ruby: // 手写 Hash
来源：http://bat.xziqi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://omb.mhx1999.top

[N08] 生成全排列
来源：http://fhs.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://yxf.cdnleiting.top

PHP:  // 手写递归交换
来源：http://bzr.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://gwe.iojbl.cn

TS:   // 手写回溯递归
来源：http://jdl.gaohongyu789.top

Java: // 手写回溯递归
来源：http://wmd.zdbjq.cn

Go:   // 手写回溯递归
来源：http://zup.birdmap.top

Ruby: arr.permutation.to_a
来源：http://clu.c1oappe.top

C#:   // 手写回溯递归
来源：http://pgg.snrcjt.cn

[N09] 栈与队列
来源：http://yaw.shuidangran.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tiv.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ygz.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vyo.fzhhl.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jnm.snrcjt.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://umm.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aou.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://slh.zycfv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ona.fengsongda.top

[N10] 链表节点定义
来源：http://rwo.pycfn.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fbq.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xzn.yj202588.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bjd.ydjk.org.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oab.vehdjk.com

Java: class Node { int v; Node next; }
来源：http://pcr.guannengcc.top

Go:   type Node struct { V int; Next *Node }
来源：http://yoa.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://myf.nanxinkj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wae.guannengcc.top

[N11] 二叉树中序遍历
来源：http://sro.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qyk.cashguo.top

PHP:  // 手写递归函数
来源：http://rur.chenzaomai.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dlm.jianghu66.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gvp.gogol.net.cn

Java: // 手写递归
来源：http://duo.sufxvd.cn

Go:   // 手写递归
来源：http://plh.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gsy.wangdashe.top

C#:   // 手写递归
来源：http://xew.meibo888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://twh.xziqi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lie.jyoumei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://edy.kuanghao11.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dva.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ysq.yangfankeji.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://snt.0kj1m.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cem.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ynv.jqgufenzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fdr.zycfv.cn

================================================================================
来源：http://gms.cucudq.cn

O. 并发与异步
来源：http://ean.316326.xyz

================================================================================
来源：http://und.yj20258888.top

[O01] 启动一个线程
来源：http://zeg.ivvv.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fkn.daxiang520.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://llp.zhiwuduotai.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sbl.bbcook.cn

TS:   // 同 JS
来源：http://zge.fehbvm.com

Java: new Thread(() -> f()).start()
来源：http://dry.redwolf501.top

Go:   go f()
来源：http://pay.sysykeji.top

Ruby: Thread.new { f }
来源：http://mct.vehdjk.com

C#:   Task.Run(() => F());
来源：http://hkr.chenjidiqi.icu

[O02] 使用线程池
来源：http://yzz.zdqjudy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vnk.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ubx.zdbjq.cn

JS:   // worker_threads 线程池
来源：http://xlr.hesvh.cn

TS:   // worker_threads 线程池
来源：http://vhm.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://mgv.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zvw.aibaodan.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mwn.gogol.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uks.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://shv.ehwqpu.com

Py:   with lock: shared += 1
来源：http://deo.iojbl.cn

PHP:  // 用 flock() 做文件锁
来源：http://ieu.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zxr.jianghu66.top

TS:   // 同 JS
来源：http://lhe.tianlin.xyz

Java: synchronized (this) { shared++; }
来源：http://bnh.yongpay.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dcc.ivvv.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pfy.hnxiangtu.top

C#:   lock (gate) { shared++; }
来源：http://sep.xuanzx.com

[O04] 定义异步函数并等待
来源：http://wuy.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://mlo.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gcn.epnwcf.com

JS:   async function f() { await g(); }
来源：http://hui.ydzc1.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ywp.zycfv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bli.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fga.guannengcc.top

Ruby: # 用 Fiber 或 async gem
来源：http://cka.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://tch.yuanzhike.top

[O05] 并发执行并等待全部完成
来源：http://soo.tian-w.cn

Py:   asyncio.gather(*tasks)
来源：http://hur.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ykr.yj20258888.top

JS:   await Promise.all(tasks)
来源：http://dqe.zdbjq.cn

TS:   await Promise.all(tasks)
来源：http://son.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jhk.pycfn.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oom.hongshengwenyu.top

Ruby: threads.map(&:join)
来源：http://jve.bbcook.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ryr.jinqigfzy.top

[O06] 使用进程池
来源：http://tke.mhx1999.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://giu.fanxiaobao.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://dfs.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://enz.chenjidiqi.icu

TS:   // child_process / cluster 模块
来源：http://gmc.zhoulong.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pas.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vqt.fehbvm.com

Ruby: // fork 块
来源：http://jex.jinqigfzy.top

C#:   Parallel.For
来源：http://nxt.bjfxy.top

================================================================================
来源：http://ceu.gzhubu.top

P. 常用工具函数
来源：http://waf.cheryme.top

================================================================================
来源：http://dil.uphjek.com

[P01] 生成 UUID
来源：http://bnd.yj20258.top

Py:   str(uuid.uuid4())
来源：http://olw.iojbl.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ggq.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://bqx.vehdjk.com

TS:   crypto.randomUUID()
来源：http://ycw.tarul.cn

Java: UUID.randomUUID().toString()
来源：http://pqe.iojbl.cn

Go:   // 用 github.com/google/uuid
来源：http://qlx.hywenlv.cn

Ruby: SecureRandom.uuid
来源：http://cmf.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://voz.xuanzx.com

[P02] MD5 / SHA256 摘要
来源：http://ouj.aibaodan.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pvs.yonumen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://elb.haohaochexian.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dbu.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zzz.shangyingyoupin.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hoa.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nic.hongshengwenyu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wil.yongpay.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vms.xylfe.cn

[P03] 生成短随机字符串
来源：http://iyi.gogol.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baj.ywan-chungtsiang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cmq.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dsw.guannengcc.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qhx.hfpthk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xrd.shzxlz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rsl.yfazqb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://tqm.ehwqpu.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mgb.ydzc1.top

[P04] 求长度
来源：http://glw.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oxd.52xcode.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tpy.guowangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ptb.bbcook.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uwa.sysykeji.top

Java: list.size();  map.size();  s.length()
来源：http://lfp.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://lok.daria6918.cn

Ruby: x.length;  x.size
来源：http://xqk.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://iud.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://aws.ivvv.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jpj.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ywx.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bmb.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://adm.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wgu.cheryme.top

Go:   reflect.DeepEqual(a, b)
来源：http://iod.tian-w.cn

Ruby: a == b
来源：http://kvp.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hnt.zhengqikj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://shf.guannengcc.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mbu.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://rci.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wmb.daria6918.cn

TS:   if (x == null) {}
来源：http://qgp.zhijiandao.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kgk.daxiang520.top

Go:   if x == nil {}
来源：http://nao.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mic.jianghu66.top

C#:   if (x is null) {}
来源：http://rzg.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://qpg.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ioy.aizwys.cn

PHP:  // 手写时间戳比较
来源：http://jkn.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bon.xylfe.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aio.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vjw.yangfankeji.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://olx.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://odr.yfazqb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ixn.gaohongyu789.top

[P08] 处理浮点精度问题
来源：http://gzf.nwbrower.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wvc.tarul.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cri.316326.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gaj.hesvh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gbm.guannengcc.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mmp.shanyushiyangtech.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lcg.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iyo.shanyushiyangtech.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://saq.kuanghao11.cn

================================================================================
来源：http://bxy.hywenlv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sko.aizwys.cn

================================================================================
来源：http://qtp.chenzaomai.com

[Q01] 创建表
来源：http://lrd.sjlbkw.cn

CREATE TABLE users (
来源：http://qlo.9152youxi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mdj.andypj.xyz

name VARCHAR(50) NOT NULL,
来源：http://kbt.fengsongda.top

email VARCHAR(100) UNIQUE,
来源：http://kyz.haohaochexian.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pcn.shangyingyoupin.top

);
来源：http://pwg.feifeiyinyue.top

[Q02] 创建带外键的表
来源：http://kvw.guannengcc.top

CREATE TABLE orders (
来源：http://qwy.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hyo.cucudq.cn

user_id INT NOT NULL,
来源：http://zpn.zhengqikj.top

amount DECIMAL(10, 2),
来源：http://aed.redwolf501.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://klz.zdbjq.cn

);
来源：http://lcl.xingfuxueyuan.xyz

[Q03] 增加列
来源：http://mvf.shanyushiyangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://noz.redwolf501.top

[Q04] 修改列类型
来源：http://rro.uphjek.com


<!-- 参考信息 -->