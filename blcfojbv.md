代发 wailian999

Ruby: exit 1
来源：http://cec.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cem.zdbjq.cn

[M06] 向标准错误输出
来源：http://lrl.zdqjudy.top

Py:   print("err", file=sys.stderr)
来源：http://gda.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ksm.yueranfly.top

JS:   console.error("err")
来源：http://iew.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://bqz.chenzaomai.com

Java: System.err.println("err")
来源：http://iai.daxiang520.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://afs.gzhubu.top

Ruby: warn "err"
来源：http://exy.guannengcc.top

C#:   Console.Error.WriteLine("err")
来源：http://lko.birdmap.top

[M07] 判断是否为主入口
来源：http://epx.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://ydx.dianchejie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tav.jinghuilouyu.cn

JS:   require.main === module
来源：http://ilb.shanyushiyangkeji.top

TS:   require.main === module
来源：http://ehf.0kj1m.cn

Java: public static void main(String[] args)
来源：http://wrr.jinqigufen.top

Go:   func main()
来源：http://awj.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cxx.fktsv.cn

C#:   static void Main(string[] args)
来源：http://dcr.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://fey.ctjpmb.com

Py:   platform.system();  platform.python_version()
来源：http://iuv.svipenyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://jlr.dashuyun.cn

JS:   process.platform;  process.version
来源：http://wiq.9152youxi.cn

TS:   process.platform;  process.version
来源：http://kji.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jbl.yangfankeji.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://evd.bbcook.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cdf.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hgc.daxiang520.top

================================================================================
来源：http://cdk.dianchejie.cn

N. 数据结构与算法
来源：http://slw.gaohongyu789.top

================================================================================
来源：http://mjg.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://nsx.gotoacloud.top

Py:   bisect.bisect_left(arr, x)
来源：http://vdg.jqgfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uvo.fzhhl.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pgx.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pbq.haohaochexian.top

Java: Arrays.binarySearch(arr, x)
来源：http://yiy.svipenyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://zoh.zhijiandao.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ivd.guowangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://imi.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://iio.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://urp.aizwys.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hui.cucudq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rtk.fktsv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rra.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ocz.hcnkem.com

Go:   slices.Sort(arr)
来源：http://iki.fengsongda.top

Ruby: arr.sort
来源：http://fsw.snrcjt.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xom.guowangkeji.top

[N03] 快速排序（分治示例）
来源：http://jfx.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tyx.shangyingyoupin.top

PHP:  // 递归实现，或用 usort
来源：http://nth.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wor.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://anb.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rjp.xingfuxueyuan.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mzm.hysaishi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ush.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hcv.haohaochexian.top

[N04] 斐波那契数列
来源：http://rje.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pqk.zhiwuduotai.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rrp.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ydq.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jrf.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://czb.zhixingplan.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ytj.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mou.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wff.chenlongwang.top

[N05] 最大公约数
来源：http://txz.fktsv.cn

Py:   math.gcd(a, b)
来源：http://drj.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dtn.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qoc.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vum.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vws.zdqjudy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xjy.shanyushiyangtech.top

Ruby: a.gcd(b)
来源：http://hyi.daxiang520.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kel.fehbvm.com

[N06] 判断回文字符串
来源：http://gws.feifeiyinyue.top

Py:   s == s[::-1]
来源：http://yas.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://lnr.gzhubu.top

JS:   s === [...s].reverse().join("")
来源：http://bxe.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://wlu.ctjpmb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bju.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://cdl.9152youxi.cn

Ruby: s == s.reverse
来源：http://yxq.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nvw.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://unw.jlsjyb.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lif.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nly.shuidangran.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kfh.zdqjudy.top

TS:   // 手写 Map<string, number>
来源：http://asm.hnxiangtu.top

Java: // 手写 HashMap
来源：http://bkq.meibo888.top

Go:   // 手写 map[int]int
来源：http://gyy.xuanzx.com

Ruby: // 手写 Hash
来源：http://pmu.birdmap.top

C#:   // 手写 Dictionary<int, int>
来源：http://hht.cdnleiting.top

[N08] 生成全排列
来源：http://cye.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://wjp.xingfuxueyuan.xyz

PHP:  // 手写递归交换
来源：http://iir.zhixingplan.top

JS:   // 手写回溯递归
来源：http://nlj.fktsv.cn

TS:   // 手写回溯递归
来源：http://chy.jyoumei.cn

Java: // 手写回溯递归
来源：http://qtx.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://zis.jinqigfzy.top

Ruby: arr.permutation.to_a
来源：http://jvy.sjlbkw.cn

C#:   // 手写回溯递归
来源：http://hwz.yuxming.cn

[N09] 栈与队列
来源：http://xdx.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ovw.jqgufenzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dtq.sysykeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wde.pengpengdd.cyou

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ghd.daxiang520.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://muz.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kks.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cyl.wangdashe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yuo.316326.xyz

[N10] 链表节点定义
来源：http://cvm.9152youxi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uwl.ctjpmb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://lgx.xuanzx.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rdw.snrcjt.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://evr.shanyushiyangkeji.top

Java: class Node { int v; Node next; }
来源：http://gdm.zhongyouzk.top

Go:   type Node struct { V int; Next *Node }
来源：http://nzb.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zda.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vcv.ywan-chungtsiang.top

[N11] 二叉树中序遍历
来源：http://gjr.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://txl.mhx1999.top

PHP:  // 手写递归函数
来源：http://gkv.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ees.hfpthk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xdz.zhengqikj.top

Java: // 手写递归
来源：http://alw.jinyuanbaomall.cn

Go:   // 手写递归
来源：http://tjy.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vdr.jyoumei.cn

C#:   // 手写递归
来源：http://pnt.gzhubu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lyr.hammf.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sqc.dianchejie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ipn.xuetiantiany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://itm.yonumen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fur.shanyushiyangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wjw.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xmz.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://goq.tarul.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://izf.ydzc1.top

================================================================================
来源：http://atl.hfpthk.cn

O. 并发与异步
来源：http://lsv.aibaodan.cn

================================================================================
来源：http://dox.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://fai.jinqigfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qcj.shangyingyoupin.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fpn.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gtk.hcnkem.com

TS:   // 同 JS
来源：http://drx.ivvv.top

Java: new Thread(() -> f()).start()
来源：http://ygp.cqqwz.cn

Go:   go f()
来源：http://tma.svipenyu.cn

Ruby: Thread.new { f }
来源：http://nsa.pycfn.com

C#:   Task.Run(() => F());
来源：http://clf.shanyushiyangkeji.top

[O02] 使用线程池
来源：http://myn.pengpengdd.cyou

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ebe.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yfz.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://edm.feifeiyinyue.top

TS:   // worker_threads 线程池
来源：http://ife.chenjidiqi.icu

Java: Executors.newFixedThreadPool(4)
来源：http://zsp.yj202588.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gqa.snrcjt.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uue.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tam.gaohongyu789.top

[O03] 加锁保护共享数据
来源：http://xge.fktsv.cn

Py:   with lock: shared += 1
来源：http://wgq.daxiang520.top

PHP:  // 用 flock() 做文件锁
来源：http://lhr.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hlx.bjfxy.top

TS:   // 同 JS
来源：http://yfd.hongshengwenyu.top

Java: synchronized (this) { shared++; }
来源：http://pqn.haohaochexian.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://skl.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dak.meibo888.top

C#:   lock (gate) { shared++; }
来源：http://fow.hesvh.cn

[O04] 定义异步函数并等待
来源：http://uyf.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://xfa.hcnkem.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dby.zycfv.cn

JS:   async function f() { await g(); }
来源：http://jma.cucudq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://udd.bbcook.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yyh.zdbjq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tyh.vqdsnc.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pjk.smart0.xyz

C#:   async Task F() { await G(); }
来源：http://rvl.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://plp.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://wex.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jdg.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://boy.tanke756.top

TS:   await Promise.all(tasks)
来源：http://inj.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rnh.smart0.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ujv.redwolf501.top

Ruby: threads.map(&:join)
来源：http://wen.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bkl.zdqjudy.top

[O06] 使用进程池
来源：http://ynq.aizwys.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://thu.fengsongda.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nhu.ppjwa.cn

JS:   // child_process / cluster 模块
来源：http://tfm.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://zop.fzhhl.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oyu.redwolf501.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://srv.xuanzx.com

Ruby: // fork 块
来源：http://anz.gaohongyu789.top

C#:   Parallel.For
来源：http://djj.fanxiaobao.xyz

================================================================================
来源：http://szu.daxiang520.top

P. 常用工具函数
来源：http://bqe.feifeiyinyue.top

================================================================================
来源：http://nhw.xziqi.cn

[P01] 生成 UUID
来源：http://mxz.zhiwuduotai.top

Py:   str(uuid.uuid4())
来源：http://pdl.chenlongwang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wyf.nanxuanxn.top

JS:   crypto.randomUUID()
来源：http://apd.hcnkem.com

TS:   crypto.randomUUID()
来源：http://ymi.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://wzx.birdmap.top

Go:   // 用 github.com/google/uuid
来源：http://niv.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://bsp.shuidangran.top

C#:   Guid.NewGuid().ToString()
来源：http://igz.epnwcf.com

[P02] MD5 / SHA256 摘要
来源：http://iwa.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ivf.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sia.mhx1999.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dpy.hysaishi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rtk.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cwp.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zjo.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tpq.xuetiantiany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xte.ctjpmb.com

[P03] 生成短随机字符串
来源：http://ost.kuanghao11.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iaz.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pnk.haohaochexian.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ifl.xuetiantiany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dch.wangshuangyany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uwt.hnqzz.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tuj.xinyue.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://kov.jlsjyb.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cwp.yonumen.top

[P04] 求长度
来源：http://vfn.shanyushiyangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://toh.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vev.yfazqb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lrf.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mkj.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://iwo.sweek.top

Go:   len(arr);  len(m)
来源：http://tfu.ctjpmb.com

Ruby: x.length;  x.size
来源：http://bla.yueranfly.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://emo.hywenlv.cn

[P05] 判断两个对象内容是否相等
来源：http://qpa.zycfv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://edw.xuanzx.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zhb.chenzaomai.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dev.xingfuxueyuan.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qqk.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://szc.316326.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://qhc.jianghu66.top

Ruby: a == b
来源：http://xvn.yuanzhike.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cge.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ytn.jinyuanbaomall.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uel.epnwcf.com

PHP:  if (empty($x)) {}
来源：http://ozm.xziqi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tag.gaohongyu789.top

TS:   if (x == null) {}
来源：http://izw.aibaodan.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gpi.daria6918.cn

Go:   if x == nil {}
来源：http://jja.havefunace.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nbw.birdmap.top

C#:   if (x is null) {}
来源：http://esy.gzhubu.top

[P07] 防抖与节流
来源：http://kgc.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ovl.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://oii.yj202588.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ifi.cheryme.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zmh.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uws.hongshengwenyu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://phx.yj202588.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mmg.sxryk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bbi.birdmap.top

[P08] 处理浮点精度问题
来源：http://jfk.0kj1m.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cdd.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ovo.nwbrower.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://apd.ivvv.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lzg.kuanghao11.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cua.nwbrower.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://byl.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://faq.zhijiandao.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://was.tanke756.top

================================================================================
来源：http://gch.dianchejie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gql.hywenlv.cn

================================================================================
来源：http://csh.chenlongwang.top

[Q01] 创建表
来源：http://dhw.yanxiufei.cn

CREATE TABLE users (
来源：http://fvr.redwolf501.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lqz.gzhubu.top

name VARCHAR(50) NOT NULL,
来源：http://usx.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://tii.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://byk.fktsv.cn

);
来源：http://nwz.gogol.net.cn

[Q02] 创建带外键的表
来源：http://zob.andypj.xyz

CREATE TABLE orders (
来源：http://ygo.cucudq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://svm.zhixingplan.top

user_id INT NOT NULL,
来源：http://wua.jinqigufen.top

amount DECIMAL(10, 2),
来源：http://vdj.zhoulong.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fdf.guannengcc.top

);
来源：http://moc.jiagoushi.top

[Q03] 增加列
来源：http://zgu.sweek.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fge.bjfxy.top

[Q04] 修改列类型
来源：http://qip.chenjidiqi.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uyu.smart0.xyz

[Q05] 重命名列
来源：http://hiq.jinyuanbaomall.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lny.zdqjudy.top

[Q06] 删除列
来源：http://qkr.hnqzz.top

ALTER TABLE users DROP COLUMN age;
来源：http://uou.shzxlz.cn

[Q07] 删除表
来源：http://nuz.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://zni.mhx1999.top

[Q08] 创建普通索引
来源：http://ifw.c1oappe.top


<!-- 参考信息 -->